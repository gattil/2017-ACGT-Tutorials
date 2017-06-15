---
title: Pipelines
permalink: /docs/pipelines_1/
redirect_from: /index.html
---

##### Building Pipelines

Automatize phylogenetic reconstruction and positive selection analyses for a group of files within a folder

1. MSA alignment is inferred with PRANK 151112
2. Fasta2Phylip is a software to convert fasta files into phylip files. https://indra.mullins.microbiol.washington.edu/perlscript/docs/Sequence.html
3. Phylogentic tree recostruction is performed applying GTR + Gamma
4. CodeML control file (Ctl) preparation
5. CodeML execution



```bash
#!/bin/bash

DIR=/Users/lorenzogatti/Desktop/expipelines
FILES=${DIR}/*.fasta

for f in $FILES
do
  echo "Processing $f file..."
  # take action on each file. $f store current file name

  #0. Get filename
  filename=$(basename $f)

  # 1. MSA alignment
  #muscle -in $f -out ${f}.aln
  #prank -d=$f -o=${f}.aln -codon -F -f=phylip
  prank -d=$f -o=${f}.aln -codon -F

  # 2. Covert fasta file in Phylip format
  Fasta2Phylip.pl ${f}.aln.best.fas ${DIR}/${filename}.aln.best.phy

  # 3. Tree reconstruction
  phyml -i ${DIR}/${filename}.aln.best.phy -m 'GTR' -t 'e' -a 'e' -f 'm'

  # 4. Prepare control file codeml
  cp ${DIR}/codeml_template.txt ${DIR}/codeml_${filename}.ctl
  echo "seqfile = ${DIR}/${filename}.aln.best.phy" >> ${DIR}/codeml_${filename}.ctl
  echo "treefile = ${DIR}/${filename}.phy_phyml_tree.txt" >> ${DIR}/codeml_${filename}.ctl
  echo "outfile = ${DIR}/${filename}_fr.txt" >> ${DIR}/codeml_${filename}.ctl

  # 5. Execute codeml
  codeml ${DIR}/codeml_${filename}.ctl
done


```

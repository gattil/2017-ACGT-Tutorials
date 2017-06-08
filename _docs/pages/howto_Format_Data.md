---
title: Data formats in bioinformatics
permalink: /docs/howto_Format_Data/
redirect_from: /index.html
---


### Sequence and (Multi) Sequence Alignment formats

#### Fasta

#### Phylip

---

### Tree formats

#### Newick  

The Newick tree format (or Newick notation or New Hampshire tree format) is a way of representing graph trees with edge lengths using parentheses and commas. It is a standard for representing trees in computer-readable form makes use of the correspondence between trees and nested parentheses, noticed in 1857 by the famous English mathematician Arthur Cayley. If we have this rooted tree:

<center><img src="../../img/intro_tree_example.png" alt="" title="" width="75%"></center>

then in the tree file it is represented by the following sequence of printable characters:

    (B,(A,C,E),D);

Branch lengths can be incorporated into a tree by putting a real number, with or without decimal point, after a node and preceded by a colon. This represents the length of the branch immediately below that node. Thus the above tree might have lengths represented as:

    (B:6.0,(A:5.0,C:3.0,E:4.0):5.0,D:11.0);

#### PhyloXML

PhyloXML is an XML language for the analysis, exchange, and storage of phylogenetic trees (or networks) and associated data. The structure of phyloXML is described by XML Schema Definition (XSD) language.

```xml
<phyloxml xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xsi:schemaLocation="http://www.phyloxml.org http://www.phyloxml.org/1.10/phyloxml.xsd"
xmlns="http://www.phyloxml.org">
<phylogeny rooted="true">
 <name>example from Prof. Joe Felsenstein's book "Inferring Phylogenies"</name>
 <description>MrBayes based on MAFFT alignment</description>
 <clade>
    <clade branch_length="0.06">
       <confidence type="probability">0.88</confidence>
       <clade branch_length="0.102">
          <name>A</name>
       </clade>
       <clade branch_length="0.23">
          <name>B</name>
       </clade>
    </clade>
    <clade branch_length="0.4">
       <name>C</name>
    </clade>
 </clade>
</phylogeny>
</phyloxml>
```
[More informations](https://en.wikipedia.org/wiki/PhyloXML)


---
### Multi purpose file formats

#### Nexux

The NEXUS file format (usually .nex or .nxs) is widely used in bioinformatics. Several popular phylogenetic programs such as PAUP*, MrBayes, Mesquite, MacClade and SplitsTree use this format.

```text
#NEXUS
Begin data;
Dimensions ntax=4 nchar=15;
Format datatype=dna missing=? gap=-;
Matrix
A   atgctagctagctcg
B   atgcta??tag-tag
C   atgttagctag-tgg
D   atgttagctag-tag           
;
End;

Begin Taxa;
  Taxalabels A B C D;
End;

Begin Trees;
  Tree tree1 = ((A,B),(C,D));
End;

```

---

1. http://evolution.genetics.washington.edu/phylip/newicktree.html
2. https://en.wikipedia.org/wiki/Nexus_file
3. https://en.wikipedia.org/wiki/PhyloXML

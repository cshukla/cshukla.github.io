---
layout: template1
title: Software
---

<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-111431367-3"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-111431367-3');
</script>

Much of my research leverages a recent genomic technique called massively parallel reporter assays (MPRAs). Since the early days of molecular biology, scientists have used reporter assays for different applications including studying the regulation of gene expression. While conventionally, one regulatory element is assayed at a given time, recent breakthroughs in microarray based nucleotide synthesis and next generation sequencing have allowed scientists to test several thousand elements in a single massively parallel reporter assay (MPRA). 

MPRA's were first demonstrated in [Patwardhan R.P. *et al.* (2009)](http://www.nature.com/nbt/journal/v27/n12/abs/nbt.1589.html) and [Melnikov A. *et al.* (2012)](http://www.nature.com/nbt/journal/v30/n3/full/nbt.2137.html) and the underlying technology has only become stronger and more robust in the following years. Recently, there has been a flurry of papers which have used MPRA's to test potential enhancer elements, eQTL's, SNP's as well as repressive elements - [Ulirsch J.C. *et al.* (2016)](http://www.cell.com/cell/fulltext/S0092-8674(16)30493-7), [Tewhey R. *et al* (2016)](http://www.cell.com/cell/fulltext/S0092-8674(16)30421-4), [Ernst J. *et al.* (2016)](http://www.nature.com/nbt/journal/v34/n11/full/nbt.3678.html). Although many "games" are being played by clever scientists to deduce regulatory elements using MPRAs, currently there is no dedicated software for analyzing MPRAs - which often have constraints a bit different from other *-Seq technologies. 

To solve this problem, we developed software to help with all computational aspects of MPRAs. We begin with a function to design the oligo pool and carry forward to mapping, normalizing, modeling and infering regulatory sequences from the input regions. We end by implementing a simple machine learning approach to discover k-mers enriched in the infered regulatory sequences. All the functionalities are provided in an easy to use R package. Since the publication is not yet out, the GitHub repo is private. However, if you want access to it, please [contact me](mailto:cshukla@g.harvard.edu).

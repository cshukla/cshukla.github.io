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

#### Oligo Games (MPRNA)

In the post-genomic era, thousands of putative noncoding regulatory regions have been identified, such as enhancers, promoters, long noncoding RNAs (lncRNAs) and a cadre of small peptides. These ever-growing catalogs require high-throughput assays to test their functionality at scale. Massively parallel reporter assays have greatly enhanced the understanding of noncoding DNA elements en masse. I have developed a massively parallel RNA assay (MPRNA) that can assay 10,000 or more RNA segments for RNA-based functionality. I also developed software to help with all computational aspects of MPRNA - designing the oligo pool, mapping sequencing reads, normalizing the MPRNA data, modeling it appropriately and infering regulatory sequences from the input regions. We have also implemented a simple machine learning approach to discover k-mers enriched in the inferred regulatory sequences. All the functionalities are provided in an easy to use [R package hosted on GitHub](https://github.com/cshukla/oligoGames){:target="_blank"}.

We applied MPRNA to identify RNA-based nuclear localization domains harbored in lncRNAs. We examined a pool of 11,969 oligos densely tiling 38 human lncRNAs that were fused to a cytosolic transcript. After cell fractionation and barcode sequencing, we identified 109 unique RNA regions that significantly enriched this cytosolic transcript in the nucleus including a cytosine-rich motif. These nuclear enrichment sequences are highly conserved and over-represented in global nuclear fractionation sequencing. Importantly, many of these regions were independently validated by single molecule RNA fluorescence in situ hybridization. Overall, we demonstrate the utility of MPRNA for future investigation of RNA-based functionalities. 

<center><img src="https://github.com/cshukla/cshukla.github.io/blob/master/assets/img/oligoGames.synopsis.jp2?raw=true" style="width:500px;height:362px;"></center>

#### Local Repeats

More than half the human and mouse genomes are comprised of repetitive sequences, such as transposable elements (TEs), which have been implicated in many biological processes. In contrast, much less is known about other repeats, such as local repeats that occur in multiple instances within a given locus in the genome but not elsewhere. I began by systematically characterize local repeats in the genomic locus of the Firre long noncoding RNA (lncRNA). We found a conserved function for the RRD repeat as a ribonucleic nuclear retention signal that is sufficient to retain an otherwise cytoplasmic mRNA in the nucleus. We also identified a repeat, termed R0, that can function as a DNA enhancer element within the intronic sequences of Firre. Collectively, our data suggests that local repeats can have diverse functionalities and molecular modalities in the Firre locus and perhaps more globally in other lncRNAs. The scripts for analyzing Local Repeats can be found [here](https://github.com/cshukla/Local-Repeats){:target="_blank"}.

<center><img src="https://github.com/cshukla/cshukla.github.io/blob/master/assets/img/firreRepeatsSmall.jp2?raw=true" style="width:500px;height:383px;"></center>
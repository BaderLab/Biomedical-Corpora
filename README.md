# Biomedical Corpora

A collection of annotated, freely distributable, biomedical corpora, which can be used for training supervised machine learning methods for various tasks in biomedical text-mining and information extraction.

All corpora are provided in `corpora`. They are divided into subdirectories `NER`, for corpora which can be used to train **named entity recognition** (NER) solutions, and `Relation Extraction`, for corpora which can be used to train **relation/event extraction** solutions. Corpora are provided in both a CoNLL-like format and a [Standoff](http://brat.nlplab.org/standoff.html) format.

Most corpora in the CoNLL-like format were originally collected [here](https://github.com/cambridgeltl/MTL-Bioinformatics-2016). In many cases, the tags were mapped to 4-letter codes:

| Old tag  | New tag |
| ------------- | ------------- |
| `Chemical`, `Simple_chemical`  | `CHED`  |
| `Disease` | `DISO`  |
| `Organism`, `Species`, `NCBITaxon`, `Taxon`  | `LIVB`  |
| `Cellular_component` | `COMP`  |
| `Cell`, `cell_type`  | `CLTP`  |
| `cell_line` | `CLLN`  |
| `Gene`, `Protein`, `Gene_or_gene_product`, `GGP`  | `PRGE`  |

> Mappings were largely inspired by this [API](http://bioinformatics.ua.pt/becas/#!/api).

Corpora names (loosely) follow the naming scheme: `<corpus_name>_<entity>_<tagset>`.

## Download

To download the corpora, simply clone the repository locally:

```bash
$ git clone https://github.com/BaderLab/Biomedical-Corpora.git
```

Or click the green `Clone or download` button and select `Download ZIP`.

## Resources

https://github.com/spyysalo provides many useful repositories for working with these corpora. Many of the most popular corpora have their own repositories (e.g. [S800](https://github.com/spyysalo/s800), [NCBI-Disease](https://github.com/spyysalo/ncbi-disease)) which contain code for collecting the corpus from its original source and converting it into a format suitable for training a machine learning classifier (e.g. CoNLL or [Standoff](http://brat.nlplab.org/standoff.html)).

## Table of Corpora

A list of various biomedical corpora and their corresponsding publications:

| Corpora | Text Genre | Standard | Entities (Count) | Publication |
| --- | --- | --- | --- | --- |
| [AnatEM](http://nactem.ac.uk/anatomytagger/) | Scientific Article | Gold | 12 Anatomical entities | [link](https://academic.oup.com/bioinformatics/article/30/6/868/285282) |
| [AZDC](http://diego.asu.edu/downloads/AZDC_6-26-2009.txt) | Scientific Article | Gold | Disease | [link](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=FLnUx4cAAAAJ&citation_for_view=FLnUx4cAAAAJ:ufrVoPGSRksC) |
| [BioCreative II GM](https://sourceforge.net/projects/biocreative/files/biocreative2entitytagging/1.1/) | Scientific Article | Gold | Genes/proteins (24,583) | [link](https://doi.org/10.1186/gb-2008-9-s2-s2) |
| [BioInfer](http://mars.cs.utu.fi/BioInfer/?q=download) | Scientific Article | Gold | Genes/proteins | [link](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-8-50) |
| [BioSemantics](https://biosemantics.org/index.php/resources/chemical-patent-corpus) | Patent | Gold | Chemicals, Disease | [link](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0107477) |
| BC4CHEMD | Scientific Article | Gold | Chemicals (84,310) | [link](https://www.ncbi.nlm.nih.gov/pubmed/25810766) |
| [BC5CDR](http://www.biocreative.org/tasks/biocreative-v/track-3-cdr/) | Scientific Article | Gold | Chemicals (15,935), Disease (12,852) | [link](academic.oup.com/database/article/doi/10.1093/database/baw068/2630414) |
| BioNLP09 | Scientific Article | Gold | Genes/proteins (14,963) | [link](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-9-10) |
| BioNLP11EPI | Scientific Article | Gold | Genes/proteins (15,811) | [link](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-13-S11-S2) |
| BioNLP11ID | Scientific Article | Gold | Genes/proteins (6551), Organisms (3471), Chemicals (973), Regulon-operon (87) | [link](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-13-S11-S2) |
| BioNLP13GE | Scientific Article | Gold | Genes/proteins (12,057) | [link](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.380.5420) |
| BioNLP13PC | Scientific Article | Gold | Genes/proteins (10,891), Chemicals (2487), Complexes (1502), Cellular component (1013) | [link](http://www.aclweb.org/anthology/W/W13/W13-2009.pdf) |
| [CRAFT](https://github.com/UCDenver-ccp/CRAFT) | Scientific Article | Gold | Sequence Ontology (18,974), Gene/proteins (16,064), Taxonomy (6868), Chemicals of biological interest (6053), Cell lines (5495), GO-CC (4180) | [link](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-13-161)|
| [CellFinder](https://www.informatik.hu-berlin.de/de/forschung/gebiete/wbi/resources/cellfinder) | Scientific Article | Gold | Species, Gene/proteins, Cell type, Anatomy | [link](https://www.informatik.hu-berlin.de/de/forschung/gebiete/sar/wbi/research/publications/2012/lrec2012_corpus.pdf)|
|[CHEMDNER Patent](http://www.biocreative.org/tasks/biocreative-v/track-2-chemdner/)| Patent | Gold | Chemicals |[link](https://jcheminf.springeropen.com/articles/10.1186/1758-2946-7-S1-S2)|
|[DECA](http://www.nactem.ac.uk/deca/)| Scientific Article | Gold | Genes/proteins |[link](http://bioinformatics.oxfordjournals.org/content/26/5/661.abstract?keytype=ref&ijkey=6nc2iFEN0sYYYz1)|
|Ex-PTM| Scientific Article | Gold | Genes/proteins (4698) |[link](https://dl.acm.org/citation.cfm?id=2002920)|
|[FSU-PRGE](http://pubannotation.org/projects/FSU-PRGE)| Scientific Article | Gold | Genes/proteins|[link](http://aclweb.org/anthology/W/W10/W10-1838.pdf)|
|JNLPBA| Scientific Article | Gold | Genes/proteins (35,336), DNA (10,589), Cell type (8639), Cell line (4330), RNA (1069) | [link](https://dl.acm.org/citation.cfm?id=1567610)|
|[Linneaus](http://linnaeus.sourceforge.net/)| Scientific Article | Gold | Organisms (4263) | [link](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-11-85)|
|[LocText](https://www.tagtog.net/-corpora/loctext)| Scientific Article | Gold | Organisms, Genes/proteins | [link](http://bmcproc.biomedcentral.com/articles/10.1186/1753-6561-9-S5-A4)|
|[IEPA](http://corpora.informatik.hu-berlin.de/corpora/brat2bioc/iepa_bioc.xml.zip) | Scientific Article | Gold | Genes/proteins | [link](http://psb.stanford.edu/psb-online/proceedings/psb02/abstracts/p326.html) |
|[miRNA](http://www.scai.fraunhofer.de/mirna-corpora.html)| Scientific Article | Gold | Disease, Organisms, Genes/proteins | [link](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4602280/) |
|[NCBI disease](https://www.ncbi.nlm.nih.gov/CBBresearch/Dogan/DISEASE/)| Scientific Article | Gold | Disease (6881) |[link](http://www.sciencedirect.com/science/article/pii/S1532046413001974)|
|[S800](http://species.jensenlab.org/)| Scientific Article | Gold | Organisms (3708) |[link](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0065390)|
|[Variome](http://www.opennicta.com.au/home/health/variome)| Scientific Article | Gold | Disease, Organisms, Genes/proteins|[link](http://database.oxfordjournals.org/content/2013/bat019.abstract)|

> Note, some corpora included in this table are not included for download in this repository because they are not freely distributable.

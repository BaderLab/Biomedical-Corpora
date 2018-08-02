# Biomedical Corpora

A collection of annotated, freely distributable, biomedical corpora, which can be used for training supervised machine learning methods for various tasks in biomedical text-mining and information extraction.

All corpora are provided in `corpora`. They are divided into subdirectories `NER`, for corpora which can be used to train **named entity recognition** (NER) solutions, and `Event Extraction`, for corpora which can be used to train **relation/event extraction** solutions. Corpora are provided in both a CoNLL-like format and a Standoff format. 

Most corpora in the CoNLL-like format were originally collected [here](https://github.com/cambridgeltl/MTL-Bioinformatics-2016). In many cases, the tags were mapped to 4-letter codes:

| Old tag  | New tag |
| ------------- | ------------- |
| `Anatomy`  | `ANAT`  |
| `Chemical`, `Simple_chemical`  | `CHED`  |
| `Disease` | `DISO`  |
| `Organism`, `Species`, `NCBITaxon`, `Taxon`  | `LIVB`  |
| `Cellular_component` | `COMP`  |
| `Cell`, `cell_type`  | `CLTP`  |
| `cell_line` | `CLLN`  |
| `Gene`, `Protein`, `Gene_or_gene_product`, `GGP`  | `PRGE`  |

> Mappings were largely inspired by this [API](http://bioinformatics.ua.pt/becas/#!/api).

## Download

To download the corpora, simply clone the repository locally:

```bash
$ git clone https://github.com/BaderLab/Biomedical-Corpora.git
```

Or click the green `Clone or download` button and select `Download ZIP`.

## Table of Corpora

A list of various biomedical corpora and their corresponsding publications:

| Corpora | Text Genre | Standard | Entities | Publication |
| --- | --- | --- | --- | --- |
| [AZDC](http://diego.asu.edu/downloads/AZDC_6-26-2009.txt) | Scientific Article | Gold | disease | [link](https://scholar.google.com/citations?view_op=view_citation&hl=en&user=FLnUx4cAAAAJ&citation_for_view=FLnUx4cAAAAJ:ufrVoPGSRksC) |
| [BioCreative II GM](https://sourceforge.net/projects/biocreative/files/biocreative2entitytagging/1.1/) | Scientific Article | Gold | genes/proteins | [link](https://doi.org/10.1186/gb-2008-9-s2-s2) |
| [BioInfer](http://mars.cs.utu.fi/BioInfer/?q=download) | Scientific Article | Gold | genes/proteins | [link](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-8-50) |
| [BioSemantics](https://biosemantics.org/index.php/resources/chemical-patent-corpus) | Patent | Gold | chemicals, disease | [link](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0107477) |
| [CDR](http://www.biocreative.org/tasks/biocreative-v/track-3-cdr/) | Scientific Article | Gold | chemicals, diseases | [link](academic.oup.com/database/article/doi/10.1093/database/baw068/2630414) |
| [CellFinder](https://www.informatik.hu-berlin.de/de/forschung/gebiete/wbi/resources/cellfinder) | Scientific Article | Gold | species, gene/proteins, cells, anatomy | [link](https://www.informatik.hu-berlin.de/de/forschung/gebiete/sar/wbi/research/publications/2012/lrec2012_corpus.pdf)|
|[CHEMDNER Patent](http://www.biocreative.org/tasks/biocreative-v/track-2-chemdner/)| Patent | Gold | chemicals|[link](https://jcheminf.springeropen.com/articles/10.1186/1758-2946-7-S1-S2)|
|[DECA](http://www.nactem.ac.uk/deca/)| Scientific Article | Gold | gene/proteins |[link](http://bioinformatics.oxfordjournals.org/content/26/5/661.abstract?keytype=ref&ijkey=6nc2iFEN0sYYYz1)|
|[FSU-PRGE](http://pubannotation.org/projects/FSU-PRGE)| Scientific Article | Gold | genes/proteins|[link](http://aclweb.org/anthology/W/W10/W10-1838.pdf)|
|[Linneaus](http://linnaeus.sourceforge.net/)| Scientific Article | Gold | species | [link](http://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-11-85)|
|[LocText](https://www.tagtog.net/-corpora/loctext)| Scientific Article | Gold | species, genes/proteins | [link](http://bmcproc.biomedcentral.com/articles/10.1186/1753-6561-9-S5-A4)|
|[IEPA](http://corpora.informatik.hu-berlin.de/corpora/brat2bioc/iepa_bioc.xml.zip) | Scientific Article | Gold | genes/proteins | [link](http://psb.stanford.edu/psb-online/proceedings/psb02/abstracts/p326.html) |
|[miRNA](http://www.scai.fraunhofer.de/mirna-corpora.html)| Scientific Article | Gold | diseases, species, genes/proteins | [link](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4602280/) |
|[NCBI disease](https://www.ncbi.nlm.nih.gov/CBBresearch/Dogan/DISEASE/)| Scientific Article | Gold | diseases|[link](http://www.sciencedirect.com/science/article/pii/S1532046413001974)|
|[S800](http://species.jensenlab.org/)| Scientific Article | Gold | species|[link](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0065390)|
|[Variome](http://www.opennicta.com.au/home/health/variome)| Scientific Article | Gold | diseases, species, genes/proteins|[link](http://database.oxfordjournals.org/content/2013/bat019.abstract)|

> Note, some corpora included in this table are not included for download in this repository because they are not freely distributable.

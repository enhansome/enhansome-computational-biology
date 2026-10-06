# Awesome Computational Biology with stars

A curated collection of databases, software, and papers related to computational biology.

> Computational biology involves the development and application of data-analytical and theoretical methods, mathematical modelling and computational simulation techniques to the study of biological, ecological, behavioural, and social systems. — [Wikipedia](https://en.wikipedia.org/wiki/Computational_biology)

***

## Overview

[![Resource Landscape Overview](docs/overview.png)](https://inoue0426.github.io/awesome-computational-biology/overview.html)

> Interactive version: [Resource Overview page](https://inoue0426.github.io/awesome-computational-biology/overview.html)\
> Regenerate the figure: `python scripts/generate_overview.py`

***

## GitHub Pages UI

Browse and search the resources via the [GitHub Pages UI](https://inoue0426.github.io/awesome-computational-biology/).

For treatment-response work, the [Dataset Explorer](https://inoue0426.github.io/awesome-computational-biology/dataset-explorer.html) compares curated cell-line, patient, and PDX datasets by year, sample type, perturbation metadata, matched pre/post availability, SMILES coverage, and clinical outcomes.

The [Method Explorer](https://inoue0426.github.io/awesome-computational-biology/method-explorer.html) compares drug-response and perturbation methods by task, molecular/context representation, unseen-drug support, dose/time conditioning, and patient transfer.

The [Foundation Model Explorer](https://inoue0426.github.io/awesome-computational-biology/foundation-explorer.html) compares foundation models by fine-grained modality, parameter count, pretraining scale, species, zero-shot support, weights/code availability, perturbation support, and spatial support.

The [Agent Explorer](https://inoue0426.github.io/awesome-computational-biology/agent-explorer.html) compares agentic AI systems by scientific domain, single- vs multi-agent architecture, tool/code execution, literature and web retrieval, omics and wet-lab support, autonomy, and human-in-the-loop design. The Agent Explorer table is sortable and supports domain, architecture, omics, code-execution, and year filters.

All explorer tables support sortable columns and focused filters for quick comparison, including a Recent (≥2025) toggle.

The Pages home screen also summarizes total resources, profiled datasets, methods, foundation models, agents, and the most common foundation-model modalities.

Chemical and genetic perturbation datasets can be filtered separately in the Dataset Explorer. Genetic screens can also be filtered by CRISPRi, CRISPRa, knockout, enhancer-targeting, combinatorial, or mixed perturbation modes, including mixed-resource collections.

The explorer also includes the eight perturbation datasets used in the Bison unseen-compound benchmark.

* Search matches `name`, `description`, `tasks`, `modalities`, and `tags`.
* The **Task**, **Modality**, and **Type** filters map directly to `tasks`, `modalities`, and `type` in `docs/data/resources.json`.
* Clicking badges on cards applies the corresponding filter.

***

## Table of Contents

* [Awesome Computational Biology](#awesome-computational-biology-)
  * [Table of Contents](#table-of-contents)
  * [Overview](#overview)
  * [GitHub Pages UI](#github-pages-ui)
  * [Citation](#citation)
  * [Curation Criteria (Strict)](#curation-criteria-strict)
  * [Update & Link Rot Policy](#update--link-rot-policy)
  * [Data Schema & Contribution Workflow](#data-schema--contribution-workflow)
  * [Databases](#databases)
    * [scRNA](#scrna)
    * [Compound](#compound)
    * [Pathway](#pathway)
    * [Mass Spectra](#mass-spectra)
    * [Protein](#protein)
    * [Genome](#genome)
    * [Disease](#disease)
    * [Interaction](#interaction)
      * [Drug-Gene Interaction](#drug-gene-interaction)
      * [Drug (Cell Line) Response](#drug-cell-line-response)
      * [Chemical-Protein Interaction](#chemical-protein-interaction)
      * [Protein-Protein Interaction](#protein-protein-interaction)
      * [Knowledge Graph](#knowledge-graph)
      * [Gene Regulatory Network](#gene-regulatory-network)
    * [Clinical Trial](#clinical-trial)
  * [Benchmarks & Datasets](#benchmarks--datasets)
  * [API](#api)
  * [Preprocessing Tools](#preprocessing-tools)
  * [Machine Learning Tasks and Models](#machine-learning-tasks-and-models)
    * [Drug Discovery](#drug-discovery)
      * [Drug Response Prediction](#drug-response-prediction)
      * [Drug Perturbation](#drug-perturbation)
      * [Drug Repurposing](#drug-repurposing)
      * [Drug Target Interaction](#drug-target-interaction)
      * [Compound-Protein Interaction](#compound-protein-interaction)
      * [Molecular Generation](#molecular-generation)
    * [Protein Property Prediction](#protein-property-prediction)
    * [LLM for Biology](#llm-for-biology)
    * [Foundation Models](#foundation-models)
      * [Single-cell Foundation Models](#single-cell-foundation-models)
        * [Transcriptomics Foundation Models](#transcriptomics-foundation-models)
        * [Spatial Foundation Models](#spatial-foundation-models)
        * [Multi-Omics Foundation Models](#multi-omics-foundation-models)
        * [Domain Alignment](#domain-alignment)
      * [Compound Foundation Models](#compound-foundation-models)
        * [Compound Embedding](#compound-embedding)
      * [Protein Foundation Models](#protein-foundation-models)
        * [Pre-trained Embedding](#pre-trained-embedding)
        * [Protein Structure Prediction and Design](#protein-structure-prediction-and-design)
      * [Multi-Modal Foundation Models](#multi-modal-foundation-models)
      * [Genomics Foundation Models](#genomics-foundation-models)

***

## Databases

### scRNA

* [CZ CELLxGENE](https://cellxgene.cziscience.com/) — Single-cell dataset repository and interactive explorer from the Chan Zuckerberg Initiative.
* [Gene Expression Omnibus](https://www.ncbi.nlm.nih.gov/geo/) — Public functional genomics database.
* [Human Cell Atlas](https://www.humancellatlas.org/) — Open global atlas of all cells in the human body.
* [Single Cell PORTAL](https://singlecell.broadinstitute.org/single_cell) — Public database for single-cell RNA.
* [Single Cell Expression Atlas](https://www.ebi.ac.uk/gxa/sc/home) — Public database for single-cell RNA.

### Compound

* [PubChem](https://pubchem.ncbi.nlm.nih.gov/) — One of the largest chemical databases (compounds, genes, and proteins).
* [ChEBI](https://www.ebi.ac.uk/chebi/) — Database focused on small chemical compounds.
* [ChEMBL](https://www.ebi.ac.uk/chembl/) — Bioactive molecules with drug-like properties.
* [ChemSpider](http://www.chemspider.com/) — Chemical structure database.
* [DrugTargetCommons](https://drugtargetcommons.fimm.fi/) — Community platform for curating and integrating experimental bioactivity data across drugs and targets.
* [HMDB (Human Metabolome Database)](https://hmdb.ca/) — Comprehensive database of small molecule metabolites found in the human body.
* [KEGG COMPOUND](https://www.genome.jp/kegg/compound/) — Collection of small molecules and biopolymers.
* [LIPID MAPS](https://www.lipidmaps.org/databases/lmsd/overview) — Database of lipids.
* [Rhea](https://www.rhea-db.org/) — Database of chemical reactions.
* [DrugCentral](http://drugcentral.org/) — Online drug compendium with drug mode of action and indication information.
* [Drug Repurposing Hub](https://repo-hub.broadinstitute.org/repurposing#download-data) — Collections of drug repurposing data (drug, MoA, target, etc).
* [Therapeutic Target Database](https://idrblab.net/ttd/full-data-download) — Drug-target, target-disease, and drug-disease datasets.
* [ZINC ligand discovery database](https://zinc.docking.org/) — Free database of commercially-available compounds for virtual screening.

### Pathway

* [PathwayCommons](https://www.pathwaycommons.org/) — Database of pathways and interactions.
* [KEGG PATHWAY](https://www.genome.jp/kegg/pathway.html) — Collection of pathway maps.
* [WikiPathways](https://wikipathways.org/) — Database of biological pathways.
* [Reactome](https://reactome.org/) — Expert-curated, peer-reviewed pathway database with detailed reaction mechanisms.
* [BioCyc](https://biocyc.org/) — Collection of pathway/genome databases across thousands of organisms.
* [OmniPath](https://omnipathdb.org/) — Comprehensive resource integrating protein interactions, signaling pathways, gene regulatory networks, and miRNA targets from over 100 databases.
* [SIGNOR 2.0](https://signor.uniroma2.it/) — Database of causal signaling interactions and pathways, with signed and directed relationships between proteins.
* [MSigDB (Molecular Signatures Database)](https://www.gsea-msigdb.org/gsea/msigdb) — Curated gene sets derived from pathways and biological processes.

### Mass Spectra

* [MassBank](http://www.massbank.jp/) — Open source databases and tools for mass spectrometry reference spectra.
* [MoNA MassBank of North America](https://mona.fiehnlab.ucdavis.edu/) — Meta-database of metabolite mass spectra, metadata, and associated compounds.

### Protein

* [THE HUMAN PROTEIN ATLAS](https://www.proteinatlas.org/) — Comprehensive human protein database (cells, tissues, organs).
* [PROTEIN DATA BANK (PDB)](https://www.rcsb.org/) — 3D structures of proteins, nucleic acids, complexes.
* [UniProt](https://www.uniprot.org/) — Functional information on proteins.
* [AlphaFold Protein Structure Database](https://alphafold.ebi.ac.uk/api-docs) — 3D protein structure predictions.
* [RCSB Protein Data Bank](https://www.rcsb.org/) — Repository for structural data of biological molecules.
* [Critical Assessment of Structure Prediction (CASP)](https://predictioncenter.org/) — Assessing methods for protein structure prediction.
* [Uniclust](https://uniclust.mmseqs.com/) — Clustered protein sequence databases.
* [UniRef](https://www.uniprot.org/uniref/) — Non-redundant sequence database clustering UniProtKB entries at multiple sequence identity thresholds.
* [CATH database](https://www.cathdb.info/) — Hierarchical classification of protein domain structures.
* [SAbDab](https://opig.stats.ox.ac.uk/webapps/sabdab-sabpred/sabdab) — Structural Antibody Database containing all antibody structures in the PDB.
* [OADB (Observed Antibody Space Database)](http://opig.stats.ox.ac.uk/webapps/oas/) — Database of antibody sequences from immune repertoire sequencing.
* [InterPro](https://www.ebi.ac.uk/interpro/) — Protein families, domains, and functional sites database integrating 14 member databases including Pfam and PROSITE.
* [Pfam](https://www.ebi.ac.uk/interpro/entry/pfam/) — Database of protein families described by multiple sequence alignments and hidden Markov models.
* [NeXtProt](https://www.nextprot.org/) — Expert knowledge base on human proteins with deep functional annotation, complementary to UniProt.

### Genome

* [ENCODE](https://www.encodeproject.org/) — Encyclopedia of DNA Elements; regulatory and functional genomic elements across the genome.
* [Ensembl](https://www.ensembl.org/) — Genome browser and annotation database for vertebrate and other eukaryotic genomes.
* [Human Genome Resources at NCBI](https://www.ncbi.nlm.nih.gov/projects/genome/guide/human/index.shtml) — Database for genomics, proteomics, transcriptomics, and systems biology.
* [GenBank](https://www.ncbi.nlm.nih.gov/genbank/) — NCBI's database of genetic sequences.
* [UCSC Genome Browser](https://genome.ucsc.edu/) — UCSC's genome browser.
* [cBioPortal](https://www.cbioportal.org/) — Cancer genomics database; aggregating many patient datasets.
* [OncoKB](https://www.oncokb.org/) — Precision oncology knowledge base of cancer genes, variants, and therapeutic implications.
* [10x Genomics Dataset](https://www.10xgenomics.com/resources/datasets) — Collection of single-cell datasets.
* [The Genotype-Tissue Expression (GTEx)](https://gtexportal.org/home/) — Human gene expression and regulation resource.
* [Dependency Map (DepMap)](https://depmap.org/portal/) — CRISPR-Cas9 screens in cancer cell lines.
* [Catalogue Of Somatic Mutations In Cancer (COSMIC)](https://cancer.sanger.ac.uk/cosmic) — Resource on somatic mutations in cancers.
* [MGnify](https://www.ebi.ac.uk/metagenomics/) — Resource for metagenomic and metatranscriptomic data.
* [JASPAR](http://jaspar.genereg.net/) — Database of transcription factor binding profiles.
* [gnomAD](https://gnomad.broadinstitute.org/) — Genome Aggregation Database; genetic variation from large-scale sequencing projects.
* [Rfam](https://rfam.org/) — Database of RNA families with sequence alignments and consensus structures.
* [ROADMAP Epigenomics](http://www.roadmapepigenomics.org/) — Reference epigenome maps for 111 primary human cell types and tissues, including histone modifications, chromatin accessibility, and DNA methylation.
* [FANTOM5](https://fantom.gsc.riken.jp/5/) — Functional annotation of mammalian genome; comprehensive atlas of active enhancers, promoters, and transcription start sites across human and mouse cell types.

### Disease

* [KEGG DRUG](https://www.genome.jp/kegg/drug/) — Comprehensive, approved drug information.
* [DrugBank](https://go.drugbank.com/) — Database of drugs and targets (University of Alberta).
* [DisGeNET](https://www.disgenet.org/) — Database of gene-disease associations integrating expert-curated and GWAS data.
* [OMIM (Online Mendelian Inheritance in Man)](https://www.omim.org/) — Comprehensive database of human genes and genetic disorders.
* [Open Targets Platform](https://platform.opentargets.org/) — Systematic target identification and prioritization platform integrating genetics, genomics, and drug data for drug discovery.
* [Human Phenotype Ontology (HPO)](https://hpo.jax.org/) — Standardized vocabulary of phenotypic abnormalities in human disease, linking genes, variants, and clinical features.
* [DISEASES](https://diseases.jensenlab.org/) — Gene–disease association database integrating evidence from text mining, curated databases, and experimental data.

### Interaction

#### Drug-Gene Interaction

* [DGIdb](https://www.dgidb.org/) — Drug-gene interactions and the druggable genome.
* [Comparative Toxicogenomics Database](http://ctdbase.org/) — Chemical-gene interactions, chemical-disease and gene-disease associations, chemical-phenotype associations.
* [SNAP](https://snap.stanford.edu/biodata/datasets/10002/10002-ChG-Miner.html) — Dataset of drug-gene interactions.

#### Drug (Cell Line) Response

* [NCI60](https://dtp.cancer.gov/discovery_development/nci-60/) — Focuses on 60 cancer cell lines and many drugs.
* [Genomics of Drug Sensitivity in Cancer (GDSC)](https://www.cancerrxgene.org/) — Drug sensitivity for \~1000 human cancer cell lines and hundreds of compounds.
* [Cancer Cell Line Encyclopedia](https://sites.broadinstitute.org/ccle/) — Database of \~1000 cancer cell lines.
* [CellMiner Cross Database (CellMinerCDB)](https://discover.nci.nih.gov/cellminercdb/) — Integrates multiple cancer cell line databases.

#### Chemical-Protein Interaction

* [STITCH](http://stitch.embl.de/) — Chemical-protein interactions.
* [BindingDB](https://www.bindingdb.org/rwd/bind/index.jsp) — Compounds and target database.
* [Davis kinase inhibitors DB](http://staff.cs.utu.fi/~aijrinas/dti/) — Experimental kinase inhibitor binding affinity dataset for protein–ligand interaction research.
* [Kinase Inhibitor Bioactivity Data (KIBA)](https://janeliascicomp.github.io/KIBA/) — Integrated bioactivity scores for kinase inhibitors combining Ki, Kd, and IC50 measurements.
* [PDBBind](https://www.pdbbind-plus.org.cn/) — Binding affinity data for biomolecular complexes.

#### Protein-Protein Interaction

* [STRING](https://string-db.org/) — PPI networks for multiple organisms.
* [BioGRID](https://thebiogrid.org/) — Protein, genetic, and chemical interactions.
* [HIPPIE](http://cbdm-01.zdv.uni-mainz.de/~mschaefer/hippie/) — Human protein-protein interaction database.
* [IntAct](https://www.ebi.ac.uk/intact/home) — Open-source molecular interaction database and analysis system from EMBL-EBI.

#### Knowledge Graph

* [PrimeKG](https://github.com/mims-harvard/PrimeKG) ⭐ 831 | 🐛 7 | 🌐 Jupyter Notebook | 📅 2026-06-30 — Multi-modal precision medicine knowledge graph integrating clinical, genetic, and drug data.
* [DRKG](https://github.com/gnn4dr/DRKG) ⭐ 704 | 🐛 22 | 🌐 Jupyter Notebook | 📅 2022-04-19 — Large-scale biological knowledge graph for drug discovery.
* [Hetionet](https://github.com/hetio/hetionet) ⭐ 363 | 🐛 14 | 🌐 HTML | 📅 2023-04-03 — Heterogeneous network integrating genes, diseases, drugs, pathways, and more.
* [Drug Mechanism Database (DrugMechDB)](https://github.com/SuLab/DrugMechDB/tree/2.0.1) ⭐ 79 | 🐛 12 | 🌐 Jupyter Notebook | 📅 2026-06-03 — Mechanisms of action from drug to disease.

#### Gene Regulatory Network

* [TRRUST v2](https://www.grnpedia.org/trrust/) — Manually curated database of human and mouse transcriptional regulatory interactions between transcription factors and their target genes, expanded with literature-derived evidence.
* [RegNetwork](http://www.regnetworkweb.org/) — Database of gene regulatory networks covering transcription factor–target gene and miRNA–gene interaction data across multiple species.
* [miRBase](https://www.mirbase.org/) — Reference repository for microRNA gene annotations, sequences, and experimentally validated targets.

### Clinical Trial

* [ClinicalTrials.gov](https://clinicaltrials.gov/) — Privately and publicly funded clinical studies.
* [ICD10](https://icd.who.int/browse10/2019/en) — International Classification of Diseases, 10th revision.
* [EU Drug Regulating Authorities Clinical Trials DB (EudraCT)](https://eudract.ema.europa.eu/) — European clinical trial database.
* [MIMIC-IV](https://mimic.mit.edu/) — Freely accessible critical care database.

***

## Benchmarks & Datasets

### Drug Response & Perturbation

* [JUMP Cell Painting Datasets](https://github.com/jump-cellpainting/datasets) ⭐ 190 | 🐛 27 | 🌐 Shell | 📅 2026-10-05 — Consortium-scale cell imaging perturbation datasets (chemical and genetic) for phenotypic profiling and drug discovery research.
* [scPerturb](https://github.com/sanderlab/scPerturb) ⭐ 190 | 🐛 13 | 🌐 Jupyter Notebook | 📅 2025-02-25 — Curated and continuously updated single-cell perturbation data resource spanning CRISPR and drug perturbation studies.
* [Chem-PerturBridge](https://github.com/theislab/Chem-PerturBridge) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-07-22 — Harmonized compendium and processing pipelines for small-molecule perturbation transcriptomics across heterogeneous assays and gene panels.
* [LINCS L1000 Phase 1](https://github.com/theislab/Chem-PerturBridge) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-07-22 — Phase-1 L1000 benchmark view used by Bison with 692,787 profiles, 9,233 molecules, 70 contexts, and 978 landmark genes.
* [LINCS L1000 Phase 2](https://github.com/theislab/Chem-PerturBridge) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-07-22 — Phase-2 L1000 benchmark view used by Bison with 333,263 profiles, 1,760 molecules, 30 contexts, and 978 landmark genes.
* [Novartis Perturbation Dataset](https://github.com/theislab/Chem-PerturBridge) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-07-22 — Large chemical perturbation transcriptomic screen used in Chem-PerturBridge; the Bison benchmark view contains 46,748 profiles and 3,770 molecules.
* [OP3](https://github.com/theislab/Chem-PerturBridge) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-07-22 — Chemical perturbation dataset used by Chem-PerturBridge and the Bison unseen-compound benchmark; the Bison benchmark view contains 1,813 profiles, 138 molecules, and 4 cellular contexts.
* [VCPI-0001](https://github.com/theislab/Chem-PerturBridge) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-07-22 — Bulk chemical perturbation dataset used in Chem-PerturBridge; the Bison benchmark view contains 27,517 profiles and 2,272 molecules in one cellular context.
* [VCPI-0002](https://github.com/theislab/Chem-PerturBridge) ⭐ 2 | 🐛 2 | 🌐 Python | 📅 2026-07-22 — Bulk chemical perturbation dataset used in Chem-PerturBridge; the Bison benchmark view contains 18,139 profiles and 1,488 molecules in one cellular context.
* [BEAT AML](https://biodev.github.io/BeatAML2/) — Functional ex vivo drug sensitivity measurements paired with genomics for acute myeloid leukemia.
* [Cancer Therapeutics Response Portal (CTRP)](https://portals.broadinstitute.org/ctrp/) — Drug sensitivity profiles across \~900 cancer cell lines for >400 compounds.
* [GSE191127 Breast Cancer Pre/Post Chemotherapy](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE191127) — Bulk RNA-seq and genomics from matched pre- and post-neoadjuvant chemotherapy breast tumors with treatment outcomes.
* [Genomics of Drug Sensitivity in Cancer (GDSC)](https://www.cancerrxgene.org/) — Drug sensitivity for \~1000 human cancer cell lines and hundreds of compounds.
* [LINCS L1000](https://lincsproject.org/LINCS/tools/workflows/find-the-best-place-to-obtain-the-lincs-l1000-data) — Gene expression profiles (978 landmark genes) for >20,000 chemical and genetic perturbations across cell lines.
* [MIX-Seq](https://www.nature.com/articles/s41467-020-17440-w) — Multiplexed single-cell transcriptional profiling of chemical and genetic perturbation responses across pools of cancer cell lines.
* [NCI60](https://dtp.cancer.gov/discovery_development/nci-60/) — Drug sensitivity benchmark across 60 diverse human cancer cell lines.
* [PDX-Atlas](https://muralportal.pdxatlas.org/) — Portal integrating clinical, genomic, transcriptomic, and drug-response data from patient-derived xenograft models.
* [PharmGKB](https://www.pharmgkb.org/) — Curated pharmacogenomics dataset linking genetic variants to drug response phenotypes across thousands of drugs.
* [PRISM](https://depmap.org/portal/prism/) — Cancer drug sensitivity profiling of >4,500 drugs across >900 cancer cell lines using pooled-cell-line barcoding.
* [sci-Plex](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE139944) — Single-cell chemical perturbation screen of \~650,000 transcriptomes across three cancer cell lines, 188 compounds, and four doses.
* [Tahoe-100M](https://huggingface.co/datasets/tahoebio/Tahoe-100M) — Giga-scale single-cell perturbation atlas with >100 million profiles from 50 cancer cell lines exposed to \~1,100 small molecules.

### Genetic Perturbation & Perturb-seq

* [Dixit et al. 2016 Perturb-seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90063) — Pooled CRISPR knockout with single-cell RNA-seq across K562 and dendritic-cell screens, including stimulated conditions and combinatorial perturbations.
* [Adamson et al. 2016 Perturb-seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90546) — CRISPRi Perturb-seq in K562 cells for systematic dissection of the unfolded protein response.
* [Datlinger et al. 2017 CROP-seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE92872) — Pooled CRISPR knockout screen with single-cell transcriptomic readout in Jurkat cells under T-cell receptor stimulation.
* [Norman et al. 2019 CRISPRa Perturb-seq](https://figshare.com/articles/dataset/Norman_et_al_2019_Perturb-seq/27766323) — Large-scale CRISPR activation Perturb-seq in K562 cells spanning single-gene and combinatorial perturbations.
* [Gasperini et al. 2019 CRISPRi enhancer screen](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE120861) — High-MOI single-cell CRISPRi screen in K562 cells targeting thousands of candidate enhancers to map enhancer-gene regulation.
* [Replogle et al. 2022 K562 Genome-wide Perturb-seq](https://plus.figshare.com/articles/dataset/_Mapping_information-rich_genotype-phenotype_landscapes_with_genome-scale_Perturb-seq_Replogle_et_al_2022_processed_Perturb-seq_datasets/20029387) — Genome-scale CRISPRi Perturb-seq targeting nearly all expressed genes in K562 cells.
* [Replogle et al. 2022 K562 Essential Perturb-seq](https://plus.figshare.com/articles/dataset/_Mapping_information-rich_genotype-phenotype_landscapes_with_genome-scale_Perturb-seq_Replogle_et_al_2022_processed_Perturb-seq_datasets/20029387) — CRISPRi Perturb-seq focused on essential genes in K562 cells.
* [Replogle et al. 2022 RPE1 Essential Perturb-seq](https://plus.figshare.com/articles/dataset/_Mapping_information-rich_genotype-phenotype_landscapes_with_genome-scale_Perturb-seq_Replogle_et_al_2022_processed_Perturb-seq_datasets/20029387) — CRISPRi Perturb-seq focused on essential genes in RPE1 cells.
* [Frangieh et al. 2021 Perturb-CITE-seq](https://singlecell.broadinstitute.org/single_cell/study/SCP1064/multi-modal-pooled-perturb-cite-seq-screens-in-patient-models-define-novel-mechanisms-of-cancer-immune-evasion) — Multimodal CRISPR knockout screen with RNA and surface-protein readouts in patient-derived melanoma models under immune-related conditions.

### Single-Cell & Spatial

* [scIB (Single-cell Integration Benchmarks)](https://github.com/theislab/scib) ⭐ 432 | 🐛 44 | 🌐 Python | 📅 2026-04-27 — Comprehensive benchmarking framework for single-cell data integration methods.
* [HEST Xenium virtual spatial transcriptomics](https://huggingface.co/datasets/ratschlab/HEST_Xenium_virtual_spatial_transcriptomics) — DeepSpot-M predicted transcriptome-wide ST for 59 HEST-1k 10x Xenium samples (\~13.3M cells) (gated). Paper: [DeepSpot-M](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1).
* [Tabula Muris](https://tabula-muris.ds.czbiohub.org/) — Comprehensive single-cell atlas of 20 mouse organs and tissues, enabling cross-tissue and cross-species comparisons.
* [Tabula Sapiens](https://tabula-sapiens-portal.ds.czbiohub.org/) — Comprehensive human single-cell atlas of \~500K cells from 24 organs and tissues across multiple donors.
* [TCGA virtual spatial transcriptomics atlas](https://huggingface.co/datasets/ratschlab/TCGA_virtual_spatial_transcriptomics_atlas) — DeepSpot-M predicted transcriptome-wide ST for TCGA H\&E (FF + FFPE; 28,664 slides / 32 cancer types; gated). Paper: [DeepSpot-M](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1).

### Molecular, Protein & Drug Discovery

* [MOSES](https://github.com/molecularsets/moses) ⭐ 991 | 🐛 31 | 🌐 Python | 📅 2024-07-08 — Benchmarking platform for molecular generation models.
* [TAPE (Tasks Assessing Protein Embeddings)](https://github.com/songlab-cal/tape) ⭐ 745 | 🐛 30 | 🌐 Python | 📅 2022-12-11 — Benchmark suite of five biologically meaningful semi-supervised learning tasks for evaluating protein representations.
* [GuacaMol](https://github.com/BenevolentAI/guacamol) ⭐ 535 | 🐛 13 | 🌐 Python | 📅 2024-02-11 — Benchmark suite for generative molecular design models.
* [ProteinGym](https://github.com/OATML-Markslab/ProteinGym) ⭐ 475 | 🐛 33 | 🌐 HTML | 📅 2026-03-25 — Large-scale benchmark of deep mutational scanning assays for evaluating protein fitness landscape models.
* [FLIP (Fitness Landscape Inference for Proteins)](https://github.com/J-SNACKKB/FLIP) ⭐ 141 | 🐛 4 | 🌐 Jupyter Notebook | 📅 2026-04-23 — Benchmark collection of protein fitness landscape datasets for evaluating protein ML models.
* [Bento](https://github.com/LigandPro/Bento) ⭐ 13 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-03-04 — Protein-ligand docking benchmark covering rigid, flexible, de novo, blind, induced-fit, and covalent docking tasks.
* [BACE](https://www.kaggle.com/datasets/gokturkkoch/bace) — Binary classification and regression dataset for β-secretase 1 (BACE-1) inhibitor binding affinity.
* [BindingDB Curated Sets](https://www.bindingdb.org/rwd/bind/chemsearch/marvin/SDFdownload.jsp?all_download=yes) — Curated binding affinity datasets for protein–ligand interaction benchmarking.
* [ClinTox](https://tdcommons.ai/single_pred_tasks/tox/#clintox) — Clinical toxicity dataset contrasting FDA-approved drugs with those that failed clinical trials due to toxicity.
* [CrossDocked2020](https://arxiv.org/abs/2001.01037) — Large-scale dataset for structure-based virtual screening.
* [DUD-E (Directory of Useful Decoys, Enhanced)](http://dude.docking.org/) — Structure-based virtual screening benchmark with active ligands and challenging decoy sets across diverse protein targets.
* [MoleculeNet](http://moleculenet.ai/) — Benchmark datasets for molecular machine learning.
* [PK-DB](https://pk-db.com/) — Open database of experimental pharmacokinetics (PK) and ADME data from clinical and preclinical studies.
* [QM9](https://figshare.com/collections/Quantum_chemistry_structures_and_properties_of_134_kilo_molecules/978904) — Quantum chemistry properties for 134K stable small organic molecules computed at DFT level.
* [SIDER (Side Effect Resource)](http://sideeffects.embl.de/) — Database of 1,430 approved drugs with their recorded adverse drug reactions across 27 system-organ classes.
* [Therapeutics Data Commons (TDC)](https://tdcommons.ai/) — Unified benchmark suite covering ADMET, drug-target interaction, drug response, and more.
* [Tox21](https://tripod.nih.gov/tox21/challenge/) — 12,707 compounds tested in 12 nuclear receptor and stress-response pathway biochemical assays for toxicity prediction.

### Genomics, Cancer & Biomedical Cohorts

* [1000 Genomes Project](https://www.internationalgenome.org/) — Reference panel of human genetic variation from 2,504 individuals across 26 populations.
* [CPTAC (Clinical Proteomic Tumor Analysis Consortium)](https://proteomics.cancer.gov/programs/cptac) — Multi-omic proteogenomic datasets for multiple cancer types linking proteomics with genomics.
* [The Cancer Genome Atlas (TCGA)](https://www.cancer.gov/about-nci/organization/ccg/research/structural-genomics/tcga) — Comprehensive multi-omics (genomics, transcriptomics, proteomics, methylation) dataset for 33 cancer types across \~11,000 patients.
* [UK Biobank](https://www.ukbiobank.ac.uk/) — Large-scale biomedical database of \~500K participants with genetic, imaging, and health data for population genetics and disease studies.

### General Biological ML & Knowledge Graph Benchmarks

* [OpenBioLink](https://github.com/OpenBioLink/OpenBioLink) ⭐ 164 | 🐛 11 | 🌐 Python | 📅 2024-05-03 — Benchmark datasets for biological knowledge graph completion.
* [OGB (Open Graph Benchmark)](https://ogb.stanford.edu/) — Large-scale graph ML benchmark suite including biological datasets such as ogbl-ppa (protein-protein associations) and ogbg-molhiv.

***

## API

* [PubMed E-utilities (esearch/efetch)](https://www.nlm.nih.gov/dataguide/edirect/esearch.html) — APIs for searching and retrieving biomedical literature from PubMed.
* [NCBI E-utilities](https://www.ncbi.nlm.nih.gov/books/NBK25501/) — Unified APIs for accessing NCBI databases (Gene, GEO, SRA, PubChem, etc).
* [UniProt REST API](https://www.uniprot.org/help/api) — Programmatic access to protein sequence and functional annotation data.
* [Ensembl REST API](https://rest.ensembl.org/) — API for genomic annotations, variants, genes, and comparative genomics.
* [KEGG REST API](https://www.kegg.jp/kegg/rest/keggapi.html) — API for accessing KEGG pathways, compounds, genes, and reactions.
* [ChEMBL Web Services](https://www.ebi.ac.uk/chembl/ws) — REST API for bioactive molecules, targets, and bioassays.
* [Open Targets Platform API](https://platform.opentargets.org/api) — API for target–disease associations integrating genetics, genomics, and drug data.
* [ClinicalTrials.gov API](https://clinicaltrials.gov/api/gui) — API for querying clinical trial metadata and results.

***

## Preprocessing Tools

* [DeepChem](https://github.com/deepchem/deepchem) ⭐ 7,038 | 🐛 1,211 | 🌐 Python | 📅 2026-08-20 — Deep learning library for drug discovery, quantum chemistry, and materials science.
* [RDKit](https://github.com/rdkit/rdkit) ⭐ 3,606 | 🐛 98 | 🌐 HTML | 📅 2026-10-03 — Cheminformatics software & machine learning toolkit.
* [STAR](https://github.com/alexdobin/STAR) ⭐ 2,262 | 🐛 1,010 | 🌐 C | 📅 2025-03-18 — Ultrafast universal RNA-seq aligner with support for spliced alignment and single-cell quantification via STARsolo.
* [CellChat](https://github.com/sqjin/CellChat) ⚠️ Archived — Inference and analysis of cell-cell communication ligand-receptor networks from single-cell transcriptomics data.
* [Harmony](https://github.com/immunogenomics/harmony) ⭐ 676 | 🐛 88 | 🌐 R | 📅 2026-06-05 — Fast and scalable integration of single-cell data across datasets, conditions, technologies, and species.
* [Chemistry Development Kit](https://github.com/cdk/cdk) ⭐ 606 | 🐛 13 | 🌐 Java | 📅 2026-10-05 — Cheminformatics software & machine learning tools.
* [DoubletFinder](https://github.com/chris-mcginnis-ucsf/DoubletFinder) ⭐ 569 | 🐛 23 | 🌐 R | 📅 2025-03-21 — Machine learning approach for detecting multiplet (doublet) artifacts in single-cell RNA-seq data.
* [scVelo](https://github.com/theislab/scvelo) ⭐ 512 | 🐛 83 | 🌐 Python | 📅 2026-02-25 — RNA velocity estimation for single-cell transcriptomics, inferring the direction and speed of cell differentiation.
* [CellTypist](https://github.com/Teichlab/celltypist) ⭐ 509 | 🐛 48 | 🌐 Python | 📅 2026-05-22 — Automated cell type annotation for scRNA-seq.
* [SCENIC](https://github.com/aertslab/SCENIC) ⭐ 498 | 🐛 113 | 🌐 HTML | 📅 2024-04-05 — Single-cell regulatory network inference and clustering linking transcription factors to co-expressed gene modules.
* [Numbat](https://github.com/kharchenkolab/numbat) ⭐ 231 | 🐛 80 | 🌐 R | 📅 2026-02-04 — Haplotype-aware copy number variation inference from single-cell RNA-seq using hidden Markov models.
* [CellCharter](https://github.com/CSOgroup/cellcharter) ⭐ 197 | 🐛 17 | 🌐 Python | 📅 2026-10-05 — Identification and characterization of spatial cell niches from spatial transcriptomics using VAEs and Gaussian mixture models.
* [MOGONET](https://github.com/txWang/MOGONET) ⭐ 188 | 🐛 0 | 🌐 Python | 📅 2021-03-31 — Multi-omics graph convolutional network framework for patient classification and biomarker identification.
* [COMMOT](https://github.com/zcang/COMMOT) ⭐ 146 | 🐛 27 | 🌐 Python | 📅 2026-06-25 — Optimal transport-based framework for screening cell-cell communication in spatial transcriptomics.
* [LINGER](https://github.com/Durenlab/LINGER) ⭐ 141 | 🐛 54 | 🌐 Jupyter Notebook | 📅 2026-07-11 — Neural network for gene regulatory network inference from single-cell multiome (RNA+ATAC-seq) data with bulk data pretraining.
* [NCEM](https://github.com/theislab/ncem) ⭐ 121 | 🐛 34 | 🌐 Python | 📅 2024-01-15 — GNN-based model for learning intercellular communication from spatial graphs of cells.
* [CaSpER](https://github.com/akdess/CaSpER) ⭐ 92 | 🐛 41 | 🌐 R | 📅 2021-04-05 — CNV identification and visualization by integrative analysis of single-cell or bulk RNA-seq data.
* [TIGON](https://github.com/yutongo/TIGON) ⭐ 60 | 🐛 2 | 🌐 Jupyter Notebook | 📅 2025-03-23 — Neural optimal transport method for reconstructing growth and dynamic trajectories from single-cell transcriptomics.
* [STAGATE](https://github.com/RucDongLab/STAGATE) ⭐ 54 | 🐛 12 | 🌐 Python | 📅 2023-04-28 — Adaptive graph attention auto-encoder for spatial domain identification in spatial transcriptomics.
* [AutoZyme](https://github.com/ElliotXie/autozyme) ⭐ 51 | 🐛 1 | 🌐 Python | 📅 2026-09-13 — Autonomous agentic framework that speeds up bioinformatics software (e.g. Scanpy, Seurat) on CPUs while preserving the original results.
* [ChatSpatial](https://github.com/cafferychen777/ChatSpatial) ⭐ 45 | 🐛 13 | 🌐 Python | 📅 2026-09-29 — MCP server for spatial transcriptomics analysis via natural language.
* [DeepTalk](https://github.com/JiangBioLab/DeepTalk) ⭐ 30 | 🐛 9 | 🌐 Jupyter Notebook | 📅 2024-09-06 — Graph attention network for deciphering cell-cell communication from spatial transcriptomics.
* [FlashDeconv](https://github.com/cafferychen777/flashdeconv) ⭐ 26 | 🐛 0 | 🌐 Python | 📅 2026-09-29 — High-performance spatial transcriptomics deconvolution (\~1M spots in \~3 min).
* [sciPENN](https://github.com/jlakkis/sciPENN) ⭐ 19 | 🐛 3 | 🌐 Python | 📅 2022-07-30 — RNN-based method for simultaneous protein expression prediction, uncertainty estimation, and cell-type label transfer from CITE-seq and scRNA-seq data.
* [Biopython](https://biopython.org/) — Collection of Python tools for biological computation including sequence analysis, structure parsing, and database access.
* [Scanpy](https://scanpy.readthedocs.io/en/stable/) — Python library for scRNA-seq analysis.
* [Seurat](https://satijalab.org/seurat/) — R library for scRNA-seq analysis.
* [scvi-tools](https://scvi-tools.org/) — Probabilistic models for single-cell omics data analysis.
* [Squidpy](https://squidpy.readthedocs.io/) — Python library for spatial single-cell analysis.
* [GROMACS](https://www.gromacs.org/) — Molecular dynamics simulation package for biochemical molecules.
* [MDAnalysis](https://www.mdanalysis.org/) — Python library for analyzing and altering molecular dynamics simulation trajectories.
* [OpenMM](https://openmm.org/) — High-performance toolkit for molecular simulation and GPU-accelerated MD.
* [kallisto](https://pachterlab.github.io/kallisto/) — Near-optimal RNA-seq quantification using pseudoalignment for fast transcript abundance estimation.
* [Monocle3](https://cole-trapnell-lab.github.io/monocle3/) — Single-cell trajectory analysis tool for learning developmental trajectories and ordering cells in pseudotime.
* [SeqBench](https://seqbench.com/) — Web-based molecular biology sequence workbench for primer design, cloning simulation (Gibson, Golden Gate, restriction digest), CRISPR guide RNA design, and sequence analysis, with a public REST API, OpenAPI 3.1 spec, and MCP server.

***

## Machine Learning Tasks and Models

### Drug Discovery

#### Drug Response Prediction

* [RECOVER](https://github.com/RECOVERcoalition/Recover) ⭐ 26 | 🐛 3 | 🌐 Jupyter Notebook | 📅 2024-08-13 — Machine learning framework for predicting synergistic drug combination responses across cell lines.
* [TGSA](https://github.com/violet-sto/TGSA) ⭐ 24 | 🐛 1 | 🌐 Python | 📅 2021-12-15 — Tumor gene set and attention-based model leveraging biological pathway knowledge for drug response prediction.
* [DRUML](https://github.com/CutillasLab/DRUMLR) ⭐ 12 | 🐛 2 | 🌐 R | 📅 2022-03-23 — Ensemble machine learning framework combining standard ML with deep learning to systematically rank anti-cancer drugs from proteomics and RNA-seq data.
* [MOFGCN](https://github.com/weiba/MOFGCN/tree/main) ⭐ 8 | 🐛 6 | 🌐 Python | 📅 2023-07-28 — GCN + heterogeneous network.
* [PASO](https://github.com/queryang/PASO) ⭐ 8 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2025-02-27 — Pathway-aware multi-omics drug response model combining pathway-difference features, multi-scale convolutions, Transformer encoding, and drug SMILES.
* [DeepAEG](https://github.com/zhejiangzhuque/DeepAEG) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2023-12-26 — GNN embedding + attention mechanism.
* [drGAT](https://github.com/inoue0426/drGAT) ⭐ 2 | 🐛 1 | 🌐 Jupyter Notebook | 📅 2026-02-27 — Attention-based model for drug response prediction with gene explainability.
* [DGDRP](https://github.com/minwoopak/heteronet) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2024-02-24 — Multi-view embedding neural network.
* [THERAPI](https://github.com/Sunginyoung/THERAPI) ⭐ 1 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-02-15 — Cell-line-to-patient transfer framework that aligns tumor transcriptomes with cancer cell lines and integrates perturbation and gene-level representations for patient drug response prediction.
* [DeepDSC](https://ieeexplore-ieee-org.ezp2.lib.umn.edu/stamp/stamp.jsp?tp=\&arnumber=8723620\&tag=1) — Autoencoder + fully connected NN.
* [HiDRA](https://github.com/bsml320/HiDRA) — Hierarchical network model incorporating gene and pathway-level information for cancer drug response prediction.
* [DTLCDR](https://doi.org/10.1016/j.jpha.2025.101315) — Target-based multimodal framework for preclinical cancer drug response prediction and transfer to clinical response, with explicit unseen-drug generalization.
* [EXPRESSO](https://doi.org/10.1158/0008-5472.CAN-25-5220) — Supervised treatment-response framework using pretreatment tumor transcriptomics, drug targets, and context-specific biomarkers across multiple cancer types and therapies.
* [PerturbRx](https://arxiv.org/abs/2608.21349) — Treatment-conditioned representation learning framework that transfers drug-induced latent transitions learned from single-cell perturbation data to patient-level cancer treatment-response prediction.

#### Drug Perturbation

* [State](https://github.com/ArcInstitute/state) ⭐ 713 | 🐛 61 | 🌐 Python | 📅 2026-07-24 — Transition model for predicting cellular perturbation responses across diverse contexts and sets of cells.
* [CellOT](https://github.com/bunnech/cellot) ⭐ 181 | 🐛 12 | 🌐 Python | 📅 2024-10-31 — Neural optimal transport framework for predicting single-cell responses to drug and genetic perturbations.
* [CellFlow](https://github.com/theislab/CellFlow) ⭐ 161 | 🐛 68 | 🌐 Python | 📅 2026-10-05 — Conditional flow-matching framework for modeling and predicting cellular phenotypes under chemical, genetic, and other perturbations.
* [chemCPA](https://github.com/theislab/chemCPA) ⭐ 160 | 🐛 7 | 🌐 Jupyter Notebook | 📅 2025-02-06 — Compositional perturbation autoencoder for predicting single-cell transcriptional responses to unseen drug perturbations and dose combinations.
* [biolord](https://github.com/nitzanlab/biolord) ⭐ 102 | 🐛 2 | 🌐 Python | 📅 2024-08-12 — Deep generative model that disentangles known and unknown attributes for conditional generation of single-cell states.
* [PRNet](https://github.com/Perturbation-Response-Prediction/PRnet) ⭐ 91 | 🐛 18 | 🌐 Jupyter Notebook | 📅 2024-12-13 — Deep generative model for predicting transcriptional responses to novel chemical perturbations for drug discovery.
* [PerturbNet](https://github.com/welch-lab/PerturbNet) ⭐ 69 | 🐛 3 | 🌐 Jupyter Notebook | 📅 2026-01-12 — Conditional generative model for predicting distributions of single-cell states under unseen chemical and genetic perturbations.
* [LPM](https://github.com/perturblib/perturblib) ⭐ 54 | 🐛 2 | 🌐 Python | 📅 2025-06-16 — Large perturbation model that jointly learns heterogeneous perturbation experiments by disentangling perturbation, readout, and context representations.
* [TxPert](https://github.com/valence-labs/TxPert) ⭐ 52 | 🐛 2 | 🌐 Python | 📅 2026-03-25 — Knowledge-graph-informed latent-transfer model for transcriptomic perturbation prediction across unseen single perturbations, combinations, and cross-context settings.
* [Prophet](https://github.com/theislab/prophet) ⭐ 41 | 🐛 6 | 🌐 Python | 📅 2026-02-24 — Transformer model for predicting cellular phenotypes under unseen chemical or genetic perturbations across heterogeneous assays and contexts.
* [XPert](https://github.com/GSanShui/XPert) ⭐ 27 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2025-11-22 — Knowledge-informed dual-branch Transformer for drug-induced transcriptional perturbation prediction across dose, time, and cellular context.
* [CMonge](https://github.com/AI4SCR/conditional-monge-gap) ⭐ 25 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-10 — Conditional optimal transport model for generalizable single-cell perturbation response prediction across drugs and doses.
* [PrePR-CT](https://github.com/reem12345/Cell-Type-Specific-Graphs) ⭐ 8 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2025-09-10 — Graph-based model using cell-type-specific co-expression networks as inductive priors for small-data chemical perturbation response prediction.
* [cycleCDR](https://github.com/hliulab/cycleCDR) ⭐ 5 | 🐛 0 | 🌐 Python | 📅 2024-01-24 — Interpretable cycle-consistency framework for modeling cellular responses to drug perturbations.
* [Bison](https://arxiv.org/abs/2609.32467) — Cross-dataset model for globally unseen-compound response prediction using a shared gene representation, discrete diffusion models, and matched drug-contrast supervision.

#### Drug Repurposing

* [DeepPurpose](https://github.com/kexinhuang12345/DeepPurpose) ⭐ 1,194 | 🐛 18 | 🌐 Jupyter Notebook | 📅 2024-06-10 — Deep learning library for drug repurposing.
* [TranSiGen](https://github.com/myzhengSIMM/TranSiGen) ⭐ 39 | 🐛 19 | 🌐 Jupyter Notebook | 📅 2025-01-21 — Dual-VAE architecture for ligand-based virtual screening, drug response prediction, and drug repurposing using chemical-induced transcriptional profiles.

#### Drug Target Interaction

* [GraphDTA](https://github.com/thinng/GraphDTA) ⭐ 308 | 🐛 2 | 🌐 Python | 📅 2021-04-13 — Graph neural network–based DTI prediction using molecular graphs.
* [DeepDTA](https://github.com/hkmztrk/DeepDTA) ⭐ 306 | 🐛 5 | 🌐 Python | 📅 2023-09-22 — Deep learning model using CNNs on protein sequences and drug SMILES.
* [MolTrans](https://github.com/kexinhuang12345/MolTrans) ⭐ 248 | 🐛 4 | 🌐 Jupyter Notebook | 📅 2022-07-15 — Transformer-based DTI model leveraging molecular substructures.
* [DTINet](https://github.com/luoyunan/DTINet) ⭐ 192 | 🐛 8 | 🌐 MATLAB | 📅 2022-10-30 — Network-based framework integrating heterogeneous biological data for DTI prediction.
* [DrugBAN](https://github.com/peizhenbai/DrugBAN) ⭐ 155 | 🐛 8 | 🌐 Python | 📅 2023-02-19 — Bilinear attention network for interpretable DTI prediction.
* [NeoDTI](https://github.com/FangpingWan/NeoDTI) ⭐ 79 | 🐛 3 | 🌐 Python | 📅 2021-05-13 — Library for drug-target interaction prediction.

#### Compound-Protein Interaction

* [TransformerCPI](https://github.com/lifanchen-simm/transformerCPI) ⭐ 159 | 🐛 1 | 🌐 Python | 📅 2022-06-30 — CPI prediction using Transformer.
* [MCPINN](https://github.com/mhlee0903/multi_channels_PINN) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2023-08-25 — Drug discovery via compound-protein interaction and machine learning.

#### Molecular Generation

* [DiffDock](https://github.com/gcorso/DiffDock) ⭐ 1,579 | 🐛 132 | 🌐 Python | 📅 2025-05-02 — Diffusion generative model for molecular docking, predicting the binding pose of small molecules to protein targets.
* [JTVAE](https://github.com/wengong-jin/icml18-jtnn) ⭐ 566 | 🐛 30 | 🌐 Python | 📅 2022-12-01 — Junction tree variational autoencoder for molecular graph generation that guarantees chemical validity via a hierarchical tree decomposition.
* [DiffSBDD](https://github.com/arneschneuing/DiffSBDD) ⭐ 532 | 🐛 30 | 🌐 Python | 📅 2025-06-25 — Equivariant diffusion model for structure-based drug design that generates molecules and binding conformations for protein targets.
* [Molecular Transformer](https://github.com/pschwllr/MolecularTransformer) ⭐ 429 | 🐛 2 | 🌐 Python | 📅 2022-04-18 — Sequence-to-sequence model for retrosynthesis prediction.
* [REINVENT](https://github.com/MolecularAI/Reinvent) ⚠️ Archived — Reinforcement learning for de novo drug design.
* [ReLeaSE](https://github.com/isayev/ReLeaSE) ⭐ 373 | 🐛 27 | 🌐 Jupyter Notebook | 📅 2021-12-08 — Deep reinforcement learning framework for de novo drug design combining a generative and predictive model.
* [TargetDiff](https://github.com/guanjq/targetdiff) ⭐ 347 | 🐛 13 | 🌐 Python | 📅 2024-01-10 — 3D equivariant diffusion model for structure-based drug design.
* [MolGPT](https://github.com/devalab/molgpt) ⭐ 178 | 🐛 22 | 🌐 Python | 📅 2023-07-15 — Transformer-based model for molecular generation.
* [Matcha](https://github.com/LigandPro/Matcha) ⭐ 36 | 🐛 2 | 🌐 Python | 📅 2026-09-22 — Multi-stage Riemannian flow matching model for physically valid molecular docking with scoring, pose filtering, and benchmarks.
* [PaccMannRL](https://github.com/PaccMann/paccmann_generator) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2024-05-22 — Reinforcement learning-based generative model for de novo hit-like anticancer molecule design from transcriptomic data.

### Protein Property Prediction

* [NbBayesLM](https://github.com/FairuzShadmaniShishir/NbBayesLM) ⭐ 4 | 🐛 1 | 🌐 Python | 📅 2026-05-31 — Bayesian neural network integrating protein language model embeddings and physicochemical features to predict nanobody thermostability with uncertainty estimates. [Paper](https://www.frontiersin.org/journals/bioinformatics/articles/10.3389/fbinf.2026.1832968/full)

### LLM for Biology

* [BioGPT](https://github.com/microsoft/BioGPT) ⚠️ Archived — LLM for biomedical text generation.
* [GeneGPT](https://github.com/ncbi/GeneGPT) ⭐ 430 | 🐛 0 | 🌐 Python | 📅 2025-05-08 — LLM for biomedical information, integrated with various APIs.
* [GenePT](https://github.com/yiqunchen/GenePT) ⭐ 324 | 🐛 17 | 🌐 Jupyter Notebook | 📅 2024-03-18 — Foundation LLM for single-cell data.
* [MolT5](https://github.com/blender-nlp/MolT5) ⭐ 195 | 🐛 0 | 🌐 Python | 📅 2023-09-15 — Language model for molecular tasks bridging text and SMILES, enabling molecule captioning and text-driven molecule generation.
* [ChatDrug](https://github.com/chao1224/ChatDrug) ⭐ 163 | 🐛 0 | 🌐 Python | 📅 2024-05-28 — LLM-based conversational pipeline for drug discovery, using natural language prompts for iterative drug editing and optimization.
* [scPRINT](https://github.com/cantinilab/scPRINT) ⭐ 162 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-11 — Pretrained on 50M cells for scRNA-seq denoising & zero imputation.
* [AI4Chem/ChemLLM-7B-Chat](https://huggingface.co/AI4Chem/ChemLLM-7B-Chat) — LLM for chemical & molecular science.
* [BioMedLM](https://huggingface.co/stanford-crfm/BioMedLM) — 2.7B parameter GPT-2-style language model trained exclusively on biomedical literature from PubMed for biomedical question answering and text generation.

### Agentic AI for Biology

#### General Biomedical Agents

* [Biomni](https://github.com/snap-stanford/Biomni) ⭐ 3,942 | 🐛 118 | 🌐 Python | 📅 2026-10-05 — General-purpose biomedical AI agent integrating planning, code execution, specialized tools, databases, and software across diverse biomedical research tasks.
* [ToolUniverse](https://github.com/mims-harvard/ToolUniverse) ⭐ 1,719 | 🐛 18 | 🌐 Python | 📅 2026-10-06 — Unified scientific tool ecosystem for building AI scientists that can discover, select, and execute biomedical tools and databases.
* [ClawBio](https://github.com/ClawBio/ClawBio) ⭐ 1,152 | 🐛 45 | 🌐 Python | 📅 2026-10-06 — Bioinformatics-native AI agent skill library with local-first pharmacogenomics, ancestry PCA, semantic similarity, nutrigenomics, and metagenomics skills.
* [BioMedAgent](https://github.com/BOBQWERA/BioMedAgent) ⭐ 144 | 🐛 3 | 🌐 Python | 📅 2026-09-01 — Self-evolving multi-agent framework for autonomous biomedical data analysis with tool discovery, workflow planning, code generation, execution, correction, and cross-omics analysis.
* [BioMaster](https://github.com/ai4nucleome/BioMaster) ⭐ 115 | 🐛 2 | 🌐 TypeScript | 📅 2026-07-14 — Multi-agent system for automated and auditable bioinformatics workflows spanning RNA-seq, ChIP-seq, single-cell, spatial omics, Hi-C, long reads, metagenomics, and proteomics.
* [BRAD](https://github.com/Jpickard1/BRAD) ⭐ 64 | 🐛 3 | 🌐 Python | 📅 2025-05-14 — Retrieval-augmented bioinformatics assistant integrating scientific literature, databases, external tools, and executable workflows.

#### Therapeutics & Drug Discovery Agents

* [TxAgent](https://github.com/mims-harvard/TxAgent) ⭐ 655 | 🐛 22 | 🌐 Python | 📅 2025-07-30 — Therapeutic reasoning agent using multi-step reasoning and a large scientific tool universe for drug interactions, contraindications, and personalized treatment analysis.
* [Medea](https://github.com/mims-harvard/Medea) ⭐ 131 | 🐛 8 | 🌐 Python | 📅 2026-07-17 — Multi-agent therapeutic discovery system combining research planning, biological data analysis, literature reasoning, and multi-LLM deliberation across single-cell, cell-line, and patient contexts.
* [DrugAgent](https://github.com/inoue0426/DrugAgent) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2026-07-03 — Multi-agent biomedical evidence synthesis framework for computational drug discovery with reliability-aware aggregation.

#### Bioinformatics & Omics Agents

* [Genomi](https://github.com/exon-research/genomi) ⭐ 484 | 🐛 0 | 🌐 Python | 📅 2026-08-31 — Local-first genomics agent runtime that indexes personal variants, queries evidence, and generates evidence-grounded reports while keeping raw genome data on-device.
* [AutoBA](https://github.com/JoshuaChou2018/AutoBA) ⭐ 239 | 🐛 2 | 🌐 Python | 📅 2024-11-04 — Automated multi-omics analysis agent that plans, executes, and repairs bioinformatics workflows from natural-language objectives.
* [STELLA](https://github.com/zaixizhang/STELLA) ⭐ 156 | 🐛 0 | 🌐 Python | 📅 2026-09-15 — Self-evolving biomedical research agent that expands its tool repertoire and supports literature reasoning, computational analysis, and laboratory-oriented scientific workflows.
* [GenoMAS](https://github.com/Liu-Hy/GenoMAS) ⭐ 135 | 🐛 0 | 🌐 Python | 📅 2026-04-20 — Multi-agent framework for code-driven gene-expression analysis with planning, execution, debugging, backtracking, and GEO/TCGA-based scientific discovery.
* [CASSIA](https://github.com/ElliotXie/CASSIA) ⭐ 107 | 🐛 3 | 🌐 Python | 📅 2026-09-11 — Multi-agent LLM framework for reference-free and interpretable single-cell cell-type annotation with dedicated annotation, validation, scoring, and reporting agents.
* [BioAgents](https://github.com/microsoft/bioinformagus) ⭐ 47 | 🐛 2 | 🌐 Jupyter Notebook | 📅 2026-04-21 — Multi-agent bioinformatics assistant using specialized language models and retrieval for genomics workflow development and troubleshooting.
* [BIA](https://github.com/biagent-dev/bia) ⭐ 45 | 🐛 1 | 🌐 Python | 📅 2024-08-21 — Bioinformatics agent for GEO search, sample metadata extraction, count-matrix processing, and pipeline extraction from papers.

#### Multi-Agent Scientific Labs

* [Agent Laboratory](https://github.com/SamuelSchmidgall/AgentLaboratory) ⭐ 5,887 | 🐛 61 | 🌐 Python | 📅 2025-08-20 — End-to-end multi-agent research workflow for literature review, experimentation, implementation, analysis, and report generation.
* [Virtual Lab](https://github.com/zou-group/virtual-lab) ⭐ 739 | 🐛 7 | 🌐 Jupyter Notebook | 📅 2025-12-31 — Human–AI collaborative research environment in which an LLM principal investigator coordinates specialized scientist agents for scientific discovery.

#### Paper & Workflow Agents

* [Paper2Agent](https://github.com/jmiao24/Paper2Agent) ⭐ 3,707 | 🐛 0 | 🌐 Python | 📅 2026-09-17 — Multi-agent system that transforms research papers and associated code into interactive, testable scientific agents and MCP tools.

### Foundation Models

#### Single-cell Foundation Models

##### Transcriptomics Foundation Models

* [scGPT](https://github.com/bowang-lab/scGPT) ⭐ 1,644 | 🐛 176 | 🌐 Jupyter Notebook | 📅 2026-04-29 — Transformer-based foundation model pretrained on millions of single-cell profiles.
* [scFoundation](https://github.com/biomap-research/scFoundation) ⭐ 431 | 🐛 31 | 🌐 Jupyter Notebook | 📅 2025-11-23 — Large-scale foundation model for single-cell gene expression, enabling multiple downstream tasks.
* [GEARS](https://github.com/snap-stanford/GEARS) ⭐ 414 | 🐛 21 | 🌐 Python | 📅 2025-02-01 — Graph-based model for predicting transcriptional responses to single and combinatorial genetic perturbations using biological priors.
* [scBERT](https://github.com/TencentAILabHealthcare/scBERT) ⭐ 364 | 🐛 26 | 🌐 Python | 📅 2023-12-13 — BERT-based foundation model pretrained on large-scale scRNA-seq data for cell type annotation.
* [UCE](https://github.com/snap-stanford/UCE) ⭐ 345 | 🐛 3 | 🌐 Python | 📅 2026-07-08 — Universal Cell Embeddings: zero-shot single-cell embedding model trained on 36M cells across species, tissues, and assays without fine-tuning.
* [SATURN](https://github.com/snap-stanford/SATURN) ⭐ 175 | 🐛 4 | 🌐 Jupyter Notebook | 📅 2024-07-03 — Transformer-based model integrating gene expression and protein sequences via a protein language model to learn unified multi-species cell embeddings.
* [CellFM](https://github.com/biomed-AI/CellFM) ⭐ 115 | 🐛 11 | 🌐 Jupyter Notebook | 📅 2026-09-07 — 800M-parameter single-cell foundation model pretrained on transcriptomics from 100 million human cells for annotation, integration, gene-function, and perturbation tasks.
* [CellPLM](https://github.com/OmicsML/CellPLM) ⭐ 107 | 🐛 10 | 🌐 Jupyter Notebook | 📅 2024-03-28 — Cell pre-trained language model with inter-cell transformer architecture for diverse single-cell analysis tasks.
* [BulkFormer](https://github.com/KangBoming/BulkFormer) ⭐ 85 | 🐛 7 | 🌐 Jupyter Notebook | 📅 2026-07-03 — Foundation model for bulk RNA-seq data; learns general transcriptomic representations.
* [scPRINT-2](https://github.com/cantinilab/scPRINT-2) ⭐ 39 | 🐛 2 | 🌐 Jupyter Notebook | 📅 2026-09-26 — Next-generation single-cell foundation model pretrained on 350M+ cells across 22K+ datasets and 16 species for embeddings, denoising, annotation, gene-network inference, and cross-species transfer.
* [CancerFoundation](https://github.com/BoevaLab/CancerFoundation) ⭐ 32 | 🐛 1 | 🌐 Jupyter Notebook | 📅 2025-09-12 — Single-cell RNA-seq foundation model trained exclusively on a curated dataset of malignant cells to learn cancer-specific embeddings.
* [Geneformer](https://huggingface.co/ctheodoris/Geneformer) — Context-aware, attention-based deep learning model pretrained on a large corpus of single-cell transcriptomes.

##### Spatial Foundation Models

* [UNI](https://github.com/mahmoodlab/UNI) ⭐ 785 | 🐛 32 | 🌐 Jupyter Notebook | 📅 2025-03-26 — General-purpose self-supervised pathology foundation model trained on 100K+ whole-slide images for diverse computational pathology tasks.
* [GigaPath](https://github.com/prov-gigapath/prov-gigapath) ⭐ 639 | 🐛 74 | 🌐 Python | 📅 2026-08-07 — Slide-level digital pathology foundation model pretrained on 1.3 billion pathology image tokens from whole-slide images.
* [CONCH](https://github.com/mahmoodlab/CONCH) ⭐ 535 | 🐛 16 | 🌐 Python | 📅 2025-03-26 — Vision-language foundation model for computational pathology trained with contrastive captioning on pathology image–text pairs.
* [Nicheformer](https://github.com/theislab/nicheformer) ⭐ 175 | 🐛 24 | 🌐 Jupyter Notebook | 📅 2025-11-23 — Foundation model for single-cell and spatial omics using a transformer architecture with positional embeddings to encode spatial cell information.
* [scGPT-spatial](https://github.com/bowang-lab/scGPT-spatial) ⭐ 142 | 🐛 11 | 🌐 Jupyter Notebook | 📅 2025-02-13 — Extension of scGPT for spatial transcriptomics with continual pretraining and a mixture-of-experts decoder for spatial gene expression analysis.
* [DeepSpot](https://github.com/ratschlab/DeepSpot) ⭐ 101 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-10-05 — Deep learning model predicting spatial transcriptomics from H\&E images at spot and single-cell resolution.
* [DeepSpot-M](https://github.com/ratschlab/DeepSpotM) ⭐ 58 | 🐛 2 | 🌐 Python | 📅 2026-09-04 — Multimodal foundation model for transcriptome-wide virtual spatial transcriptomics from histology.
* [AESTETIK](https://github.com/ratschlab/aestetik) ⭐ 28 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-18 — Autoencoder for spatial transcriptomics representation learning using topology and histology image knowledge.
* [DeepSpot2Cell](https://github.com/ratschlab/DeepSpot2Cell) ⭐ 21 | 🐛 0 | 🌐 Python | 📅 2026-10-05 — Predicts virtual single-cell spatial transcriptomics from H\&E using spot-level supervision (NeurIPS 2025 Imageomics).
* [Phikon](https://huggingface.co/owkin/phikon) — ViT-based pathology foundation model pretrained with iBOT self-supervision on TCGA whole-slide images.

##### Pathology Foundation Models

* [TITAN](https://github.com/mahmoodlab/TITAN) ⭐ 371 | 🐛 5 | 🌐 Python | 📅 2025-12-13 — Multimodal whole-slide pathology foundation model that combines image and language supervision for slide-level representation and zero-shot analysis.
* [GenBio-PathFM](https://github.com/genbio-ai/genbio-pathfm) ⭐ 41 | 🐛 1 | 🌐 Python | 📅 2026-04-09 — 1.1B-parameter histopathology foundation model trained on public data using morphology-aware curation and dual-stage JEPA+DINO learning.
* [Virchow2](https://huggingface.co/paige-ai/Virchow2) — 632M-parameter pathology vision transformer pretrained on 3.1M whole-slide images with mixed-magnification self-supervision.
* [H-Optimus-0](https://huggingface.co/bioptimus/H-optimus-0) — 1.1B-parameter histopathology foundation model trained with self-supervised learning on a large multi-center slide corpus.
* [H-Optimus-1](https://huggingface.co/bioptimus/H-optimus-1) — 1.1B-parameter pathology foundation model trained on billions of histology images from more than one million slides and 800K+ patients.
* [UNI2-h](https://huggingface.co/MahmoodLab/UNI2-h) — Billion-parameter histopathology vision foundation model for tile-level feature extraction and downstream computational pathology tasks.
* [Phikon-v2](https://huggingface.co/owkin/phikon-v2) — Updated pathology foundation model for general-purpose histology feature extraction and transfer learning.

##### Multi-Omics Foundation Models

* [totalVI](https://github.com/scverse/scvi-tools) ⭐ 1,701 | 🐛 33 | 🌐 Python | 📅 2026-10-06 — Probabilistic framework for joint analysis of paired scRNA-seq and protein (CITE-seq) data enabling multi-modal cell state representation across single-cell datasets.
* [MultiVI](https://github.com/scverse/scvi-tools) ⭐ 1,701 | 🐛 33 | 🌐 Python | 📅 2026-10-06 — Multi-modal variational autoencoder for integrating paired and unpaired single-cell RNA-seq and ATAC-seq measurements into a unified latent space.
* [GLUE](https://github.com/gao-lab/GLUE) ⭐ 481 | 🐛 26 | 🌐 Python | 📅 2026-02-09 — Graph-Linked Unified Embedding framework for unpaired single-cell multi-omics data integration across RNA, ATAC, methylation, and protein modalities.
* [MOFA+](https://github.com/bioFAM/MOFA2) ⭐ 427 | 🐛 66 | 🌐 R | 📅 2026-09-10 — Multi-Omics Factor Analysis framework identifying shared axes of variation across bulk and single-cell datasets including RNA, ATAC, proteomics, methylation, and copy number.
* [GeneCompass](https://github.com/xCompass-AI/GeneCompass) ⭐ 124 | 🐛 20 | 🌐 Jupyter Notebook | 📅 2026-09-04 — Large-scale foundation model integrating DNA regulatory sequences and single-cell transcriptomics from 120M+ cells across multiple species for gene regulation prediction.
* [MIDAS](https://github.com/labomics/midas) ⭐ 72 | 🐛 0 | 🌐 Python | 📅 2026-05-10 — Mosaic integration and differential accessibility model for single-cell multi-omics that handles arbitrary missing-modality combinations across transcriptomics, chromatin accessibility, and proteomics.
* [MIRA](https://github.com/cistrome/MIRA) ⭐ 70 | 🐛 23 | 🌐 HTML | 📅 2025-07-08 — Probabilistic multimodal topic model jointly modeling single-cell transcriptomics and chromatin accessibility for regulatory network inference.
* [scMulan](https://github.com/SuperBianC/scMulan) ⭐ 63 | 🐛 13 | 🌐 Jupyter Notebook | 📅 2024-05-30 — Single-cell multi-omic language model pretrained on \~10M cells spanning transcriptomics, epigenomics, and proteomics for cross-omics transfer tasks.
* [BABEL](https://github.com/wukevin/babel) ⭐ 53 | 🐛 8 | 🌐 Jupyter Notebook | 📅 2023-07-17 — Cross-modality translation model enabling prediction between scRNA-seq and scATAC-seq profiles without requiring paired single-cell measurements.
* [UnitedNet](https://github.com/LiuLab-Bioelectronics-Harvard/UnitedNet) ⭐ 53 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2024-03-31 — Interpretable multi-task deep neural network for single-cell multi-omics integration spanning transcriptomics, chromatin accessibility, and proteomics.
* [Concerto](https://github.com/melobio/Concerto-reproducibility) ⭐ 41 | 🐛 2 | 🌐 Jupyter Notebook | 📅 2022-12-29 — Contrastive self-supervised learning framework for single-cell multimodal data integration, batch correction, and reference-query mapping.
* [Multigrate](https://github.com/theislab/multigrate) ⭐ 35 | 🐛 4 | 🌐 Python | 📅 2026-10-05 — Asymmetric multi-omics variational autoencoder for integrating single-cell data across RNA, ATAC, and protein modalities with missing-modality support.
* [scButterfly](https://github.com/BioX-NKU/scButterfly) ⭐ 30 | 🐛 10 | 🌐 Python | 📅 2024-07-01 — Dual-aligned variational autoencoder for single-cell cross-modality translation between paired and unpaired multiomics data.
* [JAMIE](https://github.com/Oafish1/JAMIE) ⭐ 17 | 🐛 0 | 🌐 Python | 📅 2025-09-11 — Joint variational autoencoder for multimodal single-cell data imputation and embedding.
* [scPair](https://github.com/quon-titative-biology/scPair) ⭐ 11 | 🐛 1 | 🌐 Python | 📅 2025-09-08 — Bidirectional feedforward network for single-cell multimodal analysis with cross-modality prediction leveraging single-cell atlases.
* [SpatialGlue](https://github.com/zhanglabtools/SpatialGlue) — Graph attention network for spatial multi-omics integration jointly embedding spatial transcriptomics with chromatin accessibility or proteomics.

##### Domain Alignment

* [scArches](https://github.com/theislab/scarches) ⭐ 412 | 🐛 69 | 🌐 Jupyter Notebook | 📅 2026-06-26 — Transfer learning framework for mapping new single-cell datasets onto pre-trained reference atlases across batches, conditions, and modalities.
* [TOSICA](https://github.com/JackieHanlaopo/TOSICA) — Transformer-based framework for one-stop interpretable cell-type annotation supporting cross-dataset and cross-species transfer.

#### Compound Foundation Models

##### Compound Embedding

* [Uni-Mol](https://github.com/deepmodeling/Uni-Mol) ⭐ 1,166 | 🐛 113 | 🌐 Python | 📅 2025-05-29 — 3D molecular pretraining framework for universal representation learning on molecules and protein pockets.
* [Uni-Mol2](https://github.com/deepmodeling/Uni-Mol/tree/main/unimol2) ⭐ 1,166 | 🐛 113 | 🌐 Python | 📅 2025-05-29 — Scaled molecular pretraining model using atomic, graph, and 3D geometry features, with models up to 1.1B parameters pretrained on 800M conformations.
* [ChemBERTa-2](https://github.com/seyonechithrananda/bert-loves-chemistry) ⭐ 501 | 🐛 10 | 🌐 Jupyter Notebook | 📅 2024-10-27 — RoBERTa-based molecular language model pretrained on SMILES for small-molecule representation learning.
* [MolFormer](https://github.com/IBM/molformer) ⭐ 415 | 🐛 15 | 🌐 Jupyter Notebook | 📅 2025-09-17 — Linear attention transformer pretrained on millions of SMILES strings for efficient molecular embeddings.
* [GROVER](https://github.com/tencent-ailab/grover) ⭐ 395 | 🐛 19 | 🌐 Python | 📅 2026-02-25 — Self-supervised graph transformer for large-scale molecular representation learning from unlabeled compounds.
* [Mol2Vec](https://github.com/samoturk/mol2vec) ⚠️ Archived — Unsupervised molecular embedding method inspired by Word2Vec for learning vector representations of chemical substructures.
* [ChemFM](https://github.com/TheLuoFengLab/ChemFM) ⭐ 87 | 🐛 0 | 🌐 Python | 📅 2025-06-19 — 1B/3B-parameter chemical language model pretrained on 178M molecules for molecular representation, property prediction, generation, and synthesis tasks.

#### Protein Foundation Models

##### Pre-trained Embedding

* [Evolutionary Scale Modeling (ESM)](https://github.com/facebookresearch/esm) ⚠️ Archived — Protein embeddings.
* [ESM Cambrian (ESM C)](https://github.com/Biohub/esm) ⭐ 2,983 | 🐛 81 | 🌐 Jupyter Notebook | 📅 2026-09-16 — Protein representation foundation-model family designed as an efficient next-generation successor to ESM2, spanning 300M to multi-billion-parameter models.
* [ProtTrans](https://github.com/agemagician/ProtTrans) ⭐ 1,326 | 🐛 21 | 🌐 Jupyter Notebook | 📅 2025-05-22 — Suite of protein language models (ProtBERT, ProtT5, ProtXLNet) trained on billions of protein sequences from UniRef and BFD.
* [ProGen2](https://github.com/salesforce/progen) ⭐ 705 | 🐛 40 | 🌐 Python | 📅 2026-06-02 — Protein language model trained on diverse protein families for sequence generation and fitness prediction.
* [Ankh](https://github.com/agemagician/Ankh) ⭐ 250 | 🐛 11 | 🌐 Python | 📅 2025-06-16 — Efficient protein language model optimized for downstream prediction tasks including secondary structure, localization, and function annotation.

##### Protein Structure Prediction and Design

* [AlphaFold3](https://github.com/google-deepmind/alphafold3) ⭐ 8,611 | 🐛 28 | 🌐 Python | 📅 2026-10-06 — Predicts structures of proteins, nucleic acids, small molecules, and their complexes.
* [Boltz-1](https://github.com/jwohlwend/boltz) ⭐ 4,235 | 🐛 132 | 🌐 Python | 📅 2026-05-29 — Open-source all-atom biomolecular structure prediction model for proteins, nucleic acids, small molecules, and their complexes achieving AlphaFold3-level accuracy.
* [Boltz-2](https://github.com/jwohlwend/boltz) ⭐ 4,235 | 🐛 132 | 🌐 Python | 📅 2026-05-29 — Biomolecular foundation model jointly predicting complex structures and binding affinities for protein–ligand interaction modeling and virtual screening.
* [ESMFold](https://github.com/facebookresearch/esm) ⚠️ Archived — Fast protein structure prediction using language model embeddings.
* [OpenFold](https://github.com/aqlaboratory/openfold) ⭐ 3,435 | 🐛 246 | 🌐 Python | 📅 2025-12-16 — Trainable, memory-efficient open-source reproduction of AlphaFold2 enabling custom protein structure prediction workflows.
* [RFdiffusion](https://github.com/RosettaCommons/RFdiffusion) ⭐ 3,076 | 🐛 245 | 🌐 Python | 📅 2026-07-15 — Generative model for protein backbone design using diffusion.
* [ESM3](https://github.com/evolutionaryscale/esm) ⭐ 2,983 | 🐛 81 | 🌐 Jupyter Notebook | 📅 2026-09-16 — Multimodal protein language model that jointly reasons over sequence, structure, and function for generative protein design and engineering.
* [RoseTTAFold](https://github.com/RosettaCommons/RoseTTAFold) ⭐ 2,271 | 🐛 99 | 🌐 Python | 📅 2024-02-15 — Three-track neural network for protein structure prediction.
* [Protenix](https://github.com/bytedance/Protenix) ⭐ 2,068 | 🐛 126 | 🌐 Python | 📅 2026-09-21 — Trainable biomolecular structure-prediction framework for proteins, nucleic acids, ligands, and complexes with open training and inference pipelines.
* [Chai-1](https://github.com/chaidiscovery/chai-lab) ⭐ 2,001 | 🐛 98 | 🌐 Python | 📅 2026-06-30 — Unified molecular structure prediction model covering proteins, nucleic acids, small molecules, and complexes.
* [ProteinMPNN](https://github.com/dauparas/ProteinMPNN) ⭐ 1,867 | 🐛 89 | 🌐 Jupyter Notebook | 📅 2024-08-14 — Deep learning model for protein sequence design given backbone structure.
* [EvoDiff](https://github.com/microsoft/evodiff) ⭐ 686 | 🐛 14 | 🌐 Python | 📅 2026-01-15 — Discrete diffusion framework for protein sequence generation trained on evolutionary-scale data, supporting unconditional generation, disordered region design, and functional motif scaffolding. \[ [paper-2023](https://www.biorxiv.org/content/10.1101/2023.09.11.556673v1) ]
* [OmegaFold](https://github.com/HeliXonProtein/OmegaFold) ⭐ 627 | 🐛 49 | 🌐 Python | 📅 2022-12-12 — High-resolution de novo protein structure prediction from sequence.
* [SaProt](https://github.com/westlake-reup/SaProt) — Structure-aware protein language model using structure-aware tokens that encode both sequence and backbone geometry for improved function prediction.

#### Multi-Modal Foundation Models

* [CHIEF](https://github.com/hms-dbmi/CHIEF) ⭐ 719 | 🐛 49 | 🌐 Python | 📅 2026-01-08 — Clinical Histopathology Imaging Evaluation Foundation model integrating histology images and clinical context for pan-cancer analysis.
* [PLIP](https://github.com/PathologyFoundation/plip) ⭐ 380 | 🐛 6 | 🌐 Python | 📅 2023-09-20 — Vision-language foundation model for pathology trained with contrastive learning on pathology image–text pairs for image classification and text-to-image retrieval.
* [PathomicFusion](https://github.com/mahmoodlab/PathomicFusion) ⭐ 327 | 🐛 10 | 🌐 Jupyter Notebook | 📅 2022-08-22 — Integrated framework fusing histopathology and genomic features via CNN, GNN, and attention gating for cancer diagnosis and prognosis.
* [PORPOISE](https://github.com/mahmoodlab/PORPOISE) ⭐ 252 | 🐛 8 | 🌐 Jupyter Notebook | 📅 2023-02-07 — Pan-cancer integrative histology-genomic analysis framework using multimodal deep learning for patient stratification.
* [MUSK](https://github.com/lilab-stanford/MUSK) ⭐ 247 | 🐛 4 | 🌐 Python | 📅 2025-10-26 — Vision-language foundation model for precision oncology analyzing multimodal paired text and pathology image data for biomarker prediction and retrieval.
* [TOAD](https://github.com/mahmoodlab/TOAD) ⭐ 186 | 🐛 8 | 🌐 Python | 📅 2021-11-01 — Tumor Origin Assessment via Deep-learning; weakly-supervised multi-task model predicting cancer primary origin from H\&E whole-slide images.
* [BiomedCLIP](https://huggingface.co/microsoft/BiomedCLIP-PubMedBERT_256-vit_g_14) — CLIP-based vision-language foundation model for biomedical images and text trained on PubMed figure–caption pairs.
* [Virchow](https://huggingface.co/paige-ai/Virchow) — Million-slide digital pathology foundation model using a vision transformer and self-supervised distillation for tile-level pathology image representation.

#### Cancer Genome Foundation Models

* [TESSERA](https://github.com/JW-Sidhom-Lab/tessera) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-07-30 — Cancer-genome foundation model jointly pretrained on somatic SNVs and copy-number alterations from TCGA using masked reconstruction and cross-modal contrastive learning.
* [MutationProjector](https://doi.org/10.1101/2025.09.08.674723) — Pan-cancer genotype foundation model trained on mutations and copy-number alterations from >30K tumors for clinical representation learning.

#### Single-Cell Epigenomics Foundation Models

* [EpiAgent](https://github.com/xy-chen16/EpiAgent) ⭐ 72 | 🐛 3 | 🌐 Python | 📅 2026-06-03 — scATAC-seq foundation model pretrained on \~5M cells and >35B tokens for representation learning, annotation, imputation, perturbation prediction, and in-silico cCRE knockout.
* [scDNAm-GPT](https://github.com/ChaoqiLiang/scDNAm-GPM) ⭐ 20 | 🐛 2 | 🌐 Jupyter Notebook | 📅 2026-08-07 — Foundation model for single-cell whole-genome bisulfite sequencing with whole-genome context modeling at single-CpG resolution.
* [ChromFound](https://github.com/SAIS-LifeScience/ChromFound) ⭐ 6 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-04-25 — Genome-aware scATAC-seq foundation model pretrained on 1.97M cells across tissues and disease contexts for zero-shot cell representations, annotation, and cross-omics prediction.
* [SCARF](https://doi.org/10.1101/2025.04.07.647689) — Single-cell RNA+ATAC foundation model pretrained on >2.7M cells for multimodal representation, matching, cross-omics translation, and few-shot annotation.
* [EpiFoundation](https://doi.org/10.1101/2025.02.05.636688) — Foundation model for scATAC-seq using peak-to-gene aligned pretraining for cell representation, annotation, batch correction, and gene-expression prediction.
* [Atacformer](https://doi.org/10.1101/2025.11.03.685753) — Transformer foundation model for scATAC-seq that learns embeddings of cis-regulatory elements for clustering, annotation, and reference mapping.
* [CLM-X](https://doi.org/10.64898/2026.02.17.704943) — Multi-way Transformer foundation model jointly handling RNA-only, ATAC-only, and paired RNA–ATAC single-cell inputs for integration, translation, annotation, and perturbation prediction.

#### Other Omics Foundation Models

* [VirTues](https://github.com/bunnelab/virtues) ⭐ 157 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2026-09-07 — Spatial-proteomics foundation model learning marker-aware representations across proteins, cells, niches, and tissues from multiplexed imaging.
* [CpGPT](https://github.com/lucascamillomd/CpGPT) ⭐ 83 | 🐛 6 | 🌐 Python | 📅 2026-09-05 — DNA methylation foundation model pretrained on >150K samples for zero-shot imputation, array conversion, reference mapping, and downstream phenotype prediction.
* [MethylGPT](https://github.com/albert-ying/MethylGPT) ⭐ 67 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2026-03-05 — Transformer foundation model for DNA methylation pretrained on >150K human methylomes across thousands of datasets, with 3M/7M/15M parameter variants.
* [OmicsFM](https://github.com/CompOmics/OmicsFM) ⭐ 6 | 🐛 0 | 🌐 Python | 📅 2026-09-10 — Modality-agnostic molecular-expression foundation model with matched proteomics, bulk-transcriptomics, and single-cell-transcriptomics checkpoints.
* [Casanovo Foundation](https://github.com/Noble-Lab/casanovo-tl) ⭐ 1 | 🐛 1 | 🌐 Jupyter Notebook | 📅 2026-08-19 — Tandem mass-spectrometry proteomics foundation model that reuses a pretrained Casanovo spectrum encoder for spectrum quality, chimericity, and post-translational-modification prediction.
* [CAPTAIN](https://doi.org/10.1038/s41467-026-72882-y) — Multimodal foundation model pretrained on co-assayed single-cell RNA and protein for joint representation learning and cross-modal downstream tasks.
* [HiCFoundation](https://doi.org/10.1038/s41592-026-03097-8) — Hi-C foundation model pretrained on large-scale chromatin-contact maps for 3D-genome analysis, epigenomic prediction, and single-cell Hi-C adaptation.

#### RNA Foundation Models

* [RNA-FM](https://github.com/ml4bio/RNA-FM) ⭐ 392 | 🐛 18 | 🌐 Jupyter Notebook | 📅 2025-05-27 — General-purpose RNA foundation model pretrained on large-scale RNA sequences for structural and functional representation learning.
* [RiNALMo](https://github.com/lbcb-sci/RiNALMo) ⭐ 177 | 🐛 1 | 🌐 Python | 📅 2026-05-04 — RNA language-model family pretrained on tens of millions of RNA sequences for secondary-structure and functional prediction tasks.

#### Genomics Foundation Models

* [Enformer](https://github.com/deepmind/deepmind-research/tree/master/enformer) ⭐ 15,215 | 🐛 359 | 🌐 Jupyter Notebook | 📅 2026-06-17 — Transformer model predicting gene expression from DNA sequence.
* [Evo 2](https://github.com/arcinstitute/evo2) ⭐ 4,243 | 🐛 56 | 🌐 Jupyter Notebook | 📅 2026-06-19 — Genome foundation model trained on 9 trillion DNA base pairs across all domains of life with a 1M-token context window and single-nucleotide resolution.
* [AlphaGenome](https://github.com/google-deepmind/alphagenome) ⭐ 2,177 | 🐛 11 | 🌐 Python | 📅 2026-09-30 — Long-context DNA model predicting multimodal regulatory outputs including expression, splicing, chromatin features, and contact maps at near base-pair resolution.
* [Evo](https://github.com/evo-design/evo) ⭐ 1,574 | 🐛 41 | 🌐 Python | 📅 2026-03-20 — Long-context genomic foundation model (up to 1M tokens).
* [Nucleotide Transformer](https://github.com/instadeepai/nucleotide-transformer) ⭐ 922 | 🐛 14 | 🌐 Jupyter Notebook | 📅 2026-02-24 — Foundation model for genomic sequences across multiple species.
* [HyenaDNA](https://github.com/HazyResearch/hyena-dna) ⭐ 809 | 🐛 38 | 🌐 Assembly | 📅 2025-04-22 — Long-range genomic foundation model handling sequences up to 1M tokens with sub-quadratic attention.
* [DNABERT](https://github.com/jerryji1993/DNABERT) ⭐ 780 | 🐛 73 | 🌐 Python | 📅 2026-01-22 — Pre-trained bidirectional encoder for DNA sequence analysis.
* [DNABERT-2](https://github.com/Zhihan1996/DNABERT_2) ⭐ 517 | 🐛 52 | 🌐 Shell | 📅 2026-01-01 — Improved genome foundation model with efficient tokenization.
* [Basenji](https://github.com/calico/basenji) ⭐ 475 | 🐛 87 | 🌐 Python | 📅 2026-01-15 — Sequential regulatory activity prediction from DNA sequences.
* [GPN (Genomic Pre-trained Network)](https://github.com/songlab-cal/gpn) ⭐ 384 | 🐛 8 | 🌐 Jupyter Notebook | 📅 2026-10-01 — Masked language model for DNA sequences enabling zero-shot variant effect prediction without requiring functional annotations.
* [Borzoi](https://github.com/calico/borzoi) ⭐ 267 | 🐛 2 | 🌐 Python | 📅 2026-09-30 — Extended successor to Enformer for predicting RNA-seq coverage from long genomic sequence windows (524 kb) with improved resolution.
* [Caduceus](https://github.com/kuleshov-group/caduceus) ⭐ 252 | 🐛 10 | 🌐 Python | 📅 2026-03-18 — Bidirectional equivariant long-range DNA sequence model based on Mamba.
* [modernGENA](https://github.com/AIRI-Institute/GENA_LM) ⭐ 232 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2026-10-05 — ModernBERT-style DNA foundation-model family pretrained on hundreds of vertebrate genome assemblies for efficient long-sequence regulatory modeling.
* [Sei](https://github.com/FunctionLab/sei-framework) ⭐ 118 | 🐛 13 | 🌐 Python | 📅 2022-12-20 — Sequence-to-function framework learning a genome-wide regulatory activity code from DNA sequences for variant effect prediction.
* [DeepSEA](http://deepsea.princeton.edu/) — Deep learning framework for predicting chromatin effects of sequence alterations with single-nucleotide sensitivity across thousands of chromatin features.

***

## Citation

If you use this list in papers, slides, or documentation, please cite this repository via [`CITATION.cff`](./CITATION.cff) (also available through GitHub's **Cite this repository** button).

## Curation Criteria (Strict)

To keep quality high, additions should meet all of the following:

* The resource is trustworthy and relevant to computational biology.
* The resource has clear value to the scope and audience of this collection; highly specialized resources with limited relevance beyond a narrow application context may be declined even when technically sound.
* The primary link points to an official source (official docs, organization site, maintained repository, or official dataset page).
* The resource has evidence of technical substance: ideally a peer-reviewed paper; at minimum a preprint or official technical documentation.
* The description is factual and concise (no marketing copy).
* Duplicate or near-duplicate entries should be avoided.

We generally do **not** accept entries that are only promotional pages, personal opinion posts, or generic blog posts without technical references.

## Update & Link Rot Policy

* Link validity is monitored by the [Link Check workflow](./.github/workflows/link-check.yml).
* If a link repeatedly fails, maintainers may replace it with an official mirror/canonical URL or remove the entry until a stable URL is available.
* Contributions fixing broken links are welcome and encouraged.

## Data Schema & Contribution Workflow

* Data schema reference: [`docs/data/SCHEMA.md`](./docs/data/SCHEMA.md).
* Source-of-truth workflow:
  1. Edit/add resources in `README.md`.
  2. Regenerate machine-readable artifacts:
     * `python scripts/sync_resources_from_readme.py`
     * `python scripts/build_resources.py`
  3. Commit updated data files (`data/resources.yml`, `data/resources.json`, `data/resources.csv`, `docs/data/resources.json`) with your README change.
* Contribution guide: [`contributing.md`](./contributing.md).

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-10-06._

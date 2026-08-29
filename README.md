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

* [PrimeKG](https://github.com/mims-harvard/PrimeKG) ⭐ 817 | 🐛 7 | 🌐 Jupyter Notebook | 📅 2026-06-30 — Multi-modal precision medicine knowledge graph integrating clinical, genetic, and drug data.
* [DRKG](https://github.com/gnn4dr/DRKG) ⭐ 705 | 🐛 22 | 🌐 Jupyter Notebook | 📅 2022-04-19 — Large-scale biological knowledge graph for drug discovery.
* [Hetionet](https://github.com/hetio/hetionet) ⭐ 360 | 🐛 14 | 🌐 HTML | 📅 2023-04-03 — Heterogeneous network integrating genes, diseases, drugs, pathways, and more.
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

* [MOSES](https://github.com/molecularsets/moses) ⭐ 988 | 🐛 31 | 🌐 Python | 📅 2024-07-08 — Benchmarking platform for molecular generation models.
* [TAPE (Tasks Assessing Protein Embeddings)](https://github.com/songlab-cal/tape) ⭐ 744 | 🐛 30 | 🌐 Python | 📅 2022-12-11 — Benchmark suite of five biologically meaningful semi-supervised learning tasks for evaluating protein representations.
* [GuacaMol](https://github.com/BenevolentAI/guacamol) ⭐ 531 | 🐛 13 | 🌐 Python | 📅 2024-02-11 — Benchmark suite for generative molecular design models.
* [ProteinGym](https://github.com/OATML-Markslab/ProteinGym) ⭐ 467 | 🐛 32 | 🌐 HTML | 📅 2026-03-25 — Large-scale benchmark of deep mutational scanning assays for evaluating protein fitness landscape models.
* [scIB (Single-cell Integration Benchmarks)](https://github.com/theislab/scib) ⭐ 429 | 🐛 43 | 🌐 Python | 📅 2026-04-27 — Comprehensive benchmarking framework for single-cell data integration methods.
* [JUMP Cell Painting Datasets](https://github.com/jump-cellpainting/datasets) ⭐ 189 | 🐛 26 | 🌐 Shell | 📅 2026-08-24 — Consortium-scale cell imaging perturbation datasets (chemical and genetic) for phenotypic profiling and drug discovery research.
* [scPerturb](https://github.com/sanderlab/scPerturb) ⭐ 187 | 🐛 13 | 🌐 Jupyter Notebook | 📅 2025-02-25 — Curated and continuously updated single-cell perturbation data resource spanning CRISPR and drug perturbation studies.
* [OpenBioLink](https://github.com/OpenBioLink/OpenBioLink) ⭐ 163 | 🐛 11 | 🌐 Python | 📅 2024-05-03 — Benchmark datasets for biological knowledge graph completion.
* [FLIP (Fitness Landscape Inference for Proteins)](https://github.com/J-SNACKKB/FLIP) ⭐ 140 | 🐛 3 | 🌐 Jupyter Notebook | 📅 2026-04-23 — Benchmark collection of protein fitness landscape datasets for evaluating protein ML models.
* [Bento](https://github.com/LigandPro/Bento) ⭐ 13 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-03-04 — Protein-ligand docking benchmark covering rigid, flexible, de novo, blind, induced-fit, and covalent docking tasks.
* [1000 Genomes Project](https://www.internationalgenome.org/) — Reference panel of human genetic variation from 2,504 individuals across 26 populations.
* [BACE](https://www.kaggle.com/datasets/gokturkkoch/bace) — Binary classification and regression dataset for β-secretase 1 (BACE-1) inhibitor binding affinity.
* [BEAT AML](https://biodev.github.io/BeatAML2/) — Functional ex vivo drug sensitivity measurements paired with genomics for acute myeloid leukemia.
* [BindingDB Curated Sets](https://www.bindingdb.org/rwd/bind/chemsearch/marvin/SDFdownload.jsp?all_download=yes) — Curated binding affinity datasets for protein–ligand interaction benchmarking.
* [Cancer Therapeutics Response Portal (CTRP)](https://portals.broadinstitute.org/ctrp/) — Drug sensitivity profiles across \~900 cancer cell lines for >400 compounds.
* [ClinTox](https://tdcommons.ai/single_pred_tasks/tox/#clintox) — Clinical toxicity dataset contrasting FDA-approved drugs with those that failed clinical trials due to toxicity.
* [CPTAC (Clinical Proteomic Tumor Analysis Consortium)](https://proteomics.cancer.gov/programs/cptac) — Multi-omic proteogenomic datasets for multiple cancer types linking proteomics with genomics.
* [CrossDocked2020](https://arxiv.org/abs/2001.01037) — Large-scale dataset for structure-based virtual screening.
* [DUD-E (Directory of Useful Decoys, Enhanced)](http://dude.docking.org/) — Structure-based virtual screening benchmark with active ligands and challenging decoy sets across diverse protein targets.
* [Genomics of Drug Sensitivity in Cancer (GDSC)](https://www.cancerrxgene.org/) — Drug sensitivity for \~1000 human cancer cell lines and hundreds of compounds.
* [LINCS L1000](https://lincsproject.org/LINCS/tools/workflows/find-the-best-place-to-obtain-the-lincs-l1000-data) — Gene expression profiles (978 landmark genes) for >20,000 chemical and genetic perturbations across cell lines.
* [MoleculeNet](http://moleculenet.ai/) — Benchmark datasets for molecular machine learning.
* [NCI60](https://dtp.cancer.gov/discovery_development/nci-60/) — Drug sensitivity benchmark across 60 diverse human cancer cell lines.
* [OGB (Open Graph Benchmark)](https://ogb.stanford.edu/) — Large-scale graph ML benchmark suite including biological datasets such as ogbl-ppa (protein-protein associations) and ogbg-molhiv.
* [PharmGKB](https://www.pharmgkb.org/) — Curated pharmacogenomics dataset linking genetic variants to drug response phenotypes across thousands of drugs.
* [PK-DB](https://pk-db.com/) — Open database of experimental pharmacokinetics (PK) and ADME data from clinical and preclinical studies.
* [PRISM](https://depmap.org/portal/prism/) — Cancer drug sensitivity profiling of >4,500 drugs across >900 cancer cell lines using pooled-cell-line barcoding.
* [QM9](https://figshare.com/collections/Quantum_chemistry_structures_and_properties_of_134_kilo_molecules/978904) — Quantum chemistry properties for 134K stable small organic molecules computed at DFT level.
* [SIDER (Side Effect Resource)](http://sideeffects.embl.de/) — Database of 1,430 approved drugs with their recorded adverse drug reactions across 27 system-organ classes.
* [Tabula Muris](https://tabula-muris.ds.czbiohub.org/) — Comprehensive single-cell atlas of 20 mouse organs and tissues, enabling cross-tissue and cross-species comparisons.
* [Tabula Sapiens](https://tabula-sapiens-portal.ds.czbiohub.org/) — Comprehensive human single-cell atlas of \~500K cells from 24 organs and tissues across multiple donors.
* [The Cancer Genome Atlas (TCGA)](https://www.cancer.gov/about-nci/organization/ccg/research/structural-genomics/tcga) — Comprehensive multi-omics (genomics, transcriptomics, proteomics, methylation) dataset for 33 cancer types across \~11,000 patients.
* [TCGA virtual spatial transcriptomics atlas](https://huggingface.co/datasets/ratschlab/TCGA_virtual_spatial_transcriptomics_atlas) — DeepSpot-M predicted transcriptome-wide ST for TCGA H\&E (FF + FFPE; 28,664 slides / 32 cancer types; gated). Paper: [DeepSpot-M](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1).
* [HEST Xenium virtual spatial transcriptomics](https://huggingface.co/datasets/ratschlab/HEST_Xenium_virtual_spatial_transcriptomics) — DeepSpot-M predicted transcriptome-wide ST for 59 HEST-1k 10x Xenium samples (\~13.3M cells) (gated). Paper: [DeepSpot-M](https://www.medrxiv.org/content/10.64898/2026.06.19.26356060v1).
* [Therapeutics Data Commons (TDC)](https://tdcommons.ai/) — Unified benchmark suite covering ADMET, drug-target interaction, drug response, and more.
* [Tox21](https://tripod.nih.gov/tox21/challenge/) — 12,707 compounds tested in 12 nuclear receptor and stress-response pathway biochemical assays for toxicity prediction.
* [UK Biobank](https://www.ukbiobank.ac.uk/) — Large-scale biomedical database of \~500K participants with genetic, imaging, and health data for population genetics and disease studies.

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

* [DeepChem](https://github.com/deepchem/deepchem) ⭐ 6,967 | 🐛 1,167 | 🌐 Python | 📅 2026-08-20 — Deep learning library for drug discovery, quantum chemistry, and materials science.
* [RDKit](https://github.com/rdkit/rdkit) ⭐ 3,570 | 🐛 72 | 🌐 HTML | 📅 2026-08-28 — Cheminformatics software & machine learning toolkit.
* [STAR](https://github.com/alexdobin/STAR) ⭐ 2,241 | 🐛 1,006 | 🌐 C | 📅 2025-03-18 — Ultrafast universal RNA-seq aligner with support for spliced alignment and single-cell quantification via STARsolo.
* [CellChat](https://github.com/sqjin/CellChat) ⚠️ Archived — Inference and analysis of cell-cell communication ligand-receptor networks from single-cell transcriptomics data.
* [Harmony](https://github.com/immunogenomics/harmony) ⭐ 670 | 🐛 84 | 🌐 R | 📅 2026-06-05 — Fast and scalable integration of single-cell data across datasets, conditions, technologies, and species.
* [Chemistry Development Kit](https://github.com/cdk/cdk) ⭐ 602 | 🐛 10 | 🌐 Java | 📅 2026-08-21 — Cheminformatics software & machine learning tools.
* [DoubletFinder](https://github.com/chris-mcginnis-ucsf/DoubletFinder) ⭐ 560 | 🐛 23 | 🌐 R | 📅 2025-03-21 — Machine learning approach for detecting multiplet (doublet) artifacts in single-cell RNA-seq data.
* [scVelo](https://github.com/theislab/scvelo) ⭐ 508 | 🐛 82 | 🌐 Python | 📅 2026-02-25 — RNA velocity estimation for single-cell transcriptomics, inferring the direction and speed of cell differentiation.
* [CellTypist](https://github.com/Teichlab/celltypist) ⭐ 502 | 🐛 48 | 🌐 Python | 📅 2026-05-22 — Automated cell type annotation for scRNA-seq.
* [SCENIC](https://github.com/aertslab/SCENIC) ⭐ 496 | 🐛 113 | 🌐 HTML | 📅 2024-04-05 — Single-cell regulatory network inference and clustering linking transcription factors to co-expressed gene modules.
* [Numbat](https://github.com/kharchenkolab/numbat) ⭐ 227 | 🐛 80 | 🌐 R | 📅 2026-02-04 — Haplotype-aware copy number variation inference from single-cell RNA-seq using hidden Markov models.
* [CellCharter](https://github.com/CSOgroup/cellcharter) ⭐ 189 | 🐛 17 | 🌐 Python | 📅 2026-08-24 — Identification and characterization of spatial cell niches from spatial transcriptomics using VAEs and Gaussian mixture models.
* [MOGONET](https://github.com/txWang/MOGONET) ⭐ 187 | 🐛 0 | 🌐 Python | 📅 2021-03-31 — Multi-omics graph convolutional network framework for patient classification and biomarker identification.
* [COMMOT](https://github.com/zcang/COMMOT) ⭐ 145 | 🐛 27 | 🌐 Python | 📅 2026-06-25 — Optimal transport-based framework for screening cell-cell communication in spatial transcriptomics.
* [LINGER](https://github.com/Durenlab/LINGER) ⭐ 135 | 🐛 54 | 🌐 Jupyter Notebook | 📅 2026-07-11 — Neural network for gene regulatory network inference from single-cell multiome (RNA+ATAC-seq) data with bulk data pretraining.
* [NCEM](https://github.com/theislab/ncem) ⭐ 121 | 🐛 34 | 🌐 Python | 📅 2024-01-15 — GNN-based model for learning intercellular communication from spatial graphs of cells.
* [CaSpER](https://github.com/akdess/CaSpER) ⭐ 92 | 🐛 41 | 🌐 R | 📅 2021-04-05 — CNV identification and visualization by integrative analysis of single-cell or bulk RNA-seq data.
* [TIGON](https://github.com/yutongo/TIGON) ⭐ 59 | 🐛 2 | 🌐 Jupyter Notebook | 📅 2025-03-23 — Neural optimal transport method for reconstructing growth and dynamic trajectories from single-cell transcriptomics.
* [STAGATE](https://github.com/RucDongLab/STAGATE) ⭐ 55 | 🐛 12 | 🌐 Python | 📅 2023-04-28 — Adaptive graph attention auto-encoder for spatial domain identification in spatial transcriptomics.
* [AutoZyme](https://github.com/ElliotXie/autozyme) ⭐ 49 | 🐛 1 | 🌐 Python | 📅 2026-08-16 — Autonomous agentic framework that speeds up bioinformatics software (e.g. Scanpy, Seurat) on CPUs while preserving the original results.
* [ChatSpatial](https://github.com/cafferychen777/ChatSpatial) ⭐ 44 | 🐛 13 | 🌐 Python | 📅 2026-08-15 — MCP server for spatial transcriptomics analysis via natural language.
* [DeepTalk](https://github.com/JiangBioLab/DeepTalk) ⭐ 30 | 🐛 9 | 🌐 Jupyter Notebook | 📅 2024-09-06 — Graph attention network for deciphering cell-cell communication from spatial transcriptomics data.
* [FlashDeconv](https://github.com/cafferychen777/flashdeconv) ⭐ 26 | 🐛 0 | 🌐 Python | 📅 2026-06-30 — High-performance spatial transcriptomics deconvolution (\~1M spots in \~3 min).
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
* [DeepAEG](https://github.com/zhejiangzhuque/DeepAEG) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2023-12-26 — GNN embedding + attention mechanism.
* [drGAT](https://github.com/inoue0426/drGAT) ⭐ 2 | 🐛 1 | 🌐 Jupyter Notebook | 📅 2026-02-27 — Attention-based model for drug response prediction with gene explainability.
* [DGDRP](https://github.com/minwoopak/heteronet) ⭐ 1 | 🐛 0 | 🌐 Python | 📅 2024-02-24 — Multi-view embedding neural network.
* [DeepDSC](https://ieeexplore-ieee-org.ezp2.lib.umn.edu/stamp/stamp.jsp?tp=\&arnumber=8723620\&tag=1) — Autoencoder + fully connected NN.
* [HiDRA](https://github.com/bsml320/HiDRA) — Hierarchical network model incorporating gene and pathway-level information for cancer drug response prediction.

#### Drug Perturbation

* [CellOT](https://github.com/bunnech/cellot) ⭐ 181 | 🐛 12 | 🌐 Python | 📅 2024-10-31 — Neural optimal transport framework for predicting single-cell responses to drug and genetic perturbations.
* [chemCPA](https://github.com/theislab/chemCPA) ⭐ 157 | 🐛 7 | 🌐 Jupyter Notebook | 📅 2025-02-06 — Compositional perturbation autoencoder for predicting single-cell transcriptional responses to unseen drug perturbations and dose combinations.
* [PRNet](https://github.com/Perturbation-Response-Prediction/PRnet) ⭐ 89 | 🐛 18 | 🌐 Jupyter Notebook | 📅 2024-12-13 — Deep generative model for predicting transcriptional responses to novel chemical perturbations for drug discovery.
* [CMonge](https://github.com/AI4SCR/conditional-monge-gap) ⭐ 22 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-10 — Conditional optimal transport model for generalizable single-cell perturbation response prediction across drugs and doses.
* [cycleCDR](https://github.com/hliulab/cycleCDR) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2024-01-24 — Interpretable cycle-consistency framework for modeling cellular responses to drug perturbations.

#### Drug Repurposing

* [DeepPurpose](https://github.com/kexinhuang12345/DeepPurpose) ⭐ 1,184 | 🐛 18 | 🌐 Jupyter Notebook | 📅 2024-06-10 — Deep learning library for drug repurposing.
* [TranSiGen](https://github.com/myzhengSIMM/TranSiGen) ⭐ 37 | 🐛 19 | 🌐 Jupyter Notebook | 📅 2025-01-21 — Dual-VAE architecture for ligand-based virtual screening, drug response prediction, and drug repurposing using chemical-induced transcriptional profiles.

#### Drug Target Interaction

* [GraphDTA](https://github.com/thinng/GraphDTA) ⭐ 307 | 🐛 2 | 🌐 Python | 📅 2021-04-13 — Graph neural network–based DTI prediction using molecular graphs.
* [DeepDTA](https://github.com/hkmztrk/DeepDTA) ⭐ 304 | 🐛 5 | 🌐 Python | 📅 2023-09-22 — Deep learning model using CNNs on protein sequences and drug SMILES.
* [MolTrans](https://github.com/kexinhuang12345/MolTrans) ⭐ 242 | 🐛 4 | 🌐 Jupyter Notebook | 📅 2022-07-15 — Transformer-based DTI model leveraging molecular substructures.
* [DTINet](https://github.com/luoyunan/DTINet) ⭐ 190 | 🐛 8 | 🌐 MATLAB | 📅 2022-10-30 — Network-based framework integrating heterogeneous biological data for DTI prediction.
* [DrugBAN](https://github.com/peizhenbai/DrugBAN) ⭐ 153 | 🐛 8 | 🌐 Python | 📅 2023-02-19 — Bilinear attention network for interpretable DTI prediction.
* [NeoDTI](https://github.com/FangpingWan/NeoDTI) ⭐ 78 | 🐛 3 | 🌐 Python | 📅 2021-05-13 — Library for drug-target interaction prediction.

#### Compound-Protein Interaction

* [TransformerCPI](https://github.com/lifanchen-simm/transformerCPI) ⭐ 160 | 🐛 1 | 🌐 Python | 📅 2022-06-30 — CPI prediction using Transformer.
* [MCPINN](https://github.com/mhlee0903/multi_channels_PINN) ⭐ 4 | 🐛 0 | 🌐 Python | 📅 2023-08-25 — Drug discovery via compound-protein interaction and machine learning.

#### Molecular Generation

* [DiffDock](https://github.com/gcorso/DiffDock) ⭐ 1,571 | 🐛 132 | 🌐 Python | 📅 2025-05-02 — Diffusion generative model for molecular docking, predicting the binding pose of small molecules to protein targets.
* [JTVAE](https://github.com/wengong-jin/icml18-jtnn) ⭐ 565 | 🐛 30 | 🌐 Python | 📅 2022-12-01 — Junction tree variational autoencoder for molecular graph generation that guarantees chemical validity via a hierarchical tree decomposition.
* [DiffSBDD](https://github.com/arneschneuing/DiffSBDD) ⭐ 529 | 🐛 30 | 🌐 Python | 📅 2025-06-25 — Equivariant diffusion model for structure-based drug design that generates molecules and binding conformations for protein targets.
* [Molecular Transformer](https://github.com/pschwllr/MolecularTransformer) ⭐ 429 | 🐛 3 | 🌐 Python | 📅 2022-04-18 — Sequence-to-sequence model for retrosynthesis prediction.
* [REINVENT](https://github.com/MolecularAI/Reinvent) ⚠️ Archived — Reinforcement learning for de novo drug design.
* [ReLeaSE](https://github.com/isayev/ReLeaSE) ⭐ 373 | 🐛 27 | 🌐 Jupyter Notebook | 📅 2021-12-08 — Deep reinforcement learning framework for de novo drug design combining a generative and predictive model.
* [TargetDiff](https://github.com/guanjq/targetdiff) ⭐ 347 | 🐛 13 | 🌐 Python | 📅 2024-01-10 — 3D equivariant diffusion model for structure-based drug design.
* [MolGPT](https://github.com/devalab/molgpt) ⭐ 176 | 🐛 22 | 🌐 Python | 📅 2023-07-15 — Transformer-based model for molecular generation.
* [Matcha](https://github.com/LigandPro/Matcha) ⭐ 34 | 🐛 2 | 🌐 Python | 📅 2026-05-14 — Multi-stage Riemannian flow matching model for physically valid molecular docking with scoring, pose filtering, and benchmarks.
* [PaccMannRL](https://github.com/PaccMann/paccmann_generator) ⭐ 11 | 🐛 0 | 🌐 Python | 📅 2024-05-22 — Reinforcement learning-based generative model for de novo hit-like anticancer molecule design from transcriptomic data.

### LLM for Biology

* [BioGPT](https://github.com/microsoft/BioGPT) ⭐ 4,490 | 🐛 75 | 🌐 Python | 📅 2024-07-25 — LLM for biomedical text generation.
* [ClawBio](https://github.com/ClawBio/ClawBio) ⭐ 1,120 | 🐛 30 | 🌐 Python | 📅 2026-08-29 — Bioinformatics-native AI agent skill library with local-first pharmacogenomics, ancestry PCA, semantic similarity, nutrigenomics, and metagenomics skills.
* [GeneGPT](https://github.com/ncbi/GeneGPT) ⭐ 431 | 🐛 0 | 🌐 Python | 📅 2025-05-08 — LLM for biomedical information, integrated with various APIs.
* [GenePT](https://github.com/yiqunchen/GenePT) ⭐ 324 | 🐛 17 | 🌐 Jupyter Notebook | 📅 2024-03-18 — Foundation LLM for single-cell data.
* [MolT5](https://github.com/blender-nlp/MolT5) ⭐ 196 | 🐛 0 | 🌐 Python | 📅 2023-09-15 — Language model for molecular tasks bridging text and SMILES, enabling molecule captioning and text-driven molecule generation.
* [ChatDrug](https://github.com/chao1224/ChatDrug) ⭐ 162 | 🐛 0 | 🌐 Python | 📅 2024-05-28 — LLM-based conversational pipeline for drug discovery, using natural language prompts for iterative drug editing and optimization.
* [scPRINT](https://github.com/cantinilab/scPRINT) ⭐ 157 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-11 — Pretrained on 50M cells for scRNA-seq denoising & zero imputation.
* [CASSIA](https://github.com/ElliotXie/CASSIA) ⭐ 103 | 🐛 3 | 🌐 Python | 📅 2026-06-21 — Multi-agent LLM for reference-free, interpretable cell-type annotation of single-cell RNA-seq data, with dedicated annotation, validation, scoring, and reporting agents.
* [AI4Chem/ChemLLM-7B-Chat](https://huggingface.co/AI4Chem/ChemLLM-7B-Chat) — LLM for chemical & molecular science.
* [BioMedLM](https://huggingface.co/stanford-crfm/BioMedLM) — 2.7B parameter GPT-2-style language model trained exclusively on biomedical literature from PubMed for biomedical question answering and text generation.

### Foundation Models

#### Single-cell Foundation Models

##### Transcriptomics Foundation Models

* [scGPT](https://github.com/bowang-lab/scGPT) ⭐ 1,620 | 🐛 176 | 🌐 Jupyter Notebook | 📅 2026-04-29 — Transformer-based foundation model pretrained on millions of single-cell profiles.
* [scFoundation](https://github.com/biomap-research/scFoundation) ⭐ 427 | 🐛 31 | 🌐 Jupyter Notebook | 📅 2025-11-23 — Large-scale foundation model for single-cell gene expression, enabling multiple downstream tasks.
* [GEARS](https://github.com/snap-stanford/GEARS) ⭐ 401 | 🐛 21 | 🌐 Python | 📅 2025-02-01 — Graph-based model for predicting transcriptional responses to single and combinatorial genetic perturbations using biological priors.
* [scBERT](https://github.com/TencentAILabHealthcare/scBERT) ⭐ 361 | 🐛 26 | 🌐 Python | 📅 2023-12-13 — BERT-based foundation model pretrained on large-scale scRNA-seq data for cell type annotation.
* [UCE](https://github.com/snap-stanford/UCE) ⭐ 332 | 🐛 3 | 🌐 Python | 📅 2026-07-08 — Universal Cell Embeddings: zero-shot single-cell embedding model trained on 36M cells across species, tissues, and assays without fine-tuning.
* [SATURN](https://github.com/snap-stanford/SATURN) ⭐ 173 | 🐛 4 | 🌐 Jupyter Notebook | 📅 2024-07-03 — Transformer-based model integrating gene expression and protein sequences via a protein language model to learn unified multi-species cell embeddings.
* [CellPLM](https://github.com/OmicsML/CellPLM) ⭐ 106 | 🐛 10 | 🌐 Jupyter Notebook | 📅 2024-03-28 — Cell pre-trained language model with inter-cell transformer architecture for diverse single-cell analysis tasks.
* [BulkFormer](https://github.com/KangBoming/BulkFormer) ⭐ 79 | 🐛 6 | 🌐 Jupyter Notebook | 📅 2026-07-03 — Foundation model for bulk RNA-seq data; learns general transcriptomic representations.
* [CancerFoundation](https://github.com/BoevaLab/CancerFoundation) ⭐ 31 | 🐛 1 | 🌐 Jupyter Notebook | 📅 2025-09-12 — Single-cell RNA-seq foundation model trained exclusively on a curated dataset of malignant cells to learn cancer-specific embeddings.
* [Geneformer](https://huggingface.co/ctheodoris/Geneformer) — Context-aware, attention-based deep learning model pretrained on a large corpus of single-cell transcriptomes.

##### Spatial Foundation Models

* [UNI](https://github.com/mahmoodlab/UNI) ⭐ 769 | 🐛 32 | 🌐 Jupyter Notebook | 📅 2025-03-26 — General-purpose self-supervised pathology foundation model trained on 100K+ whole-slide images for diverse computational pathology tasks.
* [GigaPath](https://github.com/prov-gigapath/prov-gigapath) ⭐ 631 | 🐛 74 | 🌐 Python | 📅 2026-08-07 — Slide-level digital pathology foundation model pretrained on 1.3 billion pathology image tokens from whole-slide images.
* [CONCH](https://github.com/mahmoodlab/CONCH) ⭐ 527 | 🐛 16 | 🌐 Python | 📅 2025-03-26 — Vision-language foundation model for computational pathology trained with contrastive captioning on pathology image–text pairs.
* [Nicheformer](https://github.com/theislab/nicheformer) ⭐ 170 | 🐛 24 | 🌐 Jupyter Notebook | 📅 2025-11-23 — Foundation model for single-cell and spatial omics using a transformer architecture with positional embeddings to encode spatial cell information.
* [scGPT-spatial](https://github.com/bowang-lab/scGPT-spatial) ⭐ 143 | 🐛 11 | 🌐 Jupyter Notebook | 📅 2025-02-13 — Extension of scGPT for spatial transcriptomics with continual pretraining and a mixture-of-experts decoder for spatial gene expression analysis.
* [DeepSpot](https://github.com/ratschlab/DeepSpot) ⭐ 95 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-17 — Deep learning model predicting spatial transcriptomics from H\&E images at spot and single-cell resolution.
* [DeepSpot-M](https://github.com/ratschlab/DeepSpotM) ⭐ 45 | 🐛 1 | 🌐 Python | 📅 2026-08-12 — Multimodal foundation model for transcriptome-wide virtual spatial transcriptomics from histology.
* [AESTETIK](https://github.com/ratschlab/aestetik) ⭐ 26 | 🐛 0 | 🌐 Jupyter Notebook | 📅 2026-08-18 — Autoencoder for spatial transcriptomics representation learning using topology and histology image knowledge.
* [DeepSpot2Cell](https://github.com/ratschlab/DeepSpot2Cell) ⭐ 18 | 🐛 0 | 🌐 Python | 📅 2026-08-17 — Predicts virtual single-cell spatial transcriptomics from H\&E using spot-level supervision (NeurIPS 2025 Imageomics).
* [Phikon](https://huggingface.co/owkin/phikon) — ViT-based pathology foundation model pretrained with iBOT self-supervision on TCGA whole-slide images.

##### Multi-Omics Foundation Models

* [totalVI](https://github.com/scverse/scvi-tools) ⭐ 1,683 | 🐛 22 | 🌐 Python | 📅 2026-08-25 — Probabilistic framework for joint analysis of paired scRNA-seq and protein (CITE-seq) data enabling multi-modal cell state representation across single-cell datasets.
* [MultiVI](https://github.com/scverse/scvi-tools) ⭐ 1,683 | 🐛 22 | 🌐 Python | 📅 2026-08-25 — Multi-modal variational autoencoder for integrating paired and unpaired single-cell RNA-seq and ATAC-seq measurements into a unified latent space.
* [GLUE](https://github.com/gao-lab/GLUE) ⭐ 477 | 🐛 24 | 🌐 Python | 📅 2026-02-09 — Graph-Linked Unified Embedding framework for unpaired single-cell multi-omics data integration across RNA, ATAC, methylation, and protein modalities.
* [MOFA+](https://github.com/bioFAM/MOFA2) ⭐ 420 | 🐛 66 | 🌐 R | 📅 2026-08-26 — Multi-Omics Factor Analysis framework identifying shared axes of variation across bulk and single-cell datasets including RNA, ATAC, proteomics, methylation, and copy number.
* [GeneCompass](https://github.com/xCompass-AI/GeneCompass) ⭐ 122 | 🐛 20 | 🌐 Jupyter Notebook | 📅 2026-02-10 — Large-scale foundation model integrating DNA regulatory sequences and single-cell transcriptomics from 120M+ cells across multiple species for gene regulation prediction.
* [MIDAS](https://github.com/labomics/midas) ⭐ 72 | 🐛 0 | 🌐 Python | 📅 2026-05-10 — Mosaic integration and differential accessibility model for single-cell multi-omics data that handles arbitrary missing-modality combinations across transcriptomics, chromatin accessibility, and proteomics.
* [MIRA](https://github.com/cistrome/MIRA) ⭐ 70 | 🐛 23 | 🌐 HTML | 📅 2025-07-08 — Probabilistic multimodal topic model jointly modeling single-cell transcriptomics and chromatin accessibility for regulatory network inference.
* [scMulan](https://github.com/SuperBianC/scMulan) ⭐ 63 | 🐛 13 | 🌐 Jupyter Notebook | 📅 2024-05-30 — Single-cell multi-omic language model pretrained on \~10M cells spanning transcriptomics, epigenomics, and proteomics for cross-omics transfer tasks.
* [BABEL](https://github.com/wukevin/babel) ⭐ 53 | 🐛 8 | 🌐 Jupyter Notebook | 📅 2023-07-17 — Cross-modality translation model enabling prediction between scRNA-seq and scATAC-seq profiles without requiring paired single-cell measurements.
* [UnitedNet](https://github.com/LiuLab-Bioelectronics-Harvard/UnitedNet) ⭐ 53 | 🐛 5 | 🌐 Jupyter Notebook | 📅 2024-03-31 — Interpretable multi-task deep neural network for single-cell multi-omics integration spanning transcriptomics, chromatin accessibility, and proteomics.
* [Concerto](https://github.com/melobio/Concerto-reproducibility) ⭐ 41 | 🐛 2 | 🌐 Jupyter Notebook | 📅 2022-12-29 — Contrastive self-supervised learning framework for single-cell multimodal data integration, batch correction, and reference-query mapping.
* [Multigrate](https://github.com/theislab/multigrate) ⭐ 35 | 🐛 4 | 🌐 Python | 📅 2026-08-24 — Asymmetric multi-omics variational autoencoder for integrating single-cell data across RNA, ATAC, and protein modalities with missing-modality support.
* [scButterfly](https://github.com/BioX-NKU/scButterfly) ⭐ 30 | 🐛 10 | 🌐 Python | 📅 2024-07-01 — Dual-aligned variational autoencoder for single-cell cross-modality translation between paired and unpaired multiomics data.
* [JAMIE](https://github.com/Oafish1/JAMIE) ⭐ 17 | 🐛 0 | 🌐 Python | 📅 2025-09-11 — Joint variational autoencoder for multimodal single-cell data imputation and embedding.
* [scPair](https://github.com/quon-titative-biology/scPair) ⭐ 11 | 🐛 1 | 🌐 Python | 📅 2025-09-08 — Bidirectional feedforward network for single-cell multimodal analysis with cross-modality prediction leveraging single-cell atlases.
* [SpatialGlue](https://github.com/zhanglabtools/SpatialGlue) — Graph attention network for spatial multi-omics integration jointly embedding spatial transcriptomics with chromatin accessibility or proteomics.

##### Domain Alignment

* [scArches](https://github.com/theislab/scarches) ⭐ 407 | 🐛 67 | 🌐 Jupyter Notebook | 📅 2026-06-26 — Transfer learning framework for mapping new single-cell datasets onto pre-trained reference atlases across batches, conditions, and modalities.
* [TOSICA](https://github.com/JackieHanlaopo/TOSICA) — Transformer-based framework for one-stop interpretable cell-type annotation supporting cross-dataset and cross-species transfer.

#### Compound Foundation Models

##### Compound Embedding

* [Uni-Mol](https://github.com/deepmodeling/Uni-Mol) ⭐ 1,156 | 🐛 113 | 🌐 Python | 📅 2025-05-29 — 3D molecular pretraining framework for universal representation learning on molecules and protein pockets.
* [ChemBERTa-2](https://github.com/seyonechithrananda/bert-loves-chemistry) ⭐ 501 | 🐛 10 | 🌐 Jupyter Notebook | 📅 2024-10-27 — RoBERTa-based molecular language model pretrained on SMILES for small-molecule representation learning.
* [MolFormer](https://github.com/IBM/molformer) ⭐ 409 | 🐛 15 | 🌐 Jupyter Notebook | 📅 2025-09-17 — Linear attention transformer pretrained on millions of SMILES strings for efficient molecular embeddings.
* [GROVER](https://github.com/tencent-ailab/grover) ⭐ 394 | 🐛 19 | 🌐 Python | 📅 2026-02-25 — Self-supervised graph transformer for large-scale molecular representation learning from unlabeled compounds.
* [Mol2Vec](https://github.com/samoturk/mol2vec) ⚠️ Archived — Unsupervised molecular embedding method inspired by Word2Vec for learning vector representations of chemical substructures.

#### Protein Foundation Models

##### Pre-trained Embedding

* [Evolutionary Scale Modeling (ESM)](https://github.com/facebookresearch/esm) ⚠️ Archived — Protein embeddings.
* [ProtTrans](https://github.com/agemagician/ProtTrans) ⭐ 1,323 | 🐛 21 | 🌐 Jupyter Notebook | 📅 2025-05-22 — Suite of protein language models (ProtBERT, ProtT5, ProtXLNet) trained on billions of protein sequences from UniRef and BFD.
* [ProGen2](https://github.com/salesforce/progen) ⭐ 705 | 🐛 40 | 🌐 Python | 📅 2026-06-02 — Protein language model trained on diverse protein families for sequence generation and fitness prediction.
* [Ankh](https://github.com/agemagician/Ankh) ⭐ 249 | 🐛 11 | 🌐 Python | 📅 2025-06-16 — Efficient protein language model optimized for downstream prediction tasks including secondary structure, localization, and function annotation.

##### Protein Structure Prediction and Design

* [AlphaFold3](https://github.com/google-deepmind/alphafold3) ⭐ 8,500 | 🐛 17 | 🌐 Python | 📅 2026-08-19 — Predicts structures of proteins, nucleic acids, small molecules, and their complexes.
* [Boltz-1](https://github.com/jwohlwend/boltz) ⭐ 4,185 | 🐛 152 | 🌐 Python | 📅 2026-05-29 — Open-source all-atom biomolecular structure prediction model for proteins, nucleic acids, small molecules, and their complexes achieving AlphaFold3-level accuracy.
* [ESMFold](https://github.com/facebookresearch/esm) ⚠️ Archived — Fast protein structure prediction using language model embeddings.
* [OpenFold](https://github.com/aqlaboratory/openfold) ⭐ 3,420 | 🐛 245 | 🌐 Python | 📅 2025-12-16 — Trainable, memory-efficient open-source reproduction of AlphaFold2 enabling custom protein structure prediction workflows.
* [RFdiffusion](https://github.com/RosettaCommons/RFdiffusion) ⭐ 3,028 | 🐛 245 | 🌐 Python | 📅 2026-07-15 — Generative model for protein backbone design using diffusion.
* [ESM3](https://github.com/evolutionaryscale/esm) ⭐ 2,930 | 🐛 74 | 🌐 Jupyter Notebook | 📅 2026-08-27 — Multimodal protein language model that jointly reasons over sequence, structure, and function for generative protein design and engineering.
* [RoseTTAFold](https://github.com/RosettaCommons/RoseTTAFold) ⭐ 2,258 | 🐛 99 | 🌐 Python | 📅 2024-02-15 — Three-track neural network for protein structure prediction.
* [Chai-1](https://github.com/chaidiscovery/chai-lab) ⭐ 1,987 | 🐛 93 | 🌐 Python | 📅 2026-06-30 — Unified molecular structure prediction model covering proteins, nucleic acids, small molecules, and complexes.
* [ProteinMPNN](https://github.com/dauparas/ProteinMPNN) ⭐ 1,836 | 🐛 88 | 🌐 Jupyter Notebook | 📅 2024-08-14 — Deep learning model for protein sequence design given backbone structure.
* [EvoDiff](https://github.com/microsoft/evodiff) ⭐ 682 | 🐛 14 | 🌐 Python | 📅 2026-01-15 — Discrete diffusion framework for protein sequence generation trained on evolutionary-scale data, supporting unconditional generation, disordered region design, and functional motif scaffolding. \[ [paper-2023](https://www.biorxiv.org/content/10.1101/2023.09.11.556673v1) ]
* [OmegaFold](https://github.com/HeliXonProtein/OmegaFold) ⭐ 627 | 🐛 49 | 🌐 Python | 📅 2022-12-12 — High-resolution de novo protein structure prediction from sequence.
* [SaProt](https://github.com/westlake-reup/SaProt) — Structure-aware protein language model using structure-aware tokens that encode both sequence and backbone geometry for improved function prediction.

#### Multi-Modal Foundation Models

* [CHIEF](https://github.com/hms-dbmi/CHIEF) ⭐ 721 | 🐛 49 | 🌐 Python | 📅 2026-01-08 — Clinical Histopathology Imaging Evaluation Foundation model integrating histology images and clinical context for pan-cancer analysis.
* [PLIP](https://github.com/PathologyFoundation/plip) ⭐ 382 | 🐛 6 | 🌐 Python | 📅 2023-09-20 — Vision-language foundation model for pathology trained with contrastive learning on pathology image–text pairs for image classification and text-to-image retrieval.
* [PathomicFusion](https://github.com/mahmoodlab/PathomicFusion) ⭐ 327 | 🐛 10 | 🌐 Jupyter Notebook | 📅 2022-08-22 — Integrated framework fusing histopathology and genomic features via CNN, GNN, and attention gating for cancer diagnosis and prognosis.
* [PORPOISE](https://github.com/mahmoodlab/PORPOISE) ⭐ 250 | 🐛 8 | 🌐 Jupyter Notebook | 📅 2023-02-07 — Pan-cancer integrative histology-genomic analysis framework using multimodal deep learning for patient stratification.
* [MUSK](https://github.com/lilab-stanford/MUSK) ⭐ 243 | 🐛 4 | 🌐 Python | 📅 2025-10-26 — Vision-language foundation model for precision oncology analyzing multimodal paired text and pathology image data for biomarker prediction and retrieval.
* [TOAD](https://github.com/mahmoodlab/TOAD) ⭐ 186 | 🐛 8 | 🌐 Python | 📅 2021-11-01 — Tumor Origin Assessment via Deep-learning; weakly-supervised multi-task model predicting cancer primary origin from H\&E whole-slide images.
* [BiomedCLIP](https://huggingface.co/microsoft/BiomedCLIP-PubMedBERT_256-vit_g_14) — CLIP-based vision-language foundation model for biomedical images and text trained on PubMed figure–caption pairs.
* [Virchow](https://huggingface.co/paige-ai/Virchow) — Million-slide digital pathology foundation model using a vision transformer and self-supervised distillation for tile-level pathology image representation.

#### Genomics Foundation Models

* [Enformer](https://github.com/deepmind/deepmind-research/tree/master/enformer) ⭐ 15,174 | 🐛 358 | 🌐 Jupyter Notebook | 📅 2026-06-17 — Transformer model predicting gene expression from DNA sequence.
* [Evo](https://github.com/evo-design/evo) ⭐ 1,561 | 🐛 41 | 🌐 Python | 📅 2026-03-20 — Long-context genomic foundation model (up to 1M tokens).
* [Nucleotide Transformer](https://github.com/instadeepai/nucleotide-transformer) ⭐ 913 | 🐛 13 | 🌐 Jupyter Notebook | 📅 2026-02-24 — Foundation model for genomic sequences across multiple species.
* [HyenaDNA](https://github.com/HazyResearch/hyena-dna) ⭐ 808 | 🐛 38 | 🌐 Assembly | 📅 2025-04-22 — Long-range genomic foundation model handling sequences up to 1M tokens with sub-quadratic attention.
* [DNABERT](https://github.com/jerryji1993/DNABERT) ⭐ 777 | 🐛 73 | 🌐 Python | 📅 2026-01-22 — Pre-trained bidirectional encoder for DNA sequence analysis.
* [DNABERT-2](https://github.com/Zhihan1996/DNABERT_2) ⭐ 513 | 🐛 52 | 🌐 Shell | 📅 2026-01-01 — Improved genome foundation model with efficient tokenization.
* [Basenji](https://github.com/calico/basenji) ⭐ 474 | 🐛 87 | 🌐 Python | 📅 2026-01-15 — Sequential regulatory activity prediction from DNA sequences.
* [GPN (Genomic Pre-trained Network)](https://github.com/songlab-cal/gpn) ⭐ 354 | 🐛 7 | 🌐 Jupyter Notebook | 📅 2026-08-27 — Masked language model for DNA sequences enabling zero-shot variant effect prediction without requiring functional annotations.
* [Borzoi](https://github.com/calico/borzoi) ⭐ 261 | 🐛 13 | 🌐 Python | 📅 2025-08-28 — Extended successor to Enformer for predicting RNA-seq coverage from long genomic sequence windows (524 kb) with improved resolution.
* [Caduceus](https://github.com/kuleshov-group/caduceus) ⭐ 251 | 🐛 10 | 🌐 Python | 📅 2026-03-18 — Bidirectional equivariant long-range DNA sequence model based on Mamba.
* [Sei](https://github.com/FunctionLab/sei-framework) ⭐ 117 | 🐛 13 | 🌐 Python | 📅 2022-12-20 — Sequence-to-function framework learning a genome-wide regulatory activity code from DNA sequences for variant effect prediction.
* [DeepSEA](http://deepsea.princeton.edu/) — Deep learning framework for predicting chromatin effects of sequence alterations with single-nucleotide sensitivity across thousands of chromatin features.

***

## Citation

If you use this list in papers, slides, or documentation, please cite this repository via [`CITATION.cff`](./CITATION.cff) (also available through GitHub's **Cite this repository** button).

## Curation Criteria (Strict)

To keep quality high, additions should meet all of the following:

* The resource is trustworthy and relevant to computational biology.
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

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-29._

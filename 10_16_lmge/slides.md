<!-- .slide: data-background="images/title.jpg" data-state="dim-background" -->
### Enhancing Ecological Understanding through Sustainable Multi-Omics Approaches

#### A Project Proposal and Collaboration Opportunities at LMGE

<br>

Bérénice Batut

<small>Institut Francais de Bioinformatique / Auvergne Bioinformatique, Université Clermont Auvergne <br> She/her - <i class="fab fa-github"></i> @bebatut - <i class="fas fa-envelope"></i> berenice.batut@uca.fr</small>

<small>Séminaire LMGE - October 2024</small>


<small style="position: absolute; right: 0%; font-size: 0.2em; ">Photo by [Elena Mozhvilo](https://unsplash.com/@miracleday?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) </small>

Note:

- Clarify that the talk will cover both your past work and your future vision for bioinformatics infrastructure.

---

<!-- .slide: data-background="images/education.jpg" data-state="dim-background" -->

## My background <!-- .element style="color: white; background: black; padding-bottom: 20px" -->

<small style="position: absolute; right: 0%; font-size: 0.2em; bottom: -20%;">Photo by <a href="https://unsplash.com/@aaronburden?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Aaron Burden</a> on <a href="https://unsplash.com/photos/opened-book-QJDzYT_K8Xg?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a></small>

Note:

- Briefly introduce yourself and your research journey.
- Highlight key experiences and motivations that led you to focus on microorganism-environment interactions.

----

### Education

<div class="left_column" style="width:25%;">

<br>

![Illustration of me in front of a map with a red point on Lyon and linked to 3 logos: UCBL, Insa Lyon and ENS Lyon](images/study_1.png) <!-- .element width="100%" -->

</div>

<div style="text-align: left; float: right; width:65%;" data-markdown>

<i class="fas fa-calendar"></i> 2008-2011: Master of Engineering
<br><i class="fas fa-dot-circle"></i> **Bioinformatics** & modelling
<br><i class="fas fa-map-marker-alt"></i> INSA Lyon

<i class="fas fa-calendar"></i> 2010-2011: Master degree
<br><i class="fas fa-dot-circle"></i> Complex system modelling
<br><i class="fas fa-map-marker-alt"></i> ENS Lyon

</div>

Note:
- 2008-2011
    - Master of Engineering - Bioinformatics and modelling - INSA Lyon
    - Last year in parallel: Master degree - Theoretical computer science - Complex system modelling - ENS Lyon

----
### Education

<div class="left_column" style="width:25%;">

<br>

![Illustration of me in front of a map with a red point on Lyon and linked to 3 logos: UCBL, Insa Lyon and ENS Lyon](images/study.png) <!-- .element width="100%" -->

</div>

<div style="text-align: left; float: right; width:65%;" data-markdown>

<i class="fas fa-calendar"></i> 2008-2011: Master of Engineering
<br><i class="fas fa-dot-circle"></i> **Bioinformatics** & modelling
<br><i class="fas fa-map-marker-alt"></i> INSA Lyon

<i class="fas fa-calendar"></i> 2010-2011: Master degree
<br><i class="fas fa-dot-circle"></i> Complex system modelling
<br><i class="fas fa-map-marker-alt"></i> ENS Lyon

<i class="fas fa-calendar"></i> 2011-2014: PhD
<br><i class="fas fa-dot-circle"></i> **Bacterial** reductive genome **evolution**; *In silico* experimental evolution, **Comparative genomics / phylogeny**
<br><i class="fas fa-map-marker-alt"></i> LBBE & LIRIS, INSA Lyon

</div>

Note:
- 2008-2011
    - Master of Engineering - Bioinformatics and modelling - INSA Lyon
    - Last year in parallel: Master degree - Theoretical computer science - Complex system modelling - ENS Lyon



----

### Bacterial reductive genome evolution

2 aspects to study a same question


![](images/these.png) <!-- .element width="70%" -->

<small style="position: absolute; left: 0%;">[Batut et al, BMC Bioinformatics, 2013](https://link.springer.com/article/10.1186/1471-2105-14-S15-S11); [Batut et al, Nat Rev Microbiol, 2014](https://www.nature.com/articles/nrmicro3331)</small>

----
### Postdocs: From bacterial isolate to microbiome

<div class="left_column" style="width:25%;">

![Illustration of me in front of a map with a red point on Lyon and linked to 3 logos: UCBL, Insa Lyon and ENS Lyon](images/postdoc_clermont.png) <!-- .element width="100%" -->

</div>

<div style="text-align: left; float: right; width:65%;" data-markdown>

<i class="fas fa-calendar"></i> 2015-2016: Postdoc 
<br><i class="fas fa-dot-circle"></i> **Gut metagenomics**; **Tool/Workflow development**
<br><i class="fas fa-map-marker-alt"></i> CIDAM, Université d'Auvergne - Clermont-Ferrand

</div>

Note:
- 2015-2016
    - Postdoc - Clermont-Ferrand

Aim of the project

- Collect gut microbiota datasets in different databases
- Analyze them given a standard workflow

![Schema representing a simplified workflows for metagenomics. It starts on the top from a buble "Raw sequences" then go down to "Quality control" then "Sequence sorting". It then branches. On the left, "Taxonomic analysis" towards "Formatted taxonomic assignations". On the right, "Functional analysis" towards "Formatted functional assignations"](images/simplified_workflow.svg)

----
### ASaiM framework

![Schema representing the ASaiM framework. On the left, there is a sort of workflow starting with "Raw shotgun sequence data from microbiota" --> "Data upload" --> "Input dataset" --> "Data analyses" --> "Output dataset" --> "Data download" with 4 leaves "Taxonomic information", "Functional information", "Taxonomicall-related functional information", "Comparative analysis results (taxonomy, metabolism or taxonomicall-related metabolism)". Steps from "Data upload" to "Data download" are encapsulated in a big rectangle with "Galaxy instance with a custom configuration" written on the top. 1 arrow with "using" written on it starts from "Data analyses" and goes to a box with blue background labelled "Preconfigured workflows" with 2 boxes with white background in it: (1) "Workflows to analyze raw shotgun sequences from microbiota" with 2 boxes in it: (1.1) "Metagenomic/metatranscriptomic data" with a workflow: "Quality control" --> "Dereplicate" --> 2 branches: "Assign taxonomy (MetaPhlAn)" and "Remove rRNA/rDNA (SortMeRNA) --> Analyze functions (HUMAnN)", that merge in "Combine functional and taxonomic results"; (1.2) "Amplicon data" with a workflow "Control quality" --> "Dereplicate" --> "Extract rDAN (SortMeRNA)" --> "Assign taxonomy (Mothur)"; (2) "Workflows for comparative analyses" with 4 boxes: "Taxonomy", "Gene family/pathway abundances", "GO slim term abundances", "Taxonomically related gene family/pathway abundances". An arrow (with "using" written on it) starts from the "Preconfigured workflows" box toward a another box labelled "222 selected and automatically provisionned tools, organized to help user choices" with 4 boxes insides: (1) "47 manipulation tools" with rectangles "Get Data", "Manipulate files", "Manipulate sequence files", "Manipulate BAM/SAM files"; (2) "16 preprocessing tools" with boxes "Assemble paired-end sequences", "Control quality", "vsearch tool suite", "Cluster sequences", "Sort rRNA/rDNA"; (3) "149 structural and functional analysis tools" with boxes "Map against reference genomes", "Search similarity", "Mothur tool suite", "Analyze metabolism", "Assign taxonomy for all sequence types", "Combine functional and taxonomic results"; (4) "10 visualiszation, statistics and comparative analysis tools" with boxes "Visualize data", "Compute statistics". An arrow starts from the box "222 selected and automatically provisionned tools, organized to help user choices" towards the last box labelled "Imported databases". In this box, there are 3 boxes: (1) "rRNA/rDNA" with 2 boxes "SILVA" and "Rfam"; (2) "Taxonomy" with 1 box "MetaPhlAn2 database"; (3) "Functions" with 2 boxes "ChocoPhlAn" and "UniRef50"](images/asaim_v1.png) <!-- .element width="50%" -->

<small style="position: absolute; left: 0%;">[Batut et al, Gigascience, 2018](https://academic.oup.com/gigascience/article/7/6/giy057/5001424)</small>

Note:
- Simple Galaxy with only needed tools
- Need to do
    - Integrate missing tools that are used in the lab, and update existing ones
    - Build workflow

----
### Predefined and tested workflows

![ASaiM main workflow to analyze raw shotgun metagenomics data. It has 4 parts: PROCESSING (represented yellow boxes), TAXONOMIC ANALYSES (represented by the red boxes), FUNCTIONAL ANALYSES (represented by the purple boxes), FUNCTIONAL AND TAXONOMIC COMBINATION (represented by the green boxes). The workflow starts on the left, in PROCESSING part, from File "Raw reads" / FastQ on the left --> yellow box "Quality control (FastQC) and trimming (TrimGalore!)" --> File "Controlled reads" / Fasta --> yellow box "Dereplication (Vsearch)" --> File "Unique reads" / Fasta. The workflow branch then. (1) On the top, the TAXONOMIC ANALYSIS starts from the File "Unique reads" / Fasta --> red box "Taxonomic assignations (MetaPhlAn)" --> File "Taxa abundance" / Table --> 3 branches (from top to bottom): (1.1) red box "Visualization (GraPhlAn)" --> File "Community structure" / PNG; (1.2) red box "Visualization (KRONA)" --> File "Community structure" / HTML; (1.3) red box "Formatting for the different taxonomic levels" --> Different Files "Taxa abundance for species" / Table. 2 arrows start also from File "Taxa abundance" / Table to 2 boxes in FUNCTIONAL AND TAXONOMIC COMBINATION part. (2) On the bottom, the FUNCTIONAL ANALYSES starts from the File "Unique reads" / Fasta --> yellow box "rRNA/rDNA selection (SortMeRNA)" --> File "Non rRNA/rDNA reads" / Fasta --> purple box "Metabolic assignations (HUMAnN2)" --> 2 branches (from top to bottom): (2.1) File "Pathway abundance" / Table --> green box "Combination of taxonomic and metabolic assignations" --> File "Pathway abundance per taxa" / Table; (2.2) File "Gene family abundance" / Table --> 2 branches (from top to bottom): (2.2.1) green box "Combination of taxonomic and metabolic assignations" --> File "Gene family abundance per taxa" / Table; (2.2.2) purple box "Grouping to high level GO Slim terms" --> File "GOslim term abundance" / Table](images/asaim_main_wf.png) <!-- .element width="100%" -->

<small style="position: absolute; left: 0%;">[Batut et al, Gigascience, 2018](https://academic.oup.com/gigascience/article/7/6/giy057/5001424)</small>

Note:
- Introduce HUMAMnN, MetaPhlAn

----
### Postdocs: From bacterial isolate to microbiome

<div class="left_column" style="width:25%;">

![Illustration of me in front of a map with a red point on Lyon and linked to 3 logos: UCBL, Insa Lyon and ENS Lyon](images/postdocs.png) <!-- .element width="100%" -->

</div>

<div style="text-align: left; float: right; width:65%;" data-markdown>

<i class="fas fa-calendar"></i> 2015-2016: Postdoc 
<br><i class="fas fa-dot-circle"></i> **Gut metagenomics**; **Tool/Workflow development**
<br><i class="fas fa-map-marker-alt"></i> CIDAM, Université d'Auvergne - Clermont-Ferrand

<i class="fas fa-calendar"></i> 2016-2023: Postdoc 
<br><i class="fas fa-dot-circle"></i> Microbiome; **Data analyses**, **Tool/Workflow development**, **Training**, **Community**
<br><i class="fas fa-map-marker-alt"></i> [Freiburg Galaxy Team](https://galaxyproject.eu/freiburg/), Germany</small>

</div>


Note:
- 2016-now
    - Postdoc - Freiburg Galaxy team with Björn Grüning
    - de.NBI / ELIXIR
    - Gave up on idea to become Professor
    - Data analysis: RNA-seq, Microbiome - ASaiM
    - Tool development: Microbiome, Galaxy
    - Training, mentoring, community building


----

<small style="position: absolute; top: -3%; left: 0%;">Data Analysis / Host-Microbiote</small>

### Orchestration by microbiota of microglial transcriptome in young and aged mice

![](images/mossad2022_fig1.png) <!-- .element width="100%" -->

<small style="position: absolute; left: 0%;">[Mossad, Batut, et al, Nat Neurosc, 2022](https://www.nature.com/articles/s41593-022-01027-3)</small>

----

<small style="position: absolute; top: -3%; left: 0%;">Data Analysis / Host-Microbiote</small>

### Age-dependent shift in mouse gut microbiota composition

![](images/mossad2022_figS6.png) <!-- .element width="60%" -->

<small style="position: absolute; left: 0%;">[Mossad, Batut, et al, Nat Neurosc, 2022](https://www.nature.com/articles/s41593-022-01027-3)</small>

----

<small style="position: absolute; top: -3%; left: 0%;">Workflow development / Multi-omics</small>

### Integrative meta-omics in Galaxy and beyond

![](images/schiml2023_fig1.png) <!-- .element width="60%" -->

<small style="position: absolute; left: 0%;">[Schiml et al, Environmental Microbiome, 2023](https://environmentalmicrobiome.biomedcentral.com/articles/10.1186/s40793-023-00514-9)</small>

----

<small style="position: absolute; top: -3%; left: 0%;">Workflow development / Multi-omics</small>

### Integrative meta-omics in Galaxy and beyond

![](images/schiml2023_fig2.png) <!-- .element width="60%" -->

<small style="position: absolute; left: 0%;">[Schiml et al, Environmental Microbiome, 2023](https://environmentalmicrobiome.biomedcentral.com/articles/10.1186/s40793-023-00514-9)</small>

----

<small style="position: absolute; top: -3%; left: 0%;">Workflow development / Pathogens</small>

<div class="left_column" style="width:35%;">

### PathoGFAIR: (meta)genomics workflows for (foodborne) pathogens detection

</div>

<div style="text-align: left; float: right; width:55%;" data-markdown>

![](images/nasr2024_fig1.png) <!-- .element width="70%" style="margin: 0" -->

<small style="position: absolute; left: 0%;">[Nasr et al, BioRXiv, 2024](https://www.biorxiv.org/content/10.1101/2024.06.26.600753v1)</small>


</div>

----
<small style="position: absolute; top: -3%; left: 0%;">Training</small>

### Galaxy Training Network

<div class="left_column" style="width:40%; margin-left:-2em;">

![](images/gtn.png) <!-- .element style="box-shadow: 5px 5px 5px grey !important;" -->

</div>

<div class="right_column" style="width:60%;">

An **online & open infrastructure** to empower scientists and instructors
- 400+ tutorials in 30+ topics
- 190+ (130+ hours) videos 
- Computational resources: Data / Tools / Servers / TIaaS
- 400+ contributors
- Massive Online Events with 2k+ participants

<small style="position: absolute; left: 0%;">[Batut et al, Cell, 2018](https://www.cell.com/cell-systems/fulltext/S2405-4712(18)30230-8), [Hilterman et al, PLOS Comp Biol, 2023](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1010752)</small>

</div>


Note:
- Start to build an online training infrastructure for the Galaxy community
    - Rewamp GTN
    - Strengthen the community with events
- Teaching to empower 
    - users in their analysis
    - new contributors
- Big efforts to learn from different experiences
- ~40K visitors per months

----
<small style="position: absolute; top: -3%; left: 0%;">Training</small>

### OLS = Training + Mentoring

<div class="left_column" style="width:40%; margin-left:-2em;"> 

![OLS flyer](images/ols.png) <!-- .element width="45%" -->

</div>

<div class="right_column" style="width:60%;">

A 16-week long **personal mentorship** and **cohort-based training** for **Open Science ambassadors**

- 8 cohorts since 2020
- 380+ mentees from 6 continents across 55 countries
- 130+ mentors, 170+ experts, 90+ guest speakers
- 80 hours of training delivery, 120+ speakers for 230+ talks

<small style="position: absolute; left: 0%;">Batut et al, Writing</small>

</div>

Note:

- A 16-week program
    - 3 cohorts - .. participants - … mentors - … experts
    - Open Science
    - Community building
    - Inclusivity, Empowerment
- Pathways : participants → mentor, experts
- Efforts to choose speakers: women, minorities, entire worlds
- More than just mentoring, a community
    - … members
    - Active Slack with messages everydays
        - Resources
        - Events
        - Job offers
    - Ally skills
    - Developing research oriented topic
     
----
### Back in France

<div class="left_column" style="width:30%;">

![Illustration of me in front of a map with a red point on Lyon and linked to 3 logos: UCBL, Insa Lyon and ENS Lyon](images/ir.png) 

</div>

<div style="text-align: left; float: right; width:60%;" data-markdown>


<i class="fas fa-calendar"></i> 2024-Now: Research engineer 
<br><i class="fas fa-dot-circle"></i> Microbiome; **Data analyses**, **Tool/Workflow development**, **Training**
<br><i class="fas fa-map-marker-alt"></i> [Institut Francais de Bioinformatique](https://www.france-bioinformatique.fr/), [Platforme Auvergne Bioinformatique](https://mesocentre.uca.fr/projets-associes/plateforme-aubi), Université Clermont Auvergne</small>

</div>

----
<small style="position: absolute; top: -3%; left: 0%;">Workflow development, Training</small>

### ABRomics
#### A Galaxy-based One Health Antimicrobial Resistance Platform

![](images/abromics.png) <!-- .element width="80%" style="box-shadow: 5px 5px 5px grey !important;" -->

----
<small style="position: absolute; top: -3%; left: 0%;">Workflow development, Training</small>

### ABRomics
#### A Galaxy-based One Health Antimicrobial Resistance Platform

![](images/abromics_wfs.png) <!-- .element width="80%" -->

----
<small style="position: absolute; top: -3%; left: 0%;">Community</small>

### microGalaxy

<div class="left_column" style="width:40%; margin-left:-2em;"> 

![](images/microgalaxy_sketch.png) <!-- .element width="80%" style="box-shadow: 5px 5px 5px grey !important;" -->

</div>

<div class="right_column" style="width:60%;">

A gateway to tools, workflows, and training for accessible, reproducible and FAIR of **microbial** data analysis

- 290+ Tool suites
- 20+ ready-to-use **Workflows**
- 20+ **Tutorials**, 3 learning pathways
- A dedicated **interface**
- A vibrant **community** with 50+ members, Quaterly meetings, Chat, Working groups

<small style="position: absolute; left: 0%;">Nasr et al, Writing</small>

</div>

---

<!-- .slide: data-background="images/crossroad.jpg" data-state="dim-background" -->

## And Now? <!-- .element style="color: white; background: black; padding-bottom: 20px" -->

Note:

- **Key Lessons Learned**
  - Summarize the most significant challenges and lessons from your past work, particularly in terms of scalability, reproducibility, and cross-disciplinary collaboration.
- **Bridging to the Future**
  - Introduce your long-term goal: advancing bioinformatics infrastructure to enable deeper insights into microorganism-environment interactions.
    
---

<!-- .slide: data-background="images/future.jpg" data-state="dim-background" -->

## Enhancing Ecological Understanding through Sustainable Multi-Omics Approaches <!-- .element style="color: white; background: black; padding-bottom: 20px" -->

<small style="position: absolute; right: 0%; font-size: 0.2em; bottom: -20%;">
Photo by <a href="https://unsplash.com/@soymeraki?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Javier Allegue Barros</a> on <a href="https://unsplash.com/photos/silhouette-of-road-signage-during-golden-hour-C7B-ExXpOIE?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a></small>

----

### Our world belongs to the microorganisms

<div class="left_column" style="width:50%; margin-left:-2em;"> 

![](images/cell_cover_24.jpg) <!-- .element width="80%" style="box-shadow: 5px 5px 5px grey !important;" -->

</div>

<div class="right_column" style="width:50%;">

![](images/save_the_microbes_to_save_the_planet.png) <!-- .element width="80%" style="box-shadow: 5px 5px 5px grey !important;" -->

![](images/call_to_action_microbes_planetary_health.png) <!-- .element width="80%" style="box-shadow: 5px 5px 5px grey !important; margin-left: 40px; margin-top: -100px;" -->

</div>

---

### My questions

1. How can we effectively **characterize microorganisms** and their **interactions** with their environment or host?

----
<small style="position: absolute; top: -3%; left: 0%;">1. Characterizing microorganisms and their interations</small>

### Construction of biome-specific microbiome database

By reanalyzing in a standardized way data from public database

<div class="left_column" style="width:50%; margin-left:-2em;"> 

![](images/beer_microbiome.png) <!-- .element width="80%" style="box-shadow: 5px 5px 5px grey !important;" -->

</div>

<div class="right_column" style="width:50%;">

Bee Microbiome DB

2 M1 Internships in 2024 together with **IHP Team**
- DB conception, including metadata evaluation
- Standardized workflow and explorative script conception

</div>

----

<small style="position: absolute; top: -3%; left: 0%;">1. Characterizing microorganisms and their interations</small>

### Construction of biome-specific microbiome database

What I would like to do now?

- Populate the Bee Microbiome DB
- **Automatize** the process for reanalysis in Galaxy
- Include **interactive data explorations and comparative analysis**
- Curate **metadata** to improve comparative analyses
- Make the infrastructure usable for **any biome**
- Use **MGnify** workflows and publish results in MGnify database
- Include **other omics** data when available

----
<small style="position: absolute; top: -3%; left: 0%;">1. Characterizing microorganisms and their interations</small>

### Exploration of host-microbiome interactions

What I would like to do?

- Identify (public) data combining different omics data for host (bees?) and their microbiome
- Develop **standardized holo-omics workflows for multi-omics integration**
- Develop benchmarking methods for multi-omics integration workflows

----
<small style="position: absolute; top: -3%; left: 0%;">1. Characterizing microorganisms and their interations</small>

### Genome reconstruction and annotation

![](images/mags_wf_buehler.png) <!-- .element width="75%" -->

FAIRyMAGs
- Workflow Finalization, Training Material Development, Real Data Evaluation, and Resource Allocation Tool Creation
- 100k€ funded by ELIXIR 
- **Collab.**: University of Freiburg (Germany), EMBL-EBI, University of Bari (Italy)

----
<small style="position: absolute; top: -3%; left: 0%;">1. Characterizing microorganisms and their interations</small>

### Genome reconstruction and annotation

What I would like to do after?

- Develop **benchmarking infrastructure** for MAGs building workflows (Critical Assessment Challenge?)
- Develop standardized workflows
  - **Not only for bacteria**
  - **Long-reads**
  - **Single-cell amplified genomes**

----

![](images/overview_1.png) <!-- .element width="75%" -->

---

### My questions

1. How can we effectively **characterize microorganisms** and their **interactions** with their environment or host?
2. How can we **track and monitor microbial changes**?

----

<small style="position: absolute; top: -3%; left: 0%;">2. Tracking and monitor microbial changes</small>

### Pathogen detection 

<div class="left_column" style="width:35%;">

![](images/nasr2024_fig1.png) <!-- .element width="100%" -->

</div>

<div style="text-align: left; float: right; width:55%;" data-markdown>

What I would like to do?

- Improve the sensitivity and specificity of the methods
- Test with different food vehicle, different pathogens, and pathogen combinations
- Adapt for **Wastewater**

**Collab.**: University of Freiburg (Germany), CERTH (Greece), ELIXIR Wastewater Surveillance Working Group 

</div>

----

<small style="position: absolute; top: -3%; left: 0%;">2. Tracking and monitor microbial changes</small>

### Marker of future genome changes

<div class="left_column" style="width:35%;">

![](images/.png) <!-- .element width="100%" -->

</div>

<div style="text-align: left; float: right; width:55%;" data-markdown>

What I would like to do?

- 

**Collab.**: BEAGLE (INRIA, INSA, Lyon)

</div>

----
<small style="position: absolute; top: -3%; left: 0%;">2. Tracking and monitor microbial changes</small>

### Antibiotic Resistance?

----

![](images/overview_2.png) <!-- .element width="75%" -->

---

### My questions

1. How can we effectively **characterize microorganisms** and their **interactions** with their environment or host?
2. How can we **track and monitor microbial changes**?
3. How do **changes** in the environment or host **impact microorganisms**?

----

<small style="position: absolute; top: -3%; left: 0%;">3. Exploring changes in environment on microorganisms</small>

### Reductive Genome Evolution

<div class="left_column" style="width:35%;">

![](images/) <!-- .element width="100%" -->

</div>

<div style="text-align: left; float: right; width:55%;" data-markdown>

What I would like to do?

- Build a database of genomes from public data and reconstructed MAGs of species that have undergone reductive genome evolution and close relatives
- Test artificial evolution predictions for reductive genome evolution on data from this database

**Collab.**: BEAGLE (INRIA, INSA, Lyon)

</div>

----

![](images/overview_3.png) <!-- .element width="75%" -->

---

### My questions

1. How can we effectively **characterize microorganisms** and their **interactions** with their environment or host?
2. How can we **track and monitor microbial changes**?
3. How do **changes** in the environment or host **impact microorganisms**?
4. How can we develop reproducible, standardized, and FAIR bioinformatics methods to answer these questions while managing the complexity and scale of microbiome research?

----

<small style="position: absolute; top: -3%; left: 0%;">4. Developing reproducible, standardized, and FAIR bioinformatics methods</small>

### Developing reproducible, standardized, and FAIR bioinformatics methods

What I would like to do?
- Make all my **workflows FAIR**
- Document and build capacity around them using **Training**
- Develop **Federated Data Analysis** especially between Galaxy and MGnify
- Engage, Develop and Manage strong and supportive **communities** to support all this work 

Note:

- FAIR workflows
    - Reduce the entry barrier for meta-omics data analysis 
    - BRC Analytics?
- Federated Data Analysis
    - Allow LMIC to use similar resources 
- Training
    - GTN beyond Galaxy 

----

![](images/overview.png) <!-- .element width="75%" -->

---

<!-- .slide: data-background="images/collaboration.jpg" data-state="dim-background" -->

## Would you be interested in collaborating? <!-- .element style="color: white; background: black; padding-bottom: 20px" -->

---

![](images/overview.png) <!-- .element width="75%" -->


Note: 

### **Conclusion and Takeaways** (5 minutes)
   - Summarize the key aspects of your past work and how they inform your future research.
   - Reiterate the importance of building sustainable, FAIR, and reproducible bioinformatics platforms for microbiome studies.
   - Encourage questions and further discussions on potential collaborations.

---

<!-- .slide: data-background="images/thank_you.jpg" -->

<small style="position: absolute; right: 0%; font-size: 0.2em; bottom: -20%;">
Photo by <a href="https://unsplash.com/@alexas_fotos?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Alexas_Fotos</a> on <a href="https://unsplash.com/photos/brown-and-white-wooden-arrow-sign-pnGjbJEmU3o?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a></small>
  

---

![](images/overview.png) <!-- .element width="75%" -->

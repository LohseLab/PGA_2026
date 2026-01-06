# Population Genomic Analysis 2026 (PGBI11126)

GitHub repository of the [Population Genomic Analysis 2024 (PGBI11126) postgraduate course](http://www.drps.ed.ac.uk/23-24/dpt/cxpgbi11126.htm) at the University of Edinburgh 

Contacts
--------

- Course organiser: [Dr. Konrad Lohse](mailto:konrad.lohse@ed.ac.uk?subject=[PGA2024])
- Course secretary: [Miss Zofia Bekas](mailto:zofia.bekas@ed.ac.uk?subject=[PGA2024])

Course description
------------------

The course covers the core concepts of modern population genomic analysis which focuses on analysing sequence variation contained in samples of genomes. The aim is to both introduce students to the mathematical models and computational algorithms that describe the ancestry of genomes in evolving populations and show how these are applied in practice to make inferences about the interplay of evolutionary forces (genetic drift, recombination, selection and demographic history) using hands-on data examples. 

The course includes a detailed exposition of the coalescent, the canonical model of sample ancestry and the relevant data structures (genealogies, tree-sequences and graphs) for describing genetic ancestry. A major focus of the course is to understand how this basic stochastic model: 

- extends to include all fundamental evolutionary forces (recombination, population structure, admixture and natural selection) and
- is used to make inferences from both modern and ancient samples using mathematical analysis and simulation.

The course is run as a set of computer practicals which analyse genomic data (both real and simulated) through interactive jupyterLab notebooks. 
Each practical is partnered with a short pre-recorded mini lecture covering the theoretical/conceptual background. 
These should be watched ahead of the corresponding practical session.

Course admin
------------

- PGA consists of a 10 computer practical sesssion (the last one being a class excercise that accounts for 75% of the mark) which analyse population genomic data.
- **The first session will be on Tuesday 13/01/2025 @ 1400-1700 hrs in the [JCMB](https://goo.gl/maps/mYi8YMzKHiA1U9ceA) computer suite Room 1208 (follow the signs to Room 1206C, which is opposite of 1208).**
- While PGA focuses on analysing population genomic data, this will also involve using the Python programming language, which will be introduced gradually throughout the course.
  - if you have not worked with Jupyter notebooks before, please watch [this short intro video](https://www.youtube.com/watch?v=A5YyoCKxEOU) ahead of the course
  - if you are a complete Python-novice, please read sections 1. - 4.3 of the [official Python documentation](https://docs.python.org/3.6/tutorial/)

Using this repository
---------------------
1. Log into [LEARN](https://www.learn.ed.ac.uk/ultra/course).
2. Go to the [course](https://www.learn.ed.ac.uk/ultra/courses/_110711_1/outline).  
3. Click on "Course materials", then on the "Notable" icon. <img src="![Noteable](https://github.com/KLohse/PGA_course_2024/assets/17250135/349acfb6-48df-4f4a-aad4-13747caf73ff)
" width="75%" height="75%">
4. Select the "BioChemistry Notebook" from the dropdown menu and click "Start". <img src="https://github.com/KLohse/PGA_course_2024/blob/main/Noteable.png" width="75%" height="75%">
5. Click on `+GitRepo` to bring up the menu to clone this repository. <img src="" width="75%" height="75%">
6. For this you must enter the following information: <img src="https://github.com/KLohse/PGA_course_2024/blob/main/noteable2.png" width="75%" height="75%">  
  - **Git Repository URL**: `https://github.com/LohseLab/PGA_course_2024`
  - **Branch**: `main` 
7. You can now use the Jupyter file browser to navigate to the notebooks you want to execute.

Syllabus
--------
- `Practical_1`
  - coalescent simulation and relevant data structures.
  - run and analyse coalescent simulations with `msprime` and `tskit`.
  - understand how the variance of the coalescent depends on the two major axis of sampling: number of loci and number of individuals (Felsenstein 2004).
  - understand why it is natural (and helpful) to treat mutations separately from ancestry.
- `Practical_2`
  - understand why coalescent simulations are useful to gain intuition about population level processes.
  - appreciate that the site frequency spectrum (SFS) is a fundamental summary of sequence variation and how it relates to genealogical branch lengths.
  - understand the neutral expectation of the SFS.
- `Practical_3`
  - understand that summary statistics are the currency for comparing real data to idealized models of population processes/history and that such comparisons can be done either via analytic results or simulations.
  - know how coalescent simulations are used in approximate likelihood inference.
- `Practical_4`
  - ARGs and treesequences: how are they constructed and how do they differ?
  - appreciate that not all recombination events are detectable
  - understand the difference between map and physical length of a sequence
  - know that the span of trees along the genome is a random variable and that nodes are shared between many trees.
  - understand that the duality between branch lengths and popgen measures extends to correlated trees.
- `Practical_5`
  - gain familiarity with common bioinformatic file formats (FASTA, BED, VCF)
  - understand how (population) genomic data can be represented through these file formats.
  - know that the analysis of variation data often requires additional simplifications and/or re-classification of the data
  - use common Python libraries to parse, intersect, interrogate, and visualize population genomic data
  - understand that due to background selection, genetic diversity in the genome is strongly correlated with functional constraint
- `Practical_6` (Dr Derek Setter)
  - how does positive selection act to favour a beneficial mutation?
  - understand the role of drift/randomness on allele ferquency trajectories and fixation probability
  - understand the effect of positive selection on linked neutral variation
  - understand how `sweepfinder` works using simulation data
  - be able to perform a Selective sweep scan on real data
- `Practical_7` (Dr Simon Martin)
  - understand genealogical dicordance and how it depends on incomplete lineage sorting and gene flow
  - understand how the divergence history of populations affects the level of incomplete lineage sorting
  - be able to run multi-population coalescent simulations and extract genealogical information
  - learn how to detect introgression from archaic Hominins into modern humans using the D statsitic (aka the ABBA/BABA test)
- `Practical_8`
  - how to estimate differentiation between populations/species using 𝑑𝑥𝑦, 𝑑𝑛𝑒𝑡 and 𝐹𝑠𝑡 and understand how these summary statistics are defined and related to each other.
  - be able to use coalescent theory to relate estimates of divergence and differentiation obtained from whole genome data to models of equilibrium population structure and non-equilibrium population history.
  - be able to define outliers of differentiation in a genome scan.
  - be able to simulate sequence data under models of population structure and compare these to real data. 
- `Practical_9`
  - Revision session.
  - TBA
  

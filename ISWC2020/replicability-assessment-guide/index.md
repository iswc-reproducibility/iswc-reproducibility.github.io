---
title: Replicability Line of Assessment
layout: single
---

The following guidelines aim to support reproducibility of quantitative laboratory experiments with users (evaluation studies involving users conducting specified tasks in a controlled setting) in the context of the ISWC 2020 Reproducibility Initiative. (Exploratory studies are out of the scope of this evaluation as even their evaluation is challenging.)

As reproducibility of user studies may require significant resources---out of the means of this initiative---submitted (and successfully evaluated) contributions will be labelled <emph>Replicable</emph> meaning that the experiments have not been reproduced but the authors had supplied enough materials about their work so an interested researcher could re-run the experiments in question.

The authors should provide a full account of the work in question starting with the hypothesis generation, intended and study user groups, the study design and implementation and ending with the analysis of the results and their implications. These guidelines should not be seen as a final document but rather as an in-progress technical report to which we will add as we learn and accumulate experience. As all of the following materials and data cannot be fully provided in a single conference paper due to space limitations, the additional materials can be made available online in a public repository.
(Presenting the materials using this structure is recommended but not mandatory.)

These guidelines should be used in combination with the [following checklist](./checklist) for the ISWC 2020 Reproducibility Track.


# Hypothesis and Overall Design Evaluation
Authors should provide a clear hypothesis and discuss the design of its evaluation. What methods will be used to acquire evidence of its support? Which are the independent and dependent variables? Are there any factors of the environment authors need to control for? If several hypotheses are outlined, it should be clearly defined which (parts of the) experiments to refer to which hypothesis. 

# Target and Study User Groups
Authors should explicitly define the target/intended user group of the algorithm/method/system in question including demographics and their (level of) domain expertise (life sciences, cultural heritage, etc.) and technological experience (technology savvy, lay users, etc.). If knowledge regarding Semantic Web technologies is needed, that should be stated as well. As it is notoriously difficult to recruit users with suitable profiles often studies are conducted with students. If this is the case, the authors should explain how the target and study user groups overlap and differ. Further, explain how the study participants were recruited (venues, social media groups, etc.) and the compensation they received if any.

# Input Datasets
Authors should provide as much information as possible for the datasets being used. In the case of publicly available datasets provide information for the version used, when and from where they have been retrieved as well as all available metadata. If the data have been preprocessed (including anonymisation) explain why and how as well as provide any scripts and resources relevant to the preprocessing. In the cases when data cannot be made available (due to, for instance, confidentiality agreements) authors should provide as detailed description of the data as possible including different characteristics of the dataset as well as example inputs for the different tasks. Where possible sample anonymised data should be provided.

# Study Tasks
Authors should report all tasks given to the study participants together with the data used. How do these tasks relate to users’ (level of) expertise? Are these typical tasks performed on an everyday basis or rarely conducted? Is there one or several ways to solve them with a given system/method? When is a task considered solved and why? Is the success criteria binary - solved/unsolved or on a continuous scale and how is this determined? If study participants have received different sets of tasks all combinations need to be made available. Information regarding the number of study conditions a participant has to take part in (within-subject vs between-subject studies) as well as the approach used for the task assignments and balancing for ordering effects needs to be provided too. Ideally, information for the overall number of participants per condition and (sets of) tasks should be summarized in a table.

# Experimental Settings

### Setup
Authors should explicitly specify the hardware (cpu/ram/number & size of displays, etc.) and software needed, the surrounding environment where the experiment has been conducted as well as the relevant interaction context. Is the method/system in question supposed to be used in a special environment and has it been tested in such? If specialized hardware or software is needed, for instance, eye-tracking cameras, screen recording applications, multi-touch displays, joysticks, etc. it should be stated. Oftentimes, the study is monitored by an observer present in the same room. In such cases, authors should describe the observer’s role, for instance assisting the participants or timing the tasks, etc. The level of expertise/experience of each member of the evaluation team should be documented (one of: novice, some experience, experienced, very experienced).
    
### Procedure
Authors should provide a full account of the different phases of the evaluation in chronological order. Common phases include: introduction to the aim and scope of the study (including ethical issues), pre-study questionnaires regarding demographics, area and level of expertise, training materials and further instructions, the actual evaluation session, post-study interviews and questionnaires, study setting (e.g., usability lab, user’s normal environment), etc. For certain aspects where one of several possibilities has been selected (for instance questionnaires) authors should motivate its choice in comparison to others. Some studies implement think-aloud protocols or similar to acquire more information regarding participants actions and reasoning. Such protocols need to be described in detail too.

# Analysis of Collected Data

### Collected data
Ideally all raw data collected during the experiment should be available after suitable anonymization methods are applied. This includes measurements of dependent variables, observations made by the observer if one was present, time per task and overall time - average, minimum and maximum length of each session, whether one-off or longitudinal, if relevant as well as results from any standardized or custom questionnaires. In cases when study participants possess diverse backgrounds (for instance, expertise level and area) it is necessary to report the results separately for each group.
    
### Analysis
Authors should also report and motivate the selected data analysis method, which type of statistical test was used and how this relates to the study design. Additionally, the authors should explain how the figures are obtained and provide the relevant code. Finally but very importantly, authors should discuss potential biases and threats to the validity of the results. All scripts, software libraries and tools used for the data analysis need to be provided as well.  Data on pilot studies should also be submitted, in addition to key changes made prior to the final study, along with explanations for these.

Acknowledgements: These guidelines are inspired by Valentina’s experience from participating in the organization of the [VOILA! Workshop series](http://voila.visualdataweb.org/) as well as co-authoring of the [A Framework to Conduct and Report on Empirical User Studies in Semantic Web Contexts](http://www.diva-portal.org/smash/get/diva2:1261778/FULLTEXT01.pdf) paper. We thank Aba-Sah Dadzie, Catia Pesquita and Patrick Lambrix for sharing their experience, feedback and suggestions while refining this document.

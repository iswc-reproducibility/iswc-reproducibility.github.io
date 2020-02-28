---
title: Reproducibility Line of Assessment
layout: single
---

Every research paper is different and the steps to achieve reproducibility may vary, but here we provide general guidance and links to other resources that you can consider to make your research reproducibile.

In some cases, the reproducers from the Programme Committee can simply re-run software (e.g. re-run some existing benchmark). In other cases, getting the raw data for an experiment may require special data sharing agreements. Then, it would be ideal if you could provide some simulated datasets to run the evaluation. 

# Environment

Authors should explicitly specify the Operating System and tools that should be installed as the environment for running the software. Such specification should include dependencies with specific hardware features (e.g. 25 GB of RAM are needed)or dependencies within the environment (e.g. the requried compiler needs a specific version of the OS). 

# System

System setup is one of the most challenging aspects when repeating experiments. System setup will be easier to conduct if it is automatic rather than manual. Authors should test that the system they distribute can actually be installed in a new environment. The documentation should detail every step in system setup (even if a step is performed in an automatic manner provide relevant info in case changes need to be done):

- How to obtain the system?
- How to configure the environment if need be (e.g., environment variables, paths)?
- How to compile the system? (existing compilation options should be mentioned and why they are needed)
- How to use the system? (What are the configuration options and parameters to the system and where to set them?)
- How to make sure that the system is installed correctly? 

**The following are mandatory for submissions which aim at software reproducibility, and not at experiments reproducibility; However, submissions aiming at experiments reproducibility should still supply relevant tests but not necessary in such detail**

Include tests at different levels - for all levels input and output samples need to be provided. Document the tests and how to run them as well as provide relevant scripts and resources to set up the test environment: (modified from [The Turing Way: Guide to Reproducible Research](https://the-turing-way.netlify.com/introduction/introduction) )
- Unit testing - all individual or, at the very least those with key functionalities, software components/units are tested separately to ensure they are functioning as per design;
- Integration tests - several components are tested together to ensure proper interaction between them;
- System tests - the entire system is tested as a whole to ensure that it functions properly and produces the correct output from a given input. Include common and important cases as well as corner cases.

**Both software and experiments reproducibility:** The above tasks should be achieved by executing a set of scripts provided by the authors that will download needed components (systems, libraries), initialize the environment, check that software and hardware is compatible, and deploy the system. 

# Experiments

Given a system, the authors should provide the complete set of experiments to reproduce the paper's results. Typically, each experiment will consist of the following parts.

    - A setup phase where parameters are configured and data is loaded.
    - A running phase where a workload is applied and measurements are taken.
    - A clean-up phase where the system is prepared to avoid interference with the next round of experiments. 

The authors should document (i) how to perform the setup, running and clean-up phases, and (ii) how to check that these phases complete as they should. The authors should document the expected effect of the setup phase (e.g., a cold file cache is enforced) and the different steps of the running phase, e.g., by documenting the combination of command line options used to run a given experiment script.

Experiments should be automatic, e.g., via a script that takes a range of values for each experiment parameter as arguments, rather than manual, e.g., via a script that must be edited so that a constant takes the value of a given experiment parameter.


# Graphs and Plots

For each graph in the paper, the authors should describe how the graph is obtained from the experimental measurements. The submission should contain the scripts (or spreadsheets) that are used to generate the graphs. We strongly encourage authors to provide scripts for all their graphs using a tool such as Gnuplot or Matplotlib. Here are two useful tutorials for Gnuplot: a brief manual and tutorial, and a tutorial with details about creating eps figures and embed them using LaTeX and another two for Matplotlib: examples from SciPy, and a step-by-step tutorial discussing many features. 

# Further resources

- [The Turing Way: Guide to Reproducible Research](https://the-turing-way.netlify.com/introduction/introduction)

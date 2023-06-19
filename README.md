## **Comparative *16S* Amplicon Analysis using QIIME2 on the Graham Cluster: Tutorial and Resources**

This is a public repo that can be used to learn how to conduct a comparative 16S amplicon analysis via QIIME2's microbiome analysis suite [1] on the Digital Research Alliance of Canada's Graham cluster. The tutorial is written in Bookdown format and covers each command and tool used step-by-step. The analysis methods are formally reviewed in Bosch et al. [2], and outline each plug-in that is used, their associated references and the results of the study - methods are outlined in Chapter 3. 

### 🧬 **A brief review of the data used in this analysis:**

  The data used in this analysis was taken from a thesis project that focuses on the transfer of seabird nutrients from a seabird nesting colony in Cape St. Mary’s Ecological Reserve (Newfoundland, Canada) [2]. Review this graphical abstract to understand the ecological processes taking place here:

![image](https://github.com/johannabosch/QIIME2_for_Graham/assets/126937348/9ec5fe4e-161f-4e4c-9c4b-d93eb391cef2)
>  <sup> **Figure:** Seabird nutrient transfer from Bird Rock, in Cape St. Mary’s Ecological Reserve (Newfoundland) to a pond 240 m away from the seabird colony. Seen in the illustration are northern gannets (*Morus bassanus*) and black-legged kittiwakes (*Rissa tridactyla*), which both nest within the Reserve on an annual basis. <sup>                                                          

  Using targeted *16S* amplicon sequencing, we assessed how the transfer of nutrients by seabirds in Cape St. Mary's impacts the bacterial composition of sediments taken from ponds nearby a colony. We used QIIME2, a next-generation microbiome bioinformatics suite that offers a free, user-friendly, and open source platform for both advanced and beginner researchers [1]. The analysis using QIIME2 is run on the Graham cluster hosted by the Digital Research Alliance of Canada (CCDB).

___

### **Resources:**

Tutorial for this analysis: [bookdown link]

**Softwares used in this analysis:**
These are all made available through the Graham cluster by loading various environment management systems (modules) that helps users create a consistent and controlled environment for executing commands using Python, R, C/C++, Fortran, Java, MATLAB, and Julia.

[QIIME2](https://qiime2.org/) - a microbiome analysis 

[R and RStudio}(https://rstudio-education.github.io/hopr/starting.html) - used to make plots in QIIME2R and Phyloseq packages

[Python]() - used for the quality checking stage via MultiQC




___


___


### 💻 **Using the Graham cluster for data analysis:**

  The first portion of this tutorial reviews using the Graham cluster for this analysis. The benefits of using a computing cluster are that it enables efficient processing of large datasets, parallel computing for faster results (covered in my Metagenomics  tutorial - [LINK]), access to a collaborative community of researchers, and the flexibility of accessing files from any computer with internet access. Graham is a heterogeneous cluster, suitable for a variety of workloads, and located at the University of Waterloo [3]. To read more about getting started with the Graham cluster visit their documentation: https://docs.alliancecan.ca/wiki/Getting_started_with_the_new_national_systems.

  The cluster is useful for running jobs that are intensive; jobs are run as a simple text file that contains information about which allocation to run the job on, and let's you specify how many compute nodes the job needs, how much memory the job needs, and how long the job will take to run. Using CCDB is also advantageous because you can log-in to their nodes from any computer, store data and make use of their many client support services.

___


### 💬**Technical support at the Alliance:**
  E-mail CCDB if you have trouble with your account or even if you have questions about your job scripts or commands while running an analysis. They have a helpful team of individuals who will reply to your e-mails promptly and point you in the right direction.

E-mail|Purpose|
|----|-----|
accounts@tech.alliancecan.ca | For questions about accounts | 
renewals@tech.alliancecan.ca | For questions about account renewals |
globus@tech.alliancecan.ca | For questions about Globus file transfer services |
cloud@tech.alliancecan.ca | For questions about using Cloud resources |
support@tech.alliancecan.ca | For any other questions, including questions related to your bioinformatics analysis |

**NOTE:** If you are going to contact support, make sure to read this technical support page first to know what to include in your message: https://docs.alliancecan.ca/wiki/Technical_support 

___

### 📝 **Acknowledgments**
  I would like to acknowledge the *Amplicon analysis tutorial using Qiime2* by Comeau et al. [4] that was used as a primary reference while conducting the analysis through the Graham cluster, as well as the support team at the Alliance for troubleshooting issues I encountered while carrying out this project.
___
___

### 📚 **References:**

[1] Bolyen E, Rideout JR, Dillon MR, Bokulich NA, Abnet CC, Al-Ghalith GA, et al. 2019 Reproducible, interactive, scalable and extensible microbiome data science using QIIME 2. Nature Biotechnology 37: 852–857. https://doi.org/10.1038/s41587-019-0209-9

[2] Bosch, J. 2023 From Seabirds to Sediments: The ecological footprint of seabirds at a prominent North Atlantic breeding
colony tracked using a multi-proxy paleolimnological approach. Memorial University of Newfoundland [unpubl. thesis]

[3] CCDB 2023. Graham. CCDB Docs. URL: https://docs.alliancecan.ca/wiki/Graham 

[4] Comeau AM, Douglas GM, Langille M. 2017 Microbiome Helper: A custom and streamlined workflow for microbiome research. mSystems, 2:e00127-16.


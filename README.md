**What is this for?**

  This repository is public and can be used to learn how to conduct a comparative 16S amplicon analysis via QIIME2's microbiome analysis suite [1] on Compute Canada's Graham Cluster. I provide an in-depth review of the commands used for a microbiome analysis using QIIME2, and ways to use the Graham cluster - hosted by the Digital Research Alliance of Canada (CCDB). The analysis methods are reviewed in Bosch et al. [2], and outline each plug-in that is used, their associated references and the results of the study - methods are outlined in Chapter 3. I would like to acknowledge the *Amplcion analysis tutorial using Qiime2* by Comeau et al. [7] that was used as a primary reference while conducting the anaylsis through the Graham cluster, as well as the support team at CCDB for troubleshooting issues I encountered while carrying out this project.


___


**A brief methods review:**

  This bioinformatics analysis was performed with QIIME2, a next-generation microbiome bioinformatics suite that offers a free, user-friendly, and open source platform for both advanced and beginner researchers [1]. The analysis using Qiime2 is run on the Graham cluster hosted by the Digital Research Alliance of Canada (CCDB). Here, I review methods specific to a project involving both sedimentary samples and seabird fecal samples [2].


___


**Using the CCDB Graham cluster for data analysis:**

  The first portion of this tutorial reviews using the Graham cluster for this analysis. Graham is a heterogeneous cluster, suitable for a variety of workloads, and located at the University of Waterloo [3]. To read more about getting started with the Graham cluster visit their documentation: https://docs.alliancecan.ca/wiki/Getting_started_with_the_new_national_systems. The cluster is useful for running jobs that are intensive; job are run as a simple text file that contains information about which allocation to run the job on, and let's you specify how many compute nodes the job needs, how much memory the job needs, and how long the job will take to run. Using CCDB is also advantageous because you can log-in to their nodes from any computer, store data and make use of their many client support services via these emails:


___


**CCDB's Technical support:**
  E-mail CCDB if you have trouble with your account or even if you have questions about your job scripts or commands while running an analysis. They have a helpful team of individuals who will reply to your e-mails promptly and point you in the right direction.

**For questions about accounts:**   
      
      accounts@tech.alliancecan.ca
      
**For questions about account renewals:**
      
      renewals@tech.alliancecan.ca

**For questions about Globus file transfer services:**
     
     globus@tech.alliancecan.ca
      
**For questions about using Cloud resources:**
    
    cloud@tech.alliancecan.ca

**For any other questions, including questions related to your bioinformatics analysis:**
     
     support@tech.alliancecan.ca
      

**NOTE:** If you are going to contact support, make sure to read this technical support page first to know what to include in your message: https://docs.alliancecan.ca/wiki/Technical_support 

___
___
___

**References:**

[1] Bolyen E, Rideout JR, Dillon MR, Bokulich NA, Abnet CC, Al-Ghalith GA, et al. 2019 Reproducible, interactive, scalable and extensible microbiome data science using QIIME 2. Nature Biotechnology 37: 852–857. https://doi.org/10.1038/s41587-019-0209-9

[2] Bosch, J. 2023 From Seabirds to Sediments: The ecological footprint of seabirds at a prominent North Atlantic breeding
colony tracked using a multi-proxy paleolimnological approach. Memorial University of Newfoundland [unpubl. thesis]

[3] CCDB 2023. Graham. CCDB Docs. URL: https://docs.alliancecan.ca/wiki/Graham 

[5] Parada AE, Needham DM, Fuhrman JA. 2016 Every base matters: assessing small subunit rRNA primers for marine microbiomes with mock communities, time series and global field samples. Environmental microbiology. 18(5):1403-14.

[6] Walters W, Hyde ER, Berg-Lyons D, Ackermann G, Humphrey G, Parada A, et al. 2016. Improved bacterial 16S rRNA gene (V4 and V4-5) and fungal internal transcribed spacer marker gene primers for microbial community surveys. Msystems. 1(1):e00009-15.

[7] Comeau AM, Douglas GM, Langille M. 2017 Microbiome Helper: A custom and streamlined workflow for microbiome research. mSystems, 2:e00127-16.

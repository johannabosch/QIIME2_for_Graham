**A brief methods review**

  This bioinformatics analysis was performed with QIIME2, a next-generation microbiome bioinformatics suite that offers a free, user-friendly, and open source platform for both advanced and beginner researchers [1]. The analysis using Qiime2 is run on the Graham cluster hosted by the Digital Research Alliance of Canada (CCDB). Here, I review methods specific to a project involving both sedimentary samples and seabird fecal samples [2].

___

**Using the Graham Cluster**

  The first portion of this tutorial reviews using the Graham cluster for this analysis. Graham is a heterogeneous cluster, suitable for a variety of workloads, and located at the University of Waterloo [3]. To read more about getting started with the Graham cluster visit their documentation: https://docs.alliancecan.ca/wiki/Getting_started_with_the_new_national_systems. The cluster is useful for running jobs that are intensive; job are run as a simple text file that contains information about which allocation to run the job on, and let's you specify how many compute nodes the job needs, how much memory the job needs, and how long the job will take to run. Using CCDB is also advantageous because you can log-in to their nodes from any computer, store data and make use of their many client support services via these emails:
        
      ___
      accounts@tech.alliancecan.ca -- Questions about accounts
      renewals@tech.alliancecan.ca -- Questions about account renewals
      globus@tech.alliancecan.ca -- Questions about Globus file transfer services
      cloud@tech.alliancecan.ca -- Questions about using Cloud resources
      support@tech.alliancecan.ca -- For any other question or issue
      ___

  **NOTE:** If you are going to contact support, make sure to only include one issue per job, and always include the following information in your email [4]: 


*   Cluster name
*   Job ID
*   Job submission script: you can either give the full path of the script on the cluster; copy and paste the script; or attach the script file
*   File or files which contain the error message(s): give the full path of the file(s); copy and paste the file(s); or attach the error message(s) file(s)
*    Commands that you were executing
*     Avoid sending screenshots or other large image attachments except when necessary - the plain text of your commands, job script etc. is usually more helpful. See Copy and paste if you have trouble with this.
*    Software (name and version) you were trying to use
*    When did the problem happen?
*    If you want us to access, copy or edit your files, or inspect your account and possibly make changes there, say so explicitly in your email. For example, instead of attaching files to an email, you may indicate where they are located in your account and give us permission to access them. If you have already granted us permission via the CCDB interface to access your files, then you do not need to do it again in your support request.

___

**Sample review:**
  
  We began on our analysis with demultiplexed 16S amplicon sequencing data from 19 seabird fecal samples and 12 sediment samples using the V4V5 primers (515FB = GTGYCAGCMGCCGCGGTAA	926R = CCGYCAATTYMTTTRAGTTT) [5,6].You can learn more about the sequencing and library details from IMR (this is where the samples were sent for sequencing): https://imr.bio/protocols.html. The seabird fecal samples were collected from northern gannets (*Morus bassanus*), black-legged kittiwakes (*Rissa tridactyla*), common murres (*Uria aalge*), and atlantic puffins (*Fratercula arctica*), while the sediment samples are subsamples of sediment cores takes from 3 ponds; one pond ~240m upwind of a multispecies nesting colony (Bird Rock, Cape St. Mary's (CSM), Newfoundland) of gannets, kittiwakes and murres, one pond directly adjacent to an atlantic puffin colony (Little Fogo Islands, Newfoundland), and a reference pond ~2.56 km away from the multispecies colony in CSM. 


  View the 3 metadata files for these samples here:

      Metadata for all samples together https://github.com/johannabosch/QIIME2_for_Graham/blob/main/birds_metadata.csv
      Metadata for all sediment samples: https://github.com/johannabosch/QIIME2_for_Graham/blob/main/metadata.csv
      Metadata for all seabird fecal samples: https://github.com/johannabosch/QIIME2_for_Graham/blob/main/sediments_metadata.csv 
  

The analysis methods are reviewed in Bosch et al. [2], and outline each plug-in that is used, their associated references and the results of the study - methods are outlined in Chapter 3 of the thesis. I would like to acknowledge the *Amplcion analysis tutorial using Qiime2* by Comeau et al. [7] that I used to build this analysis via the Graham cluster, as well as the support team at CCDB for their continuous support while carrying out this project.

.

___
  ___

**References:**

[1] Bolyen E, Rideout JR, Dillon MR, Bokulich NA, Abnet CC, Al-Ghalith GA, et al. 2019 Reproducible, interactive, scalable and extensible microbiome data science using QIIME 2. Nature Biotechnology 37: 852–857. https://doi.org/10.1038/s41587-019-0209-9

[2] Bosch, J. 2023 Seabird ot Sediments: _. [unpubl. thesis]

[3] CCDB 2023. Graham. CCDB Docs. URL: https://docs.alliancecan.ca/wiki/Graham 

[4] CCDB 2023. Technical Support. CCDB Docs. URL: https://docs.alliancecan.ca/wiki/Technical_support 

[5] Parada AE, Needham DM, Fuhrman JA. 2016 Every base matters: assessing small subunit rRNA primers for marine microbiomes with mock communities, time series and global field samples. Environmental microbiology. 18(5):1403-14.

[6] Walters W, Hyde ER, Berg-Lyons D, Ackermann G, Humphrey G, Parada A, et al. 2016. Improved bacterial 16S rRNA gene (V4 and V4-5) and fungal internal transcribed spacer marker gene primers for microbial community surveys. Msystems. 1(1):e00009-15.

[7] Comeau AM, Douglas GM, Langille M. 2017 Microbiome Helper: A custom and streamlined workflow for microbiome research. mSystems, 2:e00127-16.

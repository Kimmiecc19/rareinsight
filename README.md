# RareInsight
RareInsight: Developing a rare disease report generator for clinicians and patients

# Scope
The scarcity of knowledge surrounding rare diseases underscores the critical necessity for collaborative research efforts to unravel their complexities and improve diagnostic and therapeutic outcomes. This research introduces RareInsight, an effort focused on developing an open-source, interactive dashboard tailored for clinicians and patients. Its primary objective is to transform the interpretation of genetic variant data into flexible and detailed reports, aiming to ease rare disease diagnosis and research.

RareInsight will be designed to process genetic variant data into customizable, interactive reports. These files are preferably generated by nf-core’s raredisease pipeline. The resulting VCF files will be used as input into the dashboard which is equipped with advanced filtering options, visualization and resources for clinicians and patients, thereby empowering users to explore detailed data and seamlessly collaborate with peers for further analysis and interpretation. The final interactive dashboard will be developed using Shiny and tested using rare disease data from dbGaP.

By encapsulating clinical relevance, genetic implications, and essential resources within these reports, RareInsight will aid in informed decision-making for both clinicians and patients. RareInsight will eliminate the proprietary limitations often present in existing tools. By adopting an open-source environment, it strives to encourage transparency and customization tailored to specific clinical or research requirements. The dashboard will also prioritize stringent data privacy and security measures to ensure the protection of sensitive genetic data.

Overall, this dashboard thrives on collaboration, by allowing researchers and clinicians to seamlessly share and collaborate on reports, fostering knowledge exchange and enriching the collective understanding of rare diseases. In essence, RareInsight is poised to redefine rare disease diagnosis and research by inviting collaboration and innovation to enhance healthcare outcomes in an open-source format.

# Workflow

![Basic outline of workflow](https://github.com/omicscodeathon/rareinsight/blob/main/figures/rareinsight_workflow.png)



# Deployment

Currently, RareInsight can be deployed from RStudio. The GitHub repository can be saved and uploaded into Rstudio where users can run the App. 

# User input

Input User Information panel: Users can input patient information to this panel.

Search Panel: Once the dashboard is initiated, the latest ClinVar variant summary file will automatically download. Users can only access the functions of the dashboard once the download has been completed. 

VCF Panel: Users can input a vcf.gz file that was ideally produced with the nf-core/raredisease pipeline. Files created with GATK can also be uploaded. Users can optionally input a filtered VCF file. Currently the script produces a filtered VCF file from the nf-core/raredisease pipeline. Users can filter their files using the filter_vcf.py script (found in the scripts folder). It includes the CSQ information from VEP, clinical diagnosis (CLNDN) and clinical significance (CLNSIG). 

# Outputs

Input User Information panel: Users can export the information in PDF format.

VCF Panel: Users can expect to visualize a VCF file in table format. Two plots are also generated to show the quality of the VCF file. 

Search Panel: Users can see and filter the ClinVar variant summary file. This file can be filtered according to a given gene, variant, disorder, ClinVar accession or dbSNP accession. It can then be further filtered by searching for specific information in the table.

Diagnostic report: Based on the search term used in the Search Panel, users can access links specific to this search term. Resources include PubMed, ClinVar, dbSNP, GeneReviews, LitVar2, gnomAD, Varsome and NORD. Patient-specific resources are also available such as RareConnect, RAReSOURCE, GARD and NORD patient organizations. 

# Contributors
- [Kimberly Christine Coetzer](https://github.com/Kimmiecc19) : PhD student, Division of Molecular Biology and Human Genetics, Department of Biomedical Sciences, Faculty of Medicine and Health Sciences, Stellenbosch University, Cape Town, South Africa
  
- [Firas Zemzem](https://github.com/Zemzemfiras1) : PhD student ,Laboratory of Cytogenetics, Molecular Genetics and Biology of Reproduction CHU Farhat Hached Sousse, Higher institute of Biotechnology of Monastir, University of Monastir, Tunisia

- [Eva Akurut](https://github.com/AkurutEva) : African Centre of Excellence in Bioinformatics and Data-intensive Sciences, Infectious Disease Institute, Makerere University, Kampala, Uganda
  
- [Gideon Akuamoah Wiafe](https://github.com/Gidoo) : MSc student, Neurogenomics Lab, Department of Medicine, Neuroscience Institute, University of Cape Town, Cape Town, South Africa; Department of Biomedical Sciences, University of Cape Coast, Cape Coast, Ghana

- [Olaitan I Awe](https://github.com/laitanawe) : Training officer, ASBCB, Cape Town, South Africa

# Thank you to the following organizations: 

- African Society for Bioinformatics and Computational Biology (ASBCB)

- National Institutes of Health (NIH) Office of Data Science Strategy (ODSS)

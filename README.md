# RiveraLab
Metagenomic Analysis   

  Please take the time to read this before beginning-- I cannot stress this enough. If you are not familiar with GitHub, please start here:   
  https://guides.github.com/activities/hello-world/  
  http://biorxiv.org/content/early/2016/04/15/048744.full-text.pdf+html   

The following folders contain information related to our metagenomic analysis. GitHub is being used for documentation and version control. 

(enter information about the study here, how samples were taken etc.)    

In order to upload these large files to galaxy we need to upload to FTP server first and then we can run fastqc joiner from there. This is how you upload ftp files. http://screencast.g2.bx.psu.edu/quickie_17_ftp_upload/flow.html 
Basically what we did was open up filezilla (server is main.g2.bx.psu.edu, user is alkhairohr@vcu.edu, password is riveraisdope) and dragged and dropped files.  

General Procudeure of Data Manipulation before analysis (varies sligthly, because this is protocol for RNA-seq):
http://linus.nci.nih.gov/~brb/GalaxyDoc.pdf
http://seqanswers.com/forums/showthread.php?t=21331

Before we can join the paired ends we must first use FASTQ_Groomer to to convert the files into the right type (fastqsanger). We choose the datafile we wanted to work with (C1_R1 and C2_R2), and we choose "Sanger & Illumina 1.8+" as the input FASTQ quality score types. Next the resulting files should be run through FASTQC to check the quality of the reads (and trimmed if needed) and then joined with FASTQ_joiner.  

 


# RiveraLab
Metagenomic Analysis   

  Please take the time to read this before beginning-- I cannot stress this enough. If you are not familiar with GitHub, please start here: https://guides.github.com/activities/hello-world/. 

The following folders contain information related to our metagenomic analysis. GitHub is being used for documentation and version control. 

(enter information about the study here, how samples were taken etc.)    
Files worked with on 3/29/16 
/home/voegtlylj/MouseData/HiSeq_150630_2X100/FASTQ/Project_MichaelKiflezghi/Sample_C1
From here we took R1 (left hand) and R2(right hand) and will run joint fastqc in galaxy

In order to upload these large files to galaxy we need to upload to FTP server first and then we can run fastqc joiner from there. This is how you upload ftp files. http://screencast.g2.bx.psu.edu/quickie_17_ftp_upload/flow.html 
Basically what we did was open up filezilla (server is main.g2.bx.psu.edu, user is alkhairohr@vcu.edu, password is riveraisdope) and dragged and dropped files.  

General Procudeure of Data Manipulation before analysis (varies sligthly, because this is protocol for RNA-seq):
http://linus.nci.nih.gov/~brb/GalaxyDoc.pdf
http://seqanswers.com/forums/showthread.php?t=21331

Before we can join the paired ends we must first use FASTQ_Groomer to to convert the files into the right type (fastqsanger). We choose the datafile we wanted to work with (C1_R1 and C2_R2), and we choose "Sanger & Illumina 1.8+" as the input FASTQ quality score types.


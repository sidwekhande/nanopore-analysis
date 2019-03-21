# nanopore-analysis
Data exploration and analysis of a set of Oxford Nanopore reads.

The task given was the identification of a species given this mystery set of reads.
Data given: GROUP10.fasta / GROUP10.fastq

##Data Quality Analysis:

Using Nanoplot - https://github.com/wdecoster/NanoPlot

Amazing visualition tool for Nanopore reads. Gives summary statistics and average read quality vs read length plots.

![](https://github.com/sidwekhande/nanopore-analysis/blob/master/Nanoplot/LengthvsQualityScatterPlot_hex.png)

Above hexplot shows average Nanopore read quality ~10 and the longest read ~17,000. It was generated by the following command:

`NanoPlot -t 2 --fastq ../GROUP10.fastq --plots hex --title "Mystery Data" --no-N50`

##Species Identification

Using the GROUP10.fasta file, I first filtered out the 25 longest reads (25LR.fasta).



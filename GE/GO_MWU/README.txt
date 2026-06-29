
I use an array (GO_MWU_array.slm) to batch process WGCNA modules for go enrichment an HPC system. This requires that the main directory with the array slurm script (GO_MWU_array.slm), contains a subdirectory for each WGCNA module, each with all required GO_MWU scripts from Mikhail Matz (https://github.com/z0on/GO_MWU/tree/master), your MWU/Fisher gene-module matrix (gene+kME) (ex. merged_hostGO_MM_MWU_red_numeric.csv), and your gene-go annotation file (annot_go_clean_final.tab).

I sub the following scripts for Mikhail Matz's GO_MWU.R script. These just have the goDivision prespecified for easy swapping between batch enrichments when batch processing.
GO_MWU_BP.R 
GO_MWU_CC.R 
GO_MWU_MF.R 

Other required scripts from Mikhail Matz (https://github.com/z0on/GO_MWU/tree/master) are:
go.obo
gomwu_a.pl
gomuw_b.pl
gomwu.functions.R


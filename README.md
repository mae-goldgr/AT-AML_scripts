# Publication_scripts: Genomic profiling of AT-AML

Manuscript: Goldgraben et al Pediatric Blood and Cancer 2020

https://onlinelibrary.wiley.com/doi/full/10.1002/pbc.28354

Scripts used in publication. This repo is no longer in development.

BAMs (GRCh37) and VCFs are available on EGA (EGAS00001004392).


#########################
### GERMLINE Analysis ###
#########################

Blood DNA WES sequencing data was plugged into the germline pipeline described 
in (https://github.com/elliefewings/wes_pipeline_01.18) 
and ran on a High Performance Computing University of Cambridge cluster CSD3.
*** Three job templates:
      06_hard_filtering 
      07_annotation and 
      08_export 
were modified for annotation with updated Ensembl vep 91 (included in Germline folder)

Exported annotated vcf data files from the pipeline were processed using the Rmarkdown scripts provided.

#########################
### SOMATIC Analysis  ###
#########################

Blood and tumour DNA WES sequencing data was plugged into the somatic pipeline described 
in (https://github.com/elliefewings/wes_somatic_pipeline_05.18) 
and ran on a High Performance Computing University of Cambridge cluster CSD3.
*** Two templates:
	06_annotation
	07_export 
were modified for annotation with updated Ensembl vep 91 (included in Somatic folder)

Exported annotated vcf data files from the pipeline were processed using the Rmarkdown scripts provided.

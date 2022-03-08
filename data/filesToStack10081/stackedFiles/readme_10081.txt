###################################
########### Disclaimer ############
This is the most recent readme publication based on all site-date combinations used during stackByTable.
Information specific to the query, including sites and dates, has been removed. The remaining content reflects general metadata for the data product.
All files used during stacking are listed at the bottom of this document, which includes the data publication dates.
##################################

This data package been produced by and downloaded from the National Ecological Observatory Network (NEON). NEON is funded by the National Science Foundation (Awards 0653461, 0752017, 1029808, 1138160, 1246537, 1638695, 1638696, 1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.

DATA PRODUCT INFORMATION
------------------------

ID: NEON.DOM.SITE.DP1.10081.001

Name: Soil microbe community composition

Description: Counts and relative abundances of archaeal, bacterial, and fungal taxa observed in soil microbial communities

NEON Science Team Supplier: Terrestrial Observation System

Abstract: This data product contains the quality-controlled laboratory data and metadata for NEON's soil bacterial, archaeal, and fungal community composition analysis derived from soil microbial sampling. Taxon tables are derived from the 16S and ITS marker gene sequencing data product, NEON.DP1.10108. The DNA sequence data are processed using standard bioinformatics software to generate taxonomic data. For additional details, see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.

Latency:
The expected time from data and/or sample collection in the field to data publication is as follows, for each of the data tables (in days) in the downloaded data package. See the Data Product User Guide for more information.

mcc\_soilSeqVariantMetadata\_16S:  730

mcc\_soilSeqVariantMetadata\_ITS:  730

mcc\_taxonTableLabSummary:  7

Brief Design Description: Soil sampling occurs annually at a minimum of one site per domain and once (sites with short growing seasons) to three times per year (sites with longer growing seasons), with collections occurring at every sampled site during the historic peak in vegetation greenness. Three pre-determined, randomly assigned locations are selected for each sampling event within each of 10 plots distributed throughout a site; sampling locations within a plot are not re-sampled. Soil samples are collected to a maximum depth of 30 cm, with organic and mineral soils sampled separately. The same samples are used for measurement of soil physical and chemical properties to maintain temporal and spatial connectivity. Subsamples of homogenized soil (rocks, roots and organic debris removed) from each of the 3 sampling locations are stored in sterile containers, frozen on dry ice in the field and shipped to an analytical facility for DNA sequence analysis using primer sets targeting the small subunit of the ribosomal RNA gene. Sequence data undergo QAQC and are processed bioinformatically using an in-house pipeline to identify unique sequence variants in the data and to taxonomically identify each sequence variant.

Brief Study Area Description: These data are collected at all NEON terrestrial sites.

Keywords: 16S, archived samples, fungi, archaea, fungal, sequencing, ITS, rRNA, material samples, taxonomy, marker genes, diversity, bacteria, community composition, microbes


DATA PACKAGE CONTENTS
---------------------

This data product contains up to 5 data tables:

mcc_taxonTableLabSummary - Summary data on laboratory methods for microbial taxon table results
mcc_soilTaxonTableMetadata_16S - Taxonomic table metadata for soil microbes from 16S marker gene sequencing analysis
mcc_soilTaxonTableMetadata_ITS - Taxonomic table metadata for soil microbes from ITS marker gene sequencing analysis
mcc_soilSeqVariantMetadata_16S - Taxon table metadata for soil microbes from sequence variant data analysis of the 16S marker gene
mcc_soilSeqVariantMetadata_ITS - Taxon table metadata for soil microbes from sequence variant data analysis of the ITS marker gene
If data are unavailable for the particular sites and dates queried, some tables may be absent.
Basic download package definition: The basic package includes the metadata and URL links to the taxonomic counts data on a per sample basis. The user can then select which taxonomic data to download.

Expanded download package definition: The expanded package includes the per-sample taxon tables for all records within the specified site and time ranges. It also includes a lab summary table that describes the bioinformatics methods, parameters, and QA criteria used to generate the taxonomic data. The [variables](http://data.neonscience.org/api/v0/documents/NEON.DP1.10081_20086_20141.001.variables.20180306T000000Z.csv) file describing contents of the taxon tables can be found in the References folder in the Data Portal’s Document Library.

FILE NAMING CONVENTIONS
-----------------------

NEON data files are named using a series of component abbreviations separated by periods. File naming conventions for NEON data files differ between NEON science teams. A file will have the same name whether it is accessed via NEON's data portal or API. Please visit https://www.neonscience.org/data-formats-conventions for a full description of the naming conventions.

ISSUE LOG
---------

This log provides a list of issues that were identified during data collection or processing, prior to publication of this data package. For a more recent log, please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10081.001.

Issue Date: 2021-01-06
Issue: Safety measures to protect personnel during the COVID-19 pandemic resulted in reduced or eliminated sampling activities for extended periods at NEON sites. Data availability may be reduced during this time.
       Date Range: 2020-03-23 to 2021-06-01
       Location(s) Affected: All
Resolution Date: 
Resolution: 

ADDITIONAL INFORMATION
----------------------

Each geneticSampleID in `sls_soilCoreCollection` may have one or more DNA extraction child records in the marker gene sequencing table `mmg_soilDnaExtraction`, each with a unique dnaSampleID. More than one dnaSampleID may exist for a single geneticSampleID if the laboratory conducts more than one DNA extraction on a sample. For each dnaSampleID, there should be one record in each taxon metadata table, `mcc_soilSeqVariantMetadata_16S` and `mcc_soilSeqVariantMetadata_ITS` for all dates within the specified date range. Queries for the expanded package will also include the taxon tables for all samples within the specified date range, with data for each dnaSampleID downloaded as a separate .csv file. The expanded package will also download the table `mcc_taxonTableLabSummary`, which includes lab summary data for all records across all date ranges. 

In the taxon table data, a given dnaSampleID for `mcc_soilSeqVariantMetadata_16S` (or ITS) is expected to generate one record for each unique sequence variant as defined by the data field taxonSequence, and the number of records per dnaSampleID should equal the number of unique sequence variants. Duplicate samples and/or missing data may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.

NEON DATA POLICY AND CITATION GUIDELINES
----------------------------------------

A citation statement is available in this data product's detail page at https://data.neonscience.org/data-products/DP1.10081.001. Please visit https://www.neonscience.org/data-policy for more information about NEON's data policy and citation guidelines.

DATA QUALITY AND VERSIONING
---------------------------

NEON data are initially published with a status of Provisional, in which updates to data and/or processing algorithms will occur on an as-needed basis, and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release, they are no longer provisional, and are associated with a stable DOI.

To learn more about provisional versus released data, please visit https://www.neonscience.org/data-revisions-releases.

POST STACKING README DOCUMENTATION
----------------------------------

Each row contains the readme filename used during stackByTable

NEON.D01.BART.DP1.10081.001.readme.20201217T040935Z.txt
NEON.D01.BART.DP1.10081.001.readme.20201217T040925Z.txt
NEON.D01.BART.DP1.10081.001.readme.20210123T023002Z.txt
NEON.D01.HARV.DP1.10081.001.readme.20201217T034750Z.txt
NEON.D01.HARV.DP1.10081.001.readme.20201217T034724Z.txt
NEON.D01.HARV.DP1.10081.001.readme.20210123T023002Z.txt
NEON.D02.SERC.DP1.10081.001.readme.20210123T023002Z.txt
NEON.D05.TREE.DP1.10081.001.readme.20210123T023002Z.txt
NEON.D07.ORNL.DP1.10081.001.readme.20210123T023002Z.txt
NEON.D08.DELA.DP1.10081.001.readme.20210123T023002Z.txt
NEON.D08.LENO.DP1.10081.001.readme.20210123T023002Z.txt

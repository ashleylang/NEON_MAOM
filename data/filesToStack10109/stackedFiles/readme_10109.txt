###################################
########### Disclaimer ############
This is the most recent readme publication based on all site-date combinations used during stackByTable.
Information specific to the query, including sites and dates, has been removed. The remaining content reflects general metadata for the data product.
All files used during stacking are listed at the bottom of this document, which includes the data publication dates.
##################################

This data package been produced by and downloaded from the National Ecological Observatory Network (NEON). NEON is funded by the National Science Foundation (Awards 0653461, 0752017, 1029808, 1138160, 1246537, 1638695, 1638696, 1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.

DATA PRODUCT INFORMATION
------------------------

ID: NEON.DOM.SITE.DP1.10109.001

Name: Soil microbe group abundances

Description: Counts and relative abundances of marker genes from total archaea, bacteria, and fungi observed by qPCR in soil microbial communities

NEON Science Team Supplier: Terrestrial Observation System

Abstract: This data product contains the quality-controlled laboratory data and metadata for NEON's soil bacterial, archaeal, and fungal group abundances analysis, which are derived from soil microbial sampling. Group abundances are quantified via qPCR on frozen, field-collected soils. For additional details, see protocol [NEON.DOC.014048](http://data.neonscience.org/api/v0/documents/NEON.DOC.014048vJ): TOS Protocol and Procedure for Soil Biogeochemical and Microbial Sampling; and science design [NEON.DOC.000908](http://data.neonscience.org/api/v0/documents/NEON.DOC.000908vB): TOS Science Design for Terrestrial Microbial Diversity.

Latency:
The expected time from data and/or sample collection in the field to data publication is as follows, for each of the data tables (in days) in the downloaded data package. See the Data Product User Guide for more information.

mga_batchResults:  14

mga_labSummary:  14

mga_soilGroupAbundances:  240

Brief Design Description: This data product was discontinued as of June 2020. Three predetermined, randomly assigned locations are selected for each sampling event within each of 10 plots distributed throughout a site; sampling locations within a plot are not re-sampled. Soil sampling occurs once (sites with short growing seasons) to three times a year (sites with longer growing seasons), with all sites sampled during the historic peak in vegetation greenness. Soil samples are collected to a maximum depth of 30 cm, with organic and mineral soils sampled separately. Subsamples of homogenized soil (rocks, roots and organic debris removed) from each of the 3 sampling locations are stored in sterile containers, frozen on dry ice in the field and shipped to an analytical facility for DNA extraction, sample preparation and qPCR analysis uses primer sets targeting the small subunit of the ribosomal RNA gene.

Brief Study Area Description: These data were collected at all NEON terrestrial sites.

Keywords: group abundances, fungi, microbe abundances, quantitative polymerase chain reaction (qPCR), bacteria, microbes, soil, archaea


DATA PACKAGE CONTENTS
---------------------

This data product contains up to 5 data tables:

mga_soilGroupAbundances - Laboratory results of gene copy number data in soil samples
mga_soilLabSummary - Summary data on laboratory methods for qPCR results in soil samples
mga_soilBatchResults - Batch-level results of analysis of gene copy number in soil samples
mga_batchResults - Batch-level results of analysis of gene copy number in soil samples
mga_labSummary - Summary data on laboratory methods for qPCR results in soil samples
If data are unavailable for the particular sites and dates queried, some tables may be absent.
Basic download package definition: The basic package includes the group abundance data.

Expanded download package definition: The expanded package includes two additional tables that provide batch level metadata and summary information about the lab methodology.

FILE NAMING CONVENTIONS
-----------------------

NEON data files are named using a series of component abbreviations separated by periods. File naming conventions for NEON data files differ between NEON science teams. A file will have the same name whether it is accessed via NEON's data portal or API. Please visit https://www.neonscience.org/data-formats-conventions for a full description of the naming conventions.

ISSUE LOG
---------

This log provides a list of issues that were identified during data collection or processing, prior to publication of this data package. For a more recent log, please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10109.001.

Issue Date: 2020-06-01
Issue: After consultation with external working group community members and the NSF, The Soil Microbe Group Abundances data product was discontinued in 2020, with the last field samples having associated group abundance data in 10-2018. Users who are interested in generating this data from NEON samples may submit a request for samples or DNA extracts from the NEON Biorepository. Alternatively, the Soil Microbe Biomass data product (DP1.10104) may be utilized as a similar measurement of the quantities of microbes in soils.
       Date Range: 2018-11-01 to 2020-06-01
       Location(s) Affected: All terrestrial sites
Resolution Date: 2020-06-01
Resolution: Data Product discontinued

ADDITIONAL INFORMATION
----------------------

Queries for this data product will return data from `mga_soilGroupAbundances` for all dates within the specified date range, as well as data from all dates for the `mga_batchResults` and `mga_labSummary` (if the expanded package is selected). Note that both soil and aquatic samples may be analyzed in the same batch and using the same methods. As such, batch and lab summary tables may include data for soil and aquatic samples. A given `mga_soilGroupAbundances.dnaSampleID` is expected to generate one record per targetTaxonGroup. Duplicate samples and/or missing data may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.

NEON DATA POLICY AND CITATION GUIDELINES
----------------------------------------

A citation statement is available in this data product's detail page at https://data.neonscience.org/data-products/DP1.10109.001. Please visit https://www.neonscience.org/data-policy for more information about NEON's data policy and citation guidelines.

DATA QUALITY AND VERSIONING
---------------------------

NEON data are initially published with a status of Provisional, in which updates to data and/or processing algorithms will occur on an as-needed basis, and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release, they are no longer provisional, and are associated with a stable DOI.

To learn more about provisional versus released data, please visit https://www.neonscience.org/data-revisions-releases.

POST STACKING README DOCUMENTATION
----------------------------------

Each row contains the readme filename used during stackByTable

NEON.D01.BART.DP1.10109.001.readme.20210123T023002Z.txt
NEON.D01.HARV.DP1.10109.001.readme.20210123T023002Z.txt
NEON.D02.SERC.DP1.10109.001.readme.20210123T023002Z.txt
NEON.D05.TREE.DP1.10109.001.readme.20210123T023002Z.txt
NEON.D07.ORNL.DP1.10109.001.readme.20210123T023002Z.txt
NEON.D08.DELA.DP1.10109.001.readme.20210123T023002Z.txt
NEON.D08.LENO.DP1.10109.001.readme.20210123T023002Z.txt

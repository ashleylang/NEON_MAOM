###################################
########### Disclaimer ############
This is the most recent readme publication based on all site-date combinations used during stackByTable.
Information specific to the query, including sites and dates, has been removed. The remaining content reflects general metadata for the data product.
All files used during stacking are listed at the bottom of this document, which includes the data publication dates.
##################################

This data package been produced by and downloaded from the National Ecological Observatory Network (NEON). NEON is funded by the National Science Foundation (Awards 0653461, 0752017, 1029808, 1138160, 1246537, 1638695, 1638696, 1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.

DATA PRODUCT INFORMATION
------------------------

ID: NEON.DOM.SITE.DP1.10104.001

Name: Soil microbe biomass

Description: Quantitative abundance of microbes in soil samples

NEON Science Team Supplier: Terrestrial Observation System

Abstract: This data product contains the quality-controlled laboratory data and metadata for microbial biomass derived from soil microbial sampling. Microbial biomass is measured by phospholipid fatty acid (PLFA) analysis, in which a set of microbial lipid biomarkers is extracted and quantified using either Gas Chromatography (GC) or Gas Chromatography-Mass Spectrometry (GS-MS).  The results are provided as the quantities of individual microbial lipids as well as the total of all measured phospholipids within a sample. For additional details, see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.

Latency:
The expected time from data and/or sample collection in the field to data publication is as follows, for each of the data tables (in days) in the downloaded data package. See the Data Product User Guide for more information.

sme_batchResults:  14

sme_labSummary:  14

sme_microbialBiomass:  240

Brief Design Description: Soil sampling occurs annually at a minimum of one site per domain and once (sites with short growing seasons) to three times per year (sites with longer growing seasons), with collections occurring at every sampled site during the historic peak in vegetation greenness. Three pre-determined, randomly assigned locations are selected for each sampling event within each of 10 plots distributed throughout a site; sampling locations within a plot are not re-sampled. Soil samples are collected to a maximum depth of 30 cm, with organic and mineral soils sampled separately. The same samples are used for measurement of soil physical and chemical properties to maintain temporal and spatial connectivity. Subsamples of homogenized soil are either sieved (mineral soils), or picked of coarse debris such as rocks, roots and organic material (organic soils) and 5-10g are transferred to cryo-safe vials. The samples are frozen and shipped on dry ice to an analytical facility, where freeze-drying, PLFA extraction and GC analysis is performed. Laboratory data are passed through the NEON automated ingest process, undergo additional QAQC testing, and quality-checked data are published on the NEON data portal.

Brief Study Area Description: These data are collected at all NEON terrestrial sites.

Keywords: phospholipid fatty acid (PFLA), abundance, bacteria, fungi, biomass, soil, function, microbes


DATA PACKAGE CONTENTS
---------------------

This data product contains up to 3 data tables:

sme_microbialBiomass - Laboratory results of microbial biomass data
sme_batchResults - Microbial biomass batch-level data
sme_labSummary - Long-term uncertainty values for soil microbial biomass analysis
If data are unavailable for the particular sites and dates queried, some tables may be absent.
Basic download package definition: The basic package includes the microbial biomass analysis results.

Expanded download package definition: The expanded packaged includes two additional summary data tables. One table provides batch-level metadata for a set of samples analyzed in the same batch. The second table provides long-term precision and accuracy metadata on the methods and instrumentation.

FILE NAMING CONVENTIONS
-----------------------

NEON data files are named using a series of component abbreviations separated by periods. File naming conventions for NEON data files differ between NEON science teams. A file will have the same name whether it is accessed via NEON's data portal or API. Please visit https://www.neonscience.org/data-formats-conventions for a full description of the naming conventions.

ISSUE LOG
---------

This log provides a list of issues that were identified during data collection or processing, prior to publication of this data package. For a more recent log, please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10104.001.

Issue Date: 2020-11-09
Issue: Discontinuation of the Soil microbe group abundances data product (DP1.10109) resulted in a gap in the spatial and temporal resolution of measurements of microbial quantities in NEON soils.
       Date Range: 2018-10-01 to 2020-01-01
       Location(s) Affected: All terrestrial sites
Resolution Date: 2020-01-01
Resolution: In 2020, the frequency of soil microbe biomass sample collection was increased. Frequency was originally every five years per site during coordinated microbes-biogeochemistry sampling bouts and has been updated to occur annually at a minimum of 1 site per domain as well as during coordinated microbes-biogeochemistry sampling bouts.

ADDITIONAL INFORMATION
----------------------

Queries for the basic data product package will return microbial biomass data in the table `sme_microbialBiomass` for all dates within the specified date range. Queries for the expanded package will also return data from all dates for `sme_batchResults` and `sme_labSummary`. A given biomassID for `sme_microbialBiomass` is expected to generate one record. The `sme_microbialBiomass` table can be joined to other soil sampling data by joining the biomassID to  table `sls_soilCoreCollection`, in the Soil physical and chemical properties, periodic data product. Duplicate samples and/or missing data may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.

NEON DATA POLICY AND CITATION GUIDELINES
----------------------------------------

A citation statement is available in this data product's detail page at https://data.neonscience.org/data-products/DP1.10104.001. Please visit https://www.neonscience.org/data-policy for more information about NEON's data policy and citation guidelines.

DATA QUALITY AND VERSIONING
---------------------------

NEON data are initially published with a status of Provisional, in which updates to data and/or processing algorithms will occur on an as-needed basis, and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release, they are no longer provisional, and are associated with a stable DOI.

To learn more about provisional versus released data, please visit https://www.neonscience.org/data-revisions-releases.

POST STACKING README DOCUMENTATION
----------------------------------

Each row contains the readme filename used during stackByTable

NEON.D01.HARV.DP1.10104.001.readme.20210123T023002Z.txt
NEON.D01.HARV.DP1.10104.001.readme.20210504T170303Z.txt
NEON.D05.TREE.DP1.10104.001.readme.20210504T165605Z.txt
NEON.D07.ORNL.DP1.10104.001.readme.20210123T023002Z.txt
NEON.D07.ORNL.DP1.10104.001.readme.20210412T165216Z.txt
NEON.D08.DELA.DP1.10104.001.readme.20210123T023002Z.txt
NEON.D08.LENO.DP1.10104.001.readme.20210123T023002Z.txt

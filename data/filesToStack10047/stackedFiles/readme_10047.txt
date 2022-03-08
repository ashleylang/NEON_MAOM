###################################
########### Disclaimer ############
This is the most recent readme publication based on all site-date combinations used during stackByTable.
Information specific to the query, including sites and dates, has been removed. The remaining content reflects general metadata for the data product.
All files used during stacking are listed at the bottom of this document, which includes the data publication dates.
##################################

This data package been produced by and downloaded from the National Ecological Observatory Network (NEON). NEON is funded by the National Science Foundation (Awards 0653461, 0752017, 1029808, 1138160, 1246537, 1638695, 1638696, 1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.

DATA PRODUCT INFORMATION
------------------------

ID: NEON.DOM.SITE.DP1.10047.001

Name: Soil physical and chemical properties, distributed initial characterization

Description: Soil physical and chemical properties measured by the NRCS as part of initial site characterization activities at NEON sites. Data are reported by pedogenic horizon, generally for the top 1m of the soil profile. Also see distributed periodic and Megapit soil data.

NEON Science Team Supplier: Terrestrial Observation System

Abstract: This data product contains quality-controlled, native sampling resolution taxonomic, physical, and chemical data from soils measured during the course of an initial soil characterization effort at each NEON site. This effort is executed by the Soil Science Division of the Natural Resources Conservation Service (NRCS), in partnership with the USDA Agriculture Research Service (ARS). For additional details, see the user guide listed in the Documentation section below. Queries for this data product will return field collection metadata, soil taxonomy, bulk density, particle size distribution, and a host of geochemical measurements on a per horizon basis, along with a summary table of external lab precision and accuracy in the expanded package. Associated with these data are soil pedon descriptions and narrative summary documents, which place the plot-level data into site-level context. These documents can be found in the [NEON Document Library](http://data.neonscience.org/documents), in the folder Soil Characterization Summaries > Distributed plots.

Latency:
Data were collected once, at the establishment of each site. Data were published within one year of collection, and future collections at existing sites are not expected.

Brief Design Description: At each site, up to 4 Tower and 30 Distributed plots are sampled, with number of plots determined by NRCS based on site variability and number of soil map units present. In most Distributed base plots, a single 1 m x 1 m x 1 m soil pit is excavated. In Tower plots and sites where pit sampling is not permitted, several 10 cm diameter, 1 m deep cores are collected from within a 1 m x 1 m square (where possible). Upon excavating a pit or collecting cores, NRCS describes the profile and all major horizons, assesses coarse fragment volumes, collects bulk density samples (most often by the clod method), then collects enough material to conduct all physical and geochemical laboratory analyses. Field sampling and descriptions follow the methods outlined in the NRCS Field Book for Describing and Sampling Soils, version 3.0. Laboratory analyses are conducted at the Kellogg Soil Survey Laboratory in Lincoln, Nebraska following the standard operating procedures outlined in the Soil Survey Laboratory Methods Manual, Report No. 42, Version 5, 2014. Some horizons do not have bulk density measurements - this includes plots and sites where cores were taken instead of pits and horizons where the bulk density sample was destroyed, lost, or of poor quality.

Brief Study Area Description: These data are collected at all NEON terrestrial sites.

Keywords: soil development, soil series, rocks, silt, soil characterization, soil taxonomy, weathering, soil properties, soil cores, soil texture, soil pits, clay, pedons, soil horizons, coarse fragments, bulk density, soil order, sand, biogeochemistry


DATA PACKAGE CONTENTS
---------------------

This data product contains up to 6 data tables:

spc_perplot - Soil initial characterization field data collected per plot
spc_perhorizon - Soil initial characterization field data collected per horizon
spc_bulkdensity - Soil initial characterization bulk density measurements
spc_particlesize - Soil initial characterization particle size measurements
spc_biogeochem - Soil initial characterization chemical measurements
spc_externalLabSummary - Long-term uncertainty values for soil initial characterization laboratory analyses
If data are unavailable for the particular sites and dates queried, some tables may be absent.
Basic download package definition: The basic data package includes the primary measurements.

Expanded download package definition: The expanded data package includes all of the data in the basic package, plus an additional data table of accuracy data from the analytical laboratory.

FILE NAMING CONVENTIONS
-----------------------

NEON data files are named using a series of component abbreviations separated by periods. File naming conventions for NEON data files differ between NEON science teams. A file will have the same name whether it is accessed via NEON's data portal or API. Please visit https://www.neonscience.org/data-formats-conventions for a full description of the naming conventions.

ISSUE LOG
---------

This log provides a list of issues that were identified during data collection or processing, prior to publication of this data package. For a more recent log, please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10047.001.

Issue Date: 2020-10-02
Issue: Until October 2020, soil physical and chemical properties were published as separate data products.
       Date Range: 2012-01-01 to 2020-10-02
       Location(s) Affected: All terrestrial sites.
Resolution Date: 2020-10-06
Resolution: In October 2020, data tables for chemical and physical properties were bundled together in a single data product for improved usability. This applies to all existing data.

Issue Date: 2020-10-02
Issue: NEON was reporting the units for several terms related to cation exchange and aluminum as centimoles per kilogram. However, in consultation with the USDA-NRCS, we determined that those units were not correct.
       Date Range: 2015-01-01 to 2018-12-31
       Location(s) Affected: All terrestrial sites.
Resolution Date: 2020-10-06
Resolution: The units were updated to centimoles charge per kilogram.

ADDITIONAL INFORMATION
----------------------

Each soil pit sampled yields a unique pitID in the `spc_perplot` table. A record from `spc_perplot` then has several child records, one for each horizon in the pit, in `spc_perhorizon`. Each horizon record from `spc_perhorizon` is expected to have zero or one child records in `spc_bulkdensity`, `spc_particlesize`, and `spc_biogeochem`. Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.

NEON DATA POLICY AND CITATION GUIDELINES
----------------------------------------

A citation statement is available in this data product's detail page at https://data.neonscience.org/data-products/DP1.10047.001. Please visit https://www.neonscience.org/data-policy for more information about NEON's data policy and citation guidelines.

DATA QUALITY AND VERSIONING
---------------------------

NEON data are initially published with a status of Provisional, in which updates to data and/or processing algorithms will occur on an as-needed basis, and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release, they are no longer provisional, and are associated with a stable DOI.

To learn more about provisional versus released data, please visit https://www.neonscience.org/data-revisions-releases.

POST STACKING README DOCUMENTATION
----------------------------------

Each row contains the readme filename used during stackByTable

NEON.D01.BART.DP1.10047.001.readme.20210123T023002Z.txt
NEON.D01.HARV.DP1.10047.001.readme.20210123T023002Z.txt
NEON.D02.SERC.DP1.10047.001.readme.20210123T023002Z.txt
NEON.D05.TREE.DP1.10047.001.readme.20210123T023002Z.txt
NEON.D07.ORNL.DP1.10047.001.readme.20210123T023002Z.txt
NEON.D08.DELA.DP1.10047.001.readme.20210123T023002Z.txt
NEON.D08.LENO.DP1.10047.001.readme.20210123T023002Z.txt

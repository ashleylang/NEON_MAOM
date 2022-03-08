###################################
########### Disclaimer ############
This is the most recent readme publication based on all site-date combinations used during stackByTable.
Information specific to the query, including sites and dates, has been removed. The remaining content reflects general metadata for the data product.
All files used during stacking are listed at the bottom of this document, which includes the data publication dates.
##################################

This data package been produced by and downloaded from the National Ecological Observatory Network (NEON). NEON is funded by the National Science Foundation (Awards 0653461, 0752017, 1029808, 1138160, 1246537, 1638695, 1638696, 1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.



DATA PRODUCT INFORMATION

------------------------



ID: NEON.DOM.SITE.DP1.10066.001



Name: Root biomass and chemistry, Megapit



Description: Standing stock of fine and coarse root biomass plus root carbon (C) and nitrogen (N) concentrations and stable isotopes from soil Megapits. Samples were collected in 10cm increments for the first 1m depth and 20cm increments thereafter to 2m depth. Ground, oven-dried root tissues from each depth increment are available for request from the NEON Biorepository. See the soil Megapit data product (DP1.00096.001) for physical and chemical data from Megapit soils.



NEON Science Team Supplier: Terrestrial Observation System



Abstract: This data product contains the quality-controlled, native sampling resolution data from NEON's belowground plant biomass stock and chemistry measurements from Megapits. Soil samples were collected at 10 cm depth increments to the first 100 cm below the surface, then 20 cm depth increments thereafter, along three vertical profiles from a single temporary soil pit at a location expected to be representative of NEON sensor-based soil plots. This sampling activity is expected to occur once at each NEON terrestrial site. Root material is sorted, dried, weighed, and analyzed, then any excess root sample material is archived in the NEON Biorepository and are available on request. For additional details, see the user guide, protocols, and science design listed in the Documentation section below. Products resulting from this sampling include root biomass by size class and live/dead status, as well as root chemistry and stable isotope ratios. A summary table of external lab precision and accuracy is included in the expanded package.

Latency:
Data were collected once, at the establishment of each site. Data were published within one year of collection, and future collections at existing sites are not expected.



Brief Design Description: Each site is sampled a single time. At each site, a soil Megapit is dug in the dominant soil type to a maximum depth of 2 m. On the exposed face of the soil pit, a tape measure visually divides the soil profile into 10 cm depth increments. Each soil pit has three vertically-oriented sampling profiles, roughly corresponding to the left, center, and right of the pit sampling face. These profiles are referred to as profile number 1, 2 and 3, respectively. From each profile, a block of soil is removed from each 10 cm depth increment, starting from the surface down to 100 cm. Once a depth of 100 cm is reached, the each profile is divided into 20 cm depth increments. By the end of sampling, up to 45 soil samples are collected, 15 per profile. Roots are sieved and then divided into four categories distinguishing between status (alive or dead) and size (> 2mm and < 2 mm, unless otherwise noted). Once roots are weighed and dried, they are sent to an external laboratory for analysis of carbon and nitrogen concentrations and stable isotopes. Any remaining root material is held in the NEON Biorepository and available upon request.



Brief Study Area Description: These data are collected at all NEON terrestrial sites.



Sensor(s): 



Keywords: soil cores, megapit, roots, carbon cycle, net primary productivity (NPP), production, belowground net primary productivity (BNPP), root distribution profile, biomass, soil pits, plant productivity, root biomass, soil properties, gross primary productivity (GPP), plants






DATA PACKAGE CONTENTS

---------------------
This data product contains up to 5 data tables:

mpr_perpitprofile - Data collected per megapit profile
mpr_perdepthincrement - Data collected per depth increment
mpr_perrootsample - Data collected per root sample
bgc_CNiso_externalSummary - Long-term uncertainty values for analysis of carbon and nitrogen concentrations and stable isotopes
mpr_carbonNitrogen - External lab analysis of carbon and nitrogen concentrations in roots
If data are unavailable for the particular sites and dates queried, some tables may be absent.
Basic download package definition: The basic data package includes the primary measurements.



Expanded download package definition: The expanded package contains an additional data table documenting accuracy and precision from the analytical laboratory.





FILE NAMING CONVENTIONS
-----------------------

NEON data files are named using a series of component abbreviations separated by periods. File naming conventions for NEON data files differ between NEON science teams. A file will have the same name whether it is accessed via NEON's data portal or API. Please visit https://www.neonscience.org/data-formats-conventions for a full description of the naming conventions.

ISSUE LOG

----------



This log provides a list of issues that were identified during data collection or processing, prior to publication of this data package. For a more recent log, please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10066.001.



Issue Date: 2020-12-01
Issue: Due to a miscommunication, samples analyzed for carbon (C) and nitrogen (N) concentrations and stable isotopes were not re-dried prior to weighing and analysis at the external lab. While all NEON root samples collected from soil Megapits were dried at 65C following sorting, they were sometimes then stored in paper bags or coin envelopes for weeks to months before being ground, transferred to vials, and shipped. During this time they may have accumulated moisture, especially in humid areas. Subsequent testing revealed that %C data are likely underestimated by 1.5-2.5% due to this lack of re-drying prior to analysis. As vegetation samples tend to have high %C (20% - 55%), this bias may have only minor impacts on many analyses, but is something for end users to keep in mind. For the other parameters (%N, C:N, d15N, d13C), testing suggests there were no detectable differences between re-dried samples and originals.
       Date Range: 2012-01-01 to 2019-01-01
       Location(s) Affected: All sites with root chemistry measurements from Megapits in this date range, with the exception of GUAN and LAJA whose tissues were re-dried for permitting/quarantine reasons.
Resolution Date: 2020-11-10
Resolution: Affected data have been flagged with dataQF = dryingProtocolError in the `mpr_carbonNitrogen` table.

Issue Date: 2020-10-02
Issue: Until October 2020, root biomass, chemistry, and stable isotopes were published as separate data products.
       Date Range: 2012-01-01 to 2020-10-06
       Location(s) Affected: All terrestrial sites.
Resolution Date: 2020-10-06
Resolution: In October 2020, data tables for chemistry and isotopes were bundled with the sampling and biomass data tables in a single data product for improved usability. This applies to all existing data.

Issue Date: 2020-01-21
Issue: The units for root biomass were inconsistently reported, both within and across NEON root data products.
       Date Range: 2012-01-01 to 2018-12-31
       Location(s) Affected: All terrestrial NEON sites where Megapit root data were collected (n = 44 out of 47)
Resolution Date: 2020-01-21
Resolution: We have standardized the root data to present mass in grams (g), mass per unit area in grams per meter squared (g/m2), and mass per unit volume in grams per meter cubed (g/m3). Previous values have been updated to reflect these revised units.





ADDITIONAL INFORMATION

----------------------




Queries for this data product will return data collected during the date range specified. The protocol dictates that up to 12 records per soil Megapit are created in the `mpr_perPitProfile` table, corresponding to 3 vertical profiles, 2 root size classes, and 2 root statuses (live/dead). Each profile in `mpr_perPitProfile` can have up to 15 child records in `mpr_perDepthIncrement`, one for each of up to 15 depth increments per vertical profile. Each record in `mpr_perDepthIncrement` creates up to 4 child records in `mpr_perRootSample`, one record per root size class per root status. Each record from `mpr_perRootSample` with sufficient sample mass is expected to appear up to two times (if analytical replicates were conducted) in `mpr_carbonNitrogen`. There should only be one instance per sampleID x analyticalRepNumber combination, but duplicates may exist where protocol and/or data entry aberrations have occurred. Users should check data carefully for anomalies before analyzing data.



NEON DATA POLICY AND CITATION GUIDELINES

----------------------------------------



A citation statement is available in this data product's detail page at https://data.neonscience.org/data-products/DP1.10066.001. Please visit https://www.neonscience.org/data-policy for more information about NEON's data policy and citation guidelines.



DATA QUALITY AND VERSIONING
---------------------------

NEON data are initially published with a status of Provisional, in which updates to data and/or processing algorithms will occur on an as-needed basis, and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release, they are no longer provisional, and are associated with a stable DOI.

To learn more about provisional versus released data, please visit https://www.neonscience.org/data-revisions-releases.

POST STACKING README DOCUMENTATION
----------------------------------

Each row contains the readme filename used during stackByTable

NEON.D01.BART.DP1.10066.001.readme.20220120T173946Z.txt
NEON.D01.HARV.DP1.10066.001.readme.20220120T173946Z.txt
NEON.D02.SERC.DP1.10066.001.readme.20220120T173946Z.txt
NEON.D05.TREE.DP1.10066.001.readme.20220120T173946Z.txt
NEON.D07.ORNL.DP1.10066.001.readme.20220120T173946Z.txt
NEON.D08.DELA.DP1.10066.001.readme.20220120T173946Z.txt
NEON.D08.LENO.DP1.10066.001.readme.20220120T173946Z.txt

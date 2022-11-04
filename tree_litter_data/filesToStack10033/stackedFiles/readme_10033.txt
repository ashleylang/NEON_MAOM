###################################
########### Disclaimer ############
This is the most recent readme publication based on all site-date combinations used during stackByTable.
Information specific to the query, including sites and dates, has been removed. The remaining content reflects general metadata for the data product.
##################################

This data package been produced by and downloaded from the National Ecological Observatory Network (NEON). NEON is funded by the National Science Foundation (Awards 0653461, 0752017, 1029808, 1138160, 1246537, 1638695, 1638696, 1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.
DATA PRODUCT INFORMATION
------------------------
ID: NEON.DOM.SITE.DP1.10033.001
Name: Litterfall and fine woody debris production and chemistry
Description: Dry weight of litterfall and fine woody debris collected from elevated and ground traps, sorted to functional group, as well as periodic measurements of litter chemistry and stable isotopes.
NEON Science Team Supplier: Terrestrial Observation System
Abstract: This data product contains the quality-controlled, native sampling resolution data from NEON's Litterfall and fine woody debris sampling. Litter is defined as material that is dropped from the forest canopy and has a butt end diameter <2cm and a length <50 cm; this material is collected in elevated 0.5m2 PVC traps. Fine woody debris is defined as material that is dropped from the forest canopy and has a butt end diameter <2cm and a length >50 cm; this material is collected in ground traps as longer material is not reliably collected by the elevated traps. Following field collection, each sample is sorted by functional group, dried and weighed. After sorting litter by functional group, needles and leaves from elevated traps from select bouts are sent for chemical analysis, with excess material archived in the NEON Biorepository and available upon request. For additional details, see the user guides, protocols, and science design listed in the Documentation section below. Products resulting from this sampling include mass of litterfall and fine woody debris by functional group as well as litter chemistry and stable isotope ratios. Summary tables of external lab precision and accuracy are included in the expanded package.
Latency:
The expected time from data and/or sample collection in the field to data publication is as follows, for each of the data tables (in days) in the downloaded data package. See the Data Product User Guides for more information.
bgc\_CNiso\_externalSummary: 30
lig_externalSummary: 30
ltr_chemistrySubsampling: 60
ltr_fielddata: 60
ltr_litterCarbonNitrogen: 270
ltr_litterLignin: 180
ltr_massdata: 60
ltr_pertrap: 30
Brief Design Description: Each qualifying tower plot in forested ecosystems has 0-2 elevated traps and 1-2 ground traps deployed. Ground traps are sampled annually. Sampling interval of elevated litter traps is variable by dominant overstory vegetation. Deciduous forests are sampled once in the spring then multiple times during fall senescence; evergreen and coniferous forests are sampled year round at monthly intervals. Traps are consistent with those used by the Smithsonian Center for Tropical Forest Science (CTFS). Mass data for each collection event are measured separately for functional groups: Leaves, Needles, Twigs/branches, Woody material, Seeds, Flowers and other non-woody reproductive structures, Other, and Mixed (unsorted). Once every five years, leaf and needle samples from elevated traps from a single collection event are analyzed for carbon and nitrogen concentrations and stable isotopes as well as lignin concentrations.
Brief Study Area Description: These data are collected at NEON terrestrial sites with overstory vegetation.
Sensor(s): 
Keywords: litterfall, biomass, turnover, plant productivity, leaves, production, senescent, net primary productivity (NPP), detritus, carbon cycle, fine woody debris, gross primary productivity (GPP), litter, vegetation
Domain: D08
DATA PACKAGE CONTENTS
---------------------
This folder contains the following documentation files:
This data product contains up to 8 data tables:
- Term descriptions, data types, and units: NEON.D08.LENO.DP1.10033.001.variables.20220926T161525Z.csv
ltr_fielddata - Field collection details and sample tracking
ltr_massdata - Dry mass of litter and fine woody debris components per trap per bout
ltr_pertrap - Record of trap establishment, contains date, trap type and location
ltr_chemistrySubsampling - Identifiers for subsamples created for chemical analyses or archive
ltr_litterCarbonNitrogen - External lab analysis of carbon and nitrogen concentrations in litter
ltr_litterLignin - External lab analysis of lignin concentrations in litter
-----------------------
NEON data files are named using a series of component abbreviations separated by periods. File naming conventions for NEON data files differ between NEON science teams. A file will have the same name whether it is accessed via NEON's data portal or API. Please visit https://www.neonscience.org/data-formats-conventions for a full description of the naming conventions.
ISSUE LOG
----------
This log provides a list of issues that were identified during data collection or processing, prior to publication of this data package. For a more recent log, please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10033.001.
Issue Date: 2022-09-13
Issue: Severe flooding destroyed several roads into Yellowstone National Park in June 2022, making the YELL and BLDE sites inaccessible to NEON staff. Observational data collection was halted during this time. Canceled data collection events are indicated in data records via the samplingImpractical field.
       Date Range: 2022-06-12 to 2022-12-31
       Location(s) Affected: YELL
Resolution Date: 
Resolution: 
Issue Date: 2020-11-19
Issue: Safety measures to protect personnel during the COVID-19 pandemic resulted in reduced or canceled sampling activities for extended periods at NEON sites. Data availability may be reduced during this time.
       Date Range: 2020-03-23 to 2021-12-31
       Location(s) Affected: All
Resolution Date: 2021-12-31
Resolution: The primary impact of the pandemic on observational data was reduced data collection. Training procedures and data quality reviews were maintained throughout the pandemic, although some previously in-person training was conducted virtually.  Scheduled measurements and sampling that were not carried out due to COVID-19 or any other causes are indicated in data records via the samplingImpractical data field.
Issue Date: 2021-02-16
Issue: Severely limited elevated litter trap collection for the 2020 season. Because of extended litter collection periods due to sampling limitations during COVID restrictions, the incidence of litter trap disturbance by resident black bears was unusually high. Over 2 collection bouts (40 traps total), only 5 traps were successfully collected in both bouts. It is not recommended these data be used to calculate productivity for the 2020 sampling year at GRSM.
       Date Range: 2020-01-01 to 2021-01-01
       Location(s) Affected: GRSM
Resolution Date: 2021-02-16
Resolution: Litter collection frequency returned to more normal levels as of the 2021 field season.
Issue Date: 2020-12-01
Issue: Due to a miscommunication, samples analyzed for carbon (C) and nitrogen (N) concentrations and stable isotopes were not re-dried prior to weighing and analysis at the external lab. While all NEON litterfall samples are dried at 65C in the domain labs, they are sometimes then stored in paper bags or coin envelopes for weeks to months before being ground, transferred to vials, and shipped. During this time they may accumulate moisture, especially in humid areas. Subsequent testing revealed that %C data are likely underestimated by 1.5-2.5% due to this lack of re-drying prior to analysis. As vegetation samples tend to have high %C (20% - 55%), this bias may have only minor impacts on many analyses, but is something for end users to keep in mind. For the other parameters (%N, C:N, d15N, d13C), testing suggests there were no detectable differences between re-dried samples and originals.
       Date Range: 2016-01-01 to 2020-08-15
       Location(s) Affected: All sites with litterfall chemistry measurements in this date range, with the exception of GUAN and PUUM whose tissues were re-dried for permitting/quarantine reasons.
Resolution Date: 2020-11-10
Resolution: Affected data have been flagged with dataQF = dryingProtocolError in the `ltr_litterCarbonNitrogen` table. For sample analysis dates starting in November 2020, all carbon-nitrogen samples are re-dried at 65C prior to analysis to drive out any residual moisture and improve data accuracy for % C. Samples collected in 2020 may have been analyzed before or after the change; check dataQF to determine which individual samples are affected.
Issue Date: 2020-10-02
Issue: Until October 2020, litter biomass, chemistry, and stable isotopes were published as separate data products.
       Date Range: 2016-01-01 to 2020-10-06
       Location(s) Affected: All terrestrial sites.
Resolution Date: 2020-10-06
Resolution: In October 2020, data tables for chemistry and isotopes were bundled with the sampling and biomass data tables in a single data product for improved usability. This applies to all existing and future data.
Issue Date: 2020-01-01
Issue: Discontinued litterfall sampling as some plots.
       Date Range: 2016-01-01 to 2020-01-01
       Location(s) Affected: D01-BART, D01-HARV, D02-SCBI, D02-SERC, D03-JERC, D05-TREE, D05-UNDE, D07-GRSM, D07-ORNL, D08-TALL
Resolution Date: 2020-06-08
Resolution: In January 2020, litter traps were removed from a subset of plots at sites where data analyses indicated reliable site level estimates of litter production were possible with a reduced number of plots. Plots to continue sampling for litterfall were selected to maintain spatial balance across the Tower airshed. In June 2020, plot selection at these sites was revised to prioritize stratification across vegetation types.
ADDITIONAL INFORMATION
----------------------
Queries for this data product will return data from all dates for `ltr_pertrap` (which may be established many years before a litter collection event), whereas the other tables will be subset to data collected during the date range specified. The protocol dictates that each trap is established once (one expected record per `ltr_pertrap.trapID`). A record from `ltr_pertrap` may have zero or more child records in `ltr_fielddata.trapID`, depending on the date range of the data downloaded; a given `ltr_fielddata.trapID` is expected to be sampled zero or one times per collectDate (local time). A record from `ltr_fielddata` may have zero (if no litter collected) or more child records in `ltr_massdata` depending on the functional groups contained in the trap and whether reweighing occurred for QA purposes. A record from `ltr_massdata` may have zero (if not sent for chemistry analyses) or one child record in `ltr_chemistrySubsampling`. Chemistry subsamples may appear one or more times in `ltr_litterCarbonNitrogen` and `ltr_litterLignin`, depending on whether analytical replicates were conducted or if C and N were analyzed separately. Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check carefully for anomalies before joining tables.
NEON DATA POLICY AND CITATION GUIDELINES
----------------------------------------
A citation statement is available in this data product's detail page at https://data.neonscience.org/data-products/DP1.10033.001. Please visit https://www.neonscience.org/data-policy for more information about NEON's data policy and citation guidelines.
DATA QUALITY AND VERSIONING
---------------------------
NEON data are initially published with a status of Provisional, in which updates to data and/or processing algorithms will occur on an as-needed basis, and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release, they are no longer provisional, and are associated with a stable DOI. 
To learn more about provisional versus released data, please visit https://www.neonscience.org/data-revisions-releases.

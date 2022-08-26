###################################
########### Disclaimer ############
This is the most recent readme publication based on all site-date combinations used during stackByTable.
Information specific to the query, including sites and dates, has been removed. The remaining content reflects general metadata for the data product.
All files used during stacking are listed at the bottom of this document, which includes the data publication dates.
##################################

This data package been produced by and downloaded from the National Ecological Observatory Network (NEON). NEON is funded by the National Science Foundation (Awards 0653461, 0752017, 1029808, 1138160, 1246537, 1638695, 1638696, 1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.





DATA PRODUCT INFORMATION


------------------------





ID: NEON.DOM.SITE.DP1.10023.001





Name: Herbaceous clip harvest





Description: Dry weight of herbaceous vegetation harvested from individual clip strips, by functional type





NEON Science Team Supplier: Terrestrial Observation System





Abstract: This data product contains the quality-controlled, native sampling resolution data from NEON's Herbaceous biomass clip harvest sampling. Herbaceous vegetation is operationally defined in this protocol as non-woody plants (i.e. grasses, sedges, forbs, some bryophytes, and non-woody vines such as Convolvulus spp. and certain Rubus spp.), as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details, see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.



Latency:

The expected time from data and/or sample collection in the field to data publication is as follows, for each of the data tables (in days) in the downloaded data package. See the Data Product User Guide for more information.



hbp_massdata:  60



hbp_perbout:  60





Brief Design Description: Clip-harvest of herbaceous biomass occurs within randomly located clip-harvest strips in 20m x 20m plots or subplots. Up to 20 non-forested Distributed plots (containing 1 clip strip per plot) and up to 30 Tower plots (containing 1-4 clip strips per plot) are sampled at each site. Tower plots are sampled every year. Tower plots at ungrazed sites are sampled once per year if there is a single annual biomass peak, and twice at sites with two biomass peaks per year in order to capture both warm season and cool season production. At grazed sites, sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.





Brief Study Area Description: These data are collected at NEON terrestrial sites.





Sensor(s): 





Keywords: vegetation, productivity, clip harvest, carbon (C), production, biomass, net primary productivity (NPP), carbon cycle, gross primary productivity (GPP), sorghum, C3 photosynthesis, wheat, soybeans, barley, maize, foliage, forbs, leaves, legumes, annual net primary productivity (ANPP), graminoids, grasses, crops, C4 photosynthesis, corn, plant productivity









DATA PACKAGE CONTENTS


---------------------
This data product contains up to 2 data tables:


hbp_perbout - Herbaceous clip harvest spatial and temporal sampling information, and sampling metadata
hbp_massdata - Herbaceous clip harvest dry mass and QA dry mass data
If data are unavailable for the particular sites and dates queried, some tables may be absent.

Basic download package definition: The basic download package includes all measurements. An expanded download package is not available for this product.





Expanded download package definition: 








FILE NAMING CONVENTIONS


-----------------------





NEON data files are named using a series of component abbreviations separated by periods. File naming conventions for NEON data files differ between NEON science teams. A file will have the same name whether it is accessed via NEON's data portal or API. Please visit https://www.neonscience.org/data-formats-conventions for a full description of the naming conventions.





ISSUE LOG


----------





This log provides a list of issues that were identified during data collection or processing, prior to publication of this data package. For a more recent log, please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.





Issue Date: 2021-01-06

Issue: Safety measures to protect personnel during the COVID-19 pandemic resulted in reduced or eliminated sampling activities for extended periods at NEON sites. Data availability may be reduced during this time.

       Date Range: 2020-03-23 to 2021-06-01

       Location(s) Affected: All

Resolution Date: 

Resolution: 



Issue Date: 2020-01-01

Issue: Prior to 2020, there was no mechanism to communicate when sampling did not occur at peak biomass.

       Date Range: 2012-01-01 to 2020-02-01

       Location(s) Affected: All terrestrial sites

Resolution Date: 2020-02-01

Resolution: In 2020, NEON added the quality flag **biophysicalCriteria** to the `hbp_perbout` table to assist users in understanding that data for this product was collected when conditions were not optimal. If conditions were suboptimal – biomass was not at peak - the field **biophysicalCriteria** is populated with a value other than 'OK - no known exceptions' but the sample is generated.



Issue Date: 2020-01-01

Issue: Prior to 2020, there was no mechanism to communicate that fewer than the targeted number plots were sampled.

       Date Range: 2012-01-01 to 2020-01-01

       Location(s) Affected: All terrestrial sites

Resolution Date: 2020-01-01

Resolution: In 2020, NEON added the quality flag **samplingImpractical** to the `hbp_perbout` table – to indicated when field sampling did not occur – and `hbp_massdata` table – to indicate when collected samples could not be processed - to assist users in understanding when data for this product are temporarily missing versus permanently unavailable. Beginning in 2020, there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table, there will always be a corresponding record generated in the `hbp_massdata` table. For example, if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g., 'location flooded') in the `hbp_perbout` table, no sample is generated, and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.



Issue Date: 2019-01-01

Issue: Samples were sorted to functional groups that included the category 'Leguminous Forbs (LFB)' but qualifying individuals were not limited to forbs.

       Date Range: 2019-01-01 to 2019-01-01

       Location(s) Affected: All terrestrial sites

Resolution Date: 2019-01-01

Resolution: Leguminous forbs and nitrogen fixers < 1 cm decimeter height are sorted to the 'N-fixer (NFX)' functional group category.



Issue Date: 2018-01-01

Issue: Distributed plot sampling on three-year intervals was not aligned with sampling and data collection for other plant biomass and productivity data products.

       Date Range: 2012-01-01 to 2018-01-01

       Location(s) Affected: All terrestrial sites

Resolution Date: 2018-01-01

Resolution: Interannual sampling schedule changed to five-year intervals to coincide with other plant biomass and productivity data products.



Issue Date: 2018-01-01

Issue: At select grazed sites, the bouts not associated with peak biomass during which harvested samples are not sorted by functional group, all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.

       Date Range: 2018-01-01 to 2018-01-01

       Location(s) Affected: All terrestrial sites

Resolution Date: 2018-01-01

Resolution: Experimental investigation, statistical analysis and consultation with the external Technical Working Group resulted in a subsampling approach: part of the plot-specific clip harvest is dried and weighed but data-driven estimates of the entire sample mass are reported.



Issue Date: 2018-01-01

Issue: Consultation with the external Technical Working Group guided statistical analyses that resulted in data-driven sampling reductions at Tower plots.

       Date Range: 2018-01-01 to 2018-01-01

       Location(s) Affected: All terrestrial sites

Resolution Date: 2018-01-01

Resolution: Prior to the 2018 sampling season, all Tower plots were sampled during each bout at each site. The design modification reduced the number of Tower plots at specific sites to a sample size that maintains the capacity to detect a 20% change in interannual herbaceous biomass productivity based on three or more years of data.



Issue Date: 2018-01-01

Issue: Consultation with the external Technical Working Group guided statistical analyses that resulted in data-driven sampling reductions at sites managed for grazing.

       Date Range: 2018-01-01 to 2018-01-01

       Location(s) Affected: All terrestrial sites managed for grazing

Resolution Date: 2018-01-01

Resolution: Prior to the 2018 sampling season, all sites managed for grazing were sampled for herbaceous biomass on a 4-week interval. The design modification increased the sampling interval from 4-weeks to 8-weeks at moderately productive sites where consumption could not be detected with a 4-week interval. At grazed sites with minimal productivity, sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.







ADDITIONAL INFORMATION


----------------------







Queries for this data product for `hbp_perbout` and `hbp_massdata` files will be subset to data collected during the date range specified. A given `hbp_perbout.clipID` is expected to be sampled zero or one times per collectDate (local time). A record from `hbp_perbout` may have zero or more child records in `hbp_massdata`, depending on whether or not herbaceous material is present in the selected clip cell (indicated by the `hbp_perbout.targetTaxaPresent` field), whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`), and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.





NEON DATA POLICY AND CITATION GUIDELINES


----------------------------------------





A citation statement is available in this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001. Please visit https://www.neonscience.org/data-policy for more information about NEON's data policy and citation guidelines.





DATA QUALITY AND VERSIONING


---------------------------





NEON data are initially published with a status of Provisional, in which updates to data and/or processing algorithms will occur on an as-needed basis, and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release, they are no longer provisional, and are associated with a stable DOI. 





To learn more about provisional versus released data, please visit https://www.neonscience.org/data-revisions-releases.

POST STACKING README DOCUMENTATION
----------------------------------

Each row contains the readme filename used during stackByTable

1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
NA,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
C4 photosynthesis,soybeans,graminoids,leaves,vegetation,foliage, C3 photosynthesis, carbon cycle, gross primary productivity (GPP), biomass, grasses, corn, legumes, barley, maize, crops, carbon (C), production, net primary productivity (NPP), productivity, forbs, clip harvest, plant productivity, annual net primary productivity (ANPP),NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.BART.DP1.10023.001.variables.20220107T002953Z.csv,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
maize,annual net primary productivity (ANPP),graminoids,plant productivity,biomass,carbon cycle, production, productivity, soybeans, gross primary productivity (GPP), corn, clip harvest, C4 photosynthesis, leaves, net primary productivity (NPP), forbs, carbon (C), C3 photosynthesis, sorghum, crops, wheat, vegetation, barley, legumes,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.BART.DP1.10023.001.variables.20211221T225423Z.csv,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
production,productivity,carbon (C),crops,wheat,carbon cycle, plant productivity, gross primary productivity (GPP), C3 photosynthesis, annual net primary productivity (ANPP), maize, sorghum, barley, C4 photosynthesis, net primary productivity (NPP), biomass, graminoids, corn, legumes, soybeans, grasses, forbs, clip harvest, leaves,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.BART.DP1.10023.001.variables.20211221T224758Z.csv,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
carbon (C),corn,carbon cycle,sorghum,legumes,productivity, vegetation, plant productivity, C3 photosynthesis, soybeans, crops, net primary productivity (NPP), foliage, leaves, grasses, production, clip harvest, annual net primary productivity (ANPP), maize, biomass, wheat, graminoids, gross primary productivity (GPP), C4 photosynthesis,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.BART.DP1.10023.001.variables.20211221T202728Z.csv,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
production,barley,biomass,productivity,maize,annual net primary productivity (ANPP), leaves, plant productivity, soybeans, carbon (C), crops, sorghum, C4 photosynthesis, clip harvest, corn, grasses, graminoids, wheat, net primary productivity (NPP), foliage, C3 photosynthesis, legumes, forbs, carbon cycle,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.BART.DP1.10023.001.variables.20211221T235756Z.csv,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
vegetation,legumes,corn,annual net primary productivity (ANPP),production,forbs, leaves, grasses, maize, productivity, soybeans, net primary productivity (NPP), C4 photosynthesis, carbon cycle, carbon (C), sorghum, biomass, crops, clip harvest, graminoids, wheat, gross primary productivity (GPP), foliage, barley,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.BART.DP1.10023.001.variables.20211222T034724Z.csv,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
C3 photosynthesis,gross primary productivity (GPP),barley,soybeans,plant productivity,annual net primary productivity (ANPP), productivity, biomass, carbon (C), foliage, production, clip harvest, leaves, net primary productivity (NPP), graminoids, legumes, carbon cycle, corn, maize, vegetation, C4 photosynthesis, crops, wheat, forbs,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.BART.DP1.10023.001.variables.20211222T032534Z.csv,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220120T173946Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
NA,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
net primary productivity (NPP),legumes,vegetation,sorghum,grasses,graminoids, maize, plant productivity, barley, soybeans, crops, leaves, clip harvest, carbon (C), biomass, corn, C4 photosynthesis, C3 photosynthesis, gross primary productivity (GPP), production, wheat, forbs, productivity, carbon cycle,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
and units: NEON.D01.BART.DP1.10023.001.variables.20220627T193348Z.csv,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D01.BART.DP1.10023.001.readme.20220627T193348Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
NA,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
leaves,plant productivity,wheat,crops,soybeans,net primary productivity (NPP), barley, foliage, vegetation, C3 photosynthesis, production, biomass, corn, C4 photosynthesis, forbs, carbon cycle, sorghum, carbon (C), grasses, clip harvest, legumes, gross primary productivity (GPP), annual net primary productivity (ANPP), maize,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20211221T002255Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
crops,graminoids,soybeans,C3 photosynthesis,net primary productivity (NPP),foliage, productivity, annual net primary productivity (ANPP), carbon (C), corn, gross primary productivity (GPP), grasses, production, sorghum, barley, vegetation, C4 photosynthesis, wheat, clip harvest, legumes, maize, forbs, plant productivity, leaves,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20220107T190008Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
graminoids,gross primary productivity (GPP),barley,maize,production,grasses, plant productivity, crops, C3 photosynthesis, wheat, clip harvest, annual net primary productivity (ANPP), leaves, corn, productivity, forbs, net primary productivity (NPP), foliage, carbon cycle, soybeans, biomass, legumes, carbon (C), vegetation,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20211221T212649Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
crops,productivity,net primary productivity (NPP),forbs,foliage,plant productivity, maize, C4 photosynthesis, sorghum, leaves, carbon (C), wheat, corn, vegetation, carbon cycle, clip harvest, annual net primary productivity (ANPP), barley, production, C3 photosynthesis, soybeans, legumes, graminoids, biomass,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20211221T202847Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
vegetation,maize,graminoids,C4 photosynthesis,carbon (C),carbon cycle, leaves, C3 photosynthesis, biomass, productivity, legumes, crops, production, grasses, plant productivity, wheat, corn, sorghum, forbs, foliage, net primary productivity (NPP), clip harvest, barley, soybeans,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20211221T232515Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
clip harvest,maize,graminoids,gross primary productivity (GPP),C3 photosynthesis,plant productivity, production, vegetation, soybeans, crops, wheat, foliage, biomass, leaves, forbs, sorghum, corn, legumes, carbon (C), carbon cycle, barley, productivity, annual net primary productivity (ANPP), C4 photosynthesis,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20211221T194450Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
foliage,production,annual net primary productivity (ANPP),gross primary productivity (GPP),C3 photosynthesis,net primary productivity (NPP), carbon cycle, corn, graminoids, crops, wheat, grasses, productivity, vegetation, soybeans, carbon (C), legumes, plant productivity, forbs, sorghum, biomass, C4 photosynthesis, clip harvest, maize,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20211222T022141Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
crops,clip harvest,C4 photosynthesis,leaves,vegetation,maize, annual net primary productivity (ANPP), gross primary productivity (GPP), C3 photosynthesis, barley, sorghum, graminoids, wheat, net primary productivity (NPP), productivity, plant productivity, forbs, grasses, biomass, corn, soybeans, carbon cycle, foliage, legumes,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20211222T005214Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
gross primary productivity (GPP),plant productivity,C3 photosynthesis,barley,maize,crops, sorghum, forbs, vegetation, biomass, C4 photosynthesis, production, carbon (C), foliage, net primary productivity (NPP), clip harvest, legumes, wheat, corn, grasses, graminoids, soybeans, productivity, carbon cycle,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20211222T031406Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220120T173946Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
NA,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
wheat,corn,production,crops,forbs,leaves, legumes, graminoids, carbon (C), foliage, plant productivity, C4 photosynthesis, soybeans, maize, vegetation, biomass, barley, carbon cycle, productivity, C3 photosynthesis, gross primary productivity (GPP), clip harvest, net primary productivity (NPP), grasses,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
and units: NEON.D01.HARV.DP1.10023.001.variables.20220627T194900Z.csv,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D01.HARV.DP1.10023.001.readme.20220627T194900Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
NA,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
soybeans,barley,C3 photosynthesis,gross primary productivity (GPP),wheat,carbon cycle, legumes, foliage, net primary productivity (NPP), biomass, sorghum, production, annual net primary productivity (ANPP), graminoids, vegetation, C4 photosynthesis, leaves, grasses, plant productivity, forbs, productivity, clip harvest, maize, crops,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211221T212323Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
vegetation,graminoids,production,gross primary productivity (GPP),legumes,carbon (C), corn, C3 photosynthesis, carbon cycle, biomass, maize, annual net primary productivity (ANPP), crops, plant productivity, wheat, foliage, grasses, productivity, net primary productivity (NPP), soybeans, sorghum, barley, clip harvest, C4 photosynthesis,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211222T040653Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
leaves,sorghum,soybeans,gross primary productivity (GPP),C3 photosynthesis,wheat, production, barley, plant productivity, carbon cycle, grasses, graminoids, crops, maize, carbon (C), clip harvest, biomass, C4 photosynthesis, foliage, productivity, corn, legumes, forbs, vegetation,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211222T005021Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
barley,legumes,grasses,vegetation,corn,leaves, crops, gross primary productivity (GPP), maize, productivity, plant productivity, sorghum, C3 photosynthesis, graminoids, annual net primary productivity (ANPP), soybeans, production, forbs, foliage, carbon (C), net primary productivity (NPP), carbon cycle, C4 photosynthesis, wheat,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211222T034256Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
biomass,legumes,forbs,C4 photosynthesis,soybeans,leaves, C3 photosynthesis, carbon (C), gross primary productivity (GPP), annual net primary productivity (ANPP), maize, net primary productivity (NPP), vegetation, wheat, sorghum, clip harvest, foliage, barley, carbon cycle, corn, crops, plant productivity, production, graminoids,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211222T033440Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
annual net primary productivity (ANPP),C4 photosynthesis,vegetation,soybeans,leaves,production, legumes, foliage, carbon cycle, crops, corn, forbs, net primary productivity (NPP), grasses, sorghum, carbon (C), gross primary productivity (GPP), productivity, C3 photosynthesis, plant productivity, graminoids, barley, maize, wheat,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211221T211923Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
annual net primary productivity (ANPP),C3 photosynthesis,vegetation,grasses,graminoids,biomass, legumes, C4 photosynthesis, crops, productivity, net primary productivity (NPP), carbon (C), carbon cycle, corn, maize, wheat, plant productivity, gross primary productivity (GPP), sorghum, foliage, leaves, forbs, barley, soybeans,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211221T214003Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
forbs,C4 photosynthesis,graminoids,foliage,legumes,corn, clip harvest, biomass, maize, barley, carbon (C), sorghum, wheat, soybeans, grasses, vegetation, gross primary productivity (GPP), C3 photosynthesis, annual net primary productivity (ANPP), net primary productivity (NPP), crops, carbon cycle, plant productivity, leaves,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211222T022716Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
carbon cycle,crops,grasses,wheat,clip harvest,net primary productivity (NPP), sorghum, annual net primary productivity (ANPP), graminoids, C4 photosynthesis, plant productivity, biomass, carbon (C), productivity, leaves, gross primary productivity (GPP), C3 photosynthesis, barley, vegetation, production, corn, soybeans, maize, foliage,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211221T202626Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
foliage,carbon cycle,production,annual net primary productivity (ANPP),net primary productivity (NPP),gross primary productivity (GPP), barley, carbon (C), productivity, plant productivity, C4 photosynthesis, graminoids, leaves, forbs, soybeans, maize, crops, grasses, biomass, vegetation, wheat, legumes, corn, sorghum,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211221T211452Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
plant productivity,maize,sorghum,biomass,gross primary productivity (GPP),barley, carbon cycle, carbon (C), production, net primary productivity (NPP), vegetation, graminoids, corn, productivity, forbs, annual net primary productivity (ANPP), soybeans, leaves, grasses, C3 photosynthesis, legumes, clip harvest, foliage, C4 photosynthesis,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20211222T003858Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220120T173946Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
NA,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
net primary productivity (NPP),C3 photosynthesis,gross primary productivity (GPP),sorghum,barley,forbs, annual net primary productivity (ANPP), crops, production, graminoids, legumes, grasses, maize, foliage, vegetation, leaves, biomass, productivity, carbon cycle, carbon (C), corn, C4 photosynthesis, clip harvest, plant productivity,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20220627T200250Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T200250Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
NA,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
carbon (C),crops,biomass,wheat,maize,forbs, grasses, graminoids, corn, barley, productivity, foliage, soybeans, clip harvest, vegetation, gross primary productivity (GPP), net primary productivity (NPP), sorghum, C4 photosynthesis, production, legumes, plant productivity, leaves, C3 photosynthesis,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20220627T195243Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T195243Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
NA,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
production,grasses,barley,gross primary productivity (GPP),crops,graminoids, vegetation, net primary productivity (NPP), corn, forbs, clip harvest, C4 photosynthesis, plant productivity, carbon (C), sorghum, C3 photosynthesis, maize, soybeans, annual net primary productivity (ANPP), biomass, legumes, carbon cycle, foliage, leaves,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
and units: NEON.D02.SERC.DP1.10023.001.variables.20220627T211246Z.csv,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D02.SERC.DP1.10023.001.readme.20220627T211246Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
NA,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
C3 photosynthesis,sorghum,wheat,barley,clip harvest,vegetation, crops, soybeans, carbon (C), plant productivity, graminoids, foliage, biomass, production, net primary productivity (NPP), gross primary productivity (GPP), leaves, C4 photosynthesis, maize, corn, grasses, carbon cycle, legumes, forbs,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D05.TREE.DP1.10023.001.variables.20211222T010249Z.csv,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
crops,carbon cycle,gross primary productivity (GPP),plant productivity,maize,barley, biomass, annual net primary productivity (ANPP), soybeans, C4 photosynthesis, sorghum, grasses, graminoids, production, net primary productivity (NPP), vegetation, carbon (C), clip harvest, leaves, foliage, legumes, wheat, forbs, productivity,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D05.TREE.DP1.10023.001.variables.20211222T022145Z.csv,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
production,carbon cycle,maize,sorghum,foliage,C3 photosynthesis, graminoids, C4 photosynthesis, wheat, soybeans, carbon (C), productivity, leaves, vegetation, plant productivity, crops, grasses, net primary productivity (NPP), clip harvest, biomass, legumes, annual net primary productivity (ANPP), gross primary productivity (GPP), barley,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D05.TREE.DP1.10023.001.variables.20211221T210038Z.csv,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
net primary productivity (NPP),wheat,vegetation,carbon (C),forbs,carbon cycle, grasses, gross primary productivity (GPP), foliage, graminoids, leaves, maize, C4 photosynthesis, corn, biomass, annual net primary productivity (ANPP), sorghum, plant productivity, production, C3 photosynthesis, productivity, crops, clip harvest, barley,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D05.TREE.DP1.10023.001.variables.20211222T030515Z.csv,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
forbs,annual net primary productivity (ANPP),productivity,carbon (C),wheat,C3 photosynthesis, net primary productivity (NPP), sorghum, graminoids, maize, plant productivity, production, legumes, leaves, foliage, grasses, clip harvest, carbon cycle, barley, biomass, vegetation, crops, soybeans, C4 photosynthesis,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D05.TREE.DP1.10023.001.variables.20211222T013833Z.csv,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
production,legumes,crops,C3 photosynthesis,clip harvest,gross primary productivity (GPP), plant productivity, net primary productivity (NPP), C4 photosynthesis, graminoids, leaves, biomass, productivity, carbon cycle, sorghum, vegetation, foliage, barley, soybeans, grasses, corn, maize, carbon (C), annual net primary productivity (ANPP),NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D05.TREE.DP1.10023.001.variables.20211221T202642Z.csv,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
production,carbon (C),maize,barley,crops,sorghum, legumes, forbs, wheat, grasses, soybeans, corn, C4 photosynthesis, C3 photosynthesis, annual net primary productivity (ANPP), plant productivity, net primary productivity (NPP), vegetation, productivity, biomass, clip harvest, gross primary productivity (GPP), leaves, foliage,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D05.TREE.DP1.10023.001.variables.20211221T204239Z.csv,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220120T173946Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
NA,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
annual net primary productivity (ANPP),wheat,vegetation,gross primary productivity (GPP),legumes,soybeans, plant productivity, crops, biomass, net primary productivity (NPP), maize, foliage, C4 photosynthesis, sorghum, productivity, production, corn, carbon (C), carbon cycle, clip harvest, grasses, C3 photosynthesis, leaves, barley,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
and units: NEON.D05.TREE.DP1.10023.001.variables.20220627T193857Z.csv,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D05.TREE.DP1.10023.001.readme.20220627T193857Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
NA,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
grasses,leaves,corn,wheat,foliage,C3 photosynthesis, graminoids, net primary productivity (NPP), crops, plant productivity, annual net primary productivity (ANPP), legumes, production, forbs, C4 photosynthesis, maize, sorghum, biomass, gross primary productivity (GPP), soybeans, carbon (C), vegetation, clip harvest, carbon cycle,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D07.ORNL.DP1.10023.001.variables.20220108T190333Z.csv,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
maize,production,plant productivity,forbs,C4 photosynthesis,leaves, sorghum, legumes, barley, vegetation, soybeans, gross primary productivity (GPP), carbon (C), corn, carbon cycle, wheat, net primary productivity (NPP), graminoids, foliage, clip harvest, C3 photosynthesis, annual net primary productivity (ANPP), grasses, productivity,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D07.ORNL.DP1.10023.001.variables.20220108T185944Z.csv,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
clip harvest,sorghum,C3 photosynthesis,foliage,wheat,production, soybeans, corn, plant productivity, forbs, barley, biomass, maize, graminoids, legumes, leaves, annual net primary productivity (ANPP), net primary productivity (NPP), crops, carbon cycle, C4 photosynthesis, grasses, vegetation, gross primary productivity (GPP),NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D07.ORNL.DP1.10023.001.variables.20211222T012817Z.csv,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
annual net primary productivity (ANPP),barley,clip harvest,carbon (C),sorghum,carbon cycle, biomass, C4 photosynthesis, C3 photosynthesis, productivity, production, leaves, gross primary productivity (GPP), graminoids, crops, soybeans, grasses, foliage, vegetation, net primary productivity (NPP), forbs, plant productivity, maize, wheat,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D07.ORNL.DP1.10023.001.variables.20211222T030947Z.csv,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
vegetation,plant productivity,forbs,clip harvest,soybeans,carbon cycle, foliage, productivity, C4 photosynthesis, leaves, corn, biomass, legumes, maize, sorghum, net primary productivity (NPP), production, barley, C3 photosynthesis, carbon (C), grasses, annual net primary productivity (ANPP), gross primary productivity (GPP), wheat,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D07.ORNL.DP1.10023.001.variables.20211222T031147Z.csv,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
C3 photosynthesis,grasses,wheat,annual net primary productivity (ANPP),graminoids,corn, crops, vegetation, production, gross primary productivity (GPP), barley, C4 photosynthesis, forbs, biomass, plant productivity, carbon (C), legumes, sorghum, net primary productivity (NPP), clip harvest, soybeans, leaves, maize, productivity,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D07.ORNL.DP1.10023.001.variables.20211221T215016Z.csv,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
carbon cycle,forbs,gross primary productivity (GPP),production,sorghum,carbon (C), grasses, crops, clip harvest, leaves, plant productivity, C4 photosynthesis, soybeans, corn, wheat, foliage, legumes, annual net primary productivity (ANPP), productivity, C3 photosynthesis, maize, net primary productivity (NPP), biomass, barley,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D07.ORNL.DP1.10023.001.variables.20211222T005200Z.csv,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220120T173946Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
NA,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
productivity,legumes,plant productivity,carbon (C),foliage,sorghum, biomass, crops, clip harvest, net primary productivity (NPP), production, annual net primary productivity (ANPP), wheat, C4 photosynthesis, carbon cycle, forbs, soybeans, grasses, maize, graminoids, barley, vegetation, corn, C3 photosynthesis,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
and units: NEON.D07.ORNL.DP1.10023.001.variables.20220627T191939Z.csv,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D07.ORNL.DP1.10023.001.readme.20220627T191939Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
NA,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
crops,clip harvest,carbon cycle,sorghum,carbon (C),plant productivity, soybeans, vegetation, productivity, grasses, corn, wheat, annual net primary productivity (ANPP), leaves, net primary productivity (NPP), foliage, maize, biomass, production, C3 photosynthesis, barley, graminoids, C4 photosynthesis, forbs,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.DELA.DP1.10023.001.variables.20211222T022928Z.csv,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
plant productivity,legumes,net primary productivity (NPP),gross primary productivity (GPP),clip harvest,biomass, carbon cycle, sorghum, annual net primary productivity (ANPP), foliage, soybeans, grasses, forbs, vegetation, leaves, carbon (C), maize, wheat, production, corn, graminoids, C3 photosynthesis, crops, barley,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.DELA.DP1.10023.001.variables.20211222T002930Z.csv,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
crops,foliage,C4 photosynthesis,grasses,productivity,barley, carbon (C), graminoids, clip harvest, legumes, plant productivity, production, wheat, carbon cycle, net primary productivity (NPP), C3 photosynthesis, corn, maize, sorghum, biomass, forbs, vegetation, annual net primary productivity (ANPP), gross primary productivity (GPP),NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.DELA.DP1.10023.001.variables.20211221T201148Z.csv,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
C4 photosynthesis,clip harvest,carbon (C),net primary productivity (NPP),plant productivity,productivity, foliage, legumes, corn, maize, annual net primary productivity (ANPP), grasses, production, sorghum, gross primary productivity (GPP), vegetation, biomass, C3 photosynthesis, wheat, barley, graminoids, leaves, soybeans, carbon cycle,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.DELA.DP1.10023.001.variables.20211221T214551Z.csv,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
leaves,grasses,productivity,net primary productivity (NPP),legumes,foliage, crops, production, plant productivity, soybeans, barley, gross primary productivity (GPP), biomass, maize, sorghum, vegetation, clip harvest, C4 photosynthesis, C3 photosynthesis, forbs, graminoids, carbon cycle, carbon (C), wheat,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.DELA.DP1.10023.001.variables.20211221T234925Z.csv,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220120T173946Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
NA,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
foliage,graminoids,plant productivity,grasses,legumes,carbon (C), net primary productivity (NPP), C4 photosynthesis, wheat, crops, C3 photosynthesis, vegetation, leaves, corn, production, annual net primary productivity (ANPP), sorghum, barley, gross primary productivity (GPP), clip harvest, productivity, carbon cycle, biomass, maize,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
and units: NEON.D08.DELA.DP1.10023.001.variables.20220627T191940Z.csv,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D08.DELA.DP1.10023.001.readme.20220627T191940Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
NA,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
C4 photosynthesis,forbs,net primary productivity (NPP),sorghum,vegetation,legumes, production, carbon cycle, soybeans, foliage, clip harvest, leaves, wheat, productivity, grasses, annual net primary productivity (ANPP), carbon (C), biomass, C3 photosynthesis, corn, barley, crops, maize, graminoids,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.LENO.DP1.10023.001.variables.20211221T232726Z.csv,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
corn,annual net primary productivity (ANPP),leaves,soybeans,grasses,biomass, wheat, carbon cycle, net primary productivity (NPP), foliage, gross primary productivity (GPP), maize, vegetation, crops, graminoids, barley, C3 photosynthesis, carbon (C), forbs, legumes, plant productivity, clip harvest, productivity, sorghum,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.LENO.DP1.10023.001.variables.20211221T212415Z.csv,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
clip harvest,carbon cycle,C4 photosynthesis,leaves,carbon (C),corn, production, barley, forbs, grasses, graminoids, wheat, gross primary productivity (GPP), biomass, maize, legumes, C3 photosynthesis, net primary productivity (NPP), soybeans, foliage, sorghum, crops, annual net primary productivity (ANPP), plant productivity,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.LENO.DP1.10023.001.variables.20211221T221951Z.csv,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
leaves,productivity,clip harvest,crops,gross primary productivity (GPP),barley, biomass, C4 photosynthesis, vegetation, corn, soybeans, forbs, C3 photosynthesis, wheat, carbon (C), plant productivity, grasses, production, annual net primary productivity (ANPP), net primary productivity (NPP), sorghum, graminoids, carbon cycle, foliage,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.LENO.DP1.10023.001.variables.20211222T034609Z.csv,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
C3 photosynthesis,grasses,productivity,graminoids,maize,forbs, clip harvest, barley, crops, legumes, gross primary productivity (GPP), carbon (C), net primary productivity (NPP), wheat, annual net primary productivity (ANPP), plant productivity, soybeans, foliage, corn, biomass, carbon cycle, leaves, sorghum, vegetation,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
and units: NEON.D08.LENO.DP1.10023.001.variables.20211222T024928Z.csv,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220120T173946Z.txt
1029808,1138160,1246537,1638695,1638696,1724433) and managed cooperatively by Battelle. These data are provided under the terms of the NEON data policy at https://www.neonscience.org/data-policy.,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
NA,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
sedges,forbs,some bryophytes,and non-woody vines such as Convolvulus spp. and certain Rubus spp.),as well as woody-stemmed plants with diameter at decimeter height (ddh) < 1 cm at the time of sampling. For additional details,see the user guide, protocols, and science design listed in the Documentation section in this data product's details webpage.,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
sampling in Tower plots occurs once every 4 or 8 weeks while livestock are present. Distributed plots are sampled once every 5 years.,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
clip harvest,carbon (C),production,biomass,net primary productivity (NPP),carbon cycle, gross primary productivity (GPP), sorghum, C3 photosynthesis, wheat, soybeans, barley, maize, foliage, forbs, leaves, legumes, annual net primary productivity (ANPP), graminoids, grasses, crops, C4 photosynthesis, corn, plant productivity,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
and units: NEON.D08.LENO.DP1.10023.001.variables.20220627T200521Z.csv,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
field protocols and data processing documentation,are available. Please visit https://data.neonscience.org/data-products/DP1.10023.001 for more information.,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
please visit this data product's detail page at https://data.neonscience.org/data-products/DP1.10023.001.,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
there will always be one record generated for each plot scheduled for sampling in the `hbp_perbout` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table,there will always be a corresponding record generated in the `hbp_massdata` table. For example,if field sampling was not possible **samplingImpractical** is populated with a value other than 'OK' (e.g.,'location flooded') in the `hbp_perbout` table,no sample is generated,and no record is generated in the `hbp_massdata` table. If **samplingImpractical** is set to 'OK' in the `hbp_perbout` table there will be a corresponding record in the `hbp_massdata` table, but **samplingImpractical** in the `hbp_massdata` table is populated with a value other than 'OK' if that sample could not be processed.,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
all biomass clipped was collected and weighed. In specific systems the process was time consuming and difficult.,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
sampling was reduced to 1 or 2 bouts per year; exclosures at these sites allow an assessment of relative grazing intensity but possibly not consumption.,NA,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
whether clipped material was sorted to functional group (`hbp_massdata.herbGroup`),and whether reweighing occurred for QA purposes (`hbp_massdata.qaDryMass`). Duplicates may exist where protocol and/or data entry aberrations have occurred; users should check data carefully for anomalies before joining tables.,NA,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt
and query reproducibility cannot be guaranteed. Once data are published as part of a Data Release,they are no longer provisional,and are associated with a stable DOI.,NA,NA,NA,NEON.D08.LENO.DP1.10023.001.readme.20220627T200521Z.txt

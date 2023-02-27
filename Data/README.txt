This readme.txt file was generated on 2022-01-18 by Laura Bibiana Ospina Rozo


GENERAL INFORMATION

1. Title of Dataset: Pretty Cool Beetles: Testing passive thermoregulation by beetle elytra

2. Author Information
	A. Principal Investigator Contact Information
		Name: Laura Ospina-Rozo
		Institution: School of Biosciences - University of Melbourne
		Address: School of Biosciences - University of Melbourne - Parkville Victoria 3010 – Australia
		Email: lospinarozo@student.unimelb.edu.au

	B. Co-investigator Contact Information
		Name: Jegadesan Subbiah
		Institution: School of Chemistry - University of Melbourne
		Email: jsubbiah@unimelb.edu.au 

	C. Co-investigator Contact Information
		Name: Ainsley Seago
		Institution: Carnegie museum of Natural History 
		Address: 
		Email: 


	D. Lab director Contact Information
		Name: Devi Stuart-Fox
		Institution: School of Biosciences - University of Melbourne 
		Address: School of Biosciences - University of Melbourne - Parkville Victoria 3010 – Australia
		ORCID: https://orcid.org/0000-0003-3362-1412 



3. Date of data collection (single date, range, approximate date): 
2019-05-01 to 2019-06-01 and 2020-11-01 to 2020-12-31

4. Geographic location of data collection: University of Melbourne. 

5. Information about funding sources that supported the collection of the data: 
This work was supported by funding from the Australian Research Council (DP190102203, FT180100216) and by the beetle division team of the Australian National Insect Collection


SHARING/ACCESS INFORMATION

1. Licenses/restrictions placed on the data: Can be re-used, should be cited

2. Links to other publicly accessible locations of the data: GitHub and FigShare



DATA & FILE OVERVIEW

1. File List: 

1_Reflectancedata.csv
2_Transmittancetopdata.csv
3_Transmittanceventraldata.csv
4_SolarSimulatorAndFilters.csv
5_TheoreticalIrradiance.csv
6_SingleElytronTempDataRaw.csv
7_SizeAndSide.csv
8_BeetleBodyTempDataRaw.csv
9_ExampleSetup.csv
10_BeetleBodyConsolidated.csv 
11_SingleElytraConsolidated.csv
12_SolarIrradianceALLWavelengths.csv


2. Relationship between files, if important:All these fileas are combined in a consolidated data frame in our code to explore the different questions we set in our manuscript. 

3. Additional related data collected that was not included in the current data package: NA

4. Are there multiple versions of the dataset? no

5. Relationship with the manuscript: All the analysis in our manuscript are based on this data set.


METHODOLOGICAL INFORMATION

1. Description of methods used for collection/generation of data: 

Files 1 to 3: Data was obtanied with a dual spectrometer to capture the reflectance, transmittance from the dorsal side of the elyra and transmittance from the ventral sid eof the elytra, from 400 to 1700 nm. 
File 4: Solar simulator data obtained from the manufacturer. Filter transimttance data was also measured with a spectrometer.
File 5: Theoretical irradiance from 400 to 1700nm. Data was found online. 
File 6: Temperature data was recorded with thermocouples in a controlled environment. Details of the set up are available in our paper. This file contains the raw data extracted from the thermometer for each sample of single elytra.
File 7: This contains mainly the side of the platform (inside the chamber) in which the sample was placed. Also, the size of each beetle corresponds to a mean value of its species. This was measured with ImageJ from calibrated pictures that included a scale bar.
File 8: Temperature data was recorded with thermocouples in a controlled environment. Details of the set up are available in our paper. This file contains the raw data extracted from the thermometer for the body of 11 recently dead beetles.
File 9: This data set contains the example of raw data obtain from the 4 thermocouples used in our set up. Two of them were used to monitor the temperature of the water bath and the chamber and ensure it remains constant. The other two were used to register the heating of the samples. 
File 10: Consolidated data after processing used to conduct the statistical analysis for the beetle body experiments. 
File 11: Consolidated data after processing used to conduct the statistical analysis for the single elytra experiments. Note: This set does not include data for the repeatability analysis. 
File 12: Standard Solar Irradiance from 280 to 4000 nm  from https://www.pveducation.org/pvcdrom/appendices/standard-solar-spectra. This file is required to calculate the contributions of different wavebands to the total radiative energy. 

2. Methods for processing the data: 
All the methods to process the data are in the section "Data Processing" of the full code. That file can be found in GitHub, Figshare and it can be access directly from a link in the manuscript sent for revision.

3. Instrument- or software-specific information needed to interpret the data: 
All data was analyzed in R 4.1.2 (R Core Team 2021). 
The spectral data was collected with the software OceanView 1.6.7.
The heating data was collected with the software provided along with the CENTER 521 Wireless Four Channel Datalogger Thermometer

4. Standards and calibration information, if appropriate: 
Heating experiments: The set up was costum made and designed for this experiment, so multiple preliminary experiments were done to calibrate it and test its repeatability. Results of this experiments are not shown here, but the full raw data contains a subset of repetitions which we used to perform a repeatability test on our data (see supplementary materials in our paper)
Measuring optical properties: Reflectance was measured against a perfectly diffuse white standard. 

5. Environmental/experimental conditions: Single elytra were obtained from museum samples. The beetles used in the beetle body experiment were collected in Orange NSW and tested after their natural death. All the experiments were done under controlled lab conditions

6. Describe any quality-assurance procedures performed on the data: We documented the experimental conditions in detail (File7) and for a subset of our sample we also collected repetitions of the same sample to evaluate repeatability. 



DATA-SPECIFIC INFORMATION FOR: 1_Reflectancedata

1. Number of variables: 57

2. Number of cases/rows: 1302

3. Variable List: 

First column is the wavelength, labeled "wl". 
Subsequent columns correspond to the  % of reflectance per wavelength of the ventral side of each of the 56 elytra we collected for the Single experiment elytra. 

4. Missing data codes: NA

5. Specialized formats or abbreviations: 

The first 4 characters of the column names are a code that correlates to the species (see the correspondent species name for these codes in the supplementary materials of our manuscript - Table 1)
The last character is a number that indicates the individual of that species since in multiple ocasions we tested 2 or more elytra of the same species.


DATA-SPECIFIC INFORMATION FOR: 2_Transmittancetopdata

1. Number of variables: 57

2. Number of cases/rows: 701

3. Variable List: 

First column is the wavelength, labeled "wl". 
Subsequent columns correspond to the  % of transmittance per wavelength of the dorsal side of each of the 56 elytra we collected for the Single experiment elytra. 

4. Missing data codes: NA

5. Specialized formats or abbreviations: 

The first 4 characters of the column names are a code that correlates to the species (see the correspondent species name for these codes in the supplementary materials of our manuscript - Table 1)
The last character is a number that indicates the individual of that species since in multiple ocasions we tested 2 or more elytra of the same species.


DATA-SPECIFIC INFORMATION FOR: 3_Transmittanceventraldata

First column is the wavelength in nm, labeled "wl". 
Subsequent columns correspond to the % of transmittance per wavelength of the ventral side of each of the 56 elytra we collected for the Single experiment elytra. 

4. Missing data codes: NA

5. Specialized formats or abbreviations: 

The first 4 characters of the column names are a code that correlates to the species (see the correspondent species name for these codes in the supplementary materials of our manuscript - Table 1)
The last character is a number that indicates the individual of that species since in multiple ocasions we tested 2 or more elytra of the same species.


DATA-SPECIFIC INFORMATION FOR: 4_SolarSimulatorAndFilters

1. Number of variables: 7

2. Number of cases/rows: 1301

3. Variable List: 

wl : wavelength (nm)
halfsun: irradiance of the solar simulator at half power (W /m2 / nm) 
visfilterTransmittance: % of transmittance per wavelength of the filter that allows the pass of visible light	
nirfilterTransmittance: % of transmittance per wavelength of the filter that allows the pass of near infrared light	
Full.f: same as halfsun	
vis.f: column halfsun *	column visfilterTransmittance / 100
nir.f: column halfsun *	column nirfilterTransmittance / 100

4. Missing data codes: NA

5. Specialized formats or abbreviations: NA


DATA-SPECIFIC INFORMATION FOR: 5_TheoreticalIrradiance

1. Number of variables: 2

2. Number of cases/rows: 658

3. Variable List: 

wl : wavelength (nm)
irradiance: theoretical solar irradiance (W /m2 / nm) 

4. Missing data codes: NA

5. Specialized formats or abbreviations: NA


DATA-SPECIFIC INFORMATION FOR: 6_SingleElytronTempDataRaw

1. Number of variables: 96

2. Number of cases/rows: 105

3. Variable List: 

light: indicates the interval of the experiment. 
Levels of the variable Light: 
"off" : the portal of the chamber was closed and the sample did not receive light. 
"on" : the portal was open and the sample received the full spectrum from the solar simulator (called TOTAL illumination in our manuscript). 
"nir" : the portal of the chamber was open but covered by the filter that allows the pass of near infrared light
"vis" : the portal of the chamber was open but covered by the filter that allows the pass of visible light

time: time point in which the temperature was collected by the data logger thermometer (s). Data was taken every 20 seconds.

columns 3 to 96: each of this column corresponds to the temperature (in degrees celsius) at a given time for each of the samples tested. 

4. Missing data codes: NA

5. Specialized formats or abbreviations: 

Labels for columns 3 to 96:
The first 4 characters of the column names are a code that correlates to the species (see the correspondent species name for these codes in the supplementary materials of our manuscript - Table 1)
The fifth character is a number that indicates the individual of that species since in multiple ocasions we tested 2 or more elytra of the same species.
The sixth character is a number that indicates the repetition, since the same elytra was tested multiple times for a subset of beetles in order to test the repeatability of our set up. 


DATA-SPECIFIC INFORMATION FOR: 7_SizeAndSide

1. Number of variables: 7

2. Number of cases/rows: 94

3. Variable List: 

ind: code for the sample following the same nomenclature descibed for the columns of File 6. 
size: mean length (cm) of beetles for the correspondent species measured from the front of the head to the end of the abdomen in calibrated pictures. 
spp: contains only the fist 4 characters of the column "ind" and it indicates the species of the beetle. The correspondent species name is registered in the supplementary material of our manuscript. 
Thermocouple: Since 2 thermocouples were used, they were alternated in the position of the side. We recorded this information in this column but did not include it in our models. 
side: The position of the sample on each side of the platform inside the chamber was registered in this column. This information was included in our models since it is more likely to have an effect if the illumination is not uniform across the platform. 
genus: Genus of each beetle

batch: This column helps to identify the subset of experiments used for models and the one used for repeatability.
Levels of the variable batch: 
"experiment": samples and repetitions that were included only in the models (results). 
"repeatability": samples and repetitions that were included only in the repeatability analysis (supplementary materials). 
"both": samples and repetitions that were used in both to calculate the results of our experiment and also in the repeatability analysis. 

The individuals that were used in the repeatability analysis were: aurs1 (repetition 1:7), oliv1 (repetition 1:7), prsi1 (repetition 1:9), rayn1 (repetition 1:7), rpmm1 (repetition 1:6), vrid2 (repetition 1:8) 

4. Missing data codes: NA

5. Specialized formats or abbreviations: NA


DATA-SPECIFIC INFORMATION FOR: 8_BeetleBodyTempDataRaw

1. Number of variables: 46

2. Number of cases/rows: 134

3. Variable List: 

light: indicates the interval of the experiment. 
Levels of the variable Light: 
"off" : the portal of the chamber was closed and the sample did not receive light. 
"on" : the portal was open and the sample received the full spectrum from the solar simulator (called TOTAL illumination in our manuscript). 
"nir" : the portal of the chamber was open but covered by the filter that allows the pass of near infrared light
"vis" : the portal of the chamber was open but covered by the filter that allows the pass of visible light

time: time point in which the temperature was collected by the data logger thermometer (s). Data was taken every 20 seconds.

columns 3 to 46: each of this column corresponds to the temperature (in degrees celsius) at a given time for each of the samples tested. 

4. Missing data codes: NA

5. Specialized formats or abbreviations: 

Labels for columns 3 to 46:
The first 3 characters of the column names are a common prefix for all samples
The fourth and fith characters are a number indicating the individual ID for a given beetle. 
The sixth character is "i" when the thermocouple was placed inside the body and "e" when it was placed under the elytra.
The seventh character is "c" when the elytra of the beetle were closed and "o" when the elytra were open. 


DATA-SPECIFIC INFORMATION FOR: 9_ExampleSetup

1. Number of variables: 5

2. Number of cases/rows: 105

3. Variable List: 

time: time point in which the temperature was collected by the data logger thermometer (s). Data was taken every 20 seconds.
T1: Thermocouple registering the temperature of Sample 1
T2: Thermocouple registering the temperature of Sample 2
tch: Thermocouple registering the temperature of the inside of the dark chamber
twb: Thermocouple registering the temperature of the water bath 

all themperature data is reported in degrees celsius

4. Missing data codes: NA

5. Specialized formats or abbreviations: NA


DATA-SPECIFIC INFORMATION FOR: 10_BeetleBodyConsolidated.csv 

1. Number of variables: 7

2. Number of cases/rows: 11

3. Variable List: 

Beetle : beetle ID

columns 2 to 7 were calculated as the Difference in heating [final change in temperature after 5 minutes (degrees celsius)] of each beetle with the elytra closed (i.e. folded on top of the body) - open (i.e. not covering the body). 
Thus, negative values of this difference indicate an excess of heating when the elytra are not covering the body.  

PairDifTOTe : Difference in heating under TOTAL illumination (degrees celsius). Thermocouple placed under the elytra.
PairDifNIRe : Difference in heating under NIR (near infrared) illumination (degrees celsius). Thermocouple placed under the elytra.		
PairDifVISe : Difference in heating under VIS (visible) illumination (degrees celsius). Thermocouple placed under the elytra.		
PairDifTOTi : Difference in heating under TOTAL illumination (degrees celsius). Thermocouple placed inside the body.
PairDifNIRi : Difference in heating under NIR illumination (degrees celsius). Thermocouple placed inside the body.
PairDifVISi : Difference in heating under VIS illumination (degrees celsius). Thermocouple placed inside the body.


4. Missing data codes: NA

5. Specialized formats or abbreviations: 


DATA-SPECIFIC INFORMATION FOR: 11_SingleElytraConsolidated.csv

1. Number of variables: 22

2. Number of cases/rows: 56

3. Variable List: 

Beetle: Code ID for each individual in the single elytra experiment. This is the same code used in files 1, 2, 3 and 6. (repetitions not included since this data set is not the one used for repeatability)
Rf_TOT: Reflectivity in TOTAL illumination (%) 
Rf_NIR: Reflectivity in NIR (near infrared) illumination (%)
Rf_VIS: Reflectivity in VIS (visible) illumination (%)
Td_TOT: Dorsal transmissivity in TOTAL illumination (%)
Td_NIR: Dorsal transmissivity in NIR illumination (%)
Td_VIS: Dorsal transmissivity in VIS illumination (%)
Tv_TOT: Ventral transmissivity in TOTAL illumination (%)
Tv_NIR: Ventral transmissivity in NIR illumination (%)
Tv_VIS: Ventral transmissivity in VIS illumination (%)
Ab_TOT: Absorptivity in TOTAL illumination (%) (calculated as 100 - (Reflectivity in TOTAL + Dorsal transmissivity in TOTAL) )
Ab_NIR: Absorptivity in NIR illumination (%) (calculated as 100 - (Reflectivity in NIR + Dorsal transmissivity in NIR) )
Ab_VIS: Absorptivity in VIS illumination (%) (calculated as 100 - (Reflectivity in VIS + Dorsal transmissivity in VIS) )
side: Side of the platform
size: length of the beetle for the correspondent species (cm)
DT5_TOT: Final change in temperature after 5 minutes (correlated with final steady state) (degrees celsius) under TOTAL illumination
DT5_NIR: Final change in temperature after 5 minutes (correlated with final steady state) (degrees celsius) under NIR illumination
DT5_VIS: Final change in temperature after 5 minutes (correlated with final steady state) (degrees celsius) under VIS illumination
maxHRTOT: maximum heating rate (delta between two adjacent points) (degrees celsius/s) under TOTAL illumination
maxHRNIR: maximum heating rate (delta between two adjacent points) (degrees celsius/s) under NIR illumination
maxHRVIS: maximum heating rate (delta between two adjacent points) (degrees celsius/s) under VIS illumination

4. Missing data codes: NA

5. Specialized formats or abbreviations: NA


DATA-SPECIFIC INFORMATION FOR: 12_SolarIrradianceALLWavelengths

1. Number of variables: 2

2. Number of cases/rows: 1883

3. Variable List: 

wl : wavelength (nm)
gobalIrrad: theoretical solar irradiance (W /m2 / nm) from 280 to 4000nm

4. Missing data codes: NA

5. Specialized formats or abbreviations: NA
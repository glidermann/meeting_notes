# How to expand the GROOM RI data management capacity to the “new” data type collected by Gliders in Europe?


# Date: July 7 2022, 14:00 - 16:00 CEST

Session chair: Alvaro Lorenzo-Lopez (NOC, UK)

# Participants
Alvaro Lorenzo-Lopez (NOC, UK),Victor Turpin (OceanOPS), Pierre Testor (LOCEAN/CNRS),Laurent Mortier(ENSTAParistech), Yves Ponçon (LOCEAN), Marc Picheral (LOV), Ehsan Abdi (CSCS), Dan Hayes (CSCS), Emma Slater (NOC-BODC),Maryam Hassani (UT), Ailin Brakstad (UiB), Alexia Cociancich (OGS), Joana Beja (EMODnet Biology/VLIZ), Patricia Cabrera (VLIZ), Rory meyers (VLIZ)

# Agenda
1) Welcoming, meeting objectives and introduction – Victor Turpin - 10 min
2) The new capacities of gliders – 45 min
    + The BioGlider project - Yves Ponçon (LOCEAN) - 10 min
    + EK80 - Laurent Mortier (LOCEAN) - 5 min
    + UVP6 - Marc Picheral (LOV) - 15 min 
    + pCO2 - Dan Hayes (CSCS) - 10 min 
    + Passive acoustic Monitoring - Dan Hayes (CSCS) - 10 min

3) The future data infrastructure - Discussion (1h) – Alvaro Lorenzo-Lopez

Access the live [Paddlet](https://padlet.com/alvarolorenzonoc/as89sbmo9y3iyfld)
+ Interoperability in the future?
+ The data infrastructure for new types of data?
    + What should be the role of GROOM RI regarding these new data types?
    + How do we shape the infrastructure to properly manage those datasets?
        + How to manage high volume data - https://catalogue.ceda.ac.uk/uuid/096690aba290452d9b7208133274b69b
    + How does GROOM engage with EU data infrastructure ?
    + Is the concept of DAC or GDAC appropriate for the new datasets?
        + GDAC by data type?
+ Real time data transmission Vs Real time data management?
    + What are the users of new datasets in real time?
    + Is an infrastructure approach needed and useful?
    + Integration by manufacturers
+ Managing new datasets in delayed mode / recovery mode.
    + Sounds, images, videos:
        + Formats
        + Storage
        + Computing power
+ Do those data type need QC ? How to QC those data ? 

# Meeting notes

## [Introduction](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/20220707_WS2-2_Introduction_Victor_Turpin.pdf)
Current data management infrastructure is addapted to the current observing capacities of gliders in the purpose of serving both operational community and scientist.

But the increase of observing capacity, complexify the management of gliders data with new type and new format higer volume of data. It is likely that the current glider data management infrastructure not addapted to these new observation. 

How can we anticipate that ? How can we benefit from the existing EU data infrastructure to continue serving same users and new ones.

## [BioGlider](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/20220707_WS2-2_BIOGLIDER-Poncon.pdf)
2 year project - 1.2M€
Exemple of what GROOM RI could do in terms of innovation and technical dev. Partners are part of GROOM RI too.
Follow up of BRIDGES. 
Sensors development. Minuatirization. Smart cables.
Idea of BioGlider coming from ZooGliders (includes a Zoocam and Sonar as well as "traditional" sensors).
+ Develop commercialy available payload UVP6, EK80,
+ Integrate multi platform (SG, SE, SL)
+ Scientific validation of the system
+ Capacity to retreive data from moorings.
+ Application : Oil and Gaz, Fisheries sectors.

UVP6 on slocum (end of year), SeaExplorer, SeaGliders (2021-2022)
EK80 (SeaGlider, may 2022), Slocum and SeaExplorer (coming)
+ half of the profiles 'only'
+ Software adaptation

Integration of both sensors on a SeaGlider is already a success.

Note that surface vehicule can complete those multiplatform, multisensor mission, making the data management even more complexe.

Scientific validation is also an important part of the project. Question of the complementatity of the two sensors, frequency, frame rate...

Last aspect of the project is about retreiving data form moorings with accoustic communication.
From data management, mooring data comming from a gliders may be challenging. How to build the interoperability ?
Collection from mooring and data transmission from glider, this exercice is being designed and will be tested in the coming years.

## [EK80](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/20220707_WS2-2_BIOGLIDER_EK80_Ladroit.pdf)
Laurent Mortier is presenting on behlaf of Yoann Ladroit.
EK80 is popular on vessels, but not on autonomous vehicles.
Surface vehicule and gliders are at the front of this question.

EK80 is: 
+ EchoSounder miniaturised (SIMRAD/KONGBERG)
+ Multiple frequency. Broader frequency, multple wavelength.
+ Data Acquisition: Depend of the housing. 
+ Data format: raw data are binary data, depending on the channels, configurations, metadata and external data (position).
+ Capacity to format those data in netcdf (plan)
+ For a 45 day cruise, 2 terabytes (.raw data) are created and can be stored on the vessels
+ RT data management already in place for sail drones.

Already lot of experiments of the minutirezed EK80.

## [UVP6](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/20220707_WS2-2_uvp6_groom_data_management.pdf)

Underwater Vision Profiler = particule counter above 100µm
Imaging device for plankton and particules >650µm.
Camera make images and compute the images.
+ Low power sensor.
+ Light
+ Versatil

Capable to do the classification of particule up to 25 classes today. Use for ecology and carbon pump studies

RT data transmision is operational, used by Argo-BGC. 
+ Limited in scope compared to the capacity of UVP6
+ Frame (i.e. format) exists for data and metadata. It covers aboundance, identification of the plakton

Recovery Data collection display and access is operational too.
+ Portal to access the data exist. EcoPart 
+ Recovery data = 400GB or 1TB.


Integration 
+ on SeaExplorer is operational and RT data visualisation also through GLIMPSE
+ On SeaGlider, integration is operational. Only few data are transmitted. But improvement is on progress. No visualisation yet. 
+ Slocum, first test by th end of 2022.

The case of float is interesting regarding the RT data. The data chain is being developed by Coriolis.

Real Time is usefull for: 
+ Instrument control, 
+ Aboundance in RT (droplet, eggs, copepod, bubble) would permit to re-orient the mission live thanks.
+ Cruise support
+ Green Ocean Modeling

To improve data flow RT:
+ includ the taxonomie indetification
+ Improve ... - look in the presentation.
+ Broke data from ECO part

## [PCO2, CH4 and PAM](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/20220707_WS2-2_CyprusSubsea_EUDataManag_EUMR-PAM.pdf)
CSCS is involved in GROOM II, TEchOceanS, EU Marine Project, BRIDGES, NSF project (US), Cyprus project.

### Passive Accoustic Monitoring with Gliders has pros and cons
+ Pro : Quieter than other platforms, far from the surface noise/echos, long endurance, low intrusive, deep, combined with other data
+ cons : undifined source of the sounds, low data in real time, slow moving, low precision of navigation/localization

Exemple of experiment (TNA, NOC, SeaGliders): Hydrophone integration of the SeaGliders. 
+ [deployement track](https://mars.noc.ac.uk/missions/eumr-blt/vehicles/eltanin)
+ [glider core data](https://linkedsystems.uk/erddap/files/Public_Glider_Data_0711/Eltanin_20210622/)
+ [acoustics data](http://dx.doi.org/10.5285/096690aba290452d9b7208133274b69b)
+ [real time files available here including those text files mentioned](https://linkedsystems.uk/erddap/files/Public_Compressed_RAW_Glider_Data_1112/)

Files are in raw formed saved internally. Processing can be done onboard. In the future, smaller version can be develop without processing onboard but with low power capacity.
Softwares have been developed (gListen board) to transmit accoustic spectra.
Files are now on the Glider CPU to be send RT on the shore
SMART cable can support the RT flow for "instrument control","Detecting event","Time Series of spectra". Limited in volume but usefull for piloting.

Recovery data (waveform): Traditional way to store gliders data was not addapted to this type of data.

### PCO2 

Carbon data acquisition on a glider still being tested and valided


# Discussion

## Generic questions
Victor Turpin : Data in RT are usefull for the instrument control and piloting. But is it usefull for sharing RT data largely.

Laurent Mortier: the rational for data transmitted in RT today is still unclear, why not those data?
Pierre Tesot: The rational exist, it is just that we are not at the level of using it very well. for PCO2 for exemple will certainly be usefull. 

Victor Turpin: Also, UVP6 pushed data in real time from Argo floats, the rational is that it is usefull for the BGC community.

Pierre Testor: UVP6 data in depth beem ? Why Depth and not time ? 
It is depending on the speed of the instrument.

## [discussion outcome (padlet)](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/20220707_WS2-2_PadletOutcome.pdf)


**Is the concept of DAC or GDAC appropriate for the new datasets**

Pierre Testor: Keeping all the data from an platform is a priority. Fragmentation of the data set is a risk. Centralizing the data is very important, but links could be enough.

Joana Beja: Pierre stop at the gliders users. The rest of the community is not interested in the glider but the data. GDAC may not be easy to access the datasets.

Pierre Testor: depending of the variable, data management is different, also regarding user needs.
Operational Oceanography are not the targeted user. So the service should be re-thinked.

Dick Shaap: GDAC is needed for the operational network need their own service. Both are needed, GDAC and EU intergrators.

Laurent Mortier : Data service is difficult. providing a robust service is crucial. This goes in favor of the service provided GDAC. Limited resources.

Pierre Testor: We already have difficulties to manage the std variables. How can we do that for new data sets ?

Joana Beja: dick comment apply to physical ocean data (RT validation), biology need expert data to validate it. So GDAC approach is probably not aplicable to the biology.

**What should be the role of GROOM RI regarding these new data types Find the best place for Long term archiving**

Offer single access does not mean single place to store the data. single access to get gliders data distributed.

**What should be the role of GROOM RI in the European Data Infrastructure Landscape**

GROOM RI could work as a high level management/operation.

Participate in interoperability exercises with other RIs : Help the fragmented infrastructures to make the digital services better. Interoperability is key. 

**Near Real Time Data. Can we do more with a dedicated infrastructure?**

+ Depends on the type of data, this is not straightforward for Biological data (e.g. taxa identification from images that require validation from experts)

EMODNET Biology is ready to ingest NRT data. The question is what is more interesting for user to use validated data or non validated data. Metadata and validation is necessary to make the data usefull.

EcoTaxa allow people to validate the data. How many specialist are looking at those data. For species it is very complex, for functional group it is already validated.

EMODNET Biology is getting ready to ingest the NRT data for UVP6.

*"Need to re-listen the meeting from 15h50 to 15h55"*

**Managing New datasets in delayed/recovery mode. What are the challenges?**
+ linking the data together
Specific repository for different data type is needed, but we need to connect those repository together.

+ Lack of Image repositories and Imagery metadata catalogues linked. 
Linking data and metadata is necessary for any type of data.
Same think for accoustics.

+ EK80 data processed into identifying groups and individuals. But **raw data** don't know?













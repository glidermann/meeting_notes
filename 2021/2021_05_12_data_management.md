Welcome to the “Data processing and management” room.

Co-leads: Victor Turpin, Justin Buck

## Agenda
May 12 Wednesday 
	16:00 - 17:30 CEST / 7:00 - 8:30 PDT / 22:00 - 23:30 AWST
Data Management: Assign people to paragraphs (V. Turpin, J. Buck)

## Participants: 
Victor Turpin, Justin Buck, Soeren Thomsen, Thierry Carval, Catherine Schmechtig, Gui Castelao, Charitha Pattiaratchi, Mun Woo, Chenyi Luo, Yunchang Kwak, Yumi Song, Kate Patterson, Adam Comeau, Sue L’Orsa, Anh Tran, Miguel Charcos

------------------------------
Agenda 	 	 	
45 min:
Presentation of the different potential topics / issues we want to tackle together (based on first survey)
Define the outcome of these 2 weeks exercises.
45 min:
	Draft outline of the document(s)
	Assign people to paraph.
-------------------------------
Second session partipant, fill up this section please : 
Glider groups already involved in the data management process :

Glider groups not involved in the data management process :
-------------------------------
DAC documents general review:
Different approaches, different flows, different services.
Harmonizing the procedure will have to much impact on the user. We need to document the different approached and make sure each approach reach the final common target (OG1.0, OceanOPS, GDAC, GTS)
-------------------------------
Note of the 2de meeting : 
Metadata about what is at sea? Can manufacturers provide the metadata of what is at sea (glider S/N, sensors) in the data files?
Catalogue of the metadata associated with the data that can be populated with time. In order to operate with a minimum set of metadata. Central point where everyone can feed the metadata and export to produce netcdf.
Difficulty in having everyone feeding the same system.
Difficulty in updating the data set without reprocessing the full data set.
→ Versioning. Needs to become a BP. Get Guilherme's advice.
-------------------------------
What document is needed / missing?

During the first session of the workshop the need for accessible information to implement the OceanGliders data and metadata flow has been highlighted. Indeed, new glider groups or PI willing to contribute to OceanGliders are facing difficulties to achieve the first steps of the data management process.
Another discussion around metadata requirements to make good use of non direct measurements (e.g. oxygen, chl-a, backscatter) in real time shows the need for clearer information in this regard. 
More experienced users, including Data Assembly Center representatives, pointed out the need for documentation related to the use of vocabulary services for OceanGliders.
Finally servicing data to end users should also be described properly for the OceanGliders community.




The simple scheme below shows each step of the data and metadata flow.


The green circle indicates the scope of the document we aim to produce during and after this workshop.

This document should be addressed to any glider group willing to join the OceanGliders program or improve its current contribution to the program.
This document should better define and explain the requirements in terms of data and metadata for PIs and operators.
This document should specify the relationship between DACs, OceanOPS and Pis/Operators. → Diagram needed. 
This document should recognize the different approaches developed by Data Assembly Centers and describe the data and metadata flows for each. 
This document should explain the benefits of sharing data and metadata in order to encourage operators and PIs to share it. 



Suggested title : “How to submit data and metadata to OceanGliders and why ?”

The document will describe the different stages to integrate OceanGliders from a data management point of view. It will address this question for any gliders groups. 
To avoid a too long document that can be discouraging for “beginners”, this document will summarize the different stages and point to detailed documentation produced by the Data Assembly Center (DACs).
Those detailed documents will be living documents that will evolve in time as OceanGliders data management is progressing.
The document will address “newcomers” needs by delivering key guidelines to join OceanGliders. It will also encourage more experienced users to improve the efficiency of their contribution to the OceanGliders program by delivering high level requirements to make the most of the data that can be delivered by glider in real time.
The data management section of the BP document should be addressed aside of this document. 

Overlaps with RTQC and pre-deployment operation has been highlighted and should be addressed in collaboration with those groups.



Suggested outline
Draft version 1.0Connexion
May 2021

Introduction ( DanH help write and/or review, Jay review, Miguel Reviewer)
Why
By being acknowledge as a GOOS OCG network, OceanGliders has the mandate to build a data management system that implement the FAIR principles (Findable, Accessible, Interoperable, Reusable) (ref.)
Consequently, data sets produced by OceanGliders must be publicly available and data management procedure should be harmonized within the network. Also, cross-network standardization is strongly encouraged to increase the value of GOOS data in general.
 
Since the creation of OceanGliders, in 2016, the need for harmonization across the different data standards has been very well identify. Although the three existing data formats, IOOS(ref.), IMOS(ref.) and EGO (ref.) seems very similar, the discrepancies between them leads to a strong under use of the gliders data globally. By harmonizing and standardising data management approaches, the use of OceanGliders data will be facilitated for a larger community of users.
There are many benefits from having unique data management procedures and format within OceanGliders:
Easier integration by new glider groups in the OceanGliders networks.
Tools for piloting, data analysis, data management, etc. that could be shared, co-develop, and used by different glider groups.
Monitoring of the network will be facilitated and upgraded.
Expend the usage of gliders data by the modelling and data assimilation communities
Allow large scale analysis (e.g. Boundary current, water transformation, Oxygen minimum zone, ocean heat wave)
Facilitate cross-network data analysis
The overarching goal of having a harmonized data management procedure is to strengthen the network and empower the use of the data produced by the OceanGliders community for climate studies, ocean health monitoring and operational services like forecast and warnings.
Who uses the data
There are different types of OceanGliders data users they can be regrouped into 3 families.
Data manager and data aggregators need gliders data to complete their catalogue and provide these data to any ocean data users. They also build data product that aggregate ocean data from many different sources.
The scientist and the PIs. They use the data to do science, to understand the ocean processes, climate changes, understand air-sea interactions during storms, monitor ocean heath and ecosystem, measure water transformations and study boundary currents. Pis and scientist are interested in high quality data sets to achieve their studies.
The data assimilation and modelling community use the data to feed the models. They produce ocean forecast and ocean reanalysis for climate studies and operational services. This community of users are also very interested in accessing the gliders data in real time.

GOOS role
Led by the Intergovernmental Oceanographic Commission (IOC) of UNESCO, the Global Ocean Observing System supports a community of international, regional, and national ocean observing programmes, governments, UN agencies, research organizations and individual scientists in the building of a fully integrated global observing system that captures essential physical, chemical, biological, and ecological ocean properties.
OceanGliders is one of the nine international ocean observing programs of the GOOS with Argo, OceanSites, DBCP, GOSHIP, SOT, GLOOS, AniBOS and the Global High Frequency Radar Network. GOOS is providing continuous requirement to implement a more unified, efficient, and transparent ocean observing system
Contributing to OceanGliders
The OceanGliders program has been created almost a decade after the popularization of the use of the gliders for scientific ocean observations. Despite great progresses, the development of OceanGliders has been limited by the lack of common rules on format and data procedures. The aim of this document is to guide any user willing to engage with OceanGliders data management.
To facilitate data contribution to OceanGliders, we have identified 4 stages of engagement that we will describe in detail later in the document. Here is a short definition of those stages.
·         Stage 1: Monitoring the activity
OceanGliders and OceanOPS are monitoring the global glider activity upstream data availability in global data centres. By doing so, the development of the program can be accurately assessed and the gaps in the data flow can be identified.
Monitoring is possible by providing deployment metadata to OceanOPS.
·         Stage 2: Sharing the gliders data
This second stage of engagement aims at building a global OceanGliders data set under a unique format and harmonized vocabularies. At this stage, there are no requirements in terms of data delivery timeliness.
OceanGliders data sets are centralised  into a Global Data Assembly Centre (GDAC).
·         Stage 3: Sharing gliders data in real time
Sharing gliders data in real time under a common format contributes to the improvement of the operational services promoted by the GOOS and regional institutes. It also allows the monitoring of the OceanGliders activity in real time.
Real time data aims to be distributed on GTS and GDAC.
·         Stage 4: Sharing delayed mode quality-controlled data
After being qualified by PIs data sets are pushed to the GDAC and published by scientific data publication centre. GDAC aims to archive the best possible data sets.
What (and how?)
Stage 1: Monitoring the activity
Monitoring the OceanGliders network is the role of OceanOPS. For integration reasons, in the OceanOPS (www.ocean-ops.org) system, a glider mission is called a “platform” and each “platform” must be linked to a “program”.
All that can be deployed or installed, equipped with sensors (an observing entity) is considered as a “Platform” at OceanOPS (float, drifting buoys, weather station on ships, XBT, Mooring deployment, tide gauge, glider mission…).
A “program” defines a group of platforms or cruises managed by the same operator. It materializes the implementing, operating, and responsible team. A program is bound to one country, to one or several agencies, to a set of contact points. It is usually a national/agency-implementation of the observing system. In the case of multiple agencies involved, one should be identified as lead.
The following document describes shortly the metadata OceanOPS requires to register a glider mission.
short document to the metadata needs for OceanGliders.
More detailed documents describing the architecture of the OceanOPS systems are available here: documentation to the metadata scheme and API documentation

Stage 2: Sharing the gliders data
The common format OG1.0 (OceanGliders V1.0) describes what is requested in terms of

Stage 3:
Stage 4:
Who
Stages?
Current practices in the community (the short summaries by DAC)
BODC 
AODN / IMOS
Data providers willing to get their data hosted in AODN can contact us via email at info@aodn.org.au. The Australian Ocean Data Network provides storage for both static and ongoing datasets. Conversation around whether the dataset will be delivered through the AODN portal (a data collection, ongoing) or AWS S3 / THREDDS server (static dataset) will be held as a preamble of the submission process. 
 
The process described below the case of a user who wants to archive data and have a metadata record describing it.  Further information is available from the AODN portal website https://help.aodn.org.au/contributing-data/.
Process for ongoing data collection requires further discussion in relation to the ongoing
submission of data files, and data publication to the AODN portal.
 
Metadata Officer
To assist metadata creation in these situations, the AODN directs users to utilise our AODN Data Submission tool - https://metadataentry.aodn.org.au/submit/. The tool provides a user-friendly interface to guide users in the creation of both metadata to describe their data, and where applicable, data submission in the one process. Help documentation is provided to users in the use of the tool, and if further assistance is required, the AODN metadata officer is the point of contact. The AODN Data Submission tool requires that users create a log in, and after a user has successfully submitted their metadata and data for upload, this process is not automated but the submission will be checked over by the metadata officer and a relevant data officer (dependent on the data type and source). Information to create a metadata record consist in an abstract, keywords, details for principal investigator(s), organisations details, geographic extent, temporal extent, instruments, parameters, methods, and if links to related documents.
Both the metadata and data will not be uploaded to the relevant metadata catalogue (IMOS or AODN), until after both have been qualitatively and quantitatively checked. A link will be provided from the metadata record to the location of the data.
Data Officer
The data that is submitted to the AODN under these circumstances can cover a broad range of scientific disciplines. Where possible, the data officer assigned to check the data will be within their recognised area of expertise. Outside this, data officers are unable to comment on the quality of the scientific work undertaken. The data officer will work with the user to upload the data in the most appropriate format, NetCDF being the preferred format. Where possible, files may be saved in different formats to increase their likelihood of long-term preservation. Whenever this is done, copies of the original file are also kept.
Information on the contents of NetCDF files currently being uploaded by IMOS Ocean Gliders to AODN is found in the following document: http://content.aodn.org.au/Documents/IMOS/Facilities/Ocean_glider/Delayed_Mode_QAQC_Best_Practice_Manual_OceanGliders_LATEST.pdf
DFO
Glider fleets
Department of Fisheries and Oceans Canada (DFO) have seven Sea Explorer gliders from Alseamar and one Slocum glider in partner with the University of Victoria.   The gliders are managed at Bedford Institute of Oceanography in Dartmouth, Nova Scotia, and the Institute of Ocean Sciences in Sidney, British Columbia. And, the Marine Environmental Data Section (MEDS) in Ottawa, Ontario, manages glider data.
Data Flow
Before launching a glider, it should have a WMO number.  Once the glider is deployed,  the deployment operator will send the metadata related to the mission:  ship name, glider name, mission number, deployment date and location,  principal investigator, deployment operator, sensors information to MEDS.  MEDS will record the metadata into the system for data processing.  MEDS will also declare the information at https://www.ocean-ops.org/board?t=oceangliders.  Besides sending metadata to MEDS, the deployment operator also makes raw glider data available via FTP site or HTTP so that the system can automatically access the raw data. MEDS used SOCIB software as the primary data processing to generate L0, L1 and L2 NetCDF files.  Then, the L1 NetCDF file is converted to EGO NetCDF format using an in-house Java program that maps SOCIB variables to equivalent EGO variables.  The EGO NetCDF file is split into mono NetCDF files.  The mono NetCDF files are transformed into TESAC format for Global Telecommunication System (GTS) dissemination.  The EGO and mono profile NetCDF files are made available automatically to the MEDS FTP site, ftp://ftp.isdm.gc.ca/pub/glider/, and manually to ftp://ftp.ifremer.fr/ifremer/glider/v2/  
IOOS
Data providers wishing to submit real-time and/or delayed mode data sets to the United States Integrated Ocean Observing System (IOOS) glider data assembly center (DAC) must first register and receive a user account.  Registration is typically done by emailing the IOOS DAC support group at glider.dac.support@noaa.gov and provide the
following information:
Full name
Email address
Phone Number
Institution
The user receives a user account and temporary password that should be changed immediately upon logging in for the first time.
Once registered, the user may submit real-time and/or delayed mode datasets using the following process:
For data sets that are to be released to the Global Telecommunication System (GTS, real-time data sets only), the data provider should request a WMO id from the DAC support team (glider.dac.support@noaa.gov).  WMO ids are unique to a single glider deployed in one of the WMO regions and should only be used for deployment of the same glider in the region for which it is assigned.
Native telemetered glider data files are parsed to retrieve individual profiles from the time-series data set. The indexed profiles are then written to the NetCDF format according to the specification provided at https://ioos.github.io/ioosngdac/ngdac-netcdf-file-format-version-2.html which attempts to conform to CF, ACDD and IOOS Metadata Profile standards. The NetCDF format detailed here stores a single profile time-series that can include any number of time indexed variables with the exception of the following variables:
a.  Calculated water currents and their associated GPS coordinates, all of which are stored as scalar variables containing a single u, v, latitude and longitude according to CF specifications.
b. A trajectory variable, containing a string or character array, specifying the unique name of the dataset which can also be interpreted as the deployment name.  This string has the following format: glider-YYYYmmddTHHMM (glider name and ISO-8601 formatted deployment start date and time).
c. Descriptions of the instruments contained in the glider payload are stored as empty scalar variables who attributes convey information about the instrument including instrument type, calibration date(s) and serial number.
The deployment name (1b) is registered on the IOOS Glider DAC deployment registration page located at https://gliders.ioos.us/providers/. The following information is required during registration:
Glider name
ISO-8601 formatted date/timestamp
Attribution of the funding agencies.

Following deployment registration, the data provider uploads one or more profile-based NetCDF files (described in 2) via ftp to the DAC data submission server.  These individual files are then aggregated into a TrajectoryProfile dataset via NOAA Environmental Research Division’s Data Access Program (ERDDAP), located at https://gliders.ioos.us/erddap/info and real-time data set status is monitored at https://marine.rutgers.edu/cool/data/gliders/dac/status.
The National Data Buoy Center harvests new data from all data sets for which a valid WMO id has been supplied, encodes the data to the profiling float BUFR format and releases the messages to GTS.
It is anticipated that the U.S. IOOS Glider Data Assembly will undertake the conversion of existing a future submitted data sets to the OceanGliders 1.0 NetCDF format, once it is adopted (2021 or 2022).  While we do not anticipate a change to our existing data format to accomplish this, it is very likely that we will ask data providers to submit additional metadata to be included in the OceanGliders data sets.  We are currently reviewing and comparing the OceanGliders format to our existing format in order to identify and missing metadata.
SOCIB
This document describes the flow of glider data in SOCIB. It first sketches the different data types and provides an overview of the data flow of each of these types. Then, it lists and explains the various types of outputs created along the process. For the netcdf outputs, a brief description is provided of the three processing levels and their dissemination mechanisms. The role of the metadata catalog is then discussed highlighting its importance along the process. Finally, we provide an overview of the vision and possible future improvements inside SOCIB and the international landscape.
The data management processes have been defined in the framework of SOCIB operations and fine tuned along the years. These results will support the elaboration of the data management best practices of glider data in the context of the task 6.2 of WP6 of JERICO-S3.
 
Glider Data Flows
SOCIB glider data workflow involves personnel of the glider facility, data managers and scientists along the glider data lifecycle. Figure 1 (see source for more details) explains the role of the various actors along the different steps of the operation and the data flow. It also describes the processes along the three major flows for real time (RT), recovery data and delayed mode (DM) and scientific corrections. Figure 1 also illustrates the main outputs for the community: 
Reports about the operations are created by the glider facility
Glider data is disseminated through the main European data providers in addition to the SOCIB dissemination mechanisms
Data outputs are of various types as we will describe in the following section. Most of the data management processes are performed automatically. The metadata catalog plays a critical role in the automatic processes and supporting hand-operation. RT data is fully automated.
Recovery data follows a similar flow than the real time cycle on mission conclusion. In this case, the data is collected by the glider operators and uploaded to an ftp server manually. Delay mode data flow involves higher human intervention in the loop to tackle data intercomparison and occurs once the recovered data outputs are available.
Quality control (QC) in SOCIB is defined using the results obtained from our historical data (10 years). The application of this QC is currently performed manually to support and optimize the glider operations. Automatic QC in RT and recovery is not operational yet.
Data Outputs
We create three types of data outputs: data files (netcdf), plots (png) and trajectories (kmz). RT data is collected automatically from the dockerserver to create the glider trajectory and visualize science parameters in the dapp application. Simultaneously, the SOCIB Glider Toolbox produces netcdf files and plots of real time and recovery data. The SOCIB glider toolbox is been used by leading institutions to process their glider data such as NOAA fisheries (Reiss et al 2021) and DFO-MPO (mission report).
Plots are used to support the operation and to facilitate the visualization of key measured variables in RT. Glider operators and principal investigators (PI) use the netcdf files to assess the RT and recovery data. In addition, an automatic tool monitors the engineering data from the glider and detects potential failures of the glider during the mission. This tool creates png figures and provides email alerts to glider operators when issues in the engineering or science data are detected. The SOCIB salinity correction toolbox is used to perform delay mode data. The calibration of glider data is performed using the vessel data from missions in the same transects as the glider close to the same missions dates. The delay mode uses white maximization image analysis (see Allen et al 2020) to calibrate the salinity against vessel data. The output of the DM process consists of netcdf files, figures and calibration coefficients that are stored in a database.
 
Data Levels and Dissemination
Netcdf files are created for various levels of data: L0, L1 and L2. The L0 netcdf contains scientific and engineering information as it is sent from the glider. L1 netcdf files contain calibrations, unit corrections and derived variables such as salinity. The L1 processing also Automatically calculates some of the delayed mode corrections including the thermal lag. L1 netcdf files are outputted in two separate formats, the SOCIB format shared through the SOCIB Thredds Data Server, and the EGO format pushed to the Coriolis ftp so it is aggregated into Coriolis (and in turn, into the Copernicus Marine Service) and GTS. EMOdnet has the capability to collect SOCIB data via the SOCIB Data API and the thredds server. It is planned that this mechanism will be applied to all of SOCIB glider data during the summer in order to respond to the European Commision to use the “real” source as much as possible with the purpose of making users closer to producers. Currently, SOCIB glider data is made available in EMODnet via CMEMS. Mission metadata is also uploaded to SeaDataNet by operators that create and upload cruise summary reports (CSR) for our glider missions. In addition to L0 and L1, L2 netcdf files are also created (gridded data of the glider profiles). The DM process creates L1_corr netcdf. All data outputs, L0, L1, L1_corr and L2, are also shared using the common SOCIB dissemination mechanisms (thredds, viewers, api,...). 
Metadata catalog 
Figure 2 highlights the importance of the metadata database in the data lifecycle. The combination between the metadata catalog and the processing mechanisms allows us to perform the flow in an automatic way. It also allows us to incorporate in the workflow, glider operations from institutions outside SOCIB. In fact, the same processing chain has been applied to various types of external gliders in the context of international projects and TNA calls. Our catalog records metadata related to the equipment (platform, instrument and sensor level), deployments and processes used to handle the data of each instrument is flexible enough to allow the registration of multiplatform observatories including gliders, research vessels, mooring, HFR, fix stations, weather stations, … This catalog is complemented with an User Graphical Interface that facilitates the glider operators to input their metadata. The information in this catalog is partially exposed through SOCIB Data API, which not only provides information of the data and data products but it gives access to the users to the equipment information in the database.
Vision into the future
Technical debts regarding the present workflow includes the link with Coriolis, which ideally should be readdressed to better use some of the machine-to-machine tools available at SOCIB, such as our Data API. In addition, we believe that the availability of a global database would simplify the process of collecting glider and mission’s metadata across borders. This database should of course provide the opportunity to link the metadata to datasets in a flexible way so the metadata can be updated afterwards by data operators. This metadata catalog should account for the fact that the data lives by nature in a distributed landscape. It will also be beneficial to have an API supporting the access and visibility of the metadata. A global metadata catalogue would also support the processing at a global scale by GDACs by providing a common metadata repository that assimilates the information of the operations in a comprehensive manner.
Internally, we aim to complete the automatic QC implementation soon. We also hope for funding opportunities in order to provide processing services to the community of various types of gliders by using our current infrastructure including our metadata catalog, the metadata editor application and the processing chain that is internally operational.
Coriolis
How to provide glider data to Coriolis (users point of view)
To provide glider observations toCoriolis, providers have to push the data to Coriolis ftp server.·        
ftp eftp.ifremer.fr
Contact codac@ifremer.fr for user name and password.
Glider data submission directory structure : submit/XXX/XXX_YYYYMMDD/ where:
XXX: glider name
 YYYYMMDD : deployment date of the glider
Inside each deployment repository, we need raw files (m and dat files for slocum, netcdf or bpo files for seaglider and gz files for seaexplorer) and json files containing all the necessary information (global attributes, sensors information, calibration coefficient) if the provider wants us to decode data. Otherwise, we need final files if the provider/DAC generate itself the files that we must disseminate.
Data recovery (Coriolis point of view)
If we must decode data:
We check the json files format and informations
We use a matlab decoder developed by Ifremer ( https://www.seanoe.org/data/00343/45402/ ) to produce the files to disseminate (explained in the next chapter). Note that a compiled version is available. It’s not necessary to have a matlab license to run the decoder 
If we get already decoded data:
We check the format of the netcdf files received. If needed, we produce the profiles files from the EGO/OCEANGLIDERS netcdf file. 
Note that we can get/produce/disseminate data in real time on a daily basis.
Data format
We produce and disseminate two types of netcdf files.
The timeseries EGO/OCEANGLIDERS netcdf file (at the moment describe here: https://archimer.ifremer.fr/doc/00239/34980/ ). It contains the full dataset of the glider deployment (one file per deployment)
·        
The netcdf profile files (one file per profile) when it’s possible.
Formats of these files are systematically checked by our format checker (available here : https://www.seanoe.org/data/00344/45538/ )
Diffusion
All decoded and recovered data are available on an ftp space ( ftp://ftp.ifremer.fr/ifremer/glider/v2/ ). We generate index files at the root of this space to facilitate the search for data
An ERDDAP is link the this space ( http://www.ifremer.fr/erddap/tabledap/OceanGlidersGDACTrajectories.html )
This ERDDAP is used for the map of the https://www.oceangliders.org/ website.
The profiles files are ingested into Coriolis database then automatically disseminate to different projects like Copernicus or Emodnet physics
It’s also possible to assign DOI to each deployment dataset (https://www.seanoe.org/data/00453/56454/ )
Summary of tools / documentations / link  used
Matlab decoder : https://www.seanoe.org/data/00343/45402/ .
The complete documentation available in the link. Some functionalities: decode data from seaglider, slocum and seaexplorer, create EGO file and profile files, apply NRT QC to data, possibility to compute some parameters with the intermediate parameters and calibration coefficients ( PSAL, BBP700, DOXY, CHLA, TURBIDITY)
Format checker : https://www.seanoe.org/data/00344/45538/
Format manual : https://archimer.ifremer.fr/doc/00239/34980/
FTP: ftp://ftp.ifremer.fr/ifremer/glider/v2/
ERDDAPP Glider : http://www.ifremer.fr/erddap/tabledap/OceanGlidersGDACTrajectories.html
Improvement
By experience, we have some difficulties.
For provider: provide complete and correct jsons. The way to fill/retrieve this metadata should be facilitated. As long as we have to check and correct the jsons, the ingestion cannot be automated. 
Get coefficient calibration: Very important for example to compute, validate DOXY. We have difficulty in recovering these coefficients from providers.
Manage a common format between DACs as all DAC use their own tools. The future OCEANGLIDERS format will help a lot.
How to contribute to OceanGliders (present  simplified approach to contribute to OceanGliders helping new users see past the differences between current practices in DACs; include/promote tools/services that can help people)?
Stage0 : Program registration (Adam Comeau reviewer)
What, Why, How, Who
Stage1 : Activity registration (Adam Comeau reviewer)
What, Why, How, Who
Stage2 : Data Sharing (Justin, Corentin reviewer, Claire, Yumi Song Reviewer, Miguel Reviewer)
What, Why, How, Who
Stage3 : Sharing data in Real Time (Justin, Tania,  Corentin reviewer, Miguel Reviewer)
What, Why, How, Who
Improving impact of Real Time data sharing ? 
Oxygen (Catherine S review)
Optical
Acoustics sensors, imagery? → link to specific repositories?
New sensors
Conclusion. 
Include discussion on harmonising practices
Step 1 detailed outline + assign people to write.
Step 2 meeting for each section with different people. Every two weeks. 5-6 people at each meeting - start with section 2 and 3 and t
Step 3 Jay pearlman advisor editor.

As a first step, the DAC representative will draft a one page to broadly describe the procedures they use.

The second step will be to harmonize the draft togethers and link to existing and more detailed documents.

A third step will be to get the review of a large community. The idea is to identify the gaps from future users.


The timeline has been suggested by Pierre Testor before submitting to Frontiers.
2021/09/01 is the deadline to get meeting participant feedback.
2022/04/01 is the deadline to get OceanGliders community feedback before submission to Frontiers.
Groups of DAC representatives : John Kerfoot (US IOOS), Victor Turpin (OceanOPS), Justin Buck (BODC), Corentin Guyot (Coriolis), Mun Woo (IMOS), Anh Tran (DFO), Miguel Charcos (SOCIB). 
Other documentation are required and missing  : 
Metadata management: Best Practice for the use of vocab services for 	OceanGliders. 
Best Practices in data dissemination to other networks and infrastructures. 

------------ Note from previous meeting -----------
Draft half page first each DAC, share together, and see if we are able to draft

Real time data and metadata flow: From operator to GTS / From operator to GDAC / From operator to OceanOPS 	+Kerfoot +Justin + Miguel
How to make the most of real time data flow! The example of oxygen. Document the metadata needs for effective utilization of oxygen data from gliders. 
How to jump in and start providing data. Where do you start and why (OG1.0). From the beginner's point of view.
	How to submit data and metadata to OceanGliders and why - From a beginners view. (+ extra information - what we would like to have). 
	Groups of experience user : John Kerfoot (US IOOS), Victor Turpin - OceanOPS, Justin Buck (BODC), Corentin Guyot (Coriolis), Mun Woo (IMOS), Anh Tran (DFO), Miguel Charcos (SOCIB). 
Draft half page first each DAC, share together, and see if we are able to draft

Suggestions/comment from audience
Pierre Testor : At some point we would have to discuss what are the variables that are ‘OceanGliders’. Difficult question. For the moment, in the GOOS network specification sheet we have T, S, O2 and currents (broad definition can incl. turbulence, not relevant in RTQC yet). Might be better discussed in the data management chapter?

Selected SOP/document sections:


Adam Comeau : Operator to OceanOPS. Further definition, better definitions.
John, control vocab, searching and getting information easier. How do we deal with control vocab.

Meetings notes:
Set documentation regarding processing : metadata, parameter, units.
Set of documentation regarding QC :
Cookbook for argo oxygen is used for OceanGliders at Coriolis.
Thierry : build a reliable channel between operator and data center. CHla not yet fully implemented for gliders. 
John : RT difficult to access metadata needed for Oxygen processing
Victor: Metadata is hard to get
Overlap with Oxygen group.
access calibration sheets not to overload the operator workload
Thierry Carval to Everyone (4:42 PM)
By default, as done with Argo, oxygen data circulates in real time with a qc flag set to 3 (probably bad but correctable). As soon as we have the proper calibrations, qc is switched from 3 to 1 (good data)

Gui : Unique identification for data set and versioning.

Miguel : tool to update metadata. All metadata are not available at the start of the mission. Facilitate the way users provide metadata. (editor, online tool, data base, oceanOPS ?)

Tierry: It's up to end user to decide whether he wants to use doxy data flagged 3
castelao to Everyone (4:43 PM): @Thierry +1

Chari: comments on oxygen the Oxygen SOP group
Gui: points to the challenge of the right balance between providers and data centers
Gui: we can only make it easier to let data to move  John: some part can also be done on the DACs, ask not for more but less and ask for pdf etc, maybe we can add this at DACs

Stuart Pearce: sorry to make my comment here instead of the Zoom call, but my microphone was not working well.  As someone who very recently had to go from beginner to submitting data to a DAC, I would have appreciated an ordered background reading list to get over the steep learning curve.  Having to sort aimlessly through the “standards” and understand the terminology took a long time.  I was always willing to read lengthy documents, but often would find I wasn’t reading the right thing first and would jump around to find the next bit.  Since all the DACs have at least in common that you should prepare your own set of the basic metadata, I think that ordered reading might help. +1 (Callum Rollo)











May 21 Friday 
	16:00 - 17:30 CEST / 7:00 - 8:30 PDT / 22:00 - 23:30 AWST
Data Management: Review session (V. Turpin, J. Buck)

Participants: Pierre Testor, Victor Turpin, Jay Pearlman, John Kerfoot, Miguel Charcos, Yumi Song, Pauline Simpson, Sam Woodman, Claire Gourcuff, Catherine Schmechtig, Adam Comeau, Kate Patterson, Sue L’Orsa, Gui Castelao , Corentin Guyot, Tania Morales, Mark Bushnell, Justin Buck, Dan Hayes, Anh Tran, Soeren Thomsen

Meetings notes:
Discussion of metadata - is there an comprehensive metadata format that can be used widely? This could be completed as appropriate for each system so that not all elements of the format would be filled in. 
The metadata from slocum is not sufficient. 
How can we address versionings and unique identification. This should recognize the need to subset data sets and have unique identification.  This is needed for updates of data files. 

comment from Mark: Very good idea to make SOP detail paper a different document in the OBPS repo. Easier to update the various SOPs



















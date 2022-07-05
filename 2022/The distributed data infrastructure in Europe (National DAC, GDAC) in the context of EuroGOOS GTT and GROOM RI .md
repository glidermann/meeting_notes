# The distributed data infrastructure in Europe (National DAC, GDAC) in the context of EuroGOOS GTT and GROOM RI ?


# Date: July 5 2022, 14:00 - 16:00 CEST

Session chair: Pierre Testor (CNRS, France)

# Participants
Victor Turpin (OceanOPS), Pierre Testor (LOCEAN/CNRS)
**add your name and affiliation here**
Johannes Karstensen (GEOMAR), Catherine Schmechtig (CNRS), Emma Slater (NOC - BODC), Kimmo Tikka (FMI), Callum Rollo (VOTO), Yves Ponçon(LOCEAN/CNRS), Antonio Bussani (OGS), Antonio Novellino, (ETT - EMODnet), Patrick Gorringe (SMHI - EMODnet), Ailin Brakstad (UiB), Alexia Cociancich (OGS), Corentin Guyot (Ifremer), Inês Martins (IH - Portugal), Evi Bourma (HCMR), Maryam Hassani (UT), Nunzia Pirro (OGS), Claire Gourcuff (Euro-Argo)

# Agenda
1) [Welcoming and meeting objectives](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/WS2_1_welcome_PierreTestor.pdf) – 5 min (Pierre Testor)
2) [Introduction](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/WS2_1_Introduction_Victor_Turpin.pdf) – 10 min (Victor Turpin)
    + GROOM I outcome
    + Status of EU real time glider data flow (GDAC and GTS)
3) Presentations of EU glider data aggregators – mandate, gliders data providers, data distribution and users - 45 min
    + [SeaDataNet](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/20220705_GlidersInSeaDataNet.pdf) (Michèle Fichaut)
    + [EMODNET Physics](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/20220705_EMODnetPhysics%40GROOM1.pdf) (Antonio Novellino)
    + [Copernicus Marine Insitu TAC](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/06-INSTAC-CopernicusMarine-GROOMII.pdf) (Sylvie Pouliquen)
4) [Discussion](https://github.com/OceanGlidersCommunity/meeting_notes/blob/main/2022/WS2_1_welcome_PierreTestor.pdf) – 1h – (Pierre Testor)
    + Which real time data flow for the infrastructure?
    + GTS delivery
    + Delayed time data flow
    + Agreement from the audience to review the Road map

# Meeting notes
Intruction PT : Maps from different data integrators are not always similar. There are overlap, but very difficult to have a unified overview.

Meeting objective : Bring community together, discuss relevant DM topic. Week 1 was about where we want to be in 2 years time. DM services of GROOM RI

Week2  : where do we want to be in 5 years. Evolution of the DM structure of trhe GROOM RI and optimization of the current system.

Decade of work regarding data managmeent. the sketch of data flow is demonstrating this progresses. But there are issues in this flow. Introducing confusion. GTS is also an issu.
Unsuccess in the delayed mode. Great progress but issues, BP to set up to make the system more robust and efficient.

EU data aggregators will present.

1h discussion after that. Question in the agenda. take time to think of it. 
Final question on agreement amongst partners, technicalities, financial support, etc.


### Victor Turpin presentation :

Groom 2 roadmap

Identify gap in data infrastucture. Identify key partners
Scheme is the outcome of GROOM 1. "GROOM 1 butterfly". All data push through to GDAC via DAC. DAC produce common format. GDAC distributes downstream.

Some difficulties: hard to maintain in the long run. Some nodes recieve data multiple times (CMEMS, EMODnet, Seadatanet). GDAC not recieving most of the data. Want to rationalise and simplify this. nrt flow sometimes more complex. How to converge to unique GDAC/central portal/distribution node? Goal of today's discussion. What is the national data centers' role in this. 

Delayed mode data in Europe do not reach the GDAC. Hard to see who is pushing data to GDAC. Clarrify who is in charge of delated mode processing, QC and pushing to GDAC. It's a lot of work. Cannot be achieved by PIs, last 5 years show this.


### Michele Fichaut Seadatanet - IFremer , French NODC

Coordinator of SeaDataCloud and SeaDataNet 2 projects.


SeaDataNet is an EU research infrastructure. Covers multiple projects from the 90s. Role is to federate EU NODCs monitoring EU seas. Single virtual data centre allows users to search data from 35 countries. Represents more than 100 NODCs. Distribute complete datasets to priveleged users. 

SDN is also AISBl, head quarter in Bruxels.
Infra funded by projects linked to SDN (EMODNET, envri FAIR, Blue Cloud)
SDN collect DM data from NODCs (physics, and other type of data)
SDN chemistry has already chemistry data

SeaDataNet sits underneath EMODNET. SeaDataNet is a high quality archive of data. It is exposed through EMODNET and COPERNICUS MARINE services. SeaDataNet is not oriented for nrt. Works with delayed mode data

Mandate for glider data: ingests, validate and store glider data under EGO. Deliverable: map EGO file format to SDN format (SeaDataNet format). At present only take data from EGO/copernicus GDAC, not from European DACS. 


Expend data type to new data type. Task led by BODC, design to work in cooperation with GROOM. EGO file mapped to SDN format.

Data put in SDN from copernicus. Converted from EGO format to SDN format to be distrubuted on the SDN portal.

via the [octopus tool](https://www.seadatanet.org/Software/OCTOPUS)

EGO files managed by Coriolis are send to SDN.
Only few data sets can be converted. Due to errors in the metadata. inconsistencies between flags and value. Inconsitancy in the QC format.
Missing mapping to vocabularies (P01, platform code and names)

Many EGO files have errors. Missing global attributes, bad flags, missing maps to BODC codes...

To move on, files have been copied in a separate place in SDN and corrected there. Feed back to data provide (DFO, CSIC) 
New data updated every 3/4 months.

Have converted 492 glider files to SDN format (81 %). Update every 3-4 months. Each glider data file has metadata file, accesible through the SDN webapp.

Distribution of the data, 1500 files downloaded (CMCC) to make the product to SDN and 

Emma: have you considered using ERDDAP to convert to your nc format?

Michele: Want all the data in the same cloud, ERDDAP is not well adapted to this purpose

Victor: Better than data delivery to SDN goes via EGO/copernicus rather than direct from DAC. New OG1.0 format will solve most issues raised by Michele here. Hopefully easier in future

Mark: We've been chasing a moving target with EGO. Be good to have a stable format that resovled these

Claire: Surprised at errors during file conversion. Thought there was a checker at GDAC level to enforce format compliance? Is problem with EGO format or with checking at GDAC level?

Michele: Should be a checker, but errors still present. We considered implementing checker at first, but considered files correct initially. Now there is check and correct in octopus

Corentin Guyot: Errors are due to old formats. All files have not been regenerated. Last evolution of the EGO format are aligned with SDN requirements. The checker must evolve with the format. The last format and checker are fully compliant with SDN.

Pierre: Could have avoided this work at SDN if old files had been reprocessed. This is an issue at EGO.

Sylvie : As long as the activity is funded the work can be done in due time. Otherwise delays and overlaps is diffuclt to avoid.

Emma : Sometimes SDN have mandatory information that are not mandatory at the EGO level. Empty variables are unchecked while it is checked by SDN. also P01 vs OG1 vocab can be an issue. 

 
### Antontio Novellino: EMODnet physics
Antonio Novellino : Update of the situation in EMODNET Physics. EMODNET Physics is under important evolution currently. Good to present it.

EMODnet is a program started 10 years ago. Networks of experts to provide commission with specific products. Now in the centralisation phase. By the end of 2022, all thematic portals will be combined into a single point of access. In parallel thematic blocks will get more power to support providers with their data flow into EMODnet. 

EMODNET 'centralization phase'. Move all the portal to accessible in the same data portal.

Aim to collect data in RT, nrt and delayed mode. Both in situ data and reanalysis.

Combining international sources not touched by other EU initiatives (river flow).

Supporting harmonisation and common standards: Not reinvent the wheel.

System is global in scope. 

EMODNET Physics is not only about data. Give help to communities to deliver, and make visible their data. HF radar is a great exemple of how EMODNET Physics can support network to deliver data to EU data aggregators.
The cooperation between EU data aggregators is a reality and is key for mapping the same data ingested from different sources.

Ingestion process: connect to more operators. To accomodate new data sources consistently. Adopted two phase approach:
1. As soon as connected to a provider, make data available "as is"
2. Validate metadata, map data to consistent standards (INSTAC) and now provide the new data to users

Work in partnership with SDN etc.

Better organise activity: eurogoos, SDN, emodnet, CMS INS in the Marine Insitu Collaboration Working Group. Example of recommendations: identification. Best way to identify data and platforms

Backend: moving toward centralisation:
- Data layer
- Service layer: monitoring etc.
- Application layer: map viewer, API, web catalogue

Developping tools for M2M exchange:  adopted and support ERDDAP. Have a well-working docker application for this. Can provide it to people willing to set up their own ERDDAP. EMODnet physics set up an ERDDAP docker in China under another collaboration. Working well for other people too. VOTO have also set up an ERDDAP with the help of EMODnet team. 

Important to think of the tools we use for dataflow. 

EMODnet work with glider community since 2018 workshop. Push towards KPIs for oceanOPS. Common and unique format for glider data. 3 levels of timing for glider data:
- near real time push to GTS
- recovery push by prodivers for higher res data. 
- validated data to NODCs
At the moment, only nrt data is being made available. As Michele presented, only able to get data from Coriolis. Big hole in data provided.
Developed scripts to support oceanOPS: creating KPIs. Part of oceanOPS dashboard.
Can see glider data on emodNET physics portal. Interactive plots, data download etc. Uses ERDDAP under the hood, so get data in whatever format you want. Make many processed products available from glider data. e.g. SST from operational gliders.

**questions**

Victor: How did VOTO ERDDAP work? ERDDAP displays VOTO data, how do you collect data in common format?

Antonio: Can use ERDDAP for two main purposes: easy way to collect data from your system e.g. if glider is transferring from a specialist format, get ERDDAP to ingest in this format then have ERDDAP display all the metadata that you want. Operational dataset can then be made available by ERDDAP. Tell ERDDAP how to map input variables to standard vocabularies once, then works for all future data input in that format. Docker isntance they provide does not currently support OG1.0 format, but we can work on this.

Victor: Good that this solution is provided to users, but for research infra like GROOM, we need to common format available. All people are busy, we need this tool to be adaptable for GROOM requirements.

Antonio: In last 2/3 years we are really pushing providers to setup infrastructure. This way data responsibility stays at provider level. Aggregators just point/link to the data. Start from same sources and formats.

From practical perspective it is easy to set ERDDAP system up.
What is needed is to set up the ERDDAP to be a single place to take the data format.
Can be a solution for other providers, not only VOTO. OG1.0 will be an export option from ERDDAP once the format is finalised and an export function is incorporated into ERDDAP


# Copernicus Marine Service : Sylvie Pouliquen
Copernicus deals with past and present data, green, blue and white data.
Cooperation with SDN and EMODNET is operational. Lost of common gliders data between the three Integrators.

Copernicus is focusing in a limited number of parameters needed by the modelers. Glider is one of the plaform integrated by INSITU TAC (more than 7000 platforms).

INSITU TAC collect and perform automatic QC on the data and provide homogeneous quality data sets in NRT. Extra quality control every 6 months.

Catalogue allows providers to know how many people have use their data (link in the presentation). SOCIB is sharing data and use is well tracked by Copernicus.

No real GDAC so Copernicus must get the data form the GTS too. If a central portal would be set up, the Copernicus data aggregation would be simpler and easier to track.

Most of the users are scientist (2/3rd). Multi platform / Multiparameter is the number one product.

As for Argo, an OceanGliders GDAC is the way foreward. But in the meantime, priority is Coriolis, then Local provider, then GTS.



Mainly provide data via ftp through Copernicus Marine

Recommend following FAIR principles. This is a deliverable to uniquely identify data and use of common vocabularies

Recommend to setup portal with best version of GROOM-RI data. So delayed mode data should be provided here. Avoid different versions in difference services. Aggregators should now have to guess which is the best version of a dataset. Happens if data arriving from several streams.

**questions**

Pierre: what is the place of Coriolis? Could it be GDAC from gliders?

Sylvie: not presented as Coriolis is under the EGO GDAC. Within GROOM 2 era must identify who is institute to do job. Could be Coriolis or someone else. It is a commitment. Coriolis did it during GROOM 1. Discussion open in this GROOM 2 era.

Emma: what is the time target? BODC push to UK Met Office quicker via GTS than GDAC.

Sylvie: Pulling within a few hours. Within argo push to GDAC and GTS at the same time. Could be the same for gliders? Generate nc file and push it to both streams

Emma: Need to speed up GDAC ftp harvest. Currently it is daily.

Sylvie: Currenty every 30 minutes

Pierre: Target is a minute! Very ambitiuos. Hurricate prediction wants it within the hour.

Sylvie: Hurricane data should come through GTS. Faster the network can provide data, the faster we can process/distribute it

Victor: Coriolis as a GDAC has not disapeared. But why is it so difficult to make progress with this scheme? Is the current schmeme not good? Or do we just need to push conclusions of GROOM 1 more? GTS, is there a national duty/legal constraint? If so national met office should support the task. Otherwise this EU infra can handle it.

Sylvie: for argo, conclusion is data has to go via national met office. Should not bypass met office


Fiona Carse NOC: Glider, Argo, Seal are pushed by UK NODC. For UK Met office it is not a legal obligation that they handle the data, only that they ensure it is shared

### Open Discussion

Victor: Vision of OceanOBS and OceanGliders technical coordinator. I don't think it is necessary to rethink/redisign nrt. Lots of groups are doing the job properly. Need to engage more people in an easier way. Should be easy for a glider group to enter the dataflow. ERDDAP is good for people who can enter the system. What about QC though? This is currently done at DAC level. How will this be applied in ERDDAP model where data collectors are providing the data themselves. ERDDAP is good for collecting data

Sylvie: ERDDAP is an API to access data. If there is enough metadata it is good. Need to have an API to access all EU data in one way. In GROOM 1 we advised to put it all on an ftp at a GDAC. Maybe you want a more distributed system, but the user should have a single point of access for the end user. With ERDDAP you need an ERDDAP that points to all data, not just at one hosting point. 

Pierre: ERDDAP is a tool for data managers, not for PIs. Don't feel like the community of operators have the experience to use is. Is there a need to centralise data somewhere? I like the ftp, even if it doesn't provide complex services like discovery. Nice simple way to get at the data though.

Victor: ERDDAP is another way to push (or give access of) data to one central place. Still want one central place for this. This is necessary for OcanGliders. We have the processing chain, others have e.g. the SOCIB toolbox. ERDDAP is another tool for data conversion, but we still need a GDAC for monitoring distribution etc.

Antonio: Concerning ERDDAP. Easy tool to facilitate federation. If you have ERDDAPs at provider level, easy to have a server that links and explores all those servers. Does not serve QC! That needs to be done by some other tool/process. For people who are willing to setup the system, the common catalogue will directly to link to theirs. For people who do not have this ability, data can be hosted by the central catalogue ERDDAP directly. The concept of ERDDAP seems like an ideal tool for this community. For those who wish to share data, can keep doing so. ERDDAP can just read the ftp server and provide that data too. This helps interoperability with other communities.

Fiona: Met office to make some Irish argo floats available through GTS as this project doesn't have resources for their own dataset, so this kind of thing is fine. Also euroargo processing data for smaller countries

Sylvie: Need to have the data and information in the EGO format made available by glider operators/data centres. This is the first thing. After that consider data availability like ftp, ERDDAP etc. But first must have the mandatory information! Lots to do in metadata specification in EGO/OG1.0. This must be done first. ERDDAP is a clear contender for this, but get the data correct first. What do we need to do to enable this for data providers?


Johannes: full agree with Sylvie. When we add inter-disciplinary teams need to consider their flow. e.g. dissolved CO2 system. If we need a GDAC to ingest physical and BGC data, what is the rationale for this? Could ERDDAP just provide a place for the data? From mooring network we have a good data format, but things like pCO2 are archived at a totally different data center that has no conception of ocean science data storage practice. More of these things will come up in future. Could be incompatible with single GDAC goal.


Pierre: must think what infra is needed. Doensn't prevent us trying to make a good solution for the variables we have now

Johannes: Making an ERDDAP server to link to many datasets provided by the wider glider community is great. This obviates the need to a GDAC in my opinion. Antonio has setup ERDDAP servers for many different communitied. Federated together these make a GDAC

Pierre: These ERDDAPs must be setup and maintained. What we choose will depend on resources available. 

Callum: We're waiting on finalising the OG1.0 format so we can push data onward

Rob Thomas: erddap.com to search for data in any ERDDAP. need to refine data, but you can search for metadata terms like "glider"

Sylvie: Need this glider data standard. This is a blocker to providind data to GDACs. What is blocking other data providers? We agree that we would like a common point of access to this data. No consensus of what this point would be, ERDDAP is one option. 


Emma : from DAC metadata is the most delicate part... Lots of is effort is down on DACs. This should be shared with PIs, and Operators. Sensors from manufactuere are not providing standarded engineering units. Collecting metadata requires a lot of manpower, especially if multiple gliders are deployed. This work could be shared with PIs/engineers. If these people put in metadata this would make things easier. Lots of duplication of effore


Sylvie: Had these problems with Argo. Asked manufacturers to provide some of this data in machine to machine manner. We collect metadata when mission is planned, rather than waiting til after recovery. This could be done by glider engineers

Emma: Many sensors can be attatched to gliders. We also recieve data in different file formats. 

Pierre: PIs are struggling to provide (meta)data of adequate quality. What can we do to help them?


Sylvie ; If you could provide us with the best version of data Copernicus could rely on this data set. From a central access point. Will facilitate and secure data to this community.

Pierre: DOI from Seanoe should be updated.

Sylvie : Format must remain the same between the different data sets. 

Johannes : Access to many gliders data is avaible on Pangea. The question is why are they not harvested ? Published in Pangea you get a DOI (same as Seanoe). 

Many PIs are not ready to serve Delayed mode, QC's data to a GDAC that mixes up DOIs etc. This is a labour intensive process that is not present for argo, as argo floats are never recovered. Heterogenic by nature. DOIs are important, national commitments may force people to publish elsewhere. Best for GROOM to collect info on where the data are hosted. Not to copy it.

Victor: Understand Johannes' point, but concered for data format. What is the format on pangea? If it is not common with other datasets or with nrt data. How will people use it for bigger applications? Good that it's published, we can harvest it, but format matters

Johannes: The format is a detail, but the metadata are all there. Will find a zipped netcdf of something like the EGO format in these pangea datasets. It's important to agree on this standard format.

Victor: For data aggregators, this common format is not a detail. It should be something we rely on. Otherwise we cannot work with it.

Claire: Raise issue of high resolution data for gliders which do not send all data in nrt. Data that you collect just after recovery, where do they fit in? How do we address this? 

Pierre: As shown in presentation it should be provided by the PI to the DAC.

Claire: Would operational centers want this unprocessed high resolution data?

Pierre: data quality more important for delayed mode

Victor: Antonio showed idea of this "recovery mode" data. It is unclear at present how this is managed. Need more clarity in the roadmap. Do we use this or only rely on delayed mode? Not clear in 2018, still not clear now.

Kimmo: Lots of effort put in to remove duplicates. If we have many levels of processing, which version of data is then saved/used? How can the system hadle this?

Victor: without a formal statement/engagement face the same risks seen today. Data management has a cost. Must be taken into account

Sylvie : The road map is for the RI, what need to be done, who will do the differnt task. If you stop on what needs to be done, and do not consider the cost you would not reach the level of an infrastructure.

Pierre: Map the resources, what is done today... What would be the mandate and scope of the GROOM RI ? What would you like to have has a european support for data management ? Wish list !























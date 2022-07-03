# GliderTools

Welcome to the “GliderTools” room. 

Session co-leads: Isabelle Giddy, Thomas Ryan-Keogh, Dhruv Balwada, Callum Rollo, Sarah Nicholson, Soeren Thomsen


## Agenda
May 24 Monday 
	16:00 - 17:30 CEST / 7:00 - 8:30 PDT / 22:00 - 23:30 AWST
GliderTools: (I. Giddy, T. Ryan-Keogh, D. Balwada, C. Rollo, S. Thomsen, S. Nicholson)

You missed the session? The discussion goes on here: 

Presentation

Original GliderTools publication

Current GliderTools capabilities and potential: Show some example notebooks (Callum Rollo)
https://github.com/GliderToolsCommunity/glidertools-demo 

Joined discuss future vision of package structure (Soeren Thomsen)

GliderTools as a way to promote Glider Best Practices (all)

How to get involved? Join the discussion on GitHub at any time, no Python coding skills required! (all)

Important link: 
https://github.com/GliderToolsCommunity/GliderTools 
https://github.com/GliderToolsCommunity/glidertools-demo 
https://github.com/GliderToolsCommunity/GliderTools/discussions/107 


Participants: 
Soeren Thomsen (https://github.com/ThomsenSoeren/)
Dan Hayes, 
Gui Castelão (https://github.com/castelao/)
Sarah Nicholson (https://github.com/sarahnicholson)
Thomas Ryan-Keogh (https://github.com/tjryankeogh/) 
Callum Rollo (https://github.com/callumrollo/)
Carolina Amadio, 
John Kerfoot (https://github.com/kerfoot/) 
Isabelle Giddy (https://github.com/isgiddy/) 
María Valladares, 
Yumi Song, 
Dhruv Balwada (https://github.com/dhruvbalwada)
Tom Hull (https://github.com/tomhull/) 
Filipa Carvalho, 
Brita Irving, 
Julius Busecke (https://github.com/jbusecke/) 
Nikolaos Zarokanellos, 
Alice Pietri (https://github.com/AlicePietri/) 

Meeting notes:
Tommy gives Presentation on History, timeline and outlook of GliderTools
Callum goes through the glider tools-demo 
 
Try to get an uniform format for OceanGliders
3 DACS, IMOS, IOOS, Coriolis
Chari: Will you be able to import different format nc files? The different DAC formats?
Callum / Sarah: Already can / should be trivial to add different formats.
Chari: It isn't trivial to do, have to test with the standard files.
Gui: There will exist different formats - translate as much information as you can to a common format OG 1.2. 
Question: What is the purpose / Vision of GiderTools?
Tommy: DMQC: Code to implement / integrate best practices (or options to do this)  
Soeren: If integratable/interpretable tools already exist - not plan to rebuild, but integrate to GliderTools  - manage community efforts , available tools could fall under GliderTool community 
Gui: Think it has power to be more that DMQC - power in data exploration as well, to help ask scientific questions 
Izzy: Would it be useful to add statistical methods to this as well then ? 
Charitha: other products, derived variables, subsetting data, visualisation, manipulation - lots of steps
Soeren: Focus on the development of GliderTools - future vision, not what is there already 
Charitha: GliderScope? https://imos.org.au/gliderscope matlab based
Dhruv: GliderTools is open source - everyone's tool
What about geostrophic velocity/ gridded plot -come functionalities are there, not all of them 
if you have three things you want to do, a new entrant can see a standard method for implementing some of these variables - GliderTools can provide the details 
is Gliderscope open source, are the details well documented, if there is someone new can they contribute and discuss - how do they do that? 
Charitha - gliderscope version 8 released 2 months ago, not open source yet - they don't have enough support for this to be open source yet, matlab based , version control has been a problem
Julius: - git based workflow handy for version control - open source projects need someone/group of people to keep an eye on things 
important that things are discussed openly (i.e not long email lists), github discussions useful for this
only rigid choice around software is that everything is designed around xarray  - everything else is modular
get data into xarray (eg through a parser )
if software is designed well enough/modular enough can be used broadly
could be open to implementing more functionality, but focus first on a common workflow 
Gui: - Being open source doesn’t mean a community software
leaders - different ways to guide open source? 
specific cases of glider types of data which makes things easier afterwards (xglider)
a monolithic package reaches a stage where it becomes limited, so split - more in favour of an ecosystem instead of one big tool that does everything, not one solution for all - build compatible tools that are interpretable? 
support for Charitha  - difficult to share software, but huge value in well established tools 
Dhruv: suggest access, allowing new people to build on / convert code from matlab to python/ see the steps involved 
Gui: Difficult to bring old packages to the new way we work 
Charitha: 
- not going to learn python at this stage but happy for someone to convert  gliderscope to python - doesn’t want to be the version control person 
gliderscope is a non-expert toolbox, target audience people who don’t have any previous coding skills 
Julius: community of people who try to bring all the knowledge together and make it accessible, maybe a future option could be to develop a GUI that doesn’t require source code. A big vision is to take over knowledge and translate it/ create compatibility across systems, not to lose knowledge or users. In the end, we want to do awesome science! 
Gui: Missing clear data model. Once there is a well defined data model, easier for tools to communicate with each other. 
Soeren: Suggest to keep GliderTools flexible. We need to think about naming of the toolboxes. Currently have GliderTools Community and GliderTools. But the idea is to have an environment of tools that are inter-interpretable/ compatible..  
Callum: xarray is a standard structure, don’t have to agree as a standard format for storing data as long as it can be pulled through xarray
Gui: Disagrees. xarray is not sufficient
Callum: What is missing?
Gui: how to operate with the data? profiles/ series of profiles, subsurface? There is more than xarray - how you use xarray. Data model - which kind of information and where to find these data , CF naming protocols. Clear data model so that tools can know what to expect.
Julius: useful if Gui can put in a specific example, there is CF xarray. These things are what xarray should be able to do. Suggests working directly with xarray developers. 
Gui: some procedures are useful to treat as profiles, timeseries, chunks - move discussion offline (Julius: @gui I would love to )
Tom: - dbd reader; associated flight model - api join with those packages 
very interested to see source code from glidescope
Charitha: Formatting:  3 DACS; the differences are what you call the parameters so the glidertools method for reading in is flexible and would work with these formats. Problem is which format do you specify -suggests a table with naming protocols spelt out 
Dhruv: is this technically difficult/cumbersome
John: Metadata. Doesn’t see the translating of formats as impossible. OG 1.0 format is very heavy on metadata.  
Chari: Also taken other data into account, IMOS, 25 platforms to collect temperature data, change this from old data
Dhruv: Some of the issues of naming/metadata - things are a little upstream of glidertools, once some consensus is reached, glider tools can move from there.
Callum: Case of being flexible at this point 
John: Take home point: work to do translation is not trivial, but well within the realm of possibility - fundamental issue is getting the required metadata. None of the DACS are going to scrape what they have been already doing. Going to need to write translators. Likes the idea of fundamental underlying data model being xarray. Can write a separate translator for each format and attach to glidertools. 
Chari: raw manufacturers data to netcdf  
Gui Castelao: For instance, if I want to communicate with CoTeDe (https://github.com/castelao/CoTeDe) with GliderTools, how should I expect to find the required information. For instance, where is the latitude for a specific measurement?
John: SLOCUM, native data format is frustrating. Has written a package that takes the .dat files from SLOCUM to translate SLOCUM data into something readable . Takes raw datafiles and saves as netcdf and then moves onto GliderTools. Offering his package https://github.com/kerfoot/gncutils;  https://github.com/kerfoot/slocum 

Julius: John’s workflow is 100% what pangeo recommends in/out xarray. Encode everything in attributes. Could factor out reading / visualisation into separate packages. Avoid “one thing does all”. Modular coding.  What is the union of all metadata? Can we get an idea of what are the same attributes and what are the unique ones? Best case is having all the attributes in the xarray dataset and putting defaults in for what is missing.  What is the ideal dataset that we want to process
with GliderTools.
Action item: Create a dictionary of all possible metadata entries (and possible names) 
Tom: First page - workflow diagram - guiding users to the right tool
John: dbdreader is doing the binary unpacking / johns package reads in tabular data 
Julius: Should we add a ‘related’/‘compatible’ package section in the docs?or maybe even ‘partially compatible’ as well
Gui: doing samples for OG1.0 - data model does not need to be OG 1.0; does not recommend it? for the software side, but using OG1.0 and a way to communicate between different groups.

Soeren: These tools can support smaller research groups, who don’t have inhouse expertise on all variables
Chari: We are trying to promote the use of Glider data - reach wider community, not limited to people using gliders, make people comfortable in using the data whatever discipline they come from 


John: Python package to import Slocum tabular ascii data files: https://github.com/kerfoot/gdm

Gui: Real-time QC tool CoTeDe (https://github.com/castelao/CoTeDe)
useful for operators 

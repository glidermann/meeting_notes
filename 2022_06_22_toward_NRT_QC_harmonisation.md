# Joint European data management workshop - RTQC harmonisation session

## Session details
22nd June 2022 15:00 - 16:30 CEST

## Agenda
Chair: Justin Buck
Notes: Callum Rollo, Victor Turpin 

[Opening presenation - Victor Turpin](link here)

## Participants
Justin Buck (NOC), Victor Turpin (OceanOps, France), Soeren Thomsen (LOCEAN, France), Maryam Hassani (UT), Pierre Testor (LOCEAN/CNRS, France), Dave Hebert (BIO.DFO Canada), Callum Rollo (VOTO, Sweden), Carolina Amadio (OGS), Kimmo Tikka (FMI, Finland), Clara M. Loureiro (UAz, Portugal)
- please at your name

## Notes arrising during opening slides (Victor)

- please support note taking

Gui has been leading NRT QC.

SOCIB toolbox, could not find NRT process applied in this toolbox.

Coriolis processing [link](https://www.seanoe.org/data/00343/45402/). Also used for Argo

Bastien Questse's [toolbox](http://www.byqueste.com/toolbox.html) works for nrt but is mostly used in delayed mode. No longer actively maintained

GliderTools can work in NRT with SeaExplorer, but designed with delayed mode in mind. 


IOOS qartod approach is by variable, not by platform. Has extensive manual. Regularly updated. Have many tests and QC methods.

IMOS have ANFOG user manual. Have automated and manual QC routines

[CoTeDe](https://github.com/castelao/CoTeDe) takes a different approach (by Gui). Idea is to implement modular tests. Can set custom test sets and thresholds. Can perform a tuning then store those settings. Could be beneficial for different ocean basins to use different standards.

Gui: Wide group. Surprising range of opinions between groups. Looking for common ground. Important for NRT QC is to consider pre-existing material. No sense in reinventing the wheel. Most of these tools have a lot in common. Started from XBT cookbook maybe? Have evolved ever since.

Victor: Toward a unified methodology in Europe? Want to improve datasets availability and user uptake. These would be improved by a compliance document for quality controls. Since beginning of EGO we want to share tools and code.

Soeren: Some parallels to status of delaye mode. We have linked some methods but not managed ot converge yet. That's ok. Still a good result. One option is to copmlete parameter chapters of the SOPs. Other option is dedicated document for each method. Minium would be to populate them with the existing. For next month at least. At least add NRT QC for oxygen and salinity


Gui: CoTeDe(https://github.com/castelao/CoTeDe/tree/master/cotede/qctests) implements common mechanics like spike test etc. We cannot setup a standard set of rules without making it very wide. The operator should define the tests and limits as they know the platform best. CoTeDe provides an engine to be tuned by the operator. The user sets this up by a json file. This file (https://github.com/castelao/CoTeDe/blob/master/cotede/qc_cfg/eurogoos.json) sets the tests to be used, and the threshold to apply.

Emma: from Rutgers meeting, we set up a slack and had a QC group (led by Inmaculada Ruiz). How should we communicate going forward? That channel has gone quiet. If tests are better fine tuned to regions, are people publishing those limits and fine tuning so others can use them?

Gui: There has been no activity in this QC slack group for some time, mea culpa! I have no authority here, I am just giving my optionion, "Gui's opinion". We want a curation of configurations. CoTeDe can handle many data types. Going forward we want to configure the tuning, curate the thresholds that are being used. Would be good to have those available for new users.

Victor: That slack group never picked up momentum. Shows that that was the wrong method perhaps. Now we try another method.

Justin: How do we get momentum going forward?

Callum: Do we wait for OG1.0 before implementing QC?

Victor: OG1.0 should have a QC array for each variable. The procedure is independant from the format however.

Justin: OG1.0 is very similar to EGO. It is if anythign simplified, no extra time dimenstion for GPS for instance. In OG1.0 have a simpler timebase, so EGO tools should work with OG1.0. Just need extra metadata in OG1.0

Gui: OG1.0 is independant of the QC procedure. OG1.0 would faciliate the design of these QC tools. It will make the job much easier.


## Discussion topics and notes

### Which approach ?

Soeren: key learning: small interoperable packages. Not monolithic. OG1.0 would help. Make an effort to make these tools work together.

Justin: Are there pre-requisites for a hackathon of a QC project? How much prep work needed?

Soeren: Get people to talk and document it? Meet up again a couple of months later. This attempt was made to glidertools but didn't really kick off. It's useful to have an org that will pay someone to work on other people's open source project. This is the pangeo approach and is being adopted by e.g. NASA. Support open source and harmonisation. Introducing this culture to a community

Gui: Agree with Soeren. Community has to decide to use or contribute to open source. As an org we have to propose a curated definition of procedures. If you will use a datasets, should record which tests with which thresholds were applied.

Emma: How would a hackathon work? How would you define whether something has passed? How easy is it for someone to integrate code into their systems

Soeren: Problem is lots of tools are hidden. Need will of people to adopt open source languages and make it opne for contrbutions. Need it open to contribute not just free to use. a user wants to see how well used a package is. All new PhD students are familiar with this approach, this is the way the wind is blowing. On top have some professional coders to maintain it.

Justin: where do you envision these pros coming from.

Soeren: Julius helps our repos. Pangeo have a mission to support open science. Rabernat allows this as he wants to support this ecosystem. Need someone skilled like this to do hard technical stuff. Because of this work they attracted funding from NASA and it snowballs. Demonstrates how they can support other communities.

Gui: basic concept is once you get critical mass it's easier to pay short time to make incremental improvements. A hackathon should not require any previous knowledge. Take contributions from people who aren't coders.

Victor: see benefit of open source for new generation. Should not throw away historic tools of older groups though. Urges caution on how to move forward on this. More tools, more diversity makes us more robust.

Soeren: Reality is that old tools will become obselete/outdated if they are not made open source. People retire. Tools are abandoned. New students want to contribute. Tricky to work around patents sometimes. Scientists want to share but sometimes cannot. 

Justin: Currenlty raising this at NOC. Need an institutional policy on open source to make it easier for us to engage with such developments 

Kimmo: I support open source, thus when packages grow, decisions made in code should be documented. So github with active developer base would be a good solution. Problems I have mat are, for example, usage of propietary sofware/packages (matlab&packages). Some codes needs to be used with some type of gliders, maintaining the compatibility between code and platform is hard.

Justin: DO we need to increase skills of the community to make these tools more usable. 

Kimmo : Find format from which we can start using toolboxes. **One common format for all glider types**. 


Justin: Key question, how do we compare the results? Can set out to make the same test but get diffent results. Inevitably these tools give different results. Takes a lot of effort to test those


Callum : Test data set to test the tools. Simple approach. For several gliders.


Soeren: we get test datasets from OceanGliders. Owners of those datasets can check the tools to see if they meet with the groups approval. Have challenges in the test datasts. Does your tool fix it? Great for e.g. time lag of oxygen data. How to motivate developers of tools? No one wants to set up this on a per tool basis. Someone needs to set it up...

Gui: open source directly resolves this if everyone has access. Comparability is important. Over the past decade we have evolved from personal use to something better. Very important to consider ethics of open source. Cite sources and reference where the work came from. Commercial interests must be guarded against. Make sure people's effort is respected, not stolen.

Soeren: OS often used to save money. Getting free labour from the community. People need to earn money. Projects like GROOM should include budget for OS development. 

Justin: would open science policies effectively override institutional policies to make such collaboration possible? If all results must be open access, code must be too. Public funding == public access.

Soeren : How to move to open source without pissing of the people who have develop tools for decades ? We do not want to loose their knowledge and activity in the development of the community tools.


Callum: what tools are poeple use right now? Are they happy with them?

Gui: What is needed, how do we share knowledge?

Justin: At what point can we begin a hack concept?

Gui: What is the objective? Everyone has great knowledge. What can we achieve better together? A hackathon? Could do one next week! Key to have a goal though. People want to invest in something that will save them time.


Justin : You are describing this as key objectives of the BP you are leading?


Gui: we can share knowledge without reaching consensus.

Emma: in BODC do not want to develop a new QC tool. Do not have the resources for that. Want to share the burden. Could be things we miss that others have noticed. Want to adopt a community built tool where they can contirbute a bit. 

Justin: agrees

Victor: Coriolis has an open processing chain. Is developed by one institute. Can request to use it for free. How is this different from the open source tools we want to develop?

Soeren: motivation is low to contribute to something if there is no mechanism to do it? It is open but not open source. No feedback for the community.

Gui: It's more than just applying a patch or an Issue. It is at a community level, you can change the scope of the project, change the team composition, make design decisions. These are the hard things that we can do with a truly open project. This is the importance of a community. 

Justin: we have experience with Coriolis data processing chain. We use it for argo. Have had to put a lot of effort into including it in our CI system. This was a lot of effort! Also we're moving to Python. Coriolis uses matlab. This is where you get differences. See it likely to have a toolbox doing a similar thing in each language. It's not that one is better, but different orgs standardise on different environments. It's ok to have several tools. 

Soeren: argopy has been adopted as a community project now after starting a community project. This sharing of the load helps

Angel: argopy is a great tool and great example. Comes from a matlab background but appreciates the effort now. Hackathon: take some existing glider profiles with known outcome and see if the tools can fix it. e.g. give them nrt or subsampled profiles and see if they match the results that we know from a manually processed full dataset. Make some notebooks! Students like these things.

Justin: follow ups. We shold make issues on the NRT QC github repo. We should get those issues raised ahead of week 2.

#### Minimum set of test ?


#### CoTeDe


### Which tools ?


#### Sharing code ?


#### Compare results ?



### Which timeline ?


### Which team ? 
#### European ? Global ?


#### Who are the expert ?
- Gui

### Key actions to progress the topic?


### Who wants to contribute please?


## Comments:
Soeren: - each of the 4 OceanGliders SOPs has a dedicated RTQC section. It would be great if these documents are the place to converge. At the moment we are only listing approaches there but everything is set up and we now just need to populate these sections, refine, converge add code etc.

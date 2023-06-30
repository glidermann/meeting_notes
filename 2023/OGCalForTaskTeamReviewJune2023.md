# Progress report from the OceanGliders data management task team
In responce to [https://www.oceangliders.org/wp-content/uploads/2023/06/OceanGliders-Call-for-Task-Team.pdf](https://www.oceangliders.org/wp-content/uploads/2023/06/OceanGliders-Call-for-Task-Team.pdf )

## Chair and co-Chair
Dan Hayes (hayes.daniel@ucy.ac.cy), Victor Turpin (vturpin@ocean-ops.org)

## Membership
Justin Buck (BODC), Guilherme Castelao (SIO), Thierry Carval (IFREMER), Juan Gabriel Fernandez (SOCIB), Emma Gardner (BODC), Corentin Guyot (IFREMER), Mark Hebden (BODC), John Kerfoot (US IOOS), Miguel Charcos Llorens (SOCIB), Kevin O’Brien (NOAA), Benedicte Pasqueir (IMOS), Callum Rollo (VOTO), Jennifer Sevadjian (SIO), Mun Woo (ANFOG, IMOS).

## Report on progresses
The initial group formed in 2018 was pretty large with 111 members reachable through the Task team mailing list (og-dm@jcommops.org) and gathered around the slack channel [https://oceangliderdmtt.slack.com](https://oceangliderdmtt.slack.com).
It is worth saying that the mailing list and the stalck channel are not often used since about 2 years.

4 working groups emerged at the early stage of the task team.
* Format harmonization
* BUFR format
* Real Time QC
* Delayed Time QC. 

While Format harmonization and BUFR format working group achieved their objective (see paragraph below), the Real Time QC and the delayed time QC did not progress much. Thuse, we will not report about it here.

### OG1.0
The group met regularly since 2019. Status of the discussions and format is reported here: [https://github.com/OceanGlidersCommunity/OG-format-user-manual](https://github.com/OceanGlidersCommunity/OG-format-user-manual).

The group manage to finally reach a consensus on a common format. The latest version is accessible here: https://oceangliderscommunity.github.io/OG-format-user-manual/
There is a need now for a large communication about it and work on the remaining but not blocking issues.

Despite this great progress, there are many topics to be develop to strengthen the OG1.0.
Amongst them vocabularies and real time QC.

This topic are part of the draft work plan being drafted by the OceanGliders data management task team.

### BUFR format
There is now a BUFR format dedicated to OceanGliders data. 
Ocean Glider’s BUFR format is defined in [WMO's table D by descriptor 3-15-012](https://github.com/wmo-im/BUFR4/blob/master/BUFR_TableD_en_15.csv). 
The archived proposal and related discussions can be found at: [wmo-im/BUFR4#16](https://github.com/wmo-im/BUFR4/issues/16)

The format only concern Temperature and Salinity data. We made that choice to accelerate the validation of the format with WMO colleagueS. .
Agreeing about chla and Oxygen data was more complicated than expected and the use of those data opertionnaly, through GTs, without accessing the calibration coefficient of the sensors (not available in the BUFR format) make limited sense compared to the benefit of having a dedicated BUFR format for gliders for T and S data righ now. 

### OGDMTT priorities and work plan
The OGDMTT will renew its membership and chair by the end of the year through a dedicated call (OCt 2023 - Dec 2023).
Priorities for the OGDMTT for the end of the year are:
* Communication around OG1.0,
* Communication around BUFR
* Review of exiting procedure around Delayed mode quality control,
* Call for new members, new chairs, new ToR, new work plan.

The work plan of the OGDMTT for the next years is currently being discussed here: [https://docs.google.com/document/d/1I5w8OyhP7SsdIyWFmjDlJOE8cCWBQN6TC2iYPf6Bdb8/edit?usp=sharing](https://docs.google.com/document/d/1I5w8OyhP7SsdIyWFmjDlJOE8cCWBQN6TC2iYPf6Bdb8/edit?usp=sharing)

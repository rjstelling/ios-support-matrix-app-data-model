#Support Matrix for iOS Data Models

> An evolving set of JSON files that describe all the features and capabilities of iOS devices.

##1. Introduction

This repository is a collaborative effort aiming to codify all the characteristics of iOS devices so they can eaisly be consumed by infomation systems and applications.

##2. Repository Layout

    /
    /README.md						(this file)
	/ios-device-example-format.json	(an example file, this is most likely temporary)
	/devices						(directory containing a JSON file per device)
    	/iphone.json
		/iphone_3g.json
	/bin							(tools for manipulating the data)
	

##3. Device File Format

###3.1 Root Container

Each file contains at its root one JSON dictionary. In the future tools will be provided to output a sinfle JSON file containing, at its root a JSON array of these dictionaries.  

###3.2 Fields

Field names are of the format: `words_seperated_by_underscores`.

####3.2.1 `device_id`
**Type:** STRING

**Values:** *TODO*

####3.2.2 `device_title`
**Type:** STRING

**Values:** *TODO*

####3.2.3 `device_model_strings`
**Type:** ARRAY

**Values:** *TODO*

####3.2.4 `device_model_ids`
**Type:** ARRAY

**Values:** *TODO*

####3.2.5 `storage`
**Type:** ARRAY

**Values:** *TODO*

####3.2.6 `ram`
**Type:** NUMBER

**Values:** *TODO*

####3.2.7 `colours`
**Type:** ARRAY

**Values:** *TODO*

####3.2.8 `processor_name`
**Type:** STRING

**Values:** *TODO*

####3.2.9 `architecture`
**Type:** STRING

**Values:** *TODO*

####3.2.10 `device_launch_date`
**Type:** DATE

**Values:** *TODO*

####3.2.11 `device_discontinued_date`
**Type:** DATE

**Values:** *TODO*

####3.2.12 `os_versions`
**Type:** ARRAY

An array of dictionaries containing the following fields:

#####3.2.12.1 `version_name`
**Type:** STRING

**Values:** *TODO*

#####3.2.12.2 `version`
**Type:** NUMBER

**Values:** *TODO*

#####3.2.12.3 `build`
**Type:** STRING

**Values:** *TODO*

#####3.2.12.4 `baseband`
**Type:** STRING

**Values:** *TODO*

#####3.2.12.5 `release_date`
**Type:** DATE

**Values:** *TODO*

#####3.2.12.6 `support_level`
**Type:** NUMBER

**Values:** *TODO*
 
####3.2.13 `geekbench_v2_score`
**Type:** NUMBER

**Values:** *TODO*

####3.2.14 `geekbench_v3_single_core`
**Type:** NUMBER | null

**Values:** *TODO*

####3.2.15 `geekbench_v3_multi_core`
**Type:** NUMBER | null

**Values:** *TODO*

**Notes:** Can be `null` if no data is available.

####3.2.16 `capabilities`
**Type:** ARRAY

An array of dictionaries containing the following fields:

#####3.2.16.1 `capability`
**Type:** STRING

**Values:** *TODO*

#####3.2.16.2 `value`
**Type:** STRING | NUMBER | ARRAY

**Values:** *TODO*
 
####3.2.17 `notes`
**Type:** STRING

**Values:** *TODO*

####3.2.18 `last_updated`
**Type:** STRING

**Values:** *TODO*
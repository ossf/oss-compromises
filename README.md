# Open Source Software Compromises Dataset

This is an attempt to create a comprehensive dataset of open source software compromises. The intention is to help parties that want prevent and mitigate open source software compromises.

All contributions are welcome. Initial effort will focus only on collecting data related to open source software compromises that happen after October 1, 2022. This is an experimental effort. TODO: Elaborate

## Inclusion Criteria, or What is an Open Source Software Compromise?

Compromises ought to be included in this dataset if both conditions (1) and (2) are met. “Compromise” implies that an attack has actually occurred.

Condition 1: The compromise arises from a vulnerability, introduced unintentionally or maliciously, in the open source software supply chain.

Condition 2: The compromise has a high impact. “High impact” means either “many” parties affected, especially parties associated with “critical infrastructure,” and/or the compromise results in “severe damage.”

Alternatively, vulnerabilities without an associated compromise ought to be included if the potential impact is vast and there is a high likelihood of undetected compromises, e.g. Heartbleed.


## Who Is Responsible for Maintaining This Dataset?

This is a volunteer effort. There exist a set of maintainers that have personally volunteered their effort in the past to maintain separate, related datasets, and it’s therefore likely that this same group will also continue to devote time to maintaining this dataset. Others are welcome to contribute too. But it is a strictly volunteer effort.

## What is the Recommended Timeline for Announcing Compromises?

This dataset is meant to capture only publicly reported compromises. So there must be publicly available information about the compromise. It is not intended to be a source of zero-days or otherwise undisclosed vulnerabilities.

## How Do I Submit a Compromise?

Make a PR and place a new YAML file into the compromises folder. Each compromise is associated with one YAML file. This project uses a specific structure, described below, for data collection purposes. Fields marked optional are optional. For an example YAML file, see the 'dydx-compromise.yaml' file in the `compromises` folder.


Note on naming the file: Use `id-name` where is 

TODO: Use a table here

compromise-id

NOTE: Use the next highest number, locating the current number by examining the comrpomi


| Field                           | Required      | Description    |
| -------------                   | ------------- | -------------  |
| compromise-name                 |               |  Content Cell  |
| description                     |               |  Content Cell  |
| compromise-classification       |               |  Content Cell  |
| cwe                             |               |  Content Cell  |
| mitre-attack                    |               |  Content Cell  |
| ecosystem                       |               |  Content Cell  |
| earliest-evidence-of-compromise |               |  Content Cell  |
| date-entry-was-created          |               |  Content Cell  |
| date-entry-was-last-updated     |               |  Content Cell  |
| references                      |               |  Content Cell  |
| malicious-intent                |               |  Content Cell  |
| packages-affected               |               |  Content Cell  |
| IOCs                            |               |  Content Cell  |




compromise-name:
description:
compromise-classification:
Note - Use attack class labels from this attack tree (https://arxiv.org/abs/2204.04008), creating a separate label for each of the relevant nodes that apply to the attack, to the best of existing knowledge.
cwe: (optional) https://cwe.mitre.org/
mitre-attack: (optional) https://attack.mitre.org 
ecosystem:
earliest-evidence-of-compromise: YYmm or YYmmdd
date-entry-was-created:
date-entry-was-last-updated:
references:
malicious-intent:
packages-affected: [ foo, bar, … ]
IOCs: (optional) [rule1, rule2]
  --rule-name
  --rule-type
  --rule-specification

# Adversary Engagement Ontology #

[Adversary Engagement (AE)](https://aeontology.sail-lab.org/) ontology is an extension of the [Unified Cyber Ontology (UCO)](https://unifiedcyberontology.org/) with the goal of defining and standardizing information representation in cyber adversary engagement operations and interactions. [Adversary engagement](https://engage.mitre.org/) is the strategic use of denial and deception tactics aimed at increasing the cost and decreasing the value of an adversary's cyber operations. The goals of adversary engagement can include detecting adversaries on a network, eliciting intelligence about them, or affecting them by raising the cost and lowering the value of their cyber operations.

The AE ontology aims to standardize and simplify the documentation and transmission of the deployment configuration of cyber adversary engagement tools and techniques. This helps to ensure a consistent and efficient approach to adversary engagement across organizations and domains. The standardization provided by the AE ontology enables better collaboration and sharing of information among stakeholders, leading to more effective utilization of adversary engagement operations.

AEO Website: http://www.adversaryengagementontology.org/

## Use cases ##
The Adversary Engagement Ontology (AEO) serves several purposes:

- It provides a systematic approach for the development, representation, and management of concepts and categories within the domain of cyber adversary engagement.

- It fosters a shared understanding of concepts and their relationships in Adversary Engagement, which can be utilized for communication, reasoning, and decision-making in forensic analysis.

- Scholars, researchers, and academicians can utilize AEO to define AE concepts, establish relationships between them, and organize them into a structured framework.

- Practitioners and vendors can leverage AEO to configure deployments and set up the necessary tools for risk mitigation.

![alt text](https://github.com/UNHSAILLab/AdvEng/blob/main/ae_diagram.png?raw=true)

## Objectives ##

1. The Adversary Engagement (AE) ontology aims to establish a sub-ontology within the Unified Cyber Ontology (UCO) that incorporates and expands upon the foundational concepts found in MITRE's open-source ENGAGE and ATT&CK knowledge models. The ultimate goal is to advance the field of cyber adversary engagement by exploring new avenues, including the interactions between smart agents and the implementation of decoy and obfuscated data.
2. The AE ontology endeavors to bring together a diverse and inclusive community of stakeholders, comprising members from academia, government, non-profit, and for-profit organizations, to actively participate in the development, implementation, and sustained support of the Adversary Engagement (AE) ontology.


## Scope ##
The Adversary Engagement (AE) ontology focuses on the subject matter pertaining to engaging with adversaries. Drawing upon concepts from the Unified Cyber Ontology (UCO), MITRE ATT&CK, and MITRE ENGAGE, the AEO selectively incorporates relevant ideas and categories. Additionally, there exist several concepts that overlap with the Cyber Threat Intelligence (CTI) ontology and other domains within cybersecurity. The AEO strives to encompass only those concepts that are directly related to adversary engagement and does not aim to be all-inclusive.


## Approach ##

The Adversary Engagement (AE) ontology is defined as a specific domain ontology within the Linux Foundation Cyber Domain Ontology project and conforms to the Unified Cyber Ontology ecosystem. AEO is a systematic method for the development, representation, and management of concepts and categories in a specific an adversary engagement knowledge model. This involves defining concepts, creating relationships between them, and organizing them into a structured framework. The goal of an AEO is to provide a shared understanding of the concepts and their relationships in a adversary engagement, which can be used for communication, reasoning, and decision-making tasks. 

- - - - 

# Overview #

## Examples ##
There are three examples inside the `\examples\` folder.
- [Breadcrumb](https://github.com/UNHSAILLab/Adversary-Engagement-Ontology/tree/main/examples/Breadcrumb)
- [Fluid Deception](https://github.com/UNHSAILLab/Adversary-Engagement-Ontology/tree/main/examples/Fluid%20Deception)
- [Honeypot](https://github.com/UNHSAILLab/Adversary-Engagement-Ontology/tree/main/examples/Honeypot)

## Classes Tree ##
 ```
  ├── engagement:Event
  ├── uco-action:Action
  │    ├── engagement:Access
  │    ├── engagement:Alert
  │    ├── engagement:Deploy
  │    ├── engagement:Respond
  │    ├── engagement:Obfuscate
  │    ├── engagement:Beacon
  ├── uco-action:ActionLifecycle
  │    ├── attack:cyberKillChain
  ├── uco-action:ActionPattern
  │    ├── attack:AttackPattern
  │    ├── attack:DefensePattern
  ├── uco-core:UcoObject
  │    ├── engagement:DataSource
  │    ├── engagement:DataTarget
  │    ├── engagement:LureObject
  │    │     ├── engagement:Breadcrumb
  │    │     ├── engagement:Decoy
  │    │     ├── engagement:HoneyObject
  │    │         ├── engagement:HoneyToken
  │    │         ├── engagement:Honeypot
  │    ├── engagement:BreadcrumbTrail
  │    ├── engagement:Malware
  │    ├── engagement:Narrative
  │    ├── engagement:PlannedEvent
  │    ├── engagement:PocketLitter
  │    ├── engagement:Resource
  │    ├── engagement:Sandbox
  │    ├── engagement:Storyline
  │    ├── objective:Objective
  ├── uco-identity:Identity
  │    ├── identiy:Persona
  │    ├── uco-identity:Organization
  │    │     ├── identity:Team
```


## Individuals ##
```
├── engagement:Objective
│    ├── objective:Affect
│    ├── objective:Collect
│    ├── objective:CommandAndControl
│    ├── objective:CredentialAccess
│    ├── objective:Deny
│    ├── objective:Detect
│    ├── objective:DevelopResource
│    ├── objective:Direct
│    ├── objective:Discover
│    ├── objective:Disrupt
│    ├── objective:Elicit
│    ├── objective:Evade
│    ├── objective:Execute
│    ├── objective:Exfilitrate
│    ├── objective:Expose
│    ├── objective:Impact
│    ├── objective:GainInitialAccess
│    ├── objective:MoveLaterally
│    ├── objective:Motivate
│    ├── objective:Persist
│    ├── objective:Prevent
│    ├── objective:PrivilegeEscalate
│    ├── objective:Reassure
│    ├── objective:Reconnaissance
│    ├── objective:TimeSink
│    ├── objective:Track
│    ├── objective:Trap
│    ├── objective:Plan
│    ├── objective:Prepare
│    ├── objective:Lure
│    ├── objective:Analyze
├── engagement:Role
│    ├── role:RedTeam
│    ├── role:BlueTeam
│    ├── role:PurpleTeam
│    ├── role:Adversary
│    ├── role:Defender

```

## Properties Tree ##
```
├── engagement:alertContext
├── engagement:eventContext
├── engagement:hasCharacterization
├── engagement:hasEvent
├── engagement:hasStoryline
├── engagement:honeypotInteractionType
├── engagement:eventAttribute
├── engagement:eventType
├── engagement:hasBreadcrumb
├── objective:hasObjective
├── objective:hasAttackSurface
├── engagement:breadcrumbTargetObject
├── engagement:hasCharacterization
├── engagement:hasPerceptionCharacterization
```

## Current Release ##
The current release of AEO is version 0.2.0 

The latest release of the Adversary Engagement Ontology (AEO), version 0.2.0, has incorporated necessary refinements and updates. In accordance with Semantic Versioning principles, the AEO will continue to accept additive improvements, but any backwards-incompatible changes will be deferred until the next release, which is planned to occur within a minimum period of 6 months and a maximum period of 12 months.

## I have a question!

Before you post a Github issue or send an email ensure you've done this checklist:

1. [Determined scope](https://aeontology.sail-lab.org/start.php#scope) of your task. It is not necessary for most parties to understand all aspects of the ontology, mapping methods, and supporting tools.

2. Search the [Issues tab](https://github.com/UNHSAILLab/Adversary-Engagement-Ontology/issues) for duplicative issues.  Please know, however, that the AEO community primarily tracks issues in a Jira instance available to community members.  The Github Issue tracker can still be a way AEO issues are reported by users who have not registered with the community, but work on the issues will be scheduled and tracked in Jira.

## NOTICE
This software was produced for the U.S. Government under contract FA8702-22-C-0001,
and is subject to the Rights in Data-General Clause 52.227-14, Alt. IV (DEC 2007)
C2023 The MITRE Corporation. All Rights Reserved.
Released under MITRE PRS 18-4297, and under the Cyber Domain Ontology project's Apache 2 license.

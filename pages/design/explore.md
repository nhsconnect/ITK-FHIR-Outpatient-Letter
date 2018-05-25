---
title: Messaging Architecture Overview
keywords:  messaging
tags: [fhir,messaging]
sidebar: foundations_sidebar
permalink: explore.html
summary: "Overview of the Messaging Architecture section"
---

{% include custom/search.warnbanner.html %}
{% include custom/messaging_overview.svg %}

## Overview ##

This section gives details of the document profiles and associated transport and work-flow. 

## Pre-Requisites for FHIR ITK3 Messaging Solutions ##

## ITK3 Messaging Requirements ##

- SHALL support HL7 FHIR version STU3
- When using ITK3 and MESH SHALL implement ITK3 Sender and/or Receiver Responsibilities as per [ITK3 Sender and Receiver Requirements](..\explore_snd&rec_req.html)
- Resources sent SHALL identify the CareConnect Profile where a CareConnect Profile is included in the bundle using the [FHIR Base Resource](https://hl7.org/fhir/resource-definitions.html#Resource.meta)
- SHALL support XML format for all NHS Digital ITK3 interactions.


## FHIR Conformance ##

- SHOULD declare a Conformance identifying the list of profiles and message bundles supported.







# RADAR-Repository-Review

This file provides a quick review of the purpose of each major repository in the RADAR-CNS project
Each link and definition is defined using the first paragraph description in the top of each repository, described in the [Style Guide](RADAR-Style-Guide.md)

## Repositories
<https://github.com/RADAR-CNS/RADAR-Android-Application-Status>
Plugin that sends application statuses about the RADAR pRMT app.

<https://github.com/RADAR-CNS/RADAR-Android-Audio>
Audio plugin for the RADAR passive remote monitoring app. It uses openSMILE to process audio from
the phone's microphone, extracts features from it, and sends those features.

<https://github.com/RADAR-CNS/RADAR-Android-Biovotion>
Biovotion VSM plugin for the RADAR-AndroidApplication app, to be run on an Android 4.4 (or later) device with Bluetooth Low Energy (Bluetooth 4.0 or later), to interact with Biovotion VSM devices.

<https://github.com/RADAR-CNS/RADAR-Android-Empatica>	
Application to be run on an Android 4.4 (or later) device with Bluetooth Low Energy (Bluetooth 4.0 or later), to interact with the Empatica.

<https://github.com/RADAR-CNS/RADAR-Android-Pebble>
Pebble plugin for the RADAR-AndroidApplication app, to be run on an Android 4.4 (or later) device with Bluetooth Low Energy (Bluetooth 4.0 or later), to interact with wearable devices.

<https://github.com/RADAR-CNS/RADAR-Android-Phone>	
Application to be run on an Android 4.4 (or later) device. This collects data from the Phone light sensor, battery status and acceleration.

<https://github.com/RADAR-CNS/RADAR-AndroidApplication>	
Application to be run on an Android 4.4 (or later) device with Bluetooth Low Energy (Bluetooth 4.0 or later), to interact with wearable devices. The app is cloned from the [Empatica sample app][2].

<https://github.com/RADAR-CNS/RADAR-Backend>	
Based on Confluent Platform to standardise, analyse and persistent data collected by RADAR-CNS data sources. Data is consumed and produced in Apache Avro format using the schemas stored inside the RADAR-CNS [schema repository](https://github.com/<https://github.com/RADAR-CNS/RADAR-CNS/RADAR-Schemas).

<https://github.com/RADAR-CNS/RADAR-Commons>
Common utilities library containing basic schemas, streaming features, testing bridges and utils.

<https://github.com/RADAR-CNS/RADAR-Commons-Android>
Base module for the RADAR passive remote monitoring app. Plugins for that app should implement the API from this base library.

<https://github.com/RADAR-CNS/RADAR-Cordova-OpenSmile-Plugin>
Plugin that create a csv file and store the output of opensmile tool for audio recordings.

<https://github.com/RADAR-CNS/RADAR-Dashboard>
An [Angular](https://angular.io/) and [D3](https://d3js.org/) web application to manage and monitor research data from the [RADAR-CNS Platform](http://RADAR-cns.org/).

<https://github.com/RADAR-CNS/RADAR-Design>	
UI/UX Design Documents for the RADAR-CNS Project

<https://github.com/RADAR-CNS/RADAR-Docker>	
The dockerized RADAR stack or deploying the RADAR-CNS platform.

<https://github.com/RADAR-CNS/RADAR-Gateway>	
No documentation

<https://github.com/RADAR-CNS/RADAR-HDFS-Sink-Connector>	
Contains HDFS-Sink-Connector of RADAR-CNS platform

<https://github.com/RADAR-CNS/RADAR-Identity>	
Code for accessing WSO2IS

<https://github.com/RADAR-CNS/RADAR-MongoDB-Sink-Connector>	
Implements the hot-storage support for RADAR-CNS platform using MongoDBSinkConnector

<https://github.com/RADAR-CNS/RADAR-Questionnaire>	
Hybrid mobile application to actively capture data for the RADAR-CNS Platform.

<https://github.com/RADAR-CNS/RADAR-RestApi>	
This project implents the downstream REST API for the RADAR-CNS project

<https://github.com/RADAR-CNS/RADAR-Schemas>	
Avro schemas used in RADAR-CNS. The schemas are divided into three parts: `commons` for the passive remote monitoring application and the backend, `restapi` for the REST API, and `questionnaire` for the active remote monitoring application.

<https://github.com/RADAR-CNS/RADAR-Security>	
Authentication, Authorisation, De-Identification and Encryption for the RADAR platform and data management

<https://github.com/RADAR-CNS/RADAR-Security-Annotation>	
"Base plugin for security for RADAR APIs. This plugin provides the `@Secured(String[] rolesAllowed, String[] scopesAllowed)` annotation. There is no actual implementation in this plugin.""

<https://github.com/RADAR-CNS/RADAR-Security-Annotation-WSO2IS>	
WSO2IS maven plugin for security for RADAR APIs. This plugin provides an authentication and authorization filter implementation for [<https://github.com/RADAR-CNS/RADAR-Security-Base](https://github.com/RADAR-CNS/RADAR-Security-Base) plugin. It is sufficient to include this plugin only, you don't need to include the base plugin as well.

<https://github.com/RADAR-CNS/Restructure-HDFS-topic/>	
Data streamed to HDFS using the [RADAR HDFS sink connector](https://github.com/RADAR-CNS/RADAR-HDFS-Sink-Connector) is streamed to files based on sensor only. This package can transform that output to a local directory structure as follows: `userId/topic/date_hour.csv`. The date and hour is extracted from the `time` field of each record, and is formatted in UTC time.

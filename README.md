# ![LOGO](logo.png) PatientView **flow**ground Connector

## Description

A generated **flow**ground connector for the PatientView API (version 1.0).

Generated from: https://api.apis.guru/v2/specs/patientview.org/1.0/swagger.json<br/>
Generated at: 2019-05-07T17:43:37+03:00

## API Description

The recommended REST API endpoints to be used when integrating with PatientView

## Authorization

This API does not require authorization.

## Actions

### Log In

> Authenticate using username and password, returns token, which must be added to X-Auth-Token in header of all future requests

*Tags:* `auth-controller`

### Log Out

*Tags:* `auth-controller`

#### Input Parameters
* `token` - _required_ - token

### Get Basic User Information

> Once logged in and have a token, get basic user information including group role membership

*Tags:* `auth-controller`

#### Input Parameters
* `token` - _required_ - token

### Get Basic Patient Information

> Given a User ID, get basic patient information for a user from clinical data stored in FHIR

*Tags:* `patient-controller`

#### Input Parameters
* `userId` - _required_ - userId

### getPatientManagementDiagnoses

*Tags:* `patient-management-controller`

### getPatientManagementLookupTypes

*Tags:* `patient-management-controller`

### validatePatientManagement

*Tags:* `patient-management-controller`

### getPatientManagement

*Tags:* `patient-management-controller`

#### Input Parameters
* `userId` - _required_ - userId
* `groupId` - _required_ - groupId
* `identifierId` - _required_ - identifierId

### savePatientManagement

*Tags:* `patient-management-controller`

#### Input Parameters
* `userId` - _required_ - userId
* `groupId` - _required_ - groupId
* `identifierId` - _required_ - identifierId

### savePatientManagementSurgeries

*Tags:* `patient-management-controller`

#### Input Parameters
* `userId` - _required_ - userId
* `groupId` - _required_ - groupId
* `identifierId` - _required_ - identifierId

### Get Available Observations Types For a User

> Given a User ID retrieve a list of available observation types for that user (where they have observation data).

*Tags:* `observation-heading-controller`

#### Input Parameters
* `userId` - _required_ - userId

### Get Observations of Multiple Types For a User

> Given a User ID and search parameters, retrieve a page of observations.

*Tags:* `observation-controller`

#### Input Parameters
* `userId` - _required_ - userId
* `code` - _required_ - code
* `limit` - _required_ - limit
* `offset` - _required_ - offset
* `orderDirection` - _required_ - orderDirection

### Get Observations of a Certain Type For a User

> Given a User ID and observation code, retrieve all observations.

*Tags:* `observation-controller`

#### Input Parameters
* `userId` - _required_ - userId
* `code` - _required_ - code

### Get patient entered Observations of a Certain Type For a User

> Given a User ID and observation code, retrieve patient entered observations.

*Tags:* `observation-controller`

#### Input Parameters
* `userId` - _required_ - userId
* `code` - _required_ - code

### Get Available Patient Entered Observations Types For a User

> Given a User ID retrieve a list of available observation types for that user (where they have patient entered observation data).

*Tags:* `observation-heading-controller`

#### Input Parameters
* `userId` - _required_ - userId

## License

**flow**ground :- Telekom iPaaS / patientview-org-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.

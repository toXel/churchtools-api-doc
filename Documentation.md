# ChurchTools API Documentation

[TOC]

## Basics
All data is returned in the JSON format.

## Main

#### login
##### Usage
`http://churchtools.server/?q=login`

Parameters are sent via HTTP POST:
- email: admin@example.com
- password: admin
- directtool: yes (needed for API login)

## ChurchDB
Functions for managing the people of your church.
### Usage
`http://churchtools.server/?q=churchdb/ajax&func=<functionName>&<parameters>`

### Get functions

#### getMasterData
Get an array with all relevant master data for JS-View.

#### getAllPersonData
Returns all persons in the ChurchDB
##### Parameters
- (optional) p_id: ID of a person

#### getAllPersonArchiveData
Returns all archived persons

#### getAllRels
Returns all relations (partner, parents, kids, ...) for all persons

#### getPersonDetails
Recives all data for a person
##### Parameters
- id: ID of a person

#### getPersonDetailsLogs
Returns log entries regarding person details for a person
##### Parameters
- id: ID of a person

#### getSearchableData
Returns person data to search for

#### getPersonByName
Search for persons by name
##### Parameters
- searchpattern: Part of the name you're searching for
- withmydeps:

#### getPersonById
Search for persons by ID
##### Parameters
- id: person ID

#### getGroupAutomaticEMail

#### getImportTables

#### getTableContent
Returns the content of a given table name
##### Parameters
- table: Name of the table

#### getMasterDataTableNames


#### mailchimp
Function for sending mails with mailchimp.com

#### sendsms
Function for sending SMS

#### pollForNews

#### f_geocode_person
#### f_geocode_gruppe
#### createAddress
#### createGroup
#### deleteLastGroupStatistic
#### deleteGroup
#### f_image
#### f_bereich
#### f_note
#### add_rel
#### del_rel
#### GroupMeeting
#### moveMeetingDataFromGroupPerson
#### addEvent
#### del_note
#### setCMSUser
#### send_email
#### deletePerson
#### archivePerson
#### undoArchivePerson
#### delPersonTag
#### delGroupTag
#### addNewTag
#### addPersonTag
#### addGroupTag
#### addPersonDistrictRelation
#### delPersonDistrictRelation
#### addPersonGruppentypRelation
#### delPersonGruppentypRelation
#### delPersonGroupRelation
#### editPersonGroupRelation
#### addPersonGroupRelation
#### sendInvitationMail
#### setPersonPassword
#### sendEMailToPersonIds
#### loadAuthData
#### deactivatePerson
#### activatePerson
#### saveGroupAutomaticEMail
#### addPersonAuth
#### saveDomainAuth

## ChurchCal

#### getMasterData
#### getAllowedPeopleForCalendar
#### getEvent
#### getEventChangeImpact
#### saveSplittedEvent
#### createEvent
#### updateEvent
#### deleteEvent
#### saveReminder

## ChurchReport

#### getMasterDataTablenames
#### getMasterData
#### loadQuery

## ChurchResource

#### getBookings
#### getMasterDataTablenames
#### getMasterData
#### saveSplittedBooking
#### saveSplittedEvent
#### createEvent
#### updateEvent
#### deleteEvent

## ChurchService

#### getMasterDataTablenames
#### getMasterData
#### updateEvent
#### createEvent
#### deleteEvent
#### getEventChangeImpact
#### saveSplittedEvent
#### getEventTemplates
#### updateEventService
#### getAbsent
#### getGroupAndTagInfos
#### addOrRemoveServiceToEvent
#### sendEMailToPersonIds
#### saveTemplate
#### deleteTemplate
#### delFile
#### renameFile
#### copyFile
#### getFiles
#### getAllSongs
#### getSongStatistics
#### addNewSong
#### editSong
#### delSong
#### editArrangement
#### addArrangement
#### delArrangement
#### deleteSong
#### makeAsStandardArrangement
#### saveAbsent
#### delAbsent
#### saveNote
#### getServiceGroupPersonWeight
#### editServiceGroupPersonWeight
#### getChurchDBMasterData
#### loadAllAgendaTemplates
#### loadAgendas
#### loadAgendaForEvent
#### loadAgendaItems
#### saveItem
#### saveAgenda
#### loadItem
#### saveServiceGroupNote
#### deleteItemEventRelation
#### addItemEventRelation
#### deleteItem
#### deleteAgenda

## ChurchWiki

#### getMasterDataTablenames
#### getMasterData
#### save
#### load
#### loadHistory
#### showonstartpage
#### delFile
#### renameFile

# Comparison of Opencast integrations into LMS

## Disclaimer

This feature comparison is a high-level overview of Opencast integrations into multiple LMS and other portals. It is meant as an overview for existing Opencast adopters and deciders who are thinking about adopting Opencast to their institution.

Please note that while this document tries hard to compare the features across the different LMS, it is still often comparing apples with pears as technical details and integration depth might vary.

## Feature overview

### Video management features

| Feature                                            | Moodle                 | ILIAS              | Stud.IP    | Tobira | Olat | Blackboard | Canvas |
| -------------------------------------------------- | ---------------------- | ------------------ | ---------- | ------ | ---- | ---------- | ------ |
| Upload videos<br>[Details](#user-content-upload)                | ✓                      | ✓                  | ✓          |        |      |            |        |
| ➞ By teachers                                      | ✓                      | ✓                  | ✓          |        |      |            |        |
| ➞ By students                                      | Only with role changes |                    |            |        |      |            |        |
| Scheduling<br>[Details](#user-content-sched)                    | ✗                      | ✓                  | ✓          |        |      |            |        |
| ➞ Of own lectures / in own lecture halls           | ✗                      |                    |            |        |      |            |        |
| ➞ At arbitrary times / in arbitrary lecture halls  | ✗                      |                    |            |        |      |            |        |
| Metadata<br>[Details](#user-content-meta)                       | ✓                      | ✓                  | ✓          |        |      |            |        |
| Subtitles<br>[Details](#user-content-subtit)                    | ✓                      | ✓                  | ✓          |        |      |            |        |
| Editor<br>[Details](#user-content-editor)                       | ✓                      | ✓                  | ✓          |        |      |            |        |
| Playlists<br>[Details](#user-content-playlist)                  | ✗                      | ✗                  | ✓          |        |      |            |        |
| Bulk actions<br>[Details](#user-content-bulk)                   | ✓                      | ✗                  | ✓          |        |      |            |        |
| Tags<br>[Details](#user-content-tags)                           | ✗                      | ✗                  | ✓          |        |      |            |        |
| Linksharing / Direct access<br>[Details](#user-content-sharing) | ✓                      |                    | ✓          |        |      |            |        |
| Batch upload<br>[Details](#user-content-batch)                  | ✓                      | ✗                  | ✗          |        |      |            |        |
| Backup and Im- / export of Opencast stuff in LMS courses<br>[Details](#user-content-backup-im-export)     | ✓                      | ✗                  | ✓ (Partly) |        |      |            |        |
| Start a custom workflow<br>[Details](#user-content-custwf)      | ✓                      | ✓                  | ✗          |        |      |            |        |

### Video playback features

| Feature                                | Moodle                | ILIAS | Stud.IP | Tobira | Olat | Blackboard | Canvas |
| -------------------------------------- | --------------------- | ----- | ------- | ------ | ---- | ---------- | ------ |
| Paella player<br>[Details](#user-content-player)    | ✓                     | ✓     | ✓       |        |      |            |        |
| ➞ Version                              | 7                     | 7     | 7       |        |      |            |        |
| ➞ Delivery via LTI                     | ✓ (for some features) | ✗     | ✓       |        |      |            |        |
| ➞ Delivery from within LMS             | ✓ (for some features) | ✓     | ✗       |        |      |            |        |
| ➞ Paella Plugins                       | ✓ (Only via LTI)      |       | ✓       |        |      |            |        |
| Video download<br>[Details](#user-content-download) | ✓                     | ✓     | ✓       |        |      |            |        |

### Additional integrations

| Feature                                           | Moodle | ILIAS | Stud.IP | Tobira | Olat | Blackboard | Canvas |
| ------------------------------------------------- | ------ | ----- | ------- | ------ | ---- | ---------- | ------ |
| Annotation tool integration<br>[Details](#user-content-annot)  | ✗      | ✓     | ✓       |        |      |            |        |
| Opencast Studio integration<br>[Details](#user-content-studio) | ✓      | ✓     | ✓       |        |      |            |        |
| ➞ Via LTI<br>[Details](#user-content-studio)                   | ✓      | ✗     | ✓       |        |      |            |        |
| ➞ Via Shibboleth<br>[Details](#user-content-studio)            | ✗      | ✓     | ✗       |        |      |            |        |
| ➞ ACL Over Studio<br>[Details](#user-content-acl-over-studio)  | ✗      | ✓     | ✗       |        |      |            |        |
| Tobira integration<br>[Details](#user-content-tobira)          | ✗      | ✓     | ✗       |        |      |            |        |

### Technical features

| Feature                                                | Moodle    | ILIAS                            | Stud.IP                   | Tobira | Olat | Blackboard | Canvas |
| ------------------------------------------------------ | --------- | -------------------------------- | ------------------------- | ------ | ---- | ---------- | ------ |
| Opencast PHP library<br>[Details](#user-content-phplib)             | ✓         | ✓                                | ✓                         |        |      |            |        |
| Opencast feature discovering<br>[Details](#user-content-discover)   | By config | By config in ILIAS (publication) | By config & by "guessing" |        |      |            |        |
| List provider for languages<br>[Details](#user-content-listlang)    | ✗         | ✓                                | ✗                         |        |      |            |        |
| List provider for licences<br>[Details](#user-content-listlic)      | ✗         | ✓                                | ✗                         |        |      |            |        |
| Authentication<br>[Details](#user-content-auth)                     | ✓         | ✓                                | ✓                         |        |      |            |        |
| ➞ External API                                         | ✓         | ✓                                | ✗                         |        |      |            |        |
| ➞ LTI                                                  | ✓         | ✗                                | ✓                         |        |      |            |        |
| ➞ JWT                                                  | ✗         | ✗ (Wished)                       | ✗ (Planned)               |        |      |            |        |
| Permission handling<br>[Details](#user-content-perms)               | ✓         | ✓                                | ✓                         |        |      |            |        |
| ➞ ACL<br>[Details](#user-content-perms)                             | ✓         | ✗                                | ✓                         |        |      |            |        |
| ➞ LTI<br>[Details](#user-content-perms)                             | ✓         | ✗                                | ✓                         |        |      |            |        |
| ➞ User Provider<br>[Details](#user-content-perms)                   | ✓         | ✗                                | ✓                         |        |      |            |        |
| ➞ Shibboleth<br>[Details](#user-content-perms)                      | ✗         | ✓                                | ✗                         |        |      |            |        |
| Enforcing permissions (against known IDs)              | ✓         | ✗                                | ✓                         |        |      |            |        |
| Multi tenancy support<br>[Details](#user-content-tenants)           | ✓         | ✗                                | ✓                         |        |      |            |        |
| Tracking protection circumvention<br>[Details](#user-content-track) | ✗         | ✗ (Not needed)                   | ✓                         |        |      |            |        |
| Maintenance Support<br>[Details](#user-content-maintenance-support) | ✓         | ✗                  | ✗          |        |      |            |        |

## Feature details

### <a name="user-content-upload"></a>Upload videos

In the LMS, it is possible to upload videos which will thereafter be stored and processed in Opencast.

### <a name="user-content-sched"></a>Scheduling

In the LMS, it is possible to see, set and update the scheduling of recordings on capture agents which are configured in Opencast.

### <a name="user-content-meta"></a>Metadata

In the LMS, it is possible to set and update the metadata of videos. This is done during the video upload as well as after the processing of the video.
[See details in the Opencast documentation](https://docs.opencast.org/r/16.x/admin/#configuration/metadata/)

### <a name="user-content-subtit"></a>Subtitles

In the LMS, it is possible to set and update subtitles for existing videos to be used in the player.
[See details in the Opencast documentation](https://docs.opencast.org/r/16.x/admin/#configuration/subtitles/)

### <a name="user-content-editor"></a>Editor

In the LMS, it is possible to edit existing videos (in terms of trimming / cutting) which will thereafter be re-processed and re-published in Opencast.
[See details in the Opencast documentation](https://docs.opencast.org/r/16.x/admin/#configuration/videoeditor.overview/)
[See a demo installation of the Opencast editor](https://editor.opencast.org/)

### <a name="user-content-playlist"></a>Playlists

The LMS is able to create playlists as well as to consume and manage existing playlists in Opencast.
[See details in the Opencast documentation](https://docs.opencast.org/r/16.x/admin/#configuration/playlists/)

### <a name="user-content-bulk"></a>Bulk actions

In the LMS, it is possible to apply the same operation (for example unpublish or delete) to a set of videos at once instead of having to apply the operation to each video individually.

### <a name="user-content-batch"></a>Batch upload

In the LMS, it is possible to upload multiple videos at once for processing instead of having to upload each video individually.

### <a name="user-content-tags"></a>Tags

TBD

### <a name="user-content-sharing"></a>Linksharing / Direct access

In the LMS, it is possible to set the permissions of an existing video in a way that it is publicly accessible. Additionally, a direct access URL is generated with can be handed over to non-LMS users for watching the video.

### <a name="user-content-backup-im-export"></a>Backup and Im- / export of Opencast stuff in LMS courses 

The LMS is able to backup, import and export Opencast Series/Videos from one course to another either by event duplication or ACL Change method.

### <a name="user-content-custwf"></a>Start a custom workflow

In the LMS, in addition to standard video processing actions (like deleting, unpublishing, editing), it is possible to start an arbitrary custom Opencast workflow which does arbitrary things. The necessary parameters to run the Opencast workflow are requested from the user in the LMS before starting the workflow.
[See details in the Opencast documentation](https://docs.opencast.org/r/16.x/admin/#configuration/workflow/)

### <a name="user-content-player"></a>Paella player

In the LMS, videos are played with the Paella Player (which is the standard player in Opencast). There may be differences in the Paella Player version, the way of delivery to the user's browser and the support for Paella plugins.

[See details in the Opencast documentation](https://docs.opencast.org/r/16.x/admin/#configuration/player/paella.player7/configuration/)
[See details on the Paella Player project website](https://paellaplayer.upv.es/)

### <a name="user-content-download"></a>Video download

In the LMS, it is possible to download existing videos to the user's computer.

TBD: Clarify if the download is located in the Integration plugin or in the Paella player, which videos can be downloaded (the original or the processed video) and which LMS roles (student, teacher) can use the download.

### <a name="user-content-annot"></a>Annotation tool integration

From the LMS, it is possible to process an existing video in the Opencast annotation tool.
[See details in the Annotation tool repository](https://github.com/opencast/annotation-tool)

### <a name="user-content-studio"></a>Opencast Studio integration

From the LMS, it is possible to record a video in Opencast Studio, process it directly in Opencast and add it to the LMS in the end.
[See details in the Opencast documentation](https://docs.opencast.org/r/16.x/admin/#configuration/studio/)
[See a demo installation of Opencast Studio](https://studio.opencast.org/)

#### <a name="user-content-acl-over-studio"></a>ACL Over Studio

The LMS is able pass user ACLs via the link to Opencast Studio using the query string.

### <a name="user-content-tobira"></a>Tobira integration

From the LMS, it is possible to publish a video in Tobira.
[See details in the Tobira repository](https://github.com/elan-ev/tobira/)
[See a demo installation of Tobira](https://tobira.opencast.org/)

### <a name="user-content-phplib"></a>Opencast PHP library

The communication between the LMS and Opencast is built on the Opencast PHP library by ELAN e.V. instead of custom LMS code.
[See details in the Opencast PHP library repository](https://github.com/elan-ev/opencast-php-library)

### <a name="user-content-discover"></a>Opencast feature discovering

The LMS will discover the resources and assets associated with an event to extract specific desired values, such as links or metadata. For example, in ILIAS, there is a mechanism to automatically retrieve a video link from event publications in an efficient and structured manner. Administrators can configure the player publication settings by specifying details such as the channel ID, media type, MIME type, and other parameters. This configuration instructs the plugin to extract the desired link from the event's publications.

### <a name="user-content-listlang"></a>List provider for languages

The LMS is able to retrieve the languages which are configured in Opencast instead of urging the LMS admin to configure them locally.

### <a name="user-content-listlic"></a>List provider for licences

The LMS is able to retrieve the licences which are configured in Opencast instead of urging the LMS admin to configure them locally.

### <a name="user-content-user-content-auth"></a>Authentication

The LMS must authenticate against Opencast. This can be achieved with multiple technologies.

### <a name="user-content-perms"></a>Permission handling

The LMS and Opencast should share a common understanding which videos should be accessed by which user and which user has which role. This can be achieved with multiple technologies.

### Enforcing permissions (against known IDs)

TBD

### <a name="user-content-tenants"></a>Multi tenancy support

The LMS is able to communicate with multiple Opencast instances or with multiple tenants of the same Opencast installation. All features of the integration must respect multi-tenancy.

### <a name="user-content-track"></a>Tracking protection circumvention

TBD

### <a name="user-content-maintenance-support"></a>Maintenance Support

The LMS is able to fetch the maintenance data from Opencast and syncronize its maintenance period with Opencast.

## Status of this document

This document is currently work-in-progress. The following main points need to be addressed before considering it as final:

- Double-check the feature list for Moodle
- Double-check the feature list for ILIAS
- Double-check the feature list for Stud.IP
- Add features for Tobira
- Add features for Olat
- Add features for Blackboard
- Add features for Canvas
- Complete the feature descriptions
- Amend the feature descriptions with links to the Opencast documentation where possible
- Amend the feature descriptions with links to the particular LMS integration documentation where possible
- (optional) Add a feature comparison for the integration of competitor systems like Panopto or Kaltura into the LMS

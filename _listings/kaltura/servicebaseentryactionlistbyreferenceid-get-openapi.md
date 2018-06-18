---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Baseentry Action Listbyreferenceid
  description: List base entries by filter according to reference id
  version: 3.3.0
host: www.kaltura.com
basePath: /api_v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /service/baseentry/action/add:
    get:
      summary: Get Service Baseentry Action Add
      description: Generic add entry, should be used when the uploaded entry type
        is not known.
      operationId: baseEntry.add
      x-api-path-slug: servicebaseentryactionadd-get
      parameters:
      - in: query
        name: entry[accessControlId]
        description: The Access Control ID assigned to this entry (null when not set,
          send -1 to remove)
      - in: query
        name: entry[adminTags]
        description: Entry admin tags can be updated only by administrators
      - in: query
        name: entry[bitrates]
      - in: query
        name: entry[categoriesIds]
        description: Comma separated list of ids of categories to which this entry
          belongs
      - in: query
        name: entry[categories]
        description: Comma separated list of full names of categories to which this
          entry belongs
      - in: query
        name: entry[conversionProfileId]
        description: Override the default ingestion profile
      - in: query
        name: entry[conversionQuality]
        description: '`insertOnly`Override the default conversion quality'
      - in: query
        name: entry[creatorId]
        description: '`insertOnly`The ID of the user who created this entry'
      - in: query
        name: entry[creditUrl]
        description: The URL for credits
      - in: query
        name: entry[creditUserName]
        description: The user name used for credits
      - in: query
        name: entry[currentBroadcastStartTime]
        description: The time (unix timestamp in milliseconds) in which the entry
          broadcast started or 0 when the entry is off the air
      - in: query
        name: entry[dataContent]
        description: The data of the entry
      - in: query
        name: entry[description]
        description: Entry description
      - in: query
        name: entry[displayInSearch]
        description: 'Enum Type: `KalturaEntryDisplayInSearchType`should we display
          this entry in search'
      - in: query
        name: entry[documentType]
        description: '`insertOnly`Enum Type: `KalturaDocumentType`The type of the
          document'
      - in: query
        name: entry[dvrStatus]
        description: 'Enum Type: `KalturaDVRStatus`DVR Status Enabled/Disabled'
      - in: query
        name: entry[dvrWindow]
        description: Window of time which the DVR allows for backwards scrubbing (in
          minutes)
      - in: query
        name: entry[editorType]
        description: 'Enum Type: `KalturaEditorType`The editor type used to edit the
          metadata'
      - in: query
        name: entry[encodingIP1]
        description: The broadcast primary ip
      - in: query
        name: entry[encodingIP2]
        description: The broadcast secondary ip
      - in: query
        name: entry[endDate]
        description: Entry scheduling end date (null when not set, send -1 to remove)
      - in: query
        name: entry[entitledUsersEdit]
        description: list of user ids that are entitled to edit the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: entry[entitledUsersPublish]
        description: list of user ids that are entitled to publish the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: entry[externalSourceType]
        description: '`insertOnly`Enum Type: `KalturaExternalMediaSourceType`The source
          type of the external media'
      - in: query
        name: entry[filters]
      - in: query
        name: entry[groupId]
      - in: query
        name: entry[hlsStreamUrl]
        description: HLS URL - URL for live stream playback on mobile device
      - in: query
        name: entry[lastElapsedRecordingTime]
        description: Elapsed recording time (in msec) up to the point where the live
          stream was last stopped (unpublished)
      - in: query
        name: entry[licenseType]
        description: 'Enum Type: `KalturaLicenseType`License type used for this entry'
      - in: query
        name: entry[liveStreamConfigurations]
      - in: query
        name: entry[mediaType]
        description: '`insertOnly`Enum Type: `KalturaMediaType`The media type of the
          entry'
      - in: query
        name: entry[msDuration]
        description: The duration in miliseconds
      - in: query
        name: entry[name]
        description: Entry name (Min 1 chars)
      - in: query
        name: entry[objectType]
      - in: query
        name: entry[offlineMessage]
        description: The message to be presented when the stream is offline
      - in: query
        name: entry[operationAttributes]
      - in: query
        name: entry[parentEntryId]
        description: ID of source root entry, used for defining entires association
      - in: query
        name: entry[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: entry[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: entry[playlistContent]
        description: Content of the playlist - XML if the playlistType is dynamic
          text if the playlistType is static url if the playlistType is mRss
      - in: query
        name: entry[playlistId]
        description: Playlist id to be played
      - in: query
        name: entry[playlistType]
        description: 'Enum Type: `KalturaPlaylistType`Type of playlist'
      - in: query
        name: entry[primaryBroadcastingUrl]
      - in: query
        name: entry[primaryRtspBroadcastingUrl]
      - in: query
        name: entry[publishConfigurations]
      - in: query
        name: entry[pushPublishEnabled]
        description: 'Enum Type: `KalturaLivePublishStatus`Flag denoting whether entry
          should be published by the media server'
      - in: query
        name: entry[recordedEntryId]
        description: Recorded entry id
      - in: query
        name: entry[recordingOptions][shouldCopyEntitlement]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldCopyScheduling]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldCopyThumbnail]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldMakeHidden]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordStatus]
        description: 'Enum Type: `KalturaRecordStatus`Recording Status Enabled/Disabled'
      - in: query
        name: entry[redirectEntryId]
        description: IF not empty, points to an entry ID the should replace this current
          entrys id
      - in: query
        name: entry[referenceId]
        description: Entry external reference id
      - in: query
        name: entry[repeat]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that the segments
          should be repeated for ever'
      - in: query
        name: entry[retrieveDataContentByGet]
        description: '`insertOnly`indicator whether to return the object for get action
          with the dataContent field'
      - in: query
        name: entry[searchProviderId]
        description: '`insertOnly`The ID of the media in the importing site'
      - in: query
        name: entry[searchProviderType]
        description: '`insertOnly`Enum Type: `KalturaSearchProviderType`The search
          provider type used to import this entry'
      - in: query
        name: entry[secondaryBroadcastingUrl]
      - in: query
        name: entry[secondaryRtspBroadcastingUrl]
      - in: query
        name: entry[sourceType]
        description: '`insertOnly`Enum Type: `KalturaSourceType`The source type of
          the entry'
      - in: query
        name: entry[startDate]
        description: Entry scheduling start date (null when not set, send -1 to remove)
      - in: query
        name: entry[streamName]
      - in: query
        name: entry[streamPassword]
        description: The broadcast password
      - in: query
        name: entry[streams]
      - in: query
        name: entry[streamUrl]
        description: The stream url
      - in: query
        name: entry[tags]
        description: Entry tags
      - in: query
        name: entry[templateEntryId]
        description: '`insertOnly`Template entry id'
      - in: query
        name: entry[totalResults]
        description: Maximum count of results to be returned in playlist execution
      - in: query
        name: entry[type]
        description: 'Enum Type: `KalturaEntryType`The type of the entry, this is
          auto filled by the derived entry object'
      - in: query
        name: entry[urlManager]
        description: URL Manager to handle the live stream URL (for instance, add
          token)
      - in: query
        name: entry[userId]
        description: The ID of the user who is the owner of this entry
      - in: query
        name: No Name
      - in: query
        name: type
        description: 'Enum Type: `KalturaEntryType`'
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Add
  /service/baseentry/action/addContent:
    post:
      summary: Post Service Baseentry Action Addcontent
      description: Attach content resource to entry in status NO_MEDIA
      operationId: baseEntry.addContent
      x-api-path-slug: servicebaseentryactionaddcontent-post
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      - in: query
        name: resource[assetId]
        description: ID of the source asset
      - in: query
        name: resource[content]
        description: Textual content
      - in: query
        name: resource[dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[entryId]
        description: ID of the source entry
      - in: formData
        name: resource[fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[objectType]
      - in: query
        name: resource[privateKey]
        description: SSH private key
      - in: query
        name: resource[publicKey]
        description: SSH public key
      - in: query
        name: resource[resources]
      - in: query
        name: resource[resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][content]
        description: Textual content
      - in: query
        name: resource[resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][objectType]
      - in: query
        name: resource[resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resources]
      - in: query
        name: resource[resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][resource][content]
        description: Textual content
      - in: query
        name: resource[resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][resource][objectType]
      - in: query
        name: resource[resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resource][resources]
      - in: query
        name: resource[resource][resource][resource][assetId]
        description: ID of the source asset
      - in: query
        name: resource[resource][resource][resource][content]
        description: Textual content
      - in: query
        name: resource[resource][resource][resource][dropFolderFileId]
        description: Id of the drop folder file object
      - in: query
        name: resource[resource][resource][resource][entryId]
        description: ID of the source entry
      - in: formData
        name: resource[resource][resource][resource][fileData]
        description: Represents the $_FILE
      - in: query
        name: resource[resource][resource][resource][fileSyncObjectType]
        description: The object type of the file sync object
      - in: query
        name: resource[resource][resource][resource][flavorParamsId]
        description: ID of the source flavor params, set to null to use the source
          flavor
      - in: query
        name: resource[resource][resource][resource][forceAsyncDownload]
        description: Force Import Job
      - in: query
        name: resource[resource][resource][resource][keepOriginalFile]
        description: Should keep original file (false = mv, true = cp)
      - in: query
        name: resource[resource][resource][resource][keyPassphrase]
        description: Passphrase for SSH keys
      - in: query
        name: resource[resource][resource][resource][localFilePath]
        description: Full path to the local file
      - in: query
        name: resource[resource][resource][resource][objectId]
        description: The object id of the file sync object
      - in: query
        name: resource[resource][resource][resource][objectSubType]
        description: The object sub-type of the file sync object
      - in: query
        name: resource[resource][resource][resource][objectType]
      - in: query
        name: resource[resource][resource][resource][privateKey]
        description: SSH private key
      - in: query
        name: resource[resource][resource][resource][publicKey]
        description: SSH public key
      - in: query
        name: resource[resource][resource][resource][resources]
      - in: query
        name: resource[resource][resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[resource][resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[resource][storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[resource][token]
        description: Token that returned from upload
      - in: query
        name: resource[resource][url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[resource][version]
        description: The version of the file sync object
      - in: query
        name: resource[storageProfileId]
        description: ID of storage profile to be associated with the created file
          sync, used for file serving URL composing
      - in: query
        name: resource[token]
        description: Token that returned from upload
      - in: query
        name: resource[url]
        description: Remote URL, FTP, HTTP or HTTPS
      - in: query
        name: resource[version]
        description: The version of the file sync object
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - AddContent
  /service/baseentry/action/addFromUploadedFile:
    get:
      summary: Get Service Baseentry Action Addfromuploadedfile
      description: Generic add entry using an uploaded file, should be used when the
        uploaded entry type is not known.
      operationId: baseEntry.addFromUploadedFile
      x-api-path-slug: servicebaseentryactionaddfromuploadedfile-get
      parameters:
      - in: query
        name: entry[accessControlId]
        description: The Access Control ID assigned to this entry (null when not set,
          send -1 to remove)
      - in: query
        name: entry[adminTags]
        description: Entry admin tags can be updated only by administrators
      - in: query
        name: entry[bitrates]
      - in: query
        name: entry[categoriesIds]
        description: Comma separated list of ids of categories to which this entry
          belongs
      - in: query
        name: entry[categories]
        description: Comma separated list of full names of categories to which this
          entry belongs
      - in: query
        name: entry[conversionProfileId]
        description: Override the default ingestion profile
      - in: query
        name: entry[conversionQuality]
        description: '`insertOnly`Override the default conversion quality'
      - in: query
        name: entry[creatorId]
        description: '`insertOnly`The ID of the user who created this entry'
      - in: query
        name: entry[creditUrl]
        description: The URL for credits
      - in: query
        name: entry[creditUserName]
        description: The user name used for credits
      - in: query
        name: entry[currentBroadcastStartTime]
        description: The time (unix timestamp in milliseconds) in which the entry
          broadcast started or 0 when the entry is off the air
      - in: query
        name: entry[dataContent]
        description: The data of the entry
      - in: query
        name: entry[description]
        description: Entry description
      - in: query
        name: entry[displayInSearch]
        description: 'Enum Type: `KalturaEntryDisplayInSearchType`should we display
          this entry in search'
      - in: query
        name: entry[documentType]
        description: '`insertOnly`Enum Type: `KalturaDocumentType`The type of the
          document'
      - in: query
        name: entry[dvrStatus]
        description: 'Enum Type: `KalturaDVRStatus`DVR Status Enabled/Disabled'
      - in: query
        name: entry[dvrWindow]
        description: Window of time which the DVR allows for backwards scrubbing (in
          minutes)
      - in: query
        name: entry[editorType]
        description: 'Enum Type: `KalturaEditorType`The editor type used to edit the
          metadata'
      - in: query
        name: entry[encodingIP1]
        description: The broadcast primary ip
      - in: query
        name: entry[encodingIP2]
        description: The broadcast secondary ip
      - in: query
        name: entry[endDate]
        description: Entry scheduling end date (null when not set, send -1 to remove)
      - in: query
        name: entry[entitledUsersEdit]
        description: list of user ids that are entitled to edit the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: entry[entitledUsersPublish]
        description: list of user ids that are entitled to publish the entry (no server
          enforcement) The difference between entitledUsersEdit and entitledUsersPublish
          is applicative only
      - in: query
        name: entry[externalSourceType]
        description: '`insertOnly`Enum Type: `KalturaExternalMediaSourceType`The source
          type of the external media'
      - in: query
        name: entry[filters]
      - in: query
        name: entry[groupId]
      - in: query
        name: entry[hlsStreamUrl]
        description: HLS URL - URL for live stream playback on mobile device
      - in: query
        name: entry[lastElapsedRecordingTime]
        description: Elapsed recording time (in msec) up to the point where the live
          stream was last stopped (unpublished)
      - in: query
        name: entry[licenseType]
        description: 'Enum Type: `KalturaLicenseType`License type used for this entry'
      - in: query
        name: entry[liveStreamConfigurations]
      - in: query
        name: entry[mediaType]
        description: '`insertOnly`Enum Type: `KalturaMediaType`The media type of the
          entry'
      - in: query
        name: entry[msDuration]
        description: The duration in miliseconds
      - in: query
        name: entry[name]
        description: Entry name (Min 1 chars)
      - in: query
        name: entry[objectType]
      - in: query
        name: entry[offlineMessage]
        description: The message to be presented when the stream is offline
      - in: query
        name: entry[operationAttributes]
      - in: query
        name: entry[parentEntryId]
        description: ID of source root entry, used for defining entires association
      - in: query
        name: entry[partnerData]
        description: Can be used to store various partner related data as a string
      - in: query
        name: entry[partnerSortValue]
        description: Can be used to store various partner related data as a numeric
          value
      - in: query
        name: entry[playlistContent]
        description: Content of the playlist - XML if the playlistType is dynamic
          text if the playlistType is static url if the playlistType is mRss
      - in: query
        name: entry[playlistId]
        description: Playlist id to be played
      - in: query
        name: entry[playlistType]
        description: 'Enum Type: `KalturaPlaylistType`Type of playlist'
      - in: query
        name: entry[primaryBroadcastingUrl]
      - in: query
        name: entry[primaryRtspBroadcastingUrl]
      - in: query
        name: entry[publishConfigurations]
      - in: query
        name: entry[pushPublishEnabled]
        description: 'Enum Type: `KalturaLivePublishStatus`Flag denoting whether entry
          should be published by the media server'
      - in: query
        name: entry[recordedEntryId]
        description: Recorded entry id
      - in: query
        name: entry[recordingOptions][shouldCopyEntitlement]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldCopyScheduling]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldCopyThumbnail]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordingOptions][shouldMakeHidden]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: entry[recordStatus]
        description: 'Enum Type: `KalturaRecordStatus`Recording Status Enabled/Disabled'
      - in: query
        name: entry[redirectEntryId]
        description: IF not empty, points to an entry ID the should replace this current
          entrys id
      - in: query
        name: entry[referenceId]
        description: Entry external reference id
      - in: query
        name: entry[repeat]
        description: 'Enum Type: `KalturaNullableBoolean`Indicates that the segments
          should be repeated for ever'
      - in: query
        name: entry[retrieveDataContentByGet]
        description: '`insertOnly`indicator whether to return the object for get action
          with the dataContent field'
      - in: query
        name: entry[searchProviderId]
        description: '`insertOnly`The ID of the media in the importing site'
      - in: query
        name: entry[searchProviderType]
        description: '`insertOnly`Enum Type: `KalturaSearchProviderType`The search
          provider type used to import this entry'
      - in: query
        name: entry[secondaryBroadcastingUrl]
      - in: query
        name: entry[secondaryRtspBroadcastingUrl]
      - in: query
        name: entry[sourceType]
        description: '`insertOnly`Enum Type: `KalturaSourceType`The source type of
          the entry'
      - in: query
        name: entry[startDate]
        description: Entry scheduling start date (null when not set, send -1 to remove)
      - in: query
        name: entry[streamName]
      - in: query
        name: entry[streamPassword]
        description: The broadcast password
      - in: query
        name: entry[streams]
      - in: query
        name: entry[streamUrl]
        description: The stream url
      - in: query
        name: entry[tags]
        description: Entry tags
      - in: query
        name: entry[templateEntryId]
        description: '`insertOnly`Template entry id'
      - in: query
        name: entry[totalResults]
        description: Maximum count of results to be returned in playlist execution
      - in: query
        name: entry[type]
        description: 'Enum Type: `KalturaEntryType`The type of the entry, this is
          auto filled by the derived entry object'
      - in: query
        name: entry[urlManager]
        description: URL Manager to handle the live stream URL (for instance, add
          token)
      - in: query
        name: entry[userId]
        description: The ID of the user who is the owner of this entry
      - in: query
        name: No Name
      - in: query
        name: type
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: uploadTokenId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - AddFromUploadedFile
  /service/baseentry/action/anonymousRank:
    get:
      summary: Get Service Baseentry Action Anonymousrank
      description: Anonymously rank an entry, no validation is done on duplicate rankings.
      operationId: baseEntry.anonymousRank
      x-api-path-slug: servicebaseentryactionanonymousrank-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      - in: query
        name: rank
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - AnonymousRank
  /service/baseentry/action/approve:
    get:
      summary: Get Service Baseentry Action Approve
      description: Approve the entry and mark the pending flags (if any) as moderated
        (this will make the entry playable).
      operationId: baseEntry.approve
      x-api-path-slug: servicebaseentryactionapprove-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Approve
  /service/baseentry/action/clone:
    get:
      summary: Get Service Baseentry Action Clone
      description: Clone an entry with optional attributes to apply to the clone
      operationId: baseEntry.clone
      x-api-path-slug: servicebaseentryactionclone-get
      parameters:
      - in: query
        name: entryId
        description: Id of entry to clone
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Clone
  /service/baseentry/action/count:
    get:
      summary: Get Service Baseentry Action Count
      description: Count base entries by filter.
      operationId: baseEntry.count
      x-api-path-slug: servicebaseentryactioncount-get
      parameters:
      - in: query
        name: filter[accessControlIdEqual]
      - in: query
        name: filter[accessControlIdIn]
      - in: query
        name: filter[adminTagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[adminTagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[adminTagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[assetParamsIdsMatchAnd]
      - in: query
        name: filter[assetParamsIdsMatchOr]
      - in: query
        name: filter[categoriesFullNameIn]
      - in: query
        name: filter[categoriesIdsEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[categoriesIdsMatchAnd]
      - in: query
        name: filter[categoriesIdsMatchOr]
        description: All entries of the categories, excluding their child categories
      - in: query
        name: filter[categoriesIdsNotContains]
      - in: query
        name: filter[categoriesMatchAnd]
      - in: query
        name: filter[categoriesMatchOr]
        description: All entries within these categories or their child categories
      - in: query
        name: filter[categoriesNotContains]
      - in: query
        name: filter[categoryAncestorIdIn]
        description: All entries within this categoy or in child categories
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system after a specific time/date (standard
          timestamp format)
      - in: query
        name: filter[createdAtLessThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system before a specific time/date (standard
          timestamp format)
      - in: query
        name: filter[creatorIdEqual]
      - in: query
        name: filter[documentTypeEqual]
        description: 'Enum Type: `KalturaDocumentType`'
      - in: query
        name: filter[documentTypeIn]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationGreaterThan]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[durationLessThan]
      - in: query
        name: filter[durationTypeMatchOr]
      - in: query
        name: filter[endDateGreaterThanOrEqualOrNull]
      - in: query
        name: filter[endDateGreaterThanOrEqual]
      - in: query
        name: filter[endDateLessThanOrEqualOrNull]
      - in: query
        name: filter[endDateLessThanOrEqual]
      - in: query
        name: filter[entitledUsersEditMatchAnd]
      - in: query
        name: filter[entitledUsersEditMatchOr]
      - in: query
        name: filter[entitledUsersPublishMatchAnd]
      - in: query
        name: filter[entitledUsersPublishMatchOr]
      - in: query
        name: filter[externalSourceTypeEqual]
        description: 'Enum Type: `KalturaExternalMediaSourceType`'
      - in: query
        name: filter[externalSourceTypeIn]
      - in: query
        name: filter[flavorParamsIdsMatchAnd]
      - in: query
        name: filter[flavorParamsIdsMatchOr]
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[groupIdEqual]
      - in: query
        name: filter[hasMediaServerHostname]
      - in: query
        name: filter[idEqual]
        description: This filter should be in use for retrieving only a specific entry
          (identified by its entryId)
      - in: query
        name: filter[idIn]
        description: This filter should be in use for retrieving few specific entries
          (string should include comma separated list of entryId strings)
      - in: query
        name: filter[idNotIn]
      - in: query
        name: filter[isLive]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isRecordedEntryIdEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isRoot]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[lastPlayedAtGreaterThanOrEqual]
      - in: query
        name: filter[lastPlayedAtLessThanOrEqual]
      - in: query
        name: filter[limit]
      - in: query
        name: filter[mediaDateGreaterThanOrEqual]
      - in: query
        name: filter[mediaDateLessThanOrEqual]
      - in: query
        name: filter[mediaTypeEqual]
        description: 'Enum Type: `KalturaMediaType`'
      - in: query
        name: filter[mediaTypeIn]
      - in: query
        name: filter[moderationStatusEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: filter[moderationStatusIn]
      - in: query
        name: filter[moderationStatusNotEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: filter[moderationStatusNotIn]
      - in: query
        name: filter[nameEqual]
        description: This filter should be in use for retrieving entries with a specific
          name
      - in: query
        name: filter[nameLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[nameMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[nameMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentEntryIdEqual]
      - in: query
        name: filter[partnerIdEqual]
        description: This filter should be in use for retrieving only entries which
          were uploaded by/assigned to users of a specific Kaltura Partner (identified
          by Partner ID)
      - in: query
        name: filter[partnerIdIn]
        description: This filter should be in use for retrieving only entries within
          Kaltura network which were uploaded by/assigned to users of few Kaltura
          Partners  (string should include comma separated list of PartnerIDs)
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[redirectFromEntryId]
        description: The id of the original entry
      - in: query
        name: filter[referenceIdEqual]
      - in: query
        name: filter[referenceIdIn]
      - in: query
        name: filter[replacedEntryIdEqual]
      - in: query
        name: filter[replacedEntryIdIn]
      - in: query
        name: filter[replacementStatusEqual]
        description: 'Enum Type: `KalturaEntryReplacementStatus`'
      - in: query
        name: filter[replacementStatusIn]
      - in: query
        name: filter[replacingEntryIdEqual]
      - in: query
        name: filter[replacingEntryIdIn]
      - in: query
        name: filter[rootEntryIdEqual]
      - in: query
        name: filter[rootEntryIdIn]
      - in: query
        name: filter[searchTextMatchAnd]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within all of the following metadata
          attributes: name, description, tags, adminTags'
      - in: query
        name: filter[searchTextMatchOr]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within at least one of the following
          metadata attributes: name, description, tags, adminTags'
      - in: query
        name: filter[sourceTypeEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: filter[sourceTypeIn]
      - in: query
        name: filter[sourceTypeNotEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: filter[sourceTypeNotIn]
      - in: query
        name: filter[startDateGreaterThanOrEqualOrNull]
      - in: query
        name: filter[startDateGreaterThanOrEqual]
      - in: query
        name: filter[startDateLessThanOrEqualOrNull]
      - in: query
        name: filter[startDateLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, at a specific {'
      - in: query
        name: filter[statusIn]
        description: This filter should be in use for retrieving only entries, at
          few specific {
      - in: query
        name: filter[statusNotEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, not at a specific {'
      - in: query
        name: filter[statusNotIn]
        description: This filter should be in use for retrieving only entries, not
          at few specific {
      - in: query
        name: filter[tagsAdminTagsMultiLikeAnd]
      - in: query
        name: filter[tagsAdminTagsMultiLikeOr]
      - in: query
        name: filter[tagsAdminTagsNameMultiLikeAnd]
      - in: query
        name: filter[tagsAdminTagsNameMultiLikeOr]
      - in: query
        name: filter[tagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsNameMultiLikeAnd]
      - in: query
        name: filter[tagsNameMultiLikeOr]
      - in: query
        name: filter[totalRankGreaterThanOrEqual]
      - in: query
        name: filter[totalRankLessThanOrEqual]
      - in: query
        name: filter[typeEqual]
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: filter[typeIn]
        description: This filter should be in use for retrieving entries of few {
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdEqual]
        description: This filter parameter should be in use for retrieving only entries,
          uploaded by/assigned to a specific user (identified by user Id)
      - in: query
        name: filter[userIdIn]
      - in: query
        name: filter[userIdNotIn]
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Count
  /service/baseentry/action/delete:
    get:
      summary: Get Service Baseentry Action Delete
      description: Delete an entry.
      operationId: baseEntry.delete
      x-api-path-slug: servicebaseentryactiondelete-get
      parameters:
      - in: query
        name: entryId
        description: Entry id to delete
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Delete
  /service/baseentry/action/export:
    get:
      summary: Get Service Baseentry Action Export
      description: ""
      operationId: baseEntry.export
      x-api-path-slug: servicebaseentryactionexport-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      - in: query
        name: storageProfileId
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Export
  /service/baseentry/action/flag:
    get:
      summary: Get Service Baseentry Action Flag
      description: Flag inappropriate entry for moderation.
      operationId: baseEntry.flag
      x-api-path-slug: servicebaseentryactionflag-get
      parameters:
      - in: query
        name: moderationFlag[comments]
        description: The comment that was added to the flag
      - in: query
        name: moderationFlag[flaggedEntryId]
        description: If moderation flag is set for entry, this is the flagged entry
          id
      - in: query
        name: moderationFlag[flaggedUserId]
        description: If moderation flag is set for user, this is the flagged user
          id
      - in: query
        name: moderationFlag[flagType]
        description: 'Enum Type: `KalturaModerationFlagType`'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Flag
  /service/baseentry/action/get:
    get:
      summary: Get Service Baseentry Action Get
      description: Get base entry by ID.
      operationId: baseEntry.get
      x-api-path-slug: servicebaseentryactionget-get
      parameters:
      - in: query
        name: entryId
        description: Entry id
      - in: query
        name: No Name
      - in: query
        name: version
        description: Desired version of the data
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Get
  /service/baseentry/action/getByIds:
    get:
      summary: Get Service Baseentry Action Getbyids
      description: Get an array of KalturaBaseEntry objects by a comma-separated list
        of ids.
      operationId: baseEntry.getByIds
      x-api-path-slug: servicebaseentryactiongetbyids-get
      parameters:
      - in: query
        name: entryIds
        description: Comma separated string of entry ids
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - GetByIds
  /service/baseentry/action/getContextData:
    get:
      summary: Get Service Baseentry Action Getcontextdata
      description: 'This action delivers entry-related data, based on the user''s
        context: access control, restriction, playback format and storage information.'
      operationId: baseEntry.getContextData
      x-api-path-slug: servicebaseentryactiongetcontextdata-get
      parameters:
      - in: query
        name: contextDataParams[contexts]
      - in: query
        name: contextDataParams[flavorAssetId]
        description: Id of the current flavor
      - in: query
        name: contextDataParams[flavorTags]
        description: The tags of the flavors that should be used for playback
      - in: query
        name: contextDataParams[hashes]
      - in: query
        name: contextDataParams[ip]
        description: IP to be used to test geographic location conditions
      - in: query
        name: contextDataParams[ks]
        description: Kaltura session to be used to test session and user conditions
      - in: query
        name: contextDataParams[mediaProtocol]
        description: Protocol of the specific media object
      - in: query
        name: contextDataParams[objectType]
      - in: query
        name: contextDataParams[referrer]
        description: URL to be used to test domain conditions
      - in: query
        name: contextDataParams[streamerType]
        description: 'Playback streamer type: RTMP, HTTP, appleHttps, rtsp, sl'
      - in: query
        name: contextDataParams[time]
        description: Unix timestamp (In seconds) to be used to test entry scheduling,
          keep null to use now
      - in: query
        name: contextDataParams[userAgent]
        description: Browser or client application to be used to test agent conditions
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - GetContextData
  /service/baseentry/action/getPlaybackContext:
    get:
      summary: Get Service Baseentry Action Getplaybackcontext
      description: This action delivers all data relevant for player
      operationId: baseEntry.getPlaybackContext
      x-api-path-slug: servicebaseentryactiongetplaybackcontext-get
      parameters:
      - in: query
        name: contextDataParams[contexts]
      - in: query
        name: contextDataParams[flavorAssetId]
        description: Id of the current flavor
      - in: query
        name: contextDataParams[flavorTags]
        description: The tags of the flavors that should be used for playback
      - in: query
        name: contextDataParams[hashes]
      - in: query
        name: contextDataParams[ip]
        description: IP to be used to test geographic location conditions
      - in: query
        name: contextDataParams[ks]
        description: Kaltura session to be used to test session and user conditions
      - in: query
        name: contextDataParams[mediaProtocol]
        description: Protocol of the specific media object
      - in: query
        name: contextDataParams[referrer]
        description: URL to be used to test domain conditions
      - in: query
        name: contextDataParams[streamerType]
        description: 'Playback streamer type: RTMP, HTTP, appleHttps, rtsp, sl'
      - in: query
        name: contextDataParams[time]
        description: Unix timestamp (In seconds) to be used to test entry scheduling,
          keep null to use now
      - in: query
        name: contextDataParams[userAgent]
        description: Browser or client application to be used to test agent conditions
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - GetPlaybackContext
  /service/baseentry/action/getRemotePaths:
    get:
      summary: Get Service Baseentry Action Getremotepaths
      description: Get remote storage existing paths for the asset.
      operationId: baseEntry.getRemotePaths
      x-api-path-slug: servicebaseentryactiongetremotepaths-get
      parameters:
      - in: query
        name: entryId
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - GetRemotePaths
  /service/baseentry/action/index:
    get:
      summary: Get Service Baseentry Action Index
      description: Index an entry by id.
      operationId: baseEntry.index
      x-api-path-slug: servicebaseentryactionindex-get
      parameters:
      - in: query
        name: id
      - in: query
        name: No Name
      - in: query
        name: shouldUpdate
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - Index
  /service/baseentry/action/list:
    get:
      summary: Get Service Baseentry Action List
      description: List base entries by filter with paging support.
      operationId: baseEntry.list
      x-api-path-slug: servicebaseentryactionlist-get
      parameters:
      - in: query
        name: filter[accessControlIdEqual]
      - in: query
        name: filter[accessControlIdIn]
      - in: query
        name: filter[adminTagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[adminTagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[adminTagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[advancedSearch][attribute]
        description: 'Enum Type: `KalturaBaseEntryCompareAttribute`'
      - in: query
        name: filter[advancedSearch][categoriesMatchOr]
      - in: query
        name: filter[advancedSearch][categoryEntryStatusIn]
      - in: query
        name: filter[advancedSearch][categoryIdEqual]
      - in: query
        name: filter[advancedSearch][comparison]
        description: 'Enum Type: `KalturaSearchConditionComparison`'
      - in: query
        name: filter[advancedSearch][contentLike]
      - in: query
        name: filter[advancedSearch][contentMultiLikeAnd]
      - in: query
        name: filter[advancedSearch][contentMultiLikeOr]
      - in: query
        name: filter[advancedSearch][cuePointsFreeText]
      - in: query
        name: filter[advancedSearch][cuePointSubTypeEqual]
      - in: query
        name: filter[advancedSearch][cuePointTypeIn]
      - in: query
        name: filter[advancedSearch][depthGreaterThanEqual]
      - in: query
        name: filter[advancedSearch][distributionProfileId]
      - in: query
        name: filter[advancedSearch][distributionSunStatus]
        description: 'Enum Type: `KalturaEntryDistributionSunStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionFlag]
        description: 'Enum Type: `KalturaEntryDistributionFlag`'
      - in: query
        name: filter[advancedSearch][entryDistributionStatus]
        description: 'Enum Type: `KalturaEntryDistributionStatus`'
      - in: query
        name: filter[advancedSearch][entryDistributionValidationErrors]
        description: Comma seperated validation error types
      - in: query
        name: filter[advancedSearch][extendedStatusEqual]
        description: 'Enum Type: `KalturaUserEntryExtendedStatus`'
      - in: query
        name: filter[advancedSearch][extendedStatusIn]
      - in: query
        name: filter[advancedSearch][field]
      - in: query
        name: filter[advancedSearch][hasEntryDistributionValidationErrors]
      - in: query
        name: filter[advancedSearch][idEqual]
      - in: query
        name: filter[advancedSearch][idIn]
      - in: query
        name: filter[advancedSearch][indexIdGreaterThan]
      - in: query
        name: filter[advancedSearch][isQuiz]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[advancedSearch][items]
      - in: query
        name: filter[advancedSearch][memberIdEq]
      - in: query
        name: filter[advancedSearch][memberIdIn]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchAnd]
      - in: query
        name: filter[advancedSearch][memberPermissionsMatchOr]
      - in: query
        name: filter[advancedSearch][metadataProfileId]
      - in: query
        name: filter[advancedSearch][noDistributionProfiles]
      - in: query
        name: filter[advancedSearch][not]
      - in: query
        name: filter[advancedSearch][objectType]
      - in: query
        name: filter[advancedSearch][orderBy]
        description: 'Enum Type: `KalturaCategoryEntryAdvancedOrderBy`'
      - in: query
        name: filter[advancedSearch][type]
        description: 'Enum Type: `KalturaSearchOperatorType`'
      - in: query
        name: filter[advancedSearch][updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[advancedSearch][updatedAtLessThanOrEqual]
      - in: query
        name: filter[advancedSearch][userIdEqual]
      - in: query
        name: filter[advancedSearch][userIdIn]
      - in: query
        name: filter[advancedSearch][value]
      - in: query
        name: filter[advancedSearch][watermarkId]
      - in: query
        name: filter[assetParamsIdsMatchAnd]
      - in: query
        name: filter[assetParamsIdsMatchOr]
      - in: query
        name: filter[categoriesFullNameIn]
      - in: query
        name: filter[categoriesIdsEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[categoriesIdsMatchAnd]
      - in: query
        name: filter[categoriesIdsMatchOr]
        description: All entries of the categories, excluding their child categories
      - in: query
        name: filter[categoriesIdsNotContains]
      - in: query
        name: filter[categoriesMatchAnd]
      - in: query
        name: filter[categoriesMatchOr]
        description: All entries within these categories or their child categories
      - in: query
        name: filter[categoriesNotContains]
      - in: query
        name: filter[categoryAncestorIdIn]
        description: All entries within this categoy or in child categories
      - in: query
        name: filter[createdAtGreaterThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system after a specific time/date (standard
          timestamp format)
      - in: query
        name: filter[createdAtLessThanOrEqual]
        description: This filter parameter should be in use for retrieving only entries
          which were created at Kaltura system before a specific time/date (standard
          timestamp format)
      - in: query
        name: filter[creatorIdEqual]
      - in: query
        name: filter[documentTypeEqual]
        description: 'Enum Type: `KalturaDocumentType`'
      - in: query
        name: filter[documentTypeIn]
      - in: query
        name: filter[durationGreaterThanOrEqual]
      - in: query
        name: filter[durationGreaterThan]
      - in: query
        name: filter[durationLessThanOrEqual]
      - in: query
        name: filter[durationLessThan]
      - in: query
        name: filter[durationTypeMatchOr]
      - in: query
        name: filter[endDateGreaterThanOrEqualOrNull]
      - in: query
        name: filter[endDateGreaterThanOrEqual]
      - in: query
        name: filter[endDateLessThanOrEqualOrNull]
      - in: query
        name: filter[endDateLessThanOrEqual]
      - in: query
        name: filter[entitledUsersEditMatchAnd]
      - in: query
        name: filter[entitledUsersEditMatchOr]
      - in: query
        name: filter[entitledUsersPublishMatchAnd]
      - in: query
        name: filter[entitledUsersPublishMatchOr]
      - in: query
        name: filter[externalSourceTypeEqual]
        description: 'Enum Type: `KalturaExternalMediaSourceType`'
      - in: query
        name: filter[externalSourceTypeIn]
      - in: query
        name: filter[flavorParamsIdsMatchAnd]
      - in: query
        name: filter[flavorParamsIdsMatchOr]
      - in: query
        name: filter[freeText]
      - in: query
        name: filter[groupIdEqual]
      - in: query
        name: filter[hasMediaServerHostname]
      - in: query
        name: filter[idEqual]
        description: This filter should be in use for retrieving only a specific entry
          (identified by its entryId)
      - in: query
        name: filter[idIn]
        description: This filter should be in use for retrieving few specific entries
          (string should include comma separated list of entryId strings)
      - in: query
        name: filter[idNotIn]
      - in: query
        name: filter[isLive]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isRecordedEntryIdEmpty]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[isRoot]
        description: 'Enum Type: `KalturaNullableBoolean`'
      - in: query
        name: filter[lastPlayedAtGreaterThanOrEqual]
      - in: query
        name: filter[lastPlayedAtLessThanOrEqual]
      - in: query
        name: filter[limit]
      - in: query
        name: filter[mediaDateGreaterThanOrEqual]
      - in: query
        name: filter[mediaDateLessThanOrEqual]
      - in: query
        name: filter[mediaTypeEqual]
        description: 'Enum Type: `KalturaMediaType`'
      - in: query
        name: filter[mediaTypeIn]
      - in: query
        name: filter[moderationStatusEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: filter[moderationStatusIn]
      - in: query
        name: filter[moderationStatusNotEqual]
        description: 'Enum Type: `KalturaEntryModerationStatus`'
      - in: query
        name: filter[moderationStatusNotIn]
      - in: query
        name: filter[nameEqual]
        description: This filter should be in use for retrieving entries with a specific
          name
      - in: query
        name: filter[nameLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[nameMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[nameMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[objectType]
      - in: query
        name: filter[orderBy]
      - in: query
        name: filter[parentEntryIdEqual]
      - in: query
        name: filter[partnerIdEqual]
        description: This filter should be in use for retrieving only entries which
          were uploaded by/assigned to users of a specific Kaltura Partner (identified
          by Partner ID)
      - in: query
        name: filter[partnerIdIn]
        description: This filter should be in use for retrieving only entries within
          Kaltura network which were uploaded by/assigned to users of few Kaltura
          Partners  (string should include comma separated list of PartnerIDs)
      - in: query
        name: filter[partnerSortValueGreaterThanOrEqual]
      - in: query
        name: filter[partnerSortValueLessThanOrEqual]
      - in: query
        name: filter[redirectFromEntryId]
        description: The id of the original entry
      - in: query
        name: filter[referenceIdEqual]
      - in: query
        name: filter[referenceIdIn]
      - in: query
        name: filter[replacedEntryIdEqual]
      - in: query
        name: filter[replacedEntryIdIn]
      - in: query
        name: filter[replacementStatusEqual]
        description: 'Enum Type: `KalturaEntryReplacementStatus`'
      - in: query
        name: filter[replacementStatusIn]
      - in: query
        name: filter[replacingEntryIdEqual]
      - in: query
        name: filter[replacingEntryIdIn]
      - in: query
        name: filter[rootEntryIdEqual]
      - in: query
        name: filter[rootEntryIdIn]
      - in: query
        name: filter[searchTextMatchAnd]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within all of the following metadata
          attributes: name, description, tags, adminTags'
      - in: query
        name: filter[searchTextMatchOr]
        description: 'This filter should be in use for retrieving specific entries
          while search match the input string within at least one of the following
          metadata attributes: name, description, tags, adminTags'
      - in: query
        name: filter[sourceTypeEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: filter[sourceTypeIn]
      - in: query
        name: filter[sourceTypeNotEqual]
        description: 'Enum Type: `KalturaSourceType`'
      - in: query
        name: filter[sourceTypeNotIn]
      - in: query
        name: filter[startDateGreaterThanOrEqualOrNull]
      - in: query
        name: filter[startDateGreaterThanOrEqual]
      - in: query
        name: filter[startDateLessThanOrEqualOrNull]
      - in: query
        name: filter[startDateLessThanOrEqual]
      - in: query
        name: filter[statusEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, at a specific {'
      - in: query
        name: filter[statusIn]
        description: This filter should be in use for retrieving only entries, at
          few specific {
      - in: query
        name: filter[statusNotEqual]
        description: 'Enum Type: `KalturaEntryStatus`This filter should be in use
          for retrieving only entries, not at a specific {'
      - in: query
        name: filter[statusNotIn]
        description: This filter should be in use for retrieving only entries, not
          at few specific {
      - in: query
        name: filter[tagsAdminTagsMultiLikeAnd]
      - in: query
        name: filter[tagsAdminTagsMultiLikeOr]
      - in: query
        name: filter[tagsAdminTagsNameMultiLikeAnd]
      - in: query
        name: filter[tagsAdminTagsNameMultiLikeOr]
      - in: query
        name: filter[tagsLike]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsMultiLikeAnd]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsMultiLikeOr]
        description: This filter should be in use for retrieving specific entries
      - in: query
        name: filter[tagsNameMultiLikeAnd]
      - in: query
        name: filter[tagsNameMultiLikeOr]
      - in: query
        name: filter[totalRankGreaterThanOrEqual]
      - in: query
        name: filter[totalRankLessThanOrEqual]
      - in: query
        name: filter[typeEqual]
        description: 'Enum Type: `KalturaEntryType`'
      - in: query
        name: filter[typeIn]
        description: This filter should be in use for retrieving entries of few {
      - in: query
        name: filter[updatedAtGreaterThanOrEqual]
      - in: query
        name: filter[updatedAtLessThanOrEqual]
      - in: query
        name: filter[userIdEqual]
        description: This filter parameter should be in use for retrieving only entries,
          uploaded by/assigned to a specific user (identified by user Id)
      - in: query
        name: filter[userIdIn]
      - in: query
        name: filter[userIdNotIn]
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - List
  /service/baseentry/action/listByReferenceId:
    get:
      summary: Get Service Baseentry Action Listbyreferenceid
      description: List base entries by filter according to reference id
      operationId: baseEntry.listByReferenceId
      x-api-path-slug: servicebaseentryactionlistbyreferenceid-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: pager[pageIndex]
        description: The page number for which {pageSize} of objects should be retrieved
          (Default is 1)
      - in: query
        name: pager[pageSize]
        description: The number of objects to retrieve
      - in: query
        name: refId
        description: Entry Reference ID
      responses:
        200:
          description: OK
      tags:
      - Service
      - Baseentry
      - Action
      - ListByReferenceId
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---
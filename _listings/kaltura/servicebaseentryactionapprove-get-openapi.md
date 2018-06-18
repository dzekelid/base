---
swagger: "2.0"
x-collection-name: Kaltura
x-complete: 0
info:
  title: Kaltura VPaaS Get Service Baseentry Action Approve
  description: Approve the entry and mark the pending flags (if any) as moderated
    (this will make the entry playable).
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
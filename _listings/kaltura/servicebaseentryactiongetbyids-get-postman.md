{
  "info": {
    "name": "Kaltura VPaaS Get Service Baseentry Action Getbyids",
    "_postman_id": "54172121-8737-4184-aab2-fc7f6cd11b03",
    "description": "Get an array of KalturaBaseEntry objects by a comma-separated list of ids.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "3b768400-d8c4-4c04-8727-e7f5cc5a6b07",
          "name": "baseEntry.add",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/add?entry[accessControlId]=%7B%7D&entry[adminTags]=%7B%7D&entry[bitrates]=%7B%7D&entry[categoriesIds]=%7B%7D&entry[categories]=%7B%7D&entry[conversionProfileId]=%7B%7D&entry[conversionQuality]=%7B%7D&entry[creatorId]=%7B%7D&entry[creditUrl]=%7B%7D&entry[creditUserName]=%7B%7D&entry[currentBroadcastStartTime]=%7B%7D&entry[dataContent]=%7B%7D&entry[description]=%7B%7D&entry[displayInSearch]=%7B%7D&entry[documentType]=%7B%7D&entry[dvrStatus]=%7B%7D&entry[dvrWindow]=%7B%7D&entry[editorType]=%7B%7D&entry[encodingIP1]=%7B%7D&entry[encodingIP2]=%7B%7D&entry[endDate]=%7B%7D&entry[entitledUsersEdit]=%7B%7D&entry[entitledUsersPublish]=%7B%7D&entry[externalSourceType]=%7B%7D&entry[filters]=%7B%7D&entry[groupId]=%7B%7D&entry[hlsStreamUrl]=%7B%7D&entry[lastElapsedRecordingTime]=%7B%7D&entry[licenseType]=%7B%7D&entry[liveStreamConfigurations]=%7B%7D&entry[mediaType]=%7B%7D&entry[msDuration]=%7B%7D&entry[name]=%7B%7D&entry[objectType]=%7B%7D&entry[offlineMessage]=%7B%7D&entry[operationAttributes]=%7B%7D&entry[parentEntryId]=%7B%7D&entry[partnerData]=%7B%7D&entry[partnerSortValue]=%7B%7D&entry[playlistContent]=%7B%7D&entry[playlistId]=%7B%7D&entry[playlistType]=%7B%7D&entry[primaryBroadcastingUrl]=%7B%7D&entry[primaryRtspBroadcastingUrl]=%7B%7D&entry[publishConfigurations]=%7B%7D&entry[pushPublishEnabled]=%7B%7D&entry[recordedEntryId]=%7B%7D&entry[recordingOptions][shouldCopyEntitlement]=%7B%7D&entry[recordingOptions][shouldCopyScheduling]=%7B%7D&entry[recordingOptions][shouldCopyThumbnail]=%7B%7D&entry[recordingOptions][shouldMakeHidden]=%7B%7D&entry[recordStatus]=%7B%7D&entry[redirectEntryId]=%7B%7D&entry[referenceId]=%7B%7D&entry[repeat]=%7B%7D&entry[retrieveDataContentByGet]=%7B%7D&entry[searchProviderId]=%7B%7D&entry[searchProviderType]=%7B%7D&entry[secondaryBroadcastingUrl]=%7B%7D&entry[secondaryRtspBroadcastingUrl]=%7B%7D&entry[sourceType]=%7B%7D&entry[startDate]=%7B%7D&entry[streamName]=%7B%7D&entry[streamPassword]=%7B%7D&entry[streams]=%7B%7D&entry[streamUrl]=%7B%7D&entry[tags]=%7B%7D&entry[templateEntryId]=%7B%7D&entry[totalResults]=%7B%7D&entry[type]=%7B%7D&entry[urlManager]=%7B%7D&entry[userId]=%7B%7D&No Name=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generic add entry, should be used when the uploaded entry type is not known."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d86e197c-5b45-4148-b003-92f0a951df1d"
            }
          ]
        },
        {
          "id": "86985084-feb8-44ce-8705-8d8b889aa44c",
          "name": "baseEntry.addContent",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/addContent?entryId=%7B%7D&No Name=%7B%7D&resource[assetId]=%7B%7D&resource[content]=%7B%7D&resource[dropFolderFileId]=%7B%7D&resource[entryId]=%7B%7D&resource[fileSyncObjectType]=%7B%7D&resource[flavorParamsId]=%7B%7D&resource[forceAsyncDownload]=%7B%7D&resource[keepOriginalFile]=%7B%7D&resource[keyPassphrase]=%7B%7D&resource[localFilePath]=%7B%7D&resource[objectId]=%7B%7D&resource[objectSubType]=%7B%7D&resource[objectType]=%7B%7D&resource[privateKey]=%7B%7D&resource[publicKey]=%7B%7D&resource[resources]=%7B%7D&resource[resource][assetId]=%7B%7D&resource[resource][content]=%7B%7D&resource[resource][dropFolderFileId]=%7B%7D&resource[resource][entryId]=%7B%7D&resource[resource][fileSyncObjectType]=%7B%7D&resource[resource][flavorParamsId]=%7B%7D&resource[resource][forceAsyncDownload]=%7B%7D&resource[resource][keepOriginalFile]=%7B%7D&resource[resource][keyPassphrase]=%7B%7D&resource[resource][localFilePath]=%7B%7D&resource[resource][objectId]=%7B%7D&resource[resource][objectSubType]=%7B%7D&resource[resource][objectType]=%7B%7D&resource[resource][privateKey]=%7B%7D&resource[resource][publicKey]=%7B%7D&resource[resource][resources]=%7B%7D&resource[resource][resource][assetId]=%7B%7D&resource[resource][resource][content]=%7B%7D&resource[resource][resource][dropFolderFileId]=%7B%7D&resource[resource][resource][entryId]=%7B%7D&resource[resource][resource][fileSyncObjectType]=%7B%7D&resource[resource][resource][flavorParamsId]=%7B%7D&resource[resource][resource][forceAsyncDownload]=%7B%7D&resource[resource][resource][keepOriginalFile]=%7B%7D&resource[resource][resource][keyPassphrase]=%7B%7D&resource[resource][resource][localFilePath]=%7B%7D&resource[resource][resource][objectId]=%7B%7D&resource[resource][resource][objectSubType]=%7B%7D&resource[resource][resource][objectType]=%7B%7D&resource[resource][resource][privateKey]=%7B%7D&resource[resource][resource][publicKey]=%7B%7D&resource[resource][resource][resources]=%7B%7D&resource[resource][resource][resource][assetId]=%7B%7D&resource[resource][resource][resource][content]=%7B%7D&resource[resource][resource][resource][dropFolderFileId]=%7B%7D&resource[resource][resource][resource][entryId]=%7B%7D&resource[resource][resource][resource][fileSyncObjectType]=%7B%7D&resource[resource][resource][resource][flavorParamsId]=%7B%7D&resource[resource][resource][resource][forceAsyncDownload]=%7B%7D&resource[resource][resource][resource][keepOriginalFile]=%7B%7D&resource[resource][resource][resource][keyPassphrase]=%7B%7D&resource[resource][resource][resource][localFilePath]=%7B%7D&resource[resource][resource][resource][objectId]=%7B%7D&resource[resource][resource][resource][objectSubType]=%7B%7D&resource[resource][resource][resource][objectType]=%7B%7D&resource[resource][resource][resource][privateKey]=%7B%7D&resource[resource][resource][resource][publicKey]=%7B%7D&resource[resource][resource][resource][resources]=%7B%7D&resource[resource][resource][resource][storageProfileId]=%7B%7D&resource[resource][resource][resource][token]=%7B%7D&resource[resource][resource][resource][url]=%7B%7D&resource[resource][resource][resource][version]=%7B%7D&resource[resource][resource][storageProfileId]=%7B%7D&resource[resource][resource][token]=%7B%7D&resource[resource][resource][url]=%7B%7D&resource[resource][resource][version]=%7B%7D&resource[resource][storageProfileId]=%7B%7D&resource[resource][token]=%7B%7D&resource[resource][url]=%7B%7D&resource[resource][version]=%7B%7D&resource[storageProfileId]=%7B%7D&resource[token]=%7B%7D&resource[url]=%7B%7D&resource[version]=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "resource[fileData]",
                  "value": "{}",
                  "disabled": false,
                  "description": "Represents the $_FILE"
                },
                {
                  "key": "resource[resource][fileData]",
                  "value": "{}",
                  "disabled": false,
                  "description": "Represents the $_FILE"
                },
                {
                  "key": "resource[resource][resource][fileData]",
                  "value": "{}",
                  "disabled": false,
                  "description": "Represents the $_FILE"
                },
                {
                  "key": "resource[resource][resource][resource][fileData]",
                  "value": "{}",
                  "disabled": false,
                  "description": "Represents the $_FILE"
                }
              ]
            },
            "description": "Attach content resource to entry in status NO_MEDIA"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9665e876-a1f9-48d1-832c-bb29ef253ca4"
            }
          ]
        },
        {
          "id": "f7756e3b-49d7-48db-870e-ee1a9566cafa",
          "name": "baseEntry.addFromUploadedFile",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/addFromUploadedFile?entry[accessControlId]=%7B%7D&entry[adminTags]=%7B%7D&entry[bitrates]=%7B%7D&entry[categoriesIds]=%7B%7D&entry[categories]=%7B%7D&entry[conversionProfileId]=%7B%7D&entry[conversionQuality]=%7B%7D&entry[creatorId]=%7B%7D&entry[creditUrl]=%7B%7D&entry[creditUserName]=%7B%7D&entry[currentBroadcastStartTime]=%7B%7D&entry[dataContent]=%7B%7D&entry[description]=%7B%7D&entry[displayInSearch]=%7B%7D&entry[documentType]=%7B%7D&entry[dvrStatus]=%7B%7D&entry[dvrWindow]=%7B%7D&entry[editorType]=%7B%7D&entry[encodingIP1]=%7B%7D&entry[encodingIP2]=%7B%7D&entry[endDate]=%7B%7D&entry[entitledUsersEdit]=%7B%7D&entry[entitledUsersPublish]=%7B%7D&entry[externalSourceType]=%7B%7D&entry[filters]=%7B%7D&entry[groupId]=%7B%7D&entry[hlsStreamUrl]=%7B%7D&entry[lastElapsedRecordingTime]=%7B%7D&entry[licenseType]=%7B%7D&entry[liveStreamConfigurations]=%7B%7D&entry[mediaType]=%7B%7D&entry[msDuration]=%7B%7D&entry[name]=%7B%7D&entry[objectType]=%7B%7D&entry[offlineMessage]=%7B%7D&entry[operationAttributes]=%7B%7D&entry[parentEntryId]=%7B%7D&entry[partnerData]=%7B%7D&entry[partnerSortValue]=%7B%7D&entry[playlistContent]=%7B%7D&entry[playlistId]=%7B%7D&entry[playlistType]=%7B%7D&entry[primaryBroadcastingUrl]=%7B%7D&entry[primaryRtspBroadcastingUrl]=%7B%7D&entry[publishConfigurations]=%7B%7D&entry[pushPublishEnabled]=%7B%7D&entry[recordedEntryId]=%7B%7D&entry[recordingOptions][shouldCopyEntitlement]=%7B%7D&entry[recordingOptions][shouldCopyScheduling]=%7B%7D&entry[recordingOptions][shouldCopyThumbnail]=%7B%7D&entry[recordingOptions][shouldMakeHidden]=%7B%7D&entry[recordStatus]=%7B%7D&entry[redirectEntryId]=%7B%7D&entry[referenceId]=%7B%7D&entry[repeat]=%7B%7D&entry[retrieveDataContentByGet]=%7B%7D&entry[searchProviderId]=%7B%7D&entry[searchProviderType]=%7B%7D&entry[secondaryBroadcastingUrl]=%7B%7D&entry[secondaryRtspBroadcastingUrl]=%7B%7D&entry[sourceType]=%7B%7D&entry[startDate]=%7B%7D&entry[streamName]=%7B%7D&entry[streamPassword]=%7B%7D&entry[streams]=%7B%7D&entry[streamUrl]=%7B%7D&entry[tags]=%7B%7D&entry[templateEntryId]=%7B%7D&entry[totalResults]=%7B%7D&entry[type]=%7B%7D&entry[urlManager]=%7B%7D&entry[userId]=%7B%7D&No Name=%7B%7D&type=%7B%7D&uploadTokenId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Generic add entry using an uploaded file, should be used when the uploaded entry type is not known."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9bf04821-a25d-44dd-9b93-5f39bce8dda0"
            }
          ]
        },
        {
          "id": "491f6d54-6cea-40ca-b82d-f6c85cbfdfa5",
          "name": "baseEntry.anonymousRank",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/anonymousRank?entryId=%7B%7D&No Name=%7B%7D&rank=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Anonymously rank an entry, no validation is done on duplicate rankings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af3a9f8c-d107-4604-bddf-816a7870a60c"
            }
          ]
        },
        {
          "id": "fe485ac8-929d-44df-9670-fa7da799a4ee",
          "name": "baseEntry.approve",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/approve?entryId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Approve the entry and mark the pending flags (if any) as moderated (this will make the entry playable)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6671696-3a05-4763-92e6-6f4d37869521"
            }
          ]
        },
        {
          "id": "dabae2e0-1669-421f-af2d-bde43ef36486",
          "name": "baseEntry.clone",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/clone?entryId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Clone an entry with optional attributes to apply to the clone"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "feda65f3-d8c9-4d43-8314-a865d109ec56"
            }
          ]
        },
        {
          "id": "4192bbb4-c745-4907-bb12-b977ce453ddd",
          "name": "baseEntry.count",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/count?filter[accessControlIdEqual]=%7B%7D&filter[accessControlIdIn]=%7B%7D&filter[adminTagsLike]=%7B%7D&filter[adminTagsMultiLikeAnd]=%7B%7D&filter[adminTagsMultiLikeOr]=%7B%7D&filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[assetParamsIdsMatchAnd]=%7B%7D&filter[assetParamsIdsMatchOr]=%7B%7D&filter[categoriesFullNameIn]=%7B%7D&filter[categoriesIdsEmpty]=%7B%7D&filter[categoriesIdsMatchAnd]=%7B%7D&filter[categoriesIdsMatchOr]=%7B%7D&filter[categoriesIdsNotContains]=%7B%7D&filter[categoriesMatchAnd]=%7B%7D&filter[categoriesMatchOr]=%7B%7D&filter[categoriesNotContains]=%7B%7D&filter[categoryAncestorIdIn]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[creatorIdEqual]=%7B%7D&filter[documentTypeEqual]=%7B%7D&filter[documentTypeIn]=%7B%7D&filter[durationGreaterThanOrEqual]=%7B%7D&filter[durationGreaterThan]=%7B%7D&filter[durationLessThanOrEqual]=%7B%7D&filter[durationLessThan]=%7B%7D&filter[durationTypeMatchOr]=%7B%7D&filter[endDateGreaterThanOrEqualOrNull]=%7B%7D&filter[endDateGreaterThanOrEqual]=%7B%7D&filter[endDateLessThanOrEqualOrNull]=%7B%7D&filter[endDateLessThanOrEqual]=%7B%7D&filter[entitledUsersEditMatchAnd]=%7B%7D&filter[entitledUsersEditMatchOr]=%7B%7D&filter[entitledUsersPublishMatchAnd]=%7B%7D&filter[entitledUsersPublishMatchOr]=%7B%7D&filter[externalSourceTypeEqual]=%7B%7D&filter[externalSourceTypeIn]=%7B%7D&filter[flavorParamsIdsMatchAnd]=%7B%7D&filter[flavorParamsIdsMatchOr]=%7B%7D&filter[freeText]=%7B%7D&filter[groupIdEqual]=%7B%7D&filter[hasMediaServerHostname]=%7B%7D&filter[idEqual]=%7B%7D&filter[idIn]=%7B%7D&filter[idNotIn]=%7B%7D&filter[isLive]=%7B%7D&filter[isRecordedEntryIdEmpty]=%7B%7D&filter[isRoot]=%7B%7D&filter[lastPlayedAtGreaterThanOrEqual]=%7B%7D&filter[lastPlayedAtLessThanOrEqual]=%7B%7D&filter[limit]=%7B%7D&filter[mediaDateGreaterThanOrEqual]=%7B%7D&filter[mediaDateLessThanOrEqual]=%7B%7D&filter[mediaTypeEqual]=%7B%7D&filter[mediaTypeIn]=%7B%7D&filter[moderationStatusEqual]=%7B%7D&filter[moderationStatusIn]=%7B%7D&filter[moderationStatusNotEqual]=%7B%7D&filter[moderationStatusNotIn]=%7B%7D&filter[nameEqual]=%7B%7D&filter[nameLike]=%7B%7D&filter[nameMultiLikeAnd]=%7B%7D&filter[nameMultiLikeOr]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[parentEntryIdEqual]=%7B%7D&filter[partnerIdEqual]=%7B%7D&filter[partnerIdIn]=%7B%7D&filter[partnerSortValueGreaterThanOrEqual]=%7B%7D&filter[partnerSortValueLessThanOrEqual]=%7B%7D&filter[redirectFromEntryId]=%7B%7D&filter[referenceIdEqual]=%7B%7D&filter[referenceIdIn]=%7B%7D&filter[replacedEntryIdEqual]=%7B%7D&filter[replacedEntryIdIn]=%7B%7D&filter[replacementStatusEqual]=%7B%7D&filter[replacementStatusIn]=%7B%7D&filter[replacingEntryIdEqual]=%7B%7D&filter[replacingEntryIdIn]=%7B%7D&filter[rootEntryIdEqual]=%7B%7D&filter[rootEntryIdIn]=%7B%7D&filter[searchTextMatchAnd]=%7B%7D&filter[searchTextMatchOr]=%7B%7D&filter[sourceTypeEqual]=%7B%7D&filter[sourceTypeIn]=%7B%7D&filter[sourceTypeNotEqual]=%7B%7D&filter[sourceTypeNotIn]=%7B%7D&filter[startDateGreaterThanOrEqualOrNull]=%7B%7D&filter[startDateGreaterThanOrEqual]=%7B%7D&filter[startDateLessThanOrEqualOrNull]=%7B%7D&filter[startDateLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[statusNotEqual]=%7B%7D&filter[statusNotIn]=%7B%7D&filter[tagsAdminTagsMultiLikeAnd]=%7B%7D&filter[tagsAdminTagsMultiLikeOr]=%7B%7D&filter[tagsAdminTagsNameMultiLikeAnd]=%7B%7D&filter[tagsAdminTagsNameMultiLikeOr]=%7B%7D&filter[tagsLike]=%7B%7D&filter[tagsMultiLikeAnd]=%7B%7D&filter[tagsMultiLikeOr]=%7B%7D&filter[tagsNameMultiLikeAnd]=%7B%7D&filter[tagsNameMultiLikeOr]=%7B%7D&filter[totalRankGreaterThanOrEqual]=%7B%7D&filter[totalRankLessThanOrEqual]=%7B%7D&filter[typeEqual]=%7B%7D&filter[typeIn]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&filter[userIdEqual]=%7B%7D&filter[userIdIn]=%7B%7D&filter[userIdNotIn]=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Count base entries by filter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60eaa924-c944-480d-a365-499ceda2f28f"
            }
          ]
        },
        {
          "id": "8e59450b-dbac-487d-b923-3f1149bbe4d9",
          "name": "baseEntry.delete",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/delete?entryId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an entry."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ce600f8-52ea-4a19-b2ce-8c3306063f6b"
            }
          ]
        },
        {
          "id": "3c40bff4-1b11-4877-afc1-f8dc9a66ce98",
          "name": "baseEntry.export",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/export?entryId=%7B%7D&No Name=%7B%7D&storageProfileId=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Service Baseentry Action Export"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43f291db-2959-4ac0-acc0-7a21a45cd858"
            }
          ]
        },
        {
          "id": "825ffbe4-df72-4490-ae69-03262ff99798",
          "name": "baseEntry.flag",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/flag?moderationFlag[comments]=%7B%7D&moderationFlag[flaggedEntryId]=%7B%7D&moderationFlag[flaggedUserId]=%7B%7D&moderationFlag[flagType]=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Flag inappropriate entry for moderation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "547d294d-e906-4cee-8e86-5da5b5b47e45"
            }
          ]
        },
        {
          "id": "9d802da0-dbd3-42b1-8f75-d8d8ec2c4e1a",
          "name": "baseEntry.get",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/get?entryId=%7B%7D&No Name=%7B%7D&version=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get base entry by ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a441a91-1ef6-4c94-b29b-5c99d52af3a6"
            }
          ]
        },
        {
          "id": "3d3f2797-ecd4-40d4-9d66-1bacce765c48",
          "name": "baseEntry.getByIds",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/getByIds?entryIds=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get an array of KalturaBaseEntry objects by a comma-separated list of ids."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5859e80e-a168-4b30-9c26-5c1ead70a7e5"
            }
          ]
        }
      ]
    }
  ]
}
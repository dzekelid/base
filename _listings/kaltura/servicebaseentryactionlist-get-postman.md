{
  "info": {
    "name": "Kaltura VPaaS Get Service Baseentry Action List",
    "_postman_id": "73402b36-be7a-42cd-8337-558408993b5e",
    "description": "List base entries by filter with paging support.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "ae9aeac0-9f02-47b0-ac91-20cf98cac775",
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
              "id": "65829b65-b2bb-48d4-9ac2-2e7f1d6ad931"
            }
          ]
        },
        {
          "id": "c8c12915-ff94-42ff-95ee-439439068626",
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
              "id": "3ed00495-5c35-4f84-9972-ef52d6e39b56"
            }
          ]
        },
        {
          "id": "9bce45f4-379f-46f5-925d-d7f6bba6d67b",
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
              "id": "a83a2195-f8d4-4a7b-8c02-5cba0da2f6fc"
            }
          ]
        },
        {
          "id": "e6da94fe-5ad7-4565-9deb-251dbfaaf07a",
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
              "id": "03bc842b-a88b-496a-8956-5ae72192da27"
            }
          ]
        },
        {
          "id": "a9c1240a-ce6b-4603-ba23-2baf95dfca07",
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
              "id": "034c6e66-bdcd-429f-95c9-5d7ae3c7e274"
            }
          ]
        },
        {
          "id": "0f12de21-f492-4376-89ed-2d6cc11721f8",
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
              "id": "a2778eb1-0c3c-4b42-98ce-ecba9fbe9822"
            }
          ]
        },
        {
          "id": "f1f484eb-ab60-4382-a311-7b7ddf7d3574",
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
              "id": "81f9f655-1a0e-421c-8672-8bdde6dbf803"
            }
          ]
        },
        {
          "id": "ce6e66b4-8526-4a4a-ba4c-fce260990888",
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
              "id": "f31b5139-553f-4a3f-877a-be5822724d66"
            }
          ]
        },
        {
          "id": "e4d7fa39-6106-484b-ab33-4fc008593284",
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
              "id": "aa590a87-396e-4fbc-ad59-49867ba11b7a"
            }
          ]
        },
        {
          "id": "28ce6bc8-e837-48ec-8356-4d0d9b60deee",
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
              "id": "d032d354-2ab5-47d2-ae40-592b0715b1e6"
            }
          ]
        },
        {
          "id": "c707b89a-e6de-4798-9506-39e2bc2f9b95",
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
              "id": "a2ee4559-38fa-4d0d-b562-a196906dc039"
            }
          ]
        },
        {
          "id": "38177f92-7c04-4306-9c0e-1ef368762d42",
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
              "id": "75001756-bbca-4c14-b82a-7c0681839059"
            }
          ]
        },
        {
          "id": "118b6572-d11c-461c-95d1-303cd0287d6a",
          "name": "baseEntry.getContextData",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/getContextData?contextDataParams[contexts]=%7B%7D&contextDataParams[flavorAssetId]=%7B%7D&contextDataParams[flavorTags]=%7B%7D&contextDataParams[hashes]=%7B%7D&contextDataParams[ip]=%7B%7D&contextDataParams[ks]=%7B%7D&contextDataParams[mediaProtocol]=%7B%7D&contextDataParams[objectType]=%7B%7D&contextDataParams[referrer]=%7B%7D&contextDataParams[streamerType]=%7B%7D&contextDataParams[time]=%7B%7D&contextDataParams[userAgent]=%7B%7D&entryId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This action delivers entry-related data, based on the user's context: access control, restriction, playback format and storage information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2047cd1b-f67d-47b9-880e-89b3b94adc28"
            }
          ]
        },
        {
          "id": "9eb1907b-d28b-4b1b-a487-c0f072f7314a",
          "name": "baseEntry.getPlaybackContext",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/getPlaybackContext?contextDataParams[contexts]=%7B%7D&contextDataParams[flavorAssetId]=%7B%7D&contextDataParams[flavorTags]=%7B%7D&contextDataParams[hashes]=%7B%7D&contextDataParams[ip]=%7B%7D&contextDataParams[ks]=%7B%7D&contextDataParams[mediaProtocol]=%7B%7D&contextDataParams[referrer]=%7B%7D&contextDataParams[streamerType]=%7B%7D&contextDataParams[time]=%7B%7D&contextDataParams[userAgent]=%7B%7D&entryId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This action delivers all data relevant for player"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0759b21c-ac84-400d-b0a3-a837a5bfa4b3"
            }
          ]
        },
        {
          "id": "be16c3db-cf8f-4ec7-bbce-69fe1e7705b7",
          "name": "baseEntry.getRemotePaths",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/getRemotePaths?entryId=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get remote storage existing paths for the asset."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "badf7c8b-9f52-48a6-9b0c-ac1adf4fddaf"
            }
          ]
        },
        {
          "id": "0169a5b6-c982-489f-8c8b-c9c665e15c0b",
          "name": "baseEntry.index",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/index?id=%7B%7D&No Name=%7B%7D&shouldUpdate=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Index an entry by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2105a452-e747-4921-b818-9bd19b26375f"
            }
          ]
        },
        {
          "id": "551c46ab-70e0-4fd4-a053-0d764370bdb1",
          "name": "baseEntry.list",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/baseentry/action/list?filter[accessControlIdEqual]=%7B%7D&filter[accessControlIdIn]=%7B%7D&filter[adminTagsLike]=%7B%7D&filter[adminTagsMultiLikeAnd]=%7B%7D&filter[adminTagsMultiLikeOr]=%7B%7D&filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[assetParamsIdsMatchAnd]=%7B%7D&filter[assetParamsIdsMatchOr]=%7B%7D&filter[categoriesFullNameIn]=%7B%7D&filter[categoriesIdsEmpty]=%7B%7D&filter[categoriesIdsMatchAnd]=%7B%7D&filter[categoriesIdsMatchOr]=%7B%7D&filter[categoriesIdsNotContains]=%7B%7D&filter[categoriesMatchAnd]=%7B%7D&filter[categoriesMatchOr]=%7B%7D&filter[categoriesNotContains]=%7B%7D&filter[categoryAncestorIdIn]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[creatorIdEqual]=%7B%7D&filter[documentTypeEqual]=%7B%7D&filter[documentTypeIn]=%7B%7D&filter[durationGreaterThanOrEqual]=%7B%7D&filter[durationGreaterThan]=%7B%7D&filter[durationLessThanOrEqual]=%7B%7D&filter[durationLessThan]=%7B%7D&filter[durationTypeMatchOr]=%7B%7D&filter[endDateGreaterThanOrEqualOrNull]=%7B%7D&filter[endDateGreaterThanOrEqual]=%7B%7D&filter[endDateLessThanOrEqualOrNull]=%7B%7D&filter[endDateLessThanOrEqual]=%7B%7D&filter[entitledUsersEditMatchAnd]=%7B%7D&filter[entitledUsersEditMatchOr]=%7B%7D&filter[entitledUsersPublishMatchAnd]=%7B%7D&filter[entitledUsersPublishMatchOr]=%7B%7D&filter[externalSourceTypeEqual]=%7B%7D&filter[externalSourceTypeIn]=%7B%7D&filter[flavorParamsIdsMatchAnd]=%7B%7D&filter[flavorParamsIdsMatchOr]=%7B%7D&filter[freeText]=%7B%7D&filter[groupIdEqual]=%7B%7D&filter[hasMediaServerHostname]=%7B%7D&filter[idEqual]=%7B%7D&filter[idIn]=%7B%7D&filter[idNotIn]=%7B%7D&filter[isLive]=%7B%7D&filter[isRecordedEntryIdEmpty]=%7B%7D&filter[isRoot]=%7B%7D&filter[lastPlayedAtGreaterThanOrEqual]=%7B%7D&filter[lastPlayedAtLessThanOrEqual]=%7B%7D&filter[limit]=%7B%7D&filter[mediaDateGreaterThanOrEqual]=%7B%7D&filter[mediaDateLessThanOrEqual]=%7B%7D&filter[mediaTypeEqual]=%7B%7D&filter[mediaTypeIn]=%7B%7D&filter[moderationStatusEqual]=%7B%7D&filter[moderationStatusIn]=%7B%7D&filter[moderationStatusNotEqual]=%7B%7D&filter[moderationStatusNotIn]=%7B%7D&filter[nameEqual]=%7B%7D&filter[nameLike]=%7B%7D&filter[nameMultiLikeAnd]=%7B%7D&filter[nameMultiLikeOr]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[parentEntryIdEqual]=%7B%7D&filter[partnerIdEqual]=%7B%7D&filter[partnerIdIn]=%7B%7D&filter[partnerSortValueGreaterThanOrEqual]=%7B%7D&filter[partnerSortValueLessThanOrEqual]=%7B%7D&filter[redirectFromEntryId]=%7B%7D&filter[referenceIdEqual]=%7B%7D&filter[referenceIdIn]=%7B%7D&filter[replacedEntryIdEqual]=%7B%7D&filter[replacedEntryIdIn]=%7B%7D&filter[replacementStatusEqual]=%7B%7D&filter[replacementStatusIn]=%7B%7D&filter[replacingEntryIdEqual]=%7B%7D&filter[replacingEntryIdIn]=%7B%7D&filter[rootEntryIdEqual]=%7B%7D&filter[rootEntryIdIn]=%7B%7D&filter[searchTextMatchAnd]=%7B%7D&filter[searchTextMatchOr]=%7B%7D&filter[sourceTypeEqual]=%7B%7D&filter[sourceTypeIn]=%7B%7D&filter[sourceTypeNotEqual]=%7B%7D&filter[sourceTypeNotIn]=%7B%7D&filter[startDateGreaterThanOrEqualOrNull]=%7B%7D&filter[startDateGreaterThanOrEqual]=%7B%7D&filter[startDateLessThanOrEqualOrNull]=%7B%7D&filter[startDateLessThanOrEqual]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[statusNotEqual]=%7B%7D&filter[statusNotIn]=%7B%7D&filter[tagsAdminTagsMultiLikeAnd]=%7B%7D&filter[tagsAdminTagsMultiLikeOr]=%7B%7D&filter[tagsAdminTagsNameMultiLikeAnd]=%7B%7D&filter[tagsAdminTagsNameMultiLikeOr]=%7B%7D&filter[tagsLike]=%7B%7D&filter[tagsMultiLikeAnd]=%7B%7D&filter[tagsMultiLikeOr]=%7B%7D&filter[tagsNameMultiLikeAnd]=%7B%7D&filter[tagsNameMultiLikeOr]=%7B%7D&filter[totalRankGreaterThanOrEqual]=%7B%7D&filter[totalRankLessThanOrEqual]=%7B%7D&filter[typeEqual]=%7B%7D&filter[typeIn]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&filter[userIdEqual]=%7B%7D&filter[userIdIn]=%7B%7D&filter[userIdNotIn]=%7B%7D&No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List base entries by filter with paging support."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3b9dea41-96d9-4958-bcd9-ac33ad0cb1e5"
            }
          ]
        }
      ]
    }
  ]
}
{
  "info": {
    "name": "Kaltura VPaaS Get Service Baseentry Action Add",
    "_postman_id": "f3c0ef55-787a-42aa-8c9f-7b1118d4e108",
    "description": "Generic add entry, should be used when the uploaded entry type is not known.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "0d153273-b5bf-4b41-8596-228f9198dd34",
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
              "id": "d2bcc31e-5652-4d56-b27d-8dd4b5358e84"
            }
          ]
        }
      ]
    }
  ]
}
---
swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 0
info:
  title: AWS OpsWorks API Describe Time Based Auto Scaling
  version: 1.0.0
  description: Describes time-based auto scaling configurations for specified instances.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeLoadBasedAutoScaling:
    get:
      summary: Describe Load Based Auto Scaling
      description: Describes load-based auto scaling configurations for specified
        layers.
      operationId: describeLoadBasedAutoScaling
      x-api-path-slug: actiondescribeloadbasedautoscaling-get
      parameters:
      - in: query
        name: LayerIds
        description: An array of layer IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Load
      - Based
      - Auto
      - Scaling
  /?Action=DescribeTimeBasedAutoScaling:
    get:
      summary: Describe Time Based Auto Scaling
      description: Describes time-based auto scaling configurations for specified
        instances.
      operationId: describeTimeBasedAutoScaling
      x-api-path-slug: actiondescribetimebasedautoscaling-get
      parameters:
      - in: query
        name: InstanceIds
        description: An array of instance IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Describe
      - Time
      - Based
      - Auto
      - Scaling
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
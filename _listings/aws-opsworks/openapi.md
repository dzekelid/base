swagger: "2.0"
x-collection-name: AWS OpsWorks
x-complete: 1
info:
  title: AWS OpsWorks API
  version: 1.0.0
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
  /?Action=SetLoadBasedAutoScaling:
    get:
      summary: Set Load Based Auto Scaling
      description: Specify the load-based auto scaling configuration for a specified
        layer.
      operationId: setLoadBasedAutoScaling
      x-api-path-slug: actionsetloadbasedautoscaling-get
      parameters:
      - in: query
        name: DownScaling
        description: An AutoScalingThresholds object with the downscaling threshold
          configuration
        type: string
      - in: query
        name: Enable
        description: Enables load-based auto scaling for the layer
        type: string
      - in: query
        name: LayerId
        description: The layer ID
        type: string
      - in: query
        name: UpScaling
        description: An AutoScalingThresholds object with the upscaling threshold
          configuration
        type: string
      responses:
        200:
          description: OK
      tags:
      - Set
      - Load
      - Based
      - Auto
      - Scaling
  /?Action=SetTimeBasedAutoScaling:
    get:
      summary: Set Time Based Auto Scaling
      description: Specify the time-based auto scaling configuration for a specified
        instance.
      operationId: setTimeBasedAutoScaling
      x-api-path-slug: actionsettimebasedautoscaling-get
      parameters:
      - in: query
        name: AutoScalingSchedule
        description: An AutoScalingSchedule with the instance schedule
        type: string
      - in: query
        name: InstanceId
        description: The instance ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - Set
      - Time
      - Based
      - Auto
      - Scaling
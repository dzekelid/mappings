---
swagger: "2.0"
x-collection-name: IBM Watson
x-complete: 0
info:
  title: |-
    IBM Watson IoT Platform Get the draft property mappings for a specific logical interface for
    a thing type.
  description: |-
    Retrieves the draft property mappings for a specific logical interface
    for the thing type.
  version: 1.0.0
basePath: /api/v0002
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /device/types/{typeId}/mappings:
    get:
      summary: Get the list of active property mappings for the device type
      description: |-
        Retrieve the list of active property mappings for the specified device
        type.  A property mapping defines how properties from inbound events are
        mapped to properties defined on an logical interface associated with
        the device type.
      operationId: retrieve-the-list-of-active-property-mappings-for-the-specified-devicetype--a-property-mapping-defin
      x-api-path-slug: devicetypestypeidmappings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Device
      - Types
      - Mappings
  /device/types/{typeId}/mappings/{logicalInterfaceId}:
    get:
      summary: |-
        Get the active property mappings for a specific logical interface
        for a device type.
      description: |-
        Retrieves the active property mappings for a specific logical
        interface for the device type.
      operationId: retrieves-the-active-property-mappings-for-a-specific-logicalinterface-for-the-device-type
      x-api-path-slug: devicetypestypeidmappingslogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Device
      - Types
      - Mappings
      - LogicalInterfaceId
  /draft/device/types/{typeId}/mappings:
    get:
      summary: Get the list of draft property mappings for the device type
      description: |-
        Retrieve the list of draft property mappings for the specified device
        type.  A property mapping defines how properties from inbound events are
        mapped to properties defined on an logical interface associated with
        the device type.
      operationId: retrieve-the-list-of-draft-property-mappings-for-the-specified-devicetype--a-property-mapping-define
      x-api-path-slug: draftdevicetypestypeidmappings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Device
      - Types
      - Mappings
    post:
      summary: |-
        Create the draft property mappings for a logical interface for the
        device type
      description: |-
        Creates the draft property mappings for an logical interface for the
        device type.  The mapping object must specify:
        - The id for for the logical interface that the mappings are for
        - The mappings that define how to map from properties on the inbound
          events to the properties on the logical interface.  The mappings
          are keyed off of the event ids defined by the physical interface
          associated with the device type.
      operationId: creates-the-draft-property-mappings-for-an-logical-interface-for-thedevice-type--the-mapping-object-
      x-api-path-slug: draftdevicetypestypeidmappings-post
      parameters:
      - in: body
        name: Device Type Property Mappings
        description: The JSON representation of the draft device type property mappings
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Device
      - Types
      - Mappings
  /draft/device/types/{typeId}/mappings/{logicalInterfaceId}:
    get:
      summary: |-
        Get the draft property mappings for a specific logical interface for
        a device type.
      description: |-
        Retrieves the draft property mappings for a specific logical
        interface for the device type.
      operationId: retrieves-the-draft-property-mappings-for-a-specific-logicalinterface-for-the-device-type
      x-api-path-slug: draftdevicetypestypeidmappingslogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Device
      - Types
      - Mappings
      - LogicalInterfaceId
    put:
      summary: |-
        Update the draft property mappings for a specific logical interface
        for the device type.
      description: |-
        Updates the draft property mappings for a specific logical interface
        for the device type.
      operationId: updates-the-draft-property-mappings-for-a-specific-logical-interfacefor-the-device-type
      x-api-path-slug: draftdevicetypestypeidmappingslogicalinterfaceid-put
      parameters:
      - in: body
        name: Device Type Property Mappings
        description: The JSON representation of the draft device type property mappings
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Device
      - Types
      - Mappings
      - LogicalInterfaceId
    delete:
      summary: |-
        Delete the draft property mappings for a specific logical interface
        for the device type.
      description: |-
        Deletes the draft property mappings for a specific logical interface
        for the device type.
      operationId: deletes-the-draft-property-mappings-for-a-specific-logical-interfacefor-the-device-type
      x-api-path-slug: draftdevicetypestypeidmappingslogicalinterfaceid-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Device
      - Types
      - Mappings
      - LogicalInterfaceId
  /thing/types/{thingTypeId}/mappings:
    get:
      summary: Get the list of active property mappings for the thing type
      description: |-
        Retrieve the list of active property mappings for the specified thing
        type.  A property mapping defines how properties from state update events
        on aggregated devices or things are mapped to properties defined on a
        logical interface associated with the thing type.
      operationId: retrieve-the-list-of-active-property-mappings-for-the-specified-thingtype--a-property-mapping-define
      x-api-path-slug: thingtypesthingtypeidmappings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Thing
      - Types
      - ThingTypeId
      - Mappings
  /thing/types/{thingTypeId}/mappings/{logicalInterfaceId}:
    get:
      summary: |-
        Get the active property mappings for a specific logical interface for
        a thing type.
      description: |-
        Retrieves the active property mappings for a specific logical interface
        for the thing type.
      operationId: retrieves-the-active-property-mappings-for-a-specific-logical-interfacefor-the-thing-type
      x-api-path-slug: thingtypesthingtypeidmappingslogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Thing
      - Types
      - ThingTypeId
      - Mappings
      - LogicalInterfaceId
  /draft/thing/types/{thingTypeId}/mappings:
    get:
      summary: Get the list of draft property mappings for the thing type
      description: |-
        Retrieve the list of draft property mappings for the specified draft
        thing type.  A property mapping defines how properties from state update
        events on aggregated devices or things are mapped to properties defined
        on a logical interface associated with the thing type.
      operationId: retrieve-the-list-of-draft-property-mappings-for-the-specified-draftthing-type--a-property-mapping-d
      x-api-path-slug: draftthingtypesthingtypeidmappings-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Thing
      - Types
      - ThingTypeId
      - Mappings
    post:
      summary: |-
        Create the draft property mappings for a logical interface for the thing
        type
      description: |-
        Creates the draft property mappings for a logical interface for the
        thing type.  The mapping object must specify:
        - The id for for the logical interface that the mappings are for
        - The mappings that define how to map from properties on the state
          update events to the properties on the logical interface.  The
          mappings are keyed off of the name of the internal properties of the
          thing type.
      operationId: creates-the-draft-property-mappings-for-a-logical-interface-for-thething-type--the-mapping-object-mu
      x-api-path-slug: draftthingtypesthingtypeidmappings-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: Thing Type Property Mappings
        description: The JSON representation of the thing type property mappings
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Thing
      - Types
      - ThingTypeId
      - Mappings
  /draft/thing/types/{thingTypeId}/mappings/{logicalInterfaceId}:
    get:
      summary: |-
        Get the draft property mappings for a specific logical interface for
        a thing type.
      description: |-
        Retrieves the draft property mappings for a specific logical interface
        for the thing type.
      operationId: retrieves-the-draft-property-mappings-for-a-specific-logical-interfacefor-the-thing-type
      x-api-path-slug: draftthingtypesthingtypeidmappingslogicalinterfaceid-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Internet of Things
      - Draft
      - Thing
      - Types
      - ThingTypeId
      - Mappings
      - LogicalInterfaceId
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
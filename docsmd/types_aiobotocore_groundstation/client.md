# GroundStationClient

> [Index](../README.md) > [GroundStation](./README.md) > GroundStationClient

!!! note ""

    Auto-generated documentation for [GroundStation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation)
    type annotations stubs module [types-aiobotocore-groundstation](https://pypi.org/project/types-aiobotocore-groundstation/).

## GroundStationClient

Type annotations and code completion for `#!python session.create_client("groundstation")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client)

```python
GroundStationClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_groundstation.client import GroundStationClient

session = get_session()
async with session.create_client("groundstation") as client:
    client: GroundStationClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("groundstation").exceptions` structure.

```python
GroundStationClient.exceptions usage example

async with session.create_client("groundstation") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.DependencyException,
        client.InvalidParameterException,
        client.ResourceLimitExceededException,
        client.ResourceNotFoundException,
    ) as e:
        print(e)
```

```python
GroundStationClient usage type checking example

from types_aiobotocore_groundstation.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("groundstation").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_contact

Cancels a contact with a specified contact ID.

Type annotations and code completion for `#!python session.create_client("groundstation").cancel_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.cancel_contact)

```python
# cancel_contact method definition

await def cancel_contact(
    self,
    *,
    contactId: str,
) -> ContactIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ContactIdResponseTypeDef](./type_defs.md#contactidresponsetypedef) 


```python
# cancel_contact method usage example with argument unpacking

kwargs: CancelContactRequestRequestTypeDef = {  # (1)
    "contactId": ...,
}

parent.cancel_contact(**kwargs)
```

1. See [:material-code-braces: CancelContactRequestRequestTypeDef](./type_defs.md#cancelcontactrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("groundstation").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_config

Creates a `Config` with the specified `configData` parameters.

Type annotations and code completion for `#!python session.create_client("groundstation").create_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_config)

```python
# create_config method definition

await def create_config(
    self,
    *,
    configData: ConfigTypeDataTypeDef,  # (1)
    name: str,
    tags: Mapping[str, str] = ...,
) -> ConfigIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef) 
2. See [:material-code-braces: ConfigIdResponseTypeDef](./type_defs.md#configidresponsetypedef) 


```python
# create_config method usage example with argument unpacking

kwargs: CreateConfigRequestRequestTypeDef = {  # (1)
    "configData": ...,
    "name": ...,
}

parent.create_config(**kwargs)
```

1. See [:material-code-braces: CreateConfigRequestRequestTypeDef](./type_defs.md#createconfigrequestrequesttypedef) 

### create\_dataflow\_endpoint\_group

Creates a `DataflowEndpoint` group containing the specified list of
`DataflowEndpoint` objects.

Type annotations and code completion for `#!python session.create_client("groundstation").create_dataflow_endpoint_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_dataflow_endpoint_group)

```python
# create_dataflow_endpoint_group method definition

await def create_dataflow_endpoint_group(
    self,
    *,
    endpointDetails: Sequence[EndpointDetailsTypeDef],  # (1)
    contactPostPassDurationSeconds: int = ...,
    contactPrePassDurationSeconds: int = ...,
    tags: Mapping[str, str] = ...,
) -> DataflowEndpointGroupIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EndpointDetailsTypeDef](./type_defs.md#endpointdetailstypedef) 
2. See [:material-code-braces: DataflowEndpointGroupIdResponseTypeDef](./type_defs.md#dataflowendpointgroupidresponsetypedef) 


```python
# create_dataflow_endpoint_group method usage example with argument unpacking

kwargs: CreateDataflowEndpointGroupRequestRequestTypeDef = {  # (1)
    "endpointDetails": ...,
}

parent.create_dataflow_endpoint_group(**kwargs)
```

1. See [:material-code-braces: CreateDataflowEndpointGroupRequestRequestTypeDef](./type_defs.md#createdataflowendpointgrouprequestrequesttypedef) 

### create\_ephemeris

Creates an Ephemeris with the specified `EphemerisData`.

Type annotations and code completion for `#!python session.create_client("groundstation").create_ephemeris` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_ephemeris)

```python
# create_ephemeris method definition

await def create_ephemeris(
    self,
    *,
    name: str,
    satelliteId: str,
    enabled: bool = ...,
    ephemeris: EphemerisDataTypeDef = ...,  # (1)
    expirationTime: Union[datetime, str] = ...,
    kmsKeyArn: str = ...,
    priority: int = ...,
    tags: Mapping[str, str] = ...,
) -> EphemerisIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EphemerisDataTypeDef](./type_defs.md#ephemerisdatatypedef) 
2. See [:material-code-braces: EphemerisIdResponseTypeDef](./type_defs.md#ephemerisidresponsetypedef) 


```python
# create_ephemeris method usage example with argument unpacking

kwargs: CreateEphemerisRequestRequestTypeDef = {  # (1)
    "name": ...,
    "satelliteId": ...,
}

parent.create_ephemeris(**kwargs)
```

1. See [:material-code-braces: CreateEphemerisRequestRequestTypeDef](./type_defs.md#createephemerisrequestrequesttypedef) 

### create\_mission\_profile

Creates a mission profile.

Type annotations and code completion for `#!python session.create_client("groundstation").create_mission_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.create_mission_profile)

```python
# create_mission_profile method definition

await def create_mission_profile(
    self,
    *,
    dataflowEdges: Sequence[Sequence[str]],
    minimumViableContactDurationSeconds: int,
    name: str,
    trackingConfigArn: str,
    contactPostPassDurationSeconds: int = ...,
    contactPrePassDurationSeconds: int = ...,
    streamsKmsKey: KmsKeyTypeDef = ...,  # (1)
    streamsKmsRole: str = ...,
    tags: Mapping[str, str] = ...,
) -> MissionProfileIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: KmsKeyTypeDef](./type_defs.md#kmskeytypedef) 
2. See [:material-code-braces: MissionProfileIdResponseTypeDef](./type_defs.md#missionprofileidresponsetypedef) 


```python
# create_mission_profile method usage example with argument unpacking

kwargs: CreateMissionProfileRequestRequestTypeDef = {  # (1)
    "dataflowEdges": ...,
    "minimumViableContactDurationSeconds": ...,
    "name": ...,
    "trackingConfigArn": ...,
}

parent.create_mission_profile(**kwargs)
```

1. See [:material-code-braces: CreateMissionProfileRequestRequestTypeDef](./type_defs.md#createmissionprofilerequestrequesttypedef) 

### delete\_config

Deletes a `Config`.

Type annotations and code completion for `#!python session.create_client("groundstation").delete_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.delete_config)

```python
# delete_config method definition

await def delete_config(
    self,
    *,
    configId: str,
    configType: ConfigCapabilityTypeType,  # (1)
) -> ConfigIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
2. See [:material-code-braces: ConfigIdResponseTypeDef](./type_defs.md#configidresponsetypedef) 


```python
# delete_config method usage example with argument unpacking

kwargs: DeleteConfigRequestRequestTypeDef = {  # (1)
    "configId": ...,
    "configType": ...,
}

parent.delete_config(**kwargs)
```

1. See [:material-code-braces: DeleteConfigRequestRequestTypeDef](./type_defs.md#deleteconfigrequestrequesttypedef) 

### delete\_dataflow\_endpoint\_group

Deletes a dataflow endpoint group.

Type annotations and code completion for `#!python session.create_client("groundstation").delete_dataflow_endpoint_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.delete_dataflow_endpoint_group)

```python
# delete_dataflow_endpoint_group method definition

await def delete_dataflow_endpoint_group(
    self,
    *,
    dataflowEndpointGroupId: str,
) -> DataflowEndpointGroupIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DataflowEndpointGroupIdResponseTypeDef](./type_defs.md#dataflowendpointgroupidresponsetypedef) 


```python
# delete_dataflow_endpoint_group method usage example with argument unpacking

kwargs: DeleteDataflowEndpointGroupRequestRequestTypeDef = {  # (1)
    "dataflowEndpointGroupId": ...,
}

parent.delete_dataflow_endpoint_group(**kwargs)
```

1. See [:material-code-braces: DeleteDataflowEndpointGroupRequestRequestTypeDef](./type_defs.md#deletedataflowendpointgrouprequestrequesttypedef) 

### delete\_ephemeris

Deletes an ephemeris See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/groundstation-2019-05-23/DeleteEphemeris).

Type annotations and code completion for `#!python session.create_client("groundstation").delete_ephemeris` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.delete_ephemeris)

```python
# delete_ephemeris method definition

await def delete_ephemeris(
    self,
    *,
    ephemerisId: str,
) -> EphemerisIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EphemerisIdResponseTypeDef](./type_defs.md#ephemerisidresponsetypedef) 


```python
# delete_ephemeris method usage example with argument unpacking

kwargs: DeleteEphemerisRequestRequestTypeDef = {  # (1)
    "ephemerisId": ...,
}

parent.delete_ephemeris(**kwargs)
```

1. See [:material-code-braces: DeleteEphemerisRequestRequestTypeDef](./type_defs.md#deleteephemerisrequestrequesttypedef) 

### delete\_mission\_profile

Deletes a mission profile.

Type annotations and code completion for `#!python session.create_client("groundstation").delete_mission_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.delete_mission_profile)

```python
# delete_mission_profile method definition

await def delete_mission_profile(
    self,
    *,
    missionProfileId: str,
) -> MissionProfileIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: MissionProfileIdResponseTypeDef](./type_defs.md#missionprofileidresponsetypedef) 


```python
# delete_mission_profile method usage example with argument unpacking

kwargs: DeleteMissionProfileRequestRequestTypeDef = {  # (1)
    "missionProfileId": ...,
}

parent.delete_mission_profile(**kwargs)
```

1. See [:material-code-braces: DeleteMissionProfileRequestRequestTypeDef](./type_defs.md#deletemissionprofilerequestrequesttypedef) 

### describe\_contact

Describes an existing contact.

Type annotations and code completion for `#!python session.create_client("groundstation").describe_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.describe_contact)

```python
# describe_contact method definition

await def describe_contact(
    self,
    *,
    contactId: str,
) -> DescribeContactResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeContactResponseTypeDef](./type_defs.md#describecontactresponsetypedef) 


```python
# describe_contact method usage example with argument unpacking

kwargs: DescribeContactRequestRequestTypeDef = {  # (1)
    "contactId": ...,
}

parent.describe_contact(**kwargs)
```

1. See [:material-code-braces: DescribeContactRequestRequestTypeDef](./type_defs.md#describecontactrequestrequesttypedef) 

### describe\_ephemeris

Describes an existing ephemeris.

Type annotations and code completion for `#!python session.create_client("groundstation").describe_ephemeris` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.describe_ephemeris)

```python
# describe_ephemeris method definition

await def describe_ephemeris(
    self,
    *,
    ephemerisId: str,
) -> DescribeEphemerisResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEphemerisResponseTypeDef](./type_defs.md#describeephemerisresponsetypedef) 


```python
# describe_ephemeris method usage example with argument unpacking

kwargs: DescribeEphemerisRequestRequestTypeDef = {  # (1)
    "ephemerisId": ...,
}

parent.describe_ephemeris(**kwargs)
```

1. See [:material-code-braces: DescribeEphemerisRequestRequestTypeDef](./type_defs.md#describeephemerisrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("groundstation").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.generate_presigned_url)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_agent\_configuration

.

Type annotations and code completion for `#!python session.create_client("groundstation").get_agent_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_agent_configuration)

```python
# get_agent_configuration method definition

await def get_agent_configuration(
    self,
    *,
    agentId: str,
) -> GetAgentConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAgentConfigurationResponseTypeDef](./type_defs.md#getagentconfigurationresponsetypedef) 


```python
# get_agent_configuration method usage example with argument unpacking

kwargs: GetAgentConfigurationRequestRequestTypeDef = {  # (1)
    "agentId": ...,
}

parent.get_agent_configuration(**kwargs)
```

1. See [:material-code-braces: GetAgentConfigurationRequestRequestTypeDef](./type_defs.md#getagentconfigurationrequestrequesttypedef) 

### get\_config

Returns `Config` information.

Type annotations and code completion for `#!python session.create_client("groundstation").get_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_config)

```python
# get_config method definition

await def get_config(
    self,
    *,
    configId: str,
    configType: ConfigCapabilityTypeType,  # (1)
) -> GetConfigResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
2. See [:material-code-braces: GetConfigResponseTypeDef](./type_defs.md#getconfigresponsetypedef) 


```python
# get_config method usage example with argument unpacking

kwargs: GetConfigRequestRequestTypeDef = {  # (1)
    "configId": ...,
    "configType": ...,
}

parent.get_config(**kwargs)
```

1. See [:material-code-braces: GetConfigRequestRequestTypeDef](./type_defs.md#getconfigrequestrequesttypedef) 

### get\_dataflow\_endpoint\_group

Returns the dataflow endpoint group.

Type annotations and code completion for `#!python session.create_client("groundstation").get_dataflow_endpoint_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_dataflow_endpoint_group)

```python
# get_dataflow_endpoint_group method definition

await def get_dataflow_endpoint_group(
    self,
    *,
    dataflowEndpointGroupId: str,
) -> GetDataflowEndpointGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDataflowEndpointGroupResponseTypeDef](./type_defs.md#getdataflowendpointgroupresponsetypedef) 


```python
# get_dataflow_endpoint_group method usage example with argument unpacking

kwargs: GetDataflowEndpointGroupRequestRequestTypeDef = {  # (1)
    "dataflowEndpointGroupId": ...,
}

parent.get_dataflow_endpoint_group(**kwargs)
```

1. See [:material-code-braces: GetDataflowEndpointGroupRequestRequestTypeDef](./type_defs.md#getdataflowendpointgrouprequestrequesttypedef) 

### get\_minute\_usage

Returns the number of reserved minutes used by account.

Type annotations and code completion for `#!python session.create_client("groundstation").get_minute_usage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_minute_usage)

```python
# get_minute_usage method definition

await def get_minute_usage(
    self,
    *,
    month: int,
    year: int,
) -> GetMinuteUsageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMinuteUsageResponseTypeDef](./type_defs.md#getminuteusageresponsetypedef) 


```python
# get_minute_usage method usage example with argument unpacking

kwargs: GetMinuteUsageRequestRequestTypeDef = {  # (1)
    "month": ...,
    "year": ...,
}

parent.get_minute_usage(**kwargs)
```

1. See [:material-code-braces: GetMinuteUsageRequestRequestTypeDef](./type_defs.md#getminuteusagerequestrequesttypedef) 

### get\_mission\_profile

Returns a mission profile.

Type annotations and code completion for `#!python session.create_client("groundstation").get_mission_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_mission_profile)

```python
# get_mission_profile method definition

await def get_mission_profile(
    self,
    *,
    missionProfileId: str,
) -> GetMissionProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMissionProfileResponseTypeDef](./type_defs.md#getmissionprofileresponsetypedef) 


```python
# get_mission_profile method usage example with argument unpacking

kwargs: GetMissionProfileRequestRequestTypeDef = {  # (1)
    "missionProfileId": ...,
}

parent.get_mission_profile(**kwargs)
```

1. See [:material-code-braces: GetMissionProfileRequestRequestTypeDef](./type_defs.md#getmissionprofilerequestrequesttypedef) 

### get\_satellite

Returns a satellite.

Type annotations and code completion for `#!python session.create_client("groundstation").get_satellite` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.get_satellite)

```python
# get_satellite method definition

await def get_satellite(
    self,
    *,
    satelliteId: str,
) -> GetSatelliteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSatelliteResponseTypeDef](./type_defs.md#getsatelliteresponsetypedef) 


```python
# get_satellite method usage example with argument unpacking

kwargs: GetSatelliteRequestRequestTypeDef = {  # (1)
    "satelliteId": ...,
}

parent.get_satellite(**kwargs)
```

1. See [:material-code-braces: GetSatelliteRequestRequestTypeDef](./type_defs.md#getsatelliterequestrequesttypedef) 

### list\_configs

Returns a list of `Config` objects.

Type annotations and code completion for `#!python session.create_client("groundstation").list_configs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_configs)

```python
# list_configs method definition

await def list_configs(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListConfigsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListConfigsResponseTypeDef](./type_defs.md#listconfigsresponsetypedef) 


```python
# list_configs method usage example with argument unpacking

kwargs: ListConfigsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_configs(**kwargs)
```

1. See [:material-code-braces: ListConfigsRequestRequestTypeDef](./type_defs.md#listconfigsrequestrequesttypedef) 

### list\_contacts

Returns a list of contacts.

Type annotations and code completion for `#!python session.create_client("groundstation").list_contacts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_contacts)

```python
# list_contacts method definition

await def list_contacts(
    self,
    *,
    endTime: Union[datetime, str],
    startTime: Union[datetime, str],
    statusList: Sequence[ContactStatusType],  # (1)
    groundStation: str = ...,
    maxResults: int = ...,
    missionProfileArn: str = ...,
    nextToken: str = ...,
    satelliteArn: str = ...,
) -> ListContactsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContactStatusType](./literals.md#contactstatustype) 
2. See [:material-code-braces: ListContactsResponseTypeDef](./type_defs.md#listcontactsresponsetypedef) 


```python
# list_contacts method usage example with argument unpacking

kwargs: ListContactsRequestRequestTypeDef = {  # (1)
    "endTime": ...,
    "startTime": ...,
    "statusList": ...,
}

parent.list_contacts(**kwargs)
```

1. See [:material-code-braces: ListContactsRequestRequestTypeDef](./type_defs.md#listcontactsrequestrequesttypedef) 

### list\_dataflow\_endpoint\_groups

Returns a list of `DataflowEndpoint` groups.

Type annotations and code completion for `#!python session.create_client("groundstation").list_dataflow_endpoint_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_dataflow_endpoint_groups)

```python
# list_dataflow_endpoint_groups method definition

await def list_dataflow_endpoint_groups(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDataflowEndpointGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDataflowEndpointGroupsResponseTypeDef](./type_defs.md#listdataflowendpointgroupsresponsetypedef) 


```python
# list_dataflow_endpoint_groups method usage example with argument unpacking

kwargs: ListDataflowEndpointGroupsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_dataflow_endpoint_groups(**kwargs)
```

1. See [:material-code-braces: ListDataflowEndpointGroupsRequestRequestTypeDef](./type_defs.md#listdataflowendpointgroupsrequestrequesttypedef) 

### list\_ephemerides

List existing ephemerides.

Type annotations and code completion for `#!python session.create_client("groundstation").list_ephemerides` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_ephemerides)

```python
# list_ephemerides method definition

await def list_ephemerides(
    self,
    *,
    endTime: Union[datetime, str],
    satelliteId: str,
    startTime: Union[datetime, str],
    maxResults: int = ...,
    nextToken: str = ...,
    statusList: Sequence[EphemerisStatusType] = ...,  # (1)
) -> ListEphemeridesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EphemerisStatusType](./literals.md#ephemerisstatustype) 
2. See [:material-code-braces: ListEphemeridesResponseTypeDef](./type_defs.md#listephemeridesresponsetypedef) 


```python
# list_ephemerides method usage example with argument unpacking

kwargs: ListEphemeridesRequestRequestTypeDef = {  # (1)
    "endTime": ...,
    "satelliteId": ...,
    "startTime": ...,
}

parent.list_ephemerides(**kwargs)
```

1. See [:material-code-braces: ListEphemeridesRequestRequestTypeDef](./type_defs.md#listephemeridesrequestrequesttypedef) 

### list\_ground\_stations

Returns a list of ground stations.

Type annotations and code completion for `#!python session.create_client("groundstation").list_ground_stations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_ground_stations)

```python
# list_ground_stations method definition

await def list_ground_stations(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    satelliteId: str = ...,
) -> ListGroundStationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListGroundStationsResponseTypeDef](./type_defs.md#listgroundstationsresponsetypedef) 


```python
# list_ground_stations method usage example with argument unpacking

kwargs: ListGroundStationsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_ground_stations(**kwargs)
```

1. See [:material-code-braces: ListGroundStationsRequestRequestTypeDef](./type_defs.md#listgroundstationsrequestrequesttypedef) 

### list\_mission\_profiles

Returns a list of mission profiles.

Type annotations and code completion for `#!python session.create_client("groundstation").list_mission_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_mission_profiles)

```python
# list_mission_profiles method definition

await def list_mission_profiles(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListMissionProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMissionProfilesResponseTypeDef](./type_defs.md#listmissionprofilesresponsetypedef) 


```python
# list_mission_profiles method usage example with argument unpacking

kwargs: ListMissionProfilesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_mission_profiles(**kwargs)
```

1. See [:material-code-braces: ListMissionProfilesRequestRequestTypeDef](./type_defs.md#listmissionprofilesrequestrequesttypedef) 

### list\_satellites

Returns a list of satellites.

Type annotations and code completion for `#!python session.create_client("groundstation").list_satellites` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_satellites)

```python
# list_satellites method definition

await def list_satellites(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListSatellitesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSatellitesResponseTypeDef](./type_defs.md#listsatellitesresponsetypedef) 


```python
# list_satellites method usage example with argument unpacking

kwargs: ListSatellitesRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_satellites(**kwargs)
```

1. See [:material-code-braces: ListSatellitesRequestRequestTypeDef](./type_defs.md#listsatellitesrequestrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags for a specified resource.

Type annotations and code completion for `#!python session.create_client("groundstation").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### register\_agent

.

Type annotations and code completion for `#!python session.create_client("groundstation").register_agent` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.register_agent)

```python
# register_agent method definition

await def register_agent(
    self,
    *,
    agentDetails: AgentDetailsTypeDef,  # (1)
    discoveryData: DiscoveryDataTypeDef,  # (2)
) -> RegisterAgentResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AgentDetailsTypeDef](./type_defs.md#agentdetailstypedef) 
2. See [:material-code-braces: DiscoveryDataTypeDef](./type_defs.md#discoverydatatypedef) 
3. See [:material-code-braces: RegisterAgentResponseTypeDef](./type_defs.md#registeragentresponsetypedef) 


```python
# register_agent method usage example with argument unpacking

kwargs: RegisterAgentRequestRequestTypeDef = {  # (1)
    "agentDetails": ...,
    "discoveryData": ...,
}

parent.register_agent(**kwargs)
```

1. See [:material-code-braces: RegisterAgentRequestRequestTypeDef](./type_defs.md#registeragentrequestrequesttypedef) 

### reserve\_contact

Reserves a contact using specified parameters.

Type annotations and code completion for `#!python session.create_client("groundstation").reserve_contact` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.reserve_contact)

```python
# reserve_contact method definition

await def reserve_contact(
    self,
    *,
    endTime: Union[datetime, str],
    groundStation: str,
    missionProfileArn: str,
    satelliteArn: str,
    startTime: Union[datetime, str],
    tags: Mapping[str, str] = ...,
) -> ContactIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ContactIdResponseTypeDef](./type_defs.md#contactidresponsetypedef) 


```python
# reserve_contact method usage example with argument unpacking

kwargs: ReserveContactRequestRequestTypeDef = {  # (1)
    "endTime": ...,
    "groundStation": ...,
    "missionProfileArn": ...,
    "satelliteArn": ...,
    "startTime": ...,
}

parent.reserve_contact(**kwargs)
```

1. See [:material-code-braces: ReserveContactRequestRequestTypeDef](./type_defs.md#reservecontactrequestrequesttypedef) 

### tag\_resource

Assigns a tag to a resource.

Type annotations and code completion for `#!python session.create_client("groundstation").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Deassigns a resource tag.

Type annotations and code completion for `#!python session.create_client("groundstation").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_agent\_status

.

Type annotations and code completion for `#!python session.create_client("groundstation").update_agent_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_agent_status)

```python
# update_agent_status method definition

await def update_agent_status(
    self,
    *,
    agentId: str,
    aggregateStatus: AggregateStatusTypeDef,  # (1)
    componentStatuses: Sequence[ComponentStatusDataTypeDef],  # (2)
    taskId: str,
) -> UpdateAgentStatusResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AggregateStatusTypeDef](./type_defs.md#aggregatestatustypedef) 
2. See [:material-code-braces: ComponentStatusDataTypeDef](./type_defs.md#componentstatusdatatypedef) 
3. See [:material-code-braces: UpdateAgentStatusResponseTypeDef](./type_defs.md#updateagentstatusresponsetypedef) 


```python
# update_agent_status method usage example with argument unpacking

kwargs: UpdateAgentStatusRequestRequestTypeDef = {  # (1)
    "agentId": ...,
    "aggregateStatus": ...,
    "componentStatuses": ...,
    "taskId": ...,
}

parent.update_agent_status(**kwargs)
```

1. See [:material-code-braces: UpdateAgentStatusRequestRequestTypeDef](./type_defs.md#updateagentstatusrequestrequesttypedef) 

### update\_config

Updates the `Config` used when scheduling contacts.

Type annotations and code completion for `#!python session.create_client("groundstation").update_config` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_config)

```python
# update_config method definition

await def update_config(
    self,
    *,
    configData: ConfigTypeDataTypeDef,  # (1)
    configId: str,
    configType: ConfigCapabilityTypeType,  # (2)
    name: str,
) -> ConfigIdResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ConfigTypeDataTypeDef](./type_defs.md#configtypedatatypedef) 
2. See [:material-code-brackets: ConfigCapabilityTypeType](./literals.md#configcapabilitytypetype) 
3. See [:material-code-braces: ConfigIdResponseTypeDef](./type_defs.md#configidresponsetypedef) 


```python
# update_config method usage example with argument unpacking

kwargs: UpdateConfigRequestRequestTypeDef = {  # (1)
    "configData": ...,
    "configId": ...,
    "configType": ...,
    "name": ...,
}

parent.update_config(**kwargs)
```

1. See [:material-code-braces: UpdateConfigRequestRequestTypeDef](./type_defs.md#updateconfigrequestrequesttypedef) 

### update\_ephemeris

Updates an existing ephemeris See also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/groundstation-2019-05-23/UpdateEphemeris).

Type annotations and code completion for `#!python session.create_client("groundstation").update_ephemeris` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_ephemeris)

```python
# update_ephemeris method definition

await def update_ephemeris(
    self,
    *,
    enabled: bool,
    ephemerisId: str,
    name: str = ...,
    priority: int = ...,
) -> EphemerisIdResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EphemerisIdResponseTypeDef](./type_defs.md#ephemerisidresponsetypedef) 


```python
# update_ephemeris method usage example with argument unpacking

kwargs: UpdateEphemerisRequestRequestTypeDef = {  # (1)
    "enabled": ...,
    "ephemerisId": ...,
}

parent.update_ephemeris(**kwargs)
```

1. See [:material-code-braces: UpdateEphemerisRequestRequestTypeDef](./type_defs.md#updateephemerisrequestrequesttypedef) 

### update\_mission\_profile

Updates a mission profile.

Type annotations and code completion for `#!python session.create_client("groundstation").update_mission_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.update_mission_profile)

```python
# update_mission_profile method definition

await def update_mission_profile(
    self,
    *,
    missionProfileId: str,
    contactPostPassDurationSeconds: int = ...,
    contactPrePassDurationSeconds: int = ...,
    dataflowEdges: Sequence[Sequence[str]] = ...,
    minimumViableContactDurationSeconds: int = ...,
    name: str = ...,
    streamsKmsKey: KmsKeyTypeDef = ...,  # (1)
    streamsKmsRole: str = ...,
    trackingConfigArn: str = ...,
) -> MissionProfileIdResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: KmsKeyTypeDef](./type_defs.md#kmskeytypedef) 
2. See [:material-code-braces: MissionProfileIdResponseTypeDef](./type_defs.md#missionprofileidresponsetypedef) 


```python
# update_mission_profile method usage example with argument unpacking

kwargs: UpdateMissionProfileRequestRequestTypeDef = {  # (1)
    "missionProfileId": ...,
}

parent.update_mission_profile(**kwargs)
```

1. See [:material-code-braces: UpdateMissionProfileRequestRequestTypeDef](./type_defs.md#updatemissionprofilerequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("groundstation").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> GroundStationClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("groundstation").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/groundstation.html#GroundStation.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("groundstation").get_paginator` method with overloads.

- `client.get_paginator("list_configs")` -> [ListConfigsPaginator](./paginators.md#listconfigspaginator)
- `client.get_paginator("list_contacts")` -> [ListContactsPaginator](./paginators.md#listcontactspaginator)
- `client.get_paginator("list_dataflow_endpoint_groups")` -> [ListDataflowEndpointGroupsPaginator](./paginators.md#listdataflowendpointgroupspaginator)
- `client.get_paginator("list_ephemerides")` -> [ListEphemeridesPaginator](./paginators.md#listephemeridespaginator)
- `client.get_paginator("list_ground_stations")` -> [ListGroundStationsPaginator](./paginators.md#listgroundstationspaginator)
- `client.get_paginator("list_mission_profiles")` -> [ListMissionProfilesPaginator](./paginators.md#listmissionprofilespaginator)
- `client.get_paginator("list_satellites")` -> [ListSatellitesPaginator](./paginators.md#listsatellitespaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("groundstation").get_waiter` method with overloads.

- `client.get_waiter("contact_scheduled")` -> [ContactScheduledWaiter](./waiters.md#contactscheduledwaiter)


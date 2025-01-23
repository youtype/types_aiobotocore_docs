# MediaLiveClient

> [Index](../README.md) > [MediaLive](./README.md) > MediaLiveClient

!!! note ""

    Auto-generated documentation for [MediaLive](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#medialive)
    type annotations stubs module [types-aiobotocore-medialive](https://pypi.org/project/types-aiobotocore-medialive/).

## MediaLiveClient

Type annotations and code completion for `#!python session.create_client("medialive")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client)

```python
# MediaLiveClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_medialive.client import MediaLiveClient

session = get_session()
async with session.create_client("medialive") as client:
    client: MediaLiveClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("medialive").exceptions` structure.

```python
# MediaLiveClient.exceptions usage example

async with session.create_client("medialive") as client:
    try:
        do_something(client)
    except (
            client.BadGatewayException,
        client.BadRequestException,
        client.ClientError,
        client.ConflictException,
        client.ForbiddenException,
        client.GatewayTimeoutException,
        client.InternalServerErrorException,
        client.NotFoundException,
        client.TooManyRequestsException,
        client.UnprocessableEntityException,
    ) as e:
        print(e)
```

```python
# MediaLiveClient usage type checking example

from types_aiobotocore_medialive.client import Exceptions

def handle_error(exc: Exceptions.BadGatewayException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("medialive").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("medialive").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/generate_presigned_url.html)

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


### accept\_input\_device\_transfer

Accept an incoming input device transfer.

Type annotations and code completion for `#!python session.create_client("medialive").accept_input_device_transfer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/accept_input_device_transfer.html)

```python
# accept_input_device_transfer method definition

await def accept_input_device_transfer(
    self,
    *,
    InputDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# accept_input_device_transfer method usage example with argument unpacking

kwargs: AcceptInputDeviceTransferRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.accept_input_device_transfer(**kwargs)
```

1. See [:material-code-braces: AcceptInputDeviceTransferRequestRequestTypeDef](./type_defs.md#acceptinputdevicetransferrequestrequesttypedef) 

### batch\_delete

Starts delete of resources.

Type annotations and code completion for `#!python session.create_client("medialive").batch_delete` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/batch_delete.html)

```python
# batch_delete method definition

await def batch_delete(
    self,
    *,
    ChannelIds: Sequence[str] = ...,
    InputIds: Sequence[str] = ...,
    InputSecurityGroupIds: Sequence[str] = ...,
    MultiplexIds: Sequence[str] = ...,
) -> BatchDeleteResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDeleteResponseTypeDef](./type_defs.md#batchdeleteresponsetypedef) 


```python
# batch_delete method usage example with argument unpacking

kwargs: BatchDeleteRequestRequestTypeDef = {  # (1)
    "ChannelIds": ...,
}

parent.batch_delete(**kwargs)
```

1. See [:material-code-braces: BatchDeleteRequestRequestTypeDef](./type_defs.md#batchdeleterequestrequesttypedef) 

### batch\_start

Starts existing resources.

Type annotations and code completion for `#!python session.create_client("medialive").batch_start` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/batch_start.html)

```python
# batch_start method definition

await def batch_start(
    self,
    *,
    ChannelIds: Sequence[str] = ...,
    MultiplexIds: Sequence[str] = ...,
) -> BatchStartResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchStartResponseTypeDef](./type_defs.md#batchstartresponsetypedef) 


```python
# batch_start method usage example with argument unpacking

kwargs: BatchStartRequestRequestTypeDef = {  # (1)
    "ChannelIds": ...,
}

parent.batch_start(**kwargs)
```

1. See [:material-code-braces: BatchStartRequestRequestTypeDef](./type_defs.md#batchstartrequestrequesttypedef) 

### batch\_stop

Stops running resources.

Type annotations and code completion for `#!python session.create_client("medialive").batch_stop` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/batch_stop.html)

```python
# batch_stop method definition

await def batch_stop(
    self,
    *,
    ChannelIds: Sequence[str] = ...,
    MultiplexIds: Sequence[str] = ...,
) -> BatchStopResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchStopResponseTypeDef](./type_defs.md#batchstopresponsetypedef) 


```python
# batch_stop method usage example with argument unpacking

kwargs: BatchStopRequestRequestTypeDef = {  # (1)
    "ChannelIds": ...,
}

parent.batch_stop(**kwargs)
```

1. See [:material-code-braces: BatchStopRequestRequestTypeDef](./type_defs.md#batchstoprequestrequesttypedef) 

### batch\_update\_schedule

Update a channel schedule.

Type annotations and code completion for `#!python session.create_client("medialive").batch_update_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/batch_update_schedule.html)

```python
# batch_update_schedule method definition

await def batch_update_schedule(
    self,
    *,
    ChannelId: str,
    Creates: BatchScheduleActionCreateRequestTypeDef = ...,  # (1)
    Deletes: BatchScheduleActionDeleteRequestTypeDef = ...,  # (2)
) -> BatchUpdateScheduleResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: BatchScheduleActionCreateRequestTypeDef](./type_defs.md#batchscheduleactioncreaterequesttypedef) 
2. See [:material-code-braces: BatchScheduleActionDeleteRequestTypeDef](./type_defs.md#batchscheduleactiondeleterequesttypedef) 
3. See [:material-code-braces: BatchUpdateScheduleResponseTypeDef](./type_defs.md#batchupdatescheduleresponsetypedef) 


```python
# batch_update_schedule method usage example with argument unpacking

kwargs: BatchUpdateScheduleRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.batch_update_schedule(**kwargs)
```

1. See [:material-code-braces: BatchUpdateScheduleRequestRequestTypeDef](./type_defs.md#batchupdateschedulerequestrequesttypedef) 

### cancel\_input\_device\_transfer

Cancel an input device transfer that you have requested.

Type annotations and code completion for `#!python session.create_client("medialive").cancel_input_device_transfer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/cancel_input_device_transfer.html)

```python
# cancel_input_device_transfer method definition

await def cancel_input_device_transfer(
    self,
    *,
    InputDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_input_device_transfer method usage example with argument unpacking

kwargs: CancelInputDeviceTransferRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.cancel_input_device_transfer(**kwargs)
```

1. See [:material-code-braces: CancelInputDeviceTransferRequestRequestTypeDef](./type_defs.md#cancelinputdevicetransferrequestrequesttypedef) 

### claim\_device

Send a request to claim an AWS Elemental device that you have purchased from a
third-party vendor.

Type annotations and code completion for `#!python session.create_client("medialive").claim_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/claim_device.html)

```python
# claim_device method definition

await def claim_device(
    self,
    *,
    Id: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# claim_device method usage example with argument unpacking

kwargs: ClaimDeviceRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.claim_device(**kwargs)
```

1. See [:material-code-braces: ClaimDeviceRequestRequestTypeDef](./type_defs.md#claimdevicerequestrequesttypedef) 

### create\_channel

Creates a new channel.

Type annotations and code completion for `#!python session.create_client("medialive").create_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_channel.html)

```python
# create_channel method definition

await def create_channel(
    self,
    *,
    CdiInputSpecification: CdiInputSpecificationTypeDef = ...,  # (1)
    ChannelClass: ChannelClassType = ...,  # (2)
    Destinations: Sequence[OutputDestinationUnionTypeDef] = ...,  # (3)
    EncoderSettings: EncoderSettingsTypeDef = ...,  # (4)
    InputAttachments: Sequence[InputAttachmentUnionTypeDef] = ...,  # (5)
    InputSpecification: InputSpecificationTypeDef = ...,  # (6)
    LogLevel: LogLevelType = ...,  # (7)
    Maintenance: MaintenanceCreateSettingsTypeDef = ...,  # (8)
    Name: str = ...,
    RequestId: str = ...,
    Reserved: str = ...,
    RoleArn: str = ...,
    Tags: Mapping[str, str] = ...,
    Vpc: VpcOutputSettingsTypeDef = ...,  # (9)
    AnywhereSettings: AnywhereSettingsTypeDef = ...,  # (10)
    ChannelEngineVersion: ChannelEngineVersionRequestTypeDef = ...,  # (11)
    DryRun: bool = ...,
) -> CreateChannelResponseTypeDef:  # (12)
    ...
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
3. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) [:material-code-braces: OutputDestinationOutputTypeDef](./type_defs.md#outputdestinationoutputtypedef) 
4. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
5. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) [:material-code-braces: InputAttachmentOutputTypeDef](./type_defs.md#inputattachmentoutputtypedef) 
6. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
7. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
8. See [:material-code-braces: MaintenanceCreateSettingsTypeDef](./type_defs.md#maintenancecreatesettingstypedef) 
9. See [:material-code-braces: VpcOutputSettingsTypeDef](./type_defs.md#vpcoutputsettingstypedef) 
10. See [:material-code-braces: AnywhereSettingsTypeDef](./type_defs.md#anywheresettingstypedef) 
11. See [:material-code-braces: ChannelEngineVersionRequestTypeDef](./type_defs.md#channelengineversionrequesttypedef) 
12. See [:material-code-braces: CreateChannelResponseTypeDef](./type_defs.md#createchannelresponsetypedef) 


```python
# create_channel method usage example with argument unpacking

kwargs: CreateChannelRequestRequestTypeDef = {  # (1)
    "CdiInputSpecification": ...,
}

parent.create_channel(**kwargs)
```

1. See [:material-code-braces: CreateChannelRequestRequestTypeDef](./type_defs.md#createchannelrequestrequesttypedef) 

### create\_input

Create an input.

Type annotations and code completion for `#!python session.create_client("medialive").create_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_input.html)

```python
# create_input method definition

await def create_input(
    self,
    *,
    Destinations: Sequence[InputDestinationRequestTypeDef] = ...,  # (1)
    InputDevices: Sequence[InputDeviceSettingsTypeDef] = ...,  # (2)
    InputSecurityGroups: Sequence[str] = ...,
    MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,  # (3)
    Name: str = ...,
    RequestId: str = ...,
    RoleArn: str = ...,
    Sources: Sequence[InputSourceRequestTypeDef] = ...,  # (4)
    Tags: Mapping[str, str] = ...,
    Type: InputTypeType = ...,  # (5)
    Vpc: InputVpcRequestTypeDef = ...,  # (6)
    SrtSettings: SrtSettingsRequestTypeDef = ...,  # (7)
    InputNetworkLocation: InputNetworkLocationType = ...,  # (8)
    MulticastSettings: MulticastSettingsCreateRequestTypeDef = ...,  # (9)
) -> CreateInputResponseTypeDef:  # (10)
    ...
```

1. See [:material-code-braces: InputDestinationRequestTypeDef](./type_defs.md#inputdestinationrequesttypedef) 
2. See [:material-code-braces: InputDeviceSettingsTypeDef](./type_defs.md#inputdevicesettingstypedef) 
3. See [:material-code-braces: MediaConnectFlowRequestTypeDef](./type_defs.md#mediaconnectflowrequesttypedef) 
4. See [:material-code-braces: InputSourceRequestTypeDef](./type_defs.md#inputsourcerequesttypedef) 
5. See [:material-code-brackets: InputTypeType](./literals.md#inputtypetype) 
6. See [:material-code-braces: InputVpcRequestTypeDef](./type_defs.md#inputvpcrequesttypedef) 
7. See [:material-code-braces: SrtSettingsRequestTypeDef](./type_defs.md#srtsettingsrequesttypedef) 
8. See [:material-code-brackets: InputNetworkLocationType](./literals.md#inputnetworklocationtype) 
9. See [:material-code-braces: MulticastSettingsCreateRequestTypeDef](./type_defs.md#multicastsettingscreaterequesttypedef) 
10. See [:material-code-braces: CreateInputResponseTypeDef](./type_defs.md#createinputresponsetypedef) 


```python
# create_input method usage example with argument unpacking

kwargs: CreateInputRequestRequestTypeDef = {  # (1)
    "Destinations": ...,
}

parent.create_input(**kwargs)
```

1. See [:material-code-braces: CreateInputRequestRequestTypeDef](./type_defs.md#createinputrequestrequesttypedef) 

### create\_input\_security\_group

Creates a Input Security Group.

Type annotations and code completion for `#!python session.create_client("medialive").create_input_security_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_input_security_group.html)

```python
# create_input_security_group method definition

await def create_input_security_group(
    self,
    *,
    Tags: Mapping[str, str] = ...,
    WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...,  # (1)
) -> CreateInputSecurityGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InputWhitelistRuleCidrTypeDef](./type_defs.md#inputwhitelistrulecidrtypedef) 
2. See [:material-code-braces: CreateInputSecurityGroupResponseTypeDef](./type_defs.md#createinputsecuritygroupresponsetypedef) 


```python
# create_input_security_group method usage example with argument unpacking

kwargs: CreateInputSecurityGroupRequestRequestTypeDef = {  # (1)
    "Tags": ...,
}

parent.create_input_security_group(**kwargs)
```

1. See [:material-code-braces: CreateInputSecurityGroupRequestRequestTypeDef](./type_defs.md#createinputsecuritygrouprequestrequesttypedef) 

### create\_multiplex

Create a new multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").create_multiplex` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_multiplex.html)

```python
# create_multiplex method definition

await def create_multiplex(
    self,
    *,
    AvailabilityZones: Sequence[str],
    MultiplexSettings: MultiplexSettingsTypeDef,  # (1)
    Name: str,
    RequestId: str,
    Tags: Mapping[str, str] = ...,
) -> CreateMultiplexResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
2. See [:material-code-braces: CreateMultiplexResponseTypeDef](./type_defs.md#createmultiplexresponsetypedef) 


```python
# create_multiplex method usage example with argument unpacking

kwargs: CreateMultiplexRequestRequestTypeDef = {  # (1)
    "AvailabilityZones": ...,
    "MultiplexSettings": ...,
    "Name": ...,
    "RequestId": ...,
}

parent.create_multiplex(**kwargs)
```

1. See [:material-code-braces: CreateMultiplexRequestRequestTypeDef](./type_defs.md#createmultiplexrequestrequesttypedef) 

### create\_multiplex\_program

Create a new program in the multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").create_multiplex_program` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_multiplex_program.html)

```python
# create_multiplex_program method definition

await def create_multiplex_program(
    self,
    *,
    MultiplexId: str,
    MultiplexProgramSettings: MultiplexProgramSettingsTypeDef,  # (1)
    ProgramName: str,
    RequestId: str,
) -> CreateMultiplexProgramResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MultiplexProgramSettingsTypeDef](./type_defs.md#multiplexprogramsettingstypedef) 
2. See [:material-code-braces: CreateMultiplexProgramResponseTypeDef](./type_defs.md#createmultiplexprogramresponsetypedef) 


```python
# create_multiplex_program method usage example with argument unpacking

kwargs: CreateMultiplexProgramRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
    "MultiplexProgramSettings": ...,
    "ProgramName": ...,
    "RequestId": ...,
}

parent.create_multiplex_program(**kwargs)
```

1. See [:material-code-braces: CreateMultiplexProgramRequestRequestTypeDef](./type_defs.md#createmultiplexprogramrequestrequesttypedef) 

### create\_partner\_input

Create a partner input.

Type annotations and code completion for `#!python session.create_client("medialive").create_partner_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_partner_input.html)

```python
# create_partner_input method definition

await def create_partner_input(
    self,
    *,
    InputId: str,
    RequestId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreatePartnerInputResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreatePartnerInputResponseTypeDef](./type_defs.md#createpartnerinputresponsetypedef) 


```python
# create_partner_input method usage example with argument unpacking

kwargs: CreatePartnerInputRequestRequestTypeDef = {  # (1)
    "InputId": ...,
}

parent.create_partner_input(**kwargs)
```

1. See [:material-code-braces: CreatePartnerInputRequestRequestTypeDef](./type_defs.md#createpartnerinputrequestrequesttypedef) 

### create\_tags

Create tags for a resource.

Type annotations and code completion for `#!python session.create_client("medialive").create_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_tags.html)

```python
# create_tags method definition

await def create_tags(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str] = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# create_tags method usage example with argument unpacking

kwargs: CreateTagsRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.create_tags(**kwargs)
```

1. See [:material-code-braces: CreateTagsRequestRequestTypeDef](./type_defs.md#createtagsrequestrequesttypedef) 

### delete\_channel

Starts deletion of channel.

Type annotations and code completion for `#!python session.create_client("medialive").delete_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_channel.html)

```python
# delete_channel method definition

await def delete_channel(
    self,
    *,
    ChannelId: str,
) -> DeleteChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteChannelResponseTypeDef](./type_defs.md#deletechannelresponsetypedef) 


```python
# delete_channel method usage example with argument unpacking

kwargs: DeleteChannelRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.delete_channel(**kwargs)
```

1. See [:material-code-braces: DeleteChannelRequestRequestTypeDef](./type_defs.md#deletechannelrequestrequesttypedef) 

### delete\_input

Deletes the input end point.

Type annotations and code completion for `#!python session.create_client("medialive").delete_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_input.html)

```python
# delete_input method definition

await def delete_input(
    self,
    *,
    InputId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_input method usage example with argument unpacking

kwargs: DeleteInputRequestRequestTypeDef = {  # (1)
    "InputId": ...,
}

parent.delete_input(**kwargs)
```

1. See [:material-code-braces: DeleteInputRequestRequestTypeDef](./type_defs.md#deleteinputrequestrequesttypedef) 

### delete\_input\_security\_group

Deletes an Input Security Group.

Type annotations and code completion for `#!python session.create_client("medialive").delete_input_security_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_input_security_group.html)

```python
# delete_input_security_group method definition

await def delete_input_security_group(
    self,
    *,
    InputSecurityGroupId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_input_security_group method usage example with argument unpacking

kwargs: DeleteInputSecurityGroupRequestRequestTypeDef = {  # (1)
    "InputSecurityGroupId": ...,
}

parent.delete_input_security_group(**kwargs)
```

1. See [:material-code-braces: DeleteInputSecurityGroupRequestRequestTypeDef](./type_defs.md#deleteinputsecuritygrouprequestrequesttypedef) 

### delete\_multiplex

Delete a multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").delete_multiplex` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_multiplex.html)

```python
# delete_multiplex method definition

await def delete_multiplex(
    self,
    *,
    MultiplexId: str,
) -> DeleteMultiplexResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMultiplexResponseTypeDef](./type_defs.md#deletemultiplexresponsetypedef) 


```python
# delete_multiplex method usage example with argument unpacking

kwargs: DeleteMultiplexRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.delete_multiplex(**kwargs)
```

1. See [:material-code-braces: DeleteMultiplexRequestRequestTypeDef](./type_defs.md#deletemultiplexrequestrequesttypedef) 

### delete\_multiplex\_program

Delete a program from a multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").delete_multiplex_program` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_multiplex_program.html)

```python
# delete_multiplex_program method definition

await def delete_multiplex_program(
    self,
    *,
    MultiplexId: str,
    ProgramName: str,
) -> DeleteMultiplexProgramResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteMultiplexProgramResponseTypeDef](./type_defs.md#deletemultiplexprogramresponsetypedef) 


```python
# delete_multiplex_program method usage example with argument unpacking

kwargs: DeleteMultiplexProgramRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
    "ProgramName": ...,
}

parent.delete_multiplex_program(**kwargs)
```

1. See [:material-code-braces: DeleteMultiplexProgramRequestRequestTypeDef](./type_defs.md#deletemultiplexprogramrequestrequesttypedef) 

### delete\_reservation

Delete an expired reservation.

Type annotations and code completion for `#!python session.create_client("medialive").delete_reservation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_reservation.html)

```python
# delete_reservation method definition

await def delete_reservation(
    self,
    *,
    ReservationId: str,
) -> DeleteReservationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteReservationResponseTypeDef](./type_defs.md#deletereservationresponsetypedef) 


```python
# delete_reservation method usage example with argument unpacking

kwargs: DeleteReservationRequestRequestTypeDef = {  # (1)
    "ReservationId": ...,
}

parent.delete_reservation(**kwargs)
```

1. See [:material-code-braces: DeleteReservationRequestRequestTypeDef](./type_defs.md#deletereservationrequestrequesttypedef) 

### delete\_schedule

Delete all schedule actions on a channel.

Type annotations and code completion for `#!python session.create_client("medialive").delete_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_schedule.html)

```python
# delete_schedule method definition

await def delete_schedule(
    self,
    *,
    ChannelId: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_schedule method usage example with argument unpacking

kwargs: DeleteScheduleRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.delete_schedule(**kwargs)
```

1. See [:material-code-braces: DeleteScheduleRequestRequestTypeDef](./type_defs.md#deleteschedulerequestrequesttypedef) 

### delete\_tags

Removes tags for a resource.

Type annotations and code completion for `#!python session.create_client("medialive").delete_tags` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_tags.html)

```python
# delete_tags method definition

await def delete_tags(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_tags method usage example with argument unpacking

kwargs: DeleteTagsRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.delete_tags(**kwargs)
```

1. See [:material-code-braces: DeleteTagsRequestRequestTypeDef](./type_defs.md#deletetagsrequestrequesttypedef) 

### describe\_account\_configuration

Describe account configuration.

Type annotations and code completion for `#!python session.create_client("medialive").describe_account_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_account_configuration.html)

```python
# describe_account_configuration method definition

await def describe_account_configuration(
    self,
) -> DescribeAccountConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAccountConfigurationResponseTypeDef](./type_defs.md#describeaccountconfigurationresponsetypedef) 

### describe\_channel

Gets details about a channel.

Type annotations and code completion for `#!python session.create_client("medialive").describe_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_channel.html)

```python
# describe_channel method definition

await def describe_channel(
    self,
    *,
    ChannelId: str,
) -> DescribeChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelResponseTypeDef](./type_defs.md#describechannelresponsetypedef) 


```python
# describe_channel method usage example with argument unpacking

kwargs: DescribeChannelRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.describe_channel(**kwargs)
```

1. See [:material-code-braces: DescribeChannelRequestRequestTypeDef](./type_defs.md#describechannelrequestrequesttypedef) 

### describe\_input

Produces details about an input.

Type annotations and code completion for `#!python session.create_client("medialive").describe_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_input.html)

```python
# describe_input method definition

await def describe_input(
    self,
    *,
    InputId: str,
) -> DescribeInputResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInputResponseTypeDef](./type_defs.md#describeinputresponsetypedef) 


```python
# describe_input method usage example with argument unpacking

kwargs: DescribeInputRequestRequestTypeDef = {  # (1)
    "InputId": ...,
}

parent.describe_input(**kwargs)
```

1. See [:material-code-braces: DescribeInputRequestRequestTypeDef](./type_defs.md#describeinputrequestrequesttypedef) 

### describe\_input\_device

Gets the details for the input device.

Type annotations and code completion for `#!python session.create_client("medialive").describe_input_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_input_device.html)

```python
# describe_input_device method definition

await def describe_input_device(
    self,
    *,
    InputDeviceId: str,
) -> DescribeInputDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInputDeviceResponseTypeDef](./type_defs.md#describeinputdeviceresponsetypedef) 


```python
# describe_input_device method usage example with argument unpacking

kwargs: DescribeInputDeviceRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.describe_input_device(**kwargs)
```

1. See [:material-code-braces: DescribeInputDeviceRequestRequestTypeDef](./type_defs.md#describeinputdevicerequestrequesttypedef) 

### describe\_input\_device\_thumbnail

Get the latest thumbnail data for the input device.

Type annotations and code completion for `#!python session.create_client("medialive").describe_input_device_thumbnail` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_input_device_thumbnail.html)

```python
# describe_input_device_thumbnail method definition

await def describe_input_device_thumbnail(
    self,
    *,
    InputDeviceId: str,
    Accept: AcceptHeaderType,  # (1)
) -> DescribeInputDeviceThumbnailResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: AcceptHeaderType](./literals.md#acceptheadertype) 
2. See [:material-code-braces: DescribeInputDeviceThumbnailResponseTypeDef](./type_defs.md#describeinputdevicethumbnailresponsetypedef) 


```python
# describe_input_device_thumbnail method usage example with argument unpacking

kwargs: DescribeInputDeviceThumbnailRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
    "Accept": ...,
}

parent.describe_input_device_thumbnail(**kwargs)
```

1. See [:material-code-braces: DescribeInputDeviceThumbnailRequestRequestTypeDef](./type_defs.md#describeinputdevicethumbnailrequestrequesttypedef) 

### describe\_input\_security\_group

Produces a summary of an Input Security Group.

Type annotations and code completion for `#!python session.create_client("medialive").describe_input_security_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_input_security_group.html)

```python
# describe_input_security_group method definition

await def describe_input_security_group(
    self,
    *,
    InputSecurityGroupId: str,
) -> DescribeInputSecurityGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeInputSecurityGroupResponseTypeDef](./type_defs.md#describeinputsecuritygroupresponsetypedef) 


```python
# describe_input_security_group method usage example with argument unpacking

kwargs: DescribeInputSecurityGroupRequestRequestTypeDef = {  # (1)
    "InputSecurityGroupId": ...,
}

parent.describe_input_security_group(**kwargs)
```

1. See [:material-code-braces: DescribeInputSecurityGroupRequestRequestTypeDef](./type_defs.md#describeinputsecuritygrouprequestrequesttypedef) 

### describe\_multiplex

Gets details about a multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").describe_multiplex` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_multiplex.html)

```python
# describe_multiplex method definition

await def describe_multiplex(
    self,
    *,
    MultiplexId: str,
) -> DescribeMultiplexResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMultiplexResponseTypeDef](./type_defs.md#describemultiplexresponsetypedef) 


```python
# describe_multiplex method usage example with argument unpacking

kwargs: DescribeMultiplexRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.describe_multiplex(**kwargs)
```

1. See [:material-code-braces: DescribeMultiplexRequestRequestTypeDef](./type_defs.md#describemultiplexrequestrequesttypedef) 

### describe\_multiplex\_program

Get the details for a program in a multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").describe_multiplex_program` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_multiplex_program.html)

```python
# describe_multiplex_program method definition

await def describe_multiplex_program(
    self,
    *,
    MultiplexId: str,
    ProgramName: str,
) -> DescribeMultiplexProgramResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeMultiplexProgramResponseTypeDef](./type_defs.md#describemultiplexprogramresponsetypedef) 


```python
# describe_multiplex_program method usage example with argument unpacking

kwargs: DescribeMultiplexProgramRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
    "ProgramName": ...,
}

parent.describe_multiplex_program(**kwargs)
```

1. See [:material-code-braces: DescribeMultiplexProgramRequestRequestTypeDef](./type_defs.md#describemultiplexprogramrequestrequesttypedef) 

### describe\_offering

Get details for an offering.

Type annotations and code completion for `#!python session.create_client("medialive").describe_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_offering.html)

```python
# describe_offering method definition

await def describe_offering(
    self,
    *,
    OfferingId: str,
) -> DescribeOfferingResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOfferingResponseTypeDef](./type_defs.md#describeofferingresponsetypedef) 


```python
# describe_offering method usage example with argument unpacking

kwargs: DescribeOfferingRequestRequestTypeDef = {  # (1)
    "OfferingId": ...,
}

parent.describe_offering(**kwargs)
```

1. See [:material-code-braces: DescribeOfferingRequestRequestTypeDef](./type_defs.md#describeofferingrequestrequesttypedef) 

### describe\_reservation

Get details for a reservation.

Type annotations and code completion for `#!python session.create_client("medialive").describe_reservation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_reservation.html)

```python
# describe_reservation method definition

await def describe_reservation(
    self,
    *,
    ReservationId: str,
) -> DescribeReservationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeReservationResponseTypeDef](./type_defs.md#describereservationresponsetypedef) 


```python
# describe_reservation method usage example with argument unpacking

kwargs: DescribeReservationRequestRequestTypeDef = {  # (1)
    "ReservationId": ...,
}

parent.describe_reservation(**kwargs)
```

1. See [:material-code-braces: DescribeReservationRequestRequestTypeDef](./type_defs.md#describereservationrequestrequesttypedef) 

### describe\_schedule

Get a channel schedule.

Type annotations and code completion for `#!python session.create_client("medialive").describe_schedule` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_schedule.html)

```python
# describe_schedule method definition

await def describe_schedule(
    self,
    *,
    ChannelId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> DescribeScheduleResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeScheduleResponseTypeDef](./type_defs.md#describescheduleresponsetypedef) 


```python
# describe_schedule method usage example with argument unpacking

kwargs: DescribeScheduleRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.describe_schedule(**kwargs)
```

1. See [:material-code-braces: DescribeScheduleRequestRequestTypeDef](./type_defs.md#describeschedulerequestrequesttypedef) 

### describe\_thumbnails

Describe the latest thumbnails data.

Type annotations and code completion for `#!python session.create_client("medialive").describe_thumbnails` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_thumbnails.html)

```python
# describe_thumbnails method definition

await def describe_thumbnails(
    self,
    *,
    ChannelId: str,
    PipelineId: str,
    ThumbnailType: str,
) -> DescribeThumbnailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeThumbnailsResponseTypeDef](./type_defs.md#describethumbnailsresponsetypedef) 


```python
# describe_thumbnails method usage example with argument unpacking

kwargs: DescribeThumbnailsRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
    "PipelineId": ...,
    "ThumbnailType": ...,
}

parent.describe_thumbnails(**kwargs)
```

1. See [:material-code-braces: DescribeThumbnailsRequestRequestTypeDef](./type_defs.md#describethumbnailsrequestrequesttypedef) 

### list\_channels

Produces list of channels that have been created.

Type annotations and code completion for `#!python session.create_client("medialive").list_channels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_channels.html)

```python
# list_channels method definition

await def list_channels(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelsResponseTypeDef](./type_defs.md#listchannelsresponsetypedef) 


```python
# list_channels method usage example with argument unpacking

kwargs: ListChannelsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_channels(**kwargs)
```

1. See [:material-code-braces: ListChannelsRequestRequestTypeDef](./type_defs.md#listchannelsrequestrequesttypedef) 

### list\_input\_device\_transfers

List input devices that are currently being transferred.

Type annotations and code completion for `#!python session.create_client("medialive").list_input_device_transfers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_input_device_transfers.html)

```python
# list_input_device_transfers method definition

await def list_input_device_transfers(
    self,
    *,
    TransferType: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListInputDeviceTransfersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInputDeviceTransfersResponseTypeDef](./type_defs.md#listinputdevicetransfersresponsetypedef) 


```python
# list_input_device_transfers method usage example with argument unpacking

kwargs: ListInputDeviceTransfersRequestRequestTypeDef = {  # (1)
    "TransferType": ...,
}

parent.list_input_device_transfers(**kwargs)
```

1. See [:material-code-braces: ListInputDeviceTransfersRequestRequestTypeDef](./type_defs.md#listinputdevicetransfersrequestrequesttypedef) 

### list\_input\_devices

List input devices.

Type annotations and code completion for `#!python session.create_client("medialive").list_input_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_input_devices.html)

```python
# list_input_devices method definition

await def list_input_devices(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListInputDevicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInputDevicesResponseTypeDef](./type_defs.md#listinputdevicesresponsetypedef) 


```python
# list_input_devices method usage example with argument unpacking

kwargs: ListInputDevicesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_input_devices(**kwargs)
```

1. See [:material-code-braces: ListInputDevicesRequestRequestTypeDef](./type_defs.md#listinputdevicesrequestrequesttypedef) 

### list\_input\_security\_groups

Produces a list of Input Security Groups for an account.

Type annotations and code completion for `#!python session.create_client("medialive").list_input_security_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_input_security_groups.html)

```python
# list_input_security_groups method definition

await def list_input_security_groups(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListInputSecurityGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInputSecurityGroupsResponseTypeDef](./type_defs.md#listinputsecuritygroupsresponsetypedef) 


```python
# list_input_security_groups method usage example with argument unpacking

kwargs: ListInputSecurityGroupsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_input_security_groups(**kwargs)
```

1. See [:material-code-braces: ListInputSecurityGroupsRequestRequestTypeDef](./type_defs.md#listinputsecuritygroupsrequestrequesttypedef) 

### list\_inputs

Produces list of inputs that have been created.

Type annotations and code completion for `#!python session.create_client("medialive").list_inputs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_inputs.html)

```python
# list_inputs method definition

await def list_inputs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListInputsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListInputsResponseTypeDef](./type_defs.md#listinputsresponsetypedef) 


```python
# list_inputs method usage example with argument unpacking

kwargs: ListInputsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_inputs(**kwargs)
```

1. See [:material-code-braces: ListInputsRequestRequestTypeDef](./type_defs.md#listinputsrequestrequesttypedef) 

### list\_multiplex\_programs

List the programs that currently exist for a specific multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").list_multiplex_programs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_multiplex_programs.html)

```python
# list_multiplex_programs method definition

await def list_multiplex_programs(
    self,
    *,
    MultiplexId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListMultiplexProgramsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMultiplexProgramsResponseTypeDef](./type_defs.md#listmultiplexprogramsresponsetypedef) 


```python
# list_multiplex_programs method usage example with argument unpacking

kwargs: ListMultiplexProgramsRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.list_multiplex_programs(**kwargs)
```

1. See [:material-code-braces: ListMultiplexProgramsRequestRequestTypeDef](./type_defs.md#listmultiplexprogramsrequestrequesttypedef) 

### list\_multiplexes

Retrieve a list of the existing multiplexes.

Type annotations and code completion for `#!python session.create_client("medialive").list_multiplexes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_multiplexes.html)

```python
# list_multiplexes method definition

await def list_multiplexes(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListMultiplexesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMultiplexesResponseTypeDef](./type_defs.md#listmultiplexesresponsetypedef) 


```python
# list_multiplexes method usage example with argument unpacking

kwargs: ListMultiplexesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_multiplexes(**kwargs)
```

1. See [:material-code-braces: ListMultiplexesRequestRequestTypeDef](./type_defs.md#listmultiplexesrequestrequesttypedef) 

### list\_offerings

List offerings available for purchase.

Type annotations and code completion for `#!python session.create_client("medialive").list_offerings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_offerings.html)

```python
# list_offerings method definition

await def list_offerings(
    self,
    *,
    ChannelClass: str = ...,
    ChannelConfiguration: str = ...,
    Codec: str = ...,
    Duration: str = ...,
    MaxResults: int = ...,
    MaximumBitrate: str = ...,
    MaximumFramerate: str = ...,
    NextToken: str = ...,
    Resolution: str = ...,
    ResourceType: str = ...,
    SpecialFeature: str = ...,
    VideoQuality: str = ...,
) -> ListOfferingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListOfferingsResponseTypeDef](./type_defs.md#listofferingsresponsetypedef) 


```python
# list_offerings method usage example with argument unpacking

kwargs: ListOfferingsRequestRequestTypeDef = {  # (1)
    "ChannelClass": ...,
}

parent.list_offerings(**kwargs)
```

1. See [:material-code-braces: ListOfferingsRequestRequestTypeDef](./type_defs.md#listofferingsrequestrequesttypedef) 

### list\_reservations

List purchased reservations.

Type annotations and code completion for `#!python session.create_client("medialive").list_reservations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_reservations.html)

```python
# list_reservations method definition

await def list_reservations(
    self,
    *,
    ChannelClass: str = ...,
    Codec: str = ...,
    MaxResults: int = ...,
    MaximumBitrate: str = ...,
    MaximumFramerate: str = ...,
    NextToken: str = ...,
    Resolution: str = ...,
    ResourceType: str = ...,
    SpecialFeature: str = ...,
    VideoQuality: str = ...,
) -> ListReservationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListReservationsResponseTypeDef](./type_defs.md#listreservationsresponsetypedef) 


```python
# list_reservations method usage example with argument unpacking

kwargs: ListReservationsRequestRequestTypeDef = {  # (1)
    "ChannelClass": ...,
}

parent.list_reservations(**kwargs)
```

1. See [:material-code-braces: ListReservationsRequestRequestTypeDef](./type_defs.md#listreservationsrequestrequesttypedef) 

### list\_tags\_for\_resource

Produces list of tags that have been created for a resource.

Type annotations and code completion for `#!python session.create_client("medialive").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### purchase\_offering

Purchase an offering and create a reservation.

Type annotations and code completion for `#!python session.create_client("medialive").purchase_offering` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/purchase_offering.html)

```python
# purchase_offering method definition

await def purchase_offering(
    self,
    *,
    Count: int,
    OfferingId: str,
    Name: str = ...,
    RenewalSettings: RenewalSettingsTypeDef = ...,  # (1)
    RequestId: str = ...,
    Start: str = ...,
    Tags: Mapping[str, str] = ...,
) -> PurchaseOfferingResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RenewalSettingsTypeDef](./type_defs.md#renewalsettingstypedef) 
2. See [:material-code-braces: PurchaseOfferingResponseTypeDef](./type_defs.md#purchaseofferingresponsetypedef) 


```python
# purchase_offering method usage example with argument unpacking

kwargs: PurchaseOfferingRequestRequestTypeDef = {  # (1)
    "Count": ...,
    "OfferingId": ...,
}

parent.purchase_offering(**kwargs)
```

1. See [:material-code-braces: PurchaseOfferingRequestRequestTypeDef](./type_defs.md#purchaseofferingrequestrequesttypedef) 

### reboot\_input\_device

Send a reboot command to the specified input device.

Type annotations and code completion for `#!python session.create_client("medialive").reboot_input_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/reboot_input_device.html)

```python
# reboot_input_device method definition

await def reboot_input_device(
    self,
    *,
    InputDeviceId: str,
    Force: RebootInputDeviceForceType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: RebootInputDeviceForceType](./literals.md#rebootinputdeviceforcetype) 


```python
# reboot_input_device method usage example with argument unpacking

kwargs: RebootInputDeviceRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.reboot_input_device(**kwargs)
```

1. See [:material-code-braces: RebootInputDeviceRequestRequestTypeDef](./type_defs.md#rebootinputdevicerequestrequesttypedef) 

### reject\_input\_device\_transfer

Reject the transfer of the specified input device to your AWS account.

Type annotations and code completion for `#!python session.create_client("medialive").reject_input_device_transfer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/reject_input_device_transfer.html)

```python
# reject_input_device_transfer method definition

await def reject_input_device_transfer(
    self,
    *,
    InputDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# reject_input_device_transfer method usage example with argument unpacking

kwargs: RejectInputDeviceTransferRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.reject_input_device_transfer(**kwargs)
```

1. See [:material-code-braces: RejectInputDeviceTransferRequestRequestTypeDef](./type_defs.md#rejectinputdevicetransferrequestrequesttypedef) 

### start\_channel

Starts an existing channel.

Type annotations and code completion for `#!python session.create_client("medialive").start_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/start_channel.html)

```python
# start_channel method definition

await def start_channel(
    self,
    *,
    ChannelId: str,
) -> StartChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartChannelResponseTypeDef](./type_defs.md#startchannelresponsetypedef) 


```python
# start_channel method usage example with argument unpacking

kwargs: StartChannelRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.start_channel(**kwargs)
```

1. See [:material-code-braces: StartChannelRequestRequestTypeDef](./type_defs.md#startchannelrequestrequesttypedef) 

### start\_input\_device

Start an input device that is attached to a MediaConnect flow.

Type annotations and code completion for `#!python session.create_client("medialive").start_input_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/start_input_device.html)

```python
# start_input_device method definition

await def start_input_device(
    self,
    *,
    InputDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_input_device method usage example with argument unpacking

kwargs: StartInputDeviceRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.start_input_device(**kwargs)
```

1. See [:material-code-braces: StartInputDeviceRequestRequestTypeDef](./type_defs.md#startinputdevicerequestrequesttypedef) 

### start\_input\_device\_maintenance\_window

Start a maintenance window for the specified input device.

Type annotations and code completion for `#!python session.create_client("medialive").start_input_device_maintenance_window` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/start_input_device_maintenance_window.html)

```python
# start_input_device_maintenance_window method definition

await def start_input_device_maintenance_window(
    self,
    *,
    InputDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# start_input_device_maintenance_window method usage example with argument unpacking

kwargs: StartInputDeviceMaintenanceWindowRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.start_input_device_maintenance_window(**kwargs)
```

1. See [:material-code-braces: StartInputDeviceMaintenanceWindowRequestRequestTypeDef](./type_defs.md#startinputdevicemaintenancewindowrequestrequesttypedef) 

### start\_multiplex

Start (run) the multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").start_multiplex` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/start_multiplex.html)

```python
# start_multiplex method definition

await def start_multiplex(
    self,
    *,
    MultiplexId: str,
) -> StartMultiplexResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMultiplexResponseTypeDef](./type_defs.md#startmultiplexresponsetypedef) 


```python
# start_multiplex method usage example with argument unpacking

kwargs: StartMultiplexRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.start_multiplex(**kwargs)
```

1. See [:material-code-braces: StartMultiplexRequestRequestTypeDef](./type_defs.md#startmultiplexrequestrequesttypedef) 

### stop\_channel

Stops a running channel.

Type annotations and code completion for `#!python session.create_client("medialive").stop_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/stop_channel.html)

```python
# stop_channel method definition

await def stop_channel(
    self,
    *,
    ChannelId: str,
) -> StopChannelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopChannelResponseTypeDef](./type_defs.md#stopchannelresponsetypedef) 


```python
# stop_channel method usage example with argument unpacking

kwargs: StopChannelRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.stop_channel(**kwargs)
```

1. See [:material-code-braces: StopChannelRequestRequestTypeDef](./type_defs.md#stopchannelrequestrequesttypedef) 

### stop\_input\_device

Stop an input device that is attached to a MediaConnect flow.

Type annotations and code completion for `#!python session.create_client("medialive").stop_input_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/stop_input_device.html)

```python
# stop_input_device method definition

await def stop_input_device(
    self,
    *,
    InputDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_input_device method usage example with argument unpacking

kwargs: StopInputDeviceRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.stop_input_device(**kwargs)
```

1. See [:material-code-braces: StopInputDeviceRequestRequestTypeDef](./type_defs.md#stopinputdevicerequestrequesttypedef) 

### stop\_multiplex

Stops a running multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").stop_multiplex` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/stop_multiplex.html)

```python
# stop_multiplex method definition

await def stop_multiplex(
    self,
    *,
    MultiplexId: str,
) -> StopMultiplexResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopMultiplexResponseTypeDef](./type_defs.md#stopmultiplexresponsetypedef) 


```python
# stop_multiplex method usage example with argument unpacking

kwargs: StopMultiplexRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.stop_multiplex(**kwargs)
```

1. See [:material-code-braces: StopMultiplexRequestRequestTypeDef](./type_defs.md#stopmultiplexrequestrequesttypedef) 

### transfer\_input\_device

Start an input device transfer to another AWS account.

Type annotations and code completion for `#!python session.create_client("medialive").transfer_input_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/transfer_input_device.html)

```python
# transfer_input_device method definition

await def transfer_input_device(
    self,
    *,
    InputDeviceId: str,
    TargetCustomerId: str = ...,
    TargetRegion: str = ...,
    TransferMessage: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# transfer_input_device method usage example with argument unpacking

kwargs: TransferInputDeviceRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.transfer_input_device(**kwargs)
```

1. See [:material-code-braces: TransferInputDeviceRequestRequestTypeDef](./type_defs.md#transferinputdevicerequestrequesttypedef) 

### update\_account\_configuration

Update account configuration.

Type annotations and code completion for `#!python session.create_client("medialive").update_account_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_account_configuration.html)

```python
# update_account_configuration method definition

await def update_account_configuration(
    self,
    *,
    AccountConfiguration: AccountConfigurationTypeDef = ...,  # (1)
) -> UpdateAccountConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AccountConfigurationTypeDef](./type_defs.md#accountconfigurationtypedef) 
2. See [:material-code-braces: UpdateAccountConfigurationResponseTypeDef](./type_defs.md#updateaccountconfigurationresponsetypedef) 


```python
# update_account_configuration method usage example with argument unpacking

kwargs: UpdateAccountConfigurationRequestRequestTypeDef = {  # (1)
    "AccountConfiguration": ...,
}

parent.update_account_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateAccountConfigurationRequestRequestTypeDef](./type_defs.md#updateaccountconfigurationrequestrequesttypedef) 

### update\_channel

Updates a channel.

Type annotations and code completion for `#!python session.create_client("medialive").update_channel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_channel.html)

```python
# update_channel method definition

await def update_channel(
    self,
    *,
    ChannelId: str,
    CdiInputSpecification: CdiInputSpecificationTypeDef = ...,  # (1)
    Destinations: Sequence[OutputDestinationTypeDef] = ...,  # (2)
    EncoderSettings: EncoderSettingsTypeDef = ...,  # (3)
    InputAttachments: Sequence[InputAttachmentTypeDef] = ...,  # (4)
    InputSpecification: InputSpecificationTypeDef = ...,  # (5)
    LogLevel: LogLevelType = ...,  # (6)
    Maintenance: MaintenanceUpdateSettingsTypeDef = ...,  # (7)
    Name: str = ...,
    RoleArn: str = ...,
    ChannelEngineVersion: ChannelEngineVersionRequestTypeDef = ...,  # (8)
    DryRun: bool = ...,
) -> UpdateChannelResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: CdiInputSpecificationTypeDef](./type_defs.md#cdiinputspecificationtypedef) 
2. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
3. See [:material-code-braces: EncoderSettingsTypeDef](./type_defs.md#encodersettingstypedef) 
4. See [:material-code-braces: InputAttachmentTypeDef](./type_defs.md#inputattachmenttypedef) 
5. See [:material-code-braces: InputSpecificationTypeDef](./type_defs.md#inputspecificationtypedef) 
6. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
7. See [:material-code-braces: MaintenanceUpdateSettingsTypeDef](./type_defs.md#maintenanceupdatesettingstypedef) 
8. See [:material-code-braces: ChannelEngineVersionRequestTypeDef](./type_defs.md#channelengineversionrequesttypedef) 
9. See [:material-code-braces: UpdateChannelResponseTypeDef](./type_defs.md#updatechannelresponsetypedef) 


```python
# update_channel method usage example with argument unpacking

kwargs: UpdateChannelRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.update_channel(**kwargs)
```

1. See [:material-code-braces: UpdateChannelRequestRequestTypeDef](./type_defs.md#updatechannelrequestrequesttypedef) 

### update\_channel\_class

Changes the class of the channel.

Type annotations and code completion for `#!python session.create_client("medialive").update_channel_class` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_channel_class.html)

```python
# update_channel_class method definition

await def update_channel_class(
    self,
    *,
    ChannelClass: ChannelClassType,  # (1)
    ChannelId: str,
    Destinations: Sequence[OutputDestinationTypeDef] = ...,  # (2)
) -> UpdateChannelClassResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ChannelClassType](./literals.md#channelclasstype) 
2. See [:material-code-braces: OutputDestinationTypeDef](./type_defs.md#outputdestinationtypedef) 
3. See [:material-code-braces: UpdateChannelClassResponseTypeDef](./type_defs.md#updatechannelclassresponsetypedef) 


```python
# update_channel_class method usage example with argument unpacking

kwargs: UpdateChannelClassRequestRequestTypeDef = {  # (1)
    "ChannelClass": ...,
    "ChannelId": ...,
}

parent.update_channel_class(**kwargs)
```

1. See [:material-code-braces: UpdateChannelClassRequestRequestTypeDef](./type_defs.md#updatechannelclassrequestrequesttypedef) 

### update\_input

Updates an input.

Type annotations and code completion for `#!python session.create_client("medialive").update_input` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_input.html)

```python
# update_input method definition

await def update_input(
    self,
    *,
    InputId: str,
    Destinations: Sequence[InputDestinationRequestTypeDef] = ...,  # (1)
    InputDevices: Sequence[InputDeviceRequestTypeDef] = ...,  # (2)
    InputSecurityGroups: Sequence[str] = ...,
    MediaConnectFlows: Sequence[MediaConnectFlowRequestTypeDef] = ...,  # (3)
    Name: str = ...,
    RoleArn: str = ...,
    Sources: Sequence[InputSourceRequestTypeDef] = ...,  # (4)
    SrtSettings: SrtSettingsRequestTypeDef = ...,  # (5)
    MulticastSettings: MulticastSettingsUpdateRequestTypeDef = ...,  # (6)
) -> UpdateInputResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: InputDestinationRequestTypeDef](./type_defs.md#inputdestinationrequesttypedef) 
2. See [:material-code-braces: InputDeviceRequestTypeDef](./type_defs.md#inputdevicerequesttypedef) 
3. See [:material-code-braces: MediaConnectFlowRequestTypeDef](./type_defs.md#mediaconnectflowrequesttypedef) 
4. See [:material-code-braces: InputSourceRequestTypeDef](./type_defs.md#inputsourcerequesttypedef) 
5. See [:material-code-braces: SrtSettingsRequestTypeDef](./type_defs.md#srtsettingsrequesttypedef) 
6. See [:material-code-braces: MulticastSettingsUpdateRequestTypeDef](./type_defs.md#multicastsettingsupdaterequesttypedef) 
7. See [:material-code-braces: UpdateInputResponseTypeDef](./type_defs.md#updateinputresponsetypedef) 


```python
# update_input method usage example with argument unpacking

kwargs: UpdateInputRequestRequestTypeDef = {  # (1)
    "InputId": ...,
}

parent.update_input(**kwargs)
```

1. See [:material-code-braces: UpdateInputRequestRequestTypeDef](./type_defs.md#updateinputrequestrequesttypedef) 

### update\_input\_device

Updates the parameters for the input device.

Type annotations and code completion for `#!python session.create_client("medialive").update_input_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_input_device.html)

```python
# update_input_device method definition

await def update_input_device(
    self,
    *,
    InputDeviceId: str,
    HdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,  # (1)
    Name: str = ...,
    UhdDeviceSettings: InputDeviceConfigurableSettingsTypeDef = ...,  # (1)
    AvailabilityZone: str = ...,
) -> UpdateInputDeviceResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InputDeviceConfigurableSettingsTypeDef](./type_defs.md#inputdeviceconfigurablesettingstypedef) 
2. See [:material-code-braces: InputDeviceConfigurableSettingsTypeDef](./type_defs.md#inputdeviceconfigurablesettingstypedef) 
3. See [:material-code-braces: UpdateInputDeviceResponseTypeDef](./type_defs.md#updateinputdeviceresponsetypedef) 


```python
# update_input_device method usage example with argument unpacking

kwargs: UpdateInputDeviceRequestRequestTypeDef = {  # (1)
    "InputDeviceId": ...,
}

parent.update_input_device(**kwargs)
```

1. See [:material-code-braces: UpdateInputDeviceRequestRequestTypeDef](./type_defs.md#updateinputdevicerequestrequesttypedef) 

### update\_input\_security\_group

Update an Input Security Group's Whilelists.

Type annotations and code completion for `#!python session.create_client("medialive").update_input_security_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_input_security_group.html)

```python
# update_input_security_group method definition

await def update_input_security_group(
    self,
    *,
    InputSecurityGroupId: str,
    Tags: Mapping[str, str] = ...,
    WhitelistRules: Sequence[InputWhitelistRuleCidrTypeDef] = ...,  # (1)
) -> UpdateInputSecurityGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InputWhitelistRuleCidrTypeDef](./type_defs.md#inputwhitelistrulecidrtypedef) 
2. See [:material-code-braces: UpdateInputSecurityGroupResponseTypeDef](./type_defs.md#updateinputsecuritygroupresponsetypedef) 


```python
# update_input_security_group method usage example with argument unpacking

kwargs: UpdateInputSecurityGroupRequestRequestTypeDef = {  # (1)
    "InputSecurityGroupId": ...,
}

parent.update_input_security_group(**kwargs)
```

1. See [:material-code-braces: UpdateInputSecurityGroupRequestRequestTypeDef](./type_defs.md#updateinputsecuritygrouprequestrequesttypedef) 

### update\_multiplex

Updates a multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").update_multiplex` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_multiplex.html)

```python
# update_multiplex method definition

await def update_multiplex(
    self,
    *,
    MultiplexId: str,
    MultiplexSettings: MultiplexSettingsTypeDef = ...,  # (1)
    Name: str = ...,
    PacketIdentifiersMapping: Mapping[str, MultiplexProgramPacketIdentifiersMapUnionTypeDef] = ...,  # (2)
) -> UpdateMultiplexResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: MultiplexSettingsTypeDef](./type_defs.md#multiplexsettingstypedef) 
2. See [:material-code-braces: MultiplexProgramPacketIdentifiersMapTypeDef](./type_defs.md#multiplexprogrampacketidentifiersmaptypedef) [:material-code-braces: MultiplexProgramPacketIdentifiersMapOutputTypeDef](./type_defs.md#multiplexprogrampacketidentifiersmapoutputtypedef) 
3. See [:material-code-braces: UpdateMultiplexResponseTypeDef](./type_defs.md#updatemultiplexresponsetypedef) 


```python
# update_multiplex method usage example with argument unpacking

kwargs: UpdateMultiplexRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
}

parent.update_multiplex(**kwargs)
```

1. See [:material-code-braces: UpdateMultiplexRequestRequestTypeDef](./type_defs.md#updatemultiplexrequestrequesttypedef) 

### update\_multiplex\_program

Update a program in a multiplex.

Type annotations and code completion for `#!python session.create_client("medialive").update_multiplex_program` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_multiplex_program.html)

```python
# update_multiplex_program method definition

await def update_multiplex_program(
    self,
    *,
    MultiplexId: str,
    ProgramName: str,
    MultiplexProgramSettings: MultiplexProgramSettingsTypeDef = ...,  # (1)
) -> UpdateMultiplexProgramResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MultiplexProgramSettingsTypeDef](./type_defs.md#multiplexprogramsettingstypedef) 
2. See [:material-code-braces: UpdateMultiplexProgramResponseTypeDef](./type_defs.md#updatemultiplexprogramresponsetypedef) 


```python
# update_multiplex_program method usage example with argument unpacking

kwargs: UpdateMultiplexProgramRequestRequestTypeDef = {  # (1)
    "MultiplexId": ...,
    "ProgramName": ...,
}

parent.update_multiplex_program(**kwargs)
```

1. See [:material-code-braces: UpdateMultiplexProgramRequestRequestTypeDef](./type_defs.md#updatemultiplexprogramrequestrequesttypedef) 

### update\_reservation

Update reservation.

Type annotations and code completion for `#!python session.create_client("medialive").update_reservation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_reservation.html)

```python
# update_reservation method definition

await def update_reservation(
    self,
    *,
    ReservationId: str,
    Name: str = ...,
    RenewalSettings: RenewalSettingsTypeDef = ...,  # (1)
) -> UpdateReservationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RenewalSettingsTypeDef](./type_defs.md#renewalsettingstypedef) 
2. See [:material-code-braces: UpdateReservationResponseTypeDef](./type_defs.md#updatereservationresponsetypedef) 


```python
# update_reservation method usage example with argument unpacking

kwargs: UpdateReservationRequestRequestTypeDef = {  # (1)
    "ReservationId": ...,
}

parent.update_reservation(**kwargs)
```

1. See [:material-code-braces: UpdateReservationRequestRequestTypeDef](./type_defs.md#updatereservationrequestrequesttypedef) 

### restart\_channel\_pipelines

Restart pipelines in one channel that is currently running.

Type annotations and code completion for `#!python session.create_client("medialive").restart_channel_pipelines` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/restart_channel_pipelines.html)

```python
# restart_channel_pipelines method definition

await def restart_channel_pipelines(
    self,
    *,
    ChannelId: str,
    PipelineIds: Sequence[ChannelPipelineIdToRestartType] = ...,  # (1)
) -> RestartChannelPipelinesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ChannelPipelineIdToRestartType](./literals.md#channelpipelineidtorestarttype) 
2. See [:material-code-braces: RestartChannelPipelinesResponseTypeDef](./type_defs.md#restartchannelpipelinesresponsetypedef) 


```python
# restart_channel_pipelines method usage example with argument unpacking

kwargs: RestartChannelPipelinesRequestRequestTypeDef = {  # (1)
    "ChannelId": ...,
}

parent.restart_channel_pipelines(**kwargs)
```

1. See [:material-code-braces: RestartChannelPipelinesRequestRequestTypeDef](./type_defs.md#restartchannelpipelinesrequestrequesttypedef) 

### create\_cloud\_watch\_alarm\_template

Creates a cloudwatch alarm template to dynamically generate cloudwatch metric
alarms on targeted resource types.

Type annotations and code completion for `#!python session.create_client("medialive").create_cloud_watch_alarm_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_cloud_watch_alarm_template.html)

```python
# create_cloud_watch_alarm_template method definition

await def create_cloud_watch_alarm_template(
    self,
    *,
    ComparisonOperator: CloudWatchAlarmTemplateComparisonOperatorType,  # (1)
    EvaluationPeriods: int,
    GroupIdentifier: str,
    MetricName: str,
    Name: str,
    Period: int,
    Statistic: CloudWatchAlarmTemplateStatisticType,  # (2)
    TargetResourceType: CloudWatchAlarmTemplateTargetResourceTypeType,  # (3)
    Threshold: float,
    TreatMissingData: CloudWatchAlarmTemplateTreatMissingDataType,  # (4)
    DatapointsToAlarm: int = ...,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateCloudWatchAlarmTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: CloudWatchAlarmTemplateComparisonOperatorType](./literals.md#cloudwatchalarmtemplatecomparisonoperatortype) 
2. See [:material-code-brackets: CloudWatchAlarmTemplateStatisticType](./literals.md#cloudwatchalarmtemplatestatistictype) 
3. See [:material-code-brackets: CloudWatchAlarmTemplateTargetResourceTypeType](./literals.md#cloudwatchalarmtemplatetargetresourcetypetype) 
4. See [:material-code-brackets: CloudWatchAlarmTemplateTreatMissingDataType](./literals.md#cloudwatchalarmtemplatetreatmissingdatatype) 
5. See [:material-code-braces: CreateCloudWatchAlarmTemplateResponseTypeDef](./type_defs.md#createcloudwatchalarmtemplateresponsetypedef) 


```python
# create_cloud_watch_alarm_template method usage example with argument unpacking

kwargs: CreateCloudWatchAlarmTemplateRequestRequestTypeDef = {  # (1)
    "ComparisonOperator": ...,
    "EvaluationPeriods": ...,
    "GroupIdentifier": ...,
    "MetricName": ...,
    "Name": ...,
    "Period": ...,
    "Statistic": ...,
    "TargetResourceType": ...,
    "Threshold": ...,
    "TreatMissingData": ...,
}

parent.create_cloud_watch_alarm_template(**kwargs)
```

1. See [:material-code-braces: CreateCloudWatchAlarmTemplateRequestRequestTypeDef](./type_defs.md#createcloudwatchalarmtemplaterequestrequesttypedef) 

### create\_cloud\_watch\_alarm\_template\_group

Creates a cloudwatch alarm template group to group your cloudwatch alarm
templates and to attach to signal maps for dynamically creating alarms.

Type annotations and code completion for `#!python session.create_client("medialive").create_cloud_watch_alarm_template_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_cloud_watch_alarm_template_group.html)

```python
# create_cloud_watch_alarm_template_group method definition

await def create_cloud_watch_alarm_template_group(
    self,
    *,
    Name: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateCloudWatchAlarmTemplateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateCloudWatchAlarmTemplateGroupResponseTypeDef](./type_defs.md#createcloudwatchalarmtemplategroupresponsetypedef) 


```python
# create_cloud_watch_alarm_template_group method usage example with argument unpacking

kwargs: CreateCloudWatchAlarmTemplateGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_cloud_watch_alarm_template_group(**kwargs)
```

1. See [:material-code-braces: CreateCloudWatchAlarmTemplateGroupRequestRequestTypeDef](./type_defs.md#createcloudwatchalarmtemplategrouprequestrequesttypedef) 

### create\_event\_bridge\_rule\_template

Creates an eventbridge rule template to monitor events and send notifications
to your targeted resources.

Type annotations and code completion for `#!python session.create_client("medialive").create_event_bridge_rule_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_event_bridge_rule_template.html)

```python
# create_event_bridge_rule_template method definition

await def create_event_bridge_rule_template(
    self,
    *,
    EventType: EventBridgeRuleTemplateEventTypeType,  # (1)
    GroupIdentifier: str,
    Name: str,
    Description: str = ...,
    EventTargets: Sequence[EventBridgeRuleTemplateTargetTypeDef] = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateEventBridgeRuleTemplateResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: EventBridgeRuleTemplateEventTypeType](./literals.md#eventbridgeruletemplateeventtypetype) 
2. See [:material-code-braces: EventBridgeRuleTemplateTargetTypeDef](./type_defs.md#eventbridgeruletemplatetargettypedef) 
3. See [:material-code-braces: CreateEventBridgeRuleTemplateResponseTypeDef](./type_defs.md#createeventbridgeruletemplateresponsetypedef) 


```python
# create_event_bridge_rule_template method usage example with argument unpacking

kwargs: CreateEventBridgeRuleTemplateRequestRequestTypeDef = {  # (1)
    "EventType": ...,
    "GroupIdentifier": ...,
    "Name": ...,
}

parent.create_event_bridge_rule_template(**kwargs)
```

1. See [:material-code-braces: CreateEventBridgeRuleTemplateRequestRequestTypeDef](./type_defs.md#createeventbridgeruletemplaterequestrequesttypedef) 

### create\_event\_bridge\_rule\_template\_group

Creates an eventbridge rule template group to group your eventbridge rule
templates and to attach to signal maps for dynamically creating notification
rules.

Type annotations and code completion for `#!python session.create_client("medialive").create_event_bridge_rule_template_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_event_bridge_rule_template_group.html)

```python
# create_event_bridge_rule_template_group method definition

await def create_event_bridge_rule_template_group(
    self,
    *,
    Name: str,
    Description: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateEventBridgeRuleTemplateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateEventBridgeRuleTemplateGroupResponseTypeDef](./type_defs.md#createeventbridgeruletemplategroupresponsetypedef) 


```python
# create_event_bridge_rule_template_group method usage example with argument unpacking

kwargs: CreateEventBridgeRuleTemplateGroupRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_event_bridge_rule_template_group(**kwargs)
```

1. See [:material-code-braces: CreateEventBridgeRuleTemplateGroupRequestRequestTypeDef](./type_defs.md#createeventbridgeruletemplategrouprequestrequesttypedef) 

### create\_signal\_map

Initiates the creation of a new signal map.

Type annotations and code completion for `#!python session.create_client("medialive").create_signal_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_signal_map.html)

```python
# create_signal_map method definition

await def create_signal_map(
    self,
    *,
    DiscoveryEntryPointArn: str,
    Name: str,
    CloudWatchAlarmTemplateGroupIdentifiers: Sequence[str] = ...,
    Description: str = ...,
    EventBridgeRuleTemplateGroupIdentifiers: Sequence[str] = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateSignalMapResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateSignalMapResponseTypeDef](./type_defs.md#createsignalmapresponsetypedef) 


```python
# create_signal_map method usage example with argument unpacking

kwargs: CreateSignalMapRequestRequestTypeDef = {  # (1)
    "DiscoveryEntryPointArn": ...,
    "Name": ...,
}

parent.create_signal_map(**kwargs)
```

1. See [:material-code-braces: CreateSignalMapRequestRequestTypeDef](./type_defs.md#createsignalmaprequestrequesttypedef) 

### delete\_cloud\_watch\_alarm\_template

Deletes a cloudwatch alarm template.

Type annotations and code completion for `#!python session.create_client("medialive").delete_cloud_watch_alarm_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_cloud_watch_alarm_template.html)

```python
# delete_cloud_watch_alarm_template method definition

await def delete_cloud_watch_alarm_template(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_cloud_watch_alarm_template method usage example with argument unpacking

kwargs: DeleteCloudWatchAlarmTemplateRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_cloud_watch_alarm_template(**kwargs)
```

1. See [:material-code-braces: DeleteCloudWatchAlarmTemplateRequestRequestTypeDef](./type_defs.md#deletecloudwatchalarmtemplaterequestrequesttypedef) 

### delete\_cloud\_watch\_alarm\_template\_group

Deletes a cloudwatch alarm template group.

Type annotations and code completion for `#!python session.create_client("medialive").delete_cloud_watch_alarm_template_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_cloud_watch_alarm_template_group.html)

```python
# delete_cloud_watch_alarm_template_group method definition

await def delete_cloud_watch_alarm_template_group(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_cloud_watch_alarm_template_group method usage example with argument unpacking

kwargs: DeleteCloudWatchAlarmTemplateGroupRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_cloud_watch_alarm_template_group(**kwargs)
```

1. See [:material-code-braces: DeleteCloudWatchAlarmTemplateGroupRequestRequestTypeDef](./type_defs.md#deletecloudwatchalarmtemplategrouprequestrequesttypedef) 

### delete\_event\_bridge\_rule\_template

Deletes an eventbridge rule template.

Type annotations and code completion for `#!python session.create_client("medialive").delete_event_bridge_rule_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_event_bridge_rule_template.html)

```python
# delete_event_bridge_rule_template method definition

await def delete_event_bridge_rule_template(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_event_bridge_rule_template method usage example with argument unpacking

kwargs: DeleteEventBridgeRuleTemplateRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_event_bridge_rule_template(**kwargs)
```

1. See [:material-code-braces: DeleteEventBridgeRuleTemplateRequestRequestTypeDef](./type_defs.md#deleteeventbridgeruletemplaterequestrequesttypedef) 

### delete\_event\_bridge\_rule\_template\_group

Deletes an eventbridge rule template group.

Type annotations and code completion for `#!python session.create_client("medialive").delete_event_bridge_rule_template_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_event_bridge_rule_template_group.html)

```python
# delete_event_bridge_rule_template_group method definition

await def delete_event_bridge_rule_template_group(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_event_bridge_rule_template_group method usage example with argument unpacking

kwargs: DeleteEventBridgeRuleTemplateGroupRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_event_bridge_rule_template_group(**kwargs)
```

1. See [:material-code-braces: DeleteEventBridgeRuleTemplateGroupRequestRequestTypeDef](./type_defs.md#deleteeventbridgeruletemplategrouprequestrequesttypedef) 

### delete\_signal\_map

Deletes the specified signal map.

Type annotations and code completion for `#!python session.create_client("medialive").delete_signal_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_signal_map.html)

```python
# delete_signal_map method definition

await def delete_signal_map(
    self,
    *,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_signal_map method usage example with argument unpacking

kwargs: DeleteSignalMapRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.delete_signal_map(**kwargs)
```

1. See [:material-code-braces: DeleteSignalMapRequestRequestTypeDef](./type_defs.md#deletesignalmaprequestrequesttypedef) 

### get\_cloud\_watch\_alarm\_template

Retrieves the specified cloudwatch alarm template.

Type annotations and code completion for `#!python session.create_client("medialive").get_cloud_watch_alarm_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/get_cloud_watch_alarm_template.html)

```python
# get_cloud_watch_alarm_template method definition

await def get_cloud_watch_alarm_template(
    self,
    *,
    Identifier: str,
) -> GetCloudWatchAlarmTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCloudWatchAlarmTemplateResponseTypeDef](./type_defs.md#getcloudwatchalarmtemplateresponsetypedef) 


```python
# get_cloud_watch_alarm_template method usage example with argument unpacking

kwargs: GetCloudWatchAlarmTemplateRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_cloud_watch_alarm_template(**kwargs)
```

1. See [:material-code-braces: GetCloudWatchAlarmTemplateRequestRequestTypeDef](./type_defs.md#getcloudwatchalarmtemplaterequestrequesttypedef) 

### get\_cloud\_watch\_alarm\_template\_group

Retrieves the specified cloudwatch alarm template group.

Type annotations and code completion for `#!python session.create_client("medialive").get_cloud_watch_alarm_template_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/get_cloud_watch_alarm_template_group.html)

```python
# get_cloud_watch_alarm_template_group method definition

await def get_cloud_watch_alarm_template_group(
    self,
    *,
    Identifier: str,
) -> GetCloudWatchAlarmTemplateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCloudWatchAlarmTemplateGroupResponseTypeDef](./type_defs.md#getcloudwatchalarmtemplategroupresponsetypedef) 


```python
# get_cloud_watch_alarm_template_group method usage example with argument unpacking

kwargs: GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_cloud_watch_alarm_template_group(**kwargs)
```

1. See [:material-code-braces: GetCloudWatchAlarmTemplateGroupRequestRequestTypeDef](./type_defs.md#getcloudwatchalarmtemplategrouprequestrequesttypedef) 

### get\_event\_bridge\_rule\_template

Retrieves the specified eventbridge rule template.

Type annotations and code completion for `#!python session.create_client("medialive").get_event_bridge_rule_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/get_event_bridge_rule_template.html)

```python
# get_event_bridge_rule_template method definition

await def get_event_bridge_rule_template(
    self,
    *,
    Identifier: str,
) -> GetEventBridgeRuleTemplateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventBridgeRuleTemplateResponseTypeDef](./type_defs.md#geteventbridgeruletemplateresponsetypedef) 


```python
# get_event_bridge_rule_template method usage example with argument unpacking

kwargs: GetEventBridgeRuleTemplateRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_event_bridge_rule_template(**kwargs)
```

1. See [:material-code-braces: GetEventBridgeRuleTemplateRequestRequestTypeDef](./type_defs.md#geteventbridgeruletemplaterequestrequesttypedef) 

### get\_event\_bridge\_rule\_template\_group

Retrieves the specified eventbridge rule template group.

Type annotations and code completion for `#!python session.create_client("medialive").get_event_bridge_rule_template_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/get_event_bridge_rule_template_group.html)

```python
# get_event_bridge_rule_template_group method definition

await def get_event_bridge_rule_template_group(
    self,
    *,
    Identifier: str,
) -> GetEventBridgeRuleTemplateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventBridgeRuleTemplateGroupResponseTypeDef](./type_defs.md#geteventbridgeruletemplategroupresponsetypedef) 


```python
# get_event_bridge_rule_template_group method usage example with argument unpacking

kwargs: GetEventBridgeRuleTemplateGroupRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_event_bridge_rule_template_group(**kwargs)
```

1. See [:material-code-braces: GetEventBridgeRuleTemplateGroupRequestRequestTypeDef](./type_defs.md#geteventbridgeruletemplategrouprequestrequesttypedef) 

### get\_signal\_map

Retrieves the specified signal map.

Type annotations and code completion for `#!python session.create_client("medialive").get_signal_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/get_signal_map.html)

```python
# get_signal_map method definition

await def get_signal_map(
    self,
    *,
    Identifier: str,
) -> GetSignalMapResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSignalMapResponseTypeDef](./type_defs.md#getsignalmapresponsetypedef) 


```python
# get_signal_map method usage example with argument unpacking

kwargs: GetSignalMapRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.get_signal_map(**kwargs)
```

1. See [:material-code-braces: GetSignalMapRequestRequestTypeDef](./type_defs.md#getsignalmaprequestrequesttypedef) 

### list\_cloud\_watch\_alarm\_template\_groups

Lists cloudwatch alarm template groups.

Type annotations and code completion for `#!python session.create_client("medialive").list_cloud_watch_alarm_template_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_cloud_watch_alarm_template_groups.html)

```python
# list_cloud_watch_alarm_template_groups method definition

await def list_cloud_watch_alarm_template_groups(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    Scope: str = ...,
    SignalMapIdentifier: str = ...,
) -> ListCloudWatchAlarmTemplateGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCloudWatchAlarmTemplateGroupsResponseTypeDef](./type_defs.md#listcloudwatchalarmtemplategroupsresponsetypedef) 


```python
# list_cloud_watch_alarm_template_groups method usage example with argument unpacking

kwargs: ListCloudWatchAlarmTemplateGroupsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_cloud_watch_alarm_template_groups(**kwargs)
```

1. See [:material-code-braces: ListCloudWatchAlarmTemplateGroupsRequestRequestTypeDef](./type_defs.md#listcloudwatchalarmtemplategroupsrequestrequesttypedef) 

### list\_cloud\_watch\_alarm\_templates

Lists cloudwatch alarm templates.

Type annotations and code completion for `#!python session.create_client("medialive").list_cloud_watch_alarm_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_cloud_watch_alarm_templates.html)

```python
# list_cloud_watch_alarm_templates method definition

await def list_cloud_watch_alarm_templates(
    self,
    *,
    GroupIdentifier: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Scope: str = ...,
    SignalMapIdentifier: str = ...,
) -> ListCloudWatchAlarmTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCloudWatchAlarmTemplatesResponseTypeDef](./type_defs.md#listcloudwatchalarmtemplatesresponsetypedef) 


```python
# list_cloud_watch_alarm_templates method usage example with argument unpacking

kwargs: ListCloudWatchAlarmTemplatesRequestRequestTypeDef = {  # (1)
    "GroupIdentifier": ...,
}

parent.list_cloud_watch_alarm_templates(**kwargs)
```

1. See [:material-code-braces: ListCloudWatchAlarmTemplatesRequestRequestTypeDef](./type_defs.md#listcloudwatchalarmtemplatesrequestrequesttypedef) 

### list\_event\_bridge\_rule\_template\_groups

Lists eventbridge rule template groups.

Type annotations and code completion for `#!python session.create_client("medialive").list_event_bridge_rule_template_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_event_bridge_rule_template_groups.html)

```python
# list_event_bridge_rule_template_groups method definition

await def list_event_bridge_rule_template_groups(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    SignalMapIdentifier: str = ...,
) -> ListEventBridgeRuleTemplateGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventBridgeRuleTemplateGroupsResponseTypeDef](./type_defs.md#listeventbridgeruletemplategroupsresponsetypedef) 


```python
# list_event_bridge_rule_template_groups method usage example with argument unpacking

kwargs: ListEventBridgeRuleTemplateGroupsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_event_bridge_rule_template_groups(**kwargs)
```

1. See [:material-code-braces: ListEventBridgeRuleTemplateGroupsRequestRequestTypeDef](./type_defs.md#listeventbridgeruletemplategroupsrequestrequesttypedef) 

### list\_event\_bridge\_rule\_templates

Lists eventbridge rule templates.

Type annotations and code completion for `#!python session.create_client("medialive").list_event_bridge_rule_templates` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_event_bridge_rule_templates.html)

```python
# list_event_bridge_rule_templates method definition

await def list_event_bridge_rule_templates(
    self,
    *,
    GroupIdentifier: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    SignalMapIdentifier: str = ...,
) -> ListEventBridgeRuleTemplatesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEventBridgeRuleTemplatesResponseTypeDef](./type_defs.md#listeventbridgeruletemplatesresponsetypedef) 


```python
# list_event_bridge_rule_templates method usage example with argument unpacking

kwargs: ListEventBridgeRuleTemplatesRequestRequestTypeDef = {  # (1)
    "GroupIdentifier": ...,
}

parent.list_event_bridge_rule_templates(**kwargs)
```

1. See [:material-code-braces: ListEventBridgeRuleTemplatesRequestRequestTypeDef](./type_defs.md#listeventbridgeruletemplatesrequestrequesttypedef) 

### list\_signal\_maps

Lists signal maps.

Type annotations and code completion for `#!python session.create_client("medialive").list_signal_maps` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_signal_maps.html)

```python
# list_signal_maps method definition

await def list_signal_maps(
    self,
    *,
    CloudWatchAlarmTemplateGroupIdentifier: str = ...,
    EventBridgeRuleTemplateGroupIdentifier: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListSignalMapsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListSignalMapsResponseTypeDef](./type_defs.md#listsignalmapsresponsetypedef) 


```python
# list_signal_maps method usage example with argument unpacking

kwargs: ListSignalMapsRequestRequestTypeDef = {  # (1)
    "CloudWatchAlarmTemplateGroupIdentifier": ...,
}

parent.list_signal_maps(**kwargs)
```

1. See [:material-code-braces: ListSignalMapsRequestRequestTypeDef](./type_defs.md#listsignalmapsrequestrequesttypedef) 

### start\_delete\_monitor\_deployment

Initiates a deployment to delete the monitor of the specified signal map.

Type annotations and code completion for `#!python session.create_client("medialive").start_delete_monitor_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/start_delete_monitor_deployment.html)

```python
# start_delete_monitor_deployment method definition

await def start_delete_monitor_deployment(
    self,
    *,
    Identifier: str,
) -> StartDeleteMonitorDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartDeleteMonitorDeploymentResponseTypeDef](./type_defs.md#startdeletemonitordeploymentresponsetypedef) 


```python
# start_delete_monitor_deployment method usage example with argument unpacking

kwargs: StartDeleteMonitorDeploymentRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.start_delete_monitor_deployment(**kwargs)
```

1. See [:material-code-braces: StartDeleteMonitorDeploymentRequestRequestTypeDef](./type_defs.md#startdeletemonitordeploymentrequestrequesttypedef) 

### start\_monitor\_deployment

Initiates a deployment to deploy the latest monitor of the specified signal map.

Type annotations and code completion for `#!python session.create_client("medialive").start_monitor_deployment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/start_monitor_deployment.html)

```python
# start_monitor_deployment method definition

await def start_monitor_deployment(
    self,
    *,
    Identifier: str,
    DryRun: bool = ...,
) -> StartMonitorDeploymentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartMonitorDeploymentResponseTypeDef](./type_defs.md#startmonitordeploymentresponsetypedef) 


```python
# start_monitor_deployment method usage example with argument unpacking

kwargs: StartMonitorDeploymentRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.start_monitor_deployment(**kwargs)
```

1. See [:material-code-braces: StartMonitorDeploymentRequestRequestTypeDef](./type_defs.md#startmonitordeploymentrequestrequesttypedef) 

### start\_update\_signal\_map

Initiates an update for the specified signal map.

Type annotations and code completion for `#!python session.create_client("medialive").start_update_signal_map` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/start_update_signal_map.html)

```python
# start_update_signal_map method definition

await def start_update_signal_map(
    self,
    *,
    Identifier: str,
    CloudWatchAlarmTemplateGroupIdentifiers: Sequence[str] = ...,
    Description: str = ...,
    DiscoveryEntryPointArn: str = ...,
    EventBridgeRuleTemplateGroupIdentifiers: Sequence[str] = ...,
    ForceRediscovery: bool = ...,
    Name: str = ...,
) -> StartUpdateSignalMapResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartUpdateSignalMapResponseTypeDef](./type_defs.md#startupdatesignalmapresponsetypedef) 


```python
# start_update_signal_map method usage example with argument unpacking

kwargs: StartUpdateSignalMapRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.start_update_signal_map(**kwargs)
```

1. See [:material-code-braces: StartUpdateSignalMapRequestRequestTypeDef](./type_defs.md#startupdatesignalmaprequestrequesttypedef) 

### update\_cloud\_watch\_alarm\_template

Updates the specified cloudwatch alarm template.

Type annotations and code completion for `#!python session.create_client("medialive").update_cloud_watch_alarm_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_cloud_watch_alarm_template.html)

```python
# update_cloud_watch_alarm_template method definition

await def update_cloud_watch_alarm_template(
    self,
    *,
    Identifier: str,
    ComparisonOperator: CloudWatchAlarmTemplateComparisonOperatorType = ...,  # (1)
    DatapointsToAlarm: int = ...,
    Description: str = ...,
    EvaluationPeriods: int = ...,
    GroupIdentifier: str = ...,
    MetricName: str = ...,
    Name: str = ...,
    Period: int = ...,
    Statistic: CloudWatchAlarmTemplateStatisticType = ...,  # (2)
    TargetResourceType: CloudWatchAlarmTemplateTargetResourceTypeType = ...,  # (3)
    Threshold: float = ...,
    TreatMissingData: CloudWatchAlarmTemplateTreatMissingDataType = ...,  # (4)
) -> UpdateCloudWatchAlarmTemplateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: CloudWatchAlarmTemplateComparisonOperatorType](./literals.md#cloudwatchalarmtemplatecomparisonoperatortype) 
2. See [:material-code-brackets: CloudWatchAlarmTemplateStatisticType](./literals.md#cloudwatchalarmtemplatestatistictype) 
3. See [:material-code-brackets: CloudWatchAlarmTemplateTargetResourceTypeType](./literals.md#cloudwatchalarmtemplatetargetresourcetypetype) 
4. See [:material-code-brackets: CloudWatchAlarmTemplateTreatMissingDataType](./literals.md#cloudwatchalarmtemplatetreatmissingdatatype) 
5. See [:material-code-braces: UpdateCloudWatchAlarmTemplateResponseTypeDef](./type_defs.md#updatecloudwatchalarmtemplateresponsetypedef) 


```python
# update_cloud_watch_alarm_template method usage example with argument unpacking

kwargs: UpdateCloudWatchAlarmTemplateRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_cloud_watch_alarm_template(**kwargs)
```

1. See [:material-code-braces: UpdateCloudWatchAlarmTemplateRequestRequestTypeDef](./type_defs.md#updatecloudwatchalarmtemplaterequestrequesttypedef) 

### update\_cloud\_watch\_alarm\_template\_group

Updates the specified cloudwatch alarm template group.

Type annotations and code completion for `#!python session.create_client("medialive").update_cloud_watch_alarm_template_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_cloud_watch_alarm_template_group.html)

```python
# update_cloud_watch_alarm_template_group method definition

await def update_cloud_watch_alarm_template_group(
    self,
    *,
    Identifier: str,
    Description: str = ...,
) -> UpdateCloudWatchAlarmTemplateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateCloudWatchAlarmTemplateGroupResponseTypeDef](./type_defs.md#updatecloudwatchalarmtemplategroupresponsetypedef) 


```python
# update_cloud_watch_alarm_template_group method usage example with argument unpacking

kwargs: UpdateCloudWatchAlarmTemplateGroupRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_cloud_watch_alarm_template_group(**kwargs)
```

1. See [:material-code-braces: UpdateCloudWatchAlarmTemplateGroupRequestRequestTypeDef](./type_defs.md#updatecloudwatchalarmtemplategrouprequestrequesttypedef) 

### update\_event\_bridge\_rule\_template

Updates the specified eventbridge rule template.

Type annotations and code completion for `#!python session.create_client("medialive").update_event_bridge_rule_template` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_event_bridge_rule_template.html)

```python
# update_event_bridge_rule_template method definition

await def update_event_bridge_rule_template(
    self,
    *,
    Identifier: str,
    Description: str = ...,
    EventTargets: Sequence[EventBridgeRuleTemplateTargetTypeDef] = ...,  # (1)
    EventType: EventBridgeRuleTemplateEventTypeType = ...,  # (2)
    GroupIdentifier: str = ...,
    Name: str = ...,
) -> UpdateEventBridgeRuleTemplateResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: EventBridgeRuleTemplateTargetTypeDef](./type_defs.md#eventbridgeruletemplatetargettypedef) 
2. See [:material-code-brackets: EventBridgeRuleTemplateEventTypeType](./literals.md#eventbridgeruletemplateeventtypetype) 
3. See [:material-code-braces: UpdateEventBridgeRuleTemplateResponseTypeDef](./type_defs.md#updateeventbridgeruletemplateresponsetypedef) 


```python
# update_event_bridge_rule_template method usage example with argument unpacking

kwargs: UpdateEventBridgeRuleTemplateRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_event_bridge_rule_template(**kwargs)
```

1. See [:material-code-braces: UpdateEventBridgeRuleTemplateRequestRequestTypeDef](./type_defs.md#updateeventbridgeruletemplaterequestrequesttypedef) 

### update\_event\_bridge\_rule\_template\_group

Updates the specified eventbridge rule template group.

Type annotations and code completion for `#!python session.create_client("medialive").update_event_bridge_rule_template_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_event_bridge_rule_template_group.html)

```python
# update_event_bridge_rule_template_group method definition

await def update_event_bridge_rule_template_group(
    self,
    *,
    Identifier: str,
    Description: str = ...,
) -> UpdateEventBridgeRuleTemplateGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEventBridgeRuleTemplateGroupResponseTypeDef](./type_defs.md#updateeventbridgeruletemplategroupresponsetypedef) 


```python
# update_event_bridge_rule_template_group method usage example with argument unpacking

kwargs: UpdateEventBridgeRuleTemplateGroupRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.update_event_bridge_rule_template_group(**kwargs)
```

1. See [:material-code-braces: UpdateEventBridgeRuleTemplateGroupRequestRequestTypeDef](./type_defs.md#updateeventbridgeruletemplategrouprequestrequesttypedef) 

### create\_channel\_placement\_group

Create a ChannelPlacementGroup in the specified Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").create_channel_placement_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_channel_placement_group.html)

```python
# create_channel_placement_group method definition

await def create_channel_placement_group(
    self,
    *,
    ClusterId: str,
    Name: str = ...,
    Nodes: Sequence[str] = ...,
    RequestId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateChannelPlacementGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateChannelPlacementGroupResponseTypeDef](./type_defs.md#createchannelplacementgroupresponsetypedef) 


```python
# create_channel_placement_group method usage example with argument unpacking

kwargs: CreateChannelPlacementGroupRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.create_channel_placement_group(**kwargs)
```

1. See [:material-code-braces: CreateChannelPlacementGroupRequestRequestTypeDef](./type_defs.md#createchannelplacementgrouprequestrequesttypedef) 

### create\_cluster

Create a new Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").create_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_cluster.html)

```python
# create_cluster method definition

await def create_cluster(
    self,
    *,
    ClusterType: ClusterTypeType = ...,  # (1)
    InstanceRoleArn: str = ...,
    Name: str = ...,
    NetworkSettings: ClusterNetworkSettingsCreateRequestTypeDef = ...,  # (2)
    RequestId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> CreateClusterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ClusterTypeType](./literals.md#clustertypetype) 
2. See [:material-code-braces: ClusterNetworkSettingsCreateRequestTypeDef](./type_defs.md#clusternetworksettingscreaterequesttypedef) 
3. See [:material-code-braces: CreateClusterResponseTypeDef](./type_defs.md#createclusterresponsetypedef) 


```python
# create_cluster method usage example with argument unpacking

kwargs: CreateClusterRequestRequestTypeDef = {  # (1)
    "ClusterType": ...,
}

parent.create_cluster(**kwargs)
```

1. See [:material-code-braces: CreateClusterRequestRequestTypeDef](./type_defs.md#createclusterrequestrequesttypedef) 

### create\_network

Create as many Networks as you need.

Type annotations and code completion for `#!python session.create_client("medialive").create_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_network.html)

```python
# create_network method definition

await def create_network(
    self,
    *,
    IpPools: Sequence[IpPoolCreateRequestTypeDef] = ...,  # (1)
    Name: str = ...,
    RequestId: str = ...,
    Routes: Sequence[RouteCreateRequestTypeDef] = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateNetworkResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IpPoolCreateRequestTypeDef](./type_defs.md#ippoolcreaterequesttypedef) 
2. See [:material-code-braces: RouteCreateRequestTypeDef](./type_defs.md#routecreaterequesttypedef) 
3. See [:material-code-braces: CreateNetworkResponseTypeDef](./type_defs.md#createnetworkresponsetypedef) 


```python
# create_network method usage example with argument unpacking

kwargs: CreateNetworkRequestRequestTypeDef = {  # (1)
    "IpPools": ...,
}

parent.create_network(**kwargs)
```

1. See [:material-code-braces: CreateNetworkRequestRequestTypeDef](./type_defs.md#createnetworkrequestrequesttypedef) 

### create\_node

Create a Node in the specified Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").create_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_node.html)

```python
# create_node method definition

await def create_node(
    self,
    *,
    ClusterId: str,
    Name: str = ...,
    NodeInterfaceMappings: Sequence[NodeInterfaceMappingCreateRequestTypeDef] = ...,  # (1)
    RequestId: str = ...,
    Role: NodeRoleType = ...,  # (2)
    Tags: Mapping[str, str] = ...,
) -> CreateNodeResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: NodeInterfaceMappingCreateRequestTypeDef](./type_defs.md#nodeinterfacemappingcreaterequesttypedef) 
2. See [:material-code-brackets: NodeRoleType](./literals.md#noderoletype) 
3. See [:material-code-braces: CreateNodeResponseTypeDef](./type_defs.md#createnoderesponsetypedef) 


```python
# create_node method usage example with argument unpacking

kwargs: CreateNodeRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.create_node(**kwargs)
```

1. See [:material-code-braces: CreateNodeRequestRequestTypeDef](./type_defs.md#createnoderequestrequesttypedef) 

### create\_node\_registration\_script

Create the Register Node script for all the nodes intended for a specific
Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").create_node_registration_script` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/create_node_registration_script.html)

```python
# create_node_registration_script method definition

await def create_node_registration_script(
    self,
    *,
    ClusterId: str,
    Id: str = ...,
    Name: str = ...,
    NodeInterfaceMappings: Sequence[NodeInterfaceMappingTypeDef] = ...,  # (1)
    RequestId: str = ...,
    Role: NodeRoleType = ...,  # (2)
) -> CreateNodeRegistrationScriptResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: NodeInterfaceMappingTypeDef](./type_defs.md#nodeinterfacemappingtypedef) 
2. See [:material-code-brackets: NodeRoleType](./literals.md#noderoletype) 
3. See [:material-code-braces: CreateNodeRegistrationScriptResponseTypeDef](./type_defs.md#createnoderegistrationscriptresponsetypedef) 


```python
# create_node_registration_script method usage example with argument unpacking

kwargs: CreateNodeRegistrationScriptRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.create_node_registration_script(**kwargs)
```

1. See [:material-code-braces: CreateNodeRegistrationScriptRequestRequestTypeDef](./type_defs.md#createnoderegistrationscriptrequestrequesttypedef) 

### delete\_channel\_placement\_group

Delete the specified ChannelPlacementGroup that exists in the specified Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").delete_channel_placement_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_channel_placement_group.html)

```python
# delete_channel_placement_group method definition

await def delete_channel_placement_group(
    self,
    *,
    ChannelPlacementGroupId: str,
    ClusterId: str,
) -> DeleteChannelPlacementGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteChannelPlacementGroupResponseTypeDef](./type_defs.md#deletechannelplacementgroupresponsetypedef) 


```python
# delete_channel_placement_group method usage example with argument unpacking

kwargs: DeleteChannelPlacementGroupRequestRequestTypeDef = {  # (1)
    "ChannelPlacementGroupId": ...,
    "ClusterId": ...,
}

parent.delete_channel_placement_group(**kwargs)
```

1. See [:material-code-braces: DeleteChannelPlacementGroupRequestRequestTypeDef](./type_defs.md#deletechannelplacementgrouprequestrequesttypedef) 

### delete\_cluster

Delete a Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").delete_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_cluster.html)

```python
# delete_cluster method definition

await def delete_cluster(
    self,
    *,
    ClusterId: str,
) -> DeleteClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteClusterResponseTypeDef](./type_defs.md#deleteclusterresponsetypedef) 


```python
# delete_cluster method usage example with argument unpacking

kwargs: DeleteClusterRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.delete_cluster(**kwargs)
```

1. See [:material-code-braces: DeleteClusterRequestRequestTypeDef](./type_defs.md#deleteclusterrequestrequesttypedef) 

### delete\_network

Delete a Network.

Type annotations and code completion for `#!python session.create_client("medialive").delete_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_network.html)

```python
# delete_network method definition

await def delete_network(
    self,
    *,
    NetworkId: str,
) -> DeleteNetworkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteNetworkResponseTypeDef](./type_defs.md#deletenetworkresponsetypedef) 


```python
# delete_network method usage example with argument unpacking

kwargs: DeleteNetworkRequestRequestTypeDef = {  # (1)
    "NetworkId": ...,
}

parent.delete_network(**kwargs)
```

1. See [:material-code-braces: DeleteNetworkRequestRequestTypeDef](./type_defs.md#deletenetworkrequestrequesttypedef) 

### delete\_node

Delete a Node.

Type annotations and code completion for `#!python session.create_client("medialive").delete_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/delete_node.html)

```python
# delete_node method definition

await def delete_node(
    self,
    *,
    ClusterId: str,
    NodeId: str,
) -> DeleteNodeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteNodeResponseTypeDef](./type_defs.md#deletenoderesponsetypedef) 


```python
# delete_node method usage example with argument unpacking

kwargs: DeleteNodeRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
    "NodeId": ...,
}

parent.delete_node(**kwargs)
```

1. See [:material-code-braces: DeleteNodeRequestRequestTypeDef](./type_defs.md#deletenoderequestrequesttypedef) 

### describe\_channel\_placement\_group

Get details about a ChannelPlacementGroup.

Type annotations and code completion for `#!python session.create_client("medialive").describe_channel_placement_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_channel_placement_group.html)

```python
# describe_channel_placement_group method definition

await def describe_channel_placement_group(
    self,
    *,
    ChannelPlacementGroupId: str,
    ClusterId: str,
) -> DescribeChannelPlacementGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeChannelPlacementGroupResponseTypeDef](./type_defs.md#describechannelplacementgroupresponsetypedef) 


```python
# describe_channel_placement_group method usage example with argument unpacking

kwargs: DescribeChannelPlacementGroupRequestRequestTypeDef = {  # (1)
    "ChannelPlacementGroupId": ...,
    "ClusterId": ...,
}

parent.describe_channel_placement_group(**kwargs)
```

1. See [:material-code-braces: DescribeChannelPlacementGroupRequestRequestTypeDef](./type_defs.md#describechannelplacementgrouprequestrequesttypedef) 

### describe\_cluster

Get details about a Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").describe_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_cluster.html)

```python
# describe_cluster method definition

await def describe_cluster(
    self,
    *,
    ClusterId: str,
) -> DescribeClusterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeClusterResponseTypeDef](./type_defs.md#describeclusterresponsetypedef) 


```python
# describe_cluster method usage example with argument unpacking

kwargs: DescribeClusterRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.describe_cluster(**kwargs)
```

1. See [:material-code-braces: DescribeClusterRequestRequestTypeDef](./type_defs.md#describeclusterrequestrequesttypedef) 

### describe\_network

Get details about a Network.

Type annotations and code completion for `#!python session.create_client("medialive").describe_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_network.html)

```python
# describe_network method definition

await def describe_network(
    self,
    *,
    NetworkId: str,
) -> DescribeNetworkResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNetworkResponseTypeDef](./type_defs.md#describenetworkresponsetypedef) 


```python
# describe_network method usage example with argument unpacking

kwargs: DescribeNetworkRequestRequestTypeDef = {  # (1)
    "NetworkId": ...,
}

parent.describe_network(**kwargs)
```

1. See [:material-code-braces: DescribeNetworkRequestRequestTypeDef](./type_defs.md#describenetworkrequestrequesttypedef) 

### describe\_node

Get details about a Node in the specified Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").describe_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/describe_node.html)

```python
# describe_node method definition

await def describe_node(
    self,
    *,
    ClusterId: str,
    NodeId: str,
) -> DescribeNodeResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeNodeResponseTypeDef](./type_defs.md#describenoderesponsetypedef) 


```python
# describe_node method usage example with argument unpacking

kwargs: DescribeNodeRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
    "NodeId": ...,
}

parent.describe_node(**kwargs)
```

1. See [:material-code-braces: DescribeNodeRequestRequestTypeDef](./type_defs.md#describenoderequestrequesttypedef) 

### list\_channel\_placement\_groups

Retrieve the list of ChannelPlacementGroups in the specified Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").list_channel_placement_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_channel_placement_groups.html)

```python
# list_channel_placement_groups method definition

await def list_channel_placement_groups(
    self,
    *,
    ClusterId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListChannelPlacementGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListChannelPlacementGroupsResponseTypeDef](./type_defs.md#listchannelplacementgroupsresponsetypedef) 


```python
# list_channel_placement_groups method usage example with argument unpacking

kwargs: ListChannelPlacementGroupsRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.list_channel_placement_groups(**kwargs)
```

1. See [:material-code-braces: ListChannelPlacementGroupsRequestRequestTypeDef](./type_defs.md#listchannelplacementgroupsrequestrequesttypedef) 

### list\_clusters

Retrieve the list of Clusters.

Type annotations and code completion for `#!python session.create_client("medialive").list_clusters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_clusters.html)

```python
# list_clusters method definition

await def list_clusters(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListClustersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListClustersResponseTypeDef](./type_defs.md#listclustersresponsetypedef) 


```python
# list_clusters method usage example with argument unpacking

kwargs: ListClustersRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_clusters(**kwargs)
```

1. See [:material-code-braces: ListClustersRequestRequestTypeDef](./type_defs.md#listclustersrequestrequesttypedef) 

### list\_networks

Retrieve the list of Networks.

Type annotations and code completion for `#!python session.create_client("medialive").list_networks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_networks.html)

```python
# list_networks method definition

await def list_networks(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListNetworksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNetworksResponseTypeDef](./type_defs.md#listnetworksresponsetypedef) 


```python
# list_networks method usage example with argument unpacking

kwargs: ListNetworksRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_networks(**kwargs)
```

1. See [:material-code-braces: ListNetworksRequestRequestTypeDef](./type_defs.md#listnetworksrequestrequesttypedef) 

### list\_nodes

Retrieve the list of Nodes.

Type annotations and code completion for `#!python session.create_client("medialive").list_nodes` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_nodes.html)

```python
# list_nodes method definition

await def list_nodes(
    self,
    *,
    ClusterId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListNodesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNodesResponseTypeDef](./type_defs.md#listnodesresponsetypedef) 


```python
# list_nodes method usage example with argument unpacking

kwargs: ListNodesRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.list_nodes(**kwargs)
```

1. See [:material-code-braces: ListNodesRequestRequestTypeDef](./type_defs.md#listnodesrequestrequesttypedef) 

### update\_channel\_placement\_group

Change the settings for a ChannelPlacementGroup.

Type annotations and code completion for `#!python session.create_client("medialive").update_channel_placement_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_channel_placement_group.html)

```python
# update_channel_placement_group method definition

await def update_channel_placement_group(
    self,
    *,
    ChannelPlacementGroupId: str,
    ClusterId: str,
    Name: str = ...,
    Nodes: Sequence[str] = ...,
) -> UpdateChannelPlacementGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateChannelPlacementGroupResponseTypeDef](./type_defs.md#updatechannelplacementgroupresponsetypedef) 


```python
# update_channel_placement_group method usage example with argument unpacking

kwargs: UpdateChannelPlacementGroupRequestRequestTypeDef = {  # (1)
    "ChannelPlacementGroupId": ...,
    "ClusterId": ...,
}

parent.update_channel_placement_group(**kwargs)
```

1. See [:material-code-braces: UpdateChannelPlacementGroupRequestRequestTypeDef](./type_defs.md#updatechannelplacementgrouprequestrequesttypedef) 

### update\_cluster

Change the settings for a Cluster.

Type annotations and code completion for `#!python session.create_client("medialive").update_cluster` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_cluster.html)

```python
# update_cluster method definition

await def update_cluster(
    self,
    *,
    ClusterId: str,
    Name: str = ...,
    NetworkSettings: ClusterNetworkSettingsUpdateRequestTypeDef = ...,  # (1)
) -> UpdateClusterResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ClusterNetworkSettingsUpdateRequestTypeDef](./type_defs.md#clusternetworksettingsupdaterequesttypedef) 
2. See [:material-code-braces: UpdateClusterResponseTypeDef](./type_defs.md#updateclusterresponsetypedef) 


```python
# update_cluster method usage example with argument unpacking

kwargs: UpdateClusterRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
}

parent.update_cluster(**kwargs)
```

1. See [:material-code-braces: UpdateClusterRequestRequestTypeDef](./type_defs.md#updateclusterrequestrequesttypedef) 

### update\_network

Change the settings for a Network.

Type annotations and code completion for `#!python session.create_client("medialive").update_network` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_network.html)

```python
# update_network method definition

await def update_network(
    self,
    *,
    NetworkId: str,
    IpPools: Sequence[IpPoolUpdateRequestTypeDef] = ...,  # (1)
    Name: str = ...,
    Routes: Sequence[RouteUpdateRequestTypeDef] = ...,  # (2)
) -> UpdateNetworkResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: IpPoolUpdateRequestTypeDef](./type_defs.md#ippoolupdaterequesttypedef) 
2. See [:material-code-braces: RouteUpdateRequestTypeDef](./type_defs.md#routeupdaterequesttypedef) 
3. See [:material-code-braces: UpdateNetworkResponseTypeDef](./type_defs.md#updatenetworkresponsetypedef) 


```python
# update_network method usage example with argument unpacking

kwargs: UpdateNetworkRequestRequestTypeDef = {  # (1)
    "NetworkId": ...,
}

parent.update_network(**kwargs)
```

1. See [:material-code-braces: UpdateNetworkRequestRequestTypeDef](./type_defs.md#updatenetworkrequestrequesttypedef) 

### update\_node

Change the settings for a Node.

Type annotations and code completion for `#!python session.create_client("medialive").update_node` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_node.html)

```python
# update_node method definition

await def update_node(
    self,
    *,
    ClusterId: str,
    NodeId: str,
    Name: str = ...,
    Role: NodeRoleType = ...,  # (1)
) -> UpdateNodeResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NodeRoleType](./literals.md#noderoletype) 
2. See [:material-code-braces: UpdateNodeResponseTypeDef](./type_defs.md#updatenoderesponsetypedef) 


```python
# update_node method usage example with argument unpacking

kwargs: UpdateNodeRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
    "NodeId": ...,
}

parent.update_node(**kwargs)
```

1. See [:material-code-braces: UpdateNodeRequestRequestTypeDef](./type_defs.md#updatenoderequestrequesttypedef) 

### update\_node\_state

Update the state of a node.

Type annotations and code completion for `#!python session.create_client("medialive").update_node_state` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/update_node_state.html)

```python
# update_node_state method definition

await def update_node_state(
    self,
    *,
    ClusterId: str,
    NodeId: str,
    State: UpdateNodeStateType = ...,  # (1)
) -> UpdateNodeStateResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: UpdateNodeStateType](./literals.md#updatenodestatetype) 
2. See [:material-code-braces: UpdateNodeStateResponseTypeDef](./type_defs.md#updatenodestateresponsetypedef) 


```python
# update_node_state method usage example with argument unpacking

kwargs: UpdateNodeStateRequestRequestTypeDef = {  # (1)
    "ClusterId": ...,
    "NodeId": ...,
}

parent.update_node_state(**kwargs)
```

1. See [:material-code-braces: UpdateNodeStateRequestRequestTypeDef](./type_defs.md#updatenodestaterequestrequesttypedef) 

### list\_versions

Retrieves an array of all the encoder engine versions that are available in
this AWS account.

Type annotations and code completion for `#!python session.create_client("medialive").list_versions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive/client/list_versions.html)

```python
# list_versions method definition

await def list_versions(
    self,
) -> ListVersionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListVersionsResponseTypeDef](./type_defs.md#listversionsresponsetypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("medialive").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("medialive").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("medialive").get_paginator` method with overloads.

- `client.get_paginator("describe_schedule")` -> [DescribeSchedulePaginator](./paginators.md#describeschedulepaginator)
- `client.get_paginator("list_channel_placement_groups")` -> [ListChannelPlacementGroupsPaginator](./paginators.md#listchannelplacementgroupspaginator)
- `client.get_paginator("list_channels")` -> [ListChannelsPaginator](./paginators.md#listchannelspaginator)
- `client.get_paginator("list_cloud_watch_alarm_template_groups")` -> [ListCloudWatchAlarmTemplateGroupsPaginator](./paginators.md#listcloudwatchalarmtemplategroupspaginator)
- `client.get_paginator("list_cloud_watch_alarm_templates")` -> [ListCloudWatchAlarmTemplatesPaginator](./paginators.md#listcloudwatchalarmtemplatespaginator)
- `client.get_paginator("list_clusters")` -> [ListClustersPaginator](./paginators.md#listclusterspaginator)
- `client.get_paginator("list_event_bridge_rule_template_groups")` -> [ListEventBridgeRuleTemplateGroupsPaginator](./paginators.md#listeventbridgeruletemplategroupspaginator)
- `client.get_paginator("list_event_bridge_rule_templates")` -> [ListEventBridgeRuleTemplatesPaginator](./paginators.md#listeventbridgeruletemplatespaginator)
- `client.get_paginator("list_input_device_transfers")` -> [ListInputDeviceTransfersPaginator](./paginators.md#listinputdevicetransferspaginator)
- `client.get_paginator("list_input_devices")` -> [ListInputDevicesPaginator](./paginators.md#listinputdevicespaginator)
- `client.get_paginator("list_input_security_groups")` -> [ListInputSecurityGroupsPaginator](./paginators.md#listinputsecuritygroupspaginator)
- `client.get_paginator("list_inputs")` -> [ListInputsPaginator](./paginators.md#listinputspaginator)
- `client.get_paginator("list_multiplex_programs")` -> [ListMultiplexProgramsPaginator](./paginators.md#listmultiplexprogramspaginator)
- `client.get_paginator("list_multiplexes")` -> [ListMultiplexesPaginator](./paginators.md#listmultiplexespaginator)
- `client.get_paginator("list_networks")` -> [ListNetworksPaginator](./paginators.md#listnetworkspaginator)
- `client.get_paginator("list_nodes")` -> [ListNodesPaginator](./paginators.md#listnodespaginator)
- `client.get_paginator("list_offerings")` -> [ListOfferingsPaginator](./paginators.md#listofferingspaginator)
- `client.get_paginator("list_reservations")` -> [ListReservationsPaginator](./paginators.md#listreservationspaginator)
- `client.get_paginator("list_signal_maps")` -> [ListSignalMapsPaginator](./paginators.md#listsignalmapspaginator)




### get_waiter

Type annotations and code completion for `#!python session.create_client("medialive").get_waiter` method with overloads.

- `client.get_waiter("channel_created")` -> [ChannelCreatedWaiter](./waiters.md#channelcreatedwaiter)
- `client.get_waiter("channel_deleted")` -> [ChannelDeletedWaiter](./waiters.md#channeldeletedwaiter)
- `client.get_waiter("channel_placement_group_assigned")` -> [ChannelPlacementGroupAssignedWaiter](./waiters.md#channelplacementgroupassignedwaiter)
- `client.get_waiter("channel_placement_group_deleted")` -> [ChannelPlacementGroupDeletedWaiter](./waiters.md#channelplacementgroupdeletedwaiter)
- `client.get_waiter("channel_placement_group_unassigned")` -> [ChannelPlacementGroupUnassignedWaiter](./waiters.md#channelplacementgroupunassignedwaiter)
- `client.get_waiter("channel_running")` -> [ChannelRunningWaiter](./waiters.md#channelrunningwaiter)
- `client.get_waiter("channel_stopped")` -> [ChannelStoppedWaiter](./waiters.md#channelstoppedwaiter)
- `client.get_waiter("cluster_created")` -> [ClusterCreatedWaiter](./waiters.md#clustercreatedwaiter)
- `client.get_waiter("cluster_deleted")` -> [ClusterDeletedWaiter](./waiters.md#clusterdeletedwaiter)
- `client.get_waiter("input_attached")` -> [InputAttachedWaiter](./waiters.md#inputattachedwaiter)
- `client.get_waiter("input_deleted")` -> [InputDeletedWaiter](./waiters.md#inputdeletedwaiter)
- `client.get_waiter("input_detached")` -> [InputDetachedWaiter](./waiters.md#inputdetachedwaiter)
- `client.get_waiter("multiplex_created")` -> [MultiplexCreatedWaiter](./waiters.md#multiplexcreatedwaiter)
- `client.get_waiter("multiplex_deleted")` -> [MultiplexDeletedWaiter](./waiters.md#multiplexdeletedwaiter)
- `client.get_waiter("multiplex_running")` -> [MultiplexRunningWaiter](./waiters.md#multiplexrunningwaiter)
- `client.get_waiter("multiplex_stopped")` -> [MultiplexStoppedWaiter](./waiters.md#multiplexstoppedwaiter)
- `client.get_waiter("node_deregistered")` -> [NodeDeregisteredWaiter](./waiters.md#nodederegisteredwaiter)
- `client.get_waiter("node_registered")` -> [NodeRegisteredWaiter](./waiters.md#noderegisteredwaiter)
- `client.get_waiter("signal_map_created")` -> [SignalMapCreatedWaiter](./waiters.md#signalmapcreatedwaiter)
- `client.get_waiter("signal_map_monitor_deleted")` -> [SignalMapMonitorDeletedWaiter](./waiters.md#signalmapmonitordeletedwaiter)
- `client.get_waiter("signal_map_monitor_deployed")` -> [SignalMapMonitorDeployedWaiter](./waiters.md#signalmapmonitordeployedwaiter)
- `client.get_waiter("signal_map_updated")` -> [SignalMapUpdatedWaiter](./waiters.md#signalmapupdatedwaiter)


# IoTWirelessClient

> [Index](../README.md) > [IoTWireless](./README.md) > IoTWirelessClient

!!! note ""

    Auto-generated documentation for [IoTWireless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#iotwireless)
    type annotations stubs module [types-aiobotocore-iotwireless](https://pypi.org/project/types-aiobotocore-iotwireless/).

## IoTWirelessClient

Type annotations and code completion for `#!python session.create_client("iotwireless")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client)

```python
# IoTWirelessClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_iotwireless.client import IoTWirelessClient

session = get_session()
async with session.create_client("iotwireless") as client:
    client: IoTWirelessClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("iotwireless").exceptions` structure.

```python
# IoTWirelessClient.exceptions usage example

async with session.create_client("iotwireless") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.TooManyTagsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# IoTWirelessClient usage type checking example

from types_aiobotocore_iotwireless.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("iotwireless").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("iotwireless").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/generate_presigned_url.html)

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


### associate\_aws\_account\_with\_partner\_account

Associates a partner account with your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").associate_aws_account_with_partner_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/associate_aws_account_with_partner_account.html)

```python
# associate_aws_account_with_partner_account method definition

await def associate_aws_account_with_partner_account(
    self,
    *,
    Sidewalk: SidewalkAccountInfoTypeDef,  # (1)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> AssociateAwsAccountWithPartnerAccountResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SidewalkAccountInfoTypeDef](./type_defs.md#sidewalkaccountinfotypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: AssociateAwsAccountWithPartnerAccountResponseTypeDef](./type_defs.md#associateawsaccountwithpartneraccountresponsetypedef) 


```python
# associate_aws_account_with_partner_account method usage example with argument unpacking

kwargs: AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef = {  # (1)
    "Sidewalk": ...,
}

parent.associate_aws_account_with_partner_account(**kwargs)
```

1. See [:material-code-braces: AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef](./type_defs.md#associateawsaccountwithpartneraccountrequestrequesttypedef) 

### associate\_multicast\_group\_with\_fuota\_task

Associate a multicast group with a FUOTA task.

Type annotations and code completion for `#!python session.create_client("iotwireless").associate_multicast_group_with_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/associate_multicast_group_with_fuota_task.html)

```python
# associate_multicast_group_with_fuota_task method definition

await def associate_multicast_group_with_fuota_task(
    self,
    *,
    Id: str,
    MulticastGroupId: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_multicast_group_with_fuota_task method usage example with argument unpacking

kwargs: AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "MulticastGroupId": ...,
}

parent.associate_multicast_group_with_fuota_task(**kwargs)
```

1. See [:material-code-braces: AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef](./type_defs.md#associatemulticastgroupwithfuotataskrequestrequesttypedef) 

### associate\_wireless\_device\_with\_fuota\_task

Associate a wireless device with a FUOTA task.

Type annotations and code completion for `#!python session.create_client("iotwireless").associate_wireless_device_with_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/associate_wireless_device_with_fuota_task.html)

```python
# associate_wireless_device_with_fuota_task method definition

await def associate_wireless_device_with_fuota_task(
    self,
    *,
    Id: str,
    WirelessDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_wireless_device_with_fuota_task method usage example with argument unpacking

kwargs: AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "WirelessDeviceId": ...,
}

parent.associate_wireless_device_with_fuota_task(**kwargs)
```

1. See [:material-code-braces: AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewithfuotataskrequestrequesttypedef) 

### associate\_wireless\_device\_with\_multicast\_group

Associates a wireless device with a multicast group.

Type annotations and code completion for `#!python session.create_client("iotwireless").associate_wireless_device_with_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/associate_wireless_device_with_multicast_group.html)

```python
# associate_wireless_device_with_multicast_group method definition

await def associate_wireless_device_with_multicast_group(
    self,
    *,
    Id: str,
    WirelessDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_wireless_device_with_multicast_group method usage example with argument unpacking

kwargs: AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "WirelessDeviceId": ...,
}

parent.associate_wireless_device_with_multicast_group(**kwargs)
```

1. See [:material-code-braces: AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewithmulticastgrouprequestrequesttypedef) 

### associate\_wireless\_device\_with\_thing

Associates a wireless device with a thing.

Type annotations and code completion for `#!python session.create_client("iotwireless").associate_wireless_device_with_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/associate_wireless_device_with_thing.html)

```python
# associate_wireless_device_with_thing method definition

await def associate_wireless_device_with_thing(
    self,
    *,
    Id: str,
    ThingArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_wireless_device_with_thing method usage example with argument unpacking

kwargs: AssociateWirelessDeviceWithThingRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "ThingArn": ...,
}

parent.associate_wireless_device_with_thing(**kwargs)
```

1. See [:material-code-braces: AssociateWirelessDeviceWithThingRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewiththingrequestrequesttypedef) 

### associate\_wireless\_gateway\_with\_certificate

Associates a wireless gateway with a certificate.

Type annotations and code completion for `#!python session.create_client("iotwireless").associate_wireless_gateway_with_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/associate_wireless_gateway_with_certificate.html)

```python
# associate_wireless_gateway_with_certificate method definition

await def associate_wireless_gateway_with_certificate(
    self,
    *,
    Id: str,
    IotCertificateId: str,
) -> AssociateWirelessGatewayWithCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateWirelessGatewayWithCertificateResponseTypeDef](./type_defs.md#associatewirelessgatewaywithcertificateresponsetypedef) 


```python
# associate_wireless_gateway_with_certificate method usage example with argument unpacking

kwargs: AssociateWirelessGatewayWithCertificateRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "IotCertificateId": ...,
}

parent.associate_wireless_gateway_with_certificate(**kwargs)
```

1. See [:material-code-braces: AssociateWirelessGatewayWithCertificateRequestRequestTypeDef](./type_defs.md#associatewirelessgatewaywithcertificaterequestrequesttypedef) 

### associate\_wireless\_gateway\_with\_thing

Associates a wireless gateway with a thing.

Type annotations and code completion for `#!python session.create_client("iotwireless").associate_wireless_gateway_with_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/associate_wireless_gateway_with_thing.html)

```python
# associate_wireless_gateway_with_thing method definition

await def associate_wireless_gateway_with_thing(
    self,
    *,
    Id: str,
    ThingArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# associate_wireless_gateway_with_thing method usage example with argument unpacking

kwargs: AssociateWirelessGatewayWithThingRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "ThingArn": ...,
}

parent.associate_wireless_gateway_with_thing(**kwargs)
```

1. See [:material-code-braces: AssociateWirelessGatewayWithThingRequestRequestTypeDef](./type_defs.md#associatewirelessgatewaywiththingrequestrequesttypedef) 

### cancel\_multicast\_group\_session

Cancels an existing multicast group session.

Type annotations and code completion for `#!python session.create_client("iotwireless").cancel_multicast_group_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/cancel_multicast_group_session.html)

```python
# cancel_multicast_group_session method definition

await def cancel_multicast_group_session(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# cancel_multicast_group_session method usage example with argument unpacking

kwargs: CancelMulticastGroupSessionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.cancel_multicast_group_session(**kwargs)
```

1. See [:material-code-braces: CancelMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#cancelmulticastgroupsessionrequestrequesttypedef) 

### create\_destination

Creates a new destination that maps a device message to an AWS IoT rule.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_destination.html)

```python
# create_destination method definition

await def create_destination(
    self,
    *,
    Name: str,
    ExpressionType: ExpressionTypeType,  # (1)
    Expression: str,
    RoleArn: str,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ClientRequestToken: str = ...,
) -> CreateDestinationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef) 


```python
# create_destination method usage example with argument unpacking

kwargs: CreateDestinationRequestRequestTypeDef = {  # (1)
    "Name": ...,
    "ExpressionType": ...,
    "Expression": ...,
    "RoleArn": ...,
}

parent.create_destination(**kwargs)
```

1. See [:material-code-braces: CreateDestinationRequestRequestTypeDef](./type_defs.md#createdestinationrequestrequesttypedef) 

### create\_device\_profile

Creates a new device profile.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_device_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_device_profile.html)

```python
# create_device_profile method definition

await def create_device_profile(
    self,
    *,
    Name: str = ...,
    LoRaWAN: LoRaWANDeviceProfileTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ClientRequestToken: str = ...,
    Sidewalk: Mapping[str, Any] = ...,
) -> CreateDeviceProfileResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LoRaWANDeviceProfileTypeDef](./type_defs.md#lorawandeviceprofiletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateDeviceProfileResponseTypeDef](./type_defs.md#createdeviceprofileresponsetypedef) 


```python
# create_device_profile method usage example with argument unpacking

kwargs: CreateDeviceProfileRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_device_profile(**kwargs)
```

1. See [:material-code-braces: CreateDeviceProfileRequestRequestTypeDef](./type_defs.md#createdeviceprofilerequestrequesttypedef) 

### create\_fuota\_task

Creates a FUOTA task.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_fuota_task.html)

```python
# create_fuota_task method definition

await def create_fuota_task(
    self,
    *,
    FirmwareUpdateImage: str,
    FirmwareUpdateRole: str,
    Name: str = ...,
    Description: str = ...,
    ClientRequestToken: str = ...,
    LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    RedundancyPercent: int = ...,
    FragmentSizeBytes: int = ...,
    FragmentIntervalMS: int = ...,
    Descriptor: str = ...,
) -> CreateFuotaTaskResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LoRaWANFuotaTaskTypeDef](./type_defs.md#lorawanfuotatasktypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateFuotaTaskResponseTypeDef](./type_defs.md#createfuotataskresponsetypedef) 


```python
# create_fuota_task method usage example with argument unpacking

kwargs: CreateFuotaTaskRequestRequestTypeDef = {  # (1)
    "FirmwareUpdateImage": ...,
    "FirmwareUpdateRole": ...,
}

parent.create_fuota_task(**kwargs)
```

1. See [:material-code-braces: CreateFuotaTaskRequestRequestTypeDef](./type_defs.md#createfuotataskrequestrequesttypedef) 

### create\_multicast\_group

Creates a multicast group.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_multicast_group.html)

```python
# create_multicast_group method definition

await def create_multicast_group(
    self,
    *,
    LoRaWAN: LoRaWANMulticastTypeDef,  # (1)
    Name: str = ...,
    Description: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateMulticastGroupResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LoRaWANMulticastTypeDef](./type_defs.md#lorawanmulticasttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateMulticastGroupResponseTypeDef](./type_defs.md#createmulticastgroupresponsetypedef) 


```python
# create_multicast_group method usage example with argument unpacking

kwargs: CreateMulticastGroupRequestRequestTypeDef = {  # (1)
    "LoRaWAN": ...,
}

parent.create_multicast_group(**kwargs)
```

1. See [:material-code-braces: CreateMulticastGroupRequestRequestTypeDef](./type_defs.md#createmulticastgrouprequestrequesttypedef) 

### create\_network\_analyzer\_configuration

Creates a new network analyzer configuration.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_network_analyzer_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_network_analyzer_configuration.html)

```python
# create_network_analyzer_configuration method definition

await def create_network_analyzer_configuration(
    self,
    *,
    Name: str,
    TraceContent: TraceContentTypeDef = ...,  # (1)
    WirelessDevices: Sequence[str] = ...,
    WirelessGateways: Sequence[str] = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ClientRequestToken: str = ...,
    MulticastGroups: Sequence[str] = ...,
) -> CreateNetworkAnalyzerConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: TraceContentTypeDef](./type_defs.md#tracecontenttypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateNetworkAnalyzerConfigurationResponseTypeDef](./type_defs.md#createnetworkanalyzerconfigurationresponsetypedef) 


```python
# create_network_analyzer_configuration method usage example with argument unpacking

kwargs: CreateNetworkAnalyzerConfigurationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_network_analyzer_configuration(**kwargs)
```

1. See [:material-code-braces: CreateNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#createnetworkanalyzerconfigurationrequestrequesttypedef) 

### create\_service\_profile

Creates a new service profile.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_service_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_service_profile.html)

```python
# create_service_profile method definition

await def create_service_profile(
    self,
    *,
    Name: str = ...,
    LoRaWAN: LoRaWANServiceProfileTypeDef = ...,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ClientRequestToken: str = ...,
) -> CreateServiceProfileResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LoRaWANServiceProfileTypeDef](./type_defs.md#lorawanserviceprofiletypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateServiceProfileResponseTypeDef](./type_defs.md#createserviceprofileresponsetypedef) 


```python
# create_service_profile method usage example with argument unpacking

kwargs: CreateServiceProfileRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.create_service_profile(**kwargs)
```

1. See [:material-code-braces: CreateServiceProfileRequestRequestTypeDef](./type_defs.md#createserviceprofilerequestrequesttypedef) 

### create\_wireless\_device

Provisions a wireless device.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_wireless_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_wireless_device.html)

```python
# create_wireless_device method definition

await def create_wireless_device(
    self,
    *,
    Type: WirelessDeviceTypeType,  # (1)
    DestinationName: str,
    Name: str = ...,
    Description: str = ...,
    ClientRequestToken: str = ...,
    LoRaWAN: LoRaWANDeviceTypeDef = ...,  # (2)
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    Positioning: PositioningConfigStatusType = ...,  # (4)
    Sidewalk: SidewalkCreateWirelessDeviceTypeDef = ...,  # (5)
) -> CreateWirelessDeviceResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
2. See [:material-code-braces: LoRaWANDeviceTypeDef](./type_defs.md#lorawandevicetypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-brackets: PositioningConfigStatusType](./literals.md#positioningconfigstatustype) 
5. See [:material-code-braces: SidewalkCreateWirelessDeviceTypeDef](./type_defs.md#sidewalkcreatewirelessdevicetypedef) 
6. See [:material-code-braces: CreateWirelessDeviceResponseTypeDef](./type_defs.md#createwirelessdeviceresponsetypedef) 


```python
# create_wireless_device method usage example with argument unpacking

kwargs: CreateWirelessDeviceRequestRequestTypeDef = {  # (1)
    "Type": ...,
    "DestinationName": ...,
}

parent.create_wireless_device(**kwargs)
```

1. See [:material-code-braces: CreateWirelessDeviceRequestRequestTypeDef](./type_defs.md#createwirelessdevicerequestrequesttypedef) 

### create\_wireless\_gateway

Provisions a wireless gateway.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_wireless_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_wireless_gateway.html)

```python
# create_wireless_gateway method definition

await def create_wireless_gateway(
    self,
    *,
    LoRaWAN: LoRaWANGatewayTypeDef,  # (1)
    Name: str = ...,
    Description: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    ClientRequestToken: str = ...,
) -> CreateWirelessGatewayResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: LoRaWANGatewayTypeDef](./type_defs.md#lorawangatewaytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateWirelessGatewayResponseTypeDef](./type_defs.md#createwirelessgatewayresponsetypedef) 


```python
# create_wireless_gateway method usage example with argument unpacking

kwargs: CreateWirelessGatewayRequestRequestTypeDef = {  # (1)
    "LoRaWAN": ...,
}

parent.create_wireless_gateway(**kwargs)
```

1. See [:material-code-braces: CreateWirelessGatewayRequestRequestTypeDef](./type_defs.md#createwirelessgatewayrequestrequesttypedef) 

### create\_wireless\_gateway\_task

Creates a task for a wireless gateway.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_wireless_gateway_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_wireless_gateway_task.html)

```python
# create_wireless_gateway_task method definition

await def create_wireless_gateway_task(
    self,
    *,
    Id: str,
    WirelessGatewayTaskDefinitionId: str,
) -> CreateWirelessGatewayTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateWirelessGatewayTaskResponseTypeDef](./type_defs.md#createwirelessgatewaytaskresponsetypedef) 


```python
# create_wireless_gateway_task method usage example with argument unpacking

kwargs: CreateWirelessGatewayTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "WirelessGatewayTaskDefinitionId": ...,
}

parent.create_wireless_gateway_task(**kwargs)
```

1. See [:material-code-braces: CreateWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#createwirelessgatewaytaskrequestrequesttypedef) 

### create\_wireless\_gateway\_task\_definition

Creates a gateway task definition.

Type annotations and code completion for `#!python session.create_client("iotwireless").create_wireless_gateway_task_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/create_wireless_gateway_task_definition.html)

```python
# create_wireless_gateway_task_definition method definition

await def create_wireless_gateway_task_definition(
    self,
    *,
    AutoCreateTasks: bool,
    Name: str = ...,
    Update: UpdateWirelessGatewayTaskCreateTypeDef = ...,  # (1)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateWirelessGatewayTaskDefinitionResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: UpdateWirelessGatewayTaskCreateTypeDef](./type_defs.md#updatewirelessgatewaytaskcreatetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateWirelessGatewayTaskDefinitionResponseTypeDef](./type_defs.md#createwirelessgatewaytaskdefinitionresponsetypedef) 


```python
# create_wireless_gateway_task_definition method usage example with argument unpacking

kwargs: CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef = {  # (1)
    "AutoCreateTasks": ...,
}

parent.create_wireless_gateway_task_definition(**kwargs)
```

1. See [:material-code-braces: CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#createwirelessgatewaytaskdefinitionrequestrequesttypedef) 

### delete\_destination

Deletes a destination.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_destination.html)

```python
# delete_destination method definition

await def delete_destination(
    self,
    *,
    Name: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_destination method usage example with argument unpacking

kwargs: DeleteDestinationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.delete_destination(**kwargs)
```

1. See [:material-code-braces: DeleteDestinationRequestRequestTypeDef](./type_defs.md#deletedestinationrequestrequesttypedef) 

### delete\_device\_profile

Deletes a device profile.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_device_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_device_profile.html)

```python
# delete_device_profile method definition

await def delete_device_profile(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_device_profile method usage example with argument unpacking

kwargs: DeleteDeviceProfileRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_device_profile(**kwargs)
```

1. See [:material-code-braces: DeleteDeviceProfileRequestRequestTypeDef](./type_defs.md#deletedeviceprofilerequestrequesttypedef) 

### delete\_fuota\_task

Deletes a FUOTA task.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_fuota_task.html)

```python
# delete_fuota_task method definition

await def delete_fuota_task(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_fuota_task method usage example with argument unpacking

kwargs: DeleteFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_fuota_task(**kwargs)
```

1. See [:material-code-braces: DeleteFuotaTaskRequestRequestTypeDef](./type_defs.md#deletefuotataskrequestrequesttypedef) 

### delete\_multicast\_group

Deletes a multicast group if it is not in use by a fuota task.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_multicast_group.html)

```python
# delete_multicast_group method definition

await def delete_multicast_group(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_multicast_group method usage example with argument unpacking

kwargs: DeleteMulticastGroupRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_multicast_group(**kwargs)
```

1. See [:material-code-braces: DeleteMulticastGroupRequestRequestTypeDef](./type_defs.md#deletemulticastgrouprequestrequesttypedef) 

### delete\_network\_analyzer\_configuration

Deletes a network analyzer configuration.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_network_analyzer_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_network_analyzer_configuration.html)

```python
# delete_network_analyzer_configuration method definition

await def delete_network_analyzer_configuration(
    self,
    *,
    ConfigurationName: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_network_analyzer_configuration method usage example with argument unpacking

kwargs: DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef = {  # (1)
    "ConfigurationName": ...,
}

parent.delete_network_analyzer_configuration(**kwargs)
```

1. See [:material-code-braces: DeleteNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#deletenetworkanalyzerconfigurationrequestrequesttypedef) 

### delete\_queued\_messages

Remove queued messages from the downlink queue.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_queued_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_queued_messages.html)

```python
# delete_queued_messages method definition

await def delete_queued_messages(
    self,
    *,
    Id: str,
    MessageId: str,
    WirelessDeviceType: WirelessDeviceTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 


```python
# delete_queued_messages method usage example with argument unpacking

kwargs: DeleteQueuedMessagesRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "MessageId": ...,
}

parent.delete_queued_messages(**kwargs)
```

1. See [:material-code-braces: DeleteQueuedMessagesRequestRequestTypeDef](./type_defs.md#deletequeuedmessagesrequestrequesttypedef) 

### delete\_service\_profile

Deletes a service profile.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_service_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_service_profile.html)

```python
# delete_service_profile method definition

await def delete_service_profile(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_service_profile method usage example with argument unpacking

kwargs: DeleteServiceProfileRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_service_profile(**kwargs)
```

1. See [:material-code-braces: DeleteServiceProfileRequestRequestTypeDef](./type_defs.md#deleteserviceprofilerequestrequesttypedef) 

### delete\_wireless\_device

Deletes a wireless device.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_wireless_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_wireless_device.html)

```python
# delete_wireless_device method definition

await def delete_wireless_device(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_wireless_device method usage example with argument unpacking

kwargs: DeleteWirelessDeviceRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_wireless_device(**kwargs)
```

1. See [:material-code-braces: DeleteWirelessDeviceRequestRequestTypeDef](./type_defs.md#deletewirelessdevicerequestrequesttypedef) 

### delete\_wireless\_device\_import\_task

Delete an import task.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_wireless_device_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_wireless_device_import_task.html)

```python
# delete_wireless_device_import_task method definition

await def delete_wireless_device_import_task(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_wireless_device_import_task method usage example with argument unpacking

kwargs: DeleteWirelessDeviceImportTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_wireless_device_import_task(**kwargs)
```

1. See [:material-code-braces: DeleteWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#deletewirelessdeviceimporttaskrequestrequesttypedef) 

### delete\_wireless\_gateway

Deletes a wireless gateway.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_wireless_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_wireless_gateway.html)

```python
# delete_wireless_gateway method definition

await def delete_wireless_gateway(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_wireless_gateway method usage example with argument unpacking

kwargs: DeleteWirelessGatewayRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_wireless_gateway(**kwargs)
```

1. See [:material-code-braces: DeleteWirelessGatewayRequestRequestTypeDef](./type_defs.md#deletewirelessgatewayrequestrequesttypedef) 

### delete\_wireless\_gateway\_task

Deletes a wireless gateway task.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_wireless_gateway_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_wireless_gateway_task.html)

```python
# delete_wireless_gateway_task method definition

await def delete_wireless_gateway_task(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_wireless_gateway_task method usage example with argument unpacking

kwargs: DeleteWirelessGatewayTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_wireless_gateway_task(**kwargs)
```

1. See [:material-code-braces: DeleteWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#deletewirelessgatewaytaskrequestrequesttypedef) 

### delete\_wireless\_gateway\_task\_definition

Deletes a wireless gateway task definition.

Type annotations and code completion for `#!python session.create_client("iotwireless").delete_wireless_gateway_task_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/delete_wireless_gateway_task_definition.html)

```python
# delete_wireless_gateway_task_definition method definition

await def delete_wireless_gateway_task_definition(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_wireless_gateway_task_definition method usage example with argument unpacking

kwargs: DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.delete_wireless_gateway_task_definition(**kwargs)
```

1. See [:material-code-braces: DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#deletewirelessgatewaytaskdefinitionrequestrequesttypedef) 

### deregister\_wireless\_device

Deregister a wireless device from AWS IoT Wireless.

Type annotations and code completion for `#!python session.create_client("iotwireless").deregister_wireless_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/deregister_wireless_device.html)

```python
# deregister_wireless_device method definition

await def deregister_wireless_device(
    self,
    *,
    Identifier: str,
    WirelessDeviceType: WirelessDeviceTypeType = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 


```python
# deregister_wireless_device method usage example with argument unpacking

kwargs: DeregisterWirelessDeviceRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
}

parent.deregister_wireless_device(**kwargs)
```

1. See [:material-code-braces: DeregisterWirelessDeviceRequestRequestTypeDef](./type_defs.md#deregisterwirelessdevicerequestrequesttypedef) 

### disassociate\_aws\_account\_from\_partner\_account

Disassociates your AWS account from a partner account.

Type annotations and code completion for `#!python session.create_client("iotwireless").disassociate_aws_account_from_partner_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/disassociate_aws_account_from_partner_account.html)

```python
# disassociate_aws_account_from_partner_account method definition

await def disassociate_aws_account_from_partner_account(
    self,
    *,
    PartnerAccountId: str,
    PartnerType: PartnerTypeType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PartnerTypeType](./literals.md#partnertypetype) 


```python
# disassociate_aws_account_from_partner_account method usage example with argument unpacking

kwargs: DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef = {  # (1)
    "PartnerAccountId": ...,
    "PartnerType": ...,
}

parent.disassociate_aws_account_from_partner_account(**kwargs)
```

1. See [:material-code-braces: DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef](./type_defs.md#disassociateawsaccountfrompartneraccountrequestrequesttypedef) 

### disassociate\_multicast\_group\_from\_fuota\_task

Disassociates a multicast group from a fuota task.

Type annotations and code completion for `#!python session.create_client("iotwireless").disassociate_multicast_group_from_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/disassociate_multicast_group_from_fuota_task.html)

```python
# disassociate_multicast_group_from_fuota_task method definition

await def disassociate_multicast_group_from_fuota_task(
    self,
    *,
    Id: str,
    MulticastGroupId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_multicast_group_from_fuota_task method usage example with argument unpacking

kwargs: DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "MulticastGroupId": ...,
}

parent.disassociate_multicast_group_from_fuota_task(**kwargs)
```

1. See [:material-code-braces: DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef](./type_defs.md#disassociatemulticastgroupfromfuotataskrequestrequesttypedef) 

### disassociate\_wireless\_device\_from\_fuota\_task

Disassociates a wireless device from a FUOTA task.

Type annotations and code completion for `#!python session.create_client("iotwireless").disassociate_wireless_device_from_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/disassociate_wireless_device_from_fuota_task.html)

```python
# disassociate_wireless_device_from_fuota_task method definition

await def disassociate_wireless_device_from_fuota_task(
    self,
    *,
    Id: str,
    WirelessDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_wireless_device_from_fuota_task method usage example with argument unpacking

kwargs: DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "WirelessDeviceId": ...,
}

parent.disassociate_wireless_device_from_fuota_task(**kwargs)
```

1. See [:material-code-braces: DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefromfuotataskrequestrequesttypedef) 

### disassociate\_wireless\_device\_from\_multicast\_group

Disassociates a wireless device from a multicast group.

Type annotations and code completion for `#!python session.create_client("iotwireless").disassociate_wireless_device_from_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/disassociate_wireless_device_from_multicast_group.html)

```python
# disassociate_wireless_device_from_multicast_group method definition

await def disassociate_wireless_device_from_multicast_group(
    self,
    *,
    Id: str,
    WirelessDeviceId: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_wireless_device_from_multicast_group method usage example with argument unpacking

kwargs: DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "WirelessDeviceId": ...,
}

parent.disassociate_wireless_device_from_multicast_group(**kwargs)
```

1. See [:material-code-braces: DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefrommulticastgrouprequestrequesttypedef) 

### disassociate\_wireless\_device\_from\_thing

Disassociates a wireless device from its currently associated thing.

Type annotations and code completion for `#!python session.create_client("iotwireless").disassociate_wireless_device_from_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/disassociate_wireless_device_from_thing.html)

```python
# disassociate_wireless_device_from_thing method definition

await def disassociate_wireless_device_from_thing(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_wireless_device_from_thing method usage example with argument unpacking

kwargs: DisassociateWirelessDeviceFromThingRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.disassociate_wireless_device_from_thing(**kwargs)
```

1. See [:material-code-braces: DisassociateWirelessDeviceFromThingRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefromthingrequestrequesttypedef) 

### disassociate\_wireless\_gateway\_from\_certificate

Disassociates a wireless gateway from its currently associated certificate.

Type annotations and code completion for `#!python session.create_client("iotwireless").disassociate_wireless_gateway_from_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/disassociate_wireless_gateway_from_certificate.html)

```python
# disassociate_wireless_gateway_from_certificate method definition

await def disassociate_wireless_gateway_from_certificate(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_wireless_gateway_from_certificate method usage example with argument unpacking

kwargs: DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.disassociate_wireless_gateway_from_certificate(**kwargs)
```

1. See [:material-code-braces: DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef](./type_defs.md#disassociatewirelessgatewayfromcertificaterequestrequesttypedef) 

### disassociate\_wireless\_gateway\_from\_thing

Disassociates a wireless gateway from its currently associated thing.

Type annotations and code completion for `#!python session.create_client("iotwireless").disassociate_wireless_gateway_from_thing` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/disassociate_wireless_gateway_from_thing.html)

```python
# disassociate_wireless_gateway_from_thing method definition

await def disassociate_wireless_gateway_from_thing(
    self,
    *,
    Id: str,
) -> Dict[str, Any]:
    ...
```



```python
# disassociate_wireless_gateway_from_thing method usage example with argument unpacking

kwargs: DisassociateWirelessGatewayFromThingRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.disassociate_wireless_gateway_from_thing(**kwargs)
```

1. See [:material-code-braces: DisassociateWirelessGatewayFromThingRequestRequestTypeDef](./type_defs.md#disassociatewirelessgatewayfromthingrequestrequesttypedef) 

### get\_destination

Gets information about a destination.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_destination.html)

```python
# get_destination method definition

await def get_destination(
    self,
    *,
    Name: str,
) -> GetDestinationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDestinationResponseTypeDef](./type_defs.md#getdestinationresponsetypedef) 


```python
# get_destination method usage example with argument unpacking

kwargs: GetDestinationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_destination(**kwargs)
```

1. See [:material-code-braces: GetDestinationRequestRequestTypeDef](./type_defs.md#getdestinationrequestrequesttypedef) 

### get\_device\_profile

Gets information about a device profile.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_device_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_device_profile.html)

```python
# get_device_profile method definition

await def get_device_profile(
    self,
    *,
    Id: str,
) -> GetDeviceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDeviceProfileResponseTypeDef](./type_defs.md#getdeviceprofileresponsetypedef) 


```python
# get_device_profile method usage example with argument unpacking

kwargs: GetDeviceProfileRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_device_profile(**kwargs)
```

1. See [:material-code-braces: GetDeviceProfileRequestRequestTypeDef](./type_defs.md#getdeviceprofilerequestrequesttypedef) 

### get\_event\_configuration\_by\_resource\_types

Get the event configuration based on resource types.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_event_configuration_by_resource_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_event_configuration_by_resource_types.html)

```python
# get_event_configuration_by_resource_types method definition

await def get_event_configuration_by_resource_types(
    self,
) -> GetEventConfigurationByResourceTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEventConfigurationByResourceTypesResponseTypeDef](./type_defs.md#geteventconfigurationbyresourcetypesresponsetypedef) 

### get\_fuota\_task

Gets information about a FUOTA task.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_fuota_task.html)

```python
# get_fuota_task method definition

await def get_fuota_task(
    self,
    *,
    Id: str,
) -> GetFuotaTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFuotaTaskResponseTypeDef](./type_defs.md#getfuotataskresponsetypedef) 


```python
# get_fuota_task method usage example with argument unpacking

kwargs: GetFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_fuota_task(**kwargs)
```

1. See [:material-code-braces: GetFuotaTaskRequestRequestTypeDef](./type_defs.md#getfuotataskrequestrequesttypedef) 

### get\_log\_levels\_by\_resource\_types

Returns current default log levels or log levels by resource types.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_log_levels_by_resource_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_log_levels_by_resource_types.html)

```python
# get_log_levels_by_resource_types method definition

await def get_log_levels_by_resource_types(
    self,
) -> GetLogLevelsByResourceTypesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetLogLevelsByResourceTypesResponseTypeDef](./type_defs.md#getloglevelsbyresourcetypesresponsetypedef) 

### get\_metric\_configuration

Get the metric configuration status for this AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_metric_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_metric_configuration.html)

```python
# get_metric_configuration method definition

await def get_metric_configuration(
    self,
) -> GetMetricConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMetricConfigurationResponseTypeDef](./type_defs.md#getmetricconfigurationresponsetypedef) 

### get\_metrics

Get the summary metrics for this AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_metrics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_metrics.html)

```python
# get_metrics method definition

await def get_metrics(
    self,
    *,
    SummaryMetricQueries: Sequence[SummaryMetricQueryTypeDef] = ...,  # (1)
) -> GetMetricsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SummaryMetricQueryTypeDef](./type_defs.md#summarymetricquerytypedef) 
2. See [:material-code-braces: GetMetricsResponseTypeDef](./type_defs.md#getmetricsresponsetypedef) 


```python
# get_metrics method usage example with argument unpacking

kwargs: GetMetricsRequestRequestTypeDef = {  # (1)
    "SummaryMetricQueries": ...,
}

parent.get_metrics(**kwargs)
```

1. See [:material-code-braces: GetMetricsRequestRequestTypeDef](./type_defs.md#getmetricsrequestrequesttypedef) 

### get\_multicast\_group

Gets information about a multicast group.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_multicast_group.html)

```python
# get_multicast_group method definition

await def get_multicast_group(
    self,
    *,
    Id: str,
) -> GetMulticastGroupResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMulticastGroupResponseTypeDef](./type_defs.md#getmulticastgroupresponsetypedef) 


```python
# get_multicast_group method usage example with argument unpacking

kwargs: GetMulticastGroupRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_multicast_group(**kwargs)
```

1. See [:material-code-braces: GetMulticastGroupRequestRequestTypeDef](./type_defs.md#getmulticastgrouprequestrequesttypedef) 

### get\_multicast\_group\_session

Gets information about a multicast group session.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_multicast_group_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_multicast_group_session.html)

```python
# get_multicast_group_session method definition

await def get_multicast_group_session(
    self,
    *,
    Id: str,
) -> GetMulticastGroupSessionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMulticastGroupSessionResponseTypeDef](./type_defs.md#getmulticastgroupsessionresponsetypedef) 


```python
# get_multicast_group_session method usage example with argument unpacking

kwargs: GetMulticastGroupSessionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_multicast_group_session(**kwargs)
```

1. See [:material-code-braces: GetMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#getmulticastgroupsessionrequestrequesttypedef) 

### get\_network\_analyzer\_configuration

Get network analyzer configuration.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_network_analyzer_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_network_analyzer_configuration.html)

```python
# get_network_analyzer_configuration method definition

await def get_network_analyzer_configuration(
    self,
    *,
    ConfigurationName: str,
) -> GetNetworkAnalyzerConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetNetworkAnalyzerConfigurationResponseTypeDef](./type_defs.md#getnetworkanalyzerconfigurationresponsetypedef) 


```python
# get_network_analyzer_configuration method usage example with argument unpacking

kwargs: GetNetworkAnalyzerConfigurationRequestRequestTypeDef = {  # (1)
    "ConfigurationName": ...,
}

parent.get_network_analyzer_configuration(**kwargs)
```

1. See [:material-code-braces: GetNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#getnetworkanalyzerconfigurationrequestrequesttypedef) 

### get\_partner\_account

Gets information about a partner account.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_partner_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_partner_account.html)

```python
# get_partner_account method definition

await def get_partner_account(
    self,
    *,
    PartnerAccountId: str,
    PartnerType: PartnerTypeType,  # (1)
) -> GetPartnerAccountResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PartnerTypeType](./literals.md#partnertypetype) 
2. See [:material-code-braces: GetPartnerAccountResponseTypeDef](./type_defs.md#getpartneraccountresponsetypedef) 


```python
# get_partner_account method usage example with argument unpacking

kwargs: GetPartnerAccountRequestRequestTypeDef = {  # (1)
    "PartnerAccountId": ...,
    "PartnerType": ...,
}

parent.get_partner_account(**kwargs)
```

1. See [:material-code-braces: GetPartnerAccountRequestRequestTypeDef](./type_defs.md#getpartneraccountrequestrequesttypedef) 

### get\_position

Get the position information for a given resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_position.html)

```python
# get_position method definition

await def get_position(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
) -> GetPositionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
2. See [:material-code-braces: GetPositionResponseTypeDef](./type_defs.md#getpositionresponsetypedef) 


```python
# get_position method usage example with argument unpacking

kwargs: GetPositionRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
}

parent.get_position(**kwargs)
```

1. See [:material-code-braces: GetPositionRequestRequestTypeDef](./type_defs.md#getpositionrequestrequesttypedef) 

### get\_position\_configuration

Get position configuration for a given resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_position_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_position_configuration.html)

```python
# get_position_configuration method definition

await def get_position_configuration(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
) -> GetPositionConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
2. See [:material-code-braces: GetPositionConfigurationResponseTypeDef](./type_defs.md#getpositionconfigurationresponsetypedef) 


```python
# get_position_configuration method usage example with argument unpacking

kwargs: GetPositionConfigurationRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
}

parent.get_position_configuration(**kwargs)
```

1. See [:material-code-braces: GetPositionConfigurationRequestRequestTypeDef](./type_defs.md#getpositionconfigurationrequestrequesttypedef) 

### get\_position\_estimate

Get estimated position information as a payload in GeoJSON format.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_position_estimate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_position_estimate.html)

```python
# get_position_estimate method definition

await def get_position_estimate(
    self,
    *,
    WiFiAccessPoints: Sequence[WiFiAccessPointTypeDef] = ...,  # (1)
    CellTowers: CellTowersTypeDef = ...,  # (2)
    Ip: IpTypeDef = ...,  # (3)
    Gnss: GnssTypeDef = ...,  # (4)
    Timestamp: TimestampTypeDef = ...,
) -> GetPositionEstimateResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: WiFiAccessPointTypeDef](./type_defs.md#wifiaccesspointtypedef) 
2. See [:material-code-braces: CellTowersTypeDef](./type_defs.md#celltowerstypedef) 
3. See [:material-code-braces: IpTypeDef](./type_defs.md#iptypedef) 
4. See [:material-code-braces: GnssTypeDef](./type_defs.md#gnsstypedef) 
5. See [:material-code-braces: GetPositionEstimateResponseTypeDef](./type_defs.md#getpositionestimateresponsetypedef) 


```python
# get_position_estimate method usage example with argument unpacking

kwargs: GetPositionEstimateRequestRequestTypeDef = {  # (1)
    "WiFiAccessPoints": ...,
}

parent.get_position_estimate(**kwargs)
```

1. See [:material-code-braces: GetPositionEstimateRequestRequestTypeDef](./type_defs.md#getpositionestimaterequestrequesttypedef) 

### get\_resource\_event\_configuration

Get the event configuration for a particular resource identifier.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_resource_event_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_resource_event_configuration.html)

```python
# get_resource_event_configuration method definition

await def get_resource_event_configuration(
    self,
    *,
    Identifier: str,
    IdentifierType: IdentifierTypeType,  # (1)
    PartnerType: EventNotificationPartnerTypeType = ...,  # (2)
) -> GetResourceEventConfigurationResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: IdentifierTypeType](./literals.md#identifiertypetype) 
2. See [:material-code-brackets: EventNotificationPartnerTypeType](./literals.md#eventnotificationpartnertypetype) 
3. See [:material-code-braces: GetResourceEventConfigurationResponseTypeDef](./type_defs.md#getresourceeventconfigurationresponsetypedef) 


```python
# get_resource_event_configuration method usage example with argument unpacking

kwargs: GetResourceEventConfigurationRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
    "IdentifierType": ...,
}

parent.get_resource_event_configuration(**kwargs)
```

1. See [:material-code-braces: GetResourceEventConfigurationRequestRequestTypeDef](./type_defs.md#getresourceeventconfigurationrequestrequesttypedef) 

### get\_resource\_log\_level

Fetches the log-level override, if any, for a given resource-ID and
resource-type.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_resource_log_level` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_resource_log_level.html)

```python
# get_resource_log_level method definition

await def get_resource_log_level(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: str,
) -> GetResourceLogLevelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourceLogLevelResponseTypeDef](./type_defs.md#getresourceloglevelresponsetypedef) 


```python
# get_resource_log_level method usage example with argument unpacking

kwargs: GetResourceLogLevelRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
}

parent.get_resource_log_level(**kwargs)
```

1. See [:material-code-braces: GetResourceLogLevelRequestRequestTypeDef](./type_defs.md#getresourceloglevelrequestrequesttypedef) 

### get\_resource\_position

Get the position information for a given wireless device or a wireless gateway
resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_resource_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_resource_position.html)

```python
# get_resource_position method definition

await def get_resource_position(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
) -> GetResourcePositionResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
2. See [:material-code-braces: GetResourcePositionResponseTypeDef](./type_defs.md#getresourcepositionresponsetypedef) 


```python
# get_resource_position method usage example with argument unpacking

kwargs: GetResourcePositionRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
}

parent.get_resource_position(**kwargs)
```

1. See [:material-code-braces: GetResourcePositionRequestRequestTypeDef](./type_defs.md#getresourcepositionrequestrequesttypedef) 

### get\_service\_endpoint

Gets the account-specific endpoint for Configuration and Update Server (CUPS)
protocol or LoRaWAN Network Server (LNS) connections.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_service_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_service_endpoint.html)

```python
# get_service_endpoint method definition

await def get_service_endpoint(
    self,
    *,
    ServiceType: WirelessGatewayServiceTypeType = ...,  # (1)
) -> GetServiceEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WirelessGatewayServiceTypeType](./literals.md#wirelessgatewayservicetypetype) 
2. See [:material-code-braces: GetServiceEndpointResponseTypeDef](./type_defs.md#getserviceendpointresponsetypedef) 


```python
# get_service_endpoint method usage example with argument unpacking

kwargs: GetServiceEndpointRequestRequestTypeDef = {  # (1)
    "ServiceType": ...,
}

parent.get_service_endpoint(**kwargs)
```

1. See [:material-code-braces: GetServiceEndpointRequestRequestTypeDef](./type_defs.md#getserviceendpointrequestrequesttypedef) 

### get\_service\_profile

Gets information about a service profile.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_service_profile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_service_profile.html)

```python
# get_service_profile method definition

await def get_service_profile(
    self,
    *,
    Id: str,
) -> GetServiceProfileResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceProfileResponseTypeDef](./type_defs.md#getserviceprofileresponsetypedef) 


```python
# get_service_profile method usage example with argument unpacking

kwargs: GetServiceProfileRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_service_profile(**kwargs)
```

1. See [:material-code-braces: GetServiceProfileRequestRequestTypeDef](./type_defs.md#getserviceprofilerequestrequesttypedef) 

### get\_wireless\_device

Gets information about a wireless device.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_device.html)

```python
# get_wireless_device method definition

await def get_wireless_device(
    self,
    *,
    Identifier: str,
    IdentifierType: WirelessDeviceIdTypeType,  # (1)
) -> GetWirelessDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WirelessDeviceIdTypeType](./literals.md#wirelessdeviceidtypetype) 
2. See [:material-code-braces: GetWirelessDeviceResponseTypeDef](./type_defs.md#getwirelessdeviceresponsetypedef) 


```python
# get_wireless_device method usage example with argument unpacking

kwargs: GetWirelessDeviceRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
    "IdentifierType": ...,
}

parent.get_wireless_device(**kwargs)
```

1. See [:material-code-braces: GetWirelessDeviceRequestRequestTypeDef](./type_defs.md#getwirelessdevicerequestrequesttypedef) 

### get\_wireless\_device\_import\_task

Get information about an import task and count of device onboarding summary
information for the import task.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_device_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_device_import_task.html)

```python
# get_wireless_device_import_task method definition

await def get_wireless_device_import_task(
    self,
    *,
    Id: str,
) -> GetWirelessDeviceImportTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWirelessDeviceImportTaskResponseTypeDef](./type_defs.md#getwirelessdeviceimporttaskresponsetypedef) 


```python
# get_wireless_device_import_task method usage example with argument unpacking

kwargs: GetWirelessDeviceImportTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_wireless_device_import_task(**kwargs)
```

1. See [:material-code-braces: GetWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#getwirelessdeviceimporttaskrequestrequesttypedef) 

### get\_wireless\_device\_statistics

Gets operating information about a wireless device.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_device_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_device_statistics.html)

```python
# get_wireless_device_statistics method definition

await def get_wireless_device_statistics(
    self,
    *,
    WirelessDeviceId: str,
) -> GetWirelessDeviceStatisticsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWirelessDeviceStatisticsResponseTypeDef](./type_defs.md#getwirelessdevicestatisticsresponsetypedef) 


```python
# get_wireless_device_statistics method usage example with argument unpacking

kwargs: GetWirelessDeviceStatisticsRequestRequestTypeDef = {  # (1)
    "WirelessDeviceId": ...,
}

parent.get_wireless_device_statistics(**kwargs)
```

1. See [:material-code-braces: GetWirelessDeviceStatisticsRequestRequestTypeDef](./type_defs.md#getwirelessdevicestatisticsrequestrequesttypedef) 

### get\_wireless\_gateway

Gets information about a wireless gateway.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_gateway.html)

```python
# get_wireless_gateway method definition

await def get_wireless_gateway(
    self,
    *,
    Identifier: str,
    IdentifierType: WirelessGatewayIdTypeType,  # (1)
) -> GetWirelessGatewayResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WirelessGatewayIdTypeType](./literals.md#wirelessgatewayidtypetype) 
2. See [:material-code-braces: GetWirelessGatewayResponseTypeDef](./type_defs.md#getwirelessgatewayresponsetypedef) 


```python
# get_wireless_gateway method usage example with argument unpacking

kwargs: GetWirelessGatewayRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
    "IdentifierType": ...,
}

parent.get_wireless_gateway(**kwargs)
```

1. See [:material-code-braces: GetWirelessGatewayRequestRequestTypeDef](./type_defs.md#getwirelessgatewayrequestrequesttypedef) 

### get\_wireless\_gateway\_certificate

Gets the ID of the certificate that is currently associated with a wireless
gateway.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_gateway_certificate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_gateway_certificate.html)

```python
# get_wireless_gateway_certificate method definition

await def get_wireless_gateway_certificate(
    self,
    *,
    Id: str,
) -> GetWirelessGatewayCertificateResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWirelessGatewayCertificateResponseTypeDef](./type_defs.md#getwirelessgatewaycertificateresponsetypedef) 


```python
# get_wireless_gateway_certificate method usage example with argument unpacking

kwargs: GetWirelessGatewayCertificateRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_wireless_gateway_certificate(**kwargs)
```

1. See [:material-code-braces: GetWirelessGatewayCertificateRequestRequestTypeDef](./type_defs.md#getwirelessgatewaycertificaterequestrequesttypedef) 

### get\_wireless\_gateway\_firmware\_information

Gets the firmware version and other information about a wireless gateway.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_gateway_firmware_information` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_gateway_firmware_information.html)

```python
# get_wireless_gateway_firmware_information method definition

await def get_wireless_gateway_firmware_information(
    self,
    *,
    Id: str,
) -> GetWirelessGatewayFirmwareInformationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWirelessGatewayFirmwareInformationResponseTypeDef](./type_defs.md#getwirelessgatewayfirmwareinformationresponsetypedef) 


```python
# get_wireless_gateway_firmware_information method usage example with argument unpacking

kwargs: GetWirelessGatewayFirmwareInformationRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_wireless_gateway_firmware_information(**kwargs)
```

1. See [:material-code-braces: GetWirelessGatewayFirmwareInformationRequestRequestTypeDef](./type_defs.md#getwirelessgatewayfirmwareinformationrequestrequesttypedef) 

### get\_wireless\_gateway\_statistics

Gets operating information about a wireless gateway.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_gateway_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_gateway_statistics.html)

```python
# get_wireless_gateway_statistics method definition

await def get_wireless_gateway_statistics(
    self,
    *,
    WirelessGatewayId: str,
) -> GetWirelessGatewayStatisticsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWirelessGatewayStatisticsResponseTypeDef](./type_defs.md#getwirelessgatewaystatisticsresponsetypedef) 


```python
# get_wireless_gateway_statistics method usage example with argument unpacking

kwargs: GetWirelessGatewayStatisticsRequestRequestTypeDef = {  # (1)
    "WirelessGatewayId": ...,
}

parent.get_wireless_gateway_statistics(**kwargs)
```

1. See [:material-code-braces: GetWirelessGatewayStatisticsRequestRequestTypeDef](./type_defs.md#getwirelessgatewaystatisticsrequestrequesttypedef) 

### get\_wireless\_gateway\_task

Gets information about a wireless gateway task.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_gateway_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_gateway_task.html)

```python
# get_wireless_gateway_task method definition

await def get_wireless_gateway_task(
    self,
    *,
    Id: str,
) -> GetWirelessGatewayTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWirelessGatewayTaskResponseTypeDef](./type_defs.md#getwirelessgatewaytaskresponsetypedef) 


```python
# get_wireless_gateway_task method usage example with argument unpacking

kwargs: GetWirelessGatewayTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_wireless_gateway_task(**kwargs)
```

1. See [:material-code-braces: GetWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#getwirelessgatewaytaskrequestrequesttypedef) 

### get\_wireless\_gateway\_task\_definition

Gets information about a wireless gateway task definition.

Type annotations and code completion for `#!python session.create_client("iotwireless").get_wireless_gateway_task_definition` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/get_wireless_gateway_task_definition.html)

```python
# get_wireless_gateway_task_definition method definition

await def get_wireless_gateway_task_definition(
    self,
    *,
    Id: str,
) -> GetWirelessGatewayTaskDefinitionResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetWirelessGatewayTaskDefinitionResponseTypeDef](./type_defs.md#getwirelessgatewaytaskdefinitionresponsetypedef) 


```python
# get_wireless_gateway_task_definition method usage example with argument unpacking

kwargs: GetWirelessGatewayTaskDefinitionRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.get_wireless_gateway_task_definition(**kwargs)
```

1. See [:material-code-braces: GetWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#getwirelessgatewaytaskdefinitionrequestrequesttypedef) 

### list\_destinations

Lists the destinations registered to your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_destinations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_destinations.html)

```python
# list_destinations method definition

await def list_destinations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDestinationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef) 


```python
# list_destinations method usage example with argument unpacking

kwargs: ListDestinationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_destinations(**kwargs)
```

1. See [:material-code-braces: ListDestinationsRequestRequestTypeDef](./type_defs.md#listdestinationsrequestrequesttypedef) 

### list\_device\_profiles

Lists the device profiles registered to your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_device_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_device_profiles.html)

```python
# list_device_profiles method definition

await def list_device_profiles(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
    DeviceProfileType: DeviceProfileTypeType = ...,  # (1)
) -> ListDeviceProfilesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: DeviceProfileTypeType](./literals.md#deviceprofiletypetype) 
2. See [:material-code-braces: ListDeviceProfilesResponseTypeDef](./type_defs.md#listdeviceprofilesresponsetypedef) 


```python
# list_device_profiles method usage example with argument unpacking

kwargs: ListDeviceProfilesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_device_profiles(**kwargs)
```

1. See [:material-code-braces: ListDeviceProfilesRequestRequestTypeDef](./type_defs.md#listdeviceprofilesrequestrequesttypedef) 

### list\_devices\_for\_wireless\_device\_import\_task

List the Sidewalk devices in an import task and their onboarding status.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_devices_for_wireless_device_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_devices_for_wireless_device_import_task.html)

```python
# list_devices_for_wireless_device_import_task method definition

await def list_devices_for_wireless_device_import_task(
    self,
    *,
    Id: str,
    MaxResults: int = ...,
    NextToken: str = ...,
    Status: OnboardStatusType = ...,  # (1)
) -> ListDevicesForWirelessDeviceImportTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OnboardStatusType](./literals.md#onboardstatustype) 
2. See [:material-code-braces: ListDevicesForWirelessDeviceImportTaskResponseTypeDef](./type_defs.md#listdevicesforwirelessdeviceimporttaskresponsetypedef) 


```python
# list_devices_for_wireless_device_import_task method usage example with argument unpacking

kwargs: ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.list_devices_for_wireless_device_import_task(**kwargs)
```

1. See [:material-code-braces: ListDevicesForWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#listdevicesforwirelessdeviceimporttaskrequestrequesttypedef) 

### list\_event\_configurations

List event configurations where at least one event topic has been enabled.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_event_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_event_configurations.html)

```python
# list_event_configurations method definition

await def list_event_configurations(
    self,
    *,
    ResourceType: EventNotificationResourceTypeType,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListEventConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: EventNotificationResourceTypeType](./literals.md#eventnotificationresourcetypetype) 
2. See [:material-code-braces: ListEventConfigurationsResponseTypeDef](./type_defs.md#listeventconfigurationsresponsetypedef) 


```python
# list_event_configurations method usage example with argument unpacking

kwargs: ListEventConfigurationsRequestRequestTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.list_event_configurations(**kwargs)
```

1. See [:material-code-braces: ListEventConfigurationsRequestRequestTypeDef](./type_defs.md#listeventconfigurationsrequestrequesttypedef) 

### list\_fuota\_tasks

Lists the FUOTA tasks registered to your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_fuota_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_fuota_tasks.html)

```python
# list_fuota_tasks method definition

await def list_fuota_tasks(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFuotaTasksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListFuotaTasksResponseTypeDef](./type_defs.md#listfuotatasksresponsetypedef) 


```python
# list_fuota_tasks method usage example with argument unpacking

kwargs: ListFuotaTasksRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_fuota_tasks(**kwargs)
```

1. See [:material-code-braces: ListFuotaTasksRequestRequestTypeDef](./type_defs.md#listfuotatasksrequestrequesttypedef) 

### list\_multicast\_groups

Lists the multicast groups registered to your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_multicast_groups` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_multicast_groups.html)

```python
# list_multicast_groups method definition

await def list_multicast_groups(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMulticastGroupsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMulticastGroupsResponseTypeDef](./type_defs.md#listmulticastgroupsresponsetypedef) 


```python
# list_multicast_groups method usage example with argument unpacking

kwargs: ListMulticastGroupsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_multicast_groups(**kwargs)
```

1. See [:material-code-braces: ListMulticastGroupsRequestRequestTypeDef](./type_defs.md#listmulticastgroupsrequestrequesttypedef) 

### list\_multicast\_groups\_by\_fuota\_task

List all multicast groups associated with a fuota task.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_multicast_groups_by_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_multicast_groups_by_fuota_task.html)

```python
# list_multicast_groups_by_fuota_task method definition

await def list_multicast_groups_by_fuota_task(
    self,
    *,
    Id: str,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListMulticastGroupsByFuotaTaskResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMulticastGroupsByFuotaTaskResponseTypeDef](./type_defs.md#listmulticastgroupsbyfuotataskresponsetypedef) 


```python
# list_multicast_groups_by_fuota_task method usage example with argument unpacking

kwargs: ListMulticastGroupsByFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.list_multicast_groups_by_fuota_task(**kwargs)
```

1. See [:material-code-braces: ListMulticastGroupsByFuotaTaskRequestRequestTypeDef](./type_defs.md#listmulticastgroupsbyfuotataskrequestrequesttypedef) 

### list\_network\_analyzer\_configurations

Lists the network analyzer configurations.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_network_analyzer_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_network_analyzer_configurations.html)

```python
# list_network_analyzer_configurations method definition

await def list_network_analyzer_configurations(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListNetworkAnalyzerConfigurationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListNetworkAnalyzerConfigurationsResponseTypeDef](./type_defs.md#listnetworkanalyzerconfigurationsresponsetypedef) 


```python
# list_network_analyzer_configurations method usage example with argument unpacking

kwargs: ListNetworkAnalyzerConfigurationsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_network_analyzer_configurations(**kwargs)
```

1. See [:material-code-braces: ListNetworkAnalyzerConfigurationsRequestRequestTypeDef](./type_defs.md#listnetworkanalyzerconfigurationsrequestrequesttypedef) 

### list\_partner\_accounts

Lists the partner accounts associated with your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_partner_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_partner_accounts.html)

```python
# list_partner_accounts method definition

await def list_partner_accounts(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPartnerAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListPartnerAccountsResponseTypeDef](./type_defs.md#listpartneraccountsresponsetypedef) 


```python
# list_partner_accounts method usage example with argument unpacking

kwargs: ListPartnerAccountsRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_partner_accounts(**kwargs)
```

1. See [:material-code-braces: ListPartnerAccountsRequestRequestTypeDef](./type_defs.md#listpartneraccountsrequestrequesttypedef) 

### list\_position\_configurations

List position configurations for a given resource, such as positioning solvers.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_position_configurations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_position_configurations.html)

```python
# list_position_configurations method definition

await def list_position_configurations(
    self,
    *,
    ResourceType: PositionResourceTypeType = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListPositionConfigurationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
2. See [:material-code-braces: ListPositionConfigurationsResponseTypeDef](./type_defs.md#listpositionconfigurationsresponsetypedef) 


```python
# list_position_configurations method usage example with argument unpacking

kwargs: ListPositionConfigurationsRequestRequestTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.list_position_configurations(**kwargs)
```

1. See [:material-code-braces: ListPositionConfigurationsRequestRequestTypeDef](./type_defs.md#listpositionconfigurationsrequestrequesttypedef) 

### list\_queued\_messages

List queued messages in the downlink queue.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_queued_messages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_queued_messages.html)

```python
# list_queued_messages method definition

await def list_queued_messages(
    self,
    *,
    Id: str,
    NextToken: str = ...,
    MaxResults: int = ...,
    WirelessDeviceType: WirelessDeviceTypeType = ...,  # (1)
) -> ListQueuedMessagesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
2. See [:material-code-braces: ListQueuedMessagesResponseTypeDef](./type_defs.md#listqueuedmessagesresponsetypedef) 


```python
# list_queued_messages method usage example with argument unpacking

kwargs: ListQueuedMessagesRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.list_queued_messages(**kwargs)
```

1. See [:material-code-braces: ListQueuedMessagesRequestRequestTypeDef](./type_defs.md#listqueuedmessagesrequestrequesttypedef) 

### list\_service\_profiles

Lists the service profiles registered to your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_service_profiles` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_service_profiles.html)

```python
# list_service_profiles method definition

await def list_service_profiles(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListServiceProfilesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListServiceProfilesResponseTypeDef](./type_defs.md#listserviceprofilesresponsetypedef) 


```python
# list_service_profiles method usage example with argument unpacking

kwargs: ListServiceProfilesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_service_profiles(**kwargs)
```

1. See [:material-code-braces: ListServiceProfilesRequestRequestTypeDef](./type_defs.md#listserviceprofilesrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags (metadata) you have assigned to the resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_tags_for_resource.html)

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

### list\_wireless\_device\_import\_tasks

List wireless devices that have been added to an import task.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_wireless_device_import_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_wireless_device_import_tasks.html)

```python
# list_wireless_device_import_tasks method definition

await def list_wireless_device_import_tasks(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListWirelessDeviceImportTasksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWirelessDeviceImportTasksResponseTypeDef](./type_defs.md#listwirelessdeviceimporttasksresponsetypedef) 


```python
# list_wireless_device_import_tasks method usage example with argument unpacking

kwargs: ListWirelessDeviceImportTasksRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_wireless_device_import_tasks(**kwargs)
```

1. See [:material-code-braces: ListWirelessDeviceImportTasksRequestRequestTypeDef](./type_defs.md#listwirelessdeviceimporttasksrequestrequesttypedef) 

### list\_wireless\_devices

Lists the wireless devices registered to your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_wireless_devices` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_wireless_devices.html)

```python
# list_wireless_devices method definition

await def list_wireless_devices(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    DestinationName: str = ...,
    DeviceProfileId: str = ...,
    ServiceProfileId: str = ...,
    WirelessDeviceType: WirelessDeviceTypeType = ...,  # (1)
    FuotaTaskId: str = ...,
    MulticastGroupId: str = ...,
) -> ListWirelessDevicesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype) 
2. See [:material-code-braces: ListWirelessDevicesResponseTypeDef](./type_defs.md#listwirelessdevicesresponsetypedef) 


```python
# list_wireless_devices method usage example with argument unpacking

kwargs: ListWirelessDevicesRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_wireless_devices(**kwargs)
```

1. See [:material-code-braces: ListWirelessDevicesRequestRequestTypeDef](./type_defs.md#listwirelessdevicesrequestrequesttypedef) 

### list\_wireless\_gateway\_task\_definitions

List the wireless gateway tasks definitions registered to your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_wireless_gateway_task_definitions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_wireless_gateway_task_definitions.html)

```python
# list_wireless_gateway_task_definitions method definition

await def list_wireless_gateway_task_definitions(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    TaskDefinitionType: WirelessGatewayTaskDefinitionTypeType = ...,  # (1)
) -> ListWirelessGatewayTaskDefinitionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: WirelessGatewayTaskDefinitionTypeType](./literals.md#wirelessgatewaytaskdefinitiontypetype) 
2. See [:material-code-braces: ListWirelessGatewayTaskDefinitionsResponseTypeDef](./type_defs.md#listwirelessgatewaytaskdefinitionsresponsetypedef) 


```python
# list_wireless_gateway_task_definitions method usage example with argument unpacking

kwargs: ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_wireless_gateway_task_definitions(**kwargs)
```

1. See [:material-code-braces: ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef](./type_defs.md#listwirelessgatewaytaskdefinitionsrequestrequesttypedef) 

### list\_wireless\_gateways

Lists the wireless gateways registered to your AWS account.

Type annotations and code completion for `#!python session.create_client("iotwireless").list_wireless_gateways` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/list_wireless_gateways.html)

```python
# list_wireless_gateways method definition

await def list_wireless_gateways(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListWirelessGatewaysResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListWirelessGatewaysResponseTypeDef](./type_defs.md#listwirelessgatewaysresponsetypedef) 


```python
# list_wireless_gateways method usage example with argument unpacking

kwargs: ListWirelessGatewaysRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_wireless_gateways(**kwargs)
```

1. See [:material-code-braces: ListWirelessGatewaysRequestRequestTypeDef](./type_defs.md#listwirelessgatewaysrequestrequesttypedef) 

### put\_position\_configuration

Put position configuration for a given resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").put_position_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/put_position_configuration.html)

```python
# put_position_configuration method definition

await def put_position_configuration(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
    Solvers: PositionSolverConfigurationsTypeDef = ...,  # (2)
    Destination: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 
2. See [:material-code-braces: PositionSolverConfigurationsTypeDef](./type_defs.md#positionsolverconfigurationstypedef) 


```python
# put_position_configuration method usage example with argument unpacking

kwargs: PutPositionConfigurationRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
}

parent.put_position_configuration(**kwargs)
```

1. See [:material-code-braces: PutPositionConfigurationRequestRequestTypeDef](./type_defs.md#putpositionconfigurationrequestrequesttypedef) 

### put\_resource\_log\_level

Sets the log-level override for a resource-ID and resource-type.

Type annotations and code completion for `#!python session.create_client("iotwireless").put_resource_log_level` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/put_resource_log_level.html)

```python
# put_resource_log_level method definition

await def put_resource_log_level(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: str,
    LogLevel: LogLevelType,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 


```python
# put_resource_log_level method usage example with argument unpacking

kwargs: PutResourceLogLevelRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
    "LogLevel": ...,
}

parent.put_resource_log_level(**kwargs)
```

1. See [:material-code-braces: PutResourceLogLevelRequestRequestTypeDef](./type_defs.md#putresourceloglevelrequestrequesttypedef) 

### reset\_all\_resource\_log\_levels

Removes the log-level overrides for all resources; wireless devices, wireless
gateways, and fuota tasks.

Type annotations and code completion for `#!python session.create_client("iotwireless").reset_all_resource_log_levels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/reset_all_resource_log_levels.html)

```python
# reset_all_resource_log_levels method definition

await def reset_all_resource_log_levels(
    self,
) -> Dict[str, Any]:
    ...
```


### reset\_resource\_log\_level

Removes the log-level override, if any, for a specific resource-ID and
resource-type.

Type annotations and code completion for `#!python session.create_client("iotwireless").reset_resource_log_level` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/reset_resource_log_level.html)

```python
# reset_resource_log_level method definition

await def reset_resource_log_level(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: str,
) -> Dict[str, Any]:
    ...
```



```python
# reset_resource_log_level method usage example with argument unpacking

kwargs: ResetResourceLogLevelRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
}

parent.reset_resource_log_level(**kwargs)
```

1. See [:material-code-braces: ResetResourceLogLevelRequestRequestTypeDef](./type_defs.md#resetresourceloglevelrequestrequesttypedef) 

### send\_data\_to\_multicast\_group

Sends the specified data to a multicast group.

Type annotations and code completion for `#!python session.create_client("iotwireless").send_data_to_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/send_data_to_multicast_group.html)

```python
# send_data_to_multicast_group method definition

await def send_data_to_multicast_group(
    self,
    *,
    Id: str,
    PayloadData: str,
    WirelessMetadata: MulticastWirelessMetadataTypeDef,  # (1)
) -> SendDataToMulticastGroupResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MulticastWirelessMetadataTypeDef](./type_defs.md#multicastwirelessmetadatatypedef) 
2. See [:material-code-braces: SendDataToMulticastGroupResponseTypeDef](./type_defs.md#senddatatomulticastgroupresponsetypedef) 


```python
# send_data_to_multicast_group method usage example with argument unpacking

kwargs: SendDataToMulticastGroupRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "PayloadData": ...,
    "WirelessMetadata": ...,
}

parent.send_data_to_multicast_group(**kwargs)
```

1. See [:material-code-braces: SendDataToMulticastGroupRequestRequestTypeDef](./type_defs.md#senddatatomulticastgrouprequestrequesttypedef) 

### send\_data\_to\_wireless\_device

Sends a decrypted application data frame to a device.

Type annotations and code completion for `#!python session.create_client("iotwireless").send_data_to_wireless_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/send_data_to_wireless_device.html)

```python
# send_data_to_wireless_device method definition

await def send_data_to_wireless_device(
    self,
    *,
    Id: str,
    TransmitMode: int,
    PayloadData: str,
    WirelessMetadata: WirelessMetadataTypeDef = ...,  # (1)
) -> SendDataToWirelessDeviceResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: WirelessMetadataTypeDef](./type_defs.md#wirelessmetadatatypedef) 
2. See [:material-code-braces: SendDataToWirelessDeviceResponseTypeDef](./type_defs.md#senddatatowirelessdeviceresponsetypedef) 


```python
# send_data_to_wireless_device method usage example with argument unpacking

kwargs: SendDataToWirelessDeviceRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "TransmitMode": ...,
    "PayloadData": ...,
}

parent.send_data_to_wireless_device(**kwargs)
```

1. See [:material-code-braces: SendDataToWirelessDeviceRequestRequestTypeDef](./type_defs.md#senddatatowirelessdevicerequestrequesttypedef) 

### start\_bulk\_associate\_wireless\_device\_with\_multicast\_group

Starts a bulk association of all qualifying wireless devices with a multicast
group.

Type annotations and code completion for `#!python session.create_client("iotwireless").start_bulk_associate_wireless_device_with_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/start_bulk_associate_wireless_device_with_multicast_group.html)

```python
# start_bulk_associate_wireless_device_with_multicast_group method definition

await def start_bulk_associate_wireless_device_with_multicast_group(
    self,
    *,
    Id: str,
    QueryString: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# start_bulk_associate_wireless_device_with_multicast_group method usage example with argument unpacking

kwargs: StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.start_bulk_associate_wireless_device_with_multicast_group(**kwargs)
```

1. See [:material-code-braces: StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef](./type_defs.md#startbulkassociatewirelessdevicewithmulticastgrouprequestrequesttypedef) 

### start\_bulk\_disassociate\_wireless\_device\_from\_multicast\_group

Starts a bulk disassociatin of all qualifying wireless devices from a multicast
group.

Type annotations and code completion for `#!python session.create_client("iotwireless").start_bulk_disassociate_wireless_device_from_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/start_bulk_disassociate_wireless_device_from_multicast_group.html)

```python
# start_bulk_disassociate_wireless_device_from_multicast_group method definition

await def start_bulk_disassociate_wireless_device_from_multicast_group(
    self,
    *,
    Id: str,
    QueryString: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# start_bulk_disassociate_wireless_device_from_multicast_group method usage example with argument unpacking

kwargs: StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.start_bulk_disassociate_wireless_device_from_multicast_group(**kwargs)
```

1. See [:material-code-braces: StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef](./type_defs.md#startbulkdisassociatewirelessdevicefrommulticastgrouprequestrequesttypedef) 

### start\_fuota\_task

Starts a FUOTA task.

Type annotations and code completion for `#!python session.create_client("iotwireless").start_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/start_fuota_task.html)

```python
# start_fuota_task method definition

await def start_fuota_task(
    self,
    *,
    Id: str,
    LoRaWAN: LoRaWANStartFuotaTaskTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LoRaWANStartFuotaTaskTypeDef](./type_defs.md#lorawanstartfuotatasktypedef) 


```python
# start_fuota_task method usage example with argument unpacking

kwargs: StartFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.start_fuota_task(**kwargs)
```

1. See [:material-code-braces: StartFuotaTaskRequestRequestTypeDef](./type_defs.md#startfuotataskrequestrequesttypedef) 

### start\_multicast\_group\_session

Starts a multicast group session.

Type annotations and code completion for `#!python session.create_client("iotwireless").start_multicast_group_session` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/start_multicast_group_session.html)

```python
# start_multicast_group_session method definition

await def start_multicast_group_session(
    self,
    *,
    Id: str,
    LoRaWAN: LoRaWANMulticastSessionTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LoRaWANMulticastSessionTypeDef](./type_defs.md#lorawanmulticastsessiontypedef) 


```python
# start_multicast_group_session method usage example with argument unpacking

kwargs: StartMulticastGroupSessionRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "LoRaWAN": ...,
}

parent.start_multicast_group_session(**kwargs)
```

1. See [:material-code-braces: StartMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#startmulticastgroupsessionrequestrequesttypedef) 

### start\_single\_wireless\_device\_import\_task

Start import task for a single wireless device.

Type annotations and code completion for `#!python session.create_client("iotwireless").start_single_wireless_device_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/start_single_wireless_device_import_task.html)

```python
# start_single_wireless_device_import_task method definition

await def start_single_wireless_device_import_task(
    self,
    *,
    DestinationName: str,
    Sidewalk: SidewalkSingleStartImportInfoTypeDef,  # (1)
    ClientRequestToken: str = ...,
    DeviceName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> StartSingleWirelessDeviceImportTaskResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SidewalkSingleStartImportInfoTypeDef](./type_defs.md#sidewalksinglestartimportinfotypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: StartSingleWirelessDeviceImportTaskResponseTypeDef](./type_defs.md#startsinglewirelessdeviceimporttaskresponsetypedef) 


```python
# start_single_wireless_device_import_task method usage example with argument unpacking

kwargs: StartSingleWirelessDeviceImportTaskRequestRequestTypeDef = {  # (1)
    "DestinationName": ...,
    "Sidewalk": ...,
}

parent.start_single_wireless_device_import_task(**kwargs)
```

1. See [:material-code-braces: StartSingleWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#startsinglewirelessdeviceimporttaskrequestrequesttypedef) 

### start\_wireless\_device\_import\_task

Start import task for provisioning Sidewalk devices in bulk using an S3 CSV
file.

Type annotations and code completion for `#!python session.create_client("iotwireless").start_wireless_device_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/start_wireless_device_import_task.html)

```python
# start_wireless_device_import_task method definition

await def start_wireless_device_import_task(
    self,
    *,
    DestinationName: str,
    Sidewalk: SidewalkStartImportInfoTypeDef,  # (1)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> StartWirelessDeviceImportTaskResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SidewalkStartImportInfoTypeDef](./type_defs.md#sidewalkstartimportinfotypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: StartWirelessDeviceImportTaskResponseTypeDef](./type_defs.md#startwirelessdeviceimporttaskresponsetypedef) 


```python
# start_wireless_device_import_task method usage example with argument unpacking

kwargs: StartWirelessDeviceImportTaskRequestRequestTypeDef = {  # (1)
    "DestinationName": ...,
    "Sidewalk": ...,
}

parent.start_wireless_device_import_task(**kwargs)
```

1. See [:material-code-braces: StartWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#startwirelessdeviceimporttaskrequestrequesttypedef) 

### tag\_resource

Adds a tag to a resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### test\_wireless\_device

Simulates a provisioned device by sending an uplink data payload of
<code>Hello</code>.

Type annotations and code completion for `#!python session.create_client("iotwireless").test_wireless_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/test_wireless_device.html)

```python
# test_wireless_device method definition

await def test_wireless_device(
    self,
    *,
    Id: str,
) -> TestWirelessDeviceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: TestWirelessDeviceResponseTypeDef](./type_defs.md#testwirelessdeviceresponsetypedef) 


```python
# test_wireless_device method usage example with argument unpacking

kwargs: TestWirelessDeviceRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.test_wireless_device(**kwargs)
```

1. See [:material-code-braces: TestWirelessDeviceRequestRequestTypeDef](./type_defs.md#testwirelessdevicerequestrequesttypedef) 

### untag\_resource

Removes one or more tags from a resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_destination

Updates properties of a destination.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_destination` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_destination.html)

```python
# update_destination method definition

await def update_destination(
    self,
    *,
    Name: str,
    ExpressionType: ExpressionTypeType = ...,  # (1)
    Expression: str = ...,
    Description: str = ...,
    RoleArn: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ExpressionTypeType](./literals.md#expressiontypetype) 


```python
# update_destination method usage example with argument unpacking

kwargs: UpdateDestinationRequestRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.update_destination(**kwargs)
```

1. See [:material-code-braces: UpdateDestinationRequestRequestTypeDef](./type_defs.md#updatedestinationrequestrequesttypedef) 

### update\_event\_configuration\_by\_resource\_types

Update the event configuration based on resource types.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_event_configuration_by_resource_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_event_configuration_by_resource_types.html)

```python
# update_event_configuration_by_resource_types method definition

await def update_event_configuration_by_resource_types(
    self,
    *,
    DeviceRegistrationState: DeviceRegistrationStateResourceTypeEventConfigurationTypeDef = ...,  # (1)
    Proximity: ProximityResourceTypeEventConfigurationTypeDef = ...,  # (2)
    Join: JoinResourceTypeEventConfigurationTypeDef = ...,  # (3)
    ConnectionStatus: ConnectionStatusResourceTypeEventConfigurationTypeDef = ...,  # (4)
    MessageDeliveryStatus: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef = ...,  # (5)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: DeviceRegistrationStateResourceTypeEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateresourcetypeeventconfigurationtypedef) 
2. See [:material-code-braces: ProximityResourceTypeEventConfigurationTypeDef](./type_defs.md#proximityresourcetypeeventconfigurationtypedef) 
3. See [:material-code-braces: JoinResourceTypeEventConfigurationTypeDef](./type_defs.md#joinresourcetypeeventconfigurationtypedef) 
4. See [:material-code-braces: ConnectionStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#connectionstatusresourcetypeeventconfigurationtypedef) 
5. See [:material-code-braces: MessageDeliveryStatusResourceTypeEventConfigurationTypeDef](./type_defs.md#messagedeliverystatusresourcetypeeventconfigurationtypedef) 


```python
# update_event_configuration_by_resource_types method usage example with argument unpacking

kwargs: UpdateEventConfigurationByResourceTypesRequestRequestTypeDef = {  # (1)
    "DeviceRegistrationState": ...,
}

parent.update_event_configuration_by_resource_types(**kwargs)
```

1. See [:material-code-braces: UpdateEventConfigurationByResourceTypesRequestRequestTypeDef](./type_defs.md#updateeventconfigurationbyresourcetypesrequestrequesttypedef) 

### update\_fuota\_task

Updates properties of a FUOTA task.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_fuota_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_fuota_task.html)

```python
# update_fuota_task method definition

await def update_fuota_task(
    self,
    *,
    Id: str,
    Name: str = ...,
    Description: str = ...,
    LoRaWAN: LoRaWANFuotaTaskTypeDef = ...,  # (1)
    FirmwareUpdateImage: str = ...,
    FirmwareUpdateRole: str = ...,
    RedundancyPercent: int = ...,
    FragmentSizeBytes: int = ...,
    FragmentIntervalMS: int = ...,
    Descriptor: str = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LoRaWANFuotaTaskTypeDef](./type_defs.md#lorawanfuotatasktypedef) 


```python
# update_fuota_task method usage example with argument unpacking

kwargs: UpdateFuotaTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_fuota_task(**kwargs)
```

1. See [:material-code-braces: UpdateFuotaTaskRequestRequestTypeDef](./type_defs.md#updatefuotataskrequestrequesttypedef) 

### update\_log\_levels\_by\_resource\_types

Set default log level, or log levels by resource types.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_log_levels_by_resource_types` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_log_levels_by_resource_types.html)

```python
# update_log_levels_by_resource_types method definition

await def update_log_levels_by_resource_types(
    self,
    *,
    DefaultLogLevel: LogLevelType = ...,  # (1)
    FuotaTaskLogOptions: Sequence[FuotaTaskLogOptionUnionTypeDef] = ...,  # (2)
    WirelessDeviceLogOptions: Sequence[WirelessDeviceLogOptionUnionTypeDef] = ...,  # (3)
    WirelessGatewayLogOptions: Sequence[WirelessGatewayLogOptionUnionTypeDef] = ...,  # (4)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype) 
2. See [:material-code-braces: FuotaTaskLogOptionTypeDef](./type_defs.md#fuotatasklogoptiontypedef) [:material-code-braces: FuotaTaskLogOptionOutputTypeDef](./type_defs.md#fuotatasklogoptionoutputtypedef) 
3. See [:material-code-braces: WirelessDeviceLogOptionTypeDef](./type_defs.md#wirelessdevicelogoptiontypedef) [:material-code-braces: WirelessDeviceLogOptionOutputTypeDef](./type_defs.md#wirelessdevicelogoptionoutputtypedef) 
4. See [:material-code-braces: WirelessGatewayLogOptionTypeDef](./type_defs.md#wirelessgatewaylogoptiontypedef) [:material-code-braces: WirelessGatewayLogOptionOutputTypeDef](./type_defs.md#wirelessgatewaylogoptionoutputtypedef) 


```python
# update_log_levels_by_resource_types method usage example with argument unpacking

kwargs: UpdateLogLevelsByResourceTypesRequestRequestTypeDef = {  # (1)
    "DefaultLogLevel": ...,
}

parent.update_log_levels_by_resource_types(**kwargs)
```

1. See [:material-code-braces: UpdateLogLevelsByResourceTypesRequestRequestTypeDef](./type_defs.md#updateloglevelsbyresourcetypesrequestrequesttypedef) 

### update\_metric\_configuration

Update the summary metric configuration.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_metric_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_metric_configuration.html)

```python
# update_metric_configuration method definition

await def update_metric_configuration(
    self,
    *,
    SummaryMetric: SummaryMetricConfigurationTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SummaryMetricConfigurationTypeDef](./type_defs.md#summarymetricconfigurationtypedef) 


```python
# update_metric_configuration method usage example with argument unpacking

kwargs: UpdateMetricConfigurationRequestRequestTypeDef = {  # (1)
    "SummaryMetric": ...,
}

parent.update_metric_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateMetricConfigurationRequestRequestTypeDef](./type_defs.md#updatemetricconfigurationrequestrequesttypedef) 

### update\_multicast\_group

Updates properties of a multicast group session.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_multicast_group` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_multicast_group.html)

```python
# update_multicast_group method definition

await def update_multicast_group(
    self,
    *,
    Id: str,
    Name: str = ...,
    Description: str = ...,
    LoRaWAN: LoRaWANMulticastTypeDef = ...,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LoRaWANMulticastTypeDef](./type_defs.md#lorawanmulticasttypedef) 


```python
# update_multicast_group method usage example with argument unpacking

kwargs: UpdateMulticastGroupRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_multicast_group(**kwargs)
```

1. See [:material-code-braces: UpdateMulticastGroupRequestRequestTypeDef](./type_defs.md#updatemulticastgrouprequestrequesttypedef) 

### update\_network\_analyzer\_configuration

Update network analyzer configuration.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_network_analyzer_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_network_analyzer_configuration.html)

```python
# update_network_analyzer_configuration method definition

await def update_network_analyzer_configuration(
    self,
    *,
    ConfigurationName: str,
    TraceContent: TraceContentTypeDef = ...,  # (1)
    WirelessDevicesToAdd: Sequence[str] = ...,
    WirelessDevicesToRemove: Sequence[str] = ...,
    WirelessGatewaysToAdd: Sequence[str] = ...,
    WirelessGatewaysToRemove: Sequence[str] = ...,
    Description: str = ...,
    MulticastGroupsToAdd: Sequence[str] = ...,
    MulticastGroupsToRemove: Sequence[str] = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TraceContentTypeDef](./type_defs.md#tracecontenttypedef) 


```python
# update_network_analyzer_configuration method usage example with argument unpacking

kwargs: UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef = {  # (1)
    "ConfigurationName": ...,
}

parent.update_network_analyzer_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#updatenetworkanalyzerconfigurationrequestrequesttypedef) 

### update\_partner\_account

Updates properties of a partner account.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_partner_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_partner_account.html)

```python
# update_partner_account method definition

await def update_partner_account(
    self,
    *,
    Sidewalk: SidewalkUpdateAccountTypeDef,  # (1)
    PartnerAccountId: str,
    PartnerType: PartnerTypeType,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SidewalkUpdateAccountTypeDef](./type_defs.md#sidewalkupdateaccounttypedef) 
2. See [:material-code-brackets: PartnerTypeType](./literals.md#partnertypetype) 


```python
# update_partner_account method usage example with argument unpacking

kwargs: UpdatePartnerAccountRequestRequestTypeDef = {  # (1)
    "Sidewalk": ...,
    "PartnerAccountId": ...,
    "PartnerType": ...,
}

parent.update_partner_account(**kwargs)
```

1. See [:material-code-braces: UpdatePartnerAccountRequestRequestTypeDef](./type_defs.md#updatepartneraccountrequestrequesttypedef) 

### update\_position

Update the position information of a resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_position.html)

```python
# update_position method definition

await def update_position(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
    Position: Sequence[float],
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 


```python
# update_position method usage example with argument unpacking

kwargs: UpdatePositionRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
    "Position": ...,
}

parent.update_position(**kwargs)
```

1. See [:material-code-braces: UpdatePositionRequestRequestTypeDef](./type_defs.md#updatepositionrequestrequesttypedef) 

### update\_resource\_event\_configuration

Update the event configuration for a particular resource identifier.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_resource_event_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_resource_event_configuration.html)

```python
# update_resource_event_configuration method definition

await def update_resource_event_configuration(
    self,
    *,
    Identifier: str,
    IdentifierType: IdentifierTypeType,  # (1)
    PartnerType: EventNotificationPartnerTypeType = ...,  # (2)
    DeviceRegistrationState: DeviceRegistrationStateEventConfigurationTypeDef = ...,  # (3)
    Proximity: ProximityEventConfigurationTypeDef = ...,  # (4)
    Join: JoinEventConfigurationTypeDef = ...,  # (5)
    ConnectionStatus: ConnectionStatusEventConfigurationTypeDef = ...,  # (6)
    MessageDeliveryStatus: MessageDeliveryStatusEventConfigurationTypeDef = ...,  # (7)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: IdentifierTypeType](./literals.md#identifiertypetype) 
2. See [:material-code-brackets: EventNotificationPartnerTypeType](./literals.md#eventnotificationpartnertypetype) 
3. See [:material-code-braces: DeviceRegistrationStateEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateeventconfigurationtypedef) 
4. See [:material-code-braces: ProximityEventConfigurationTypeDef](./type_defs.md#proximityeventconfigurationtypedef) 
5. See [:material-code-braces: JoinEventConfigurationTypeDef](./type_defs.md#joineventconfigurationtypedef) 
6. See [:material-code-braces: ConnectionStatusEventConfigurationTypeDef](./type_defs.md#connectionstatuseventconfigurationtypedef) 
7. See [:material-code-braces: MessageDeliveryStatusEventConfigurationTypeDef](./type_defs.md#messagedeliverystatuseventconfigurationtypedef) 


```python
# update_resource_event_configuration method usage example with argument unpacking

kwargs: UpdateResourceEventConfigurationRequestRequestTypeDef = {  # (1)
    "Identifier": ...,
    "IdentifierType": ...,
}

parent.update_resource_event_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateResourceEventConfigurationRequestRequestTypeDef](./type_defs.md#updateresourceeventconfigurationrequestrequesttypedef) 

### update\_resource\_position

Update the position information of a given wireless device or a wireless
gateway resource.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_resource_position` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_resource_position.html)

```python
# update_resource_position method definition

await def update_resource_position(
    self,
    *,
    ResourceIdentifier: str,
    ResourceType: PositionResourceTypeType,  # (1)
    GeoJsonPayload: BlobTypeDef = ...,
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: PositionResourceTypeType](./literals.md#positionresourcetypetype) 


```python
# update_resource_position method usage example with argument unpacking

kwargs: UpdateResourcePositionRequestRequestTypeDef = {  # (1)
    "ResourceIdentifier": ...,
    "ResourceType": ...,
}

parent.update_resource_position(**kwargs)
```

1. See [:material-code-braces: UpdateResourcePositionRequestRequestTypeDef](./type_defs.md#updateresourcepositionrequestrequesttypedef) 

### update\_wireless\_device

Updates properties of a wireless device.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_wireless_device` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_wireless_device.html)

```python
# update_wireless_device method definition

await def update_wireless_device(
    self,
    *,
    Id: str,
    DestinationName: str = ...,
    Name: str = ...,
    Description: str = ...,
    LoRaWAN: LoRaWANUpdateDeviceTypeDef = ...,  # (1)
    Positioning: PositioningConfigStatusType = ...,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: LoRaWANUpdateDeviceTypeDef](./type_defs.md#lorawanupdatedevicetypedef) 
2. See [:material-code-brackets: PositioningConfigStatusType](./literals.md#positioningconfigstatustype) 


```python
# update_wireless_device method usage example with argument unpacking

kwargs: UpdateWirelessDeviceRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_wireless_device(**kwargs)
```

1. See [:material-code-braces: UpdateWirelessDeviceRequestRequestTypeDef](./type_defs.md#updatewirelessdevicerequestrequesttypedef) 

### update\_wireless\_device\_import\_task

Update an import task to add more devices to the task.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_wireless_device_import_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_wireless_device_import_task.html)

```python
# update_wireless_device_import_task method definition

await def update_wireless_device_import_task(
    self,
    *,
    Id: str,
    Sidewalk: SidewalkUpdateImportInfoTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: SidewalkUpdateImportInfoTypeDef](./type_defs.md#sidewalkupdateimportinfotypedef) 


```python
# update_wireless_device_import_task method usage example with argument unpacking

kwargs: UpdateWirelessDeviceImportTaskRequestRequestTypeDef = {  # (1)
    "Id": ...,
    "Sidewalk": ...,
}

parent.update_wireless_device_import_task(**kwargs)
```

1. See [:material-code-braces: UpdateWirelessDeviceImportTaskRequestRequestTypeDef](./type_defs.md#updatewirelessdeviceimporttaskrequestrequesttypedef) 

### update\_wireless\_gateway

Updates properties of a wireless gateway.

Type annotations and code completion for `#!python session.create_client("iotwireless").update_wireless_gateway` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless/client/update_wireless_gateway.html)

```python
# update_wireless_gateway method definition

await def update_wireless_gateway(
    self,
    *,
    Id: str,
    Name: str = ...,
    Description: str = ...,
    JoinEuiFilters: Sequence[Sequence[str]] = ...,
    NetIdFilters: Sequence[str] = ...,
    MaxEirp: float = ...,
) -> Dict[str, Any]:
    ...
```



```python
# update_wireless_gateway method usage example with argument unpacking

kwargs: UpdateWirelessGatewayRequestRequestTypeDef = {  # (1)
    "Id": ...,
}

parent.update_wireless_gateway(**kwargs)
```

1. See [:material-code-braces: UpdateWirelessGatewayRequestRequestTypeDef](./type_defs.md#updatewirelessgatewayrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("iotwireless").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("iotwireless").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client)

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






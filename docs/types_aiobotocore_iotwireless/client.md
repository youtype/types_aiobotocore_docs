<a id="iotwirelessclient-for-aiobotocore-iotwireless-module"></a>

# IoTWirelessClient for aiobotocore IoTWireless module

> [Index](../README.md) > [IoTWireless](./README.md) > IoTWirelessClient

Auto-generated documentation for
[IoTWireless](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless)
type annotations stubs module
[types-aiobotocore-iotwireless](https://pypi.org/project/types-aiobotocore-iotwireless/).

- [IoTWirelessClient for aiobotocore IoTWireless module](#iotwirelessclient-for-aiobotocore-iotwireless-module)
  - [IoTWirelessClient](#iotwirelessclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_aws_account_with_partner_account](#associate_aws_account_with_partner_account)
    - [associate_multicast_group_with_fuota_task](#associate_multicast_group_with_fuota_task)
    - [associate_wireless_device_with_fuota_task](#associate_wireless_device_with_fuota_task)
    - [associate_wireless_device_with_multicast_group](#associate_wireless_device_with_multicast_group)
    - [associate_wireless_device_with_thing](#associate_wireless_device_with_thing)
    - [associate_wireless_gateway_with_certificate](#associate_wireless_gateway_with_certificate)
    - [associate_wireless_gateway_with_thing](#associate_wireless_gateway_with_thing)
    - [can_paginate](#can_paginate)
    - [cancel_multicast_group_session](#cancel_multicast_group_session)
    - [create_destination](#create_destination)
    - [create_device_profile](#create_device_profile)
    - [create_fuota_task](#create_fuota_task)
    - [create_multicast_group](#create_multicast_group)
    - [create_service_profile](#create_service_profile)
    - [create_wireless_device](#create_wireless_device)
    - [create_wireless_gateway](#create_wireless_gateway)
    - [create_wireless_gateway_task](#create_wireless_gateway_task)
    - [create_wireless_gateway_task_definition](#create_wireless_gateway_task_definition)
    - [delete_destination](#delete_destination)
    - [delete_device_profile](#delete_device_profile)
    - [delete_fuota_task](#delete_fuota_task)
    - [delete_multicast_group](#delete_multicast_group)
    - [delete_queued_messages](#delete_queued_messages)
    - [delete_service_profile](#delete_service_profile)
    - [delete_wireless_device](#delete_wireless_device)
    - [delete_wireless_gateway](#delete_wireless_gateway)
    - [delete_wireless_gateway_task](#delete_wireless_gateway_task)
    - [delete_wireless_gateway_task_definition](#delete_wireless_gateway_task_definition)
    - [disassociate_aws_account_from_partner_account](#disassociate_aws_account_from_partner_account)
    - [disassociate_multicast_group_from_fuota_task](#disassociate_multicast_group_from_fuota_task)
    - [disassociate_wireless_device_from_fuota_task](#disassociate_wireless_device_from_fuota_task)
    - [disassociate_wireless_device_from_multicast_group](#disassociate_wireless_device_from_multicast_group)
    - [disassociate_wireless_device_from_thing](#disassociate_wireless_device_from_thing)
    - [disassociate_wireless_gateway_from_certificate](#disassociate_wireless_gateway_from_certificate)
    - [disassociate_wireless_gateway_from_thing](#disassociate_wireless_gateway_from_thing)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_destination](#get_destination)
    - [get_device_profile](#get_device_profile)
    - [get_fuota_task](#get_fuota_task)
    - [get_log_levels_by_resource_types](#get_log_levels_by_resource_types)
    - [get_multicast_group](#get_multicast_group)
    - [get_multicast_group_session](#get_multicast_group_session)
    - [get_network_analyzer_configuration](#get_network_analyzer_configuration)
    - [get_partner_account](#get_partner_account)
    - [get_resource_event_configuration](#get_resource_event_configuration)
    - [get_resource_log_level](#get_resource_log_level)
    - [get_service_endpoint](#get_service_endpoint)
    - [get_service_profile](#get_service_profile)
    - [get_wireless_device](#get_wireless_device)
    - [get_wireless_device_statistics](#get_wireless_device_statistics)
    - [get_wireless_gateway](#get_wireless_gateway)
    - [get_wireless_gateway_certificate](#get_wireless_gateway_certificate)
    - [get_wireless_gateway_firmware_information](#get_wireless_gateway_firmware_information)
    - [get_wireless_gateway_statistics](#get_wireless_gateway_statistics)
    - [get_wireless_gateway_task](#get_wireless_gateway_task)
    - [get_wireless_gateway_task_definition](#get_wireless_gateway_task_definition)
    - [list_destinations](#list_destinations)
    - [list_device_profiles](#list_device_profiles)
    - [list_fuota_tasks](#list_fuota_tasks)
    - [list_multicast_groups](#list_multicast_groups)
    - [list_multicast_groups_by_fuota_task](#list_multicast_groups_by_fuota_task)
    - [list_partner_accounts](#list_partner_accounts)
    - [list_queued_messages](#list_queued_messages)
    - [list_service_profiles](#list_service_profiles)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_wireless_devices](#list_wireless_devices)
    - [list_wireless_gateway_task_definitions](#list_wireless_gateway_task_definitions)
    - [list_wireless_gateways](#list_wireless_gateways)
    - [put_resource_log_level](#put_resource_log_level)
    - [reset_all_resource_log_levels](#reset_all_resource_log_levels)
    - [reset_resource_log_level](#reset_resource_log_level)
    - [send_data_to_multicast_group](#send_data_to_multicast_group)
    - [send_data_to_wireless_device](#send_data_to_wireless_device)
    - [start_bulk_associate_wireless_device_with_multicast_group](#start_bulk_associate_wireless_device_with_multicast_group)
    - [start_bulk_disassociate_wireless_device_from_multicast_group](#start_bulk_disassociate_wireless_device_from_multicast_group)
    - [start_fuota_task](#start_fuota_task)
    - [start_multicast_group_session](#start_multicast_group_session)
    - [tag_resource](#tag_resource)
    - [test_wireless_device](#test_wireless_device)
    - [untag_resource](#untag_resource)
    - [update_destination](#update_destination)
    - [update_fuota_task](#update_fuota_task)
    - [update_log_levels_by_resource_types](#update_log_levels_by_resource_types)
    - [update_multicast_group](#update_multicast_group)
    - [update_network_analyzer_configuration](#update_network_analyzer_configuration)
    - [update_partner_account](#update_partner_account)
    - [update_resource_event_configuration](#update_resource_event_configuration)
    - [update_wireless_device](#update_wireless_device)
    - [update_wireless_gateway](#update_wireless_gateway)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="iotwirelessclient"></a>

## IoTWirelessClient

Type annotations for `session.create_client("iotwireless")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_iotwireless.client import IoTWirelessClient

session = get_session()
async with session.create_client("iotwireless") as client:
    client: IoTWirelessClient
```

Boto3 documentation:
[IoTWireless.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_iotwireless.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ThrottlingException`
- `Exceptions.TooManyTagsException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

IoTWirelessClient exceptions.

Type annotations for `session.create_client("iotwireless").exceptions` method.

Boto3 documentation:
[IoTWireless.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate\_aws\_account\_with\_partner\_account"></a>

### associate_aws_account_with_partner_account

Associates a partner account with your AWS account.

Type annotations for
`session.create_client("iotwireless").associate_aws_account_with_partner_account`
method.

Boto3 documentation:
[IoTWireless.Client.associate_aws_account_with_partner_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_aws_account_with_partner_account)

Asynchronous method. Use
`await associate_aws_account_with_partner_account(...)` for a synchronous call.

Arguments mapping described in
[AssociateAwsAccountWithPartnerAccountRequestRequestTypeDef](./type_defs.md#associateawsaccountwithpartneraccountrequestrequesttypedef).

Keyword-only arguments:

- `Sidewalk`:
  [SidewalkAccountInfoTypeDef](./type_defs.md#sidewalkaccountinfotypedef)
  *(required)*
- `ClientRequestToken`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[AssociateAwsAccountWithPartnerAccountResponseTypeDef](./type_defs.md#associateawsaccountwithpartneraccountresponsetypedef).

<a id="associate\_multicast\_group\_with\_fuota\_task"></a>

### associate_multicast_group_with_fuota_task

Associate a multicast group with a FUOTA task.

Type annotations for
`session.create_client("iotwireless").associate_multicast_group_with_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.associate_multicast_group_with_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_multicast_group_with_fuota_task)

Asynchronous method. Use `await associate_multicast_group_with_fuota_task(...)`
for a synchronous call.

Arguments mapping described in
[AssociateMulticastGroupWithFuotaTaskRequestRequestTypeDef](./type_defs.md#associatemulticastgroupwithfuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `MulticastGroupId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="associate\_wireless\_device\_with\_fuota\_task"></a>

### associate_wireless_device_with_fuota_task

Associate a wireless device with a FUOTA task.

Type annotations for
`session.create_client("iotwireless").associate_wireless_device_with_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.associate_wireless_device_with_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_wireless_device_with_fuota_task)

Asynchronous method. Use `await associate_wireless_device_with_fuota_task(...)`
for a synchronous call.

Arguments mapping described in
[AssociateWirelessDeviceWithFuotaTaskRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewithfuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `WirelessDeviceId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="associate\_wireless\_device\_with\_multicast\_group"></a>

### associate_wireless_device_with_multicast_group

Associates a wireless device with a multicast group.

Type annotations for
`session.create_client("iotwireless").associate_wireless_device_with_multicast_group`
method.

Boto3 documentation:
[IoTWireless.Client.associate_wireless_device_with_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_wireless_device_with_multicast_group)

Asynchronous method. Use
`await associate_wireless_device_with_multicast_group(...)` for a synchronous
call.

Arguments mapping described in
[AssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewithmulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `WirelessDeviceId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="associate\_wireless\_device\_with\_thing"></a>

### associate_wireless_device_with_thing

Associates a wireless device with a thing.

Type annotations for
`session.create_client("iotwireless").associate_wireless_device_with_thing`
method.

Boto3 documentation:
[IoTWireless.Client.associate_wireless_device_with_thing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_wireless_device_with_thing)

Asynchronous method. Use `await associate_wireless_device_with_thing(...)` for
a synchronous call.

Arguments mapping described in
[AssociateWirelessDeviceWithThingRequestRequestTypeDef](./type_defs.md#associatewirelessdevicewiththingrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `ThingArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="associate\_wireless\_gateway\_with\_certificate"></a>

### associate_wireless_gateway_with_certificate

Associates a wireless gateway with a certificate.

Type annotations for
`session.create_client("iotwireless").associate_wireless_gateway_with_certificate`
method.

Boto3 documentation:
[IoTWireless.Client.associate_wireless_gateway_with_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_wireless_gateway_with_certificate)

Asynchronous method. Use
`await associate_wireless_gateway_with_certificate(...)` for a synchronous
call.

Arguments mapping described in
[AssociateWirelessGatewayWithCertificateRequestRequestTypeDef](./type_defs.md#associatewirelessgatewaywithcertificaterequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `IotCertificateId`: `str` *(required)*

Returns a `Coroutine` for
[AssociateWirelessGatewayWithCertificateResponseTypeDef](./type_defs.md#associatewirelessgatewaywithcertificateresponsetypedef).

<a id="associate\_wireless\_gateway\_with\_thing"></a>

### associate_wireless_gateway_with_thing

Associates a wireless gateway with a thing.

Type annotations for
`session.create_client("iotwireless").associate_wireless_gateway_with_thing`
method.

Boto3 documentation:
[IoTWireless.Client.associate_wireless_gateway_with_thing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.associate_wireless_gateway_with_thing)

Asynchronous method. Use `await associate_wireless_gateway_with_thing(...)` for
a synchronous call.

Arguments mapping described in
[AssociateWirelessGatewayWithThingRequestRequestTypeDef](./type_defs.md#associatewirelessgatewaywiththingrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `ThingArn`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("iotwireless").can_paginate`
method.

Boto3 documentation:
[IoTWireless.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_multicast\_group\_session"></a>

### cancel_multicast_group_session

Cancels an existing multicast group session.

Type annotations for
`session.create_client("iotwireless").cancel_multicast_group_session` method.

Boto3 documentation:
[IoTWireless.Client.cancel_multicast_group_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.cancel_multicast_group_session)

Asynchronous method. Use `await cancel_multicast_group_session(...)` for a
synchronous call.

Arguments mapping described in
[CancelMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#cancelmulticastgroupsessionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create\_destination"></a>

### create_destination

Creates a new destination that maps a device message to an AWS IoT rule.

Type annotations for `session.create_client("iotwireless").create_destination`
method.

Boto3 documentation:
[IoTWireless.Client.create_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_destination)

Asynchronous method. Use `await create_destination(...)` for a synchronous
call.

Arguments mapping described in
[CreateDestinationRequestRequestTypeDef](./type_defs.md#createdestinationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ExpressionType`: [ExpressionTypeType](./literals.md#expressiontypetype)
  *(required)*
- `Expression`: `str` *(required)*
- `RoleArn`: `str` *(required)*
- `Description`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ClientRequestToken`: `str`

Returns a `Coroutine` for
[CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef).

<a id="create\_device\_profile"></a>

### create_device_profile

Creates a new device profile.

Type annotations for
`session.create_client("iotwireless").create_device_profile` method.

Boto3 documentation:
[IoTWireless.Client.create_device_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_device_profile)

Asynchronous method. Use `await create_device_profile(...)` for a synchronous
call.

Arguments mapping described in
[CreateDeviceProfileRequestRequestTypeDef](./type_defs.md#createdeviceprofilerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str`
- `LoRaWAN`:
  [LoRaWANDeviceProfileTypeDef](./type_defs.md#lorawandeviceprofiletypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ClientRequestToken`: `str`

Returns a `Coroutine` for
[CreateDeviceProfileResponseTypeDef](./type_defs.md#createdeviceprofileresponsetypedef).

<a id="create\_fuota\_task"></a>

### create_fuota_task

Creates a FUOTA task.

Type annotations for `session.create_client("iotwireless").create_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.create_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_fuota_task)

Asynchronous method. Use `await create_fuota_task(...)` for a synchronous call.

Arguments mapping described in
[CreateFuotaTaskRequestRequestTypeDef](./type_defs.md#createfuotataskrequestrequesttypedef).

Keyword-only arguments:

- `FirmwareUpdateImage`: `str` *(required)*
- `FirmwareUpdateRole`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `ClientRequestToken`: `str`
- `LoRaWAN`: [LoRaWANFuotaTaskTypeDef](./type_defs.md#lorawanfuotatasktypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateFuotaTaskResponseTypeDef](./type_defs.md#createfuotataskresponsetypedef).

<a id="create\_multicast\_group"></a>

### create_multicast_group

Creates a multicast group.

Type annotations for
`session.create_client("iotwireless").create_multicast_group` method.

Boto3 documentation:
[IoTWireless.Client.create_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_multicast_group)

Asynchronous method. Use `await create_multicast_group(...)` for a synchronous
call.

Arguments mapping described in
[CreateMulticastGroupRequestRequestTypeDef](./type_defs.md#createmulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `LoRaWAN`: [LoRaWANMulticastTypeDef](./type_defs.md#lorawanmulticasttypedef)
  *(required)*
- `Name`: `str`
- `Description`: `str`
- `ClientRequestToken`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateMulticastGroupResponseTypeDef](./type_defs.md#createmulticastgroupresponsetypedef).

<a id="create\_service\_profile"></a>

### create_service_profile

Creates a new service profile.

Type annotations for
`session.create_client("iotwireless").create_service_profile` method.

Boto3 documentation:
[IoTWireless.Client.create_service_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_service_profile)

Asynchronous method. Use `await create_service_profile(...)` for a synchronous
call.

Arguments mapping described in
[CreateServiceProfileRequestRequestTypeDef](./type_defs.md#createserviceprofilerequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str`
- `LoRaWAN`:
  [LoRaWANServiceProfileTypeDef](./type_defs.md#lorawanserviceprofiletypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ClientRequestToken`: `str`

Returns a `Coroutine` for
[CreateServiceProfileResponseTypeDef](./type_defs.md#createserviceprofileresponsetypedef).

<a id="create\_wireless\_device"></a>

### create_wireless_device

Provisions a wireless device.

Type annotations for
`session.create_client("iotwireless").create_wireless_device` method.

Boto3 documentation:
[IoTWireless.Client.create_wireless_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_device)

Asynchronous method. Use `await create_wireless_device(...)` for a synchronous
call.

Arguments mapping described in
[CreateWirelessDeviceRequestRequestTypeDef](./type_defs.md#createwirelessdevicerequestrequesttypedef).

Keyword-only arguments:

- `Type`: [WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype)
  *(required)*
- `DestinationName`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `ClientRequestToken`: `str`
- `LoRaWAN`: [LoRaWANDeviceTypeDef](./type_defs.md#lorawandevicetypedef)
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateWirelessDeviceResponseTypeDef](./type_defs.md#createwirelessdeviceresponsetypedef).

<a id="create\_wireless\_gateway"></a>

### create_wireless_gateway

Provisions a wireless gateway.

Type annotations for
`session.create_client("iotwireless").create_wireless_gateway` method.

Boto3 documentation:
[IoTWireless.Client.create_wireless_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_gateway)

Asynchronous method. Use `await create_wireless_gateway(...)` for a synchronous
call.

Arguments mapping described in
[CreateWirelessGatewayRequestRequestTypeDef](./type_defs.md#createwirelessgatewayrequestrequesttypedef).

Keyword-only arguments:

- `LoRaWAN`: [LoRaWANGatewayTypeDef](./type_defs.md#lorawangatewaytypedef)
  *(required)*
- `Name`: `str`
- `Description`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ClientRequestToken`: `str`

Returns a `Coroutine` for
[CreateWirelessGatewayResponseTypeDef](./type_defs.md#createwirelessgatewayresponsetypedef).

<a id="create\_wireless\_gateway\_task"></a>

### create_wireless_gateway_task

Creates a task for a wireless gateway.

Type annotations for
`session.create_client("iotwireless").create_wireless_gateway_task` method.

Boto3 documentation:
[IoTWireless.Client.create_wireless_gateway_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_gateway_task)

Asynchronous method. Use `await create_wireless_gateway_task(...)` for a
synchronous call.

Arguments mapping described in
[CreateWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#createwirelessgatewaytaskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `WirelessGatewayTaskDefinitionId`: `str` *(required)*

Returns a `Coroutine` for
[CreateWirelessGatewayTaskResponseTypeDef](./type_defs.md#createwirelessgatewaytaskresponsetypedef).

<a id="create\_wireless\_gateway\_task\_definition"></a>

### create_wireless_gateway_task_definition

Creates a gateway task definition.

Type annotations for
`session.create_client("iotwireless").create_wireless_gateway_task_definition`
method.

Boto3 documentation:
[IoTWireless.Client.create_wireless_gateway_task_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.create_wireless_gateway_task_definition)

Asynchronous method. Use `await create_wireless_gateway_task_definition(...)`
for a synchronous call.

Arguments mapping described in
[CreateWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#createwirelessgatewaytaskdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `AutoCreateTasks`: `bool` *(required)*
- `Name`: `str`
- `Update`:
  [UpdateWirelessGatewayTaskCreateTypeDef](./type_defs.md#updatewirelessgatewaytaskcreatetypedef)
- `ClientRequestToken`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateWirelessGatewayTaskDefinitionResponseTypeDef](./type_defs.md#createwirelessgatewaytaskdefinitionresponsetypedef).

<a id="delete\_destination"></a>

### delete_destination

Deletes a destination.

Type annotations for `session.create_client("iotwireless").delete_destination`
method.

Boto3 documentation:
[IoTWireless.Client.delete_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_destination)

Asynchronous method. Use `await delete_destination(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDestinationRequestRequestTypeDef](./type_defs.md#deletedestinationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_device\_profile"></a>

### delete_device_profile

Deletes a device profile.

Type annotations for
`session.create_client("iotwireless").delete_device_profile` method.

Boto3 documentation:
[IoTWireless.Client.delete_device_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_device_profile)

Asynchronous method. Use `await delete_device_profile(...)` for a synchronous
call.

Arguments mapping described in
[DeleteDeviceProfileRequestRequestTypeDef](./type_defs.md#deletedeviceprofilerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_fuota\_task"></a>

### delete_fuota_task

Deletes a FUOTA task.

Type annotations for `session.create_client("iotwireless").delete_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.delete_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_fuota_task)

Asynchronous method. Use `await delete_fuota_task(...)` for a synchronous call.

Arguments mapping described in
[DeleteFuotaTaskRequestRequestTypeDef](./type_defs.md#deletefuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_multicast\_group"></a>

### delete_multicast_group

Deletes a multicast group if it is not in use by a fuota task.

Type annotations for
`session.create_client("iotwireless").delete_multicast_group` method.

Boto3 documentation:
[IoTWireless.Client.delete_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_multicast_group)

Asynchronous method. Use `await delete_multicast_group(...)` for a synchronous
call.

Arguments mapping described in
[DeleteMulticastGroupRequestRequestTypeDef](./type_defs.md#deletemulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_queued\_messages"></a>

### delete_queued_messages

The operation to delete queued messages.

Type annotations for
`session.create_client("iotwireless").delete_queued_messages` method.

Boto3 documentation:
[IoTWireless.Client.delete_queued_messages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_queued_messages)

Asynchronous method. Use `await delete_queued_messages(...)` for a synchronous
call.

Arguments mapping described in
[DeleteQueuedMessagesRequestRequestTypeDef](./type_defs.md#deletequeuedmessagesrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `MessageId`: `str` *(required)*
- `WirelessDeviceType`:
  [WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_service\_profile"></a>

### delete_service_profile

Deletes a service profile.

Type annotations for
`session.create_client("iotwireless").delete_service_profile` method.

Boto3 documentation:
[IoTWireless.Client.delete_service_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_service_profile)

Asynchronous method. Use `await delete_service_profile(...)` for a synchronous
call.

Arguments mapping described in
[DeleteServiceProfileRequestRequestTypeDef](./type_defs.md#deleteserviceprofilerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_wireless\_device"></a>

### delete_wireless_device

Deletes a wireless device.

Type annotations for
`session.create_client("iotwireless").delete_wireless_device` method.

Boto3 documentation:
[IoTWireless.Client.delete_wireless_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_wireless_device)

Asynchronous method. Use `await delete_wireless_device(...)` for a synchronous
call.

Arguments mapping described in
[DeleteWirelessDeviceRequestRequestTypeDef](./type_defs.md#deletewirelessdevicerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_wireless\_gateway"></a>

### delete_wireless_gateway

Deletes a wireless gateway.

Type annotations for
`session.create_client("iotwireless").delete_wireless_gateway` method.

Boto3 documentation:
[IoTWireless.Client.delete_wireless_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_wireless_gateway)

Asynchronous method. Use `await delete_wireless_gateway(...)` for a synchronous
call.

Arguments mapping described in
[DeleteWirelessGatewayRequestRequestTypeDef](./type_defs.md#deletewirelessgatewayrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_wireless\_gateway\_task"></a>

### delete_wireless_gateway_task

Deletes a wireless gateway task.

Type annotations for
`session.create_client("iotwireless").delete_wireless_gateway_task` method.

Boto3 documentation:
[IoTWireless.Client.delete_wireless_gateway_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_wireless_gateway_task)

Asynchronous method. Use `await delete_wireless_gateway_task(...)` for a
synchronous call.

Arguments mapping described in
[DeleteWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#deletewirelessgatewaytaskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete\_wireless\_gateway\_task\_definition"></a>

### delete_wireless_gateway_task_definition

Deletes a wireless gateway task definition.

Type annotations for
`session.create_client("iotwireless").delete_wireless_gateway_task_definition`
method.

Boto3 documentation:
[IoTWireless.Client.delete_wireless_gateway_task_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.delete_wireless_gateway_task_definition)

Asynchronous method. Use `await delete_wireless_gateway_task_definition(...)`
for a synchronous call.

Arguments mapping described in
[DeleteWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#deletewirelessgatewaytaskdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_aws\_account\_from\_partner\_account"></a>

### disassociate_aws_account_from_partner_account

Disassociates your AWS account from a partner account.

Type annotations for
`session.create_client("iotwireless").disassociate_aws_account_from_partner_account`
method.

Boto3 documentation:
[IoTWireless.Client.disassociate_aws_account_from_partner_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.disassociate_aws_account_from_partner_account)

Asynchronous method. Use
`await disassociate_aws_account_from_partner_account(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateAwsAccountFromPartnerAccountRequestRequestTypeDef](./type_defs.md#disassociateawsaccountfrompartneraccountrequestrequesttypedef).

Keyword-only arguments:

- `PartnerAccountId`: `str` *(required)*
- `PartnerType`: `Literal['Sidewalk']` (see
  [PartnerTypeType](./literals.md#partnertypetype)) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_multicast\_group\_from\_fuota\_task"></a>

### disassociate_multicast_group_from_fuota_task

Disassociates a multicast group from a fuota task.

Type annotations for
`session.create_client("iotwireless").disassociate_multicast_group_from_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.disassociate_multicast_group_from_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.disassociate_multicast_group_from_fuota_task)

Asynchronous method. Use
`await disassociate_multicast_group_from_fuota_task(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateMulticastGroupFromFuotaTaskRequestRequestTypeDef](./type_defs.md#disassociatemulticastgroupfromfuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `MulticastGroupId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_wireless\_device\_from\_fuota\_task"></a>

### disassociate_wireless_device_from_fuota_task

Disassociates a wireless device from a FUOTA task.

Type annotations for
`session.create_client("iotwireless").disassociate_wireless_device_from_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.disassociate_wireless_device_from_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.disassociate_wireless_device_from_fuota_task)

Asynchronous method. Use
`await disassociate_wireless_device_from_fuota_task(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateWirelessDeviceFromFuotaTaskRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefromfuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `WirelessDeviceId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_wireless\_device\_from\_multicast\_group"></a>

### disassociate_wireless_device_from_multicast_group

Disassociates a wireless device from a multicast group.

Type annotations for
`session.create_client("iotwireless").disassociate_wireless_device_from_multicast_group`
method.

Boto3 documentation:
[IoTWireless.Client.disassociate_wireless_device_from_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.disassociate_wireless_device_from_multicast_group)

Asynchronous method. Use
`await disassociate_wireless_device_from_multicast_group(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefrommulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `WirelessDeviceId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_wireless\_device\_from\_thing"></a>

### disassociate_wireless_device_from_thing

Disassociates a wireless device from its currently associated thing.

Type annotations for
`session.create_client("iotwireless").disassociate_wireless_device_from_thing`
method.

Boto3 documentation:
[IoTWireless.Client.disassociate_wireless_device_from_thing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.disassociate_wireless_device_from_thing)

Asynchronous method. Use `await disassociate_wireless_device_from_thing(...)`
for a synchronous call.

Arguments mapping described in
[DisassociateWirelessDeviceFromThingRequestRequestTypeDef](./type_defs.md#disassociatewirelessdevicefromthingrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_wireless\_gateway\_from\_certificate"></a>

### disassociate_wireless_gateway_from_certificate

Disassociates a wireless gateway from its currently associated certificate.

Type annotations for
`session.create_client("iotwireless").disassociate_wireless_gateway_from_certificate`
method.

Boto3 documentation:
[IoTWireless.Client.disassociate_wireless_gateway_from_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.disassociate_wireless_gateway_from_certificate)

Asynchronous method. Use
`await disassociate_wireless_gateway_from_certificate(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateWirelessGatewayFromCertificateRequestRequestTypeDef](./type_defs.md#disassociatewirelessgatewayfromcertificaterequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate\_wireless\_gateway\_from\_thing"></a>

### disassociate_wireless_gateway_from_thing

Disassociates a wireless gateway from its currently associated thing.

Type annotations for
`session.create_client("iotwireless").disassociate_wireless_gateway_from_thing`
method.

Boto3 documentation:
[IoTWireless.Client.disassociate_wireless_gateway_from_thing](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.disassociate_wireless_gateway_from_thing)

Asynchronous method. Use `await disassociate_wireless_gateway_from_thing(...)`
for a synchronous call.

Arguments mapping described in
[DisassociateWirelessGatewayFromThingRequestRequestTypeDef](./type_defs.md#disassociatewirelessgatewayfromthingrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("iotwireless").generate_presigned_url` method.

Boto3 documentation:
[IoTWireless.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_destination"></a>

### get_destination

Gets information about a destination.

Type annotations for `session.create_client("iotwireless").get_destination`
method.

Boto3 documentation:
[IoTWireless.Client.get_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_destination)

Asynchronous method. Use `await get_destination(...)` for a synchronous call.

Arguments mapping described in
[GetDestinationRequestRequestTypeDef](./type_defs.md#getdestinationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*

Returns a `Coroutine` for
[GetDestinationResponseTypeDef](./type_defs.md#getdestinationresponsetypedef).

<a id="get\_device\_profile"></a>

### get_device_profile

Gets information about a device profile.

Type annotations for `session.create_client("iotwireless").get_device_profile`
method.

Boto3 documentation:
[IoTWireless.Client.get_device_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_device_profile)

Asynchronous method. Use `await get_device_profile(...)` for a synchronous
call.

Arguments mapping described in
[GetDeviceProfileRequestRequestTypeDef](./type_defs.md#getdeviceprofilerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetDeviceProfileResponseTypeDef](./type_defs.md#getdeviceprofileresponsetypedef).

<a id="get\_fuota\_task"></a>

### get_fuota_task

Gets information about a FUOTA task.

Type annotations for `session.create_client("iotwireless").get_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.get_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_fuota_task)

Asynchronous method. Use `await get_fuota_task(...)` for a synchronous call.

Arguments mapping described in
[GetFuotaTaskRequestRequestTypeDef](./type_defs.md#getfuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetFuotaTaskResponseTypeDef](./type_defs.md#getfuotataskresponsetypedef).

<a id="get\_log\_levels\_by\_resource\_types"></a>

### get_log_levels_by_resource_types

Returns current default log levels or log levels by resource types.

Type annotations for
`session.create_client("iotwireless").get_log_levels_by_resource_types` method.

Boto3 documentation:
[IoTWireless.Client.get_log_levels_by_resource_types](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_log_levels_by_resource_types)

Asynchronous method. Use `await get_log_levels_by_resource_types(...)` for a
synchronous call.

Returns a `Coroutine` for
[GetLogLevelsByResourceTypesResponseTypeDef](./type_defs.md#getloglevelsbyresourcetypesresponsetypedef).

<a id="get\_multicast\_group"></a>

### get_multicast_group

Gets information about a multicast group.

Type annotations for `session.create_client("iotwireless").get_multicast_group`
method.

Boto3 documentation:
[IoTWireless.Client.get_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_multicast_group)

Asynchronous method. Use `await get_multicast_group(...)` for a synchronous
call.

Arguments mapping described in
[GetMulticastGroupRequestRequestTypeDef](./type_defs.md#getmulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetMulticastGroupResponseTypeDef](./type_defs.md#getmulticastgroupresponsetypedef).

<a id="get\_multicast\_group\_session"></a>

### get_multicast_group_session

Gets information about a multicast group session.

Type annotations for
`session.create_client("iotwireless").get_multicast_group_session` method.

Boto3 documentation:
[IoTWireless.Client.get_multicast_group_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_multicast_group_session)

Asynchronous method. Use `await get_multicast_group_session(...)` for a
synchronous call.

Arguments mapping described in
[GetMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#getmulticastgroupsessionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetMulticastGroupSessionResponseTypeDef](./type_defs.md#getmulticastgroupsessionresponsetypedef).

<a id="get\_network\_analyzer\_configuration"></a>

### get_network_analyzer_configuration

Get NetworkAnalyzer configuration.

Type annotations for
`session.create_client("iotwireless").get_network_analyzer_configuration`
method.

Boto3 documentation:
[IoTWireless.Client.get_network_analyzer_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_network_analyzer_configuration)

Asynchronous method. Use `await get_network_analyzer_configuration(...)` for a
synchronous call.

Arguments mapping described in
[GetNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#getnetworkanalyzerconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationName`: `str` *(required)*

Returns a `Coroutine` for
[GetNetworkAnalyzerConfigurationResponseTypeDef](./type_defs.md#getnetworkanalyzerconfigurationresponsetypedef).

<a id="get\_partner\_account"></a>

### get_partner_account

Gets information about a partner account.

Type annotations for `session.create_client("iotwireless").get_partner_account`
method.

Boto3 documentation:
[IoTWireless.Client.get_partner_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_partner_account)

Asynchronous method. Use `await get_partner_account(...)` for a synchronous
call.

Arguments mapping described in
[GetPartnerAccountRequestRequestTypeDef](./type_defs.md#getpartneraccountrequestrequesttypedef).

Keyword-only arguments:

- `PartnerAccountId`: `str` *(required)*
- `PartnerType`: `Literal['Sidewalk']` (see
  [PartnerTypeType](./literals.md#partnertypetype)) *(required)*

Returns a `Coroutine` for
[GetPartnerAccountResponseTypeDef](./type_defs.md#getpartneraccountresponsetypedef).

<a id="get\_resource\_event\_configuration"></a>

### get_resource_event_configuration

Get the event configuration for a particular resource identifier.

Type annotations for
`session.create_client("iotwireless").get_resource_event_configuration` method.

Boto3 documentation:
[IoTWireless.Client.get_resource_event_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_resource_event_configuration)

Asynchronous method. Use `await get_resource_event_configuration(...)` for a
synchronous call.

Arguments mapping described in
[GetResourceEventConfigurationRequestRequestTypeDef](./type_defs.md#getresourceeventconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Identifier`: `str` *(required)*
- `IdentifierType`: `Literal['PartnerAccountId']` (see
  [IdentifierTypeType](./literals.md#identifiertypetype)) *(required)*
- `PartnerType`: `Literal['Sidewalk']` (see
  [EventNotificationPartnerTypeType](./literals.md#eventnotificationpartnertypetype))

Returns a `Coroutine` for
[GetResourceEventConfigurationResponseTypeDef](./type_defs.md#getresourceeventconfigurationresponsetypedef).

<a id="get\_resource\_log\_level"></a>

### get_resource_log_level

Fetches the log-level override, if any, for a given resource-ID and resource-
type.

Type annotations for
`session.create_client("iotwireless").get_resource_log_level` method.

Boto3 documentation:
[IoTWireless.Client.get_resource_log_level](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_resource_log_level)

Asynchronous method. Use `await get_resource_log_level(...)` for a synchronous
call.

Arguments mapping described in
[GetResourceLogLevelRequestRequestTypeDef](./type_defs.md#getresourceloglevelrequestrequesttypedef).

Keyword-only arguments:

- `ResourceIdentifier`: `str` *(required)*
- `ResourceType`: `str` *(required)*

Returns a `Coroutine` for
[GetResourceLogLevelResponseTypeDef](./type_defs.md#getresourceloglevelresponsetypedef).

<a id="get\_service\_endpoint"></a>

### get_service_endpoint

Gets the account-specific endpoint for Configuration and Update Server (CUPS)
protocol or LoRaWAN Network Server (LNS) connections.

Type annotations for
`session.create_client("iotwireless").get_service_endpoint` method.

Boto3 documentation:
[IoTWireless.Client.get_service_endpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_service_endpoint)

Asynchronous method. Use `await get_service_endpoint(...)` for a synchronous
call.

Arguments mapping described in
[GetServiceEndpointRequestRequestTypeDef](./type_defs.md#getserviceendpointrequestrequesttypedef).

Keyword-only arguments:

- `ServiceType`:
  [WirelessGatewayServiceTypeType](./literals.md#wirelessgatewayservicetypetype)

Returns a `Coroutine` for
[GetServiceEndpointResponseTypeDef](./type_defs.md#getserviceendpointresponsetypedef).

<a id="get\_service\_profile"></a>

### get_service_profile

Gets information about a service profile.

Type annotations for `session.create_client("iotwireless").get_service_profile`
method.

Boto3 documentation:
[IoTWireless.Client.get_service_profile](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_service_profile)

Asynchronous method. Use `await get_service_profile(...)` for a synchronous
call.

Arguments mapping described in
[GetServiceProfileRequestRequestTypeDef](./type_defs.md#getserviceprofilerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetServiceProfileResponseTypeDef](./type_defs.md#getserviceprofileresponsetypedef).

<a id="get\_wireless\_device"></a>

### get_wireless_device

Gets information about a wireless device.

Type annotations for `session.create_client("iotwireless").get_wireless_device`
method.

Boto3 documentation:
[IoTWireless.Client.get_wireless_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_wireless_device)

Asynchronous method. Use `await get_wireless_device(...)` for a synchronous
call.

Arguments mapping described in
[GetWirelessDeviceRequestRequestTypeDef](./type_defs.md#getwirelessdevicerequestrequesttypedef).

Keyword-only arguments:

- `Identifier`: `str` *(required)*
- `IdentifierType`:
  [WirelessDeviceIdTypeType](./literals.md#wirelessdeviceidtypetype)
  *(required)*

Returns a `Coroutine` for
[GetWirelessDeviceResponseTypeDef](./type_defs.md#getwirelessdeviceresponsetypedef).

<a id="get\_wireless\_device\_statistics"></a>

### get_wireless_device_statistics

Gets operating information about a wireless device.

Type annotations for
`session.create_client("iotwireless").get_wireless_device_statistics` method.

Boto3 documentation:
[IoTWireless.Client.get_wireless_device_statistics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_wireless_device_statistics)

Asynchronous method. Use `await get_wireless_device_statistics(...)` for a
synchronous call.

Arguments mapping described in
[GetWirelessDeviceStatisticsRequestRequestTypeDef](./type_defs.md#getwirelessdevicestatisticsrequestrequesttypedef).

Keyword-only arguments:

- `WirelessDeviceId`: `str` *(required)*

Returns a `Coroutine` for
[GetWirelessDeviceStatisticsResponseTypeDef](./type_defs.md#getwirelessdevicestatisticsresponsetypedef).

<a id="get\_wireless\_gateway"></a>

### get_wireless_gateway

Gets information about a wireless gateway.

Type annotations for
`session.create_client("iotwireless").get_wireless_gateway` method.

Boto3 documentation:
[IoTWireless.Client.get_wireless_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_wireless_gateway)

Asynchronous method. Use `await get_wireless_gateway(...)` for a synchronous
call.

Arguments mapping described in
[GetWirelessGatewayRequestRequestTypeDef](./type_defs.md#getwirelessgatewayrequestrequesttypedef).

Keyword-only arguments:

- `Identifier`: `str` *(required)*
- `IdentifierType`:
  [WirelessGatewayIdTypeType](./literals.md#wirelessgatewayidtypetype)
  *(required)*

Returns a `Coroutine` for
[GetWirelessGatewayResponseTypeDef](./type_defs.md#getwirelessgatewayresponsetypedef).

<a id="get\_wireless\_gateway\_certificate"></a>

### get_wireless_gateway_certificate

Gets the ID of the certificate that is currently associated with a wireless
gateway.

Type annotations for
`session.create_client("iotwireless").get_wireless_gateway_certificate` method.

Boto3 documentation:
[IoTWireless.Client.get_wireless_gateway_certificate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_wireless_gateway_certificate)

Asynchronous method. Use `await get_wireless_gateway_certificate(...)` for a
synchronous call.

Arguments mapping described in
[GetWirelessGatewayCertificateRequestRequestTypeDef](./type_defs.md#getwirelessgatewaycertificaterequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetWirelessGatewayCertificateResponseTypeDef](./type_defs.md#getwirelessgatewaycertificateresponsetypedef).

<a id="get\_wireless\_gateway\_firmware\_information"></a>

### get_wireless_gateway_firmware_information

Gets the firmware version and other information about a wireless gateway.

Type annotations for
`session.create_client("iotwireless").get_wireless_gateway_firmware_information`
method.

Boto3 documentation:
[IoTWireless.Client.get_wireless_gateway_firmware_information](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_wireless_gateway_firmware_information)

Asynchronous method. Use `await get_wireless_gateway_firmware_information(...)`
for a synchronous call.

Arguments mapping described in
[GetWirelessGatewayFirmwareInformationRequestRequestTypeDef](./type_defs.md#getwirelessgatewayfirmwareinformationrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetWirelessGatewayFirmwareInformationResponseTypeDef](./type_defs.md#getwirelessgatewayfirmwareinformationresponsetypedef).

<a id="get\_wireless\_gateway\_statistics"></a>

### get_wireless_gateway_statistics

Gets operating information about a wireless gateway.

Type annotations for
`session.create_client("iotwireless").get_wireless_gateway_statistics` method.

Boto3 documentation:
[IoTWireless.Client.get_wireless_gateway_statistics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_wireless_gateway_statistics)

Asynchronous method. Use `await get_wireless_gateway_statistics(...)` for a
synchronous call.

Arguments mapping described in
[GetWirelessGatewayStatisticsRequestRequestTypeDef](./type_defs.md#getwirelessgatewaystatisticsrequestrequesttypedef).

Keyword-only arguments:

- `WirelessGatewayId`: `str` *(required)*

Returns a `Coroutine` for
[GetWirelessGatewayStatisticsResponseTypeDef](./type_defs.md#getwirelessgatewaystatisticsresponsetypedef).

<a id="get\_wireless\_gateway\_task"></a>

### get_wireless_gateway_task

Gets information about a wireless gateway task.

Type annotations for
`session.create_client("iotwireless").get_wireless_gateway_task` method.

Boto3 documentation:
[IoTWireless.Client.get_wireless_gateway_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_wireless_gateway_task)

Asynchronous method. Use `await get_wireless_gateway_task(...)` for a
synchronous call.

Arguments mapping described in
[GetWirelessGatewayTaskRequestRequestTypeDef](./type_defs.md#getwirelessgatewaytaskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetWirelessGatewayTaskResponseTypeDef](./type_defs.md#getwirelessgatewaytaskresponsetypedef).

<a id="get\_wireless\_gateway\_task\_definition"></a>

### get_wireless_gateway_task_definition

Gets information about a wireless gateway task definition.

Type annotations for
`session.create_client("iotwireless").get_wireless_gateway_task_definition`
method.

Boto3 documentation:
[IoTWireless.Client.get_wireless_gateway_task_definition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.get_wireless_gateway_task_definition)

Asynchronous method. Use `await get_wireless_gateway_task_definition(...)` for
a synchronous call.

Arguments mapping described in
[GetWirelessGatewayTaskDefinitionRequestRequestTypeDef](./type_defs.md#getwirelessgatewaytaskdefinitionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[GetWirelessGatewayTaskDefinitionResponseTypeDef](./type_defs.md#getwirelessgatewaytaskdefinitionresponsetypedef).

<a id="list\_destinations"></a>

### list_destinations

Lists the destinations registered to your AWS account.

Type annotations for `session.create_client("iotwireless").list_destinations`
method.

Boto3 documentation:
[IoTWireless.Client.list_destinations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_destinations)

Asynchronous method. Use `await list_destinations(...)` for a synchronous call.

Arguments mapping described in
[ListDestinationsRequestRequestTypeDef](./type_defs.md#listdestinationsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef).

<a id="list\_device\_profiles"></a>

### list_device_profiles

Lists the device profiles registered to your AWS account.

Type annotations for
`session.create_client("iotwireless").list_device_profiles` method.

Boto3 documentation:
[IoTWireless.Client.list_device_profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_device_profiles)

Asynchronous method. Use `await list_device_profiles(...)` for a synchronous
call.

Arguments mapping described in
[ListDeviceProfilesRequestRequestTypeDef](./type_defs.md#listdeviceprofilesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListDeviceProfilesResponseTypeDef](./type_defs.md#listdeviceprofilesresponsetypedef).

<a id="list\_fuota\_tasks"></a>

### list_fuota_tasks

Lists the FUOTA tasks registered to your AWS account.

Type annotations for `session.create_client("iotwireless").list_fuota_tasks`
method.

Boto3 documentation:
[IoTWireless.Client.list_fuota_tasks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_fuota_tasks)

Asynchronous method. Use `await list_fuota_tasks(...)` for a synchronous call.

Arguments mapping described in
[ListFuotaTasksRequestRequestTypeDef](./type_defs.md#listfuotatasksrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListFuotaTasksResponseTypeDef](./type_defs.md#listfuotatasksresponsetypedef).

<a id="list\_multicast\_groups"></a>

### list_multicast_groups

Lists the multicast groups registered to your AWS account.

Type annotations for
`session.create_client("iotwireless").list_multicast_groups` method.

Boto3 documentation:
[IoTWireless.Client.list_multicast_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_multicast_groups)

Asynchronous method. Use `await list_multicast_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListMulticastGroupsRequestRequestTypeDef](./type_defs.md#listmulticastgroupsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListMulticastGroupsResponseTypeDef](./type_defs.md#listmulticastgroupsresponsetypedef).

<a id="list\_multicast\_groups\_by\_fuota\_task"></a>

### list_multicast_groups_by_fuota_task

List all multicast groups associated with a fuota task.

Type annotations for
`session.create_client("iotwireless").list_multicast_groups_by_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.list_multicast_groups_by_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_multicast_groups_by_fuota_task)

Asynchronous method. Use `await list_multicast_groups_by_fuota_task(...)` for a
synchronous call.

Arguments mapping described in
[ListMulticastGroupsByFuotaTaskRequestRequestTypeDef](./type_defs.md#listmulticastgroupsbyfuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListMulticastGroupsByFuotaTaskResponseTypeDef](./type_defs.md#listmulticastgroupsbyfuotataskresponsetypedef).

<a id="list\_partner\_accounts"></a>

### list_partner_accounts

Lists the partner accounts associated with your AWS account.

Type annotations for
`session.create_client("iotwireless").list_partner_accounts` method.

Boto3 documentation:
[IoTWireless.Client.list_partner_accounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_partner_accounts)

Asynchronous method. Use `await list_partner_accounts(...)` for a synchronous
call.

Arguments mapping described in
[ListPartnerAccountsRequestRequestTypeDef](./type_defs.md#listpartneraccountsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListPartnerAccountsResponseTypeDef](./type_defs.md#listpartneraccountsresponsetypedef).

<a id="list\_queued\_messages"></a>

### list_queued_messages

The operation to list queued messages.

Type annotations for
`session.create_client("iotwireless").list_queued_messages` method.

Boto3 documentation:
[IoTWireless.Client.list_queued_messages](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_queued_messages)

Asynchronous method. Use `await list_queued_messages(...)` for a synchronous
call.

Arguments mapping described in
[ListQueuedMessagesRequestRequestTypeDef](./type_defs.md#listqueuedmessagesrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `NextToken`: `str`
- `MaxResults`: `int`
- `WirelessDeviceType`:
  [WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype)

Returns a `Coroutine` for
[ListQueuedMessagesResponseTypeDef](./type_defs.md#listqueuedmessagesresponsetypedef).

<a id="list\_service\_profiles"></a>

### list_service_profiles

Lists the service profiles registered to your AWS account.

Type annotations for
`session.create_client("iotwireless").list_service_profiles` method.

Boto3 documentation:
[IoTWireless.Client.list_service_profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_service_profiles)

Asynchronous method. Use `await list_service_profiles(...)` for a synchronous
call.

Arguments mapping described in
[ListServiceProfilesRequestRequestTypeDef](./type_defs.md#listserviceprofilesrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListServiceProfilesResponseTypeDef](./type_defs.md#listserviceprofilesresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists the tags (metadata) you have assigned to the resource.

Type annotations for
`session.create_client("iotwireless").list_tags_for_resource` method.

Boto3 documentation:
[IoTWireless.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list\_wireless\_devices"></a>

### list_wireless_devices

Lists the wireless devices registered to your AWS account.

Type annotations for
`session.create_client("iotwireless").list_wireless_devices` method.

Boto3 documentation:
[IoTWireless.Client.list_wireless_devices](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_wireless_devices)

Asynchronous method. Use `await list_wireless_devices(...)` for a synchronous
call.

Arguments mapping described in
[ListWirelessDevicesRequestRequestTypeDef](./type_defs.md#listwirelessdevicesrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `DestinationName`: `str`
- `DeviceProfileId`: `str`
- `ServiceProfileId`: `str`
- `WirelessDeviceType`:
  [WirelessDeviceTypeType](./literals.md#wirelessdevicetypetype)
- `FuotaTaskId`: `str`
- `MulticastGroupId`: `str`

Returns a `Coroutine` for
[ListWirelessDevicesResponseTypeDef](./type_defs.md#listwirelessdevicesresponsetypedef).

<a id="list\_wireless\_gateway\_task\_definitions"></a>

### list_wireless_gateway_task_definitions

List the wireless gateway tasks definitions registered to your AWS account.

Type annotations for
`session.create_client("iotwireless").list_wireless_gateway_task_definitions`
method.

Boto3 documentation:
[IoTWireless.Client.list_wireless_gateway_task_definitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_wireless_gateway_task_definitions)

Asynchronous method. Use `await list_wireless_gateway_task_definitions(...)`
for a synchronous call.

Arguments mapping described in
[ListWirelessGatewayTaskDefinitionsRequestRequestTypeDef](./type_defs.md#listwirelessgatewaytaskdefinitionsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `TaskDefinitionType`: `Literal['UPDATE']` (see
  [WirelessGatewayTaskDefinitionTypeType](./literals.md#wirelessgatewaytaskdefinitiontypetype))

Returns a `Coroutine` for
[ListWirelessGatewayTaskDefinitionsResponseTypeDef](./type_defs.md#listwirelessgatewaytaskdefinitionsresponsetypedef).

<a id="list\_wireless\_gateways"></a>

### list_wireless_gateways

Lists the wireless gateways registered to your AWS account.

Type annotations for
`session.create_client("iotwireless").list_wireless_gateways` method.

Boto3 documentation:
[IoTWireless.Client.list_wireless_gateways](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.list_wireless_gateways)

Asynchronous method. Use `await list_wireless_gateways(...)` for a synchronous
call.

Arguments mapping described in
[ListWirelessGatewaysRequestRequestTypeDef](./type_defs.md#listwirelessgatewaysrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListWirelessGatewaysResponseTypeDef](./type_defs.md#listwirelessgatewaysresponsetypedef).

<a id="put\_resource\_log\_level"></a>

### put_resource_log_level

Sets the log-level override for a resource-ID and resource-type.

Type annotations for
`session.create_client("iotwireless").put_resource_log_level` method.

Boto3 documentation:
[IoTWireless.Client.put_resource_log_level](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.put_resource_log_level)

Asynchronous method. Use `await put_resource_log_level(...)` for a synchronous
call.

Arguments mapping described in
[PutResourceLogLevelRequestRequestTypeDef](./type_defs.md#putresourceloglevelrequestrequesttypedef).

Keyword-only arguments:

- `ResourceIdentifier`: `str` *(required)*
- `ResourceType`: `str` *(required)*
- `LogLevel`: [LogLevelType](./literals.md#logleveltype) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="reset\_all\_resource\_log\_levels"></a>

### reset_all_resource_log_levels

Removes the log-level overrides for all resources; both wireless devices and
wireless gateways.

Type annotations for
`session.create_client("iotwireless").reset_all_resource_log_levels` method.

Boto3 documentation:
[IoTWireless.Client.reset_all_resource_log_levels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.reset_all_resource_log_levels)

Asynchronous method. Use `await reset_all_resource_log_levels(...)` for a
synchronous call.

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="reset\_resource\_log\_level"></a>

### reset_resource_log_level

Removes the log-level override, if any, for a specific resource-ID and
resource- type.

Type annotations for
`session.create_client("iotwireless").reset_resource_log_level` method.

Boto3 documentation:
[IoTWireless.Client.reset_resource_log_level](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.reset_resource_log_level)

Asynchronous method. Use `await reset_resource_log_level(...)` for a
synchronous call.

Arguments mapping described in
[ResetResourceLogLevelRequestRequestTypeDef](./type_defs.md#resetresourceloglevelrequestrequesttypedef).

Keyword-only arguments:

- `ResourceIdentifier`: `str` *(required)*
- `ResourceType`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="send\_data\_to\_multicast\_group"></a>

### send_data_to_multicast_group

Sends the specified data to a multicast group.

Type annotations for
`session.create_client("iotwireless").send_data_to_multicast_group` method.

Boto3 documentation:
[IoTWireless.Client.send_data_to_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.send_data_to_multicast_group)

Asynchronous method. Use `await send_data_to_multicast_group(...)` for a
synchronous call.

Arguments mapping described in
[SendDataToMulticastGroupRequestRequestTypeDef](./type_defs.md#senddatatomulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `PayloadData`: `str` *(required)*
- `WirelessMetadata`:
  [MulticastWirelessMetadataTypeDef](./type_defs.md#multicastwirelessmetadatatypedef)
  *(required)*

Returns a `Coroutine` for
[SendDataToMulticastGroupResponseTypeDef](./type_defs.md#senddatatomulticastgroupresponsetypedef).

<a id="send\_data\_to\_wireless\_device"></a>

### send_data_to_wireless_device

Sends a decrypted application data frame to a device.

Type annotations for
`session.create_client("iotwireless").send_data_to_wireless_device` method.

Boto3 documentation:
[IoTWireless.Client.send_data_to_wireless_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.send_data_to_wireless_device)

Asynchronous method. Use `await send_data_to_wireless_device(...)` for a
synchronous call.

Arguments mapping described in
[SendDataToWirelessDeviceRequestRequestTypeDef](./type_defs.md#senddatatowirelessdevicerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `TransmitMode`: `int` *(required)*
- `PayloadData`: `str` *(required)*
- `WirelessMetadata`:
  [WirelessMetadataTypeDef](./type_defs.md#wirelessmetadatatypedef)

Returns a `Coroutine` for
[SendDataToWirelessDeviceResponseTypeDef](./type_defs.md#senddatatowirelessdeviceresponsetypedef).

<a id="start\_bulk\_associate\_wireless\_device\_with\_multicast\_group"></a>

### start_bulk_associate_wireless_device_with_multicast_group

Starts a bulk association of all qualifying wireless devices with a multicast
group.

Type annotations for
`session.create_client("iotwireless").start_bulk_associate_wireless_device_with_multicast_group`
method.

Boto3 documentation:
[IoTWireless.Client.start_bulk_associate_wireless_device_with_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_bulk_associate_wireless_device_with_multicast_group)

Asynchronous method. Use
`await start_bulk_associate_wireless_device_with_multicast_group(...)` for a
synchronous call.

Arguments mapping described in
[StartBulkAssociateWirelessDeviceWithMulticastGroupRequestRequestTypeDef](./type_defs.md#startbulkassociatewirelessdevicewithmulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `QueryString`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="start\_bulk\_disassociate\_wireless\_device\_from\_multicast\_group"></a>

### start_bulk_disassociate_wireless_device_from_multicast_group

Starts a bulk disassociatin of all qualifying wireless devices from a multicast
group.

Type annotations for
`session.create_client("iotwireless").start_bulk_disassociate_wireless_device_from_multicast_group`
method.

Boto3 documentation:
[IoTWireless.Client.start_bulk_disassociate_wireless_device_from_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_bulk_disassociate_wireless_device_from_multicast_group)

Asynchronous method. Use
`await start_bulk_disassociate_wireless_device_from_multicast_group(...)` for a
synchronous call.

Arguments mapping described in
[StartBulkDisassociateWirelessDeviceFromMulticastGroupRequestRequestTypeDef](./type_defs.md#startbulkdisassociatewirelessdevicefrommulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `QueryString`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="start\_fuota\_task"></a>

### start_fuota_task

Starts a FUOTA task.

Type annotations for `session.create_client("iotwireless").start_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.start_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_fuota_task)

Asynchronous method. Use `await start_fuota_task(...)` for a synchronous call.

Arguments mapping described in
[StartFuotaTaskRequestRequestTypeDef](./type_defs.md#startfuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `LoRaWAN`:
  [LoRaWANStartFuotaTaskTypeDef](./type_defs.md#lorawanstartfuotatasktypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="start\_multicast\_group\_session"></a>

### start_multicast_group_session

Starts a multicast group session.

Type annotations for
`session.create_client("iotwireless").start_multicast_group_session` method.

Boto3 documentation:
[IoTWireless.Client.start_multicast_group_session](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.start_multicast_group_session)

Asynchronous method. Use `await start_multicast_group_session(...)` for a
synchronous call.

Arguments mapping described in
[StartMulticastGroupSessionRequestRequestTypeDef](./type_defs.md#startmulticastgroupsessionrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `LoRaWAN`:
  [LoRaWANMulticastSessionTypeDef](./type_defs.md#lorawanmulticastsessiontypedef)
  *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="tag\_resource"></a>

### tag_resource

Adds a tag to a resource.

Type annotations for `session.create_client("iotwireless").tag_resource`
method.

Boto3 documentation:
[IoTWireless.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="test\_wireless\_device"></a>

### test_wireless_device

Simulates a provisioned device by sending an uplink data payload of `Hello` .

Type annotations for
`session.create_client("iotwireless").test_wireless_device` method.

Boto3 documentation:
[IoTWireless.Client.test_wireless_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.test_wireless_device)

Asynchronous method. Use `await test_wireless_device(...)` for a synchronous
call.

Arguments mapping described in
[TestWirelessDeviceRequestRequestTypeDef](./type_defs.md#testwirelessdevicerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*

Returns a `Coroutine` for
[TestWirelessDeviceResponseTypeDef](./type_defs.md#testwirelessdeviceresponsetypedef).

<a id="untag\_resource"></a>

### untag_resource

Removes one or more tags from a resource.

Type annotations for `session.create_client("iotwireless").untag_resource`
method.

Boto3 documentation:
[IoTWireless.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_destination"></a>

### update_destination

Updates properties of a destination.

Type annotations for `session.create_client("iotwireless").update_destination`
method.

Boto3 documentation:
[IoTWireless.Client.update_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_destination)

Asynchronous method. Use `await update_destination(...)` for a synchronous
call.

Arguments mapping described in
[UpdateDestinationRequestRequestTypeDef](./type_defs.md#updatedestinationrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `ExpressionType`: [ExpressionTypeType](./literals.md#expressiontypetype)
- `Expression`: `str`
- `Description`: `str`
- `RoleArn`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_fuota\_task"></a>

### update_fuota_task

Updates properties of a FUOTA task.

Type annotations for `session.create_client("iotwireless").update_fuota_task`
method.

Boto3 documentation:
[IoTWireless.Client.update_fuota_task](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_fuota_task)

Asynchronous method. Use `await update_fuota_task(...)` for a synchronous call.

Arguments mapping described in
[UpdateFuotaTaskRequestRequestTypeDef](./type_defs.md#updatefuotataskrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `LoRaWAN`: [LoRaWANFuotaTaskTypeDef](./type_defs.md#lorawanfuotatasktypedef)
- `FirmwareUpdateImage`: `str`
- `FirmwareUpdateRole`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_log\_levels\_by\_resource\_types"></a>

### update_log_levels_by_resource_types

Set default log level, or log levels by resource types.

Type annotations for
`session.create_client("iotwireless").update_log_levels_by_resource_types`
method.

Boto3 documentation:
[IoTWireless.Client.update_log_levels_by_resource_types](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_log_levels_by_resource_types)

Asynchronous method. Use `await update_log_levels_by_resource_types(...)` for a
synchronous call.

Arguments mapping described in
[UpdateLogLevelsByResourceTypesRequestRequestTypeDef](./type_defs.md#updateloglevelsbyresourcetypesrequestrequesttypedef).

Keyword-only arguments:

- `DefaultLogLevel`: [LogLevelType](./literals.md#logleveltype)
- `WirelessDeviceLogOptions`:
  `Sequence`\[[WirelessDeviceLogOptionTypeDef](./type_defs.md#wirelessdevicelogoptiontypedef)\]
- `WirelessGatewayLogOptions`:
  `Sequence`\[[WirelessGatewayLogOptionTypeDef](./type_defs.md#wirelessgatewaylogoptiontypedef)\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_multicast\_group"></a>

### update_multicast_group

Updates properties of a multicast group session.

Type annotations for
`session.create_client("iotwireless").update_multicast_group` method.

Boto3 documentation:
[IoTWireless.Client.update_multicast_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_multicast_group)

Asynchronous method. Use `await update_multicast_group(...)` for a synchronous
call.

Arguments mapping described in
[UpdateMulticastGroupRequestRequestTypeDef](./type_defs.md#updatemulticastgrouprequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `LoRaWAN`: [LoRaWANMulticastTypeDef](./type_defs.md#lorawanmulticasttypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_network\_analyzer\_configuration"></a>

### update_network_analyzer_configuration

Update NetworkAnalyzer configuration.

Type annotations for
`session.create_client("iotwireless").update_network_analyzer_configuration`
method.

Boto3 documentation:
[IoTWireless.Client.update_network_analyzer_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_network_analyzer_configuration)

Asynchronous method. Use `await update_network_analyzer_configuration(...)` for
a synchronous call.

Arguments mapping described in
[UpdateNetworkAnalyzerConfigurationRequestRequestTypeDef](./type_defs.md#updatenetworkanalyzerconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `ConfigurationName`: `str` *(required)*
- `TraceContent`: [TraceContentTypeDef](./type_defs.md#tracecontenttypedef)
- `WirelessDevicesToAdd`: `Sequence`\[`str`\]
- `WirelessDevicesToRemove`: `Sequence`\[`str`\]
- `WirelessGatewaysToAdd`: `Sequence`\[`str`\]
- `WirelessGatewaysToRemove`: `Sequence`\[`str`\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_partner\_account"></a>

### update_partner_account

Updates properties of a partner account.

Type annotations for
`session.create_client("iotwireless").update_partner_account` method.

Boto3 documentation:
[IoTWireless.Client.update_partner_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_partner_account)

Asynchronous method. Use `await update_partner_account(...)` for a synchronous
call.

Arguments mapping described in
[UpdatePartnerAccountRequestRequestTypeDef](./type_defs.md#updatepartneraccountrequestrequesttypedef).

Keyword-only arguments:

- `Sidewalk`:
  [SidewalkUpdateAccountTypeDef](./type_defs.md#sidewalkupdateaccounttypedef)
  *(required)*
- `PartnerAccountId`: `str` *(required)*
- `PartnerType`: `Literal['Sidewalk']` (see
  [PartnerTypeType](./literals.md#partnertypetype)) *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_resource\_event\_configuration"></a>

### update_resource_event_configuration

Update the event configuration for a particular resource identifier.

Type annotations for
`session.create_client("iotwireless").update_resource_event_configuration`
method.

Boto3 documentation:
[IoTWireless.Client.update_resource_event_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_resource_event_configuration)

Asynchronous method. Use `await update_resource_event_configuration(...)` for a
synchronous call.

Arguments mapping described in
[UpdateResourceEventConfigurationRequestRequestTypeDef](./type_defs.md#updateresourceeventconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `Identifier`: `str` *(required)*
- `IdentifierType`: `Literal['PartnerAccountId']` (see
  [IdentifierTypeType](./literals.md#identifiertypetype)) *(required)*
- `PartnerType`: `Literal['Sidewalk']` (see
  [EventNotificationPartnerTypeType](./literals.md#eventnotificationpartnertypetype))
- `DeviceRegistrationState`:
  [DeviceRegistrationStateEventConfigurationTypeDef](./type_defs.md#deviceregistrationstateeventconfigurationtypedef)
- `Proximity`:
  [ProximityEventConfigurationTypeDef](./type_defs.md#proximityeventconfigurationtypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_wireless\_device"></a>

### update_wireless_device

Updates properties of a wireless device.

Type annotations for
`session.create_client("iotwireless").update_wireless_device` method.

Boto3 documentation:
[IoTWireless.Client.update_wireless_device](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_wireless_device)

Asynchronous method. Use `await update_wireless_device(...)` for a synchronous
call.

Arguments mapping described in
[UpdateWirelessDeviceRequestRequestTypeDef](./type_defs.md#updatewirelessdevicerequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `DestinationName`: `str`
- `Name`: `str`
- `Description`: `str`
- `LoRaWAN`:
  [LoRaWANUpdateDeviceTypeDef](./type_defs.md#lorawanupdatedevicetypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update\_wireless\_gateway"></a>

### update_wireless_gateway

Updates properties of a wireless gateway.

Type annotations for
`session.create_client("iotwireless").update_wireless_gateway` method.

Boto3 documentation:
[IoTWireless.Client.update_wireless_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.update_wireless_gateway)

Asynchronous method. Use `await update_wireless_gateway(...)` for a synchronous
call.

Arguments mapping described in
[UpdateWirelessGatewayRequestRequestTypeDef](./type_defs.md#updatewirelessgatewayrequestrequesttypedef).

Keyword-only arguments:

- `Id`: `str` *(required)*
- `Name`: `str`
- `Description`: `str`
- `JoinEuiFilters`: `Sequence`\[`Sequence`\[`str`\]\]
- `NetIdFilters`: `Sequence`\[`str`\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("iotwireless").__aenter__` method.

Boto3 documentation:
[IoTWireless.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [IoTWirelessClient](#iotwirelessclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("iotwireless").__aexit__` method.

Boto3 documentation:
[IoTWireless.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotwireless.html#IoTWireless.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

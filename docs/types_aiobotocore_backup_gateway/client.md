<a id="backupgatewayclient-for-aiobotocore-backupgateway-module"></a>

# BackupGatewayClient for aiobotocore BackupGateway module

> [Index](../README.md) > [BackupGateway](./README.md) > BackupGatewayClient

Auto-generated documentation for
[BackupGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
type annotations stubs module
[types-aiobotocore-backup-gateway](https://pypi.org/project/types-aiobotocore-backup-gateway/).

- [BackupGatewayClient for aiobotocore BackupGateway module](#backupgatewayclient-for-aiobotocore-backupgateway-module)
  - [BackupGatewayClient](#backupgatewayclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [associate_gateway_to_server](#associate_gateway_to_server)
    - [can_paginate](#can_paginate)
    - [create_gateway](#create_gateway)
    - [delete_gateway](#delete_gateway)
    - [delete_hypervisor](#delete_hypervisor)
    - [disassociate_gateway_from_server](#disassociate_gateway_from_server)
    - [generate_presigned_url](#generate_presigned_url)
    - [import_hypervisor_configuration](#import_hypervisor_configuration)
    - [list_gateways](#list_gateways)
    - [list_hypervisors](#list_hypervisors)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_virtual_machines](#list_virtual_machines)
    - [put_maintenance_start_time](#put_maintenance_start_time)
    - [tag_resource](#tag_resource)
    - [test_hypervisor_configuration](#test_hypervisor_configuration)
    - [untag_resource](#untag_resource)
    - [update_gateway_information](#update_gateway_information)
    - [update_hypervisor](#update_hypervisor)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="backupgatewayclient"></a>

## BackupGatewayClient

Type annotations for `session.create_client("backup-gateway")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_backup_gateway.client import BackupGatewayClient

session = get_session()
async with session.create_client("backup-gateway") as client:
    client: BackupGatewayClient
```

Boto3 documentation:
[BackupGateway.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_backup_gateway.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.ConflictException`
- `Exceptions.InternalServerException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

BackupGatewayClient exceptions.

Type annotations for `session.create_client("backup-gateway").exceptions`
method.

Boto3 documentation:
[BackupGateway.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="associate\_gateway\_to\_server"></a>

### associate_gateway_to_server

Associates a backup gateway with your server.

Type annotations for
`session.create_client("backup-gateway").associate_gateway_to_server` method.

Boto3 documentation:
[BackupGateway.Client.associate_gateway_to_server](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.associate_gateway_to_server)

Asynchronous method. Use `await associate_gateway_to_server(...)` for a
synchronous call.

Arguments mapping described in
[AssociateGatewayToServerInputRequestTypeDef](./type_defs.md#associategatewaytoserverinputrequesttypedef).

Keyword-only arguments:

- `GatewayArn`: `str` *(required)*
- `ServerArn`: `str` *(required)*

Returns a `Coroutine` for
[AssociateGatewayToServerOutputTypeDef](./type_defs.md#associategatewaytoserveroutputtypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("backup-gateway").can_paginate`
method.

Boto3 documentation:
[BackupGateway.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_gateway"></a>

### create_gateway

Creates a backup gateway.

Type annotations for `session.create_client("backup-gateway").create_gateway`
method.

Boto3 documentation:
[BackupGateway.Client.create_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.create_gateway)

Asynchronous method. Use `await create_gateway(...)` for a synchronous call.

Arguments mapping described in
[CreateGatewayInputRequestTypeDef](./type_defs.md#creategatewayinputrequesttypedef).

Keyword-only arguments:

- `ActivationKey`: `str` *(required)*
- `GatewayDisplayName`: `str` *(required)*
- `GatewayType`: `Literal['BACKUP_VM']` (see
  [GatewayTypeType](./literals.md#gatewaytypetype)) *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[CreateGatewayOutputTypeDef](./type_defs.md#creategatewayoutputtypedef).

<a id="delete\_gateway"></a>

### delete_gateway

Deletes a backup gateway.

Type annotations for `session.create_client("backup-gateway").delete_gateway`
method.

Boto3 documentation:
[BackupGateway.Client.delete_gateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.delete_gateway)

Asynchronous method. Use `await delete_gateway(...)` for a synchronous call.

Arguments mapping described in
[DeleteGatewayInputRequestTypeDef](./type_defs.md#deletegatewayinputrequesttypedef).

Keyword-only arguments:

- `GatewayArn`: `str` *(required)*

Returns a `Coroutine` for
[DeleteGatewayOutputTypeDef](./type_defs.md#deletegatewayoutputtypedef).

<a id="delete\_hypervisor"></a>

### delete_hypervisor

Deletes a hypervisor.

Type annotations for
`session.create_client("backup-gateway").delete_hypervisor` method.

Boto3 documentation:
[BackupGateway.Client.delete_hypervisor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.delete_hypervisor)

Asynchronous method. Use `await delete_hypervisor(...)` for a synchronous call.

Arguments mapping described in
[DeleteHypervisorInputRequestTypeDef](./type_defs.md#deletehypervisorinputrequesttypedef).

Keyword-only arguments:

- `HypervisorArn`: `str` *(required)*

Returns a `Coroutine` for
[DeleteHypervisorOutputTypeDef](./type_defs.md#deletehypervisoroutputtypedef).

<a id="disassociate\_gateway\_from\_server"></a>

### disassociate_gateway_from_server

Disassociates a backup gateway from the specified server.

Type annotations for
`session.create_client("backup-gateway").disassociate_gateway_from_server`
method.

Boto3 documentation:
[BackupGateway.Client.disassociate_gateway_from_server](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.disassociate_gateway_from_server)

Asynchronous method. Use `await disassociate_gateway_from_server(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateGatewayFromServerInputRequestTypeDef](./type_defs.md#disassociategatewayfromserverinputrequesttypedef).

Keyword-only arguments:

- `GatewayArn`: `str` *(required)*

Returns a `Coroutine` for
[DisassociateGatewayFromServerOutputTypeDef](./type_defs.md#disassociategatewayfromserveroutputtypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("backup-gateway").generate_presigned_url` method.

Boto3 documentation:
[BackupGateway.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="import\_hypervisor\_configuration"></a>

### import_hypervisor_configuration

Connect to a hypervisor by importing its configuration.

Type annotations for
`session.create_client("backup-gateway").import_hypervisor_configuration`
method.

Boto3 documentation:
[BackupGateway.Client.import_hypervisor_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.import_hypervisor_configuration)

Asynchronous method. Use `await import_hypervisor_configuration(...)` for a
synchronous call.

Arguments mapping described in
[ImportHypervisorConfigurationInputRequestTypeDef](./type_defs.md#importhypervisorconfigurationinputrequesttypedef).

Keyword-only arguments:

- `Host`: `str` *(required)*
- `Name`: `str` *(required)*
- `KmsKeyArn`: `str`
- `Password`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `Username`: `str`

Returns a `Coroutine` for
[ImportHypervisorConfigurationOutputTypeDef](./type_defs.md#importhypervisorconfigurationoutputtypedef).

<a id="list\_gateways"></a>

### list_gateways

Lists backup gateways owned by an Amazon Web Services account in an Amazon Web
Services Region.

Type annotations for `session.create_client("backup-gateway").list_gateways`
method.

Boto3 documentation:
[BackupGateway.Client.list_gateways](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_gateways)

Asynchronous method. Use `await list_gateways(...)` for a synchronous call.

Arguments mapping described in
[ListGatewaysInputRequestTypeDef](./type_defs.md#listgatewaysinputrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef).

<a id="list\_hypervisors"></a>

### list_hypervisors

Lists your hypervisors.

Type annotations for `session.create_client("backup-gateway").list_hypervisors`
method.

Boto3 documentation:
[BackupGateway.Client.list_hypervisors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_hypervisors)

Asynchronous method. Use `await list_hypervisors(...)` for a synchronous call.

Arguments mapping described in
[ListHypervisorsInputRequestTypeDef](./type_defs.md#listhypervisorsinputrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListHypervisorsOutputTypeDef](./type_defs.md#listhypervisorsoutputtypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

Lists the tags applied to the resource identified by its Amazon Resource Name
(ARN).

Type annotations for
`session.create_client("backup-gateway").list_tags_for_resource` method.

Boto3 documentation:
[BackupGateway.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef).

<a id="list\_virtual\_machines"></a>

### list_virtual_machines

Lists your virtual machines.

Type annotations for
`session.create_client("backup-gateway").list_virtual_machines` method.

Boto3 documentation:
[BackupGateway.Client.list_virtual_machines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.list_virtual_machines)

Asynchronous method. Use `await list_virtual_machines(...)` for a synchronous
call.

Arguments mapping described in
[ListVirtualMachinesInputRequestTypeDef](./type_defs.md#listvirtualmachinesinputrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListVirtualMachinesOutputTypeDef](./type_defs.md#listvirtualmachinesoutputtypedef).

<a id="put\_maintenance\_start\_time"></a>

### put_maintenance_start_time

Set the maintenance start time for a gateway.

Type annotations for
`session.create_client("backup-gateway").put_maintenance_start_time` method.

Boto3 documentation:
[BackupGateway.Client.put_maintenance_start_time](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.put_maintenance_start_time)

Asynchronous method. Use `await put_maintenance_start_time(...)` for a
synchronous call.

Arguments mapping described in
[PutMaintenanceStartTimeInputRequestTypeDef](./type_defs.md#putmaintenancestarttimeinputrequesttypedef).

Keyword-only arguments:

- `GatewayArn`: `str` *(required)*
- `HourOfDay`: `int` *(required)*
- `MinuteOfHour`: `int` *(required)*
- `DayOfMonth`: `int`
- `DayOfWeek`: `int`

Returns a `Coroutine` for
[PutMaintenanceStartTimeOutputTypeDef](./type_defs.md#putmaintenancestarttimeoutputtypedef).

<a id="tag\_resource"></a>

### tag_resource

Tag the resource.

Type annotations for `session.create_client("backup-gateway").tag_resource`
method.

Boto3 documentation:
[BackupGateway.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for
[TagResourceOutputTypeDef](./type_defs.md#tagresourceoutputtypedef).

<a id="test\_hypervisor\_configuration"></a>

### test_hypervisor_configuration

Tests your hypervisor configuration to validate that backup gateway can connect
with the hypervisor and its resources.

Type annotations for
`session.create_client("backup-gateway").test_hypervisor_configuration` method.

Boto3 documentation:
[BackupGateway.Client.test_hypervisor_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.test_hypervisor_configuration)

Asynchronous method. Use `await test_hypervisor_configuration(...)` for a
synchronous call.

Arguments mapping described in
[TestHypervisorConfigurationInputRequestTypeDef](./type_defs.md#testhypervisorconfigurationinputrequesttypedef).

Keyword-only arguments:

- `GatewayArn`: `str` *(required)*
- `Host`: `str` *(required)*
- `Password`: `str`
- `Username`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag\_resource"></a>

### untag_resource

Removes tags from the resource.

Type annotations for `session.create_client("backup-gateway").untag_resource`
method.

Boto3 documentation:
[BackupGateway.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef).

Keyword-only arguments:

- `ResourceARN`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[UntagResourceOutputTypeDef](./type_defs.md#untagresourceoutputtypedef).

<a id="update\_gateway\_information"></a>

### update_gateway_information

Updates a gateway's name.

Type annotations for
`session.create_client("backup-gateway").update_gateway_information` method.

Boto3 documentation:
[BackupGateway.Client.update_gateway_information](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.update_gateway_information)

Asynchronous method. Use `await update_gateway_information(...)` for a
synchronous call.

Arguments mapping described in
[UpdateGatewayInformationInputRequestTypeDef](./type_defs.md#updategatewayinformationinputrequesttypedef).

Keyword-only arguments:

- `GatewayArn`: `str` *(required)*
- `GatewayDisplayName`: `str`

Returns a `Coroutine` for
[UpdateGatewayInformationOutputTypeDef](./type_defs.md#updategatewayinformationoutputtypedef).

<a id="update\_hypervisor"></a>

### update_hypervisor

Updates a hypervisor metadata, including its host, username, and password.

Type annotations for
`session.create_client("backup-gateway").update_hypervisor` method.

Boto3 documentation:
[BackupGateway.Client.update_hypervisor](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.update_hypervisor)

Asynchronous method. Use `await update_hypervisor(...)` for a synchronous call.

Arguments mapping described in
[UpdateHypervisorInputRequestTypeDef](./type_defs.md#updatehypervisorinputrequesttypedef).

Keyword-only arguments:

- `HypervisorArn`: `str` *(required)*
- `Host`: `str`
- `Password`: `str`
- `Username`: `str`

Returns a `Coroutine` for
[UpdateHypervisorOutputTypeDef](./type_defs.md#updatehypervisoroutputtypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("backup-gateway").__aenter__`
method.

Boto3 documentation:
[BackupGateway.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [BackupGatewayClient](#backupgatewayclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("backup-gateway").__aexit__`
method.

Boto3 documentation:
[BackupGateway.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("backup-gateway").get_paginator`
method with overloads.

- `client.get_paginator("list_gateways")` ->
  [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
- `client.get_paginator("list_hypervisors")` ->
  [ListHypervisorsPaginator](./paginators.md#listhypervisorspaginator)
- `client.get_paginator("list_virtual_machines")` ->
  [ListVirtualMachinesPaginator](./paginators.md#listvirtualmachinespaginator)

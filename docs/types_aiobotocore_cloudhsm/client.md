<a id="cloudhsmclient-for-aiobotocore-cloudhsm-module"></a>

# CloudHSMClient for aiobotocore CloudHSM module

> [Index](../README.md) > [CloudHSM](./README.md) > CloudHSMClient

Auto-generated documentation for
[CloudHSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
type annotations stubs module
[types-aiobotocore-cloudhsm](https://pypi.org/project/types-aiobotocore-cloudhsm/).

- [CloudHSMClient for aiobotocore CloudHSM module](#cloudhsmclient-for-aiobotocore-cloudhsm-module)
  - [CloudHSMClient](#cloudhsmclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_tags_to_resource](#add_tags_to_resource)
    - [can_paginate](#can_paginate)
    - [create_hapg](#create_hapg)
    - [create_hsm](#create_hsm)
    - [create_luna_client](#create_luna_client)
    - [delete_hapg](#delete_hapg)
    - [delete_hsm](#delete_hsm)
    - [delete_luna_client](#delete_luna_client)
    - [describe_hapg](#describe_hapg)
    - [describe_hsm](#describe_hsm)
    - [describe_luna_client](#describe_luna_client)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_config](#get_config)
    - [list_available_zones](#list_available_zones)
    - [list_hapgs](#list_hapgs)
    - [list_hsms](#list_hsms)
    - [list_luna_clients](#list_luna_clients)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [modify_hapg](#modify_hapg)
    - [modify_hsm](#modify_hsm)
    - [modify_luna_client](#modify_luna_client)
    - [remove_tags_from_resource](#remove_tags_from_resource)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="cloudhsmclient"></a>

## CloudHSMClient

Type annotations for `session.create_client("cloudhsm")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_cloudhsm.client import CloudHSMClient

session = get_session()
async with session.create_client("cloudhsm") as client:
    client: CloudHSMClient
```

Boto3 documentation:
[CloudHSM.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cloudhsm.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.CloudHsmInternalException`
- `Exceptions.CloudHsmServiceException`
- `Exceptions.InvalidRequestException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CloudHSMClient exceptions.

Type annotations for `session.create_client("cloudhsm").exceptions` method.

Boto3 documentation:
[CloudHSM.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add\_tags\_to\_resource"></a>

### add_tags_to_resource

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").add_tags_to_resource`
method.

Boto3 documentation:
[CloudHSM.Client.add_tags_to_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.add_tags_to_resource)

Asynchronous method. Use `await add_tags_to_resource(...)` for a synchronous
call.

Arguments mapping described in
[AddTagsToResourceRequestRequestTypeDef](./type_defs.md#addtagstoresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagList`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\] *(required)*

Returns a `Coroutine` for
[AddTagsToResourceResponseTypeDef](./type_defs.md#addtagstoresourceresponsetypedef).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("cloudhsm").can_paginate` method.

Boto3 documentation:
[CloudHSM.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create\_hapg"></a>

### create_hapg

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").create_hapg` method.

Boto3 documentation:
[CloudHSM.Client.create_hapg](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.create_hapg)

Asynchronous method. Use `await create_hapg(...)` for a synchronous call.

Arguments mapping described in
[CreateHapgRequestRequestTypeDef](./type_defs.md#createhapgrequestrequesttypedef).

Keyword-only arguments:

- `Label`: `str` *(required)*

Returns a `Coroutine` for
[CreateHapgResponseTypeDef](./type_defs.md#createhapgresponsetypedef).

<a id="create\_hsm"></a>

### create_hsm

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").create_hsm` method.

Boto3 documentation:
[CloudHSM.Client.create_hsm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.create_hsm)

Asynchronous method. Use `await create_hsm(...)` for a synchronous call.

Arguments mapping described in
[CreateHsmRequestRequestTypeDef](./type_defs.md#createhsmrequestrequesttypedef).

Keyword-only arguments:

- `SubnetId`: `str` *(required)*
- `SshKey`: `str` *(required)*
- `IamRoleArn`: `str` *(required)*
- `SubscriptionType`: `Literal['PRODUCTION']` (see
  [SubscriptionTypeType](./literals.md#subscriptiontypetype)) *(required)*
- `EniIp`: `str`
- `ExternalId`: `str`
- `ClientToken`: `str`
- `SyslogIp`: `str`

Returns a `Coroutine` for
[CreateHsmResponseTypeDef](./type_defs.md#createhsmresponsetypedef).

<a id="create\_luna\_client"></a>

### create_luna_client

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").create_luna_client`
method.

Boto3 documentation:
[CloudHSM.Client.create_luna_client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.create_luna_client)

Asynchronous method. Use `await create_luna_client(...)` for a synchronous
call.

Arguments mapping described in
[CreateLunaClientRequestRequestTypeDef](./type_defs.md#createlunaclientrequestrequesttypedef).

Keyword-only arguments:

- `Certificate`: `str` *(required)*
- `Label`: `str`

Returns a `Coroutine` for
[CreateLunaClientResponseTypeDef](./type_defs.md#createlunaclientresponsetypedef).

<a id="delete\_hapg"></a>

### delete_hapg

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").delete_hapg` method.

Boto3 documentation:
[CloudHSM.Client.delete_hapg](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.delete_hapg)

Asynchronous method. Use `await delete_hapg(...)` for a synchronous call.

Arguments mapping described in
[DeleteHapgRequestRequestTypeDef](./type_defs.md#deletehapgrequestrequesttypedef).

Keyword-only arguments:

- `HapgArn`: `str` *(required)*

Returns a `Coroutine` for
[DeleteHapgResponseTypeDef](./type_defs.md#deletehapgresponsetypedef).

<a id="delete\_hsm"></a>

### delete_hsm

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").delete_hsm` method.

Boto3 documentation:
[CloudHSM.Client.delete_hsm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.delete_hsm)

Asynchronous method. Use `await delete_hsm(...)` for a synchronous call.

Arguments mapping described in
[DeleteHsmRequestRequestTypeDef](./type_defs.md#deletehsmrequestrequesttypedef).

Keyword-only arguments:

- `HsmArn`: `str` *(required)*

Returns a `Coroutine` for
[DeleteHsmResponseTypeDef](./type_defs.md#deletehsmresponsetypedef).

<a id="delete\_luna\_client"></a>

### delete_luna_client

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").delete_luna_client`
method.

Boto3 documentation:
[CloudHSM.Client.delete_luna_client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.delete_luna_client)

Asynchronous method. Use `await delete_luna_client(...)` for a synchronous
call.

Arguments mapping described in
[DeleteLunaClientRequestRequestTypeDef](./type_defs.md#deletelunaclientrequestrequesttypedef).

Keyword-only arguments:

- `ClientArn`: `str` *(required)*

Returns a `Coroutine` for
[DeleteLunaClientResponseTypeDef](./type_defs.md#deletelunaclientresponsetypedef).

<a id="describe\_hapg"></a>

### describe_hapg

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").describe_hapg` method.

Boto3 documentation:
[CloudHSM.Client.describe_hapg](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.describe_hapg)

Asynchronous method. Use `await describe_hapg(...)` for a synchronous call.

Arguments mapping described in
[DescribeHapgRequestRequestTypeDef](./type_defs.md#describehapgrequestrequesttypedef).

Keyword-only arguments:

- `HapgArn`: `str` *(required)*

Returns a `Coroutine` for
[DescribeHapgResponseTypeDef](./type_defs.md#describehapgresponsetypedef).

<a id="describe\_hsm"></a>

### describe_hsm

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").describe_hsm` method.

Boto3 documentation:
[CloudHSM.Client.describe_hsm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.describe_hsm)

Asynchronous method. Use `await describe_hsm(...)` for a synchronous call.

Arguments mapping described in
[DescribeHsmRequestRequestTypeDef](./type_defs.md#describehsmrequestrequesttypedef).

Keyword-only arguments:

- `HsmArn`: `str`
- `HsmSerialNumber`: `str`

Returns a `Coroutine` for
[DescribeHsmResponseTypeDef](./type_defs.md#describehsmresponsetypedef).

<a id="describe\_luna\_client"></a>

### describe_luna_client

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").describe_luna_client`
method.

Boto3 documentation:
[CloudHSM.Client.describe_luna_client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.describe_luna_client)

Asynchronous method. Use `await describe_luna_client(...)` for a synchronous
call.

Arguments mapping described in
[DescribeLunaClientRequestRequestTypeDef](./type_defs.md#describelunaclientrequestrequesttypedef).

Keyword-only arguments:

- `ClientArn`: `str`
- `CertificateFingerprint`: `str`

Returns a `Coroutine` for
[DescribeLunaClientResponseTypeDef](./type_defs.md#describelunaclientresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("cloudhsm").generate_presigned_url`
method.

Boto3 documentation:
[CloudHSM.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_config"></a>

### get_config

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").get_config` method.

Boto3 documentation:
[CloudHSM.Client.get_config](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.get_config)

Asynchronous method. Use `await get_config(...)` for a synchronous call.

Arguments mapping described in
[GetConfigRequestRequestTypeDef](./type_defs.md#getconfigrequestrequesttypedef).

Keyword-only arguments:

- `ClientArn`: `str` *(required)*
- `ClientVersion`: [ClientVersionType](./literals.md#clientversiontype)
  *(required)*
- `HapgList`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[GetConfigResponseTypeDef](./type_defs.md#getconfigresponsetypedef).

<a id="list\_available\_zones"></a>

### list_available_zones

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").list_available_zones`
method.

Boto3 documentation:
[CloudHSM.Client.list_available_zones](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_available_zones)

Asynchronous method. Use `await list_available_zones(...)` for a synchronous
call.

Returns a `Coroutine` for
[ListAvailableZonesResponseTypeDef](./type_defs.md#listavailablezonesresponsetypedef).

<a id="list\_hapgs"></a>

### list_hapgs

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").list_hapgs` method.

Boto3 documentation:
[CloudHSM.Client.list_hapgs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_hapgs)

Asynchronous method. Use `await list_hapgs(...)` for a synchronous call.

Arguments mapping described in
[ListHapgsRequestRequestTypeDef](./type_defs.md#listhapgsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`

Returns a `Coroutine` for
[ListHapgsResponseTypeDef](./type_defs.md#listhapgsresponsetypedef).

<a id="list\_hsms"></a>

### list_hsms

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").list_hsms` method.

Boto3 documentation:
[CloudHSM.Client.list_hsms](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_hsms)

Asynchronous method. Use `await list_hsms(...)` for a synchronous call.

Arguments mapping described in
[ListHsmsRequestRequestTypeDef](./type_defs.md#listhsmsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`

Returns a `Coroutine` for
[ListHsmsResponseTypeDef](./type_defs.md#listhsmsresponsetypedef).

<a id="list\_luna\_clients"></a>

### list_luna_clients

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").list_luna_clients`
method.

Boto3 documentation:
[CloudHSM.Client.list_luna_clients](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_luna_clients)

Asynchronous method. Use `await list_luna_clients(...)` for a synchronous call.

Arguments mapping described in
[ListLunaClientsRequestRequestTypeDef](./type_defs.md#listlunaclientsrequestrequesttypedef).

Keyword-only arguments:

- `NextToken`: `str`

Returns a `Coroutine` for
[ListLunaClientsResponseTypeDef](./type_defs.md#listlunaclientsresponsetypedef).

<a id="list\_tags\_for\_resource"></a>

### list_tags_for_resource

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").list_tags_for_resource`
method.

Boto3 documentation:
[CloudHSM.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="modify\_hapg"></a>

### modify_hapg

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").modify_hapg` method.

Boto3 documentation:
[CloudHSM.Client.modify_hapg](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.modify_hapg)

Asynchronous method. Use `await modify_hapg(...)` for a synchronous call.

Arguments mapping described in
[ModifyHapgRequestRequestTypeDef](./type_defs.md#modifyhapgrequestrequesttypedef).

Keyword-only arguments:

- `HapgArn`: `str` *(required)*
- `Label`: `str`
- `PartitionSerialList`: `Sequence`\[`str`\]

Returns a `Coroutine` for
[ModifyHapgResponseTypeDef](./type_defs.md#modifyhapgresponsetypedef).

<a id="modify\_hsm"></a>

### modify_hsm

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").modify_hsm` method.

Boto3 documentation:
[CloudHSM.Client.modify_hsm](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.modify_hsm)

Asynchronous method. Use `await modify_hsm(...)` for a synchronous call.

Arguments mapping described in
[ModifyHsmRequestRequestTypeDef](./type_defs.md#modifyhsmrequestrequesttypedef).

Keyword-only arguments:

- `HsmArn`: `str` *(required)*
- `SubnetId`: `str`
- `EniIp`: `str`
- `IamRoleArn`: `str`
- `ExternalId`: `str`
- `SyslogIp`: `str`

Returns a `Coroutine` for
[ModifyHsmResponseTypeDef](./type_defs.md#modifyhsmresponsetypedef).

<a id="modify\_luna\_client"></a>

### modify_luna_client

This is documentation for **AWS CloudHSM Classic**.

Type annotations for `session.create_client("cloudhsm").modify_luna_client`
method.

Boto3 documentation:
[CloudHSM.Client.modify_luna_client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.modify_luna_client)

Asynchronous method. Use `await modify_luna_client(...)` for a synchronous
call.

Arguments mapping described in
[ModifyLunaClientRequestRequestTypeDef](./type_defs.md#modifylunaclientrequestrequesttypedef).

Keyword-only arguments:

- `ClientArn`: `str` *(required)*
- `Certificate`: `str` *(required)*

Returns a `Coroutine` for
[ModifyLunaClientResponseTypeDef](./type_defs.md#modifylunaclientresponsetypedef).

<a id="remove\_tags\_from\_resource"></a>

### remove_tags_from_resource

This is documentation for **AWS CloudHSM Classic**.

Type annotations for
`session.create_client("cloudhsm").remove_tags_from_resource` method.

Boto3 documentation:
[CloudHSM.Client.remove_tags_from_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.remove_tags_from_resource)

Asynchronous method. Use `await remove_tags_from_resource(...)` for a
synchronous call.

Arguments mapping described in
[RemoveTagsFromResourceRequestRequestTypeDef](./type_defs.md#removetagsfromresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeyList`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[RemoveTagsFromResourceResponseTypeDef](./type_defs.md#removetagsfromresourceresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("cloudhsm").__aenter__` method.

Boto3 documentation:
[CloudHSM.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CloudHSMClient](#cloudhsmclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("cloudhsm").__aexit__` method.

Boto3 documentation:
[CloudHSM.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("cloudhsm").get_paginator` method
with overloads.

- `client.get_paginator("list_hapgs")` ->
  [ListHapgsPaginator](./paginators.md#listhapgspaginator)
- `client.get_paginator("list_hsms")` ->
  [ListHsmsPaginator](./paginators.md#listhsmspaginator)
- `client.get_paginator("list_luna_clients")` ->
  [ListLunaClientsPaginator](./paginators.md#listlunaclientspaginator)

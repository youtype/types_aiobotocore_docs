<a id="route53recoveryreadinessclient-for-aiobotocore-route53recoveryreadiness-module"></a>

# Route53RecoveryReadinessClient for aiobotocore Route53RecoveryReadiness module

> [Index](..) > [Route53RecoveryReadiness](.) > Route53RecoveryReadinessClient

Auto-generated documentation for
[Route53RecoveryReadiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
type annotations stubs module
[types-aiobotocore-route53-recovery-readiness](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness/).

- [Route53RecoveryReadinessClient for aiobotocore Route53RecoveryReadiness module](#route53recoveryreadinessclient-for-aiobotocore-route53recoveryreadiness-module)
  - [Route53RecoveryReadinessClient](#route53recoveryreadinessclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [create_cell](#create_cell)
    - [create_cross_account_authorization](#create_cross_account_authorization)
    - [create_readiness_check](#create_readiness_check)
    - [create_recovery_group](#create_recovery_group)
    - [create_resource_set](#create_resource_set)
    - [delete_cell](#delete_cell)
    - [delete_cross_account_authorization](#delete_cross_account_authorization)
    - [delete_readiness_check](#delete_readiness_check)
    - [delete_recovery_group](#delete_recovery_group)
    - [delete_resource_set](#delete_resource_set)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_architecture_recommendations](#get_architecture_recommendations)
    - [get_cell](#get_cell)
    - [get_cell_readiness_summary](#get_cell_readiness_summary)
    - [get_readiness_check](#get_readiness_check)
    - [get_readiness_check_resource_status](#get_readiness_check_resource_status)
    - [get_readiness_check_status](#get_readiness_check_status)
    - [get_recovery_group](#get_recovery_group)
    - [get_recovery_group_readiness_summary](#get_recovery_group_readiness_summary)
    - [get_resource_set](#get_resource_set)
    - [list_cells](#list_cells)
    - [list_cross_account_authorizations](#list_cross_account_authorizations)
    - [list_readiness_checks](#list_readiness_checks)
    - [list_recovery_groups](#list_recovery_groups)
    - [list_resource_sets](#list_resource_sets)
    - [list_rules](#list_rules)
    - [list_tags_for_resources](#list_tags_for_resources)
    - [tag_resource](#tag_resource)
    - [untag_resource](#untag_resource)
    - [update_cell](#update_cell)
    - [update_readiness_check](#update_readiness_check)
    - [update_recovery_group](#update_recovery_group)
    - [update_resource_set](#update_resource_set)
    - [get_paginator](#get_paginator)

<a id="route53recoveryreadinessclient"></a>

## Route53RecoveryReadinessClient

Type annotations for `aiobotocore.create_client("route53-recovery-readiness")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_route53_recovery_readiness.client import Route53RecoveryReadinessClient

def get_route53-recovery-readiness_client() -> Route53RecoveryReadinessClient:
    return Session().client("route53-recovery-readiness")
```

Boto3 documentation:
[Route53RecoveryReadiness.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_route53_recovery_readiness.client import Exceptions

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
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

Route53RecoveryReadinessClient exceptions.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").exceptions` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").can_paginate` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_cell"></a>

### create_cell

Creates a new Cell.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").create_cell` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.create_cell](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_cell)

Asynchronous method. Use `await create_cell(...)` for a synchronous call.

Arguments mapping described in
[CreateCellRequestRequestTypeDef](./type_defs.md#createcellrequestrequesttypedef).

Keyword-only arguments:

- `CellName`: `str` *(required)*
- `Cells`: `Sequence`\[`str`\]
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateCellResponseTypeDef](./type_defs.md#createcellresponsetypedef).

<a id="create_cross_account_authorization"></a>

### create_cross_account_authorization

Create a new cross account readiness authorization.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").create_cross_account_authorization`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.create_cross_account_authorization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_cross_account_authorization)

Asynchronous method. Use `await create_cross_account_authorization(...)` for a
synchronous call.

Arguments mapping described in
[CreateCrossAccountAuthorizationRequestRequestTypeDef](./type_defs.md#createcrossaccountauthorizationrequestrequesttypedef).

Keyword-only arguments:

- `CrossAccountAuthorization`: `str` *(required)*

Returns a `Coroutine` for
[CreateCrossAccountAuthorizationResponseTypeDef](./type_defs.md#createcrossaccountauthorizationresponsetypedef).

<a id="create_readiness_check"></a>

### create_readiness_check

Creates a new Readiness Check.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").create_readiness_check`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.create_readiness_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_readiness_check)

Asynchronous method. Use `await create_readiness_check(...)` for a synchronous
call.

Arguments mapping described in
[CreateReadinessCheckRequestRequestTypeDef](./type_defs.md#createreadinesscheckrequestrequesttypedef).

Keyword-only arguments:

- `ReadinessCheckName`: `str` *(required)*
- `ResourceSetName`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateReadinessCheckResponseTypeDef](./type_defs.md#createreadinesscheckresponsetypedef).

<a id="create_recovery_group"></a>

### create_recovery_group

Creates a new Recovery Group.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").create_recovery_group`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.create_recovery_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_recovery_group)

Asynchronous method. Use `await create_recovery_group(...)` for a synchronous
call.

Arguments mapping described in
[CreateRecoveryGroupRequestRequestTypeDef](./type_defs.md#createrecoverygrouprequestrequesttypedef).

Keyword-only arguments:

- `RecoveryGroupName`: `str` *(required)*
- `Cells`: `Sequence`\[`str`\]
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateRecoveryGroupResponseTypeDef](./type_defs.md#createrecoverygroupresponsetypedef).

<a id="create_resource_set"></a>

### create_resource_set

Creates a new Resource Set.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").create_resource_set`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.create_resource_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.create_resource_set)

Asynchronous method. Use `await create_resource_set(...)` for a synchronous
call.

Arguments mapping described in
[CreateResourceSetRequestRequestTypeDef](./type_defs.md#createresourcesetrequestrequesttypedef).

Keyword-only arguments:

- `ResourceSetName`: `str` *(required)*
- `ResourceSetType`: `str` *(required)*
- `Resources`: `Sequence`\[[ResourceTypeDef](./type_defs.md#resourcetypedef)\]
  *(required)*
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateResourceSetResponseTypeDef](./type_defs.md#createresourcesetresponsetypedef).

<a id="delete_cell"></a>

### delete_cell

Deletes an existing Cell.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").delete_cell` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.delete_cell](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.delete_cell)

Asynchronous method. Use `await delete_cell(...)` for a synchronous call.

Arguments mapping described in
[DeleteCellRequestRequestTypeDef](./type_defs.md#deletecellrequestrequesttypedef).

Keyword-only arguments:

- `CellName`: `str` *(required)*

<a id="delete_cross_account_authorization"></a>

### delete_cross_account_authorization

Delete cross account readiness authorization See also: \[AWS API
Documentation\](https://docs.aws.amazon.com/goto/WebAPI/route53-recovery-
readiness-2019-12-02/DeleteCrossAccountAuthorization).

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").delete_cross_account_authorization`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.delete_cross_account_authorization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.delete_cross_account_authorization)

Asynchronous method. Use `await delete_cross_account_authorization(...)` for a
synchronous call.

Arguments mapping described in
[DeleteCrossAccountAuthorizationRequestRequestTypeDef](./type_defs.md#deletecrossaccountauthorizationrequestrequesttypedef).

Keyword-only arguments:

- `CrossAccountAuthorization`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_readiness_check"></a>

### delete_readiness_check

Deletes an existing Readiness Check.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").delete_readiness_check`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.delete_readiness_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.delete_readiness_check)

Asynchronous method. Use `await delete_readiness_check(...)` for a synchronous
call.

Arguments mapping described in
[DeleteReadinessCheckRequestRequestTypeDef](./type_defs.md#deletereadinesscheckrequestrequesttypedef).

Keyword-only arguments:

- `ReadinessCheckName`: `str` *(required)*

<a id="delete_recovery_group"></a>

### delete_recovery_group

Deletes an existing Recovery Group.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").delete_recovery_group`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.delete_recovery_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.delete_recovery_group)

Asynchronous method. Use `await delete_recovery_group(...)` for a synchronous
call.

Arguments mapping described in
[DeleteRecoveryGroupRequestRequestTypeDef](./type_defs.md#deleterecoverygrouprequestrequesttypedef).

Keyword-only arguments:

- `RecoveryGroupName`: `str` *(required)*

<a id="delete_resource_set"></a>

### delete_resource_set

Deletes an existing Resource Set.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").delete_resource_set`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.delete_resource_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.delete_resource_set)

Asynchronous method. Use `await delete_resource_set(...)` for a synchronous
call.

Arguments mapping described in
[DeleteResourceSetRequestRequestTypeDef](./type_defs.md#deleteresourcesetrequestrequesttypedef).

Keyword-only arguments:

- `ResourceSetName`: `str` *(required)*

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").generate_presigned_url`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_architecture_recommendations"></a>

### get_architecture_recommendations

Returns a collection of recommendations to improve resilliance and readiness
check quality for a Recovery Group.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_architecture_recommendations`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_architecture_recommendations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_architecture_recommendations)

Asynchronous method. Use `await get_architecture_recommendations(...)` for a
synchronous call.

Arguments mapping described in
[GetArchitectureRecommendationsRequestRequestTypeDef](./type_defs.md#getarchitecturerecommendationsrequestrequesttypedef).

Keyword-only arguments:

- `RecoveryGroupName`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[GetArchitectureRecommendationsResponseTypeDef](./type_defs.md#getarchitecturerecommendationsresponsetypedef).

<a id="get_cell"></a>

### get_cell

Returns information about a Cell.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_cell` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_cell](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_cell)

Asynchronous method. Use `await get_cell(...)` for a synchronous call.

Arguments mapping described in
[GetCellRequestRequestTypeDef](./type_defs.md#getcellrequestrequesttypedef).

Keyword-only arguments:

- `CellName`: `str` *(required)*

Returns a `Coroutine` for
[GetCellResponseTypeDef](./type_defs.md#getcellresponsetypedef).

<a id="get_cell_readiness_summary"></a>

### get_cell_readiness_summary

Returns information about readiness of a Cell.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_cell_readiness_summary`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_cell_readiness_summary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_cell_readiness_summary)

Asynchronous method. Use `await get_cell_readiness_summary(...)` for a
synchronous call.

Arguments mapping described in
[GetCellReadinessSummaryRequestRequestTypeDef](./type_defs.md#getcellreadinesssummaryrequestrequesttypedef).

Keyword-only arguments:

- `CellName`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[GetCellReadinessSummaryResponseTypeDef](./type_defs.md#getcellreadinesssummaryresponsetypedef).

<a id="get_readiness_check"></a>

### get_readiness_check

Returns information about a ReadinessCheck.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_readiness_check`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_readiness_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_readiness_check)

Asynchronous method. Use `await get_readiness_check(...)` for a synchronous
call.

Arguments mapping described in
[GetReadinessCheckRequestRequestTypeDef](./type_defs.md#getreadinesscheckrequestrequesttypedef).

Keyword-only arguments:

- `ReadinessCheckName`: `str` *(required)*

Returns a `Coroutine` for
[GetReadinessCheckResponseTypeDef](./type_defs.md#getreadinesscheckresponsetypedef).

<a id="get_readiness_check_resource_status"></a>

### get_readiness_check_resource_status

Returns detailed information about the status of an individual resource within
a Readiness Check's Resource Set.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_readiness_check_resource_status`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_readiness_check_resource_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_readiness_check_resource_status)

Asynchronous method. Use `await get_readiness_check_resource_status(...)` for a
synchronous call.

Arguments mapping described in
[GetReadinessCheckResourceStatusRequestRequestTypeDef](./type_defs.md#getreadinesscheckresourcestatusrequestrequesttypedef).

Keyword-only arguments:

- `ReadinessCheckName`: `str` *(required)*
- `ResourceIdentifier`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[GetReadinessCheckResourceStatusResponseTypeDef](./type_defs.md#getreadinesscheckresourcestatusresponsetypedef).

<a id="get_readiness_check_status"></a>

### get_readiness_check_status

Returns information about the status of a Readiness Check.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_readiness_check_status`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_readiness_check_status](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_readiness_check_status)

Asynchronous method. Use `await get_readiness_check_status(...)` for a
synchronous call.

Arguments mapping described in
[GetReadinessCheckStatusRequestRequestTypeDef](./type_defs.md#getreadinesscheckstatusrequestrequesttypedef).

Keyword-only arguments:

- `ReadinessCheckName`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[GetReadinessCheckStatusResponseTypeDef](./type_defs.md#getreadinesscheckstatusresponsetypedef).

<a id="get_recovery_group"></a>

### get_recovery_group

Returns information about a Recovery Group.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_recovery_group`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_recovery_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_recovery_group)

Asynchronous method. Use `await get_recovery_group(...)` for a synchronous
call.

Arguments mapping described in
[GetRecoveryGroupRequestRequestTypeDef](./type_defs.md#getrecoverygrouprequestrequesttypedef).

Keyword-only arguments:

- `RecoveryGroupName`: `str` *(required)*

Returns a `Coroutine` for
[GetRecoveryGroupResponseTypeDef](./type_defs.md#getrecoverygroupresponsetypedef).

<a id="get_recovery_group_readiness_summary"></a>

### get_recovery_group_readiness_summary

Returns information about a Recovery Group.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_recovery_group_readiness_summary`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_recovery_group_readiness_summary](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_recovery_group_readiness_summary)

Asynchronous method. Use `await get_recovery_group_readiness_summary(...)` for
a synchronous call.

Arguments mapping described in
[GetRecoveryGroupReadinessSummaryRequestRequestTypeDef](./type_defs.md#getrecoverygroupreadinesssummaryrequestrequesttypedef).

Keyword-only arguments:

- `RecoveryGroupName`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[GetRecoveryGroupReadinessSummaryResponseTypeDef](./type_defs.md#getrecoverygroupreadinesssummaryresponsetypedef).

<a id="get_resource_set"></a>

### get_resource_set

Returns information about a Resource Set.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_resource_set`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.get_resource_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.get_resource_set)

Asynchronous method. Use `await get_resource_set(...)` for a synchronous call.

Arguments mapping described in
[GetResourceSetRequestRequestTypeDef](./type_defs.md#getresourcesetrequestrequesttypedef).

Keyword-only arguments:

- `ResourceSetName`: `str` *(required)*

Returns a `Coroutine` for
[GetResourceSetResponseTypeDef](./type_defs.md#getresourcesetresponsetypedef).

<a id="list_cells"></a>

### list_cells

Returns a collection of Cells.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").list_cells` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.list_cells](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.list_cells)

Asynchronous method. Use `await list_cells(...)` for a synchronous call.

Arguments mapping described in
[ListCellsRequestRequestTypeDef](./type_defs.md#listcellsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListCellsResponseTypeDef](./type_defs.md#listcellsresponsetypedef).

<a id="list_cross_account_authorizations"></a>

### list_cross_account_authorizations

Returns a collection of cross account readiness authorizations.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").list_cross_account_authorizations`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.list_cross_account_authorizations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.list_cross_account_authorizations)

Asynchronous method. Use `await list_cross_account_authorizations(...)` for a
synchronous call.

Arguments mapping described in
[ListCrossAccountAuthorizationsRequestRequestTypeDef](./type_defs.md#listcrossaccountauthorizationsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListCrossAccountAuthorizationsResponseTypeDef](./type_defs.md#listcrossaccountauthorizationsresponsetypedef).

<a id="list_readiness_checks"></a>

### list_readiness_checks

Returns a collection of Readiness Checks.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").list_readiness_checks`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.list_readiness_checks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.list_readiness_checks)

Asynchronous method. Use `await list_readiness_checks(...)` for a synchronous
call.

Arguments mapping described in
[ListReadinessChecksRequestRequestTypeDef](./type_defs.md#listreadinesschecksrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListReadinessChecksResponseTypeDef](./type_defs.md#listreadinesschecksresponsetypedef).

<a id="list_recovery_groups"></a>

### list_recovery_groups

Returns a collection of Recovery Groups.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").list_recovery_groups`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.list_recovery_groups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.list_recovery_groups)

Asynchronous method. Use `await list_recovery_groups(...)` for a synchronous
call.

Arguments mapping described in
[ListRecoveryGroupsRequestRequestTypeDef](./type_defs.md#listrecoverygroupsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListRecoveryGroupsResponseTypeDef](./type_defs.md#listrecoverygroupsresponsetypedef).

<a id="list_resource_sets"></a>

### list_resource_sets

Returns a collection of Resource Sets.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").list_resource_sets`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.list_resource_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.list_resource_sets)

Asynchronous method. Use `await list_resource_sets(...)` for a synchronous
call.

Arguments mapping described in
[ListResourceSetsRequestRequestTypeDef](./type_defs.md#listresourcesetsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListResourceSetsResponseTypeDef](./type_defs.md#listresourcesetsresponsetypedef).

<a id="list_rules"></a>

### list_rules

Returns a collection of rules that are applied as part of Readiness Checks.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").list_rules` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.list_rules](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.list_rules)

Asynchronous method. Use `await list_rules(...)` for a synchronous call.

Arguments mapping described in
[ListRulesRequestRequestTypeDef](./type_defs.md#listrulesrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`
- `ResourceType`: `str`

Returns a `Coroutine` for
[ListRulesResponseTypeDef](./type_defs.md#listrulesresponsetypedef).

<a id="list_tags_for_resources"></a>

### list_tags_for_resources

Returns a list of the tags assigned to the specified resource.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").list_tags_for_resources`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.list_tags_for_resources](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.list_tags_for_resources)

Asynchronous method. Use `await list_tags_for_resources(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourcesRequestRequestTypeDef](./type_defs.md#listtagsforresourcesrequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourcesResponseTypeDef](./type_defs.md#listtagsforresourcesresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds tags to the specified resource.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").tag_resource` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes tags from the specified resource.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").untag_resource`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

<a id="update_cell"></a>

### update_cell

Updates an existing Cell.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").update_cell` method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.update_cell](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_cell)

Asynchronous method. Use `await update_cell(...)` for a synchronous call.

Arguments mapping described in
[UpdateCellRequestRequestTypeDef](./type_defs.md#updatecellrequestrequesttypedef).

Keyword-only arguments:

- `CellName`: `str` *(required)*
- `Cells`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[UpdateCellResponseTypeDef](./type_defs.md#updatecellresponsetypedef).

<a id="update_readiness_check"></a>

### update_readiness_check

Updates an exisiting Readiness Check.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").update_readiness_check`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.update_readiness_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_readiness_check)

Asynchronous method. Use `await update_readiness_check(...)` for a synchronous
call.

Arguments mapping described in
[UpdateReadinessCheckRequestRequestTypeDef](./type_defs.md#updatereadinesscheckrequestrequesttypedef).

Keyword-only arguments:

- `ReadinessCheckName`: `str` *(required)*
- `ResourceSetName`: `str` *(required)*

Returns a `Coroutine` for
[UpdateReadinessCheckResponseTypeDef](./type_defs.md#updatereadinesscheckresponsetypedef).

<a id="update_recovery_group"></a>

### update_recovery_group

Updates an existing Recovery Group.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").update_recovery_group`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.update_recovery_group](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_recovery_group)

Asynchronous method. Use `await update_recovery_group(...)` for a synchronous
call.

Arguments mapping described in
[UpdateRecoveryGroupRequestRequestTypeDef](./type_defs.md#updaterecoverygrouprequestrequesttypedef).

Keyword-only arguments:

- `Cells`: `Sequence`\[`str`\] *(required)*
- `RecoveryGroupName`: `str` *(required)*

Returns a `Coroutine` for
[UpdateRecoveryGroupResponseTypeDef](./type_defs.md#updaterecoverygroupresponsetypedef).

<a id="update_resource_set"></a>

### update_resource_set

Updates an existing Resource Set.

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").update_resource_set`
method.

Boto3 documentation:
[Route53RecoveryReadiness.Client.update_resource_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness.Client.update_resource_set)

Asynchronous method. Use `await update_resource_set(...)` for a synchronous
call.

Arguments mapping described in
[UpdateResourceSetRequestRequestTypeDef](./type_defs.md#updateresourcesetrequestrequesttypedef).

Keyword-only arguments:

- `ResourceSetName`: `str` *(required)*
- `ResourceSetType`: `str` *(required)*
- `Resources`: `Sequence`\[[ResourceTypeDef](./type_defs.md#resourcetypedef)\]
  *(required)*

Returns a `Coroutine` for
[UpdateResourceSetResponseTypeDef](./type_defs.md#updateresourcesetresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for
`aiobotocore.create_client("route53-recovery-readiness").get_paginator` method
with overloads.

- `client.get_paginator("get_cell_readiness_summary")` ->
  [GetCellReadinessSummaryPaginator](./paginators.md#getcellreadinesssummarypaginator)
- `client.get_paginator("get_readiness_check_resource_status")` ->
  [GetReadinessCheckResourceStatusPaginator](./paginators.md#getreadinesscheckresourcestatuspaginator)
- `client.get_paginator("get_readiness_check_status")` ->
  [GetReadinessCheckStatusPaginator](./paginators.md#getreadinesscheckstatuspaginator)
- `client.get_paginator("get_recovery_group_readiness_summary")` ->
  [GetRecoveryGroupReadinessSummaryPaginator](./paginators.md#getrecoverygroupreadinesssummarypaginator)
- `client.get_paginator("list_cells")` ->
  [ListCellsPaginator](./paginators.md#listcellspaginator)
- `client.get_paginator("list_cross_account_authorizations")` ->
  [ListCrossAccountAuthorizationsPaginator](./paginators.md#listcrossaccountauthorizationspaginator)
- `client.get_paginator("list_readiness_checks")` ->
  [ListReadinessChecksPaginator](./paginators.md#listreadinesscheckspaginator)
- `client.get_paginator("list_recovery_groups")` ->
  [ListRecoveryGroupsPaginator](./paginators.md#listrecoverygroupspaginator)
- `client.get_paginator("list_resource_sets")` ->
  [ListResourceSetsPaginator](./paginators.md#listresourcesetspaginator)
- `client.get_paginator("list_rules")` ->
  [ListRulesPaginator](./paginators.md#listrulespaginator)

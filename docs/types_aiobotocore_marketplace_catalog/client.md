<a id="marketplacecatalogclient-for-aiobotocore-marketplacecatalog-module"></a>

# MarketplaceCatalogClient for aiobotocore MarketplaceCatalog module

> [Index](../README.md) > [MarketplaceCatalog](./README.md) >
> MarketplaceCatalogClient

Auto-generated documentation for
[MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
type annotations stubs module
[types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).

- [MarketplaceCatalogClient for aiobotocore MarketplaceCatalog module](#marketplacecatalogclient-for-aiobotocore-marketplacecatalog-module)
  - [MarketplaceCatalogClient](#marketplacecatalogclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [cancel_change_set](#cancel_change_set)
    - [describe_change_set](#describe_change_set)
    - [describe_entity](#describe_entity)
    - [generate_presigned_url](#generate_presigned_url)
    - [list_change_sets](#list_change_sets)
    - [list_entities](#list_entities)
    - [start_change_set](#start_change_set)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="marketplacecatalogclient"></a>

## MarketplaceCatalogClient

Type annotations for `session.create_client("marketplace-catalog")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_marketplace_catalog.client import MarketplaceCatalogClient

session = get_session()
async with session.create_client("marketplace-catalog") as client:
    client: MarketplaceCatalogClient
```

Boto3 documentation:
[MarketplaceCatalog.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_marketplace_catalog.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```

Exceptions:

- `Exceptions.AccessDeniedException`
- `Exceptions.ClientError`
- `Exceptions.InternalServiceException`
- `Exceptions.ResourceInUseException`
- `Exceptions.ResourceNotFoundException`
- `Exceptions.ResourceNotSupportedException`
- `Exceptions.ServiceQuotaExceededException`
- `Exceptions.ThrottlingException`
- `Exceptions.ValidationException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MarketplaceCatalogClient exceptions.

Type annotations for `session.create_client("marketplace-catalog").exceptions`
method.

Boto3 documentation:
[MarketplaceCatalog.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("marketplace-catalog").can_paginate` method.

Boto3 documentation:
[MarketplaceCatalog.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="cancel\_change\_set"></a>

### cancel_change_set

Used to cancel an open change request.

Type annotations for
`session.create_client("marketplace-catalog").cancel_change_set` method.

Boto3 documentation:
[MarketplaceCatalog.Client.cancel_change_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.cancel_change_set)

Asynchronous method. Use `await cancel_change_set(...)` for a synchronous call.

Arguments mapping described in
[CancelChangeSetRequestRequestTypeDef](./type_defs.md#cancelchangesetrequestrequesttypedef).

Keyword-only arguments:

- `Catalog`: `str` *(required)*
- `ChangeSetId`: `str` *(required)*

Returns a `Coroutine` for
[CancelChangeSetResponseTypeDef](./type_defs.md#cancelchangesetresponsetypedef).

<a id="describe\_change\_set"></a>

### describe_change_set

Provides information about a given change set.

Type annotations for
`session.create_client("marketplace-catalog").describe_change_set` method.

Boto3 documentation:
[MarketplaceCatalog.Client.describe_change_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.describe_change_set)

Asynchronous method. Use `await describe_change_set(...)` for a synchronous
call.

Arguments mapping described in
[DescribeChangeSetRequestRequestTypeDef](./type_defs.md#describechangesetrequestrequesttypedef).

Keyword-only arguments:

- `Catalog`: `str` *(required)*
- `ChangeSetId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeChangeSetResponseTypeDef](./type_defs.md#describechangesetresponsetypedef).

<a id="describe\_entity"></a>

### describe_entity

Returns the metadata and content of the entity.

Type annotations for
`session.create_client("marketplace-catalog").describe_entity` method.

Boto3 documentation:
[MarketplaceCatalog.Client.describe_entity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.describe_entity)

Asynchronous method. Use `await describe_entity(...)` for a synchronous call.

Arguments mapping described in
[DescribeEntityRequestRequestTypeDef](./type_defs.md#describeentityrequestrequesttypedef).

Keyword-only arguments:

- `Catalog`: `str` *(required)*
- `EntityId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeEntityResponseTypeDef](./type_defs.md#describeentityresponsetypedef).

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("marketplace-catalog").generate_presigned_url` method.

Boto3 documentation:
[MarketplaceCatalog.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="list\_change\_sets"></a>

### list_change_sets

Returns the list of change sets owned by the account being used to make the
call.

Type annotations for
`session.create_client("marketplace-catalog").list_change_sets` method.

Boto3 documentation:
[MarketplaceCatalog.Client.list_change_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_change_sets)

Asynchronous method. Use `await list_change_sets(...)` for a synchronous call.

Arguments mapping described in
[ListChangeSetsRequestRequestTypeDef](./type_defs.md#listchangesetsrequestrequesttypedef).

Keyword-only arguments:

- `Catalog`: `str` *(required)*
- `FilterList`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `Sort`: [SortTypeDef](./type_defs.md#sorttypedef)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListChangeSetsResponseTypeDef](./type_defs.md#listchangesetsresponsetypedef).

<a id="list\_entities"></a>

### list_entities

Provides the list of entities of a given type.

Type annotations for
`session.create_client("marketplace-catalog").list_entities` method.

Boto3 documentation:
[MarketplaceCatalog.Client.list_entities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.list_entities)

Asynchronous method. Use `await list_entities(...)` for a synchronous call.

Arguments mapping described in
[ListEntitiesRequestRequestTypeDef](./type_defs.md#listentitiesrequestrequesttypedef).

Keyword-only arguments:

- `Catalog`: `str` *(required)*
- `EntityType`: `str` *(required)*
- `FilterList`: `Sequence`\[[FilterTypeDef](./type_defs.md#filtertypedef)\]
- `Sort`: [SortTypeDef](./type_defs.md#sorttypedef)
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[ListEntitiesResponseTypeDef](./type_defs.md#listentitiesresponsetypedef).

<a id="start\_change\_set"></a>

### start_change_set

This operation allows you to request changes for your entities.

Type annotations for
`session.create_client("marketplace-catalog").start_change_set` method.

Boto3 documentation:
[MarketplaceCatalog.Client.start_change_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.start_change_set)

Asynchronous method. Use `await start_change_set(...)` for a synchronous call.

Arguments mapping described in
[StartChangeSetRequestRequestTypeDef](./type_defs.md#startchangesetrequestrequesttypedef).

Keyword-only arguments:

- `Catalog`: `str` *(required)*
- `ChangeSet`: `Sequence`\[[ChangeTypeDef](./type_defs.md#changetypedef)\]
  *(required)*
- `ChangeSetName`: `str`
- `ClientRequestToken`: `str`

Returns a `Coroutine` for
[StartChangeSetResponseTypeDef](./type_defs.md#startchangesetresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("marketplace-catalog").__aenter__`
method.

Boto3 documentation:
[MarketplaceCatalog.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[MarketplaceCatalogClient](#marketplacecatalogclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("marketplace-catalog").__aexit__`
method.

Boto3 documentation:
[MarketplaceCatalog.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

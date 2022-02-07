<a id="simpledbclient-for-aiobotocore-simpledb-module"></a>

# SimpleDBClient for aiobotocore SimpleDB module

> [Index](..) > [SimpleDB](.) > SimpleDBClient

Auto-generated documentation for
[SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
type annotations stubs module
[types-aiobotocore-sdb](https://pypi.org/project/types-aiobotocore-sdb/).

- [SimpleDBClient for aiobotocore SimpleDB module](#simpledbclient-for-aiobotocore-simpledb-module)
  - [SimpleDBClient](#simpledbclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [batch_delete_attributes](#batch_delete_attributes)
    - [batch_put_attributes](#batch_put_attributes)
    - [can_paginate](#can_paginate)
    - [create_domain](#create_domain)
    - [delete_attributes](#delete_attributes)
    - [delete_domain](#delete_domain)
    - [domain_metadata](#domain_metadata)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_attributes](#get_attributes)
    - [list_domains](#list_domains)
    - [put_attributes](#put_attributes)
    - [select](#select)
    - [__aenter__](#__aenter__)
    - [__aexit__](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="simpledbclient"></a>

## SimpleDBClient

Type annotations for `session.create_client("sdb")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_sdb.client import SimpleDBClient

session = get_session()
async with session.create_client("sdb") as client:
    client: SimpleDBClient
```

Boto3 documentation:
[SimpleDB.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_sdb.client import Exceptions

def handle_error(exc: Exceptions.AttributeDoesNotExist) -> None:
    ...
```

Exceptions:

- `Exceptions.AttributeDoesNotExist`
- `Exceptions.ClientError`
- `Exceptions.DuplicateItemName`
- `Exceptions.InvalidNextToken`
- `Exceptions.InvalidNumberPredicates`
- `Exceptions.InvalidNumberValueTests`
- `Exceptions.InvalidParameterValue`
- `Exceptions.InvalidQueryExpression`
- `Exceptions.MissingParameter`
- `Exceptions.NoSuchDomain`
- `Exceptions.NumberDomainAttributesExceeded`
- `Exceptions.NumberDomainBytesExceeded`
- `Exceptions.NumberDomainsExceeded`
- `Exceptions.NumberItemAttributesExceeded`
- `Exceptions.NumberSubmittedAttributesExceeded`
- `Exceptions.NumberSubmittedItemsExceeded`
- `Exceptions.RequestTimeout`
- `Exceptions.TooManyRequestedAttributes`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SimpleDBClient exceptions.

Type annotations for `session.create_client("sdb").exceptions` method.

Boto3 documentation:
[SimpleDB.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="batch_delete_attributes"></a>

### batch_delete_attributes

Performs multiple DeleteAttributes operations in a single call, which reduces
round trips and latencies.

Type annotations for `session.create_client("sdb").batch_delete_attributes`
method.

Boto3 documentation:
[SimpleDB.Client.batch_delete_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.batch_delete_attributes)

Asynchronous method. Use `await batch_delete_attributes(...)` for a synchronous
call.

Arguments mapping described in
[BatchDeleteAttributesRequestRequestTypeDef](./type_defs.md#batchdeleteattributesrequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*
- `Items`:
  `Sequence`\[[DeletableItemTypeDef](./type_defs.md#deletableitemtypedef)\]
  *(required)*

<a id="batch_put_attributes"></a>

### batch_put_attributes

The `BatchPutAttributes` operation creates or replaces attributes within one or
more items.

Type annotations for `session.create_client("sdb").batch_put_attributes`
method.

Boto3 documentation:
[SimpleDB.Client.batch_put_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.batch_put_attributes)

Asynchronous method. Use `await batch_put_attributes(...)` for a synchronous
call.

Arguments mapping described in
[BatchPutAttributesRequestRequestTypeDef](./type_defs.md#batchputattributesrequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*
- `Items`:
  `Sequence`\[[ReplaceableItemTypeDef](./type_defs.md#replaceableitemtypedef)\]
  *(required)*

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("sdb").can_paginate` method.

Boto3 documentation:
[SimpleDB.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="create_domain"></a>

### create_domain

The `CreateDomain` operation creates a new domain.

Type annotations for `session.create_client("sdb").create_domain` method.

Boto3 documentation:
[SimpleDB.Client.create_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.create_domain)

Asynchronous method. Use `await create_domain(...)` for a synchronous call.

Arguments mapping described in
[CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*

<a id="delete_attributes"></a>

### delete_attributes

Deletes one or more attributes associated with an item.

Type annotations for `session.create_client("sdb").delete_attributes` method.

Boto3 documentation:
[SimpleDB.Client.delete_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.delete_attributes)

Asynchronous method. Use `await delete_attributes(...)` for a synchronous call.

Arguments mapping described in
[DeleteAttributesRequestRequestTypeDef](./type_defs.md#deleteattributesrequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*
- `ItemName`: `str` *(required)*
- `Attributes`:
  `Sequence`\[[AttributeTypeDef](./type_defs.md#attributetypedef)\]
- `Expected`: [UpdateConditionTypeDef](./type_defs.md#updateconditiontypedef)

<a id="delete_domain"></a>

### delete_domain

The `DeleteDomain` operation deletes a domain.

Type annotations for `session.create_client("sdb").delete_domain` method.

Boto3 documentation:
[SimpleDB.Client.delete_domain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.delete_domain)

Asynchronous method. Use `await delete_domain(...)` for a synchronous call.

Arguments mapping described in
[DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*

<a id="domain_metadata"></a>

### domain_metadata

Returns information about the domain, including when the domain was created,
the number of items and attributes in the domain, and the size of the attribute
names and values.

Type annotations for `session.create_client("sdb").domain_metadata` method.

Boto3 documentation:
[SimpleDB.Client.domain_metadata](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.domain_metadata)

Asynchronous method. Use `await domain_metadata(...)` for a synchronous call.

Arguments mapping described in
[DomainMetadataRequestRequestTypeDef](./type_defs.md#domainmetadatarequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*

Returns a `Coroutine` for
[DomainMetadataResultTypeDef](./type_defs.md#domainmetadataresulttypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `session.create_client("sdb").generate_presigned_url`
method.

Boto3 documentation:
[SimpleDB.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_attributes"></a>

### get_attributes

Returns all of the attributes associated with the specified item.

Type annotations for `session.create_client("sdb").get_attributes` method.

Boto3 documentation:
[SimpleDB.Client.get_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.get_attributes)

Asynchronous method. Use `await get_attributes(...)` for a synchronous call.

Arguments mapping described in
[GetAttributesRequestRequestTypeDef](./type_defs.md#getattributesrequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*
- `ItemName`: `str` *(required)*
- `AttributeNames`: `Sequence`\[`str`\]
- `ConsistentRead`: `bool`

Returns a `Coroutine` for
[GetAttributesResultTypeDef](./type_defs.md#getattributesresulttypedef).

<a id="list_domains"></a>

### list_domains

The `ListDomains` operation lists all domains associated with the Access Key
ID.

Type annotations for `session.create_client("sdb").list_domains` method.

Boto3 documentation:
[SimpleDB.Client.list_domains](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.list_domains)

Asynchronous method. Use `await list_domains(...)` for a synchronous call.

Arguments mapping described in
[ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef).

Keyword-only arguments:

- `MaxNumberOfDomains`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListDomainsResultTypeDef](./type_defs.md#listdomainsresulttypedef).

<a id="put_attributes"></a>

### put_attributes

The PutAttributes operation creates or replaces attributes in an item.

Type annotations for `session.create_client("sdb").put_attributes` method.

Boto3 documentation:
[SimpleDB.Client.put_attributes](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.put_attributes)

Asynchronous method. Use `await put_attributes(...)` for a synchronous call.

Arguments mapping described in
[PutAttributesRequestRequestTypeDef](./type_defs.md#putattributesrequestrequesttypedef).

Keyword-only arguments:

- `DomainName`: `str` *(required)*
- `ItemName`: `str` *(required)*
- `Attributes`:
  `Sequence`\[[ReplaceableAttributeTypeDef](./type_defs.md#replaceableattributetypedef)\]
  *(required)*
- `Expected`: [UpdateConditionTypeDef](./type_defs.md#updateconditiontypedef)

<a id="select"></a>

### select

The `Select` operation returns a set of attributes for `ItemNames` that match
the select expression.

Type annotations for `session.create_client("sdb").select` method.

Boto3 documentation:
[SimpleDB.Client.select](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.select)

Asynchronous method. Use `await select(...)` for a synchronous call.

Arguments mapping described in
[SelectRequestRequestTypeDef](./type_defs.md#selectrequestrequesttypedef).

Keyword-only arguments:

- `SelectExpression`: `str` *(required)*
- `NextToken`: `str`
- `ConsistentRead`: `bool`

Returns a `Coroutine` for
[SelectResultTypeDef](./type_defs.md#selectresulttypedef).

<a id="__aenter__"></a>

### __aenter__

Type annotations for `session.create_client("sdb").__aenter__` method.

Boto3 documentation:
[SimpleDB.Client.__aenter__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [SimpleDBClient](#simpledbclient).

<a id="__aexit__"></a>

### __aexit__

Type annotations for `session.create_client("sdb").__aexit__` method.

Boto3 documentation:
[SimpleDB.Client.__aexit__](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for `session.create_client("sdb").get_paginator` method with
overloads.

- `client.get_paginator("list_domains")` ->
  [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- `client.get_paginator("select")` ->
  [SelectPaginator](./paginators.md#selectpaginator)

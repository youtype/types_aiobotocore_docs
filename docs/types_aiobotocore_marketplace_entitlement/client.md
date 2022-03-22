<a id="marketplaceentitlementserviceclient-for-aiobotocore-marketplaceentitlementservice-module"></a>

# MarketplaceEntitlementServiceClient for aiobotocore MarketplaceEntitlementService module

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) >
> MarketplaceEntitlementServiceClient

Auto-generated documentation for
[MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
type annotations stubs module
[types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

- [MarketplaceEntitlementServiceClient for aiobotocore MarketplaceEntitlementService module](#marketplaceentitlementserviceclient-for-aiobotocore-marketplaceentitlementservice-module)
  - [MarketplaceEntitlementServiceClient](#marketplaceentitlementserviceclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_entitlements](#get_entitlements)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)
    - [get_paginator](#get_paginator)

<a id="marketplaceentitlementserviceclient"></a>

## MarketplaceEntitlementServiceClient

Type annotations for `session.create_client("marketplace-entitlement")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient

session = get_session()
async with session.create_client("marketplace-entitlement") as client:
    client: MarketplaceEntitlementServiceClient
```

Boto3 documentation:
[MarketplaceEntitlementService.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_marketplace_entitlement.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.InternalServiceErrorException`
- `Exceptions.InvalidParameterException`
- `Exceptions.ThrottlingException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

MarketplaceEntitlementServiceClient exceptions.

Type annotations for
`session.create_client("marketplace-entitlement").exceptions` method.

Boto3 documentation:
[MarketplaceEntitlementService.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for
`session.create_client("marketplace-entitlement").can_paginate` method.

Boto3 documentation:
[MarketplaceEntitlementService.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("marketplace-entitlement").generate_presigned_url`
method.

Boto3 documentation:
[MarketplaceEntitlementService.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get\_entitlements"></a>

### get_entitlements

GetEntitlements retrieves entitlement values for a given product.

Type annotations for
`session.create_client("marketplace-entitlement").get_entitlements` method.

Boto3 documentation:
[MarketplaceEntitlementService.Client.get_entitlements](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.get_entitlements)

Asynchronous method. Use `await get_entitlements(...)` for a synchronous call.

Arguments mapping described in
[GetEntitlementsRequestRequestTypeDef](./type_defs.md#getentitlementsrequestrequesttypedef).

Keyword-only arguments:

- `ProductCode`: `str` *(required)*
- `Filter`:
  `Mapping`\[[GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype),
  `Sequence`\[`str`\]\]
- `NextToken`: `str`
- `MaxResults`: `int`

Returns a `Coroutine` for
[GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for
`session.create_client("marketplace-entitlement").__aenter__` method.

Boto3 documentation:
[MarketplaceEntitlementService.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for
[MarketplaceEntitlementServiceClient](#marketplaceentitlementserviceclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for
`session.create_client("marketplace-entitlement").__aexit__` method.

Boto3 documentation:
[MarketplaceEntitlementService.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.

<a id="get_paginator"></a>

### get_paginator

Type annotations for
`session.create_client("marketplace-entitlement").get_paginator` method with
overloads.

- `client.get_paginator("get_entitlements")` ->
  [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)

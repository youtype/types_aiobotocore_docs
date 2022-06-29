# MarketplaceEntitlementServiceClient

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) > MarketplaceEntitlementServiceClient

!!! note ""

    Auto-generated documentation for [MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
    type annotations stubs module [types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

## MarketplaceEntitlementServiceClient

Type annotations and code completion for `#!python session.create_client("marketplace-entitlement")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_marketplace_entitlement.client import MarketplaceEntitlementServiceClient

session = get_session()
async with session.create_client("marketplace-entitlement") as client:
    client: MarketplaceEntitlementServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("marketplace-entitlement").exceptions` structure.

```python title="Usage example"
async with session.create_client("marketplace-entitlement") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServiceErrorException,
        client.InvalidParameterException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python title="Type checking example"
from types_aiobotocore_marketplace_entitlement.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("marketplace-entitlement").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("marketplace-entitlement").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.close)

```python title="Method definition"
await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("marketplace-entitlement").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.generate_presigned_url)

```python title="Method definition"
await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_entitlements

GetEntitlements retrieves entitlement values for a given product.

Type annotations and code completion for `#!python session.create_client("marketplace-entitlement").get_entitlements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.get_entitlements)

```python title="Method definition"
await def get_entitlements(
    self,
    *,
    ProductCode: str,
    Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> GetEntitlementsResultTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype) 
2. See [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: GetEntitlementsRequestRequestTypeDef = {  # (1)
    "ProductCode": ...,
}

parent.get_entitlements(**kwargs)
```

1. See [:material-code-braces: GetEntitlementsRequestRequestTypeDef](./type_defs.md#getentitlementsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("marketplace-entitlement").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> MarketplaceEntitlementServiceClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("marketplace-entitlement").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("marketplace-entitlement").get_paginator` method with overloads.

- `client.get_paginator("get_entitlements")` -> [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)




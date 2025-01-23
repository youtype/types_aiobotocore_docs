# Paginators

> [Index](../README.md) > [MarketplaceEntitlementService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#marketplaceentitlementservice)
    type annotations stubs module [types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

## GetEntitlementsPaginator

Type annotations and code completion for `#!python session.create_client("marketplace-entitlement").get_paginator("get_entitlements")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement/paginator/GetEntitlements.html#MarketplaceEntitlementService.Paginator.GetEntitlements)

```python
# GetEntitlementsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_entitlement.paginator import GetEntitlementsPaginator

session = get_session()
async with session.create_client("marketplace-entitlement") as client:  # (1)
    paginator: GetEntitlementsPaginator = client.get_paginator("get_entitlements")  # (2)
    async for item in paginator.paginate(...):
        item: GetEntitlementsResultTypeDef
        print(item)  # (3)
```

1. client: [MarketplaceEntitlementServiceClient](./client.md)
2. paginator: [GetEntitlementsPaginator](./paginators.md#getentitlementspaginator)
3. item: [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 


### paginate

Type annotations and code completion for `#!python GetEntitlementsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProductCode: str,
    Filter: Mapping[GetEntitlementFilterNameType, Sequence[str]] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetEntitlementsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetEntitlementsRequestPaginateTypeDef = {  # (1)
    "ProductCode": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetEntitlementsRequestPaginateTypeDef](./type_defs.md#getentitlementsrequestpaginatetypedef) 

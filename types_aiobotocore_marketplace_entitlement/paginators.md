<a id="paginators-for-aiobotocore-marketplaceentitlementservice-module"></a>

# Paginators for aiobotocore MarketplaceEntitlementService module

> [Index](..) > [MarketplaceEntitlementService](.) > Paginators

Auto-generated documentation for
[MarketplaceEntitlementService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService)
type annotations stubs module
[types-aiobotocore-marketplace-entitlement](https://pypi.org/project/types-aiobotocore-marketplace-entitlement/).

- [Paginators for aiobotocore MarketplaceEntitlementService module](#paginators-for-aiobotocore-marketplaceentitlementservice-module)
  - [GetEntitlementsPaginator](#getentitlementspaginator)

<a id="getentitlementspaginator"></a>

## GetEntitlementsPaginator

Type annotations for
`aiobotocore.create_client("marketplace-entitlement").get_paginator("get_entitlements")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_marketplace_entitlement.paginator import GetEntitlementsPaginator

def get_get_entitlements_paginator() -> GetEntitlementsPaginator:
    return Session().create_client("marketplace-entitlement").get_paginator("get_entitlements")
```

Boto3 documentation:
[MarketplaceEntitlementService.Paginator.GetEntitlements](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-entitlement.html#MarketplaceEntitlementService.Paginator.GetEntitlements)

Arguments for `GetEntitlementsPaginator.paginate` method:

- `ProductCode`: `str` *(required)*
- `Filter`:
  `Mapping`\[[GetEntitlementFilterNameType](./literals.md#getentitlementfilternametype),
  `Sequence`\[`str`\]\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`GetEntitlementsPaginator.paginate` returns
`_PageIterator`\[[GetEntitlementsResultTypeDef](./type_defs.md#getentitlementsresulttypedef)\].

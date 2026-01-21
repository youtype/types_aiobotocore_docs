# Examples

> [Index](../README.md) > [PartnerCentralBenefits](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PartnerCentralBenefits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-benefits.html#partnercentralbenefits)
    type annotations stubs module [types-aiobotocore-partnercentral-benefits](https://pypi.org/project/types-aiobotocore-partnercentral-benefits/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[partnercentral-benefits]` package installed.

Write your `PartnerCentralBenefits` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# PartnerCentralBenefitsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("partnercentral-benefits") as client:  # (1)
    result = await client.associate_benefit_application_resource()  # (2)
```

1. client: [PartnerCentralBenefitsClient](./client.md)
2. result: [:material-code-braces: AssociateBenefitApplicationResourceOutputTypeDef](./type_defs.md#associatebenefitapplicationresourceoutputtypedef)



#### Paginator usage example

```python
# ListBenefitAllocationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("partnercentral-benefits") as client:  # (1)
    paginator = client.get_paginator("list_benefit_allocations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PartnerCentralBenefitsClient](./client.md)
2. paginator: [ListBenefitAllocationsPaginator](./paginators.md#listbenefitallocationspaginator)
3. item: [:material-code-braces: ListBenefitAllocationsOutputTypeDef](./type_defs.md#listbenefitallocationsoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[partnercentral-benefits]`
or a standalone `types_aiobotocore_partnercentral_benefits` package, you have to explicitly specify
`client: PartnerCentralBenefitsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# PartnerCentralBenefitsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_benefits.client import PartnerCentralBenefitsClient
from types_aiobotocore_partnercentral_benefits.type_defs import AssociateBenefitApplicationResourceOutputTypeDef
from types_aiobotocore_partnercentral_benefits.type_defs import AssociateBenefitApplicationResourceInputTypeDef


session = get_session()

async with session.create_client("partnercentral-benefits") as client:
    client: PartnerCentralBenefitsClient
    kwargs: AssociateBenefitApplicationResourceInputTypeDef = {...}
    result: AssociateBenefitApplicationResourceOutputTypeDef = await client.associate_benefit_application_resource(**kwargs)
```



#### Paginator usage example

```python
# ListBenefitAllocationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_benefits.client import PartnerCentralBenefitsClient
from types_aiobotocore_partnercentral_benefits.paginator import ListBenefitAllocationsPaginator
from types_aiobotocore_partnercentral_benefits.type_defs import ListBenefitAllocationsOutputTypeDef


session = get_session()

async with session.create_client("partnercentral-benefits") as client:
    client: PartnerCentralBenefitsClient
    paginator: ListBenefitAllocationsPaginator = client.get_paginator("list_benefit_allocations")
    async for item in paginator.paginate(...):
        item: ListBenefitAllocationsOutputTypeDef
        print(item)
```



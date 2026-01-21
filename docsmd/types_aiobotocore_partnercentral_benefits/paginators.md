# Paginators

> [Index](../README.md) > [PartnerCentralBenefits](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PartnerCentralBenefits](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-benefits.html#partnercentralbenefits)
    type annotations stubs module [types-aiobotocore-partnercentral-benefits](https://pypi.org/project/types-aiobotocore-partnercentral-benefits/).

## ListBenefitAllocationsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-benefits").get_paginator("list_benefit_allocations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-benefits/paginator/ListBenefitAllocations.html#PartnerCentralBenefits.Paginator.ListBenefitAllocations)

```python
# ListBenefitAllocationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_benefits.paginator import ListBenefitAllocationsPaginator

session = get_session()
async with session.create_client("partnercentral-benefits") as client:  # (1)
    paginator: ListBenefitAllocationsPaginator = client.get_paginator("list_benefit_allocations")  # (2)
    async for item in paginator.paginate(...):
        item: ListBenefitAllocationsOutputTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralBenefitsClient](./client.md)
2. paginator: [ListBenefitAllocationsPaginator](./paginators.md#listbenefitallocationspaginator)
3. item: `AioPageIterator[ListBenefitAllocationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBenefitAllocationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    FulfillmentTypes: Sequence[FulfillmentTypeType] = ...,  # (1)
    BenefitIdentifiers: Sequence[str] = ...,
    BenefitApplicationIdentifiers: Sequence[str] = ...,
    Status: Sequence[BenefitAllocationStatusType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListBenefitAllocationsOutputTypeDef]:  # (4)
    ...
```

1. See `Sequence[FulfillmentTypeType]`
2. See `Sequence[BenefitAllocationStatusType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListBenefitAllocationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBenefitAllocationsInputPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBenefitAllocationsInputPaginateTypeDef](./type_defs.md#listbenefitallocationsinputpaginatetypedef)
## ListBenefitApplicationsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-benefits").get_paginator("list_benefit_applications")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-benefits/paginator/ListBenefitApplications.html#PartnerCentralBenefits.Paginator.ListBenefitApplications)

```python
# ListBenefitApplicationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_benefits.paginator import ListBenefitApplicationsPaginator

session = get_session()
async with session.create_client("partnercentral-benefits") as client:  # (1)
    paginator: ListBenefitApplicationsPaginator = client.get_paginator("list_benefit_applications")  # (2)
    async for item in paginator.paginate(...):
        item: ListBenefitApplicationsOutputTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralBenefitsClient](./client.md)
2. paginator: [ListBenefitApplicationsPaginator](./paginators.md#listbenefitapplicationspaginator)
3. item: `AioPageIterator[ListBenefitApplicationsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBenefitApplicationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    Programs: Sequence[str] = ...,
    FulfillmentTypes: Sequence[FulfillmentTypeType] = ...,  # (1)
    BenefitIdentifiers: Sequence[str] = ...,
    Status: Sequence[BenefitApplicationStatusType] = ...,  # (2)
    Stages: Sequence[str] = ...,
    AssociatedResources: Sequence[AssociatedResourceTypeDef] = ...,  # (3)
    AssociatedResourceArns: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[ListBenefitApplicationsOutputTypeDef]:  # (5)
    ...
```

1. See `Sequence[FulfillmentTypeType]`
2. See `Sequence[BenefitApplicationStatusType]`
3. See `Sequence[AssociatedResourceTypeDef]`
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[ListBenefitApplicationsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBenefitApplicationsInputPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBenefitApplicationsInputPaginateTypeDef](./type_defs.md#listbenefitapplicationsinputpaginatetypedef)
## ListBenefitsPaginator

Type annotations and code completion for `#!python session.create_client("partnercentral-benefits").get_paginator("list_benefits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-benefits/paginator/ListBenefits.html#PartnerCentralBenefits.Paginator.ListBenefits)

```python
# ListBenefitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_partnercentral_benefits.paginator import ListBenefitsPaginator

session = get_session()
async with session.create_client("partnercentral-benefits") as client:  # (1)
    paginator: ListBenefitsPaginator = client.get_paginator("list_benefits")  # (2)
    async for item in paginator.paginate(...):
        item: ListBenefitsOutputTypeDef
        print(item)  # (3)
```

1. client: [PartnerCentralBenefitsClient](./client.md)
2. paginator: [ListBenefitsPaginator](./paginators.md#listbenefitspaginator)
3. item: `AioPageIterator[ListBenefitsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListBenefitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Catalog: str,
    Programs: Sequence[str] = ...,
    FulfillmentTypes: Sequence[FulfillmentTypeType] = ...,  # (1)
    Status: Sequence[BenefitStatusType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListBenefitsOutputTypeDef]:  # (4)
    ...
```

1. See `Sequence[FulfillmentTypeType]`
2. See `Sequence[BenefitStatusType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListBenefitsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListBenefitsInputPaginateTypeDef = {  # (1)
    "Catalog": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListBenefitsInputPaginateTypeDef](./type_defs.md#listbenefitsinputpaginatetypedef)

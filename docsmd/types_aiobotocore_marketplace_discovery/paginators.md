# Paginators

> [Index](../README.md) > [MarketplaceDiscovery](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MarketplaceDiscovery](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-discovery.html#marketplacediscovery)
    type annotations stubs module [types-aiobotocore-marketplace-discovery](https://pypi.org/project/types-aiobotocore-marketplace-discovery/).

## GetOfferTermsPaginator

Type annotations and code completion for `#!python session.create_client("marketplace-discovery").get_paginator("get_offer_terms")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-discovery/paginator/GetOfferTerms.html#MarketplaceDiscovery.Paginator.GetOfferTerms)

```python
# GetOfferTermsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_discovery.paginator import GetOfferTermsPaginator

session = get_session()
async with session.create_client("marketplace-discovery") as client:  # (1)
    paginator: GetOfferTermsPaginator = client.get_paginator("get_offer_terms")  # (2)
    async for item in paginator.paginate(...):
        item: GetOfferTermsOutputTypeDef
        print(item)  # (3)
```

1. client: [MarketplaceDiscoveryClient](./client.md)
2. paginator: [GetOfferTermsPaginator](./paginators.md#getoffertermspaginator)
3. item: `AioPageIterator[GetOfferTermsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python GetOfferTermsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    offerId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetOfferTermsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetOfferTermsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetOfferTermsInputPaginateTypeDef = {  # (1)
    "offerId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOfferTermsInputPaginateTypeDef](./type_defs.md#getoffertermsinputpaginatetypedef)
## ListFulfillmentOptionsPaginator

Type annotations and code completion for `#!python session.create_client("marketplace-discovery").get_paginator("list_fulfillment_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-discovery/paginator/ListFulfillmentOptions.html#MarketplaceDiscovery.Paginator.ListFulfillmentOptions)

```python
# ListFulfillmentOptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_discovery.paginator import ListFulfillmentOptionsPaginator

session = get_session()
async with session.create_client("marketplace-discovery") as client:  # (1)
    paginator: ListFulfillmentOptionsPaginator = client.get_paginator("list_fulfillment_options")  # (2)
    async for item in paginator.paginate(...):
        item: ListFulfillmentOptionsOutputTypeDef
        print(item)  # (3)
```

1. client: [MarketplaceDiscoveryClient](./client.md)
2. paginator: [ListFulfillmentOptionsPaginator](./paginators.md#listfulfillmentoptionspaginator)
3. item: `AioPageIterator[ListFulfillmentOptionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFulfillmentOptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    productId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFulfillmentOptionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFulfillmentOptionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFulfillmentOptionsInputPaginateTypeDef = {  # (1)
    "productId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFulfillmentOptionsInputPaginateTypeDef](./type_defs.md#listfulfillmentoptionsinputpaginatetypedef)
## ListPurchaseOptionsPaginator

Type annotations and code completion for `#!python session.create_client("marketplace-discovery").get_paginator("list_purchase_options")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-discovery/paginator/ListPurchaseOptions.html#MarketplaceDiscovery.Paginator.ListPurchaseOptions)

```python
# ListPurchaseOptionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_discovery.paginator import ListPurchaseOptionsPaginator

session = get_session()
async with session.create_client("marketplace-discovery") as client:  # (1)
    paginator: ListPurchaseOptionsPaginator = client.get_paginator("list_purchase_options")  # (2)
    async for item in paginator.paginate(...):
        item: ListPurchaseOptionsOutputTypeDef
        print(item)  # (3)
```

1. client: [MarketplaceDiscoveryClient](./client.md)
2. paginator: [ListPurchaseOptionsPaginator](./paginators.md#listpurchaseoptionspaginator)
3. item: `AioPageIterator[ListPurchaseOptionsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPurchaseOptionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[PurchaseOptionFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListPurchaseOptionsOutputTypeDef]:  # (3)
    ...
```

1. See `Sequence[PurchaseOptionFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPurchaseOptionsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPurchaseOptionsInputPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPurchaseOptionsInputPaginateTypeDef](./type_defs.md#listpurchaseoptionsinputpaginatetypedef)
## SearchFacetsPaginator

Type annotations and code completion for `#!python session.create_client("marketplace-discovery").get_paginator("search_facets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-discovery/paginator/SearchFacets.html#MarketplaceDiscovery.Paginator.SearchFacets)

```python
# SearchFacetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_discovery.paginator import SearchFacetsPaginator

session = get_session()
async with session.create_client("marketplace-discovery") as client:  # (1)
    paginator: SearchFacetsPaginator = client.get_paginator("search_facets")  # (2)
    async for item in paginator.paginate(...):
        item: SearchFacetsOutputTypeDef
        print(item)  # (3)
```

1. client: [MarketplaceDiscoveryClient](./client.md)
2. paginator: [SearchFacetsPaginator](./paginators.md#searchfacetspaginator)
3. item: `AioPageIterator[SearchFacetsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchFacetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    searchText: str = ...,
    filters: Sequence[SearchFilterTypeDef] = ...,  # (1)
    facetTypes: Sequence[SearchFacetTypeType] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[SearchFacetsOutputTypeDef]:  # (4)
    ...
```

1. See `Sequence[SearchFilterTypeDef]`
2. See `Sequence[SearchFacetTypeType]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[SearchFacetsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchFacetsInputPaginateTypeDef = {  # (1)
    "searchText": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchFacetsInputPaginateTypeDef](./type_defs.md#searchfacetsinputpaginatetypedef)
## SearchListingsPaginator

Type annotations and code completion for `#!python session.create_client("marketplace-discovery").get_paginator("search_listings")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-discovery/paginator/SearchListings.html#MarketplaceDiscovery.Paginator.SearchListings)

```python
# SearchListingsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_marketplace_discovery.paginator import SearchListingsPaginator

session = get_session()
async with session.create_client("marketplace-discovery") as client:  # (1)
    paginator: SearchListingsPaginator = client.get_paginator("search_listings")  # (2)
    async for item in paginator.paginate(...):
        item: SearchListingsOutputTypeDef
        print(item)  # (3)
```

1. client: [MarketplaceDiscoveryClient](./client.md)
2. paginator: [SearchListingsPaginator](./paginators.md#searchlistingspaginator)
3. item: `AioPageIterator[SearchListingsOutputTypeDef]`


### paginate

Type annotations and code completion for `#!python SearchListingsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    searchText: str = ...,
    filters: Sequence[SearchFilterTypeDef] = ...,  # (1)
    sortBy: SearchListingsSortByType = ...,  # (2)
    sortOrder: SearchListingsSortOrderType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[SearchListingsOutputTypeDef]:  # (5)
    ...
```

1. See `Sequence[SearchFilterTypeDef]`
2. See [:material-code-brackets: SearchListingsSortByType](./literals.md#searchlistingssortbytype)
3. See [:material-code-brackets: SearchListingsSortOrderType](./literals.md#searchlistingssortordertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[SearchListingsOutputTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: SearchListingsInputPaginateTypeDef = {  # (1)
    "searchText": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchListingsInputPaginateTypeDef](./type_defs.md#searchlistingsinputpaginatetypedef)

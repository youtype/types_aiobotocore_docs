# Paginators

> [Index](../README.md) > [SageMakergeospatialcapabilities](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SageMakergeospatialcapabilities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#sagemakergeospatialcapabilities)
    type annotations stubs module [types-aiobotocore-sagemaker-geospatial](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial/).

## ListEarthObservationJobsPaginator

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").get_paginator("list_earth_observation_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial/paginator/ListEarthObservationJobs.html#SageMakergeospatialcapabilities.Paginator.ListEarthObservationJobs)

```python
# ListEarthObservationJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_geospatial.paginator import ListEarthObservationJobsPaginator

session = get_session()
async with session.create_client("sagemaker-geospatial") as client:  # (1)
    paginator: ListEarthObservationJobsPaginator = client.get_paginator("list_earth_observation_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListEarthObservationJobOutputTypeDef
        print(item)  # (3)
```

1. client: [SageMakergeospatialcapabilitiesClient](./client.md)
2. paginator: [ListEarthObservationJobsPaginator](./paginators.md#listearthobservationjobspaginator)
3. item: [:material-code-braces: ListEarthObservationJobOutputTypeDef](./type_defs.md#listearthobservationjoboutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListEarthObservationJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SortBy: str = ...,
    SortOrder: SortOrderType = ...,  # (1)
    StatusEquals: EarthObservationJobStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListEarthObservationJobOutputTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: EarthObservationJobStatusType](./literals.md#earthobservationjobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListEarthObservationJobOutputTypeDef](./type_defs.md#listearthobservationjoboutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEarthObservationJobInputPaginateTypeDef = {  # (1)
    "SortBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEarthObservationJobInputPaginateTypeDef](./type_defs.md#listearthobservationjobinputpaginatetypedef) 
## ListRasterDataCollectionsPaginator

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").get_paginator("list_raster_data_collections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial/paginator/ListRasterDataCollections.html#SageMakergeospatialcapabilities.Paginator.ListRasterDataCollections)

```python
# ListRasterDataCollectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_geospatial.paginator import ListRasterDataCollectionsPaginator

session = get_session()
async with session.create_client("sagemaker-geospatial") as client:  # (1)
    paginator: ListRasterDataCollectionsPaginator = client.get_paginator("list_raster_data_collections")  # (2)
    async for item in paginator.paginate(...):
        item: ListRasterDataCollectionsOutputTypeDef
        print(item)  # (3)
```

1. client: [SageMakergeospatialcapabilitiesClient](./client.md)
2. paginator: [ListRasterDataCollectionsPaginator](./paginators.md#listrasterdatacollectionspaginator)
3. item: [:material-code-braces: ListRasterDataCollectionsOutputTypeDef](./type_defs.md#listrasterdatacollectionsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListRasterDataCollectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListRasterDataCollectionsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListRasterDataCollectionsOutputTypeDef](./type_defs.md#listrasterdatacollectionsoutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRasterDataCollectionsInputPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRasterDataCollectionsInputPaginateTypeDef](./type_defs.md#listrasterdatacollectionsinputpaginatetypedef) 
## ListVectorEnrichmentJobsPaginator

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").get_paginator("list_vector_enrichment_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial/paginator/ListVectorEnrichmentJobs.html#SageMakergeospatialcapabilities.Paginator.ListVectorEnrichmentJobs)

```python
# ListVectorEnrichmentJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_sagemaker_geospatial.paginator import ListVectorEnrichmentJobsPaginator

session = get_session()
async with session.create_client("sagemaker-geospatial") as client:  # (1)
    paginator: ListVectorEnrichmentJobsPaginator = client.get_paginator("list_vector_enrichment_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListVectorEnrichmentJobOutputTypeDef
        print(item)  # (3)
```

1. client: [SageMakergeospatialcapabilitiesClient](./client.md)
2. paginator: [ListVectorEnrichmentJobsPaginator](./paginators.md#listvectorenrichmentjobspaginator)
3. item: [:material-code-braces: ListVectorEnrichmentJobOutputTypeDef](./type_defs.md#listvectorenrichmentjoboutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListVectorEnrichmentJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SortBy: str = ...,
    SortOrder: SortOrderType = ...,  # (1)
    StatusEquals: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListVectorEnrichmentJobOutputTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListVectorEnrichmentJobOutputTypeDef](./type_defs.md#listvectorenrichmentjoboutputtypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVectorEnrichmentJobInputPaginateTypeDef = {  # (1)
    "SortBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVectorEnrichmentJobInputPaginateTypeDef](./type_defs.md#listvectorenrichmentjobinputpaginatetypedef) 

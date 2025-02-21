# Paginators

> [Index](../README.md) > [HealthImaging](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [HealthImaging](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging.html#healthimaging)
    type annotations stubs module [types-aiobotocore-medical-imaging](https://pypi.org/project/types-aiobotocore-medical-imaging/).

## ListDICOMImportJobsPaginator

Type annotations and code completion for `#!python session.create_client("medical-imaging").get_paginator("list_dicom_import_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging/paginator/ListDICOMImportJobs.html#HealthImaging.Paginator.ListDICOMImportJobs)

```python
# ListDICOMImportJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medical_imaging.paginator import ListDICOMImportJobsPaginator

session = get_session()
async with session.create_client("medical-imaging") as client:  # (1)
    paginator: ListDICOMImportJobsPaginator = client.get_paginator("list_dicom_import_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListDICOMImportJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthImagingClient](./client.md)
2. paginator: [ListDICOMImportJobsPaginator](./paginators.md#listdicomimportjobspaginator)
3. item: [:material-code-braces: ListDICOMImportJobsResponseTypeDef](./type_defs.md#listdicomimportjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDICOMImportJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datastoreId: str,
    jobStatus: JobStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDICOMImportJobsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDICOMImportJobsResponseTypeDef](./type_defs.md#listdicomimportjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDICOMImportJobsRequestPaginateTypeDef = {  # (1)
    "datastoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDICOMImportJobsRequestPaginateTypeDef](./type_defs.md#listdicomimportjobsrequestpaginatetypedef) 
## ListDatastoresPaginator

Type annotations and code completion for `#!python session.create_client("medical-imaging").get_paginator("list_datastores")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging/paginator/ListDatastores.html#HealthImaging.Paginator.ListDatastores)

```python
# ListDatastoresPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medical_imaging.paginator import ListDatastoresPaginator

session = get_session()
async with session.create_client("medical-imaging") as client:  # (1)
    paginator: ListDatastoresPaginator = client.get_paginator("list_datastores")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatastoresResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthImagingClient](./client.md)
2. paginator: [ListDatastoresPaginator](./paginators.md#listdatastorespaginator)
3. item: [:material-code-braces: ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDatastoresPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datastoreStatus: DatastoreStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDatastoresResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DatastoreStatusType](./literals.md#datastorestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDatastoresResponseTypeDef](./type_defs.md#listdatastoresresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDatastoresRequestPaginateTypeDef = {  # (1)
    "datastoreStatus": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatastoresRequestPaginateTypeDef](./type_defs.md#listdatastoresrequestpaginatetypedef) 
## ListImageSetVersionsPaginator

Type annotations and code completion for `#!python session.create_client("medical-imaging").get_paginator("list_image_set_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging/paginator/ListImageSetVersions.html#HealthImaging.Paginator.ListImageSetVersions)

```python
# ListImageSetVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medical_imaging.paginator import ListImageSetVersionsPaginator

session = get_session()
async with session.create_client("medical-imaging") as client:  # (1)
    paginator: ListImageSetVersionsPaginator = client.get_paginator("list_image_set_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListImageSetVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthImagingClient](./client.md)
2. paginator: [ListImageSetVersionsPaginator](./paginators.md#listimagesetversionspaginator)
3. item: [:material-code-braces: ListImageSetVersionsResponseTypeDef](./type_defs.md#listimagesetversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListImageSetVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datastoreId: str,
    imageSetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListImageSetVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListImageSetVersionsResponseTypeDef](./type_defs.md#listimagesetversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListImageSetVersionsRequestPaginateTypeDef = {  # (1)
    "datastoreId": ...,
    "imageSetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListImageSetVersionsRequestPaginateTypeDef](./type_defs.md#listimagesetversionsrequestpaginatetypedef) 
## SearchImageSetsPaginator

Type annotations and code completion for `#!python session.create_client("medical-imaging").get_paginator("search_image_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medical-imaging/paginator/SearchImageSets.html#HealthImaging.Paginator.SearchImageSets)

```python
# SearchImageSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_medical_imaging.paginator import SearchImageSetsPaginator

session = get_session()
async with session.create_client("medical-imaging") as client:  # (1)
    paginator: SearchImageSetsPaginator = client.get_paginator("search_image_sets")  # (2)
    async for item in paginator.paginate(...):
        item: SearchImageSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [HealthImagingClient](./client.md)
2. paginator: [SearchImageSetsPaginator](./paginators.md#searchimagesetspaginator)
3. item: [:material-code-braces: SearchImageSetsResponseTypeDef](./type_defs.md#searchimagesetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchImageSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    datastoreId: str,
    searchCriteria: SearchCriteriaTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[SearchImageSetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: SearchCriteriaTypeDef](./type_defs.md#searchcriteriatypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: SearchImageSetsResponseTypeDef](./type_defs.md#searchimagesetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchImageSetsRequestPaginateTypeDef = {  # (1)
    "datastoreId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchImageSetsRequestPaginateTypeDef](./type_defs.md#searchimagesetsrequestpaginatetypedef) 

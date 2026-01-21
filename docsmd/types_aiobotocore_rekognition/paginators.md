# Paginators

> [Index](../README.md) > [Rekognition](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Rekognition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#rekognition)
    type annotations stubs module [types-aiobotocore-rekognition](https://pypi.org/project/types-aiobotocore-rekognition/).

## DescribeProjectVersionsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("describe_project_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/DescribeProjectVersions.html#Rekognition.Paginator.DescribeProjectVersions)

```python
# DescribeProjectVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import DescribeProjectVersionsPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: DescribeProjectVersionsPaginator = client.get_paginator("describe_project_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeProjectVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [DescribeProjectVersionsPaginator](./paginators.md#describeprojectversionspaginator)
3. item: `AioPageIterator[DescribeProjectVersionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeProjectVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProjectArn: str,
    VersionNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeProjectVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeProjectVersionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeProjectVersionsRequestPaginateTypeDef = {  # (1)
    "ProjectArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeProjectVersionsRequestPaginateTypeDef](./type_defs.md#describeprojectversionsrequestpaginatetypedef)
## DescribeProjectsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("describe_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/DescribeProjects.html#Rekognition.Paginator.DescribeProjects)

```python
# DescribeProjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import DescribeProjectsPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: DescribeProjectsPaginator = client.get_paginator("describe_projects")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [DescribeProjectsPaginator](./paginators.md#describeprojectspaginator)
3. item: `AioPageIterator[DescribeProjectsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProjectNames: Sequence[str] = ...,
    Features: Sequence[CustomizationFeatureType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeProjectsResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[CustomizationFeatureType]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeProjectsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeProjectsRequestPaginateTypeDef = {  # (1)
    "ProjectNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeProjectsRequestPaginateTypeDef](./type_defs.md#describeprojectsrequestpaginatetypedef)
## ListCollectionsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_collections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/ListCollections.html#Rekognition.Paginator.ListCollections)

```python
# ListCollectionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListCollectionsPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: ListCollectionsPaginator = client.get_paginator("list_collections")  # (2)
    async for item in paginator.paginate(...):
        item: ListCollectionsResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [ListCollectionsPaginator](./paginators.md#listcollectionspaginator)
3. item: `AioPageIterator[ListCollectionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCollectionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListCollectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListCollectionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCollectionsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollectionsRequestPaginateTypeDef](./type_defs.md#listcollectionsrequestpaginatetypedef)
## ListDatasetEntriesPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_dataset_entries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/ListDatasetEntries.html#Rekognition.Paginator.ListDatasetEntries)

```python
# ListDatasetEntriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListDatasetEntriesPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetEntriesResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [ListDatasetEntriesPaginator](./paginators.md#listdatasetentriespaginator)
3. item: `AioPageIterator[ListDatasetEntriesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDatasetEntriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DatasetArn: str,
    ContainsLabels: Sequence[str] = ...,
    Labeled: bool = ...,
    SourceRefContains: str = ...,
    HasErrors: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDatasetEntriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDatasetEntriesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetEntriesRequestPaginateTypeDef = {  # (1)
    "DatasetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetEntriesRequestPaginateTypeDef](./type_defs.md#listdatasetentriesrequestpaginatetypedef)
## ListDatasetLabelsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_dataset_labels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/ListDatasetLabels.html#Rekognition.Paginator.ListDatasetLabels)

```python
# ListDatasetLabelsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListDatasetLabelsPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: ListDatasetLabelsPaginator = client.get_paginator("list_dataset_labels")  # (2)
    async for item in paginator.paginate(...):
        item: ListDatasetLabelsResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [ListDatasetLabelsPaginator](./paginators.md#listdatasetlabelspaginator)
3. item: `AioPageIterator[ListDatasetLabelsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDatasetLabelsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DatasetArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDatasetLabelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDatasetLabelsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDatasetLabelsRequestPaginateTypeDef = {  # (1)
    "DatasetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetLabelsRequestPaginateTypeDef](./type_defs.md#listdatasetlabelsrequestpaginatetypedef)
## ListFacesPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_faces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/ListFaces.html#Rekognition.Paginator.ListFaces)

```python
# ListFacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListFacesPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: ListFacesPaginator = client.get_paginator("list_faces")  # (2)
    async for item in paginator.paginate(...):
        item: ListFacesResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [ListFacesPaginator](./paginators.md#listfacespaginator)
3. item: `AioPageIterator[ListFacesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CollectionId: str,
    UserId: str = ...,
    FaceIds: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFacesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFacesRequestPaginateTypeDef = {  # (1)
    "CollectionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFacesRequestPaginateTypeDef](./type_defs.md#listfacesrequestpaginatetypedef)
## ListProjectPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_project_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/ListProjectPolicies.html#Rekognition.Paginator.ListProjectPolicies)

```python
# ListProjectPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListProjectPoliciesPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: ListProjectPoliciesPaginator = client.get_paginator("list_project_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [ListProjectPoliciesPaginator](./paginators.md#listprojectpoliciespaginator)
3. item: `AioPageIterator[ListProjectPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProjectPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProjectArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListProjectPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListProjectPoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectPoliciesRequestPaginateTypeDef = {  # (1)
    "ProjectArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectPoliciesRequestPaginateTypeDef](./type_defs.md#listprojectpoliciesrequestpaginatetypedef)
## ListStreamProcessorsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_stream_processors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/ListStreamProcessors.html#Rekognition.Paginator.ListStreamProcessors)

```python
# ListStreamProcessorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListStreamProcessorsPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: ListStreamProcessorsPaginator = client.get_paginator("list_stream_processors")  # (2)
    async for item in paginator.paginate(...):
        item: ListStreamProcessorsResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [ListStreamProcessorsPaginator](./paginators.md#liststreamprocessorspaginator)
3. item: `AioPageIterator[ListStreamProcessorsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStreamProcessorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListStreamProcessorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListStreamProcessorsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStreamProcessorsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamProcessorsRequestPaginateTypeDef](./type_defs.md#liststreamprocessorsrequestpaginatetypedef)
## ListUsersPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_users")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition/paginator/ListUsers.html#Rekognition.Paginator.ListUsers)

```python
# ListUsersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListUsersPaginator

session = get_session()
async with session.create_client("rekognition") as client:  # (1)
    paginator: ListUsersPaginator = client.get_paginator("list_users")  # (2)
    async for item in paginator.paginate(...):
        item: ListUsersResponseTypeDef
        print(item)  # (3)
```

1. client: [RekognitionClient](./client.md)
2. paginator: [ListUsersPaginator](./paginators.md#listuserspaginator)
3. item: `AioPageIterator[ListUsersResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListUsersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    CollectionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListUsersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListUsersResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListUsersRequestPaginateTypeDef = {  # (1)
    "CollectionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListUsersRequestPaginateTypeDef](./type_defs.md#listusersrequestpaginatetypedef)

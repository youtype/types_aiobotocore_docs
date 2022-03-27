# Paginators

> [Index](../README.md) > [Rekognition](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Rekognition](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition)
    type annotations stubs module [types-aiobotocore-rekognition](https://pypi.org/project/types-aiobotocore-rekognition/).

## DescribeProjectVersionsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("describe_project_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjectVersions)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import DescribeProjectVersionsPaginator

session = get_session()
async with session.create_client("rekognition") as client:
    client: RekognitionClient
    paginator: DescribeProjectVersionsPaginator = client.get_paginator("describe_project_versions")
```


### paginate

Type annotations and code completion for `#!python DescribeProjectVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProjectArn: str,
    VersionNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeProjectVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeProjectVersionsResponseTypeDef](./type_defs.md#describeprojectversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef = {  # (1)
    "ProjectArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeProjectVersionsRequestDescribeProjectVersionsPaginateTypeDef](./type_defs.md#describeprojectversionsrequestdescribeprojectversionspaginatetypedef) 
## DescribeProjectsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("describe_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.DescribeProjects)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import DescribeProjectsPaginator

session = get_session()
async with session.create_client("rekognition") as client:
    client: RekognitionClient
    paginator: DescribeProjectsPaginator = client.get_paginator("describe_projects")
```


### paginate

Type annotations and code completion for `#!python DescribeProjectsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ProjectNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeProjectsResponseTypeDef](./type_defs.md#describeprojectsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeProjectsRequestDescribeProjectsPaginateTypeDef = {  # (1)
    "ProjectNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeProjectsRequestDescribeProjectsPaginateTypeDef](./type_defs.md#describeprojectsrequestdescribeprojectspaginatetypedef) 
## ListCollectionsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_collections")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListCollections)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListCollectionsPaginator

session = get_session()
async with session.create_client("rekognition") as client:
    client: RekognitionClient
    paginator: ListCollectionsPaginator = client.get_paginator("list_collections")
```


### paginate

Type annotations and code completion for `#!python ListCollectionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCollectionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCollectionsResponseTypeDef](./type_defs.md#listcollectionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCollectionsRequestListCollectionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCollectionsRequestListCollectionsPaginateTypeDef](./type_defs.md#listcollectionsrequestlistcollectionspaginatetypedef) 
## ListDatasetEntriesPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_dataset_entries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetEntries)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListDatasetEntriesPaginator

session = get_session()
async with session.create_client("rekognition") as client:
    client: RekognitionClient
    paginator: ListDatasetEntriesPaginator = client.get_paginator("list_dataset_entries")
```


### paginate

Type annotations and code completion for `#!python ListDatasetEntriesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DatasetArn: str,
    ContainsLabels: Sequence[str] = ...,
    Labeled: bool = ...,
    SourceRefContains: str = ...,
    HasErrors: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetEntriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetEntriesResponseTypeDef](./type_defs.md#listdatasetentriesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef = {  # (1)
    "DatasetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetEntriesRequestListDatasetEntriesPaginateTypeDef](./type_defs.md#listdatasetentriesrequestlistdatasetentriespaginatetypedef) 
## ListDatasetLabelsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_dataset_labels")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListDatasetLabels)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListDatasetLabelsPaginator

session = get_session()
async with session.create_client("rekognition") as client:
    client: RekognitionClient
    paginator: ListDatasetLabelsPaginator = client.get_paginator("list_dataset_labels")
```


### paginate

Type annotations and code completion for `#!python ListDatasetLabelsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    DatasetArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDatasetLabelsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDatasetLabelsResponseTypeDef](./type_defs.md#listdatasetlabelsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef = {  # (1)
    "DatasetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDatasetLabelsRequestListDatasetLabelsPaginateTypeDef](./type_defs.md#listdatasetlabelsrequestlistdatasetlabelspaginatetypedef) 
## ListFacesPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_faces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListFaces)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListFacesPaginator

session = get_session()
async with session.create_client("rekognition") as client:
    client: RekognitionClient
    paginator: ListFacesPaginator = client.get_paginator("list_faces")
```


### paginate

Type annotations and code completion for `#!python ListFacesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    CollectionId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFacesResponseTypeDef](./type_defs.md#listfacesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListFacesRequestListFacesPaginateTypeDef = {  # (1)
    "CollectionId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFacesRequestListFacesPaginateTypeDef](./type_defs.md#listfacesrequestlistfacespaginatetypedef) 
## ListStreamProcessorsPaginator

Type annotations and code completion for `#!python session.create_client("rekognition").get_paginator("list_stream_processors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rekognition.html#Rekognition.Paginator.ListStreamProcessors)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_rekognition.paginator import ListStreamProcessorsPaginator

session = get_session()
async with session.create_client("rekognition") as client:
    client: RekognitionClient
    paginator: ListStreamProcessorsPaginator = client.get_paginator("list_stream_processors")
```


### paginate

Type annotations and code completion for `#!python ListStreamProcessorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListStreamProcessorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListStreamProcessorsResponseTypeDef](./type_defs.md#liststreamprocessorsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStreamProcessorsRequestListStreamProcessorsPaginateTypeDef](./type_defs.md#liststreamprocessorsrequestliststreamprocessorspaginatetypedef) 

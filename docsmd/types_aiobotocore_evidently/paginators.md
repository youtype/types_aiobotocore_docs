# Paginators

> [Index](../README.md) > [CloudWatchEvidently](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchEvidently](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#cloudwatchevidently)
    type annotations stubs module [types-aiobotocore-evidently](https://pypi.org/project/types-aiobotocore-evidently/).

## ListExperimentsPaginator

Type annotations and code completion for `#!python session.create_client("evidently").get_paginator("list_experiments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/paginator/ListExperiments.html#CloudWatchEvidently.Paginator.ListExperiments)

```python
# ListExperimentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListExperimentsPaginator

session = get_session()
async with session.create_client("evidently") as client:  # (1)
    paginator: ListExperimentsPaginator = client.get_paginator("list_experiments")  # (2)
    async for item in paginator.paginate(...):
        item: ListExperimentsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListExperimentsPaginator](./paginators.md#listexperimentspaginator)
3. item: [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListExperimentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    project: str,
    status: ExperimentStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListExperimentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ExperimentStatusType](./literals.md#experimentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListExperimentsResponseTypeDef](./type_defs.md#listexperimentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListExperimentsRequestPaginateTypeDef = {  # (1)
    "project": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListExperimentsRequestPaginateTypeDef](./type_defs.md#listexperimentsrequestpaginatetypedef) 
## ListFeaturesPaginator

Type annotations and code completion for `#!python session.create_client("evidently").get_paginator("list_features")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/paginator/ListFeatures.html#CloudWatchEvidently.Paginator.ListFeatures)

```python
# ListFeaturesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListFeaturesPaginator

session = get_session()
async with session.create_client("evidently") as client:  # (1)
    paginator: ListFeaturesPaginator = client.get_paginator("list_features")  # (2)
    async for item in paginator.paginate(...):
        item: ListFeaturesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListFeaturesPaginator](./paginators.md#listfeaturespaginator)
3. item: [:material-code-braces: ListFeaturesResponseTypeDef](./type_defs.md#listfeaturesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFeaturesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    project: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListFeaturesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFeaturesResponseTypeDef](./type_defs.md#listfeaturesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFeaturesRequestPaginateTypeDef = {  # (1)
    "project": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFeaturesRequestPaginateTypeDef](./type_defs.md#listfeaturesrequestpaginatetypedef) 
## ListLaunchesPaginator

Type annotations and code completion for `#!python session.create_client("evidently").get_paginator("list_launches")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/paginator/ListLaunches.html#CloudWatchEvidently.Paginator.ListLaunches)

```python
# ListLaunchesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListLaunchesPaginator

session = get_session()
async with session.create_client("evidently") as client:  # (1)
    paginator: ListLaunchesPaginator = client.get_paginator("list_launches")  # (2)
    async for item in paginator.paginate(...):
        item: ListLaunchesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListLaunchesPaginator](./paginators.md#listlaunchespaginator)
3. item: [:material-code-braces: ListLaunchesResponseTypeDef](./type_defs.md#listlaunchesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLaunchesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    project: str,
    status: LaunchStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListLaunchesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LaunchStatusType](./literals.md#launchstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListLaunchesResponseTypeDef](./type_defs.md#listlaunchesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLaunchesRequestPaginateTypeDef = {  # (1)
    "project": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLaunchesRequestPaginateTypeDef](./type_defs.md#listlaunchesrequestpaginatetypedef) 
## ListProjectsPaginator

Type annotations and code completion for `#!python session.create_client("evidently").get_paginator("list_projects")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/paginator/ListProjects.html#CloudWatchEvidently.Paginator.ListProjects)

```python
# ListProjectsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListProjectsPaginator

session = get_session()
async with session.create_client("evidently") as client:  # (1)
    paginator: ListProjectsPaginator = client.get_paginator("list_projects")  # (2)
    async for item in paginator.paginate(...):
        item: ListProjectsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListProjectsPaginator](./paginators.md#listprojectspaginator)
3. item: [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListProjectsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListProjectsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListProjectsResponseTypeDef](./type_defs.md#listprojectsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProjectsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProjectsRequestPaginateTypeDef](./type_defs.md#listprojectsrequestpaginatetypedef) 
## ListSegmentReferencesPaginator

Type annotations and code completion for `#!python session.create_client("evidently").get_paginator("list_segment_references")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/paginator/ListSegmentReferences.html#CloudWatchEvidently.Paginator.ListSegmentReferences)

```python
# ListSegmentReferencesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListSegmentReferencesPaginator

session = get_session()
async with session.create_client("evidently") as client:  # (1)
    paginator: ListSegmentReferencesPaginator = client.get_paginator("list_segment_references")  # (2)
    async for item in paginator.paginate(...):
        item: ListSegmentReferencesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListSegmentReferencesPaginator](./paginators.md#listsegmentreferencespaginator)
3. item: [:material-code-braces: ListSegmentReferencesResponseTypeDef](./type_defs.md#listsegmentreferencesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSegmentReferencesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    segment: str,
    type: SegmentReferenceResourceTypeType,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListSegmentReferencesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SegmentReferenceResourceTypeType](./literals.md#segmentreferenceresourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSegmentReferencesResponseTypeDef](./type_defs.md#listsegmentreferencesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSegmentReferencesRequestPaginateTypeDef = {  # (1)
    "segment": ...,
    "type": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSegmentReferencesRequestPaginateTypeDef](./type_defs.md#listsegmentreferencesrequestpaginatetypedef) 
## ListSegmentsPaginator

Type annotations and code completion for `#!python session.create_client("evidently").get_paginator("list_segments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently/paginator/ListSegments.html#CloudWatchEvidently.Paginator.ListSegments)

```python
# ListSegmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_evidently.paginator import ListSegmentsPaginator

session = get_session()
async with session.create_client("evidently") as client:  # (1)
    paginator: ListSegmentsPaginator = client.get_paginator("list_segments")  # (2)
    async for item in paginator.paginate(...):
        item: ListSegmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchEvidentlyClient](./client.md)
2. paginator: [ListSegmentsPaginator](./paginators.md#listsegmentspaginator)
3. item: [:material-code-braces: ListSegmentsResponseTypeDef](./type_defs.md#listsegmentsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSegmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListSegmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSegmentsResponseTypeDef](./type_defs.md#listsegmentsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSegmentsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSegmentsRequestPaginateTypeDef](./type_defs.md#listsegmentsrequestpaginatetypedef) 

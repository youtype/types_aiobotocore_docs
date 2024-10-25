# Paginators

> [Index](../README.md) > [MediaConvert](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [MediaConvert](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
    type annotations stubs module [types-aiobotocore-mediaconvert](https://pypi.org/project/types-aiobotocore-mediaconvert/).

## DescribeEndpointsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconvert").get_paginator("describe_endpoints")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints)

```python
# DescribeEndpointsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import DescribeEndpointsPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:  # (1)
    paginator: DescribeEndpointsPaginator = client.get_paginator("describe_endpoints")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEndpointsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [DescribeEndpointsPaginator](./paginators.md#describeendpointspaginator)
3. item: [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEndpointsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Mode: DescribeEndpointsModeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEndpointsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DescribeEndpointsModeType](./literals.md#describeendpointsmodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef = {  # (1)
    "Mode": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef](./type_defs.md#describeendpointsrequestdescribeendpointspaginatetypedef) 
## ListJobTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("mediaconvert").get_paginator("list_job_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates)

```python
# ListJobTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListJobTemplatesPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:  # (1)
    paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [ListJobTemplatesPaginator](./paginators.md#listjobtemplatespaginator)
3. item: [:material-code-braces: ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Category: str = ...,
    ListBy: JobTemplateListByType = ...,  # (1)
    Order: OrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListJobTemplatesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: JobTemplateListByType](./literals.md#jobtemplatelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = {  # (1)
    "Category": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobTemplatesRequestListJobTemplatesPaginateTypeDef](./type_defs.md#listjobtemplatesrequestlistjobtemplatespaginatetypedef) 
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconvert").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Order: OrderType = ...,  # (1)
    Queue: str = ...,
    Status: JobStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestListJobsPaginateTypeDef = {  # (1)
    "Order": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestListJobsPaginateTypeDef](./type_defs.md#listjobsrequestlistjobspaginatetypedef) 
## ListPresetsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconvert").get_paginator("list_presets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets)

```python
# ListPresetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListPresetsPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:  # (1)
    paginator: ListPresetsPaginator = client.get_paginator("list_presets")  # (2)
    async for item in paginator.paginate(...):
        item: ListPresetsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [ListPresetsPaginator](./paginators.md#listpresetspaginator)
3. item: [:material-code-braces: ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListPresetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Category: str = ...,
    ListBy: PresetListByType = ...,  # (1)
    Order: OrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListPresetsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: PresetListByType](./literals.md#presetlistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPresetsRequestListPresetsPaginateTypeDef = {  # (1)
    "Category": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPresetsRequestListPresetsPaginateTypeDef](./type_defs.md#listpresetsrequestlistpresetspaginatetypedef) 
## ListQueuesPaginator

Type annotations and code completion for `#!python session.create_client("mediaconvert").get_paginator("list_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues)

```python
# ListQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListQueuesPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:  # (1)
    paginator: ListQueuesPaginator = client.get_paginator("list_queues")  # (2)
    async for item in paginator.paginate(...):
        item: ListQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [ListQueuesPaginator](./paginators.md#listqueuespaginator)
3. item: [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ListBy: QueueListByType = ...,  # (1)
    Order: OrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[ListQueuesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: QueueListByType](./literals.md#queuelistbytype) 
2. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListQueuesRequestListQueuesPaginateTypeDef = {  # (1)
    "ListBy": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListQueuesRequestListQueuesPaginateTypeDef](./type_defs.md#listqueuesrequestlistqueuespaginatetypedef) 
## ListVersionsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconvert").get_paginator("list_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListVersions)

```python
# ListVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListVersionsPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:  # (1)
    paginator: ListVersionsPaginator = client.get_paginator("list_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListVersionsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [ListVersionsPaginator](./paginators.md#listversionspaginator)
3. item: [:material-code-braces: ListVersionsResponseTypeDef](./type_defs.md#listversionsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVersionsResponseTypeDef](./type_defs.md#listversionsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVersionsRequestListVersionsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVersionsRequestListVersionsPaginateTypeDef](./type_defs.md#listversionsrequestlistversionspaginatetypedef) 
## SearchJobsPaginator

Type annotations and code completion for `#!python session.create_client("mediaconvert").get_paginator("search_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.SearchJobs)

```python
# SearchJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import SearchJobsPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:  # (1)
    paginator: SearchJobsPaginator = client.get_paginator("search_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: SearchJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [MediaConvertClient](./client.md)
2. paginator: [SearchJobsPaginator](./paginators.md#searchjobspaginator)
3. item: [:material-code-braces: SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SearchJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    InputFile: str = ...,
    Order: OrderType = ...,  # (1)
    Queue: str = ...,
    Status: JobStatusType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AsyncIterator[SearchJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: SearchJobsResponseTypeDef](./type_defs.md#searchjobsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SearchJobsRequestSearchJobsPaginateTypeDef = {  # (1)
    "InputFile": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SearchJobsRequestSearchJobsPaginateTypeDef](./type_defs.md#searchjobsrequestsearchjobspaginatetypedef) 

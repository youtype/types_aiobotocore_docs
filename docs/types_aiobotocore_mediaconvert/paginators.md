<a id="paginators-for-aiobotocore-mediaconvert-module"></a>

# Paginators for aiobotocore MediaConvert module

> [Index](../README.md) > [MediaConvert](./README.md) > Paginators

Auto-generated documentation for
[MediaConvert](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert)
type annotations stubs module
[types-aiobotocore-mediaconvert](https://pypi.org/project/types-aiobotocore-mediaconvert/).

- [Paginators for aiobotocore MediaConvert module](#paginators-for-aiobotocore-mediaconvert-module)
  - [DescribeEndpointsPaginator](#describeendpointspaginator)
  - [ListJobTemplatesPaginator](#listjobtemplatespaginator)
  - [ListJobsPaginator](#listjobspaginator)
  - [ListPresetsPaginator](#listpresetspaginator)
  - [ListQueuesPaginator](#listqueuespaginator)

<a id="describeendpointspaginator"></a>

## DescribeEndpointsPaginator

Type annotations for
`session.create_client("mediaconvert").get_paginator("describe_endpoints")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import DescribeEndpointsPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:
    client: MediaConvertClient
    paginator: DescribeEndpointsPaginator = client.get_paginator("describe_endpoints")
```

Boto3 documentation:
[MediaConvert.Paginator.DescribeEndpoints](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.DescribeEndpoints)

Arguments for `DescribeEndpointsPaginator.paginate` method:

- `Mode`: [DescribeEndpointsModeType](./literals.md#describeendpointsmodetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEndpointsPaginator.paginate` returns
`AsyncIterator`\[[DescribeEndpointsResponseTypeDef](./type_defs.md#describeendpointsresponsetypedef)\].

<a id="listjobtemplatespaginator"></a>

## ListJobTemplatesPaginator

Type annotations for
`session.create_client("mediaconvert").get_paginator("list_job_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListJobTemplatesPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:
    client: MediaConvertClient
    paginator: ListJobTemplatesPaginator = client.get_paginator("list_job_templates")
```

Boto3 documentation:
[MediaConvert.Paginator.ListJobTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobTemplates)

Arguments for `ListJobTemplatesPaginator.paginate` method:

- `Category`: `str`
- `ListBy`: [JobTemplateListByType](./literals.md#jobtemplatelistbytype)
- `Order`: [OrderType](./literals.md#ordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobTemplatesPaginator.paginate` returns
`AsyncIterator`\[[ListJobTemplatesResponseTypeDef](./type_defs.md#listjobtemplatesresponsetypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`session.create_client("mediaconvert").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:
    client: MediaConvertClient
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")
```

Boto3 documentation:
[MediaConvert.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `Order`: [OrderType](./literals.md#ordertype)
- `Queue`: `str`
- `Status`: [JobStatusType](./literals.md#jobstatustype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`AsyncIterator`\[[ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef)\].

<a id="listpresetspaginator"></a>

## ListPresetsPaginator

Type annotations for
`session.create_client("mediaconvert").get_paginator("list_presets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListPresetsPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:
    client: MediaConvertClient
    paginator: ListPresetsPaginator = client.get_paginator("list_presets")
```

Boto3 documentation:
[MediaConvert.Paginator.ListPresets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListPresets)

Arguments for `ListPresetsPaginator.paginate` method:

- `Category`: `str`
- `ListBy`: [PresetListByType](./literals.md#presetlistbytype)
- `Order`: [OrderType](./literals.md#ordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListPresetsPaginator.paginate` returns
`AsyncIterator`\[[ListPresetsResponseTypeDef](./type_defs.md#listpresetsresponsetypedef)\].

<a id="listqueuespaginator"></a>

## ListQueuesPaginator

Type annotations for
`session.create_client("mediaconvert").get_paginator("list_queues")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_mediaconvert.paginator import ListQueuesPaginator

session = get_session()
async with session.create_client("mediaconvert") as client:
    client: MediaConvertClient
    paginator: ListQueuesPaginator = client.get_paginator("list_queues")
```

Boto3 documentation:
[MediaConvert.Paginator.ListQueues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Paginator.ListQueues)

Arguments for `ListQueuesPaginator.paginate` method:

- `ListBy`: [QueueListByType](./literals.md#queuelistbytype)
- `Order`: [OrderType](./literals.md#ordertype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListQueuesPaginator.paginate` returns
`AsyncIterator`\[[ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef)\].

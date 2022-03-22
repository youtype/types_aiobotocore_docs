<a id="paginators-for-aiobotocore-dax-module"></a>

# Paginators for aiobotocore DAX module

> [Index](../README.md) > [DAX](./README.md) > Paginators

Auto-generated documentation for
[DAX](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
type annotations stubs module
[types-aiobotocore-dax](https://pypi.org/project/types-aiobotocore-dax/).

- [Paginators for aiobotocore DAX module](#paginators-for-aiobotocore-dax-module)
  - [DescribeClustersPaginator](#describeclusterspaginator)
  - [DescribeDefaultParametersPaginator](#describedefaultparameterspaginator)
  - [DescribeEventsPaginator](#describeeventspaginator)
  - [DescribeParameterGroupsPaginator](#describeparametergroupspaginator)
  - [DescribeParametersPaginator](#describeparameterspaginator)
  - [DescribeSubnetGroupsPaginator](#describesubnetgroupspaginator)
  - [ListTagsPaginator](#listtagspaginator)

<a id="describeclusterspaginator"></a>

## DescribeClustersPaginator

Type annotations for
`session.create_client("dax").get_paginator("describe_clusters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeClustersPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
```

Boto3 documentation:
[DAX.Paginator.DescribeClusters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters)

Arguments for `DescribeClustersPaginator.paginate` method:

- `ClusterNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeClustersPaginator.paginate` returns
`AsyncIterator`\[[DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef)\].

<a id="describedefaultparameterspaginator"></a>

## DescribeDefaultParametersPaginator

Type annotations for
`session.create_client("dax").get_paginator("describe_default_parameters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeDefaultParametersPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeDefaultParametersPaginator = client.get_paginator("describe_default_parameters")
```

Boto3 documentation:
[DAX.Paginator.DescribeDefaultParameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters)

Arguments for `DescribeDefaultParametersPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDefaultParametersPaginator.paginate` returns
`AsyncIterator`\[[DescribeDefaultParametersResponseTypeDef](./type_defs.md#describedefaultparametersresponsetypedef)\].

<a id="describeeventspaginator"></a>

## DescribeEventsPaginator

Type annotations for
`session.create_client("dax").get_paginator("describe_events")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
```

Boto3 documentation:
[DAX.Paginator.DescribeEvents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents)

Arguments for `DescribeEventsPaginator.paginate` method:

- `SourceName`: `str`
- `SourceType`: [SourceTypeType](./literals.md#sourcetypetype)
- `StartTime`: `Union`\[`datetime`, `str`\]
- `EndTime`: `Union`\[`datetime`, `str`\]
- `Duration`: `int`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeEventsPaginator.paginate` returns
`AsyncIterator`\[[DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef)\].

<a id="describeparametergroupspaginator"></a>

## DescribeParameterGroupsPaginator

Type annotations for
`session.create_client("dax").get_paginator("describe_parameter_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeParameterGroupsPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeParameterGroupsPaginator = client.get_paginator("describe_parameter_groups")
```

Boto3 documentation:
[DAX.Paginator.DescribeParameterGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups)

Arguments for `DescribeParameterGroupsPaginator.paginate` method:

- `ParameterGroupNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeParameterGroupsPaginator.paginate` returns
`AsyncIterator`\[[DescribeParameterGroupsResponseTypeDef](./type_defs.md#describeparametergroupsresponsetypedef)\].

<a id="describeparameterspaginator"></a>

## DescribeParametersPaginator

Type annotations for
`session.create_client("dax").get_paginator("describe_parameters")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeParametersPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeParametersPaginator = client.get_paginator("describe_parameters")
```

Boto3 documentation:
[DAX.Paginator.DescribeParameters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters)

Arguments for `DescribeParametersPaginator.paginate` method:

- `ParameterGroupName`: `str` *(required)*
- `Source`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeParametersPaginator.paginate` returns
`AsyncIterator`\[[DescribeParametersResponseTypeDef](./type_defs.md#describeparametersresponsetypedef)\].

<a id="describesubnetgroupspaginator"></a>

## DescribeSubnetGroupsPaginator

Type annotations for
`session.create_client("dax").get_paginator("describe_subnet_groups")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeSubnetGroupsPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeSubnetGroupsPaginator = client.get_paginator("describe_subnet_groups")
```

Boto3 documentation:
[DAX.Paginator.DescribeSubnetGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups)

Arguments for `DescribeSubnetGroupsPaginator.paginate` method:

- `SubnetGroupNames`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeSubnetGroupsPaginator.paginate` returns
`AsyncIterator`\[[DescribeSubnetGroupsResponseTypeDef](./type_defs.md#describesubnetgroupsresponsetypedef)\].

<a id="listtagspaginator"></a>

## ListTagsPaginator

Type annotations for `session.create_client("dax").get_paginator("list_tags")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: ListTagsPaginator = client.get_paginator("list_tags")
```

Boto3 documentation:
[DAX.Paginator.ListTags](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags)

Arguments for `ListTagsPaginator.paginate` method:

- `ResourceName`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTagsPaginator.paginate` returns
`AsyncIterator`\[[ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef)\].

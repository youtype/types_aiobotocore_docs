# Paginators

> [Index](../README.md) > [DAX](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [DAX](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
    type annotations stubs module [types-aiobotocore-dax](https://pypi.org/project/types-aiobotocore-dax/).

## DescribeClustersPaginator

Type annotations and code completion for `#!python session.create_client("dax").get_paginator("describe_clusters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeClustersPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeClustersPaginator = client.get_paginator("describe_clusters")
```


### paginate

Type annotations and code completion for `#!python DescribeClustersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ClusterNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeClustersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeClustersResponseTypeDef](./type_defs.md#describeclustersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeClustersRequestDescribeClustersPaginateTypeDef = {  # (1)
    "ClusterNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeClustersRequestDescribeClustersPaginateTypeDef](./type_defs.md#describeclustersrequestdescribeclusterspaginatetypedef) 
## DescribeDefaultParametersPaginator

Type annotations and code completion for `#!python session.create_client("dax").get_paginator("describe_default_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeDefaultParametersPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeDefaultParametersPaginator = client.get_paginator("describe_default_parameters")
```


### paginate

Type annotations and code completion for `#!python DescribeDefaultParametersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeDefaultParametersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDefaultParametersResponseTypeDef](./type_defs.md#describedefaultparametersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef](./type_defs.md#describedefaultparametersrequestdescribedefaultparameterspaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("dax").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")
```


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SourceName: str = ...,
    SourceType: SourceTypeType = ...,  # (1)
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    Duration: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[DescribeEventsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventsRequestDescribeEventsPaginateTypeDef = {  # (1)
    "SourceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsRequestDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsrequestdescribeeventspaginatetypedef) 
## DescribeParameterGroupsPaginator

Type annotations and code completion for `#!python session.create_client("dax").get_paginator("describe_parameter_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeParameterGroupsPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeParameterGroupsPaginator = client.get_paginator("describe_parameter_groups")
```


### paginate

Type annotations and code completion for `#!python DescribeParameterGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ParameterGroupNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeParameterGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeParameterGroupsResponseTypeDef](./type_defs.md#describeparametergroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = {  # (1)
    "ParameterGroupNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef](./type_defs.md#describeparametergroupsrequestdescribeparametergroupspaginatetypedef) 
## DescribeParametersPaginator

Type annotations and code completion for `#!python session.create_client("dax").get_paginator("describe_parameters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeParametersPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeParametersPaginator = client.get_paginator("describe_parameters")
```


### paginate

Type annotations and code completion for `#!python DescribeParametersPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ParameterGroupName: str,
    Source: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeParametersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeParametersResponseTypeDef](./type_defs.md#describeparametersresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeParametersRequestDescribeParametersPaginateTypeDef = {  # (1)
    "ParameterGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeParametersRequestDescribeParametersPaginateTypeDef](./type_defs.md#describeparametersrequestdescribeparameterspaginatetypedef) 
## DescribeSubnetGroupsPaginator

Type annotations and code completion for `#!python session.create_client("dax").get_paginator("describe_subnet_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import DescribeSubnetGroupsPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: DescribeSubnetGroupsPaginator = client.get_paginator("describe_subnet_groups")
```


### paginate

Type annotations and code completion for `#!python DescribeSubnetGroupsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    SubnetGroupNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSubnetGroupsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSubnetGroupsResponseTypeDef](./type_defs.md#describesubnetgroupsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = {  # (1)
    "SubnetGroupNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef](./type_defs.md#describesubnetgroupsrequestdescribesubnetgroupspaginatetypedef) 
## ListTagsPaginator

Type annotations and code completion for `#!python session.create_client("dax").get_paginator("list_tags")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_dax.paginator import ListTagsPaginator

session = get_session()
async with session.create_client("dax") as client:
    client: DAXClient
    paginator: ListTagsPaginator = client.get_paginator("list_tags")
```


### paginate

Type annotations and code completion for `#!python ListTagsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    ResourceName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsResponseTypeDef](./type_defs.md#listtagsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsRequestListTagsPaginateTypeDef = {  # (1)
    "ResourceName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsRequestListTagsPaginateTypeDef](./type_defs.md#listtagsrequestlisttagspaginatetypedef) 

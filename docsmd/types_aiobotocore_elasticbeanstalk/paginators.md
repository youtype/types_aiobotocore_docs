# Paginators

> [Index](../README.md) > [ElasticBeanstalk](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticBeanstalk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#elasticbeanstalk)
    type annotations stubs module [types-aiobotocore-elasticbeanstalk](https://pypi.org/project/types-aiobotocore-elasticbeanstalk/).

## DescribeApplicationVersionsPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("describe_application_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk/paginator/DescribeApplicationVersions.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions)

```python
# DescribeApplicationVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.paginator import DescribeApplicationVersionsPaginator

session = get_session()
async with session.create_client("elasticbeanstalk") as client:  # (1)
    paginator: DescribeApplicationVersionsPaginator = client.get_paginator("describe_application_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ApplicationVersionDescriptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [ElasticBeanstalkClient](./client.md)
2. paginator: [DescribeApplicationVersionsPaginator](./paginators.md#describeapplicationversionspaginator)
3. item: [:material-code-braces: ApplicationVersionDescriptionsMessageTypeDef](./type_defs.md#applicationversiondescriptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeApplicationVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationName: str = ...,
    VersionLabels: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ApplicationVersionDescriptionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ApplicationVersionDescriptionsMessageTypeDef](./type_defs.md#applicationversiondescriptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeApplicationVersionsMessagePaginateTypeDef = {  # (1)
    "ApplicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationVersionsMessagePaginateTypeDef](./type_defs.md#describeapplicationversionsmessagepaginatetypedef) 
## DescribeEnvironmentManagedActionHistoryPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("describe_environment_managed_action_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk/paginator/DescribeEnvironmentManagedActionHistory.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory)

```python
# DescribeEnvironmentManagedActionHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.paginator import DescribeEnvironmentManagedActionHistoryPaginator

session = get_session()
async with session.create_client("elasticbeanstalk") as client:  # (1)
    paginator: DescribeEnvironmentManagedActionHistoryPaginator = client.get_paginator("describe_environment_managed_action_history")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeEnvironmentManagedActionHistoryResultTypeDef
        print(item)  # (3)
```

1. client: [ElasticBeanstalkClient](./client.md)
2. paginator: [DescribeEnvironmentManagedActionHistoryPaginator](./paginators.md#describeenvironmentmanagedactionhistorypaginator)
3. item: [:material-code-braces: DescribeEnvironmentManagedActionHistoryResultTypeDef](./type_defs.md#describeenvironmentmanagedactionhistoryresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEnvironmentManagedActionHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    EnvironmentId: str = ...,
    EnvironmentName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeEnvironmentManagedActionHistoryResultTypeDef](./type_defs.md#describeenvironmentmanagedactionhistoryresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEnvironmentManagedActionHistoryRequestPaginateTypeDef = {  # (1)
    "EnvironmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEnvironmentManagedActionHistoryRequestPaginateTypeDef](./type_defs.md#describeenvironmentmanagedactionhistoryrequestpaginatetypedef) 
## DescribeEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("describe_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk/paginator/DescribeEnvironments.html#ElasticBeanstalk.Paginator.DescribeEnvironments)

```python
# DescribeEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.paginator import DescribeEnvironmentsPaginator

session = get_session()
async with session.create_client("elasticbeanstalk") as client:  # (1)
    paginator: DescribeEnvironmentsPaginator = client.get_paginator("describe_environments")  # (2)
    async for item in paginator.paginate(...):
        item: EnvironmentDescriptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [ElasticBeanstalkClient](./client.md)
2. paginator: [DescribeEnvironmentsPaginator](./paginators.md#describeenvironmentspaginator)
3. item: [:material-code-braces: EnvironmentDescriptionsMessageTypeDef](./type_defs.md#environmentdescriptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationName: str = ...,
    VersionLabel: str = ...,
    EnvironmentIds: Sequence[str] = ...,
    EnvironmentNames: Sequence[str] = ...,
    IncludeDeleted: bool = ...,
    IncludedDeletedBackTo: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[EnvironmentDescriptionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: EnvironmentDescriptionsMessageTypeDef](./type_defs.md#environmentdescriptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEnvironmentsMessagePaginateTypeDef = {  # (1)
    "ApplicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEnvironmentsMessagePaginateTypeDef](./type_defs.md#describeenvironmentsmessagepaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk/paginator/DescribeEvents.html#ElasticBeanstalk.Paginator.DescribeEvents)

```python
# DescribeEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.paginator import DescribeEventsPaginator

session = get_session()
async with session.create_client("elasticbeanstalk") as client:  # (1)
    paginator: DescribeEventsPaginator = client.get_paginator("describe_events")  # (2)
    async for item in paginator.paginate(...):
        item: EventDescriptionsMessageTypeDef
        print(item)  # (3)
```

1. client: [ElasticBeanstalkClient](./client.md)
2. paginator: [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
3. item: [:material-code-braces: EventDescriptionsMessageTypeDef](./type_defs.md#eventdescriptionsmessagetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ApplicationName: str = ...,
    VersionLabel: str = ...,
    TemplateName: str = ...,
    EnvironmentId: str = ...,
    EnvironmentName: str = ...,
    PlatformArn: str = ...,
    RequestId: str = ...,
    Severity: EventSeverityType = ...,  # (1)
    StartTime: TimestampTypeDef = ...,
    EndTime: TimestampTypeDef = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[EventDescriptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EventSeverityType](./literals.md#eventseveritytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: EventDescriptionsMessageTypeDef](./type_defs.md#eventdescriptionsmessagetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeEventsMessagePaginateTypeDef = {  # (1)
    "ApplicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessagePaginateTypeDef](./type_defs.md#describeeventsmessagepaginatetypedef) 
## ListPlatformVersionsPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("list_platform_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk/paginator/ListPlatformVersions.html#ElasticBeanstalk.Paginator.ListPlatformVersions)

```python
# ListPlatformVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_elasticbeanstalk.paginator import ListPlatformVersionsPaginator

session = get_session()
async with session.create_client("elasticbeanstalk") as client:  # (1)
    paginator: ListPlatformVersionsPaginator = client.get_paginator("list_platform_versions")  # (2)
    async for item in paginator.paginate(...):
        item: ListPlatformVersionsResultTypeDef
        print(item)  # (3)
```

1. client: [ElasticBeanstalkClient](./client.md)
2. paginator: [ListPlatformVersionsPaginator](./paginators.md#listplatformversionspaginator)
3. item: [:material-code-braces: ListPlatformVersionsResultTypeDef](./type_defs.md#listplatformversionsresulttypedef) 


### paginate

Type annotations and code completion for `#!python ListPlatformVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[PlatformFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListPlatformVersionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: PlatformFilterTypeDef](./type_defs.md#platformfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPlatformVersionsResultTypeDef](./type_defs.md#listplatformversionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPlatformVersionsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlatformVersionsRequestPaginateTypeDef](./type_defs.md#listplatformversionsrequestpaginatetypedef) 

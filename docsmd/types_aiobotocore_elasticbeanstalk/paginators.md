# Paginators

> [Index](../README.md) > [ElasticBeanstalk](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ElasticBeanstalk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk)
    type annotations stubs module [types-aiobotocore-elasticbeanstalk](https://pypi.org/project/types-aiobotocore-elasticbeanstalk/).

## DescribeApplicationVersionsPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("describe_application_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeApplicationVersions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    ApplicationName: str = ...,
    VersionLabels: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ApplicationVersionDescriptionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ApplicationVersionDescriptionsMessageTypeDef](./type_defs.md#applicationversiondescriptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef = {  # (1)
    "ApplicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeApplicationVersionsMessageDescribeApplicationVersionsPaginateTypeDef](./type_defs.md#describeapplicationversionsmessagedescribeapplicationversionspaginatetypedef) 
## DescribeEnvironmentManagedActionHistoryPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("describe_environment_managed_action_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironmentManagedActionHistory)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    EnvironmentId: str = ...,
    EnvironmentName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeEnvironmentManagedActionHistoryResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeEnvironmentManagedActionHistoryResultTypeDef](./type_defs.md#describeenvironmentmanagedactionhistoryresulttypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef = {  # (1)
    "EnvironmentId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEnvironmentManagedActionHistoryRequestDescribeEnvironmentManagedActionHistoryPaginateTypeDef](./type_defs.md#describeenvironmentmanagedactionhistoryrequestdescribeenvironmentmanagedactionhistorypaginatetypedef) 
## DescribeEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("describe_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEnvironments)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    ApplicationName: str = ...,
    VersionLabel: str = ...,
    EnvironmentIds: Sequence[str] = ...,
    EnvironmentNames: Sequence[str] = ...,
    IncludeDeleted: bool = ...,
    IncludedDeletedBackTo: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[EnvironmentDescriptionsMessageTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: EnvironmentDescriptionsMessageTypeDef](./type_defs.md#environmentdescriptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef = {  # (1)
    "ApplicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEnvironmentsMessageDescribeEnvironmentsPaginateTypeDef](./type_defs.md#describeenvironmentsmessagedescribeenvironmentspaginatetypedef) 
## DescribeEventsPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("describe_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.DescribeEvents)

```python title="Usage example"
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

```python title="Method definition"
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
    StartTime: Union[datetime, str] = ...,
    EndTime: Union[datetime, str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[EventDescriptionsMessageTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: EventSeverityType](./literals.md#eventseveritytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: EventDescriptionsMessageTypeDef](./type_defs.md#eventdescriptionsmessagetypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeEventsMessageDescribeEventsPaginateTypeDef = {  # (1)
    "ApplicationName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeEventsMessageDescribeEventsPaginateTypeDef](./type_defs.md#describeeventsmessagedescribeeventspaginatetypedef) 
## ListPlatformVersionsPaginator

Type annotations and code completion for `#!python session.create_client("elasticbeanstalk").get_paginator("list_platform_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk.Paginator.ListPlatformVersions)

```python title="Usage example"
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

```python title="Method definition"
def paginate(
    self,
    *,
    Filters: Sequence[PlatformFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPlatformVersionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: PlatformFilterTypeDef](./type_defs.md#platformfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPlatformVersionsResultTypeDef](./type_defs.md#listplatformversionsresulttypedef) 


```python title="Usage example with kwargs"
kwargs: ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPlatformVersionsRequestListPlatformVersionsPaginateTypeDef](./type_defs.md#listplatformversionsrequestlistplatformversionspaginatetypedef) 

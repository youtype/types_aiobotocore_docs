# Paginators

> [Index](../README.md) > [CloudWatchLogs](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [CloudWatchLogs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs.html#cloudwatchlogs)
    type annotations stubs module [types-aiobotocore-logs](https://pypi.org/project/types-aiobotocore-logs/).

## DescribeConfigurationTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_configuration_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeConfigurationTemplates.html#CloudWatchLogs.Paginator.DescribeConfigurationTemplates)

```python
# DescribeConfigurationTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeConfigurationTemplatesPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeConfigurationTemplatesPaginator = client.get_paginator("describe_configuration_templates")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigurationTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeConfigurationTemplatesPaginator](./paginators.md#describeconfigurationtemplatespaginator)
3. item: [:material-code-braces: DescribeConfigurationTemplatesResponseTypeDef](./type_defs.md#describeconfigurationtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigurationTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    service: str = ...,
    logTypes: Sequence[str] = ...,
    resourceTypes: Sequence[str] = ...,
    deliveryDestinationTypes: Sequence[DeliveryDestinationTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeConfigurationTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeConfigurationTemplatesResponseTypeDef](./type_defs.md#describeconfigurationtemplatesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConfigurationTemplatesRequestPaginateTypeDef = {  # (1)
    "service": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationTemplatesRequestPaginateTypeDef](./type_defs.md#describeconfigurationtemplatesrequestpaginatetypedef) 
## DescribeDeliveriesPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_deliveries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeDeliveries.html#CloudWatchLogs.Paginator.DescribeDeliveries)

```python
# DescribeDeliveriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeDeliveriesPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeDeliveriesPaginator = client.get_paginator("describe_deliveries")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDeliveriesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeDeliveriesPaginator](./paginators.md#describedeliveriespaginator)
3. item: [:material-code-braces: DescribeDeliveriesResponseTypeDef](./type_defs.md#describedeliveriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDeliveriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDeliveriesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDeliveriesResponseTypeDef](./type_defs.md#describedeliveriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDeliveriesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDeliveriesRequestPaginateTypeDef](./type_defs.md#describedeliveriesrequestpaginatetypedef) 
## DescribeDeliveryDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_delivery_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeDeliveryDestinations.html#CloudWatchLogs.Paginator.DescribeDeliveryDestinations)

```python
# DescribeDeliveryDestinationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeDeliveryDestinationsPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeDeliveryDestinationsPaginator = client.get_paginator("describe_delivery_destinations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDeliveryDestinationsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeDeliveryDestinationsPaginator](./paginators.md#describedeliverydestinationspaginator)
3. item: [:material-code-braces: DescribeDeliveryDestinationsResponseTypeDef](./type_defs.md#describedeliverydestinationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDeliveryDestinationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDeliveryDestinationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDeliveryDestinationsResponseTypeDef](./type_defs.md#describedeliverydestinationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDeliveryDestinationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDeliveryDestinationsRequestPaginateTypeDef](./type_defs.md#describedeliverydestinationsrequestpaginatetypedef) 
## DescribeDeliverySourcesPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_delivery_sources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeDeliverySources.html#CloudWatchLogs.Paginator.DescribeDeliverySources)

```python
# DescribeDeliverySourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeDeliverySourcesPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeDeliverySourcesPaginator = client.get_paginator("describe_delivery_sources")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDeliverySourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeDeliverySourcesPaginator](./paginators.md#describedeliverysourcespaginator)
3. item: [:material-code-braces: DescribeDeliverySourcesResponseTypeDef](./type_defs.md#describedeliverysourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDeliverySourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDeliverySourcesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDeliverySourcesResponseTypeDef](./type_defs.md#describedeliverysourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDeliverySourcesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDeliverySourcesRequestPaginateTypeDef](./type_defs.md#describedeliverysourcesrequestpaginatetypedef) 
## DescribeDestinationsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_destinations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeDestinations.html#CloudWatchLogs.Paginator.DescribeDestinations)

```python
# DescribeDestinationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeDestinationsPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeDestinationsPaginator = client.get_paginator("describe_destinations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeDestinationsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeDestinationsPaginator](./paginators.md#describedestinationspaginator)
3. item: [:material-code-braces: DescribeDestinationsResponseTypeDef](./type_defs.md#describedestinationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeDestinationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    DestinationNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeDestinationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeDestinationsResponseTypeDef](./type_defs.md#describedestinationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeDestinationsRequestPaginateTypeDef = {  # (1)
    "DestinationNamePrefix": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeDestinationsRequestPaginateTypeDef](./type_defs.md#describedestinationsrequestpaginatetypedef) 
## DescribeExportTasksPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_export_tasks")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeExportTasks.html#CloudWatchLogs.Paginator.DescribeExportTasks)

```python
# DescribeExportTasksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeExportTasksPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeExportTasksPaginator = client.get_paginator("describe_export_tasks")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeExportTasksResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeExportTasksPaginator](./paginators.md#describeexporttaskspaginator)
3. item: [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeExportTasksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    taskId: str = ...,
    statusCode: ExportTaskStatusCodeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeExportTasksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ExportTaskStatusCodeType](./literals.md#exporttaskstatuscodetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeExportTasksResponseTypeDef](./type_defs.md#describeexporttasksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeExportTasksRequestPaginateTypeDef = {  # (1)
    "taskId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeExportTasksRequestPaginateTypeDef](./type_defs.md#describeexporttasksrequestpaginatetypedef) 
## DescribeLogGroupsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_log_groups")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeLogGroups.html#CloudWatchLogs.Paginator.DescribeLogGroups)

```python
# DescribeLogGroupsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeLogGroupsPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeLogGroupsPaginator = client.get_paginator("describe_log_groups")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLogGroupsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeLogGroupsPaginator](./paginators.md#describeloggroupspaginator)
3. item: [:material-code-braces: DescribeLogGroupsResponseTypeDef](./type_defs.md#describeloggroupsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLogGroupsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    accountIdentifiers: Sequence[str] = ...,
    logGroupNamePrefix: str = ...,
    logGroupNamePattern: str = ...,
    includeLinkedAccounts: bool = ...,
    logGroupClass: LogGroupClassType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeLogGroupsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LogGroupClassType](./literals.md#loggroupclasstype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLogGroupsResponseTypeDef](./type_defs.md#describeloggroupsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLogGroupsRequestPaginateTypeDef = {  # (1)
    "accountIdentifiers": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLogGroupsRequestPaginateTypeDef](./type_defs.md#describeloggroupsrequestpaginatetypedef) 
## DescribeLogStreamsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_log_streams")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeLogStreams.html#CloudWatchLogs.Paginator.DescribeLogStreams)

```python
# DescribeLogStreamsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeLogStreamsPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeLogStreamsPaginator = client.get_paginator("describe_log_streams")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeLogStreamsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeLogStreamsPaginator](./paginators.md#describelogstreamspaginator)
3. item: [:material-code-braces: DescribeLogStreamsResponseTypeDef](./type_defs.md#describelogstreamsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeLogStreamsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    logGroupName: str = ...,
    logGroupIdentifier: str = ...,
    logStreamNamePrefix: str = ...,
    orderBy: OrderByType = ...,  # (1)
    descending: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeLogStreamsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OrderByType](./literals.md#orderbytype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeLogStreamsResponseTypeDef](./type_defs.md#describelogstreamsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeLogStreamsRequestPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeLogStreamsRequestPaginateTypeDef](./type_defs.md#describelogstreamsrequestpaginatetypedef) 
## DescribeMetricFiltersPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_metric_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeMetricFilters.html#CloudWatchLogs.Paginator.DescribeMetricFilters)

```python
# DescribeMetricFiltersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeMetricFiltersPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeMetricFiltersPaginator = client.get_paginator("describe_metric_filters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeMetricFiltersResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeMetricFiltersPaginator](./paginators.md#describemetricfilterspaginator)
3. item: [:material-code-braces: DescribeMetricFiltersResponseTypeDef](./type_defs.md#describemetricfiltersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeMetricFiltersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    logGroupName: str = ...,
    filterNamePrefix: str = ...,
    metricName: str = ...,
    metricNamespace: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeMetricFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeMetricFiltersResponseTypeDef](./type_defs.md#describemetricfiltersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeMetricFiltersRequestPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeMetricFiltersRequestPaginateTypeDef](./type_defs.md#describemetricfiltersrequestpaginatetypedef) 
## DescribeQueriesPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_queries")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeQueries.html#CloudWatchLogs.Paginator.DescribeQueries)

```python
# DescribeQueriesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeQueriesPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeQueriesPaginator = client.get_paginator("describe_queries")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeQueriesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeQueriesPaginator](./paginators.md#describequeriespaginator)
3. item: [:material-code-braces: DescribeQueriesResponseTypeDef](./type_defs.md#describequeriesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeQueriesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    logGroupName: str = ...,
    status: QueryStatusType = ...,  # (1)
    queryLanguage: QueryLanguageType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[DescribeQueriesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: QueryStatusType](./literals.md#querystatustype) 
2. See [:material-code-brackets: QueryLanguageType](./literals.md#querylanguagetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribeQueriesResponseTypeDef](./type_defs.md#describequeriesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeQueriesRequestPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeQueriesRequestPaginateTypeDef](./type_defs.md#describequeriesrequestpaginatetypedef) 
## DescribeResourcePoliciesPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_resource_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeResourcePolicies.html#CloudWatchLogs.Paginator.DescribeResourcePolicies)

```python
# DescribeResourcePoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeResourcePoliciesPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeResourcePoliciesPaginator = client.get_paginator("describe_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeResourcePoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeResourcePoliciesPaginator](./paginators.md#describeresourcepoliciespaginator)
3. item: [:material-code-braces: DescribeResourcePoliciesResponseTypeDef](./type_defs.md#describeresourcepoliciesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeResourcePoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeResourcePoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeResourcePoliciesResponseTypeDef](./type_defs.md#describeresourcepoliciesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeResourcePoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeResourcePoliciesRequestPaginateTypeDef](./type_defs.md#describeresourcepoliciesrequestpaginatetypedef) 
## DescribeSubscriptionFiltersPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("describe_subscription_filters")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/DescribeSubscriptionFilters.html#CloudWatchLogs.Paginator.DescribeSubscriptionFilters)

```python
# DescribeSubscriptionFiltersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import DescribeSubscriptionFiltersPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: DescribeSubscriptionFiltersPaginator = client.get_paginator("describe_subscription_filters")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSubscriptionFiltersResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [DescribeSubscriptionFiltersPaginator](./paginators.md#describesubscriptionfilterspaginator)
3. item: [:material-code-braces: DescribeSubscriptionFiltersResponseTypeDef](./type_defs.md#describesubscriptionfiltersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSubscriptionFiltersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    logGroupName: str,
    filterNamePrefix: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeSubscriptionFiltersResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSubscriptionFiltersResponseTypeDef](./type_defs.md#describesubscriptionfiltersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSubscriptionFiltersRequestPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSubscriptionFiltersRequestPaginateTypeDef](./type_defs.md#describesubscriptionfiltersrequestpaginatetypedef) 
## FilterLogEventsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("filter_log_events")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/FilterLogEvents.html#CloudWatchLogs.Paginator.FilterLogEvents)

```python
# FilterLogEventsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import FilterLogEventsPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: FilterLogEventsPaginator = client.get_paginator("filter_log_events")  # (2)
    async for item in paginator.paginate(...):
        item: FilterLogEventsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [FilterLogEventsPaginator](./paginators.md#filterlogeventspaginator)
3. item: [:material-code-braces: FilterLogEventsResponseTypeDef](./type_defs.md#filterlogeventsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python FilterLogEventsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    logGroupName: str = ...,
    logGroupIdentifier: str = ...,
    logStreamNames: Sequence[str] = ...,
    logStreamNamePrefix: str = ...,
    startTime: int = ...,
    endTime: int = ...,
    filterPattern: str = ...,
    interleaved: bool = ...,
    unmask: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[FilterLogEventsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: FilterLogEventsResponseTypeDef](./type_defs.md#filterlogeventsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: FilterLogEventsRequestPaginateTypeDef = {  # (1)
    "logGroupName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: FilterLogEventsRequestPaginateTypeDef](./type_defs.md#filterlogeventsrequestpaginatetypedef) 
## ListAnomaliesPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("list_anomalies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/ListAnomalies.html#CloudWatchLogs.Paginator.ListAnomalies)

```python
# ListAnomaliesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import ListAnomaliesPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: ListAnomaliesPaginator = client.get_paginator("list_anomalies")  # (2)
    async for item in paginator.paginate(...):
        item: ListAnomaliesResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [ListAnomaliesPaginator](./paginators.md#listanomaliespaginator)
3. item: [:material-code-braces: ListAnomaliesResponseTypeDef](./type_defs.md#listanomaliesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAnomaliesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    anomalyDetectorArn: str = ...,
    suppressionState: SuppressionStateType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListAnomaliesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SuppressionStateType](./literals.md#suppressionstatetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAnomaliesResponseTypeDef](./type_defs.md#listanomaliesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAnomaliesRequestPaginateTypeDef = {  # (1)
    "anomalyDetectorArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAnomaliesRequestPaginateTypeDef](./type_defs.md#listanomaliesrequestpaginatetypedef) 
## ListLogAnomalyDetectorsPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("list_log_anomaly_detectors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/ListLogAnomalyDetectors.html#CloudWatchLogs.Paginator.ListLogAnomalyDetectors)

```python
# ListLogAnomalyDetectorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import ListLogAnomalyDetectorsPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: ListLogAnomalyDetectorsPaginator = client.get_paginator("list_log_anomaly_detectors")  # (2)
    async for item in paginator.paginate(...):
        item: ListLogAnomalyDetectorsResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [ListLogAnomalyDetectorsPaginator](./paginators.md#listloganomalydetectorspaginator)
3. item: [:material-code-braces: ListLogAnomalyDetectorsResponseTypeDef](./type_defs.md#listloganomalydetectorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLogAnomalyDetectorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filterLogGroupArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLogAnomalyDetectorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLogAnomalyDetectorsResponseTypeDef](./type_defs.md#listloganomalydetectorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLogAnomalyDetectorsRequestPaginateTypeDef = {  # (1)
    "filterLogGroupArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLogAnomalyDetectorsRequestPaginateTypeDef](./type_defs.md#listloganomalydetectorsrequestpaginatetypedef) 
## ListLogGroupsForQueryPaginator

Type annotations and code completion for `#!python session.create_client("logs").get_paginator("list_log_groups_for_query")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/logs/paginator/ListLogGroupsForQuery.html#CloudWatchLogs.Paginator.ListLogGroupsForQuery)

```python
# ListLogGroupsForQueryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_logs.paginator import ListLogGroupsForQueryPaginator

session = get_session()
async with session.create_client("logs") as client:  # (1)
    paginator: ListLogGroupsForQueryPaginator = client.get_paginator("list_log_groups_for_query")  # (2)
    async for item in paginator.paginate(...):
        item: ListLogGroupsForQueryResponseTypeDef
        print(item)  # (3)
```

1. client: [CloudWatchLogsClient](./client.md)
2. paginator: [ListLogGroupsForQueryPaginator](./paginators.md#listloggroupsforquerypaginator)
3. item: [:material-code-braces: ListLogGroupsForQueryResponseTypeDef](./type_defs.md#listloggroupsforqueryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListLogGroupsForQueryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    queryId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListLogGroupsForQueryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListLogGroupsForQueryResponseTypeDef](./type_defs.md#listloggroupsforqueryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListLogGroupsForQueryRequestPaginateTypeDef = {  # (1)
    "queryId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListLogGroupsForQueryRequestPaginateTypeDef](./type_defs.md#listloggroupsforqueryrequestpaginatetypedef) 

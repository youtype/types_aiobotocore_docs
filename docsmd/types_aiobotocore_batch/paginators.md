# Paginators

> [Index](../README.md) > [Batch](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#batch)
    type annotations stubs module [types-aiobotocore-batch](https://pypi.org/project/types-aiobotocore-batch/).

## DescribeComputeEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("describe_compute_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/DescribeComputeEnvironments.html#Batch.Paginator.DescribeComputeEnvironments)

```python
# DescribeComputeEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import DescribeComputeEnvironmentsPaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: DescribeComputeEnvironmentsPaginator = client.get_paginator("describe_compute_environments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeComputeEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [DescribeComputeEnvironmentsPaginator](./paginators.md#describecomputeenvironmentspaginator)
3. item: `AioPageIterator[DescribeComputeEnvironmentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeComputeEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    computeEnvironments: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeComputeEnvironmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeComputeEnvironmentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeComputeEnvironmentsRequestPaginateTypeDef = {  # (1)
    "computeEnvironments": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeComputeEnvironmentsRequestPaginateTypeDef](./type_defs.md#describecomputeenvironmentsrequestpaginatetypedef)
## DescribeJobDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("describe_job_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/DescribeJobDefinitions.html#Batch.Paginator.DescribeJobDefinitions)

```python
# DescribeJobDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import DescribeJobDefinitionsPaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: DescribeJobDefinitionsPaginator = client.get_paginator("describe_job_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobDefinitionsResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [DescribeJobDefinitionsPaginator](./paginators.md#describejobdefinitionspaginator)
3. item: `AioPageIterator[DescribeJobDefinitionsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeJobDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobDefinitions: Sequence[str] = ...,
    jobDefinitionName: str = ...,
    status: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeJobDefinitionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeJobDefinitionsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeJobDefinitionsRequestPaginateTypeDef = {  # (1)
    "jobDefinitions": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobDefinitionsRequestPaginateTypeDef](./type_defs.md#describejobdefinitionsrequestpaginatetypedef)
## DescribeJobQueuesPaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("describe_job_queues")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/DescribeJobQueues.html#Batch.Paginator.DescribeJobQueues)

```python
# DescribeJobQueuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import DescribeJobQueuesPaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: DescribeJobQueuesPaginator = client.get_paginator("describe_job_queues")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeJobQueuesResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [DescribeJobQueuesPaginator](./paginators.md#describejobqueuespaginator)
3. item: `AioPageIterator[DescribeJobQueuesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeJobQueuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobQueues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeJobQueuesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeJobQueuesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeJobQueuesRequestPaginateTypeDef = {  # (1)
    "jobQueues": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeJobQueuesRequestPaginateTypeDef](./type_defs.md#describejobqueuesrequestpaginatetypedef)
## DescribeServiceEnvironmentsPaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("describe_service_environments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/DescribeServiceEnvironments.html#Batch.Paginator.DescribeServiceEnvironments)

```python
# DescribeServiceEnvironmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import DescribeServiceEnvironmentsPaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: DescribeServiceEnvironmentsPaginator = client.get_paginator("describe_service_environments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeServiceEnvironmentsResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [DescribeServiceEnvironmentsPaginator](./paginators.md#describeserviceenvironmentspaginator)
3. item: `AioPageIterator[DescribeServiceEnvironmentsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeServiceEnvironmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    serviceEnvironments: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeServiceEnvironmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeServiceEnvironmentsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeServiceEnvironmentsRequestPaginateTypeDef = {  # (1)
    "serviceEnvironments": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeServiceEnvironmentsRequestPaginateTypeDef](./type_defs.md#describeserviceenvironmentsrequestpaginatetypedef)
## ListConsumableResourcesPaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("list_consumable_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/ListConsumableResources.html#Batch.Paginator.ListConsumableResources)

```python
# ListConsumableResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import ListConsumableResourcesPaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: ListConsumableResourcesPaginator = client.get_paginator("list_consumable_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListConsumableResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [ListConsumableResourcesPaginator](./paginators.md#listconsumableresourcespaginator)
3. item: `AioPageIterator[ListConsumableResourcesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListConsumableResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: Sequence[KeyValuesPairTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListConsumableResourcesResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[KeyValuesPairTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListConsumableResourcesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListConsumableResourcesRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConsumableResourcesRequestPaginateTypeDef](./type_defs.md#listconsumableresourcesrequestpaginatetypedef)
## ListJobsByConsumableResourcePaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("list_jobs_by_consumable_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/ListJobsByConsumableResource.html#Batch.Paginator.ListJobsByConsumableResource)

```python
# ListJobsByConsumableResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import ListJobsByConsumableResourcePaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: ListJobsByConsumableResourcePaginator = client.get_paginator("list_jobs_by_consumable_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsByConsumableResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [ListJobsByConsumableResourcePaginator](./paginators.md#listjobsbyconsumableresourcepaginator)
3. item: `AioPageIterator[ListJobsByConsumableResourceResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobsByConsumableResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    consumableResource: str,
    filters: Sequence[KeyValuesPairTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListJobsByConsumableResourceResponseTypeDef]:  # (3)
    ...
```

1. See `Sequence[KeyValuesPairTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListJobsByConsumableResourceResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsByConsumableResourceRequestPaginateTypeDef = {  # (1)
    "consumableResource": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsByConsumableResourceRequestPaginateTypeDef](./type_defs.md#listjobsbyconsumableresourcerequestpaginatetypedef)
## ListJobsPaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("list_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/ListJobs.html#Batch.Paginator.ListJobs)

```python
# ListJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import ListJobsPaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: ListJobsPaginator = client.get_paginator("list_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [ListJobsPaginator](./paginators.md#listjobspaginator)
3. item: `AioPageIterator[ListJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobQueue: str = ...,
    arrayJobId: str = ...,
    multiNodeJobId: str = ...,
    jobStatus: JobStatusType = ...,  # (1)
    filters: Sequence[KeyValuesPairTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype)
2. See `Sequence[KeyValuesPairTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListJobsRequestPaginateTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListJobsRequestPaginateTypeDef](./type_defs.md#listjobsrequestpaginatetypedef)
## ListSchedulingPoliciesPaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("list_scheduling_policies")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/ListSchedulingPolicies.html#Batch.Paginator.ListSchedulingPolicies)

```python
# ListSchedulingPoliciesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import ListSchedulingPoliciesPaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: ListSchedulingPoliciesPaginator = client.get_paginator("list_scheduling_policies")  # (2)
    async for item in paginator.paginate(...):
        item: ListSchedulingPoliciesResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [ListSchedulingPoliciesPaginator](./paginators.md#listschedulingpoliciespaginator)
3. item: `AioPageIterator[ListSchedulingPoliciesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSchedulingPoliciesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSchedulingPoliciesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSchedulingPoliciesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSchedulingPoliciesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSchedulingPoliciesRequestPaginateTypeDef](./type_defs.md#listschedulingpoliciesrequestpaginatetypedef)
## ListServiceJobsPaginator

Type annotations and code completion for `#!python session.create_client("batch").get_paginator("list_service_jobs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch/paginator/ListServiceJobs.html#Batch.Paginator.ListServiceJobs)

```python
# ListServiceJobsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_batch.paginator import ListServiceJobsPaginator

session = get_session()
async with session.create_client("batch") as client:  # (1)
    paginator: ListServiceJobsPaginator = client.get_paginator("list_service_jobs")  # (2)
    async for item in paginator.paginate(...):
        item: ListServiceJobsResponseTypeDef
        print(item)  # (3)
```

1. client: [BatchClient](./client.md)
2. paginator: [ListServiceJobsPaginator](./paginators.md#listservicejobspaginator)
3. item: `AioPageIterator[ListServiceJobsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListServiceJobsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    jobQueue: str = ...,
    jobStatus: ServiceJobStatusType = ...,  # (1)
    filters: Sequence[KeyValuesPairTypeDef] = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[ListServiceJobsResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ServiceJobStatusType](./literals.md#servicejobstatustype)
2. See `Sequence[KeyValuesPairTypeDef]`
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[ListServiceJobsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListServiceJobsRequestPaginateTypeDef = {  # (1)
    "jobQueue": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListServiceJobsRequestPaginateTypeDef](./type_defs.md#listservicejobsrequestpaginatetypedef)

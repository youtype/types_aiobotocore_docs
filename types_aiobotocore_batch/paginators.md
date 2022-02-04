<a id="paginators-for-aiobotocore-batch-module"></a>

# Paginators for aiobotocore Batch module

> [Index](..) > [Batch](.) > Paginators

Auto-generated documentation for
[Batch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch)
type annotations stubs module
[types-aiobotocore-batch](https://pypi.org/project/types-aiobotocore-batch/).

- [Paginators for aiobotocore Batch module](#paginators-for-aiobotocore-batch-module)
  - [DescribeComputeEnvironmentsPaginator](#describecomputeenvironmentspaginator)
  - [DescribeJobDefinitionsPaginator](#describejobdefinitionspaginator)
  - [DescribeJobQueuesPaginator](#describejobqueuespaginator)
  - [ListJobsPaginator](#listjobspaginator)
  - [ListSchedulingPoliciesPaginator](#listschedulingpoliciespaginator)

<a id="describecomputeenvironmentspaginator"></a>

## DescribeComputeEnvironmentsPaginator

Type annotations for
`aiobotocore.create_client("batch").get_paginator("describe_compute_environments")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_batch.paginator import DescribeComputeEnvironmentsPaginator

def get_describe_compute_environments_paginator() -> DescribeComputeEnvironmentsPaginator:
    return Session().create_client("batch").get_paginator("describe_compute_environments")
```

Boto3 documentation:
[Batch.Paginator.DescribeComputeEnvironments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeComputeEnvironments)

Arguments for `DescribeComputeEnvironmentsPaginator.paginate` method:

- `computeEnvironments`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeComputeEnvironmentsPaginator.paginate` returns
`_PageIterator`\[[DescribeComputeEnvironmentsResponseTypeDef](./type_defs.md#describecomputeenvironmentsresponsetypedef)\].

<a id="describejobdefinitionspaginator"></a>

## DescribeJobDefinitionsPaginator

Type annotations for
`aiobotocore.create_client("batch").get_paginator("describe_job_definitions")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_batch.paginator import DescribeJobDefinitionsPaginator

def get_describe_job_definitions_paginator() -> DescribeJobDefinitionsPaginator:
    return Session().create_client("batch").get_paginator("describe_job_definitions")
```

Boto3 documentation:
[Batch.Paginator.DescribeJobDefinitions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobDefinitions)

Arguments for `DescribeJobDefinitionsPaginator.paginate` method:

- `jobDefinitions`: `Sequence`\[`str`\]
- `jobDefinitionName`: `str`
- `status`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeJobDefinitionsPaginator.paginate` returns
`_PageIterator`\[[DescribeJobDefinitionsResponseTypeDef](./type_defs.md#describejobdefinitionsresponsetypedef)\].

<a id="describejobqueuespaginator"></a>

## DescribeJobQueuesPaginator

Type annotations for
`aiobotocore.create_client("batch").get_paginator("describe_job_queues")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_batch.paginator import DescribeJobQueuesPaginator

def get_describe_job_queues_paginator() -> DescribeJobQueuesPaginator:
    return Session().create_client("batch").get_paginator("describe_job_queues")
```

Boto3 documentation:
[Batch.Paginator.DescribeJobQueues](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.DescribeJobQueues)

Arguments for `DescribeJobQueuesPaginator.paginate` method:

- `jobQueues`: `Sequence`\[`str`\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeJobQueuesPaginator.paginate` returns
`_PageIterator`\[[DescribeJobQueuesResponseTypeDef](./type_defs.md#describejobqueuesresponsetypedef)\].

<a id="listjobspaginator"></a>

## ListJobsPaginator

Type annotations for
`aiobotocore.create_client("batch").get_paginator("list_jobs")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_batch.paginator import ListJobsPaginator

def get_list_jobs_paginator() -> ListJobsPaginator:
    return Session().create_client("batch").get_paginator("list_jobs")
```

Boto3 documentation:
[Batch.Paginator.ListJobs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListJobs)

Arguments for `ListJobsPaginator.paginate` method:

- `jobQueue`: `str`
- `arrayJobId`: `str`
- `multiNodeJobId`: `str`
- `jobStatus`: [JobStatusType](./literals.md#jobstatustype)
- `filters`:
  `Sequence`\[[KeyValuesPairTypeDef](./type_defs.md#keyvaluespairtypedef)\]
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListJobsPaginator.paginate` returns
`_PageIterator`\[[ListJobsResponseTypeDef](./type_defs.md#listjobsresponsetypedef)\].

<a id="listschedulingpoliciespaginator"></a>

## ListSchedulingPoliciesPaginator

Type annotations for
`aiobotocore.create_client("batch").get_paginator("list_scheduling_policies")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_batch.paginator import ListSchedulingPoliciesPaginator

def get_list_scheduling_policies_paginator() -> ListSchedulingPoliciesPaginator:
    return Session().create_client("batch").get_paginator("list_scheduling_policies")
```

Boto3 documentation:
[Batch.Paginator.ListSchedulingPolicies](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/batch.html#Batch.Paginator.ListSchedulingPolicies)

Arguments for `ListSchedulingPoliciesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListSchedulingPoliciesPaginator.paginate` returns
`_PageIterator`\[[ListSchedulingPoliciesResponseTypeDef](./type_defs.md#listschedulingpoliciesresponsetypedef)\].

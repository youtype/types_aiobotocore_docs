# Examples

> [Index](../README.md) > [SSMIncidents](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SSMIncidents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-incidents.html#ssmincidents)
    type annotations stubs module [types-aiobotocore-ssm-incidents](https://pypi.org/project/types-aiobotocore-ssm-incidents/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[ssm-incidents]` package installed.

Write your `SSMIncidents` code as usual,
type checking and code completion should work out of the box.



```python
# SSMIncidentsClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-incidents") as client:  # (1)
    result = await client.batch_get_incident_findings()  # (2)
```

1. client: [SSMIncidentsClient](./client.md)
2. result: [:material-code-braces: BatchGetIncidentFindingsOutputTypeDef](./type_defs.md#batchgetincidentfindingsoutputtypedef) 



```python
# GetResourcePoliciesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-incidents") as client:  # (1)
    paginator = client.get_paginator("get_resource_policies")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SSMIncidentsClient](./client.md)
2. paginator: [GetResourcePoliciesPaginator](./paginators.md#getresourcepoliciespaginator)
3. item: [:material-code-braces: GetResourcePoliciesOutputTypeDef](./type_defs.md#getresourcepoliciesoutputtypedef) 



```python
# WaitForReplicationSetActiveWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("ssm-incidents") as client:  # (1)
    waiter = client.get_waiter("wait_for_replication_set_active")  # (2)
    await waiter.wait()
```

1. client: [SSMIncidentsClient](./client.md)
2. waiter: [WaitForReplicationSetActiveWaiter](./waiters.md#waitforreplicationsetactivewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[ssm-incidents]`
or a standalone `types_aiobotocore_ssm_incidents` package, you have to explicitly specify
`client: SSMIncidentsClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SSMIncidentsClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.client import SSMIncidentsClient
from types_aiobotocore_ssm_incidents.type_defs import BatchGetIncidentFindingsOutputTypeDef
from types_aiobotocore_ssm_incidents.type_defs import BatchGetIncidentFindingsInputTypeDef


session = get_session()

async with session.create_client("ssm-incidents") as client:
    client: SSMIncidentsClient
    kwargs: BatchGetIncidentFindingsInputTypeDef = {...}
    result: BatchGetIncidentFindingsOutputTypeDef = await client.batch_get_incident_findings(**kwargs)
```



```python
# GetResourcePoliciesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.client import SSMIncidentsClient
from types_aiobotocore_ssm_incidents.paginator import GetResourcePoliciesPaginator
from types_aiobotocore_ssm_incidents.type_defs import GetResourcePoliciesOutputTypeDef


session = get_session()

async with session.create_client("ssm-incidents") as client:
    client: SSMIncidentsClient
    paginator: GetResourcePoliciesPaginator = client.get_paginator("get_resource_policies")
    async for item in paginator.paginate(...):
        item: GetResourcePoliciesOutputTypeDef
        print(item)
```



```python
# WaitForReplicationSetActiveWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_ssm_incidents.client import SSMIncidentsClient
from types_aiobotocore_ssm_incidents.waiter import WaitForReplicationSetActiveWaiter


session = get_session()

async with session.create_client("ssm-incidents") as client:
    client: SSMIncidentsClient
    waiter: WaitForReplicationSetActiveWaiter = client.get_waiter("wait_for_replication_set_active")
    await waiter.wait()
```

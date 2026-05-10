# Examples

> [Index](../README.md) > [DevOpsAgentService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DevOpsAgentService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-agent.html#devopsagentservice)
    type annotations stubs module [types-aiobotocore-devops-agent](https://pypi.org/project/types-aiobotocore-devops-agent/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[devops-agent]` package installed.

Write your `DevOpsAgentService` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# DevOpsAgentServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("devops-agent") as client:  # (1)
    result = await client.associate_service()  # (2)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. result: [:material-code-braces: AssociateServiceOutputTypeDef](./type_defs.md#associateserviceoutputtypedef)



#### Paginator usage example

```python
# ListAgentSpacesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("devops-agent") as client:  # (1)
    paginator = client.get_paginator("list_agent_spaces")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DevOpsAgentServiceClient](./client.md)
2. paginator: [ListAgentSpacesPaginator](./paginators.md#listagentspacespaginator)
3. item: [:material-code-braces: ListAgentSpacesOutputTypeDef](./type_defs.md#listagentspacesoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[devops-agent]`
or a standalone `types_aiobotocore_devops_agent` package, you have to explicitly specify
`client: DevOpsAgentServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# DevOpsAgentServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.client import DevOpsAgentServiceClient
from types_aiobotocore_devops_agent.type_defs import AssociateServiceOutputTypeDef
from types_aiobotocore_devops_agent.type_defs import AssociateServiceInputTypeDef


session = get_session()

async with session.create_client("devops-agent") as client:
    client: DevOpsAgentServiceClient
    kwargs: AssociateServiceInputTypeDef = {...}
    result: AssociateServiceOutputTypeDef = await client.associate_service(**kwargs)
```



#### Paginator usage example

```python
# ListAgentSpacesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_devops_agent.client import DevOpsAgentServiceClient
from types_aiobotocore_devops_agent.paginator import ListAgentSpacesPaginator
from types_aiobotocore_devops_agent.type_defs import ListAgentSpacesOutputTypeDef


session = get_session()

async with session.create_client("devops-agent") as client:
    client: DevOpsAgentServiceClient
    paginator: ListAgentSpacesPaginator = client.get_paginator("list_agent_spaces")
    async for item in paginator.paginate(...):
        item: ListAgentSpacesOutputTypeDef
        print(item)
```



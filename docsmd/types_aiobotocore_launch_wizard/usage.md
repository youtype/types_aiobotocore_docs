# Examples

> [Index](../README.md) > [LaunchWizard](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#launchwizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[launch-wizard]` package installed.

Write your `LaunchWizard` code as usual,
type checking and code completion should work out of the box.



```python
# LaunchWizardClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("launch-wizard") as client:  # (1)
    result = await client.create_deployment()  # (2)
```

1. client: [LaunchWizardClient](./client.md)
2. result: [:material-code-braces: CreateDeploymentOutputTypeDef](./type_defs.md#createdeploymentoutputtypedef) 



```python
# ListDeploymentEventsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("launch-wizard") as client:  # (1)
    paginator = client.get_paginator("list_deployment_events")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [LaunchWizardClient](./client.md)
2. paginator: [ListDeploymentEventsPaginator](./paginators.md#listdeploymenteventspaginator)
3. item: [:material-code-braces: ListDeploymentEventsOutputTypeDef](./type_defs.md#listdeploymenteventsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[launch-wizard]`
or a standalone `types_aiobotocore_launch_wizard` package, you have to explicitly specify
`client: LaunchWizardClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# LaunchWizardClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_launch_wizard.client import LaunchWizardClient
from types_aiobotocore_launch_wizard.type_defs import CreateDeploymentOutputTypeDef
from types_aiobotocore_launch_wizard.type_defs import CreateDeploymentInputTypeDef


session = get_session()

async with session.create_client("launch-wizard") as client:
    client: LaunchWizardClient
    kwargs: CreateDeploymentInputTypeDef = {...}
    result: CreateDeploymentOutputTypeDef = await client.create_deployment(**kwargs)
```



```python
# ListDeploymentEventsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_launch_wizard.client import LaunchWizardClient
from types_aiobotocore_launch_wizard.paginator import ListDeploymentEventsPaginator
from types_aiobotocore_launch_wizard.type_defs import ListDeploymentEventsOutputTypeDef


session = get_session()

async with session.create_client("launch-wizard") as client:
    client: LaunchWizardClient
    paginator: ListDeploymentEventsPaginator = client.get_paginator("list_deployment_events")
    async for item in paginator.paginate(...):
        item: ListDeploymentEventsOutputTypeDef
        print(item)
```



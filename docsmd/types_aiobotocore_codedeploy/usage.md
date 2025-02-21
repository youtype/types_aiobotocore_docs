# Examples

> [Index](../README.md) > [CodeDeploy](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#codedeploy)
    type annotations stubs module [types-aiobotocore-codedeploy](https://pypi.org/project/types-aiobotocore-codedeploy/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codedeploy]` package installed.

Write your `CodeDeploy` code as usual,
type checking and code completion should work out of the box.



```python
# CodeDeployClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codedeploy") as client:  # (1)
    result = await client.add_tags_to_on_premises_instances()  # (2)
```

1. client: [CodeDeployClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListApplicationRevisionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codedeploy") as client:  # (1)
    paginator = client.get_paginator("list_application_revisions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeDeployClient](./client.md)
2. paginator: [ListApplicationRevisionsPaginator](./paginators.md#listapplicationrevisionspaginator)
3. item: [:material-code-braces: ListApplicationRevisionsOutputTypeDef](./type_defs.md#listapplicationrevisionsoutputtypedef) 



```python
# DeploymentSuccessfulWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codedeploy") as client:  # (1)
    waiter = client.get_waiter("deployment_successful")  # (2)
    await waiter.wait()
```

1. client: [CodeDeployClient](./client.md)
2. waiter: [DeploymentSuccessfulWaiter](./waiters.md#deploymentsuccessfulwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[codedeploy]`
or a standalone `types_aiobotocore_codedeploy` package, you have to explicitly specify
`client: CodeDeployClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeDeployClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.client import CodeDeployClient
from types_aiobotocore_codedeploy.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_codedeploy.type_defs import AddTagsToOnPremisesInstancesInputTypeDef


session = get_session()

async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    kwargs: AddTagsToOnPremisesInstancesInputTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.add_tags_to_on_premises_instances(**kwargs)
```



```python
# ListApplicationRevisionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.client import CodeDeployClient
from types_aiobotocore_codedeploy.paginator import ListApplicationRevisionsPaginator
from types_aiobotocore_codedeploy.type_defs import ListApplicationRevisionsOutputTypeDef


session = get_session()

async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    paginator: ListApplicationRevisionsPaginator = client.get_paginator("list_application_revisions")
    async for item in paginator.paginate(...):
        item: ListApplicationRevisionsOutputTypeDef
        print(item)
```



```python
# DeploymentSuccessfulWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.client import CodeDeployClient
from types_aiobotocore_codedeploy.waiter import DeploymentSuccessfulWaiter


session = get_session()

async with session.create_client("codedeploy") as client:
    client: CodeDeployClient
    waiter: DeploymentSuccessfulWaiter = client.get_waiter("deployment_successful")
    await waiter.wait()
```

<a id="examples-for-aiobotocore-codedeploy-module"></a>

# Examples for aiobotocore CodeDeploy module

> [Index](../README.md) > [CodeDeploy](./README.md) > Examples

- [Examples for aiobotocore CodeDeploy module](#examples-for-aiobotocore-codedeploy-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codedeploy]` package installed.

Write your `CodeDeploy` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodeDeployClient
# and provides type checking and code completion
async with session.create_client("codedeploy") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags_to_on_premises_instances()
    

    
    # paginator has type ListApplicationRevisionsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_application_revisions")
    async for item in paginator.paginate(...):
        # item has type ListApplicationRevisionsOutputTypeDef
        print(item)
    

    
    # waiter has type DeploymentSuccessfulWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("deployment_successful")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codedeploy]` or a standalone
`types_aiobotocore_codedeploy` package, you have to explicitly specify
`client: CodeDeployClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codedeploy.client import CodeDeployClient
from types_aiobotocore_codedeploy.type_defs import None
from types_aiobotocore_codedeploy.paginator import ListApplicationRevisionsPaginator
from types_aiobotocore_codedeploy.waiter import DeploymentSuccessfulWaiter
from types_aiobotocore_codedeploy.literals import PaginatorName
from types_aiobotocore_codedeploy.literals import WaiterName


session = get_session()

async with session.create_client("codedeploy") as client:
    client: CodeDeployClient

    
    result: None = client.add_tags_to_on_premises_instances()
    

    
    paginator_name: PaginatorName = "list_application_revisions"
    paginator: ListApplicationRevisionsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListApplicationRevisionsOutputTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "deployment_successful"
    waiter: DeploymentSuccessfulWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```

# Examples

> [Index](../README.md) > [WorkSpaces](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [WorkSpaces](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workspaces.html#workspaces)
    type annotations stubs module [types-aiobotocore-workspaces](https://pypi.org/project/types-aiobotocore-workspaces/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[workspaces]` package installed.

Write your `WorkSpaces` code as usual,
type checking and code completion should work out of the box.



```python
# WorkSpacesClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces") as client:  # (1)
    result = await client.accept_account_link_invitation()  # (2)
```

1. client: [WorkSpacesClient](./client.md)
2. result: [:material-code-braces: AcceptAccountLinkInvitationResultTypeDef](./type_defs.md#acceptaccountlinkinvitationresulttypedef) 



```python
# DescribeAccountModificationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("workspaces") as client:  # (1)
    paginator = client.get_paginator("describe_account_modifications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [WorkSpacesClient](./client.md)
2. paginator: [DescribeAccountModificationsPaginator](./paginators.md#describeaccountmodificationspaginator)
3. item: [:material-code-braces: DescribeAccountModificationsResultTypeDef](./type_defs.md#describeaccountmodificationsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[workspaces]`
or a standalone `types_aiobotocore_workspaces` package, you have to explicitly specify
`client: WorkSpacesClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# WorkSpacesClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces.client import WorkSpacesClient
from types_aiobotocore_workspaces.type_defs import AcceptAccountLinkInvitationResultTypeDef
from types_aiobotocore_workspaces.type_defs import AcceptAccountLinkInvitationRequestTypeDef


session = get_session()

async with session.create_client("workspaces") as client:
    client: WorkSpacesClient
    kwargs: AcceptAccountLinkInvitationRequestTypeDef = {...}
    result: AcceptAccountLinkInvitationResultTypeDef = await client.accept_account_link_invitation(**kwargs)
```



```python
# DescribeAccountModificationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_workspaces.client import WorkSpacesClient
from types_aiobotocore_workspaces.paginator import DescribeAccountModificationsPaginator
from types_aiobotocore_workspaces.type_defs import DescribeAccountModificationsResultTypeDef


session = get_session()

async with session.create_client("workspaces") as client:
    client: WorkSpacesClient
    paginator: DescribeAccountModificationsPaginator = client.get_paginator("describe_account_modifications")
    async for item in paginator.paginate(...):
        item: DescribeAccountModificationsResultTypeDef
        print(item)
```



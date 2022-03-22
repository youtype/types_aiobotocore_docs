<a id="examples-for-aiobotocore-devopsguru-module"></a>

# Examples for aiobotocore DevOpsGuru module

> [Index](../README.md) > [DevOpsGuru](./README.md) > Examples

- [Examples for aiobotocore DevOpsGuru module](#examples-for-aiobotocore-devopsguru-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[devops-guru]` package installed.

Write your `DevOpsGuru` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DevOpsGuruClient
# and provides type checking and code completion
async with session.create_client("devops-guru") as client:
    
    # result has type AddNotificationChannelResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_notification_channel()
    

    
    # paginator has type DescribeOrganizationResourceCollectionHealthPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_organization_resource_collection_health")
    async for item in paginator.paginate(...):
        # item has type DescribeOrganizationResourceCollectionHealthResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[devops-guru]` or a standalone
`types_aiobotocore_devops_guru` package, you have to explicitly specify
`client: DevOpsGuruClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.client import DevOpsGuruClient
from types_aiobotocore_devops_guru.type_defs import AddNotificationChannelResponseTypeDef
from types_aiobotocore_devops_guru.paginator import DescribeOrganizationResourceCollectionHealthPaginator

from types_aiobotocore_devops_guru.literals import PaginatorName



session = get_session()

async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient

    
    result: AddNotificationChannelResponseTypeDef = client.add_notification_channel()
    

    
    paginator_name: PaginatorName = "describe_organization_resource_collection_health"
    paginator: DescribeOrganizationResourceCollectionHealthPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationResourceCollectionHealthResponseTypeDef
        print(item)
    

    
```

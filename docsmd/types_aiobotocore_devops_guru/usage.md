# Examples

> [Index](../README.md) > [DevOpsGuru](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DevOpsGuru](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#devopsguru)
    type annotations stubs module [types-aiobotocore-devops-guru](https://pypi.org/project/types-aiobotocore-devops-guru/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[devops-guru]` package installed.

Write your `DevOpsGuru` code as usual,
type checking and code completion should work out of the box.



```python
# DevOpsGuruClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("devops-guru") as client:  # (1)
    result = await client.add_notification_channel()  # (2)
```

1. client: [DevOpsGuruClient](./client.md)
2. result: [:material-code-braces: AddNotificationChannelResponseTypeDef](./type_defs.md#addnotificationchannelresponsetypedef) 



```python
# DescribeOrganizationResourceCollectionHealthPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("devops-guru") as client:  # (1)
    paginator = client.get_paginator("describe_organization_resource_collection_health")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DevOpsGuruClient](./client.md)
2. paginator: [DescribeOrganizationResourceCollectionHealthPaginator](./paginators.md#describeorganizationresourcecollectionhealthpaginator)
3. item: [:material-code-braces: DescribeOrganizationResourceCollectionHealthResponseTypeDef](./type_defs.md#describeorganizationresourcecollectionhealthresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[devops-guru]`
or a standalone `types_aiobotocore_devops_guru` package, you have to explicitly specify
`client: DevOpsGuruClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DevOpsGuruClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.client import DevOpsGuruClient
from types_aiobotocore_devops_guru.type_defs import AddNotificationChannelResponseTypeDef
from types_aiobotocore_devops_guru.type_defs import AddNotificationChannelRequestTypeDef


session = get_session()

async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    kwargs: AddNotificationChannelRequestTypeDef = {...}
    result: AddNotificationChannelResponseTypeDef = await client.add_notification_channel(**kwargs)
```



```python
# DescribeOrganizationResourceCollectionHealthPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_devops_guru.client import DevOpsGuruClient
from types_aiobotocore_devops_guru.paginator import DescribeOrganizationResourceCollectionHealthPaginator
from types_aiobotocore_devops_guru.type_defs import DescribeOrganizationResourceCollectionHealthResponseTypeDef


session = get_session()

async with session.create_client("devops-guru") as client:
    client: DevOpsGuruClient
    paginator: DescribeOrganizationResourceCollectionHealthPaginator = client.get_paginator("describe_organization_resource_collection_health")
    async for item in paginator.paginate(...):
        item: DescribeOrganizationResourceCollectionHealthResponseTypeDef
        print(item)
```



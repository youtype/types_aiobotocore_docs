# Examples

> [Index](../README.md) > [ConnectWisdomService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ConnectWisdomService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/wisdom.html#connectwisdomservice)
    type annotations stubs module [types-aiobotocore-wisdom](https://pypi.org/project/types-aiobotocore-wisdom/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[wisdom]` package installed.

Write your `ConnectWisdomService` code as usual,
type checking and code completion should work out of the box.



```python
# ConnectWisdomServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("wisdom") as client:  # (1)
    result = await client.create_assistant()  # (2)
```

1. client: [ConnectWisdomServiceClient](./client.md)
2. result: [:material-code-braces: CreateAssistantResponseTypeDef](./type_defs.md#createassistantresponsetypedef) 



```python
# ListAssistantAssociationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("wisdom") as client:  # (1)
    paginator = client.get_paginator("list_assistant_associations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ConnectWisdomServiceClient](./client.md)
2. paginator: [ListAssistantAssociationsPaginator](./paginators.md#listassistantassociationspaginator)
3. item: [:material-code-braces: ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[wisdom]`
or a standalone `types_aiobotocore_wisdom` package, you have to explicitly specify
`client: ConnectWisdomServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ConnectWisdomServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_wisdom.client import ConnectWisdomServiceClient
from types_aiobotocore_wisdom.type_defs import CreateAssistantResponseTypeDef
from types_aiobotocore_wisdom.type_defs import CreateAssistantRequestTypeDef


session = get_session()

async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    kwargs: CreateAssistantRequestTypeDef = {...}
    result: CreateAssistantResponseTypeDef = await client.create_assistant(**kwargs)
```



```python
# ListAssistantAssociationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_wisdom.client import ConnectWisdomServiceClient
from types_aiobotocore_wisdom.paginator import ListAssistantAssociationsPaginator
from types_aiobotocore_wisdom.type_defs import ListAssistantAssociationsResponseTypeDef


session = get_session()

async with session.create_client("wisdom") as client:
    client: ConnectWisdomServiceClient
    paginator: ListAssistantAssociationsPaginator = client.get_paginator("list_assistant_associations")
    async for item in paginator.paginate(...):
        item: ListAssistantAssociationsResponseTypeDef
        print(item)
```



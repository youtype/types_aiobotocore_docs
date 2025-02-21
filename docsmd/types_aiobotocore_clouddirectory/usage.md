# Examples

> [Index](../README.md) > [CloudDirectory](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudDirectory](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/clouddirectory.html#clouddirectory)
    type annotations stubs module [types-aiobotocore-clouddirectory](https://pypi.org/project/types-aiobotocore-clouddirectory/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[clouddirectory]` package installed.

Write your `CloudDirectory` code as usual,
type checking and code completion should work out of the box.



```python
# CloudDirectoryClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("clouddirectory") as client:  # (1)
    result = await client.apply_schema()  # (2)
```

1. client: [CloudDirectoryClient](./client.md)
2. result: [:material-code-braces: ApplySchemaResponseTypeDef](./type_defs.md#applyschemaresponsetypedef) 



```python
# ListAppliedSchemaArnsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("clouddirectory") as client:  # (1)
    paginator = client.get_paginator("list_applied_schema_arns")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CloudDirectoryClient](./client.md)
2. paginator: [ListAppliedSchemaArnsPaginator](./paginators.md#listappliedschemaarnspaginator)
3. item: [:material-code-braces: ListAppliedSchemaArnsResponseTypeDef](./type_defs.md#listappliedschemaarnsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[clouddirectory]`
or a standalone `types_aiobotocore_clouddirectory` package, you have to explicitly specify
`client: CloudDirectoryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudDirectoryClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.client import CloudDirectoryClient
from types_aiobotocore_clouddirectory.type_defs import ApplySchemaResponseTypeDef
from types_aiobotocore_clouddirectory.type_defs import ApplySchemaRequestTypeDef


session = get_session()

async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    kwargs: ApplySchemaRequestTypeDef = {...}
    result: ApplySchemaResponseTypeDef = await client.apply_schema(**kwargs)
```



```python
# ListAppliedSchemaArnsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_clouddirectory.client import CloudDirectoryClient
from types_aiobotocore_clouddirectory.paginator import ListAppliedSchemaArnsPaginator
from types_aiobotocore_clouddirectory.type_defs import ListAppliedSchemaArnsResponseTypeDef


session = get_session()

async with session.create_client("clouddirectory") as client:
    client: CloudDirectoryClient
    paginator: ListAppliedSchemaArnsPaginator = client.get_paginator("list_applied_schema_arns")
    async for item in paginator.paginate(...):
        item: ListAppliedSchemaArnsResponseTypeDef
        print(item)
```



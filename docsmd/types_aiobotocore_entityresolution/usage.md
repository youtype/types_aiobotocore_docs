# Examples

> [Index](../README.md) > [EntityResolution](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [EntityResolution](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/entityresolution.html#entityresolution)
    type annotations stubs module [types-aiobotocore-entityresolution](https://pypi.org/project/types-aiobotocore-entityresolution/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[entityresolution]` package installed.

Write your `EntityResolution` code as usual,
type checking and code completion should work out of the box.



```python
# EntityResolutionClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("entityresolution") as client:  # (1)
    result = await client.add_policy_statement()  # (2)
```

1. client: [EntityResolutionClient](./client.md)
2. result: [:material-code-braces: AddPolicyStatementOutputTypeDef](./type_defs.md#addpolicystatementoutputtypedef) 



```python
# ListIdMappingJobsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("entityresolution") as client:  # (1)
    paginator = client.get_paginator("list_id_mapping_jobs")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [EntityResolutionClient](./client.md)
2. paginator: [ListIdMappingJobsPaginator](./paginators.md#listidmappingjobspaginator)
3. item: [:material-code-braces: ListIdMappingJobsOutputTypeDef](./type_defs.md#listidmappingjobsoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[entityresolution]`
or a standalone `types_aiobotocore_entityresolution` package, you have to explicitly specify
`client: EntityResolutionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# EntityResolutionClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.client import EntityResolutionClient
from types_aiobotocore_entityresolution.type_defs import AddPolicyStatementOutputTypeDef
from types_aiobotocore_entityresolution.type_defs import AddPolicyStatementInputTypeDef


session = get_session()

async with session.create_client("entityresolution") as client:
    client: EntityResolutionClient
    kwargs: AddPolicyStatementInputTypeDef = {...}
    result: AddPolicyStatementOutputTypeDef = await client.add_policy_statement(**kwargs)
```



```python
# ListIdMappingJobsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_entityresolution.client import EntityResolutionClient
from types_aiobotocore_entityresolution.paginator import ListIdMappingJobsPaginator
from types_aiobotocore_entityresolution.type_defs import ListIdMappingJobsOutputTypeDef


session = get_session()

async with session.create_client("entityresolution") as client:
    client: EntityResolutionClient
    paginator: ListIdMappingJobsPaginator = client.get_paginator("list_id_mapping_jobs")
    async for item in paginator.paginate(...):
        item: ListIdMappingJobsOutputTypeDef
        print(item)
```



# Examples

> [Index](../README.md) > [UserExperienceCustomization](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [UserExperienceCustomization](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/uxc.html#userexperiencecustomization)
    type annotations stubs module [types-aiobotocore-uxc](https://pypi.org/project/types-aiobotocore-uxc/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[uxc]` package installed.

Write your `UserExperienceCustomization` code as usual,
type checking and code completion should work out of the box.



#### Client method usage example

```python
# UserExperienceCustomizationClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("uxc") as client:  # (1)
    result = await client.list_services()  # (2)
```

1. client: [UserExperienceCustomizationClient](./client.md)
2. result: [:material-code-braces: ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef)



#### Paginator usage example

```python
# ListServicesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("uxc") as client:  # (1)
    paginator = client.get_paginator("list_services")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [UserExperienceCustomizationClient](./client.md)
2. paginator: [ListServicesPaginator](./paginators.md#listservicespaginator)
3. item: [:material-code-braces: ListServicesOutputTypeDef](./type_defs.md#listservicesoutputtypedef)




### Explicit type annotations

With `types-aiobotocore-lite[uxc]`
or a standalone `types_aiobotocore_uxc` package, you have to explicitly specify
`client: UserExperienceCustomizationClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


#### Client method usage example

```python
# UserExperienceCustomizationClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_uxc.client import UserExperienceCustomizationClient
from types_aiobotocore_uxc.type_defs import ListServicesOutputTypeDef
from types_aiobotocore_uxc.type_defs import ListServicesInputTypeDef


session = get_session()

async with session.create_client("uxc") as client:
    client: UserExperienceCustomizationClient
    kwargs: ListServicesInputTypeDef = {...}
    result: ListServicesOutputTypeDef = await client.list_services(**kwargs)
```



#### Paginator usage example

```python
# ListServicesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_uxc.client import UserExperienceCustomizationClient
from types_aiobotocore_uxc.paginator import ListServicesPaginator
from types_aiobotocore_uxc.type_defs import ListServicesOutputTypeDef


session = get_session()

async with session.create_client("uxc") as client:
    client: UserExperienceCustomizationClient
    paginator: ListServicesPaginator = client.get_paginator("list_services")
    async for item in paginator.paginate(...):
        item: ListServicesOutputTypeDef
        print(item)
```



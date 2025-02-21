# Examples

> [Index](../README.md) > [AppRegistry](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppRegistry](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog-appregistry.html#appregistry)
    type annotations stubs module [types-aiobotocore-servicecatalog-appregistry](https://pypi.org/project/types-aiobotocore-servicecatalog-appregistry/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[servicecatalog-appregistry]` package installed.

Write your `AppRegistry` code as usual,
type checking and code completion should work out of the box.



```python
# AppRegistryClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("servicecatalog-appregistry") as client:  # (1)
    result = await client.associate_attribute_group()  # (2)
```

1. client: [AppRegistryClient](./client.md)
2. result: [:material-code-braces: AssociateAttributeGroupResponseTypeDef](./type_defs.md#associateattributegroupresponsetypedef) 



```python
# ListApplicationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("servicecatalog-appregistry") as client:  # (1)
    paginator = client.get_paginator("list_applications")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [AppRegistryClient](./client.md)
2. paginator: [ListApplicationsPaginator](./paginators.md#listapplicationspaginator)
3. item: [:material-code-braces: ListApplicationsResponseTypeDef](./type_defs.md#listapplicationsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[servicecatalog-appregistry]`
or a standalone `types_aiobotocore_servicecatalog_appregistry` package, you have to explicitly specify
`client: AppRegistryClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AppRegistryClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.client import AppRegistryClient
from types_aiobotocore_servicecatalog_appregistry.type_defs import AssociateAttributeGroupResponseTypeDef
from types_aiobotocore_servicecatalog_appregistry.type_defs import AssociateAttributeGroupRequestTypeDef


session = get_session()

async with session.create_client("servicecatalog-appregistry") as client:
    client: AppRegistryClient
    kwargs: AssociateAttributeGroupRequestTypeDef = {...}
    result: AssociateAttributeGroupResponseTypeDef = await client.associate_attribute_group(**kwargs)
```



```python
# ListApplicationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.client import AppRegistryClient
from types_aiobotocore_servicecatalog_appregistry.paginator import ListApplicationsPaginator
from types_aiobotocore_servicecatalog_appregistry.type_defs import ListApplicationsResponseTypeDef


session = get_session()

async with session.create_client("servicecatalog-appregistry") as client:
    client: AppRegistryClient
    paginator: ListApplicationsPaginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)
```



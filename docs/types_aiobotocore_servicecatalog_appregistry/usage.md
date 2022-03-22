<a id="examples-for-aiobotocore-appregistry-module"></a>

# Examples for aiobotocore AppRegistry module

> [Index](../README.md) > [AppRegistry](./README.md) > Examples

- [Examples for aiobotocore AppRegistry module](#examples-for-aiobotocore-appregistry-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[servicecatalog-appregistry]` package
installed.

Write your `AppRegistry` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AppRegistryClient
# and provides type checking and code completion
async with session.create_client("servicecatalog-appregistry") as client:
    
    # result has type AssociateAttributeGroupResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_attribute_group()
    

    
    # paginator has type ListApplicationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_applications")
    async for item in paginator.paginate(...):
        # item has type ListApplicationsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[servicecatalog-appregistry]` or a standalone
`types_aiobotocore_servicecatalog_appregistry` package, you have to explicitly
specify `client: AppRegistryClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_servicecatalog_appregistry.client import AppRegistryClient
from types_aiobotocore_servicecatalog_appregistry.type_defs import AssociateAttributeGroupResponseTypeDef
from types_aiobotocore_servicecatalog_appregistry.paginator import ListApplicationsPaginator

from types_aiobotocore_servicecatalog_appregistry.literals import PaginatorName



session = get_session()

async with session.create_client("servicecatalog-appregistry") as client:
    client: AppRegistryClient

    
    result: AssociateAttributeGroupResponseTypeDef = client.associate_attribute_group()
    

    
    paginator_name: PaginatorName = "list_applications"
    paginator: ListApplicationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListApplicationsResponseTypeDef
        print(item)
    

    
```

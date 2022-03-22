<a id="examples-for-aiobotocore-databasemigrationservice-module"></a>

# Examples for aiobotocore DatabaseMigrationService module

> [Index](../README.md) > [DatabaseMigrationService](./README.md) > Examples

- [Examples for aiobotocore DatabaseMigrationService module](#examples-for-aiobotocore-databasemigrationservice-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[dms]` package installed.

Write your `DatabaseMigrationService` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DatabaseMigrationServiceClient
# and provides type checking and code completion
async with session.create_client("dms") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags_to_resource()
    

    
    # paginator has type DescribeCertificatesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_certificates")
    async for item in paginator.paginate(...):
        # item has type DescribeCertificatesResponseTypeDef
        print(item)
    

    
    # waiter has type EndpointDeletedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("endpoint_deleted")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[dms]` or a standalone `types_aiobotocore_dms`
package, you have to explicitly specify
`client: DatabaseMigrationServiceClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_dms.client import DatabaseMigrationServiceClient
from types_aiobotocore_dms.type_defs import Dict[str, Any]
from types_aiobotocore_dms.paginator import DescribeCertificatesPaginator
from types_aiobotocore_dms.waiter import EndpointDeletedWaiter
from types_aiobotocore_dms.literals import PaginatorName
from types_aiobotocore_dms.literals import WaiterName


session = get_session()

async with session.create_client("dms") as client:
    client: DatabaseMigrationServiceClient

    
    result: Dict[str, Any] = client.add_tags_to_resource()
    

    
    paginator_name: PaginatorName = "describe_certificates"
    paginator: DescribeCertificatesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeCertificatesResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "endpoint_deleted"
    waiter: EndpointDeletedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```

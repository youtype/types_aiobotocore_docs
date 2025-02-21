# Examples

> [Index](../README.md) > [DocDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DocDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb.html#docdb)
    type annotations stubs module [types-aiobotocore-docdb](https://pypi.org/project/types-aiobotocore-docdb/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[docdb]` package installed.

Write your `DocDB` code as usual,
type checking and code completion should work out of the box.



```python
# DocDBClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("docdb") as client:  # (1)
    result = await client.add_source_identifier_to_subscription()  # (2)
```

1. client: [DocDBClient](./client.md)
2. result: [:material-code-braces: AddSourceIdentifierToSubscriptionResultTypeDef](./type_defs.md#addsourceidentifiertosubscriptionresulttypedef) 



```python
# DescribeCertificatesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("docdb") as client:  # (1)
    paginator = client.get_paginator("describe_certificates")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DocDBClient](./client.md)
2. paginator: [DescribeCertificatesPaginator](./paginators.md#describecertificatespaginator)
3. item: [:material-code-braces: CertificateMessageTypeDef](./type_defs.md#certificatemessagetypedef) 



```python
# DBInstanceAvailableWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("docdb") as client:  # (1)
    waiter = client.get_waiter("db_instance_available")  # (2)
    await waiter.wait()
```

1. client: [DocDBClient](./client.md)
2. waiter: [DBInstanceAvailableWaiter](./waiters.md#dbinstanceavailablewaiter)


### Explicit type annotations

With `types-aiobotocore-lite[docdb]`
or a standalone `types_aiobotocore_docdb` package, you have to explicitly specify
`client: DocDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DocDBClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_docdb.client import DocDBClient
from types_aiobotocore_docdb.type_defs import AddSourceIdentifierToSubscriptionResultTypeDef
from types_aiobotocore_docdb.type_defs import AddSourceIdentifierToSubscriptionMessageTypeDef


session = get_session()

async with session.create_client("docdb") as client:
    client: DocDBClient
    kwargs: AddSourceIdentifierToSubscriptionMessageTypeDef = {...}
    result: AddSourceIdentifierToSubscriptionResultTypeDef = await client.add_source_identifier_to_subscription(**kwargs)
```



```python
# DescribeCertificatesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_docdb.client import DocDBClient
from types_aiobotocore_docdb.paginator import DescribeCertificatesPaginator
from types_aiobotocore_docdb.type_defs import CertificateMessageTypeDef


session = get_session()

async with session.create_client("docdb") as client:
    client: DocDBClient
    paginator: DescribeCertificatesPaginator = client.get_paginator("describe_certificates")
    async for item in paginator.paginate(...):
        item: CertificateMessageTypeDef
        print(item)
```



```python
# DBInstanceAvailableWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_docdb.client import DocDBClient
from types_aiobotocore_docdb.waiter import DBInstanceAvailableWaiter


session = get_session()

async with session.create_client("docdb") as client:
    client: DocDBClient
    waiter: DBInstanceAvailableWaiter = client.get_waiter("db_instance_available")
    await waiter.wait()
```

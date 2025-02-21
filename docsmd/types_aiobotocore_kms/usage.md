# Examples

> [Index](../README.md) > [KMS](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [KMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#kms)
    type annotations stubs module [types-aiobotocore-kms](https://pypi.org/project/types-aiobotocore-kms/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kms]` package installed.

Write your `KMS` code as usual,
type checking and code completion should work out of the box.



```python
# KMSClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kms") as client:  # (1)
    result = await client.cancel_key_deletion()  # (2)
```

1. client: [KMSClient](./client.md)
2. result: [:material-code-braces: CancelKeyDeletionResponseTypeDef](./type_defs.md#cancelkeydeletionresponsetypedef) 



```python
# DescribeCustomKeyStoresPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kms") as client:  # (1)
    paginator = client.get_paginator("describe_custom_key_stores")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [KMSClient](./client.md)
2. paginator: [DescribeCustomKeyStoresPaginator](./paginators.md#describecustomkeystorespaginator)
3. item: [:material-code-braces: DescribeCustomKeyStoresResponseTypeDef](./type_defs.md#describecustomkeystoresresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[kms]`
or a standalone `types_aiobotocore_kms` package, you have to explicitly specify
`client: KMSClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KMSClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kms.client import KMSClient
from types_aiobotocore_kms.type_defs import CancelKeyDeletionResponseTypeDef
from types_aiobotocore_kms.type_defs import CancelKeyDeletionRequestTypeDef


session = get_session()

async with session.create_client("kms") as client:
    client: KMSClient
    kwargs: CancelKeyDeletionRequestTypeDef = {...}
    result: CancelKeyDeletionResponseTypeDef = await client.cancel_key_deletion(**kwargs)
```



```python
# DescribeCustomKeyStoresPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kms.client import KMSClient
from types_aiobotocore_kms.paginator import DescribeCustomKeyStoresPaginator
from types_aiobotocore_kms.type_defs import DescribeCustomKeyStoresResponseTypeDef


session = get_session()

async with session.create_client("kms") as client:
    client: KMSClient
    paginator: DescribeCustomKeyStoresPaginator = client.get_paginator("describe_custom_key_stores")
    async for item in paginator.paginate(...):
        item: DescribeCustomKeyStoresResponseTypeDef
        print(item)
```



# Examples

> [Index](../README.md) > [Snowball](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Snowball](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snowball.html#snowball)
    type annotations stubs module [types-aiobotocore-snowball](https://pypi.org/project/types-aiobotocore-snowball/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[snowball]` package installed.

Write your `Snowball` code as usual,
type checking and code completion should work out of the box.



```python
# SnowballClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("snowball") as client:  # (1)
    result = await client.create_address()  # (2)
```

1. client: [SnowballClient](./client.md)
2. result: [:material-code-braces: CreateAddressResultTypeDef](./type_defs.md#createaddressresulttypedef) 



```python
# DescribeAddressesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("snowball") as client:  # (1)
    paginator = client.get_paginator("describe_addresses")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SnowballClient](./client.md)
2. paginator: [DescribeAddressesPaginator](./paginators.md#describeaddressespaginator)
3. item: [:material-code-braces: DescribeAddressesResultTypeDef](./type_defs.md#describeaddressesresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[snowball]`
or a standalone `types_aiobotocore_snowball` package, you have to explicitly specify
`client: SnowballClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SnowballClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_snowball.client import SnowballClient
from types_aiobotocore_snowball.type_defs import CreateAddressResultTypeDef
from types_aiobotocore_snowball.type_defs import CreateAddressRequestTypeDef


session = get_session()

async with session.create_client("snowball") as client:
    client: SnowballClient
    kwargs: CreateAddressRequestTypeDef = {...}
    result: CreateAddressResultTypeDef = await client.create_address(**kwargs)
```



```python
# DescribeAddressesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_snowball.client import SnowballClient
from types_aiobotocore_snowball.paginator import DescribeAddressesPaginator
from types_aiobotocore_snowball.type_defs import DescribeAddressesResultTypeDef


session = get_session()

async with session.create_client("snowball") as client:
    client: SnowballClient
    paginator: DescribeAddressesPaginator = client.get_paginator("describe_addresses")
    async for item in paginator.paginate(...):
        item: DescribeAddressesResultTypeDef
        print(item)
```



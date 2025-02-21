# Examples

> [Index](../README.md) > [CloudSearchDomain](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#cloudsearchdomain)
    type annotations stubs module [types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cloudsearchdomain]` package installed.

Write your `CloudSearchDomain` code as usual,
type checking and code completion should work out of the box.



```python
# CloudSearchDomainClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudsearchdomain") as client:  # (1)
    result = await client.search()  # (2)
```

1. client: [CloudSearchDomainClient](./client.md)
2. result: [:material-code-braces: SearchResponseTypeDef](./type_defs.md#searchresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[cloudsearchdomain]`
or a standalone `types_aiobotocore_cloudsearchdomain` package, you have to explicitly specify
`client: CloudSearchDomainClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudSearchDomainClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient
from types_aiobotocore_cloudsearchdomain.type_defs import SearchResponseTypeDef
from types_aiobotocore_cloudsearchdomain.type_defs import SearchRequestTypeDef


session = get_session()

async with session.create_client("cloudsearchdomain") as client:
    client: CloudSearchDomainClient
    kwargs: SearchRequestTypeDef = {...}
    result: SearchResponseTypeDef = await client.search(**kwargs)
```





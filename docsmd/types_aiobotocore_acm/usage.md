# Examples

> [Index](../README.md) > [ACM](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#acm)
    type annotations stubs module [types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[acm]` package installed.

Write your `ACM` code as usual,
type checking and code completion should work out of the box.



```python
# ACMClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("acm") as client:  # (1)
    result = await client.add_tags_to_certificate()  # (2)
```

1. client: [ACMClient](./client.md)
2. result: [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 



```python
# ListCertificatesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("acm") as client:  # (1)
    paginator = client.get_paginator("list_certificates")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ACMClient](./client.md)
2. paginator: [ListCertificatesPaginator](./paginators.md#listcertificatespaginator)
3. item: [:material-code-braces: ListCertificatesResponseTypeDef](./type_defs.md#listcertificatesresponsetypedef) 



```python
# CertificateValidatedWaiter usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("acm") as client:  # (1)
    waiter = client.get_waiter("certificate_validated")  # (2)
    await waiter.wait()
```

1. client: [ACMClient](./client.md)
2. waiter: [CertificateValidatedWaiter](./waiters.md#certificatevalidatedwaiter)


### Explicit type annotations

With `types-aiobotocore-lite[acm]`
or a standalone `types_aiobotocore_acm` package, you have to explicitly specify
`client: ACMClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ACMClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_acm.client import ACMClient
from types_aiobotocore_acm.type_defs import EmptyResponseMetadataTypeDef
from types_aiobotocore_acm.type_defs import AddTagsToCertificateRequestTypeDef


session = get_session()

async with session.create_client("acm") as client:
    client: ACMClient
    kwargs: AddTagsToCertificateRequestTypeDef = {...}
    result: EmptyResponseMetadataTypeDef = await client.add_tags_to_certificate(**kwargs)
```



```python
# ListCertificatesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_acm.client import ACMClient
from types_aiobotocore_acm.paginator import ListCertificatesPaginator
from types_aiobotocore_acm.type_defs import ListCertificatesResponseTypeDef


session = get_session()

async with session.create_client("acm") as client:
    client: ACMClient
    paginator: ListCertificatesPaginator = client.get_paginator("list_certificates")
    async for item in paginator.paginate(...):
        item: ListCertificatesResponseTypeDef
        print(item)
```



```python
# CertificateValidatedWaiter usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_acm.client import ACMClient
from types_aiobotocore_acm.waiter import CertificateValidatedWaiter


session = get_session()

async with session.create_client("acm") as client:
    client: ACMClient
    waiter: CertificateValidatedWaiter = client.get_waiter("certificate_validated")
    await waiter.wait()
```

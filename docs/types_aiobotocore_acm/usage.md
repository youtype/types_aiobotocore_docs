<a id="examples-for-aiobotocore-acm-module"></a>

# Examples for aiobotocore ACM module

> [Index](../README.md) > [ACM](./README.md) > Examples

- [Examples for aiobotocore ACM module](#examples-for-aiobotocore-acm-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[acm]` package installed.

Write your `ACM` code as usual, type checking and code completion should work
out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ACMClient
# and provides type checking and code completion
async with session.create_client("acm") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_tags_to_certificate()
    

    
    # paginator has type ListCertificatesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_certificates")
    async for item in paginator.paginate(...):
        # item has type ListCertificatesResponseTypeDef
        print(item)
    

    
    # waiter has type CertificateValidatedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("certificate_validated")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[acm]` or a standalone `types_aiobotocore_acm`
package, you have to explicitly specify `client: ACMClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_acm.client import ACMClient
from types_aiobotocore_acm.type_defs import None
from types_aiobotocore_acm.paginator import ListCertificatesPaginator
from types_aiobotocore_acm.waiter import CertificateValidatedWaiter
from types_aiobotocore_acm.literals import PaginatorName
from types_aiobotocore_acm.literals import WaiterName


session = get_session()

async with session.create_client("acm") as client:
    client: ACMClient

    
    result: None = client.add_tags_to_certificate()
    

    
    paginator_name: PaginatorName = "list_certificates"
    paginator: ListCertificatesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListCertificatesResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "certificate_validated"
    waiter: CertificateValidatedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```

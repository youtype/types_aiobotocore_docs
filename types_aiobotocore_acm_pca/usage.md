<a id="examples-for-aiobotocore-acmpca-module"></a>

# Examples for aiobotocore ACMPCA module

> [Index](../README.md) > [ACMPCA](./README.md) > Examples

- [Examples for aiobotocore ACMPCA module](#examples-for-aiobotocore-acmpca-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[acm-pca]` package installed.

Write your `ACMPCA` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ACMPCAClient
# and provides type checking and code completion
async with session.create_client("acm-pca") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListCertificateAuthoritiesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_certificate_authorities")
    async for item in paginator.paginate(...):
        # item has type ListCertificateAuthoritiesResponseTypeDef
        print(item)
    

    
    # waiter has type AuditReportCreatedWaiter and provides type checking
    # and code completion for wait method
    waiter = client.get_waiter("audit_report_created")
    await waiter.wait()
    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[acm-pca]` or a standalone
`types_aiobotocore_acm_pca` package, you have to explicitly specify
`client: ACMPCAClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_acm_pca.client import ACMPCAClient
from types_aiobotocore_acm_pca.type_defs import bool
from types_aiobotocore_acm_pca.paginator import ListCertificateAuthoritiesPaginator
from types_aiobotocore_acm_pca.waiter import AuditReportCreatedWaiter
from types_aiobotocore_acm_pca.literals import PaginatorName
from types_aiobotocore_acm_pca.literals import WaiterName


session = get_session()

async with session.create_client("acm-pca") as client:
    client: ACMPCAClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_certificate_authorities"
    paginator: ListCertificateAuthoritiesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListCertificateAuthoritiesResponseTypeDef
        print(item)
    

    
    waiter_name: WaiterName = "audit_report_created"
    waiter: AuditReportCreatedWaiter = client.get_waiter(waiter_name)
    await waiter.wait()
    
```

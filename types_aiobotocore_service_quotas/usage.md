<a id="examples-for-aiobotocore-servicequotas-module"></a>

# Examples for aiobotocore ServiceQuotas module

> [Index](../README.md) > [ServiceQuotas](./README.md) > Examples

- [Examples for aiobotocore ServiceQuotas module](#examples-for-aiobotocore-servicequotas-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[service-quotas]` package installed.

Write your `ServiceQuotas` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type ServiceQuotasClient
# and provides type checking and code completion
async with session.create_client("service-quotas") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_service_quota_template()
    

    
    # paginator has type ListAWSDefaultServiceQuotasPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_aws_default_service_quotas")
    async for item in paginator.paginate(...):
        # item has type ListAWSDefaultServiceQuotasResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[service-quotas]` or a standalone
`types_aiobotocore_service_quotas` package, you have to explicitly specify
`client: ServiceQuotasClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.client import ServiceQuotasClient
from types_aiobotocore_service_quotas.type_defs import Dict[str, Any]
from types_aiobotocore_service_quotas.paginator import ListAWSDefaultServiceQuotasPaginator

from types_aiobotocore_service_quotas.literals import PaginatorName



session = get_session()

async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient

    
    result: Dict[str, Any] = client.associate_service_quota_template()
    

    
    paginator_name: PaginatorName = "list_aws_default_service_quotas"
    paginator: ListAWSDefaultServiceQuotasPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAWSDefaultServiceQuotasResponseTypeDef
        print(item)
    

    
```

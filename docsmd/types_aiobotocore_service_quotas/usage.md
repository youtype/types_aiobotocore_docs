# Examples

> [Index](../README.md) > [ServiceQuotas](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [ServiceQuotas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/service-quotas.html#servicequotas)
    type annotations stubs module [types-aiobotocore-service-quotas](https://pypi.org/project/types-aiobotocore-service-quotas/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[service-quotas]` package installed.

Write your `ServiceQuotas` code as usual,
type checking and code completion should work out of the box.



```python
# ServiceQuotasClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("service-quotas") as client:  # (1)
    result = await client.get_aws_default_service_quota()  # (2)
```

1. client: [ServiceQuotasClient](./client.md)
2. result: [:material-code-braces: GetAWSDefaultServiceQuotaResponseTypeDef](./type_defs.md#getawsdefaultservicequotaresponsetypedef) 



```python
# ListAWSDefaultServiceQuotasPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("service-quotas") as client:  # (1)
    paginator = client.get_paginator("list_aws_default_service_quotas")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [ServiceQuotasClient](./client.md)
2. paginator: [ListAWSDefaultServiceQuotasPaginator](./paginators.md#listawsdefaultservicequotaspaginator)
3. item: [:material-code-braces: ListAWSDefaultServiceQuotasResponseTypeDef](./type_defs.md#listawsdefaultservicequotasresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[service-quotas]`
or a standalone `types_aiobotocore_service_quotas` package, you have to explicitly specify
`client: ServiceQuotasClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# ServiceQuotasClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.client import ServiceQuotasClient
from types_aiobotocore_service_quotas.type_defs import GetAWSDefaultServiceQuotaResponseTypeDef
from types_aiobotocore_service_quotas.type_defs import GetAWSDefaultServiceQuotaRequestTypeDef


session = get_session()

async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
    kwargs: GetAWSDefaultServiceQuotaRequestTypeDef = {...}
    result: GetAWSDefaultServiceQuotaResponseTypeDef = await client.get_aws_default_service_quota(**kwargs)
```



```python
# ListAWSDefaultServiceQuotasPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_service_quotas.client import ServiceQuotasClient
from types_aiobotocore_service_quotas.paginator import ListAWSDefaultServiceQuotasPaginator
from types_aiobotocore_service_quotas.type_defs import ListAWSDefaultServiceQuotasResponseTypeDef


session = get_session()

async with session.create_client("service-quotas") as client:
    client: ServiceQuotasClient
    paginator: ListAWSDefaultServiceQuotasPaginator = client.get_paginator("list_aws_default_service_quotas")
    async for item in paginator.paginate(...):
        item: ListAWSDefaultServiceQuotasResponseTypeDef
        print(item)
```



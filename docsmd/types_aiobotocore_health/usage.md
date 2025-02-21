# Examples

> [Index](../README.md) > [Health](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Health](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/health.html#health)
    type annotations stubs module [types-aiobotocore-health](https://pypi.org/project/types-aiobotocore-health/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[health]` package installed.

Write your `Health` code as usual,
type checking and code completion should work out of the box.



```python
# HealthClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("health") as client:  # (1)
    result = await client.describe_affected_accounts_for_organization()  # (2)
```

1. client: [HealthClient](./client.md)
2. result: [:material-code-braces: DescribeAffectedAccountsForOrganizationResponseTypeDef](./type_defs.md#describeaffectedaccountsfororganizationresponsetypedef) 



```python
# DescribeAffectedAccountsForOrganizationPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("health") as client:  # (1)
    paginator = client.get_paginator("describe_affected_accounts_for_organization")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [HealthClient](./client.md)
2. paginator: [DescribeAffectedAccountsForOrganizationPaginator](./paginators.md#describeaffectedaccountsfororganizationpaginator)
3. item: [:material-code-braces: DescribeAffectedAccountsForOrganizationResponseTypeDef](./type_defs.md#describeaffectedaccountsfororganizationresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[health]`
or a standalone `types_aiobotocore_health` package, you have to explicitly specify
`client: HealthClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# HealthClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_health.client import HealthClient
from types_aiobotocore_health.type_defs import DescribeAffectedAccountsForOrganizationResponseTypeDef
from types_aiobotocore_health.type_defs import DescribeAffectedAccountsForOrganizationRequestTypeDef


session = get_session()

async with session.create_client("health") as client:
    client: HealthClient
    kwargs: DescribeAffectedAccountsForOrganizationRequestTypeDef = {...}
    result: DescribeAffectedAccountsForOrganizationResponseTypeDef = await client.describe_affected_accounts_for_organization(**kwargs)
```



```python
# DescribeAffectedAccountsForOrganizationPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_health.client import HealthClient
from types_aiobotocore_health.paginator import DescribeAffectedAccountsForOrganizationPaginator
from types_aiobotocore_health.type_defs import DescribeAffectedAccountsForOrganizationResponseTypeDef


session = get_session()

async with session.create_client("health") as client:
    client: HealthClient
    paginator: DescribeAffectedAccountsForOrganizationPaginator = client.get_paginator("describe_affected_accounts_for_organization")
    async for item in paginator.paginate(...):
        item: DescribeAffectedAccountsForOrganizationResponseTypeDef
        print(item)
```



# Examples

> [Index](../README.md) > [SecurityIncidentResponse](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [SecurityIncidentResponse](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#securityincidentresponse)
    type annotations stubs module [types-aiobotocore-security-ir](https://pypi.org/project/types-aiobotocore-security-ir/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[security-ir]` package installed.

Write your `SecurityIncidentResponse` code as usual,
type checking and code completion should work out of the box.



```python
# SecurityIncidentResponseClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("security-ir") as client:  # (1)
    result = await client.batch_get_member_account_details()  # (2)
```

1. client: [SecurityIncidentResponseClient](./client.md)
2. result: [:material-code-braces: BatchGetMemberAccountDetailsResponseTypeDef](./type_defs.md#batchgetmemberaccountdetailsresponsetypedef) 



```python
# ListCaseEditsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("security-ir") as client:  # (1)
    paginator = client.get_paginator("list_case_edits")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [SecurityIncidentResponseClient](./client.md)
2. paginator: [ListCaseEditsPaginator](./paginators.md#listcaseeditspaginator)
3. item: [:material-code-braces: ListCaseEditsResponseTypeDef](./type_defs.md#listcaseeditsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[security-ir]`
or a standalone `types_aiobotocore_security_ir` package, you have to explicitly specify
`client: SecurityIncidentResponseClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# SecurityIncidentResponseClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_security_ir.client import SecurityIncidentResponseClient
from types_aiobotocore_security_ir.type_defs import BatchGetMemberAccountDetailsResponseTypeDef
from types_aiobotocore_security_ir.type_defs import BatchGetMemberAccountDetailsRequestTypeDef


session = get_session()

async with session.create_client("security-ir") as client:
    client: SecurityIncidentResponseClient
    kwargs: BatchGetMemberAccountDetailsRequestTypeDef = {...}
    result: BatchGetMemberAccountDetailsResponseTypeDef = await client.batch_get_member_account_details(**kwargs)
```



```python
# ListCaseEditsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_security_ir.client import SecurityIncidentResponseClient
from types_aiobotocore_security_ir.paginator import ListCaseEditsPaginator
from types_aiobotocore_security_ir.type_defs import ListCaseEditsResponseTypeDef


session = get_session()

async with session.create_client("security-ir") as client:
    client: SecurityIncidentResponseClient
    paginator: ListCaseEditsPaginator = client.get_paginator("list_case_edits")
    async for item in paginator.paginate(...):
        item: ListCaseEditsResponseTypeDef
        print(item)
```



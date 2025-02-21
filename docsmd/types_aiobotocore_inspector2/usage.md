# Examples

> [Index](../README.md) > [Inspector2](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#inspector2)
    type annotations stubs module [types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[inspector2]` package installed.

Write your `Inspector2` code as usual,
type checking and code completion should work out of the box.



```python
# Inspector2Client usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("inspector2") as client:  # (1)
    result = await client.associate_member()  # (2)
```

1. client: [Inspector2Client](./client.md)
2. result: [:material-code-braces: AssociateMemberResponseTypeDef](./type_defs.md#associatememberresponsetypedef) 



```python
# GetCisScanResultDetailsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("inspector2") as client:  # (1)
    paginator = client.get_paginator("get_cis_scan_result_details")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [Inspector2Client](./client.md)
2. paginator: [GetCisScanResultDetailsPaginator](./paginators.md#getcisscanresultdetailspaginator)
3. item: [:material-code-braces: GetCisScanResultDetailsResponseTypeDef](./type_defs.md#getcisscanresultdetailsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[inspector2]`
or a standalone `types_aiobotocore_inspector2` package, you have to explicitly specify
`client: Inspector2Client` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# Inspector2Client usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.client import Inspector2Client
from types_aiobotocore_inspector2.type_defs import AssociateMemberResponseTypeDef
from types_aiobotocore_inspector2.type_defs import AssociateMemberRequestTypeDef


session = get_session()

async with session.create_client("inspector2") as client:
    client: Inspector2Client
    kwargs: AssociateMemberRequestTypeDef = {...}
    result: AssociateMemberResponseTypeDef = await client.associate_member(**kwargs)
```



```python
# GetCisScanResultDetailsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_inspector2.client import Inspector2Client
from types_aiobotocore_inspector2.paginator import GetCisScanResultDetailsPaginator
from types_aiobotocore_inspector2.type_defs import GetCisScanResultDetailsResponseTypeDef


session = get_session()

async with session.create_client("inspector2") as client:
    client: Inspector2Client
    paginator: GetCisScanResultDetailsPaginator = client.get_paginator("get_cis_scan_result_details")
    async for item in paginator.paginate(...):
        item: GetCisScanResultDetailsResponseTypeDef
        print(item)
```



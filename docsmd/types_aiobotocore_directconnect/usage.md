# Examples

> [Index](../README.md) > [DirectConnect](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [DirectConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#directconnect)
    type annotations stubs module [types-aiobotocore-directconnect](https://pypi.org/project/types-aiobotocore-directconnect/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[directconnect]` package installed.

Write your `DirectConnect` code as usual,
type checking and code completion should work out of the box.



```python
# DirectConnectClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("directconnect") as client:  # (1)
    result = await client.accept_direct_connect_gateway_association_proposal()  # (2)
```

1. client: [DirectConnectClient](./client.md)
2. result: [:material-code-braces: AcceptDirectConnectGatewayAssociationProposalResultTypeDef](./type_defs.md#acceptdirectconnectgatewayassociationproposalresulttypedef) 



```python
# DescribeDirectConnectGatewayAssociationsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("directconnect") as client:  # (1)
    paginator = client.get_paginator("describe_direct_connect_gateway_associations")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [DirectConnectClient](./client.md)
2. paginator: [DescribeDirectConnectGatewayAssociationsPaginator](./paginators.md#describedirectconnectgatewayassociationspaginator)
3. item: [:material-code-braces: DescribeDirectConnectGatewayAssociationsResultTypeDef](./type_defs.md#describedirectconnectgatewayassociationsresulttypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[directconnect]`
or a standalone `types_aiobotocore_directconnect` package, you have to explicitly specify
`client: DirectConnectClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# DirectConnectClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_directconnect.client import DirectConnectClient
from types_aiobotocore_directconnect.type_defs import AcceptDirectConnectGatewayAssociationProposalResultTypeDef
from types_aiobotocore_directconnect.type_defs import AcceptDirectConnectGatewayAssociationProposalRequestTypeDef


session = get_session()

async with session.create_client("directconnect") as client:
    client: DirectConnectClient
    kwargs: AcceptDirectConnectGatewayAssociationProposalRequestTypeDef = {...}
    result: AcceptDirectConnectGatewayAssociationProposalResultTypeDef = await client.accept_direct_connect_gateway_association_proposal(**kwargs)
```



```python
# DescribeDirectConnectGatewayAssociationsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_directconnect.client import DirectConnectClient
from types_aiobotocore_directconnect.paginator import DescribeDirectConnectGatewayAssociationsPaginator
from types_aiobotocore_directconnect.type_defs import DescribeDirectConnectGatewayAssociationsResultTypeDef


session = get_session()

async with session.create_client("directconnect") as client:
    client: DirectConnectClient
    paginator: DescribeDirectConnectGatewayAssociationsPaginator = client.get_paginator("describe_direct_connect_gateway_associations")
    async for item in paginator.paginate(...):
        item: DescribeDirectConnectGatewayAssociationsResultTypeDef
        print(item)
```



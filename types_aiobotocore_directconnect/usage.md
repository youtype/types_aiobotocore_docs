<a id="examples-for-aiobotocore-directconnect-module"></a>

# Examples for aiobotocore DirectConnect module

> [Index](../README.md) > [DirectConnect](./README.md) > Examples

- [Examples for aiobotocore DirectConnect module](#examples-for-aiobotocore-directconnect-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[directconnect]` package installed.

Write your `DirectConnect` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type DirectConnectClient
# and provides type checking and code completion
async with session.create_client("directconnect") as client:
    
    # result has type AcceptDirectConnectGatewayAssociationProposalResultTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.accept_direct_connect_gateway_association_proposal()
    

    
    # paginator has type DescribeDirectConnectGatewayAssociationsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_direct_connect_gateway_associations")
    async for item in paginator.paginate(...):
        # item has type DescribeDirectConnectGatewayAssociationsResultTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[directconnect]` or a standalone
`types_aiobotocore_directconnect` package, you have to explicitly specify
`client: DirectConnectClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_directconnect.client import DirectConnectClient
from types_aiobotocore_directconnect.type_defs import AcceptDirectConnectGatewayAssociationProposalResultTypeDef
from types_aiobotocore_directconnect.paginator import DescribeDirectConnectGatewayAssociationsPaginator

from types_aiobotocore_directconnect.literals import PaginatorName



session = get_session()

async with session.create_client("directconnect") as client:
    client: DirectConnectClient

    
    result: AcceptDirectConnectGatewayAssociationProposalResultTypeDef = client.accept_direct_connect_gateway_association_proposal()
    

    
    paginator_name: PaginatorName = "describe_direct_connect_gateway_associations"
    paginator: DescribeDirectConnectGatewayAssociationsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeDirectConnectGatewayAssociationsResultTypeDef
        print(item)
    

    
```

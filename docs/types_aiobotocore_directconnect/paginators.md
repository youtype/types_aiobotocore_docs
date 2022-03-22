<a id="paginators-for-aiobotocore-directconnect-module"></a>

# Paginators for aiobotocore DirectConnect module

> [Index](../README.md) > [DirectConnect](./README.md) > Paginators

Auto-generated documentation for
[DirectConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
type annotations stubs module
[types-aiobotocore-directconnect](https://pypi.org/project/types-aiobotocore-directconnect/).

- [Paginators for aiobotocore DirectConnect module](#paginators-for-aiobotocore-directconnect-module)
  - [DescribeDirectConnectGatewayAssociationsPaginator](#describedirectconnectgatewayassociationspaginator)
  - [DescribeDirectConnectGatewayAttachmentsPaginator](#describedirectconnectgatewayattachmentspaginator)
  - [DescribeDirectConnectGatewaysPaginator](#describedirectconnectgatewayspaginator)

<a id="describedirectconnectgatewayassociationspaginator"></a>

## DescribeDirectConnectGatewayAssociationsPaginator

Type annotations for
`session.create_client("directconnect").get_paginator("describe_direct_connect_gateway_associations")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_directconnect.paginator import DescribeDirectConnectGatewayAssociationsPaginator

session = get_session()
async with session.create_client("directconnect") as client:
    client: DirectConnectClient
    paginator: DescribeDirectConnectGatewayAssociationsPaginator = client.get_paginator("describe_direct_connect_gateway_associations")
```

Boto3 documentation:
[DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations)

Arguments for `DescribeDirectConnectGatewayAssociationsPaginator.paginate`
method:

- `associationId`: `str`
- `associatedGatewayId`: `str`
- `directConnectGatewayId`: `str`
- `virtualGatewayId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDirectConnectGatewayAssociationsPaginator.paginate` returns
`AsyncIterator`\[[DescribeDirectConnectGatewayAssociationsResultTypeDef](./type_defs.md#describedirectconnectgatewayassociationsresulttypedef)\].

<a id="describedirectconnectgatewayattachmentspaginator"></a>

## DescribeDirectConnectGatewayAttachmentsPaginator

Type annotations for
`session.create_client("directconnect").get_paginator("describe_direct_connect_gateway_attachments")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_directconnect.paginator import DescribeDirectConnectGatewayAttachmentsPaginator

session = get_session()
async with session.create_client("directconnect") as client:
    client: DirectConnectClient
    paginator: DescribeDirectConnectGatewayAttachmentsPaginator = client.get_paginator("describe_direct_connect_gateway_attachments")
```

Boto3 documentation:
[DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments)

Arguments for `DescribeDirectConnectGatewayAttachmentsPaginator.paginate`
method:

- `directConnectGatewayId`: `str`
- `virtualInterfaceId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDirectConnectGatewayAttachmentsPaginator.paginate` returns
`AsyncIterator`\[[DescribeDirectConnectGatewayAttachmentsResultTypeDef](./type_defs.md#describedirectconnectgatewayattachmentsresulttypedef)\].

<a id="describedirectconnectgatewayspaginator"></a>

## DescribeDirectConnectGatewaysPaginator

Type annotations for
`session.create_client("directconnect").get_paginator("describe_direct_connect_gateways")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_directconnect.paginator import DescribeDirectConnectGatewaysPaginator

session = get_session()
async with session.create_client("directconnect") as client:
    client: DirectConnectClient
    paginator: DescribeDirectConnectGatewaysPaginator = client.get_paginator("describe_direct_connect_gateways")
```

Boto3 documentation:
[DirectConnect.Paginator.DescribeDirectConnectGateways](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)

Arguments for `DescribeDirectConnectGatewaysPaginator.paginate` method:

- `directConnectGatewayId`: `str`
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`DescribeDirectConnectGatewaysPaginator.paginate` returns
`AsyncIterator`\[[DescribeDirectConnectGatewaysResultTypeDef](./type_defs.md#describedirectconnectgatewaysresulttypedef)\].

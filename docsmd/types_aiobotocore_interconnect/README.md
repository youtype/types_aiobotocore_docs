# Interconnect module

> [Index](../README.md) > Interconnect


!!! note ""

    Auto-generated documentation for [Interconnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/interconnect.html#interconnect)
    type annotations stubs module [types-aiobotocore-interconnect](https://pypi.org/project/types-aiobotocore-interconnect/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.7.0' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Interconnect` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Interconnect` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[interconnect]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[interconnect]'

# standalone installation
python -m pip install types-aiobotocore-interconnect
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-interconnect
```

## Usage

Code samples can be found in [Examples](./usage.md).

## InterconnectClient

Type annotations and code completion for  `#!python session.create_client("interconnect")` as [InterconnectClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/interconnect.html#Interconnect.Client)

```python
# InterconnectClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_interconnect.client import InterconnectClient


session = get_session()
async with session.create_client("interconnect") as client:
    client: InterconnectClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("interconnect").get_paginator("...")`.

```python
# ListAttachPointsPaginator usage example

from types_aiobotocore_interconnect.paginator import ListAttachPointsPaginator

def get_list_attach_points_paginator() -> ListAttachPointsPaginator:
    return client.get_paginator("list_attach_points"))
```

- [ListAttachPointsPaginator](./paginators.md#listattachpointspaginator)
- [ListConnectionsPaginator](./paginators.md#listconnectionspaginator)
- [ListEnvironmentsPaginator](./paginators.md#listenvironmentspaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("interconnect").get_waiter("...")`.

```python
# ConnectionAvailableWaiter usage example

from types_aiobotocore_interconnect.waiter import ConnectionAvailableWaiter

def get_connection_available_waiter() -> ConnectionAvailableWaiter:
    return Session().client("interconnect").get_waiter("connection_available")
```

- [ConnectionAvailableWaiter](./waiters.md#connectionavailablewaiter)
- [ConnectionDeletedWaiter](./waiters.md#connectiondeletedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AttachPointTypeType usage example

from types_aiobotocore_interconnect.literals import AttachPointTypeType

def get_value() -> AttachPointTypeType:
    return "DirectConnectGateway"
```

- [AttachPointTypeType](./literals.md#attachpointtypetype)
- [ConnectionAvailableWaiterName](./literals.md#connectionavailablewaitername)
- [ConnectionDeletedWaiterName](./literals.md#connectiondeletedwaitername)
- [ConnectionStateType](./literals.md#connectionstatetype)
- [EnvironmentStateType](./literals.md#environmentstatetype)
- [ListAttachPointsPaginatorName](./literals.md#listattachpointspaginatorname)
- [ListConnectionsPaginatorName](./literals.md#listconnectionspaginatorname)
- [ListEnvironmentsPaginatorName](./literals.md#listenvironmentspaginatorname)
- [RemoteAccountIdentifierTypeType](./literals.md#remoteaccountidentifiertypetype)
- [InterconnectServiceName](./literals.md#interconnectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AttachPointTypeDef](./type_defs.md#attachpointtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [AttachPointDescriptorTypeDef](./type_defs.md#attachpointdescriptortypedef)
- [BandwidthsTypeDef](./type_defs.md#bandwidthstypedef)
- [ProviderTypeDef](./type_defs.md#providertypedef)
- [RemoteAccountIdentifierTypeDef](./type_defs.md#remoteaccountidentifiertypedef)
- [DeleteConnectionRequestTypeDef](./type_defs.md#deleteconnectionrequesttypedef)
- [DescribeConnectionProposalRequestTypeDef](./type_defs.md#describeconnectionproposalrequesttypedef)
- [GetConnectionRequestTypeDef](./type_defs.md#getconnectionrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [GetEnvironmentRequestTypeDef](./type_defs.md#getenvironmentrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAttachPointsRequestTypeDef](./type_defs.md#listattachpointsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateConnectionRequestTypeDef](./type_defs.md#updateconnectionrequesttypedef)
- [AcceptConnectionProposalRequestTypeDef](./type_defs.md#acceptconnectionproposalrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListAttachPointsResponseTypeDef](./type_defs.md#listattachpointsresponsetypedef)
- [ConnectionSummaryTypeDef](./type_defs.md#connectionsummarytypedef)
- [ConnectionTypeDef](./type_defs.md#connectiontypedef)
- [DescribeConnectionProposalResponseTypeDef](./type_defs.md#describeconnectionproposalresponsetypedef)
- [EnvironmentTypeDef](./type_defs.md#environmenttypedef)
- [ListConnectionsRequestTypeDef](./type_defs.md#listconnectionsrequesttypedef)
- [ListEnvironmentsRequestTypeDef](./type_defs.md#listenvironmentsrequesttypedef)
- [CreateConnectionRequestTypeDef](./type_defs.md#createconnectionrequesttypedef)
- [GetConnectionRequestWaitExtraTypeDef](./type_defs.md#getconnectionrequestwaitextratypedef)
- [GetConnectionRequestWaitTypeDef](./type_defs.md#getconnectionrequestwaittypedef)
- [ListAttachPointsRequestPaginateTypeDef](./type_defs.md#listattachpointsrequestpaginatetypedef)
- [ListConnectionsRequestPaginateTypeDef](./type_defs.md#listconnectionsrequestpaginatetypedef)
- [ListEnvironmentsRequestPaginateTypeDef](./type_defs.md#listenvironmentsrequestpaginatetypedef)
- [ListConnectionsResponseTypeDef](./type_defs.md#listconnectionsresponsetypedef)
- [AcceptConnectionProposalResponseTypeDef](./type_defs.md#acceptconnectionproposalresponsetypedef)
- [CreateConnectionResponseTypeDef](./type_defs.md#createconnectionresponsetypedef)
- [DeleteConnectionResponseTypeDef](./type_defs.md#deleteconnectionresponsetypedef)
- [GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef)
- [UpdateConnectionResponseTypeDef](./type_defs.md#updateconnectionresponsetypedef)
- [GetEnvironmentResponseTypeDef](./type_defs.md#getenvironmentresponsetypedef)
- [ListEnvironmentsResponseTypeDef](./type_defs.md#listenvironmentsresponsetypedef)


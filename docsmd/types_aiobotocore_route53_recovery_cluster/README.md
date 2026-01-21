# Route53RecoveryCluster module

> [Index](../README.md) > Route53RecoveryCluster


!!! note ""

    Auto-generated documentation for [Route53RecoveryCluster](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#route53recoverycluster)
    type annotations stubs module [types-aiobotocore-route53-recovery-cluster](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `Route53RecoveryCluster` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `Route53RecoveryCluster` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[route53-recovery-cluster]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[route53-recovery-cluster]'

# standalone installation
python -m pip install types-aiobotocore-route53-recovery-cluster
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-route53-recovery-cluster
```

## Usage

Code samples can be found in [Examples](./usage.md).

## Route53RecoveryClusterClient

Type annotations and code completion for  `#!python session.create_client("route53-recovery-cluster")` as [Route53RecoveryClusterClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Client)

```python
# Route53RecoveryClusterClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_route53_recovery_cluster.client import Route53RecoveryClusterClient


session = get_session()
async with session.create_client("route53-recovery-cluster") as client:
    client: Route53RecoveryClusterClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("route53-recovery-cluster").get_paginator("...")`.

```python
# ListRoutingControlsPaginator usage example

from types_aiobotocore_route53_recovery_cluster.paginator import ListRoutingControlsPaginator

def get_list_routing_controls_paginator() -> ListRoutingControlsPaginator:
    return client.get_paginator("list_routing_controls"))
```

- [ListRoutingControlsPaginator](./paginators.md#listroutingcontrolspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ListRoutingControlsPaginatorName usage example

from types_aiobotocore_route53_recovery_cluster.literals import ListRoutingControlsPaginatorName

def get_value() -> ListRoutingControlsPaginatorName:
    return "list_routing_controls"
```

- [ListRoutingControlsPaginatorName](./literals.md#listroutingcontrolspaginatorname)
- [RoutingControlStateType](./literals.md#routingcontrolstatetype)
- [Route53RecoveryClusterServiceName](./literals.md#route53recoveryclusterservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [GetRoutingControlStateRequestTypeDef](./type_defs.md#getroutingcontrolstaterequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListRoutingControlsRequestTypeDef](./type_defs.md#listroutingcontrolsrequesttypedef)
- [RoutingControlTypeDef](./type_defs.md#routingcontroltypedef)
- [UpdateRoutingControlStateEntryTypeDef](./type_defs.md#updateroutingcontrolstateentrytypedef)
- [UpdateRoutingControlStateRequestTypeDef](./type_defs.md#updateroutingcontrolstaterequesttypedef)
- [GetRoutingControlStateResponseTypeDef](./type_defs.md#getroutingcontrolstateresponsetypedef)
- [ListRoutingControlsRequestPaginateTypeDef](./type_defs.md#listroutingcontrolsrequestpaginatetypedef)
- [ListRoutingControlsResponseTypeDef](./type_defs.md#listroutingcontrolsresponsetypedef)
- [UpdateRoutingControlStatesRequestTypeDef](./type_defs.md#updateroutingcontrolstatesrequesttypedef)


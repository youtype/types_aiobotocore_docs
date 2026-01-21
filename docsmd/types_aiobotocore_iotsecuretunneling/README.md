# IoTSecureTunneling module

> [Index](../README.md) > IoTSecureTunneling


!!! note ""

    Auto-generated documentation for [IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#iotsecuretunneling)
    type annotations stubs module [types-aiobotocore-iotsecuretunneling](https://pypi.org/project/types-aiobotocore-iotsecuretunneling/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `IoTSecureTunneling` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `IoTSecureTunneling` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iotsecuretunneling]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iotsecuretunneling]'

# standalone installation
python -m pip install types-aiobotocore-iotsecuretunneling
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iotsecuretunneling
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTSecureTunnelingClient

Type annotations and code completion for  `#!python session.create_client("iotsecuretunneling")` as [IoTSecureTunnelingClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client)

```python
# IoTSecureTunnelingClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotsecuretunneling.client import IoTSecureTunnelingClient


session = get_session()
async with session.create_client("iotsecuretunneling") as client:
    client: IoTSecureTunnelingClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ClientModeType usage example

from types_aiobotocore_iotsecuretunneling.literals import ClientModeType

def get_value() -> ClientModeType:
    return "ALL"
```

- [ClientModeType](./literals.md#clientmodetype)
- [ConnectionStatusType](./literals.md#connectionstatustype)
- [TunnelStatusType](./literals.md#tunnelstatustype)
- [IoTSecureTunnelingServiceName](./literals.md#iotsecuretunnelingservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CloseTunnelRequestTypeDef](./type_defs.md#closetunnelrequesttypedef)
- [ConnectionStateTypeDef](./type_defs.md#connectionstatetypedef)
- [DescribeTunnelRequestTypeDef](./type_defs.md#describetunnelrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DestinationConfigOutputTypeDef](./type_defs.md#destinationconfigoutputtypedef)
- [DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ListTunnelsRequestTypeDef](./type_defs.md#listtunnelsrequesttypedef)
- [TunnelSummaryTypeDef](./type_defs.md#tunnelsummarytypedef)
- [TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [OpenTunnelResponseTypeDef](./type_defs.md#opentunnelresponsetypedef)
- [RotateTunnelAccessTokenResponseTypeDef](./type_defs.md#rotatetunnelaccesstokenresponsetypedef)
- [DestinationConfigUnionTypeDef](./type_defs.md#destinationconfiguniontypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [ListTunnelsResponseTypeDef](./type_defs.md#listtunnelsresponsetypedef)
- [TunnelTypeDef](./type_defs.md#tunneltypedef)
- [OpenTunnelRequestTypeDef](./type_defs.md#opentunnelrequesttypedef)
- [RotateTunnelAccessTokenRequestTypeDef](./type_defs.md#rotatetunnelaccesstokenrequesttypedef)
- [DescribeTunnelResponseTypeDef](./type_defs.md#describetunnelresponsetypedef)


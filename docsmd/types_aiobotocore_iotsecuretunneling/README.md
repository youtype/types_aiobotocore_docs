# IoTSecureTunneling module

> [Index](../README.md) > IoTSecureTunneling


!!! note ""

    Auto-generated documentation for [IoTSecureTunneling](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
    type annotations stubs module [types-aiobotocore-iotsecuretunneling](https://pypi.org/project/types-aiobotocore-iotsecuretunneling/).

## How to install



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

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_iotsecuretunneling.client import IoTSecureTunnelingClient


session = get_session()
async with session.create_client("iotsecuretunneling") as client:
    client: IoTSecureTunnelingClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
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




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef

def get_value() -> CloseTunnelRequestRequestTypeDef:
    return {
        "tunnelId": ...,
    }
```

- [CloseTunnelRequestRequestTypeDef](./type_defs.md#closetunnelrequestrequesttypedef)
- [ConnectionStateTypeDef](./type_defs.md#connectionstatetypedef)
- [DescribeTunnelRequestRequestTypeDef](./type_defs.md#describetunnelrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DestinationConfigTypeDef](./type_defs.md#destinationconfigtypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ListTunnelsRequestRequestTypeDef](./type_defs.md#listtunnelsrequestrequesttypedef)
- [TunnelSummaryTypeDef](./type_defs.md#tunnelsummarytypedef)
- [TimeoutConfigTypeDef](./type_defs.md#timeoutconfigtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [OpenTunnelResponseTypeDef](./type_defs.md#opentunnelresponsetypedef)
- [RotateTunnelAccessTokenResponseTypeDef](./type_defs.md#rotatetunnelaccesstokenresponsetypedef)
- [RotateTunnelAccessTokenRequestRequestTypeDef](./type_defs.md#rotatetunnelaccesstokenrequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ListTunnelsResponseTypeDef](./type_defs.md#listtunnelsresponsetypedef)
- [OpenTunnelRequestRequestTypeDef](./type_defs.md#opentunnelrequestrequesttypedef)
- [TunnelTypeDef](./type_defs.md#tunneltypedef)
- [DescribeTunnelResponseTypeDef](./type_defs.md#describetunnelresponsetypedef)


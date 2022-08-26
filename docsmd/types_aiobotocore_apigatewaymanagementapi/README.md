# ApiGatewayManagementApi module

> [Index](../README.md) > ApiGatewayManagementApi


!!! note ""

    Auto-generated documentation for [ApiGatewayManagementApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
    type annotations stubs module [types-aiobotocore-apigatewaymanagementapi](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ApiGatewayManagementApi` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[apigatewaymanagementapi]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[apigatewaymanagementapi]'


# standalone installation
python -m pip install types-aiobotocore-apigatewaymanagementapi
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-apigatewaymanagementapi
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ApiGatewayManagementApiClient

Type annotations and code completion for  `#!python session.create_client("apigatewaymanagementapi")` as [ApiGatewayManagementApiClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient


session = get_session()
async with session.create_client("apigatewaymanagementapi") as client:
    client: ApiGatewayManagementApiClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_apigatewaymanagementapi.literals import ApiGatewayManagementApiServiceName

def get_value() -> ApiGatewayManagementApiServiceName:
    return "apigatewaymanagementapi"
```

- [ApiGatewayManagementApiServiceName](./literals.md#apigatewaymanagementapiservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_apigatewaymanagementapi.type_defs import DeleteConnectionRequestRequestTypeDef

def get_value() -> DeleteConnectionRequestRequestTypeDef:
    return {
        "ConnectionId": ...,
    }
```

- [DeleteConnectionRequestRequestTypeDef](./type_defs.md#deleteconnectionrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [GetConnectionRequestRequestTypeDef](./type_defs.md#getconnectionrequestrequesttypedef)
- [IdentityTypeDef](./type_defs.md#identitytypedef)
- [PostToConnectionRequestRequestTypeDef](./type_defs.md#posttoconnectionrequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetConnectionResponseTypeDef](./type_defs.md#getconnectionresponsetypedef)


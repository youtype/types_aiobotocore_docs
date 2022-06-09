# SSOOIDC module

> [Index](../README.md) > SSOOIDC


!!! note ""

    Auto-generated documentation for [SSOOIDC](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
    type annotations stubs module [types-aiobotocore-sso-oidc](https://pypi.org/project/types-aiobotocore-sso-oidc/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `SSOOIDC`.

### From PyPI with pip

Install `types-aiobotocore` for `SSOOIDC` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sso-oidc]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sso-oidc]'


# standalone installation
python -m pip install types-aiobotocore-sso-oidc
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sso-oidc
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SSOOIDCClient

Type annotations and code completion for  `#!python session.create_client("sso-oidc")` as [SSOOIDCClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_oidc.client import SSOOIDCClient


session = get_session()
async with session.create_client("sso-oidc") as client:
    client: SSOOIDCClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sso_oidc.literals import SSOOIDCServiceName

def get_value() -> SSOOIDCServiceName:
    return "sso-oidc"
```

- [SSOOIDCServiceName](./literals.md#ssooidcservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef

def get_value() -> CreateTokenRequestRequestTypeDef:
    return {
        "clientId": ...,
        "clientSecret": ...,
        "grantType": ...,
        "deviceCode": ...,
    }
```

- [CreateTokenRequestRequestTypeDef](./type_defs.md#createtokenrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [RegisterClientRequestRequestTypeDef](./type_defs.md#registerclientrequestrequesttypedef)
- [StartDeviceAuthorizationRequestRequestTypeDef](./type_defs.md#startdeviceauthorizationrequestrequesttypedef)
- [CreateTokenResponseTypeDef](./type_defs.md#createtokenresponsetypedef)
- [RegisterClientResponseTypeDef](./type_defs.md#registerclientresponsetypedef)
- [StartDeviceAuthorizationResponseTypeDef](./type_defs.md#startdeviceauthorizationresponsetypedef)


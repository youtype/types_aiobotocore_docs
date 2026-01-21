# SignInService module

> [Index](../README.md) > SignInService


!!! note ""

    Auto-generated documentation for [SignInService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#signinservice)
    type annotations stubs module [types-aiobotocore-signin](https://pypi.org/project/types-aiobotocore-signin/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SignInService` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SignInService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[signin]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[signin]'

# standalone installation
python -m pip install types-aiobotocore-signin
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-signin
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SignInServiceClient

Type annotations and code completion for  `#!python session.create_client("signin")` as [SignInServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#SignInService.Client)

```python
# SignInServiceClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_signin.client import SignInServiceClient


session = get_session()
async with session.create_client("signin") as client:
    client: SignInServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# SignInServiceServiceName usage example

from types_aiobotocore_signin.literals import SignInServiceServiceName

def get_value() -> SignInServiceServiceName:
    return "signin"
```

- [SignInServiceServiceName](./literals.md#signinserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccessTokenTypeDef](./type_defs.md#accesstokentypedef)
- [CreateOAuth2TokenRequestBodyTypeDef](./type_defs.md#createoauth2tokenrequestbodytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateOAuth2TokenResponseBodyTypeDef](./type_defs.md#createoauth2tokenresponsebodytypedef)
- [CreateOAuth2TokenRequestTypeDef](./type_defs.md#createoauth2tokenrequesttypedef)
- [CreateOAuth2TokenResponseTypeDef](./type_defs.md#createoauth2tokenresponsetypedef)


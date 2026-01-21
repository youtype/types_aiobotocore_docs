# STS module

> [Index](../README.md) > STS


!!! note ""

    Auto-generated documentation for [STS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#sts)
    type annotations stubs module [types-aiobotocore-sts](https://pypi.org/project/types-aiobotocore-sts/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `STS` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `STS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sts]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sts]'

# standalone installation
python -m pip install types-aiobotocore-sts
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sts
```

## Usage

Code samples can be found in [Examples](./usage.md).

## STSClient

Type annotations and code completion for  `#!python session.create_client("sts")` as [STSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client)

```python
# STSClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_sts.client import STSClient


session = get_session()
async with session.create_client("sts") as client:
    client: STSClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# STSServiceName usage example

from types_aiobotocore_sts.literals import STSServiceName

def get_value() -> STSServiceName:
    return "sts"
```

- [STSServiceName](./literals.md#stsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef)
- [ProvidedContextTypeDef](./type_defs.md#providedcontexttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [AssumedRoleUserTypeDef](./type_defs.md#assumedroleusertypedef)
- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DecodeAuthorizationMessageRequestTypeDef](./type_defs.md#decodeauthorizationmessagerequesttypedef)
- [FederatedUserTypeDef](./type_defs.md#federatedusertypedef)
- [GetAccessKeyInfoRequestTypeDef](./type_defs.md#getaccesskeyinforequesttypedef)
- [GetDelegatedAccessTokenRequestTypeDef](./type_defs.md#getdelegatedaccesstokenrequesttypedef)
- [GetSessionTokenRequestTypeDef](./type_defs.md#getsessiontokenrequesttypedef)
- [AssumeRoleWithSAMLRequestTypeDef](./type_defs.md#assumerolewithsamlrequesttypedef)
- [AssumeRoleWithWebIdentityRequestTypeDef](./type_defs.md#assumerolewithwebidentityrequesttypedef)
- [AssumeRootRequestTypeDef](./type_defs.md#assumerootrequesttypedef)
- [AssumeRoleRequestTypeDef](./type_defs.md#assumerolerequesttypedef)
- [GetFederationTokenRequestTypeDef](./type_defs.md#getfederationtokenrequesttypedef)
- [GetWebIdentityTokenRequestTypeDef](./type_defs.md#getwebidentitytokenrequesttypedef)
- [AssumeRoleResponseTypeDef](./type_defs.md#assumeroleresponsetypedef)
- [AssumeRoleWithSAMLResponseTypeDef](./type_defs.md#assumerolewithsamlresponsetypedef)
- [AssumeRoleWithWebIdentityResponseTypeDef](./type_defs.md#assumerolewithwebidentityresponsetypedef)
- [AssumeRootResponseTypeDef](./type_defs.md#assumerootresponsetypedef)
- [DecodeAuthorizationMessageResponseTypeDef](./type_defs.md#decodeauthorizationmessageresponsetypedef)
- [GetAccessKeyInfoResponseTypeDef](./type_defs.md#getaccesskeyinforesponsetypedef)
- [GetCallerIdentityResponseTypeDef](./type_defs.md#getcalleridentityresponsetypedef)
- [GetDelegatedAccessTokenResponseTypeDef](./type_defs.md#getdelegatedaccesstokenresponsetypedef)
- [GetSessionTokenResponseTypeDef](./type_defs.md#getsessiontokenresponsetypedef)
- [GetWebIdentityTokenResponseTypeDef](./type_defs.md#getwebidentitytokenresponsetypedef)
- [GetFederationTokenResponseTypeDef](./type_defs.md#getfederationtokenresponsetypedef)


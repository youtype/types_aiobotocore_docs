<a id="type-annotations-for-aiobotocore-ssooidc-module"></a>

# Type annotations for aiobotocore SSOOIDC module

> [Index](..) > SSOOIDC

Auto-generated documentation for
[SSOOIDC](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
type annotations stubs module
[types-aiobotocore-sso-oidc](https://pypi.org/project/types-aiobotocore-sso-oidc/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[sso-oidc]'

# install as a standalone
pip install types-aiobotocore-sso-oidc
```

- [Type annotations for aiobotocore SSOOIDC module](#type-annotations-for-aiobotocore-ssooidc-module)
  - [SSOOIDCClient](#ssooidcclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="ssooidcclient"></a>

## SSOOIDCClient

Type annotations for `aiobotocore.create_client("sso-oidc")` as
[SSOOIDCClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_sso_oidc.client import SSOOIDCClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [create_token](./client.md#create_token)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [register_client](./client.md#register_client)
- [start_device_authorization](./client.md#start_device_authorization)

<a id="exceptions"></a>

### Exceptions

SSOOIDCClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- AuthorizationPendingException
- ClientError
- ExpiredTokenException
- InternalServerException
- InvalidClientException
- InvalidClientMetadataException
- InvalidGrantException
- InvalidRequestException
- InvalidScopeException
- SlowDownException
- UnauthorizedClientException
- UnsupportedGrantTypeException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_sso_oidc.literals import ServiceName, ...
```

- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef, ...
```

- [CreateTokenRequestRequestTypeDef](./type_defs.md#createtokenrequestrequesttypedef)
- [CreateTokenResponseTypeDef](./type_defs.md#createtokenresponsetypedef)
- [RegisterClientRequestRequestTypeDef](./type_defs.md#registerclientrequestrequesttypedef)
- [RegisterClientResponseTypeDef](./type_defs.md#registerclientresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [StartDeviceAuthorizationRequestRequestTypeDef](./type_defs.md#startdeviceauthorizationrequestrequesttypedef)
- [StartDeviceAuthorizationResponseTypeDef](./type_defs.md#startdeviceauthorizationresponsetypedef)

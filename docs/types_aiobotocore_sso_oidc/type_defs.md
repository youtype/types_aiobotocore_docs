<a id="typed-dictionaries-for-aiobotocore-ssooidc-module"></a>

# Typed dictionaries for aiobotocore SSOOIDC module

> [Index](../README.md) > [SSOOIDC](./README.md) > Typed dictionaries

Auto-generated documentation for
[SSOOIDC](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
type annotations stubs module
[types-aiobotocore-sso-oidc](https://pypi.org/project/types-aiobotocore-sso-oidc/).

- [Typed dictionaries for aiobotocore SSOOIDC module](#typed-dictionaries-for-aiobotocore-ssooidc-module)
  - [CreateTokenRequestRequestTypeDef](#createtokenrequestrequesttypedef)
  - [CreateTokenResponseTypeDef](#createtokenresponsetypedef)
  - [RegisterClientRequestRequestTypeDef](#registerclientrequestrequesttypedef)
  - [RegisterClientResponseTypeDef](#registerclientresponsetypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [StartDeviceAuthorizationRequestRequestTypeDef](#startdeviceauthorizationrequestrequesttypedef)
  - [StartDeviceAuthorizationResponseTypeDef](#startdeviceauthorizationresponsetypedef)

<a id="createtokenrequestrequesttypedef"></a>

## CreateTokenRequestRequestTypeDef

```python
from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef
```

Required fields:

- `clientId`: `str`
- `clientSecret`: `str`
- `grantType`: `str`
- `deviceCode`: `str`

Optional fields:

- `code`: `str`
- `refreshToken`: `str`
- `scope`: `Sequence`\[`str`\]
- `redirectUri`: `str`

<a id="createtokenresponsetypedef"></a>

## CreateTokenResponseTypeDef

```python
from types_aiobotocore_sso_oidc.type_defs import CreateTokenResponseTypeDef
```

Required fields:

- `accessToken`: `str`
- `tokenType`: `str`
- `expiresIn`: `int`
- `refreshToken`: `str`
- `idToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="registerclientrequestrequesttypedef"></a>

## RegisterClientRequestRequestTypeDef

```python
from types_aiobotocore_sso_oidc.type_defs import RegisterClientRequestRequestTypeDef
```

Required fields:

- `clientName`: `str`
- `clientType`: `str`

Optional fields:

- `scopes`: `Sequence`\[`str`\]

<a id="registerclientresponsetypedef"></a>

## RegisterClientResponseTypeDef

```python
from types_aiobotocore_sso_oidc.type_defs import RegisterClientResponseTypeDef
```

Required fields:

- `clientId`: `str`
- `clientSecret`: `str`
- `clientIdIssuedAt`: `int`
- `clientSecretExpiresAt`: `int`
- `authorizationEndpoint`: `str`
- `tokenEndpoint`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_sso_oidc.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="startdeviceauthorizationrequestrequesttypedef"></a>

## StartDeviceAuthorizationRequestRequestTypeDef

```python
from types_aiobotocore_sso_oidc.type_defs import StartDeviceAuthorizationRequestRequestTypeDef
```

Required fields:

- `clientId`: `str`
- `clientSecret`: `str`
- `startUrl`: `str`

<a id="startdeviceauthorizationresponsetypedef"></a>

## StartDeviceAuthorizationResponseTypeDef

```python
from types_aiobotocore_sso_oidc.type_defs import StartDeviceAuthorizationResponseTypeDef
```

Required fields:

- `deviceCode`: `str`
- `userCode`: `str`
- `verificationUri`: `str`
- `verificationUriComplete`: `str`
- `expiresIn`: `int`
- `interval`: `int`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

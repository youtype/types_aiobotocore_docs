# Type definitions

> [Index](../README.md) > [SSOOIDC](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SSOOIDC](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#ssooidc)
    type annotations stubs module [types-aiobotocore-sso-oidc](https://pypi.org/project/types-aiobotocore-sso-oidc/).



## CreateTokenRequestRequestTypeDef

```python
# CreateTokenRequestRequestTypeDef definition

class CreateTokenRequestRequestTypeDef(TypedDict):
    clientId: str,
    clientSecret: str,
    grantType: str,
    deviceCode: NotRequired[str],
    code: NotRequired[str],
    refreshToken: NotRequired[str],
    scope: NotRequired[Sequence[str]],
    redirectUri: NotRequired[str],
    codeVerifier: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## CreateTokenWithIAMRequestRequestTypeDef

```python
# CreateTokenWithIAMRequestRequestTypeDef definition

class CreateTokenWithIAMRequestRequestTypeDef(TypedDict):
    clientId: str,
    grantType: str,
    code: NotRequired[str],
    refreshToken: NotRequired[str],
    assertion: NotRequired[str],
    scope: NotRequired[Sequence[str]],
    redirectUri: NotRequired[str],
    subjectToken: NotRequired[str],
    subjectTokenType: NotRequired[str],
    requestedTokenType: NotRequired[str],
    codeVerifier: NotRequired[str],
```

## RegisterClientRequestRequestTypeDef

```python
# RegisterClientRequestRequestTypeDef definition

class RegisterClientRequestRequestTypeDef(TypedDict):
    clientName: str,
    clientType: str,
    scopes: NotRequired[Sequence[str]],
    redirectUris: NotRequired[Sequence[str]],
    grantTypes: NotRequired[Sequence[str]],
    issuerUrl: NotRequired[str],
    entitledApplicationArn: NotRequired[str],
```

## StartDeviceAuthorizationRequestRequestTypeDef

```python
# StartDeviceAuthorizationRequestRequestTypeDef definition

class StartDeviceAuthorizationRequestRequestTypeDef(TypedDict):
    clientId: str,
    clientSecret: str,
    startUrl: str,
```

## CreateTokenResponseTypeDef

```python
# CreateTokenResponseTypeDef definition

class CreateTokenResponseTypeDef(TypedDict):
    accessToken: str,
    tokenType: str,
    expiresIn: int,
    refreshToken: str,
    idToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTokenWithIAMResponseTypeDef

```python
# CreateTokenWithIAMResponseTypeDef definition

class CreateTokenWithIAMResponseTypeDef(TypedDict):
    accessToken: str,
    tokenType: str,
    expiresIn: int,
    refreshToken: str,
    idToken: str,
    issuedTokenType: str,
    scope: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterClientResponseTypeDef

```python
# RegisterClientResponseTypeDef definition

class RegisterClientResponseTypeDef(TypedDict):
    clientId: str,
    clientSecret: str,
    clientIdIssuedAt: int,
    clientSecretExpiresAt: int,
    authorizationEndpoint: str,
    tokenEndpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDeviceAuthorizationResponseTypeDef

```python
# StartDeviceAuthorizationResponseTypeDef definition

class StartDeviceAuthorizationResponseTypeDef(TypedDict):
    deviceCode: str,
    userCode: str,
    verificationUri: str,
    verificationUriComplete: str,
    expiresIn: int,
    interval: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

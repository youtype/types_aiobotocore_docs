# Type definitions

> [Index](../README.md) > [SignInService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SignInService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signin.html#signinservice)
    type annotations stubs module [types-aiobotocore-signin](https://pypi.org/project/types-aiobotocore-signin/).



## AccessTokenTypeDef

```python
# AccessTokenTypeDef TypedDict usage example

from types_aiobotocore_signin.type_defs import AccessTokenTypeDef


def get_value() -> AccessTokenTypeDef:
    return {
        "accessKeyId": ...,
    }


# AccessTokenTypeDef definition

class AccessTokenTypeDef(TypedDict):
    accessKeyId: str,
    secretAccessKey: str,
    sessionToken: str,
```


## CreateOAuth2TokenRequestBodyTypeDef

```python
# CreateOAuth2TokenRequestBodyTypeDef TypedDict usage example

from types_aiobotocore_signin.type_defs import CreateOAuth2TokenRequestBodyTypeDef


def get_value() -> CreateOAuth2TokenRequestBodyTypeDef:
    return {
        "clientId": ...,
    }


# CreateOAuth2TokenRequestBodyTypeDef definition

class CreateOAuth2TokenRequestBodyTypeDef(TypedDict):
    clientId: str,
    grantType: str,
    code: NotRequired[str],
    redirectUri: NotRequired[str],
    codeVerifier: NotRequired[str],
    refreshToken: NotRequired[str],
```


## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_signin.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## CreateOAuth2TokenResponseBodyTypeDef

```python
# CreateOAuth2TokenResponseBodyTypeDef TypedDict usage example

from types_aiobotocore_signin.type_defs import CreateOAuth2TokenResponseBodyTypeDef


def get_value() -> CreateOAuth2TokenResponseBodyTypeDef:
    return {
        "accessToken": ...,
    }


# CreateOAuth2TokenResponseBodyTypeDef definition

class CreateOAuth2TokenResponseBodyTypeDef(TypedDict):
    accessToken: AccessTokenTypeDef,  # (1)
    tokenType: str,
    expiresIn: int,
    refreshToken: str,
    idToken: NotRequired[str],
```

1. See [:material-code-braces: AccessTokenTypeDef](./type_defs.md#accesstokentypedef)

## CreateOAuth2TokenRequestTypeDef

```python
# CreateOAuth2TokenRequestTypeDef TypedDict usage example

from types_aiobotocore_signin.type_defs import CreateOAuth2TokenRequestTypeDef


def get_value() -> CreateOAuth2TokenRequestTypeDef:
    return {
        "tokenInput": ...,
    }


# CreateOAuth2TokenRequestTypeDef definition

class CreateOAuth2TokenRequestTypeDef(TypedDict):
    tokenInput: CreateOAuth2TokenRequestBodyTypeDef,  # (1)
```

1. See [:material-code-braces: CreateOAuth2TokenRequestBodyTypeDef](./type_defs.md#createoauth2tokenrequestbodytypedef)

## CreateOAuth2TokenResponseTypeDef

```python
# CreateOAuth2TokenResponseTypeDef TypedDict usage example

from types_aiobotocore_signin.type_defs import CreateOAuth2TokenResponseTypeDef


def get_value() -> CreateOAuth2TokenResponseTypeDef:
    return {
        "tokenOutput": ...,
    }


# CreateOAuth2TokenResponseTypeDef definition

class CreateOAuth2TokenResponseTypeDef(TypedDict):
    tokenOutput: CreateOAuth2TokenResponseBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateOAuth2TokenResponseBodyTypeDef](./type_defs.md#createoauth2tokenresponsebodytypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)


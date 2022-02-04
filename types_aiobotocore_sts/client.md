<a id="stsclient-for-aiobotocore-sts-module"></a>

# STSClient for aiobotocore STS module

> [Index](..) > [STS](.) > STSClient

Auto-generated documentation for
[STS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
type annotations stubs module
[types-aiobotocore-sts](https://pypi.org/project/types-aiobotocore-sts/).

- [STSClient for aiobotocore STS module](#stsclient-for-aiobotocore-sts-module)
  - [STSClient](#stsclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [assume_role](#assume_role)
    - [assume_role_with_saml](#assume_role_with_saml)
    - [assume_role_with_web_identity](#assume_role_with_web_identity)
    - [can_paginate](#can_paginate)
    - [decode_authorization_message](#decode_authorization_message)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_access_key_info](#get_access_key_info)
    - [get_caller_identity](#get_caller_identity)
    - [get_federation_token](#get_federation_token)
    - [get_session_token](#get_session_token)

<a id="stsclient"></a>

## STSClient

Type annotations for `aiobotocore.create_client("sts")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_sts.client import STSClient

def get_sts_client() -> STSClient:
    return Session().client("sts")
```

Boto3 documentation:
[STS.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_sts.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.ExpiredTokenException`
- `Exceptions.IDPCommunicationErrorException`
- `Exceptions.IDPRejectedClaimException`
- `Exceptions.InvalidAuthorizationMessageException`
- `Exceptions.InvalidIdentityTokenException`
- `Exceptions.MalformedPolicyDocumentException`
- `Exceptions.PackedPolicyTooLargeException`
- `Exceptions.RegionDisabledException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

STSClient exceptions.

Type annotations for `aiobotocore.create_client("sts").exceptions` method.

Boto3 documentation:
[STS.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="assume_role"></a>

### assume_role

Returns a set of temporary security credentials that you can use to access
Amazon Web Services resources that you might not normally have access to.

Type annotations for `aiobotocore.create_client("sts").assume_role` method.

Boto3 documentation:
[STS.Client.assume_role](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role)

Asynchronous method. Use `await assume_role(...)` for a synchronous call.

Arguments mapping described in
[AssumeRoleRequestRequestTypeDef](./type_defs.md#assumerolerequestrequesttypedef).

Keyword-only arguments:

- `RoleArn`: `str` *(required)*
- `RoleSessionName`: `str` *(required)*
- `PolicyArns`:
  `Sequence`\[[PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef)\]
- `Policy`: `str`
- `DurationSeconds`: `int`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `TransitiveTagKeys`: `Sequence`\[`str`\]
- `ExternalId`: `str`
- `SerialNumber`: `str`
- `TokenCode`: `str`
- `SourceIdentity`: `str`

Returns a `Coroutine` for
[AssumeRoleResponseTypeDef](./type_defs.md#assumeroleresponsetypedef).

<a id="assume_role_with_saml"></a>

### assume_role_with_saml

Returns a set of temporary security credentials for users who have been
authenticated via a SAML authentication response.

Type annotations for `aiobotocore.create_client("sts").assume_role_with_saml`
method.

Boto3 documentation:
[STS.Client.assume_role_with_saml](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role_with_saml)

Asynchronous method. Use `await assume_role_with_saml(...)` for a synchronous
call.

Arguments mapping described in
[AssumeRoleWithSAMLRequestRequestTypeDef](./type_defs.md#assumerolewithsamlrequestrequesttypedef).

Keyword-only arguments:

- `RoleArn`: `str` *(required)*
- `PrincipalArn`: `str` *(required)*
- `SAMLAssertion`: `str` *(required)*
- `PolicyArns`:
  `Sequence`\[[PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef)\]
- `Policy`: `str`
- `DurationSeconds`: `int`

Returns a `Coroutine` for
[AssumeRoleWithSAMLResponseTypeDef](./type_defs.md#assumerolewithsamlresponsetypedef).

<a id="assume_role_with_web_identity"></a>

### assume_role_with_web_identity

Returns a set of temporary security credentials for users who have been
authenticated in a mobile or web application with a web identity provider.

Type annotations for
`aiobotocore.create_client("sts").assume_role_with_web_identity` method.

Boto3 documentation:
[STS.Client.assume_role_with_web_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role_with_web_identity)

Asynchronous method. Use `await assume_role_with_web_identity(...)` for a
synchronous call.

Arguments mapping described in
[AssumeRoleWithWebIdentityRequestRequestTypeDef](./type_defs.md#assumerolewithwebidentityrequestrequesttypedef).

Keyword-only arguments:

- `RoleArn`: `str` *(required)*
- `RoleSessionName`: `str` *(required)*
- `WebIdentityToken`: `str` *(required)*
- `ProviderId`: `str`
- `PolicyArns`:
  `Sequence`\[[PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef)\]
- `Policy`: `str`
- `DurationSeconds`: `int`

Returns a `Coroutine` for
[AssumeRoleWithWebIdentityResponseTypeDef](./type_defs.md#assumerolewithwebidentityresponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("sts").can_paginate` method.

Boto3 documentation:
[STS.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="decode_authorization_message"></a>

### decode_authorization_message

Decodes additional information about the authorization status of a request from
an encoded message returned in response to an Amazon Web Services request.

Type annotations for
`aiobotocore.create_client("sts").decode_authorization_message` method.

Boto3 documentation:
[STS.Client.decode_authorization_message](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.decode_authorization_message)

Asynchronous method. Use `await decode_authorization_message(...)` for a
synchronous call.

Arguments mapping described in
[DecodeAuthorizationMessageRequestRequestTypeDef](./type_defs.md#decodeauthorizationmessagerequestrequesttypedef).

Keyword-only arguments:

- `EncodedMessage`: `str` *(required)*

Returns a `Coroutine` for
[DecodeAuthorizationMessageResponseTypeDef](./type_defs.md#decodeauthorizationmessageresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for `aiobotocore.create_client("sts").generate_presigned_url`
method.

Boto3 documentation:
[STS.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_access_key_info"></a>

### get_access_key_info

Returns the account identifier for the specified access key ID.

Type annotations for `aiobotocore.create_client("sts").get_access_key_info`
method.

Boto3 documentation:
[STS.Client.get_access_key_info](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.get_access_key_info)

Asynchronous method. Use `await get_access_key_info(...)` for a synchronous
call.

Arguments mapping described in
[GetAccessKeyInfoRequestRequestTypeDef](./type_defs.md#getaccesskeyinforequestrequesttypedef).

Keyword-only arguments:

- `AccessKeyId`: `str` *(required)*

Returns a `Coroutine` for
[GetAccessKeyInfoResponseTypeDef](./type_defs.md#getaccesskeyinforesponsetypedef).

<a id="get_caller_identity"></a>

### get_caller_identity

Returns details about the IAM user or role whose credentials are used to call
the operation.

Type annotations for `aiobotocore.create_client("sts").get_caller_identity`
method.

Boto3 documentation:
[STS.Client.get_caller_identity](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.get_caller_identity)

Asynchronous method. Use `await get_caller_identity(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetCallerIdentityResponseTypeDef](./type_defs.md#getcalleridentityresponsetypedef).

<a id="get_federation_token"></a>

### get_federation_token

Returns a set of temporary security credentials (consisting of an access key
ID, a secret access key, and a security token) for a federated user.

Type annotations for `aiobotocore.create_client("sts").get_federation_token`
method.

Boto3 documentation:
[STS.Client.get_federation_token](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.get_federation_token)

Asynchronous method. Use `await get_federation_token(...)` for a synchronous
call.

Arguments mapping described in
[GetFederationTokenRequestRequestTypeDef](./type_defs.md#getfederationtokenrequestrequesttypedef).

Keyword-only arguments:

- `Name`: `str` *(required)*
- `Policy`: `str`
- `PolicyArns`:
  `Sequence`\[[PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef)\]
- `DurationSeconds`: `int`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

Returns a `Coroutine` for
[GetFederationTokenResponseTypeDef](./type_defs.md#getfederationtokenresponsetypedef).

<a id="get_session_token"></a>

### get_session_token

Returns a set of temporary credentials for an Amazon Web Services account or
IAM user.

Type annotations for `aiobotocore.create_client("sts").get_session_token`
method.

Boto3 documentation:
[STS.Client.get_session_token](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.get_session_token)

Asynchronous method. Use `await get_session_token(...)` for a synchronous call.

Arguments mapping described in
[GetSessionTokenRequestRequestTypeDef](./type_defs.md#getsessiontokenrequestrequesttypedef).

Keyword-only arguments:

- `DurationSeconds`: `int`
- `SerialNumber`: `str`
- `TokenCode`: `str`

Returns a `Coroutine` for
[GetSessionTokenResponseTypeDef](./type_defs.md#getsessiontokenresponsetypedef).

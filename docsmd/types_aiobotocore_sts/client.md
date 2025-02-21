# STSClient

> [Index](../README.md) > [STS](./README.md) > STSClient

!!! note ""

    Auto-generated documentation for [STS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#sts)
    type annotations stubs module [types-aiobotocore-sts](https://pypi.org/project/types-aiobotocore-sts/).

## STSClient

Type annotations and code completion for `#!python session.create_client("sts")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client)

```python
# STSClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_sts.client import STSClient

session = get_session()
async with session.create_client("sts") as client:
    client: STSClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sts").exceptions` structure.

```python
# STSClient.exceptions usage example

async with session.create_client("sts") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.ExpiredTokenException,
        client.IDPCommunicationErrorException,
        client.IDPRejectedClaimException,
        client.InvalidAuthorizationMessageException,
        client.InvalidIdentityTokenException,
        client.MalformedPolicyDocumentException,
        client.PackedPolicyTooLargeException,
        client.RegionDisabledException,
    ) as e:
        print(e)
```

```python
# STSClient usage type checking example

from types_aiobotocore_sts.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("sts").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("sts").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### assume\_role

Returns a set of temporary security credentials that you can use to access
Amazon Web Services resources.

Type annotations and code completion for `#!python session.create_client("sts").assume_role` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/assume_role.html)

```python
# assume_role method definition

await def assume_role(
    self,
    *,
    RoleArn: str,
    RoleSessionName: str,
    PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,  # (1)
    Policy: str = ...,
    DurationSeconds: int = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
    TransitiveTagKeys: Sequence[str] = ...,
    ExternalId: str = ...,
    SerialNumber: str = ...,
    TokenCode: str = ...,
    SourceIdentity: str = ...,
    ProvidedContexts: Sequence[ProvidedContextTypeDef] = ...,  # (3)
) -> AssumeRoleResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ProvidedContextTypeDef](./type_defs.md#providedcontexttypedef) 
4. See [:material-code-braces: AssumeRoleResponseTypeDef](./type_defs.md#assumeroleresponsetypedef) 


```python
# assume_role method usage example with argument unpacking

kwargs: AssumeRoleRequestTypeDef = {  # (1)
    "RoleArn": ...,
    "RoleSessionName": ...,
}

parent.assume_role(**kwargs)
```

1. See [:material-code-braces: AssumeRoleRequestTypeDef](./type_defs.md#assumerolerequesttypedef) 

### assume\_role\_with\_saml

Returns a set of temporary security credentials for users who have been
authenticated via a SAML authentication response.

Type annotations and code completion for `#!python session.create_client("sts").assume_role_with_saml` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/assume_role_with_saml.html)

```python
# assume_role_with_saml method definition

await def assume_role_with_saml(
    self,
    *,
    RoleArn: str,
    PrincipalArn: str,
    SAMLAssertion: str,
    PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,  # (1)
    Policy: str = ...,
    DurationSeconds: int = ...,
) -> AssumeRoleWithSAMLResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
2. See [:material-code-braces: AssumeRoleWithSAMLResponseTypeDef](./type_defs.md#assumerolewithsamlresponsetypedef) 


```python
# assume_role_with_saml method usage example with argument unpacking

kwargs: AssumeRoleWithSAMLRequestTypeDef = {  # (1)
    "RoleArn": ...,
    "PrincipalArn": ...,
    "SAMLAssertion": ...,
}

parent.assume_role_with_saml(**kwargs)
```

1. See [:material-code-braces: AssumeRoleWithSAMLRequestTypeDef](./type_defs.md#assumerolewithsamlrequesttypedef) 

### assume\_role\_with\_web\_identity

Returns a set of temporary security credentials for users who have been
authenticated in a mobile or web application with a web identity provider.

Type annotations and code completion for `#!python session.create_client("sts").assume_role_with_web_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/assume_role_with_web_identity.html)

```python
# assume_role_with_web_identity method definition

await def assume_role_with_web_identity(
    self,
    *,
    RoleArn: str,
    RoleSessionName: str,
    WebIdentityToken: str,
    ProviderId: str = ...,
    PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,  # (1)
    Policy: str = ...,
    DurationSeconds: int = ...,
) -> AssumeRoleWithWebIdentityResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
2. See [:material-code-braces: AssumeRoleWithWebIdentityResponseTypeDef](./type_defs.md#assumerolewithwebidentityresponsetypedef) 


```python
# assume_role_with_web_identity method usage example with argument unpacking

kwargs: AssumeRoleWithWebIdentityRequestTypeDef = {  # (1)
    "RoleArn": ...,
    "RoleSessionName": ...,
    "WebIdentityToken": ...,
}

parent.assume_role_with_web_identity(**kwargs)
```

1. See [:material-code-braces: AssumeRoleWithWebIdentityRequestTypeDef](./type_defs.md#assumerolewithwebidentityrequesttypedef) 

### assume\_root

Returns a set of short term credentials you can use to perform privileged tasks
on a member account in your organization.

Type annotations and code completion for `#!python session.create_client("sts").assume_root` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/assume_root.html)

```python
# assume_root method definition

await def assume_root(
    self,
    *,
    TargetPrincipal: str,
    TaskPolicyArn: PolicyDescriptorTypeTypeDef,  # (1)
    DurationSeconds: int = ...,
) -> AssumeRootResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
2. See [:material-code-braces: AssumeRootResponseTypeDef](./type_defs.md#assumerootresponsetypedef) 


```python
# assume_root method usage example with argument unpacking

kwargs: AssumeRootRequestTypeDef = {  # (1)
    "TargetPrincipal": ...,
    "TaskPolicyArn": ...,
}

parent.assume_root(**kwargs)
```

1. See [:material-code-braces: AssumeRootRequestTypeDef](./type_defs.md#assumerootrequesttypedef) 

### decode\_authorization\_message

Decodes additional information about the authorization status of a request from
an encoded message returned in response to an Amazon Web Services request.

Type annotations and code completion for `#!python session.create_client("sts").decode_authorization_message` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/decode_authorization_message.html)

```python
# decode_authorization_message method definition

await def decode_authorization_message(
    self,
    *,
    EncodedMessage: str,
) -> DecodeAuthorizationMessageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DecodeAuthorizationMessageResponseTypeDef](./type_defs.md#decodeauthorizationmessageresponsetypedef) 


```python
# decode_authorization_message method usage example with argument unpacking

kwargs: DecodeAuthorizationMessageRequestTypeDef = {  # (1)
    "EncodedMessage": ...,
}

parent.decode_authorization_message(**kwargs)
```

1. See [:material-code-braces: DecodeAuthorizationMessageRequestTypeDef](./type_defs.md#decodeauthorizationmessagerequesttypedef) 

### get\_access\_key\_info

Returns the account identifier for the specified access key ID.

Type annotations and code completion for `#!python session.create_client("sts").get_access_key_info` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/get_access_key_info.html)

```python
# get_access_key_info method definition

await def get_access_key_info(
    self,
    *,
    AccessKeyId: str,
) -> GetAccessKeyInfoResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccessKeyInfoResponseTypeDef](./type_defs.md#getaccesskeyinforesponsetypedef) 


```python
# get_access_key_info method usage example with argument unpacking

kwargs: GetAccessKeyInfoRequestTypeDef = {  # (1)
    "AccessKeyId": ...,
}

parent.get_access_key_info(**kwargs)
```

1. See [:material-code-braces: GetAccessKeyInfoRequestTypeDef](./type_defs.md#getaccesskeyinforequesttypedef) 

### get\_caller\_identity

Returns details about the IAM user or role whose credentials are used to call
the operation.

Type annotations and code completion for `#!python session.create_client("sts").get_caller_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/get_caller_identity.html)

```python
# get_caller_identity method definition

await def get_caller_identity(
    self,
) -> GetCallerIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetCallerIdentityResponseTypeDef](./type_defs.md#getcalleridentityresponsetypedef) 

### get\_federation\_token

Returns a set of temporary security credentials (consisting of an access key
ID, a secret access key, and a security token) for a user.

Type annotations and code completion for `#!python session.create_client("sts").get_federation_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/get_federation_token.html)

```python
# get_federation_token method definition

await def get_federation_token(
    self,
    *,
    Name: str,
    Policy: str = ...,
    PolicyArns: Sequence[PolicyDescriptorTypeTypeDef] = ...,  # (1)
    DurationSeconds: int = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> GetFederationTokenResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: GetFederationTokenResponseTypeDef](./type_defs.md#getfederationtokenresponsetypedef) 


```python
# get_federation_token method usage example with argument unpacking

kwargs: GetFederationTokenRequestTypeDef = {  # (1)
    "Name": ...,
}

parent.get_federation_token(**kwargs)
```

1. See [:material-code-braces: GetFederationTokenRequestTypeDef](./type_defs.md#getfederationtokenrequesttypedef) 

### get\_session\_token

Returns a set of temporary credentials for an Amazon Web Services account or
IAM user.

Type annotations and code completion for `#!python session.create_client("sts").get_session_token` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts/client/get_session_token.html)

```python
# get_session_token method definition

await def get_session_token(
    self,
    *,
    DurationSeconds: int = ...,
    SerialNumber: str = ...,
    TokenCode: str = ...,
) -> GetSessionTokenResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSessionTokenResponseTypeDef](./type_defs.md#getsessiontokenresponsetypedef) 


```python
# get_session_token method usage example with argument unpacking

kwargs: GetSessionTokenRequestTypeDef = {  # (1)
    "DurationSeconds": ...,
}

parent.get_session_token(**kwargs)
```

1. See [:material-code-braces: GetSessionTokenRequestTypeDef](./type_defs.md#getsessiontokenrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sts").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sts").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```






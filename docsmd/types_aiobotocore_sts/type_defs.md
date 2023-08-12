# Type definitions

> [Index](../README.md) > [STS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [STS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS)
    type annotations stubs module [types-aiobotocore-sts](https://pypi.org/project/types-aiobotocore-sts/).



## PolicyDescriptorTypeTypeDef

```python
# PolicyDescriptorTypeTypeDef definition

class PolicyDescriptorTypeTypeDef(TypedDict):
    arn: NotRequired[str],
```

## ProvidedContextTypeDef

```python
# ProvidedContextTypeDef definition

class ProvidedContextTypeDef(TypedDict):
    ProviderArn: NotRequired[str],
    ContextAssertion: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## AssumedRoleUserTypeDef

```python
# AssumedRoleUserTypeDef definition

class AssumedRoleUserTypeDef(TypedDict):
    AssumedRoleId: str,
    Arn: str,
```

## CredentialsTypeDef

```python
# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    AccessKeyId: str,
    SecretAccessKey: str,
    SessionToken: str,
    Expiration: datetime,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## DecodeAuthorizationMessageRequestRequestTypeDef

```python
# DecodeAuthorizationMessageRequestRequestTypeDef definition

class DecodeAuthorizationMessageRequestRequestTypeDef(TypedDict):
    EncodedMessage: str,
```

## FederatedUserTypeDef

```python
# FederatedUserTypeDef definition

class FederatedUserTypeDef(TypedDict):
    FederatedUserId: str,
    Arn: str,
```

## GetAccessKeyInfoRequestRequestTypeDef

```python
# GetAccessKeyInfoRequestRequestTypeDef definition

class GetAccessKeyInfoRequestRequestTypeDef(TypedDict):
    AccessKeyId: str,
```

## GetSessionTokenRequestRequestTypeDef

```python
# GetSessionTokenRequestRequestTypeDef definition

class GetSessionTokenRequestRequestTypeDef(TypedDict):
    DurationSeconds: NotRequired[int],
    SerialNumber: NotRequired[str],
    TokenCode: NotRequired[str],
```

## AssumeRoleWithSAMLRequestRequestTypeDef

```python
# AssumeRoleWithSAMLRequestRequestTypeDef definition

class AssumeRoleWithSAMLRequestRequestTypeDef(TypedDict):
    RoleArn: str,
    PrincipalArn: str,
    SAMLAssertion: str,
    PolicyArns: NotRequired[Sequence[PolicyDescriptorTypeTypeDef]],  # (1)
    Policy: NotRequired[str],
    DurationSeconds: NotRequired[int],
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
## AssumeRoleWithWebIdentityRequestRequestTypeDef

```python
# AssumeRoleWithWebIdentityRequestRequestTypeDef definition

class AssumeRoleWithWebIdentityRequestRequestTypeDef(TypedDict):
    RoleArn: str,
    RoleSessionName: str,
    WebIdentityToken: str,
    ProviderId: NotRequired[str],
    PolicyArns: NotRequired[Sequence[PolicyDescriptorTypeTypeDef]],  # (1)
    Policy: NotRequired[str],
    DurationSeconds: NotRequired[int],
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
## AssumeRoleRequestRequestTypeDef

```python
# AssumeRoleRequestRequestTypeDef definition

class AssumeRoleRequestRequestTypeDef(TypedDict):
    RoleArn: str,
    RoleSessionName: str,
    PolicyArns: NotRequired[Sequence[PolicyDescriptorTypeTypeDef]],  # (1)
    Policy: NotRequired[str],
    DurationSeconds: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    TransitiveTagKeys: NotRequired[Sequence[str]],
    ExternalId: NotRequired[str],
    SerialNumber: NotRequired[str],
    TokenCode: NotRequired[str],
    SourceIdentity: NotRequired[str],
    ProvidedContexts: NotRequired[Sequence[ProvidedContextTypeDef]],  # (3)
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ProvidedContextTypeDef](./type_defs.md#providedcontexttypedef) 
## GetFederationTokenRequestRequestTypeDef

```python
# GetFederationTokenRequestRequestTypeDef definition

class GetFederationTokenRequestRequestTypeDef(TypedDict):
    Name: str,
    Policy: NotRequired[str],
    PolicyArns: NotRequired[Sequence[PolicyDescriptorTypeTypeDef]],  # (1)
    DurationSeconds: NotRequired[int],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: PolicyDescriptorTypeTypeDef](./type_defs.md#policydescriptortypetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AssumeRoleResponseTypeDef

```python
# AssumeRoleResponseTypeDef definition

class AssumeRoleResponseTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    AssumedRoleUser: AssumedRoleUserTypeDef,  # (2)
    PackedPolicySize: int,
    SourceIdentity: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: AssumedRoleUserTypeDef](./type_defs.md#assumedroleusertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeRoleWithSAMLResponseTypeDef

```python
# AssumeRoleWithSAMLResponseTypeDef definition

class AssumeRoleWithSAMLResponseTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    AssumedRoleUser: AssumedRoleUserTypeDef,  # (2)
    PackedPolicySize: int,
    Subject: str,
    SubjectType: str,
    Issuer: str,
    Audience: str,
    NameQualifier: str,
    SourceIdentity: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: AssumedRoleUserTypeDef](./type_defs.md#assumedroleusertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssumeRoleWithWebIdentityResponseTypeDef

```python
# AssumeRoleWithWebIdentityResponseTypeDef definition

class AssumeRoleWithWebIdentityResponseTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    SubjectFromWebIdentityToken: str,
    AssumedRoleUser: AssumedRoleUserTypeDef,  # (2)
    PackedPolicySize: int,
    Provider: str,
    Audience: str,
    SourceIdentity: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: AssumedRoleUserTypeDef](./type_defs.md#assumedroleusertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DecodeAuthorizationMessageResponseTypeDef

```python
# DecodeAuthorizationMessageResponseTypeDef definition

class DecodeAuthorizationMessageResponseTypeDef(TypedDict):
    DecodedMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccessKeyInfoResponseTypeDef

```python
# GetAccessKeyInfoResponseTypeDef definition

class GetAccessKeyInfoResponseTypeDef(TypedDict):
    Account: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCallerIdentityResponseTypeDef

```python
# GetCallerIdentityResponseTypeDef definition

class GetCallerIdentityResponseTypeDef(TypedDict):
    UserId: str,
    Account: str,
    Arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSessionTokenResponseTypeDef

```python
# GetSessionTokenResponseTypeDef definition

class GetSessionTokenResponseTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFederationTokenResponseTypeDef

```python
# GetFederationTokenResponseTypeDef definition

class GetFederationTokenResponseTypeDef(TypedDict):
    Credentials: CredentialsTypeDef,  # (1)
    FederatedUser: FederatedUserTypeDef,  # (2)
    PackedPolicySize: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
2. See [:material-code-braces: FederatedUserTypeDef](./type_defs.md#federatedusertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

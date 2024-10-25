# Type definitions

> [Index](../README.md) > [EKSAuth](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [EKSAuth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth)
    type annotations stubs module [types-aiobotocore-eks-auth](https://pypi.org/project/types-aiobotocore-eks-auth/).



## AssumeRoleForPodIdentityRequestRequestTypeDef

```python
# AssumeRoleForPodIdentityRequestRequestTypeDef definition

class AssumeRoleForPodIdentityRequestRequestTypeDef(TypedDict):
    clusterName: str,
    token: str,
```

## AssumedRoleUserTypeDef

```python
# AssumedRoleUserTypeDef definition

class AssumedRoleUserTypeDef(TypedDict):
    arn: str,
    assumeRoleId: str,
```

## CredentialsTypeDef

```python
# CredentialsTypeDef definition

class CredentialsTypeDef(TypedDict):
    sessionToken: str,
    secretAccessKey: str,
    accessKeyId: str,
    expiration: datetime,
```

## PodIdentityAssociationTypeDef

```python
# PodIdentityAssociationTypeDef definition

class PodIdentityAssociationTypeDef(TypedDict):
    associationArn: str,
    associationId: str,
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

## SubjectTypeDef

```python
# SubjectTypeDef definition

class SubjectTypeDef(TypedDict):
    namespace: str,
    serviceAccount: str,
```

## AssumeRoleForPodIdentityResponseTypeDef

```python
# AssumeRoleForPodIdentityResponseTypeDef definition

class AssumeRoleForPodIdentityResponseTypeDef(TypedDict):
    subject: SubjectTypeDef,  # (1)
    audience: str,
    podIdentityAssociation: PodIdentityAssociationTypeDef,  # (2)
    assumedRoleUser: AssumedRoleUserTypeDef,  # (3)
    credentials: CredentialsTypeDef,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SubjectTypeDef](./type_defs.md#subjecttypedef) 
2. See [:material-code-braces: PodIdentityAssociationTypeDef](./type_defs.md#podidentityassociationtypedef) 
3. See [:material-code-braces: AssumedRoleUserTypeDef](./type_defs.md#assumedroleusertypedef) 
4. See [:material-code-braces: CredentialsTypeDef](./type_defs.md#credentialstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

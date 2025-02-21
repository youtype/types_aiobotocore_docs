# Type definitions

> [Index](../README.md) > [SecretsManager](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SecretsManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#secretsmanager)
    type annotations stubs module [types-aiobotocore-secretsmanager](https://pypi.org/project/types-aiobotocore-secretsmanager/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_secretsmanager.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## APIErrorTypeTypeDef

```python
# APIErrorTypeTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import APIErrorTypeTypeDef


def get_value() -> APIErrorTypeTypeDef:
    return {
        "SecretId": ...,
    }


# APIErrorTypeTypeDef definition

class APIErrorTypeTypeDef(TypedDict):
    SecretId: NotRequired[str],
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "Key": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Key: NotRequired[FilterNameStringTypeType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FilterNameStringTypeType](./literals.md#filternamestringtypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## SecretValueEntryTypeDef

```python
# SecretValueEntryTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import SecretValueEntryTypeDef


def get_value() -> SecretValueEntryTypeDef:
    return {
        "ARN": ...,
    }


# SecretValueEntryTypeDef definition

class SecretValueEntryTypeDef(TypedDict):
    ARN: NotRequired[str],
    Name: NotRequired[str],
    VersionId: NotRequired[str],
    SecretBinary: NotRequired[bytes],
    SecretString: NotRequired[str],
    VersionStages: NotRequired[List[str]],
    CreatedDate: NotRequired[datetime],
```

## CancelRotateSecretRequestTypeDef

```python
# CancelRotateSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import CancelRotateSecretRequestTypeDef


def get_value() -> CancelRotateSecretRequestTypeDef:
    return {
        "SecretId": ...,
    }


# CancelRotateSecretRequestTypeDef definition

class CancelRotateSecretRequestTypeDef(TypedDict):
    SecretId: str,
```

## ReplicaRegionTypeTypeDef

```python
# ReplicaRegionTypeTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ReplicaRegionTypeTypeDef


def get_value() -> ReplicaRegionTypeTypeDef:
    return {
        "Region": ...,
    }


# ReplicaRegionTypeTypeDef definition

class ReplicaRegionTypeTypeDef(TypedDict):
    Region: NotRequired[str],
    KmsKeyId: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ReplicationStatusTypeTypeDef

```python
# ReplicationStatusTypeTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ReplicationStatusTypeTypeDef


def get_value() -> ReplicationStatusTypeTypeDef:
    return {
        "Region": ...,
    }


# ReplicationStatusTypeTypeDef definition

class ReplicationStatusTypeTypeDef(TypedDict):
    Region: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Status: NotRequired[StatusTypeType],  # (1)
    StatusMessage: NotRequired[str],
    LastAccessedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## DeleteResourcePolicyRequestTypeDef

```python
# DeleteResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import DeleteResourcePolicyRequestTypeDef


def get_value() -> DeleteResourcePolicyRequestTypeDef:
    return {
        "SecretId": ...,
    }


# DeleteResourcePolicyRequestTypeDef definition

class DeleteResourcePolicyRequestTypeDef(TypedDict):
    SecretId: str,
```

## DeleteSecretRequestTypeDef

```python
# DeleteSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import DeleteSecretRequestTypeDef


def get_value() -> DeleteSecretRequestTypeDef:
    return {
        "SecretId": ...,
    }


# DeleteSecretRequestTypeDef definition

class DeleteSecretRequestTypeDef(TypedDict):
    SecretId: str,
    RecoveryWindowInDays: NotRequired[int],
    ForceDeleteWithoutRecovery: NotRequired[bool],
```

## DescribeSecretRequestTypeDef

```python
# DescribeSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import DescribeSecretRequestTypeDef


def get_value() -> DescribeSecretRequestTypeDef:
    return {
        "SecretId": ...,
    }


# DescribeSecretRequestTypeDef definition

class DescribeSecretRequestTypeDef(TypedDict):
    SecretId: str,
```

## RotationRulesTypeTypeDef

```python
# RotationRulesTypeTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import RotationRulesTypeTypeDef


def get_value() -> RotationRulesTypeTypeDef:
    return {
        "AutomaticallyAfterDays": ...,
    }


# RotationRulesTypeTypeDef definition

class RotationRulesTypeTypeDef(TypedDict):
    AutomaticallyAfterDays: NotRequired[int],
    Duration: NotRequired[str],
    ScheduleExpression: NotRequired[str],
```

## GetRandomPasswordRequestTypeDef

```python
# GetRandomPasswordRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import GetRandomPasswordRequestTypeDef


def get_value() -> GetRandomPasswordRequestTypeDef:
    return {
        "PasswordLength": ...,
    }


# GetRandomPasswordRequestTypeDef definition

class GetRandomPasswordRequestTypeDef(TypedDict):
    PasswordLength: NotRequired[int],
    ExcludeCharacters: NotRequired[str],
    ExcludeNumbers: NotRequired[bool],
    ExcludePunctuation: NotRequired[bool],
    ExcludeUppercase: NotRequired[bool],
    ExcludeLowercase: NotRequired[bool],
    IncludeSpace: NotRequired[bool],
    RequireEachIncludedType: NotRequired[bool],
```

## GetResourcePolicyRequestTypeDef

```python
# GetResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import GetResourcePolicyRequestTypeDef


def get_value() -> GetResourcePolicyRequestTypeDef:
    return {
        "SecretId": ...,
    }


# GetResourcePolicyRequestTypeDef definition

class GetResourcePolicyRequestTypeDef(TypedDict):
    SecretId: str,
```

## GetSecretValueRequestTypeDef

```python
# GetSecretValueRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import GetSecretValueRequestTypeDef


def get_value() -> GetSecretValueRequestTypeDef:
    return {
        "SecretId": ...,
    }


# GetSecretValueRequestTypeDef definition

class GetSecretValueRequestTypeDef(TypedDict):
    SecretId: str,
    VersionId: NotRequired[str],
    VersionStage: NotRequired[str],
```

## ListSecretVersionIdsRequestTypeDef

```python
# ListSecretVersionIdsRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ListSecretVersionIdsRequestTypeDef


def get_value() -> ListSecretVersionIdsRequestTypeDef:
    return {
        "SecretId": ...,
    }


# ListSecretVersionIdsRequestTypeDef definition

class ListSecretVersionIdsRequestTypeDef(TypedDict):
    SecretId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    IncludeDeprecated: NotRequired[bool],
```

## SecretVersionsListEntryTypeDef

```python
# SecretVersionsListEntryTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import SecretVersionsListEntryTypeDef


def get_value() -> SecretVersionsListEntryTypeDef:
    return {
        "VersionId": ...,
    }


# SecretVersionsListEntryTypeDef definition

class SecretVersionsListEntryTypeDef(TypedDict):
    VersionId: NotRequired[str],
    VersionStages: NotRequired[List[str]],
    LastAccessedDate: NotRequired[datetime],
    CreatedDate: NotRequired[datetime],
    KmsKeyIds: NotRequired[List[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## PutResourcePolicyRequestTypeDef

```python
# PutResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import PutResourcePolicyRequestTypeDef


def get_value() -> PutResourcePolicyRequestTypeDef:
    return {
        "SecretId": ...,
    }


# PutResourcePolicyRequestTypeDef definition

class PutResourcePolicyRequestTypeDef(TypedDict):
    SecretId: str,
    ResourcePolicy: str,
    BlockPublicPolicy: NotRequired[bool],
```

## RemoveRegionsFromReplicationRequestTypeDef

```python
# RemoveRegionsFromReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import RemoveRegionsFromReplicationRequestTypeDef


def get_value() -> RemoveRegionsFromReplicationRequestTypeDef:
    return {
        "SecretId": ...,
    }


# RemoveRegionsFromReplicationRequestTypeDef definition

class RemoveRegionsFromReplicationRequestTypeDef(TypedDict):
    SecretId: str,
    RemoveReplicaRegions: Sequence[str],
```

## RestoreSecretRequestTypeDef

```python
# RestoreSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import RestoreSecretRequestTypeDef


def get_value() -> RestoreSecretRequestTypeDef:
    return {
        "SecretId": ...,
    }


# RestoreSecretRequestTypeDef definition

class RestoreSecretRequestTypeDef(TypedDict):
    SecretId: str,
```

## StopReplicationToReplicaRequestTypeDef

```python
# StopReplicationToReplicaRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import StopReplicationToReplicaRequestTypeDef


def get_value() -> StopReplicationToReplicaRequestTypeDef:
    return {
        "SecretId": ...,
    }


# StopReplicationToReplicaRequestTypeDef definition

class StopReplicationToReplicaRequestTypeDef(TypedDict):
    SecretId: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "SecretId": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    SecretId: str,
    TagKeys: Sequence[str],
```

## UpdateSecretVersionStageRequestTypeDef

```python
# UpdateSecretVersionStageRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import UpdateSecretVersionStageRequestTypeDef


def get_value() -> UpdateSecretVersionStageRequestTypeDef:
    return {
        "SecretId": ...,
    }


# UpdateSecretVersionStageRequestTypeDef definition

class UpdateSecretVersionStageRequestTypeDef(TypedDict):
    SecretId: str,
    VersionStage: str,
    RemoveFromVersionId: NotRequired[str],
    MoveToVersionId: NotRequired[str],
```

## ValidateResourcePolicyRequestTypeDef

```python
# ValidateResourcePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ValidateResourcePolicyRequestTypeDef


def get_value() -> ValidateResourcePolicyRequestTypeDef:
    return {
        "ResourcePolicy": ...,
    }


# ValidateResourcePolicyRequestTypeDef definition

class ValidateResourcePolicyRequestTypeDef(TypedDict):
    ResourcePolicy: str,
    SecretId: NotRequired[str],
```

## ValidationErrorsEntryTypeDef

```python
# ValidationErrorsEntryTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ValidationErrorsEntryTypeDef


def get_value() -> ValidationErrorsEntryTypeDef:
    return {
        "CheckName": ...,
    }


# ValidationErrorsEntryTypeDef definition

class ValidationErrorsEntryTypeDef(TypedDict):
    CheckName: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchGetSecretValueRequestTypeDef

```python
# BatchGetSecretValueRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import BatchGetSecretValueRequestTypeDef


def get_value() -> BatchGetSecretValueRequestTypeDef:
    return {
        "SecretIdList": ...,
    }


# BatchGetSecretValueRequestTypeDef definition

class BatchGetSecretValueRequestTypeDef(TypedDict):
    SecretIdList: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListSecretsRequestTypeDef

```python
# ListSecretsRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ListSecretsRequestTypeDef


def get_value() -> ListSecretsRequestTypeDef:
    return {
        "IncludePlannedDeletion": ...,
    }


# ListSecretsRequestTypeDef definition

class ListSecretsRequestTypeDef(TypedDict):
    IncludePlannedDeletion: NotRequired[bool],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortOrder: NotRequired[SortOrderTypeType],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
## CancelRotateSecretResponseTypeDef

```python
# CancelRotateSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import CancelRotateSecretResponseTypeDef


def get_value() -> CancelRotateSecretResponseTypeDef:
    return {
        "ARN": ...,
    }


# CancelRotateSecretResponseTypeDef definition

class CancelRotateSecretResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    VersionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourcePolicyResponseTypeDef

```python
# DeleteResourcePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import DeleteResourcePolicyResponseTypeDef


def get_value() -> DeleteResourcePolicyResponseTypeDef:
    return {
        "ARN": ...,
    }


# DeleteResourcePolicyResponseTypeDef definition

class DeleteResourcePolicyResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSecretResponseTypeDef

```python
# DeleteSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import DeleteSecretResponseTypeDef


def get_value() -> DeleteSecretResponseTypeDef:
    return {
        "ARN": ...,
    }


# DeleteSecretResponseTypeDef definition

class DeleteSecretResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    DeletionDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRandomPasswordResponseTypeDef

```python
# GetRandomPasswordResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import GetRandomPasswordResponseTypeDef


def get_value() -> GetRandomPasswordResponseTypeDef:
    return {
        "RandomPassword": ...,
    }


# GetRandomPasswordResponseTypeDef definition

class GetRandomPasswordResponseTypeDef(TypedDict):
    RandomPassword: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import GetResourcePolicyResponseTypeDef


def get_value() -> GetResourcePolicyResponseTypeDef:
    return {
        "ARN": ...,
    }


# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResourcePolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSecretValueResponseTypeDef

```python
# GetSecretValueResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import GetSecretValueResponseTypeDef


def get_value() -> GetSecretValueResponseTypeDef:
    return {
        "ARN": ...,
    }


# GetSecretValueResponseTypeDef definition

class GetSecretValueResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    VersionId: str,
    SecretBinary: bytes,
    SecretString: str,
    VersionStages: List[str],
    CreatedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourcePolicyResponseTypeDef

```python
# PutResourcePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import PutResourcePolicyResponseTypeDef


def get_value() -> PutResourcePolicyResponseTypeDef:
    return {
        "ARN": ...,
    }


# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSecretValueResponseTypeDef

```python
# PutSecretValueResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import PutSecretValueResponseTypeDef


def get_value() -> PutSecretValueResponseTypeDef:
    return {
        "ARN": ...,
    }


# PutSecretValueResponseTypeDef definition

class PutSecretValueResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    VersionId: str,
    VersionStages: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreSecretResponseTypeDef

```python
# RestoreSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import RestoreSecretResponseTypeDef


def get_value() -> RestoreSecretResponseTypeDef:
    return {
        "ARN": ...,
    }


# RestoreSecretResponseTypeDef definition

class RestoreSecretResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateSecretResponseTypeDef

```python
# RotateSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import RotateSecretResponseTypeDef


def get_value() -> RotateSecretResponseTypeDef:
    return {
        "ARN": ...,
    }


# RotateSecretResponseTypeDef definition

class RotateSecretResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    VersionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopReplicationToReplicaResponseTypeDef

```python
# StopReplicationToReplicaResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import StopReplicationToReplicaResponseTypeDef


def get_value() -> StopReplicationToReplicaResponseTypeDef:
    return {
        "ARN": ...,
    }


# StopReplicationToReplicaResponseTypeDef definition

class StopReplicationToReplicaResponseTypeDef(TypedDict):
    ARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecretResponseTypeDef

```python
# UpdateSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import UpdateSecretResponseTypeDef


def get_value() -> UpdateSecretResponseTypeDef:
    return {
        "ARN": ...,
    }


# UpdateSecretResponseTypeDef definition

class UpdateSecretResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    VersionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecretVersionStageResponseTypeDef

```python
# UpdateSecretVersionStageResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import UpdateSecretVersionStageResponseTypeDef


def get_value() -> UpdateSecretVersionStageResponseTypeDef:
    return {
        "ARN": ...,
    }


# UpdateSecretVersionStageResponseTypeDef definition

class UpdateSecretVersionStageResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetSecretValueResponseTypeDef

```python
# BatchGetSecretValueResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import BatchGetSecretValueResponseTypeDef


def get_value() -> BatchGetSecretValueResponseTypeDef:
    return {
        "SecretValues": ...,
    }


# BatchGetSecretValueResponseTypeDef definition

class BatchGetSecretValueResponseTypeDef(TypedDict):
    SecretValues: List[SecretValueEntryTypeDef],  # (1)
    Errors: List[APIErrorTypeTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SecretValueEntryTypeDef](./type_defs.md#secretvalueentrytypedef) 
2. See [:material-code-braces: APIErrorTypeTypeDef](./type_defs.md#apierrortypetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSecretValueRequestTypeDef

```python
# PutSecretValueRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import PutSecretValueRequestTypeDef


def get_value() -> PutSecretValueRequestTypeDef:
    return {
        "SecretId": ...,
    }


# PutSecretValueRequestTypeDef definition

class PutSecretValueRequestTypeDef(TypedDict):
    SecretId: str,
    ClientRequestToken: NotRequired[str],
    SecretBinary: NotRequired[BlobTypeDef],
    SecretString: NotRequired[str],
    VersionStages: NotRequired[Sequence[str]],
    RotationToken: NotRequired[str],
```

## UpdateSecretRequestTypeDef

```python
# UpdateSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import UpdateSecretRequestTypeDef


def get_value() -> UpdateSecretRequestTypeDef:
    return {
        "SecretId": ...,
    }


# UpdateSecretRequestTypeDef definition

class UpdateSecretRequestTypeDef(TypedDict):
    SecretId: str,
    ClientRequestToken: NotRequired[str],
    Description: NotRequired[str],
    KmsKeyId: NotRequired[str],
    SecretBinary: NotRequired[BlobTypeDef],
    SecretString: NotRequired[str],
```

## ReplicateSecretToRegionsRequestTypeDef

```python
# ReplicateSecretToRegionsRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ReplicateSecretToRegionsRequestTypeDef


def get_value() -> ReplicateSecretToRegionsRequestTypeDef:
    return {
        "SecretId": ...,
    }


# ReplicateSecretToRegionsRequestTypeDef definition

class ReplicateSecretToRegionsRequestTypeDef(TypedDict):
    SecretId: str,
    AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef],  # (1)
    ForceOverwriteReplicaSecret: NotRequired[bool],
```

1. See [:material-code-braces: ReplicaRegionTypeTypeDef](./type_defs.md#replicaregiontypetypedef) 
## CreateSecretRequestTypeDef

```python
# CreateSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import CreateSecretRequestTypeDef


def get_value() -> CreateSecretRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateSecretRequestTypeDef definition

class CreateSecretRequestTypeDef(TypedDict):
    Name: str,
    ClientRequestToken: NotRequired[str],
    Description: NotRequired[str],
    KmsKeyId: NotRequired[str],
    SecretBinary: NotRequired[BlobTypeDef],
    SecretString: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    AddReplicaRegions: NotRequired[Sequence[ReplicaRegionTypeTypeDef]],  # (2)
    ForceOverwriteReplicaSecret: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ReplicaRegionTypeTypeDef](./type_defs.md#replicaregiontypetypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "SecretId": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    SecretId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSecretResponseTypeDef

```python
# CreateSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import CreateSecretResponseTypeDef


def get_value() -> CreateSecretResponseTypeDef:
    return {
        "ARN": ...,
    }


# CreateSecretResponseTypeDef definition

class CreateSecretResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    VersionId: str,
    ReplicationStatus: List[ReplicationStatusTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationStatusTypeTypeDef](./type_defs.md#replicationstatustypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveRegionsFromReplicationResponseTypeDef

```python
# RemoveRegionsFromReplicationResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import RemoveRegionsFromReplicationResponseTypeDef


def get_value() -> RemoveRegionsFromReplicationResponseTypeDef:
    return {
        "ARN": ...,
    }


# RemoveRegionsFromReplicationResponseTypeDef definition

class RemoveRegionsFromReplicationResponseTypeDef(TypedDict):
    ARN: str,
    ReplicationStatus: List[ReplicationStatusTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationStatusTypeTypeDef](./type_defs.md#replicationstatustypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicateSecretToRegionsResponseTypeDef

```python
# ReplicateSecretToRegionsResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ReplicateSecretToRegionsResponseTypeDef


def get_value() -> ReplicateSecretToRegionsResponseTypeDef:
    return {
        "ARN": ...,
    }


# ReplicateSecretToRegionsResponseTypeDef definition

class ReplicateSecretToRegionsResponseTypeDef(TypedDict):
    ARN: str,
    ReplicationStatus: List[ReplicationStatusTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicationStatusTypeTypeDef](./type_defs.md#replicationstatustypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSecretResponseTypeDef

```python
# DescribeSecretResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import DescribeSecretResponseTypeDef


def get_value() -> DescribeSecretResponseTypeDef:
    return {
        "ARN": ...,
    }


# DescribeSecretResponseTypeDef definition

class DescribeSecretResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    Description: str,
    KmsKeyId: str,
    RotationEnabled: bool,
    RotationLambdaARN: str,
    RotationRules: RotationRulesTypeTypeDef,  # (1)
    LastRotatedDate: datetime,
    LastChangedDate: datetime,
    LastAccessedDate: datetime,
    DeletedDate: datetime,
    NextRotationDate: datetime,
    Tags: List[TagTypeDef],  # (2)
    VersionIdsToStages: Dict[str, List[str]],
    OwningService: str,
    CreatedDate: datetime,
    PrimaryRegion: str,
    ReplicationStatus: List[ReplicationStatusTypeTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: RotationRulesTypeTypeDef](./type_defs.md#rotationrulestypetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ReplicationStatusTypeTypeDef](./type_defs.md#replicationstatustypetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateSecretRequestTypeDef

```python
# RotateSecretRequestTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import RotateSecretRequestTypeDef


def get_value() -> RotateSecretRequestTypeDef:
    return {
        "SecretId": ...,
    }


# RotateSecretRequestTypeDef definition

class RotateSecretRequestTypeDef(TypedDict):
    SecretId: str,
    ClientRequestToken: NotRequired[str],
    RotationLambdaARN: NotRequired[str],
    RotationRules: NotRequired[RotationRulesTypeTypeDef],  # (1)
    RotateImmediately: NotRequired[bool],
```

1. See [:material-code-braces: RotationRulesTypeTypeDef](./type_defs.md#rotationrulestypetypedef) 
## SecretListEntryTypeDef

```python
# SecretListEntryTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import SecretListEntryTypeDef


def get_value() -> SecretListEntryTypeDef:
    return {
        "ARN": ...,
    }


# SecretListEntryTypeDef definition

class SecretListEntryTypeDef(TypedDict):
    ARN: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    KmsKeyId: NotRequired[str],
    RotationEnabled: NotRequired[bool],
    RotationLambdaARN: NotRequired[str],
    RotationRules: NotRequired[RotationRulesTypeTypeDef],  # (1)
    LastRotatedDate: NotRequired[datetime],
    LastChangedDate: NotRequired[datetime],
    LastAccessedDate: NotRequired[datetime],
    DeletedDate: NotRequired[datetime],
    NextRotationDate: NotRequired[datetime],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    SecretVersionsToStages: NotRequired[Dict[str, List[str]]],
    OwningService: NotRequired[str],
    CreatedDate: NotRequired[datetime],
    PrimaryRegion: NotRequired[str],
```

1. See [:material-code-braces: RotationRulesTypeTypeDef](./type_defs.md#rotationrulestypetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListSecretVersionIdsResponseTypeDef

```python
# ListSecretVersionIdsResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ListSecretVersionIdsResponseTypeDef


def get_value() -> ListSecretVersionIdsResponseTypeDef:
    return {
        "Versions": ...,
    }


# ListSecretVersionIdsResponseTypeDef definition

class ListSecretVersionIdsResponseTypeDef(TypedDict):
    Versions: List[SecretVersionsListEntryTypeDef],  # (1)
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SecretVersionsListEntryTypeDef](./type_defs.md#secretversionslistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecretsRequestPaginateTypeDef

```python
# ListSecretsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ListSecretsRequestPaginateTypeDef


def get_value() -> ListSecretsRequestPaginateTypeDef:
    return {
        "IncludePlannedDeletion": ...,
    }


# ListSecretsRequestPaginateTypeDef definition

class ListSecretsRequestPaginateTypeDef(TypedDict):
    IncludePlannedDeletion: NotRequired[bool],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    SortOrder: NotRequired[SortOrderTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-brackets: SortOrderTypeType](./literals.md#sortordertypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ValidateResourcePolicyResponseTypeDef

```python
# ValidateResourcePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ValidateResourcePolicyResponseTypeDef


def get_value() -> ValidateResourcePolicyResponseTypeDef:
    return {
        "PolicyValidationPassed": ...,
    }


# ValidateResourcePolicyResponseTypeDef definition

class ValidateResourcePolicyResponseTypeDef(TypedDict):
    PolicyValidationPassed: bool,
    ValidationErrors: List[ValidationErrorsEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidationErrorsEntryTypeDef](./type_defs.md#validationerrorsentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSecretsResponseTypeDef

```python
# ListSecretsResponseTypeDef TypedDict usage example

from types_aiobotocore_secretsmanager.type_defs import ListSecretsResponseTypeDef


def get_value() -> ListSecretsResponseTypeDef:
    return {
        "SecretList": ...,
    }


# ListSecretsResponseTypeDef definition

class ListSecretsResponseTypeDef(TypedDict):
    SecretList: List[SecretListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SecretListEntryTypeDef](./type_defs.md#secretlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

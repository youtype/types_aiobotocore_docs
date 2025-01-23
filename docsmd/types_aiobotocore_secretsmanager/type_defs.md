# Type definitions

> [Index](../README.md) > [SecretsManager](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SecretsManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#secretsmanager)
    type annotations stubs module [types-aiobotocore-secretsmanager](https://pypi.org/project/types-aiobotocore-secretsmanager/).

## BlobTypeDef

```python
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
# APIErrorTypeTypeDef definition

class APIErrorTypeTypeDef(TypedDict):
    SecretId: NotRequired[str],
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Key: NotRequired[FilterNameStringTypeType],  # (1)
    Values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FilterNameStringTypeType](./literals.md#filternamestringtypetype) 
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

## SecretValueEntryTypeDef

```python
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

## CancelRotateSecretRequestRequestTypeDef

```python
# CancelRotateSecretRequestRequestTypeDef definition

class CancelRotateSecretRequestRequestTypeDef(TypedDict):
    SecretId: str,
```

## ReplicaRegionTypeTypeDef

```python
# ReplicaRegionTypeTypeDef definition

class ReplicaRegionTypeTypeDef(TypedDict):
    Region: NotRequired[str],
    KmsKeyId: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ReplicationStatusTypeTypeDef

```python
# ReplicationStatusTypeTypeDef definition

class ReplicationStatusTypeTypeDef(TypedDict):
    Region: NotRequired[str],
    KmsKeyId: NotRequired[str],
    Status: NotRequired[StatusTypeType],  # (1)
    StatusMessage: NotRequired[str],
    LastAccessedDate: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    SecretId: str,
```

## DeleteSecretRequestRequestTypeDef

```python
# DeleteSecretRequestRequestTypeDef definition

class DeleteSecretRequestRequestTypeDef(TypedDict):
    SecretId: str,
    RecoveryWindowInDays: NotRequired[int],
    ForceDeleteWithoutRecovery: NotRequired[bool],
```

## DescribeSecretRequestRequestTypeDef

```python
# DescribeSecretRequestRequestTypeDef definition

class DescribeSecretRequestRequestTypeDef(TypedDict):
    SecretId: str,
```

## RotationRulesTypeTypeDef

```python
# RotationRulesTypeTypeDef definition

class RotationRulesTypeTypeDef(TypedDict):
    AutomaticallyAfterDays: NotRequired[int],
    Duration: NotRequired[str],
    ScheduleExpression: NotRequired[str],
```

## GetRandomPasswordRequestRequestTypeDef

```python
# GetRandomPasswordRequestRequestTypeDef definition

class GetRandomPasswordRequestRequestTypeDef(TypedDict):
    PasswordLength: NotRequired[int],
    ExcludeCharacters: NotRequired[str],
    ExcludeNumbers: NotRequired[bool],
    ExcludePunctuation: NotRequired[bool],
    ExcludeUppercase: NotRequired[bool],
    ExcludeLowercase: NotRequired[bool],
    IncludeSpace: NotRequired[bool],
    RequireEachIncludedType: NotRequired[bool],
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    SecretId: str,
```

## GetSecretValueRequestRequestTypeDef

```python
# GetSecretValueRequestRequestTypeDef definition

class GetSecretValueRequestRequestTypeDef(TypedDict):
    SecretId: str,
    VersionId: NotRequired[str],
    VersionStage: NotRequired[str],
```

## ListSecretVersionIdsRequestRequestTypeDef

```python
# ListSecretVersionIdsRequestRequestTypeDef definition

class ListSecretVersionIdsRequestRequestTypeDef(TypedDict):
    SecretId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    IncludeDeprecated: NotRequired[bool],
```

## SecretVersionsListEntryTypeDef

```python
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
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    SecretId: str,
    ResourcePolicy: str,
    BlockPublicPolicy: NotRequired[bool],
```

## RemoveRegionsFromReplicationRequestRequestTypeDef

```python
# RemoveRegionsFromReplicationRequestRequestTypeDef definition

class RemoveRegionsFromReplicationRequestRequestTypeDef(TypedDict):
    SecretId: str,
    RemoveReplicaRegions: Sequence[str],
```

## RestoreSecretRequestRequestTypeDef

```python
# RestoreSecretRequestRequestTypeDef definition

class RestoreSecretRequestRequestTypeDef(TypedDict):
    SecretId: str,
```

## StopReplicationToReplicaRequestRequestTypeDef

```python
# StopReplicationToReplicaRequestRequestTypeDef definition

class StopReplicationToReplicaRequestRequestTypeDef(TypedDict):
    SecretId: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    SecretId: str,
    TagKeys: Sequence[str],
```

## UpdateSecretVersionStageRequestRequestTypeDef

```python
# UpdateSecretVersionStageRequestRequestTypeDef definition

class UpdateSecretVersionStageRequestRequestTypeDef(TypedDict):
    SecretId: str,
    VersionStage: str,
    RemoveFromVersionId: NotRequired[str],
    MoveToVersionId: NotRequired[str],
```

## ValidateResourcePolicyRequestRequestTypeDef

```python
# ValidateResourcePolicyRequestRequestTypeDef definition

class ValidateResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourcePolicy: str,
    SecretId: NotRequired[str],
```

## ValidationErrorsEntryTypeDef

```python
# ValidationErrorsEntryTypeDef definition

class ValidationErrorsEntryTypeDef(TypedDict):
    CheckName: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## BatchGetSecretValueRequestRequestTypeDef

```python
# BatchGetSecretValueRequestRequestTypeDef definition

class BatchGetSecretValueRequestRequestTypeDef(TypedDict):
    SecretIdList: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListSecretsRequestRequestTypeDef

```python
# ListSecretsRequestRequestTypeDef definition

class ListSecretsRequestRequestTypeDef(TypedDict):
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
# DeleteResourcePolicyResponseTypeDef definition

class DeleteResourcePolicyResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSecretResponseTypeDef

```python
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
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRandomPasswordResponseTypeDef

```python
# GetRandomPasswordResponseTypeDef definition

class GetRandomPasswordResponseTypeDef(TypedDict):
    RandomPassword: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
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
# PutResourcePolicyResponseTypeDef definition

class PutResourcePolicyResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSecretValueResponseTypeDef

```python
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
# RestoreSecretResponseTypeDef definition

class RestoreSecretResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotateSecretResponseTypeDef

```python
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
# StopReplicationToReplicaResponseTypeDef definition

class StopReplicationToReplicaResponseTypeDef(TypedDict):
    ARN: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSecretResponseTypeDef

```python
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
# UpdateSecretVersionStageResponseTypeDef definition

class UpdateSecretVersionStageResponseTypeDef(TypedDict):
    ARN: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetSecretValueResponseTypeDef

```python
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
## PutSecretValueRequestRequestTypeDef

```python
# PutSecretValueRequestRequestTypeDef definition

class PutSecretValueRequestRequestTypeDef(TypedDict):
    SecretId: str,
    ClientRequestToken: NotRequired[str],
    SecretBinary: NotRequired[BlobTypeDef],
    SecretString: NotRequired[str],
    VersionStages: NotRequired[Sequence[str]],
    RotationToken: NotRequired[str],
```

## UpdateSecretRequestRequestTypeDef

```python
# UpdateSecretRequestRequestTypeDef definition

class UpdateSecretRequestRequestTypeDef(TypedDict):
    SecretId: str,
    ClientRequestToken: NotRequired[str],
    Description: NotRequired[str],
    KmsKeyId: NotRequired[str],
    SecretBinary: NotRequired[BlobTypeDef],
    SecretString: NotRequired[str],
```

## ReplicateSecretToRegionsRequestRequestTypeDef

```python
# ReplicateSecretToRegionsRequestRequestTypeDef definition

class ReplicateSecretToRegionsRequestRequestTypeDef(TypedDict):
    SecretId: str,
    AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef],  # (1)
    ForceOverwriteReplicaSecret: NotRequired[bool],
```

1. See [:material-code-braces: ReplicaRegionTypeTypeDef](./type_defs.md#replicaregiontypetypedef) 
## CreateSecretRequestRequestTypeDef

```python
# CreateSecretRequestRequestTypeDef definition

class CreateSecretRequestRequestTypeDef(TypedDict):
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
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    SecretId: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateSecretResponseTypeDef

```python
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
## RotateSecretRequestRequestTypeDef

```python
# RotateSecretRequestRequestTypeDef definition

class RotateSecretRequestRequestTypeDef(TypedDict):
    SecretId: str,
    ClientRequestToken: NotRequired[str],
    RotationLambdaARN: NotRequired[str],
    RotationRules: NotRequired[RotationRulesTypeTypeDef],  # (1)
    RotateImmediately: NotRequired[bool],
```

1. See [:material-code-braces: RotationRulesTypeTypeDef](./type_defs.md#rotationrulestypetypedef) 
## SecretListEntryTypeDef

```python
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
# ListSecretsResponseTypeDef definition

class ListSecretsResponseTypeDef(TypedDict):
    SecretList: List[SecretListEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SecretListEntryTypeDef](./type_defs.md#secretlistentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

# Type definitions

> [Index](../README.md) > [GameSparks](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [GameSparks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
    type annotations stubs module [types-aiobotocore-gamesparks](https://pypi.org/project/types-aiobotocore-gamesparks/).

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




## ConnectionTypeDef

```python
# ConnectionTypeDef definition

class ConnectionTypeDef(TypedDict):
    Created: NotRequired[datetime],
    Id: NotRequired[str],
```

## CreateGameRequestRequestTypeDef

```python
# CreateGameRequestRequestTypeDef definition

class CreateGameRequestRequestTypeDef(TypedDict):
    GameName: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## GameDetailsTypeDef

```python
# GameDetailsTypeDef definition

class GameDetailsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Created: NotRequired[datetime],
    Description: NotRequired[str],
    EnableTerminationProtection: NotRequired[bool],
    LastUpdated: NotRequired[datetime],
    Name: NotRequired[str],
    State: NotRequired[GameStateType],  # (1)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: GameStateType](./literals.md#gamestatetype) 
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

## CreateSnapshotRequestRequestTypeDef

```python
# CreateSnapshotRequestRequestTypeDef definition

class CreateSnapshotRequestRequestTypeDef(TypedDict):
    GameName: str,
    Description: NotRequired[str],
```

## CreateStageRequestRequestTypeDef

```python
# CreateStageRequestRequestTypeDef definition

class CreateStageRequestRequestTypeDef(TypedDict):
    GameName: str,
    Role: str,
    StageName: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## StageDetailsTypeDef

```python
# StageDetailsTypeDef definition

class StageDetailsTypeDef(TypedDict):
    Arn: NotRequired[str],
    Created: NotRequired[datetime],
    Description: NotRequired[str],
    GameKey: NotRequired[str],
    LastUpdated: NotRequired[datetime],
    LogGroup: NotRequired[str],
    Name: NotRequired[str],
    Role: NotRequired[str],
    State: NotRequired[StageStateType],  # (1)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: StageStateType](./literals.md#stagestatetype) 
## DeleteGameRequestRequestTypeDef

```python
# DeleteGameRequestRequestTypeDef definition

class DeleteGameRequestRequestTypeDef(TypedDict):
    GameName: str,
```

## DeleteStageRequestRequestTypeDef

```python
# DeleteStageRequestRequestTypeDef definition

class DeleteStageRequestRequestTypeDef(TypedDict):
    GameName: str,
    StageName: str,
```

## DeploymentResultTypeDef

```python
# DeploymentResultTypeDef definition

class DeploymentResultTypeDef(TypedDict):
    Message: NotRequired[str],
    ResultCode: NotRequired[ResultCodeType],  # (1)
```

1. See [:material-code-brackets: ResultCodeType](./literals.md#resultcodetype) 
## DisconnectPlayerRequestRequestTypeDef

```python
# DisconnectPlayerRequestRequestTypeDef definition

class DisconnectPlayerRequestRequestTypeDef(TypedDict):
    GameName: str,
    PlayerId: str,
    StageName: str,
```

## ExportSnapshotRequestRequestTypeDef

```python
# ExportSnapshotRequestRequestTypeDef definition

class ExportSnapshotRequestRequestTypeDef(TypedDict):
    GameName: str,
    SnapshotId: str,
```

## ExtensionDetailsTypeDef

```python
# ExtensionDetailsTypeDef definition

class ExtensionDetailsTypeDef(TypedDict):
    Description: NotRequired[str],
    Name: NotRequired[str],
    Namespace: NotRequired[str],
```

## ExtensionVersionDetailsTypeDef

```python
# ExtensionVersionDetailsTypeDef definition

class ExtensionVersionDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    Namespace: NotRequired[str],
    Schema: NotRequired[str],
    Version: NotRequired[str],
```

## SectionTypeDef

```python
# SectionTypeDef definition

class SectionTypeDef(TypedDict):
    Attributes: NotRequired[Dict[str, Any]],
    Name: NotRequired[str],
    Size: NotRequired[int],
```

## GameSummaryTypeDef

```python
# GameSummaryTypeDef definition

class GameSummaryTypeDef(TypedDict):
    Description: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[GameStateType],  # (1)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: GameStateType](./literals.md#gamestatetype) 
## GeneratedCodeJobDetailsTypeDef

```python
# GeneratedCodeJobDetailsTypeDef definition

class GeneratedCodeJobDetailsTypeDef(TypedDict):
    Description: NotRequired[str],
    ExpirationTime: NotRequired[datetime],
    GeneratedCodeJobId: NotRequired[str],
    S3Url: NotRequired[str],
    Status: NotRequired[GeneratedCodeJobStateType],  # (1)
```

1. See [:material-code-brackets: GeneratedCodeJobStateType](./literals.md#generatedcodejobstatetype) 
## GeneratorTypeDef

```python
# GeneratorTypeDef definition

class GeneratorTypeDef(TypedDict):
    GameSdkVersion: NotRequired[str],
    Language: NotRequired[str],
    TargetPlatform: NotRequired[str],
```

## GetExtensionRequestRequestTypeDef

```python
# GetExtensionRequestRequestTypeDef definition

class GetExtensionRequestRequestTypeDef(TypedDict):
    Name: str,
    Namespace: str,
```

## GetExtensionVersionRequestRequestTypeDef

```python
# GetExtensionVersionRequestRequestTypeDef definition

class GetExtensionVersionRequestRequestTypeDef(TypedDict):
    ExtensionVersion: str,
    Name: str,
    Namespace: str,
```

## GetGameConfigurationRequestRequestTypeDef

```python
# GetGameConfigurationRequestRequestTypeDef definition

class GetGameConfigurationRequestRequestTypeDef(TypedDict):
    GameName: str,
    Sections: NotRequired[Sequence[str]],
```

## GetGameRequestRequestTypeDef

```python
# GetGameRequestRequestTypeDef definition

class GetGameRequestRequestTypeDef(TypedDict):
    GameName: str,
```

## GetGeneratedCodeJobRequestRequestTypeDef

```python
# GetGeneratedCodeJobRequestRequestTypeDef definition

class GetGeneratedCodeJobRequestRequestTypeDef(TypedDict):
    GameName: str,
    JobId: str,
    SnapshotId: str,
```

## GetPlayerConnectionStatusRequestRequestTypeDef

```python
# GetPlayerConnectionStatusRequestRequestTypeDef definition

class GetPlayerConnectionStatusRequestRequestTypeDef(TypedDict):
    GameName: str,
    PlayerId: str,
    StageName: str,
```

## GetSnapshotRequestRequestTypeDef

```python
# GetSnapshotRequestRequestTypeDef definition

class GetSnapshotRequestRequestTypeDef(TypedDict):
    GameName: str,
    SnapshotId: str,
    Sections: NotRequired[Sequence[str]],
```

## GetStageDeploymentRequestRequestTypeDef

```python
# GetStageDeploymentRequestRequestTypeDef definition

class GetStageDeploymentRequestRequestTypeDef(TypedDict):
    GameName: str,
    StageName: str,
    DeploymentId: NotRequired[str],
```

## GetStageRequestRequestTypeDef

```python
# GetStageRequestRequestTypeDef definition

class GetStageRequestRequestTypeDef(TypedDict):
    GameName: str,
    StageName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListExtensionVersionsRequestRequestTypeDef

```python
# ListExtensionVersionsRequestRequestTypeDef definition

class ListExtensionVersionsRequestRequestTypeDef(TypedDict):
    Name: str,
    Namespace: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListExtensionsRequestRequestTypeDef

```python
# ListExtensionsRequestRequestTypeDef definition

class ListExtensionsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGamesRequestRequestTypeDef

```python
# ListGamesRequestRequestTypeDef definition

class ListGamesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListGeneratedCodeJobsRequestRequestTypeDef

```python
# ListGeneratedCodeJobsRequestRequestTypeDef definition

class ListGeneratedCodeJobsRequestRequestTypeDef(TypedDict):
    GameName: str,
    SnapshotId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSnapshotsRequestRequestTypeDef

```python
# ListSnapshotsRequestRequestTypeDef definition

class ListSnapshotsRequestRequestTypeDef(TypedDict):
    GameName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SnapshotSummaryTypeDef

```python
# SnapshotSummaryTypeDef definition

class SnapshotSummaryTypeDef(TypedDict):
    Created: NotRequired[datetime],
    Description: NotRequired[str],
    Id: NotRequired[str],
    LastUpdated: NotRequired[datetime],
```

## ListStageDeploymentsRequestRequestTypeDef

```python
# ListStageDeploymentsRequestRequestTypeDef definition

class ListStageDeploymentsRequestRequestTypeDef(TypedDict):
    GameName: str,
    StageName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListStagesRequestRequestTypeDef

```python
# ListStagesRequestRequestTypeDef definition

class ListStagesRequestRequestTypeDef(TypedDict):
    GameName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## StageSummaryTypeDef

```python
# StageSummaryTypeDef definition

class StageSummaryTypeDef(TypedDict):
    Description: NotRequired[str],
    GameKey: NotRequired[str],
    Name: NotRequired[str],
    State: NotRequired[StageStateType],  # (1)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: StageStateType](./literals.md#stagestatetype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## SectionModificationTypeDef

```python
# SectionModificationTypeDef definition

class SectionModificationTypeDef(TypedDict):
    Operation: OperationType,  # (1)
    Path: str,
    Section: str,
    Value: NotRequired[Mapping[str, Any]],
```

1. See [:material-code-brackets: OperationType](./literals.md#operationtype) 
## StartStageDeploymentRequestRequestTypeDef

```python
# StartStageDeploymentRequestRequestTypeDef definition

class StartStageDeploymentRequestRequestTypeDef(TypedDict):
    GameName: str,
    SnapshotId: str,
    StageName: str,
    ClientToken: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateGameRequestRequestTypeDef

```python
# UpdateGameRequestRequestTypeDef definition

class UpdateGameRequestRequestTypeDef(TypedDict):
    GameName: str,
    Description: NotRequired[str],
```

## UpdateSnapshotRequestRequestTypeDef

```python
# UpdateSnapshotRequestRequestTypeDef definition

class UpdateSnapshotRequestRequestTypeDef(TypedDict):
    GameName: str,
    SnapshotId: str,
    Description: NotRequired[str],
```

## UpdateStageRequestRequestTypeDef

```python
# UpdateStageRequestRequestTypeDef definition

class UpdateStageRequestRequestTypeDef(TypedDict):
    GameName: str,
    StageName: str,
    Description: NotRequired[str],
    Role: NotRequired[str],
```

## ImportGameConfigurationSourceTypeDef

```python
# ImportGameConfigurationSourceTypeDef definition

class ImportGameConfigurationSourceTypeDef(TypedDict):
    File: Union[str, bytes, IO[Any], StreamingBody],
```

## CreateGameResultTypeDef

```python
# CreateGameResultTypeDef definition

class CreateGameResultTypeDef(TypedDict):
    Game: GameDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameDetailsTypeDef](./type_defs.md#gamedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisconnectPlayerResultTypeDef

```python
# DisconnectPlayerResultTypeDef definition

class DisconnectPlayerResultTypeDef(TypedDict):
    DisconnectFailures: List[str],
    DisconnectSuccesses: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportSnapshotResultTypeDef

```python
# ExportSnapshotResultTypeDef definition

class ExportSnapshotResultTypeDef(TypedDict):
    S3Url: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGameResultTypeDef

```python
# GetGameResultTypeDef definition

class GetGameResultTypeDef(TypedDict):
    Game: GameDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameDetailsTypeDef](./type_defs.md#gamedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPlayerConnectionStatusResultTypeDef

```python
# GetPlayerConnectionStatusResultTypeDef definition

class GetPlayerConnectionStatusResultTypeDef(TypedDict):
    Connections: List[ConnectionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConnectionTypeDef](./type_defs.md#connectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartGeneratedCodeJobResultTypeDef

```python
# StartGeneratedCodeJobResultTypeDef definition

class StartGeneratedCodeJobResultTypeDef(TypedDict):
    GeneratedCodeJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGameResultTypeDef

```python
# UpdateGameResultTypeDef definition

class UpdateGameResultTypeDef(TypedDict):
    Game: GameDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameDetailsTypeDef](./type_defs.md#gamedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateStageResultTypeDef

```python
# CreateStageResultTypeDef definition

class CreateStageResultTypeDef(TypedDict):
    Stage: StageDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageDetailsTypeDef](./type_defs.md#stagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetStageResultTypeDef

```python
# GetStageResultTypeDef definition

class GetStageResultTypeDef(TypedDict):
    Stage: StageDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageDetailsTypeDef](./type_defs.md#stagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateStageResultTypeDef

```python
# UpdateStageResultTypeDef definition

class UpdateStageResultTypeDef(TypedDict):
    Stage: StageDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageDetailsTypeDef](./type_defs.md#stagedetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StageDeploymentDetailsTypeDef

```python
# StageDeploymentDetailsTypeDef definition

class StageDeploymentDetailsTypeDef(TypedDict):
    Created: NotRequired[datetime],
    DeploymentAction: NotRequired[DeploymentActionType],  # (1)
    DeploymentId: NotRequired[str],
    DeploymentResult: NotRequired[DeploymentResultTypeDef],  # (2)
    DeploymentState: NotRequired[DeploymentStateType],  # (3)
    LastUpdated: NotRequired[datetime],
    SnapshotId: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentActionType](./literals.md#deploymentactiontype) 
2. See [:material-code-braces: DeploymentResultTypeDef](./type_defs.md#deploymentresulttypedef) 
3. See [:material-code-brackets: DeploymentStateType](./literals.md#deploymentstatetype) 
## StageDeploymentSummaryTypeDef

```python
# StageDeploymentSummaryTypeDef definition

class StageDeploymentSummaryTypeDef(TypedDict):
    DeploymentAction: NotRequired[DeploymentActionType],  # (1)
    DeploymentId: NotRequired[str],
    DeploymentResult: NotRequired[DeploymentResultTypeDef],  # (2)
    DeploymentState: NotRequired[DeploymentStateType],  # (3)
    LastUpdated: NotRequired[datetime],
    SnapshotId: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentActionType](./literals.md#deploymentactiontype) 
2. See [:material-code-braces: DeploymentResultTypeDef](./type_defs.md#deploymentresulttypedef) 
3. See [:material-code-brackets: DeploymentStateType](./literals.md#deploymentstatetype) 
## GetExtensionResultTypeDef

```python
# GetExtensionResultTypeDef definition

class GetExtensionResultTypeDef(TypedDict):
    Extension: ExtensionDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExtensionDetailsTypeDef](./type_defs.md#extensiondetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExtensionsResultTypeDef

```python
# ListExtensionsResultTypeDef definition

class ListExtensionsResultTypeDef(TypedDict):
    Extensions: List[ExtensionDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExtensionDetailsTypeDef](./type_defs.md#extensiondetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExtensionVersionResultTypeDef

```python
# GetExtensionVersionResultTypeDef definition

class GetExtensionVersionResultTypeDef(TypedDict):
    ExtensionVersion: ExtensionVersionDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExtensionVersionDetailsTypeDef](./type_defs.md#extensionversiondetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExtensionVersionsResultTypeDef

```python
# ListExtensionVersionsResultTypeDef definition

class ListExtensionVersionsResultTypeDef(TypedDict):
    ExtensionVersions: List[ExtensionVersionDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExtensionVersionDetailsTypeDef](./type_defs.md#extensionversiondetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GameConfigurationDetailsTypeDef

```python
# GameConfigurationDetailsTypeDef definition

class GameConfigurationDetailsTypeDef(TypedDict):
    Created: NotRequired[datetime],
    LastUpdated: NotRequired[datetime],
    Sections: NotRequired[Dict[str, SectionTypeDef]],  # (1)
```

1. See [:material-code-braces: SectionTypeDef](./type_defs.md#sectiontypedef) 
## SnapshotDetailsTypeDef

```python
# SnapshotDetailsTypeDef definition

class SnapshotDetailsTypeDef(TypedDict):
    Created: NotRequired[datetime],
    Description: NotRequired[str],
    Id: NotRequired[str],
    LastUpdated: NotRequired[datetime],
    Sections: NotRequired[Dict[str, SectionTypeDef]],  # (1)
```

1. See [:material-code-braces: SectionTypeDef](./type_defs.md#sectiontypedef) 
## ListGamesResultTypeDef

```python
# ListGamesResultTypeDef definition

class ListGamesResultTypeDef(TypedDict):
    Games: List[GameSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameSummaryTypeDef](./type_defs.md#gamesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGeneratedCodeJobResultTypeDef

```python
# GetGeneratedCodeJobResultTypeDef definition

class GetGeneratedCodeJobResultTypeDef(TypedDict):
    GeneratedCodeJob: GeneratedCodeJobDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeneratedCodeJobDetailsTypeDef](./type_defs.md#generatedcodejobdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGeneratedCodeJobsResultTypeDef

```python
# ListGeneratedCodeJobsResultTypeDef definition

class ListGeneratedCodeJobsResultTypeDef(TypedDict):
    GeneratedCodeJobs: List[GeneratedCodeJobDetailsTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GeneratedCodeJobDetailsTypeDef](./type_defs.md#generatedcodejobdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartGeneratedCodeJobRequestRequestTypeDef

```python
# StartGeneratedCodeJobRequestRequestTypeDef definition

class StartGeneratedCodeJobRequestRequestTypeDef(TypedDict):
    GameName: str,
    Generator: GeneratorTypeDef,  # (1)
    SnapshotId: str,
```

1. See [:material-code-braces: GeneratorTypeDef](./type_defs.md#generatortypedef) 
## ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef

```python
# ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef definition

class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(TypedDict):
    Name: str,
    Namespace: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListExtensionsRequestListExtensionsPaginateTypeDef

```python
# ListExtensionsRequestListExtensionsPaginateTypeDef definition

class ListExtensionsRequestListExtensionsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGamesRequestListGamesPaginateTypeDef

```python
# ListGamesRequestListGamesPaginateTypeDef definition

class ListGamesRequestListGamesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef

```python
# ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef definition

class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(TypedDict):
    GameName: str,
    SnapshotId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSnapshotsRequestListSnapshotsPaginateTypeDef

```python
# ListSnapshotsRequestListSnapshotsPaginateTypeDef definition

class ListSnapshotsRequestListSnapshotsPaginateTypeDef(TypedDict):
    GameName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef

```python
# ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef definition

class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(TypedDict):
    GameName: str,
    StageName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListStagesRequestListStagesPaginateTypeDef

```python
# ListStagesRequestListStagesPaginateTypeDef definition

class ListStagesRequestListStagesPaginateTypeDef(TypedDict):
    GameName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSnapshotsResultTypeDef

```python
# ListSnapshotsResultTypeDef definition

class ListSnapshotsResultTypeDef(TypedDict):
    NextToken: str,
    Snapshots: List[SnapshotSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotSummaryTypeDef](./type_defs.md#snapshotsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStagesResultTypeDef

```python
# ListStagesResultTypeDef definition

class ListStagesResultTypeDef(TypedDict):
    NextToken: str,
    Stages: List[StageSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageSummaryTypeDef](./type_defs.md#stagesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGameConfigurationRequestRequestTypeDef

```python
# UpdateGameConfigurationRequestRequestTypeDef definition

class UpdateGameConfigurationRequestRequestTypeDef(TypedDict):
    GameName: str,
    Modifications: Sequence[SectionModificationTypeDef],  # (1)
```

1. See [:material-code-braces: SectionModificationTypeDef](./type_defs.md#sectionmodificationtypedef) 
## ImportGameConfigurationRequestRequestTypeDef

```python
# ImportGameConfigurationRequestRequestTypeDef definition

class ImportGameConfigurationRequestRequestTypeDef(TypedDict):
    GameName: str,
    ImportSource: ImportGameConfigurationSourceTypeDef,  # (1)
```

1. See [:material-code-braces: ImportGameConfigurationSourceTypeDef](./type_defs.md#importgameconfigurationsourcetypedef) 
## GetStageDeploymentResultTypeDef

```python
# GetStageDeploymentResultTypeDef definition

class GetStageDeploymentResultTypeDef(TypedDict):
    StageDeployment: StageDeploymentDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageDeploymentDetailsTypeDef](./type_defs.md#stagedeploymentdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartStageDeploymentResultTypeDef

```python
# StartStageDeploymentResultTypeDef definition

class StartStageDeploymentResultTypeDef(TypedDict):
    StageDeployment: StageDeploymentDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageDeploymentDetailsTypeDef](./type_defs.md#stagedeploymentdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStageDeploymentsResultTypeDef

```python
# ListStageDeploymentsResultTypeDef definition

class ListStageDeploymentsResultTypeDef(TypedDict):
    NextToken: str,
    StageDeployments: List[StageDeploymentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StageDeploymentSummaryTypeDef](./type_defs.md#stagedeploymentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGameConfigurationResultTypeDef

```python
# GetGameConfigurationResultTypeDef definition

class GetGameConfigurationResultTypeDef(TypedDict):
    GameConfiguration: GameConfigurationDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameConfigurationDetailsTypeDef](./type_defs.md#gameconfigurationdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportGameConfigurationResultTypeDef

```python
# ImportGameConfigurationResultTypeDef definition

class ImportGameConfigurationResultTypeDef(TypedDict):
    GameConfiguration: GameConfigurationDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameConfigurationDetailsTypeDef](./type_defs.md#gameconfigurationdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGameConfigurationResultTypeDef

```python
# UpdateGameConfigurationResultTypeDef definition

class UpdateGameConfigurationResultTypeDef(TypedDict):
    GameConfiguration: GameConfigurationDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GameConfigurationDetailsTypeDef](./type_defs.md#gameconfigurationdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSnapshotResultTypeDef

```python
# CreateSnapshotResultTypeDef definition

class CreateSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotDetailsTypeDef](./type_defs.md#snapshotdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSnapshotResultTypeDef

```python
# GetSnapshotResultTypeDef definition

class GetSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotDetailsTypeDef](./type_defs.md#snapshotdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSnapshotResultTypeDef

```python
# UpdateSnapshotResultTypeDef definition

class UpdateSnapshotResultTypeDef(TypedDict):
    Snapshot: SnapshotDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SnapshotDetailsTypeDef](./type_defs.md#snapshotdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

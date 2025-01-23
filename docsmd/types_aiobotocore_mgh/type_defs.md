# Type definitions

> [Index](../README.md) > [MigrationHub](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MigrationHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#migrationhub)
    type annotations stubs module [types-aiobotocore-mgh](https://pypi.org/project/types-aiobotocore-mgh/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## ApplicationStateTypeDef

```python
# ApplicationStateTypeDef definition

class ApplicationStateTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    ApplicationStatus: NotRequired[ApplicationStatusType],  # (1)
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
## CreatedArtifactTypeDef

```python
# CreatedArtifactTypeDef definition

class CreatedArtifactTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
```

## DiscoveredResourceTypeDef

```python
# DiscoveredResourceTypeDef definition

class DiscoveredResourceTypeDef(TypedDict):
    ConfigurationId: str,
    Description: NotRequired[str],
```

## SourceResourceTypeDef

```python
# SourceResourceTypeDef definition

class SourceResourceTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    StatusDetail: NotRequired[str],
```

## CreateProgressUpdateStreamRequestRequestTypeDef

```python
# CreateProgressUpdateStreamRequestRequestTypeDef definition

class CreateProgressUpdateStreamRequestRequestTypeDef(TypedDict):
    ProgressUpdateStreamName: str,
    DryRun: NotRequired[bool],
```

## DeleteProgressUpdateStreamRequestRequestTypeDef

```python
# DeleteProgressUpdateStreamRequestRequestTypeDef definition

class DeleteProgressUpdateStreamRequestRequestTypeDef(TypedDict):
    ProgressUpdateStreamName: str,
    DryRun: NotRequired[bool],
```

## DescribeApplicationStateRequestRequestTypeDef

```python
# DescribeApplicationStateRequestRequestTypeDef definition

class DescribeApplicationStateRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
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

## DescribeMigrationTaskRequestRequestTypeDef

```python
# DescribeMigrationTaskRequestRequestTypeDef definition

class DescribeMigrationTaskRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
```

## DisassociateCreatedArtifactRequestRequestTypeDef

```python
# DisassociateCreatedArtifactRequestRequestTypeDef definition

class DisassociateCreatedArtifactRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    CreatedArtifactName: str,
    DryRun: NotRequired[bool],
```

## DisassociateDiscoveredResourceRequestRequestTypeDef

```python
# DisassociateDiscoveredResourceRequestRequestTypeDef definition

class DisassociateDiscoveredResourceRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    ConfigurationId: str,
    DryRun: NotRequired[bool],
```

## DisassociateSourceResourceRequestRequestTypeDef

```python
# DisassociateSourceResourceRequestRequestTypeDef definition

class DisassociateSourceResourceRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    SourceResourceName: str,
    DryRun: NotRequired[bool],
```

## ImportMigrationTaskRequestRequestTypeDef

```python
# ImportMigrationTaskRequestRequestTypeDef definition

class ImportMigrationTaskRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    DryRun: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationStatesRequestRequestTypeDef

```python
# ListApplicationStatesRequestRequestTypeDef definition

class ListApplicationStatesRequestRequestTypeDef(TypedDict):
    ApplicationIds: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListCreatedArtifactsRequestRequestTypeDef

```python
# ListCreatedArtifactsRequestRequestTypeDef definition

class ListCreatedArtifactsRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDiscoveredResourcesRequestRequestTypeDef

```python
# ListDiscoveredResourcesRequestRequestTypeDef definition

class ListDiscoveredResourcesRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMigrationTaskUpdatesRequestRequestTypeDef

```python
# ListMigrationTaskUpdatesRequestRequestTypeDef definition

class ListMigrationTaskUpdatesRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListMigrationTasksRequestRequestTypeDef

```python
# ListMigrationTasksRequestRequestTypeDef definition

class ListMigrationTasksRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    ResourceName: NotRequired[str],
```

## MigrationTaskSummaryTypeDef

```python
# MigrationTaskSummaryTypeDef definition

class MigrationTaskSummaryTypeDef(TypedDict):
    ProgressUpdateStream: NotRequired[str],
    MigrationTaskName: NotRequired[str],
    Status: NotRequired[StatusType],  # (1)
    ProgressPercent: NotRequired[int],
    StatusDetail: NotRequired[str],
    UpdateDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ListProgressUpdateStreamsRequestRequestTypeDef

```python
# ListProgressUpdateStreamsRequestRequestTypeDef definition

class ListProgressUpdateStreamsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ProgressUpdateStreamSummaryTypeDef

```python
# ProgressUpdateStreamSummaryTypeDef definition

class ProgressUpdateStreamSummaryTypeDef(TypedDict):
    ProgressUpdateStreamName: NotRequired[str],
```

## ListSourceResourcesRequestRequestTypeDef

```python
# ListSourceResourcesRequestRequestTypeDef definition

class ListSourceResourcesRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ResourceAttributeTypeDef

```python
# ResourceAttributeTypeDef definition

class ResourceAttributeTypeDef(TypedDict):
    Type: ResourceAttributeTypeType,  # (1)
    Value: str,
```

1. See [:material-code-brackets: ResourceAttributeTypeType](./literals.md#resourceattributetypetype) 
## TaskTypeDef

```python
# TaskTypeDef definition

class TaskTypeDef(TypedDict):
    Status: StatusType,  # (1)
    StatusDetail: NotRequired[str],
    ProgressPercent: NotRequired[int],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## AssociateCreatedArtifactRequestRequestTypeDef

```python
# AssociateCreatedArtifactRequestRequestTypeDef definition

class AssociateCreatedArtifactRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    CreatedArtifact: CreatedArtifactTypeDef,  # (1)
    DryRun: NotRequired[bool],
```

1. See [:material-code-braces: CreatedArtifactTypeDef](./type_defs.md#createdartifacttypedef) 
## AssociateDiscoveredResourceRequestRequestTypeDef

```python
# AssociateDiscoveredResourceRequestRequestTypeDef definition

class AssociateDiscoveredResourceRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    DiscoveredResource: DiscoveredResourceTypeDef,  # (1)
    DryRun: NotRequired[bool],
```

1. See [:material-code-braces: DiscoveredResourceTypeDef](./type_defs.md#discoveredresourcetypedef) 
## AssociateSourceResourceRequestRequestTypeDef

```python
# AssociateSourceResourceRequestRequestTypeDef definition

class AssociateSourceResourceRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    SourceResource: SourceResourceTypeDef,  # (1)
    DryRun: NotRequired[bool],
```

1. See [:material-code-braces: SourceResourceTypeDef](./type_defs.md#sourceresourcetypedef) 
## DescribeApplicationStateResultTypeDef

```python
# DescribeApplicationStateResultTypeDef definition

class DescribeApplicationStateResultTypeDef(TypedDict):
    ApplicationStatus: ApplicationStatusType,  # (1)
    LastUpdatedTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationStatesResultTypeDef

```python
# ListApplicationStatesResultTypeDef definition

class ListApplicationStatesResultTypeDef(TypedDict):
    ApplicationStateList: List[ApplicationStateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationStateTypeDef](./type_defs.md#applicationstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCreatedArtifactsResultTypeDef

```python
# ListCreatedArtifactsResultTypeDef definition

class ListCreatedArtifactsResultTypeDef(TypedDict):
    CreatedArtifactList: List[CreatedArtifactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CreatedArtifactTypeDef](./type_defs.md#createdartifacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDiscoveredResourcesResultTypeDef

```python
# ListDiscoveredResourcesResultTypeDef definition

class ListDiscoveredResourcesResultTypeDef(TypedDict):
    DiscoveredResourceList: List[DiscoveredResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DiscoveredResourceTypeDef](./type_defs.md#discoveredresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSourceResourcesResultTypeDef

```python
# ListSourceResourcesResultTypeDef definition

class ListSourceResourcesResultTypeDef(TypedDict):
    SourceResourceList: List[SourceResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SourceResourceTypeDef](./type_defs.md#sourceresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationStatesRequestPaginateTypeDef

```python
# ListApplicationStatesRequestPaginateTypeDef definition

class ListApplicationStatesRequestPaginateTypeDef(TypedDict):
    ApplicationIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCreatedArtifactsRequestPaginateTypeDef

```python
# ListCreatedArtifactsRequestPaginateTypeDef definition

class ListCreatedArtifactsRequestPaginateTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDiscoveredResourcesRequestPaginateTypeDef

```python
# ListDiscoveredResourcesRequestPaginateTypeDef definition

class ListDiscoveredResourcesRequestPaginateTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMigrationTaskUpdatesRequestPaginateTypeDef

```python
# ListMigrationTaskUpdatesRequestPaginateTypeDef definition

class ListMigrationTaskUpdatesRequestPaginateTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMigrationTasksRequestPaginateTypeDef

```python
# ListMigrationTasksRequestPaginateTypeDef definition

class ListMigrationTasksRequestPaginateTypeDef(TypedDict):
    ResourceName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProgressUpdateStreamsRequestPaginateTypeDef

```python
# ListProgressUpdateStreamsRequestPaginateTypeDef definition

class ListProgressUpdateStreamsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSourceResourcesRequestPaginateTypeDef

```python
# ListSourceResourcesRequestPaginateTypeDef definition

class ListSourceResourcesRequestPaginateTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMigrationTasksResultTypeDef

```python
# ListMigrationTasksResultTypeDef definition

class ListMigrationTasksResultTypeDef(TypedDict):
    MigrationTaskSummaryList: List[MigrationTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MigrationTaskSummaryTypeDef](./type_defs.md#migrationtasksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProgressUpdateStreamsResultTypeDef

```python
# ListProgressUpdateStreamsResultTypeDef definition

class ListProgressUpdateStreamsResultTypeDef(TypedDict):
    ProgressUpdateStreamSummaryList: List[ProgressUpdateStreamSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProgressUpdateStreamSummaryTypeDef](./type_defs.md#progressupdatestreamsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutResourceAttributesRequestRequestTypeDef

```python
# PutResourceAttributesRequestRequestTypeDef definition

class PutResourceAttributesRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    ResourceAttributeList: Sequence[ResourceAttributeTypeDef],  # (1)
    DryRun: NotRequired[bool],
```

1. See [:material-code-braces: ResourceAttributeTypeDef](./type_defs.md#resourceattributetypedef) 
## MigrationTaskTypeDef

```python
# MigrationTaskTypeDef definition

class MigrationTaskTypeDef(TypedDict):
    ProgressUpdateStream: NotRequired[str],
    MigrationTaskName: NotRequired[str],
    Task: NotRequired[TaskTypeDef],  # (1)
    UpdateDateTime: NotRequired[datetime],
    ResourceAttributeList: NotRequired[List[ResourceAttributeTypeDef]],  # (2)
```

1. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
2. See [:material-code-braces: ResourceAttributeTypeDef](./type_defs.md#resourceattributetypedef) 
## MigrationTaskUpdateTypeDef

```python
# MigrationTaskUpdateTypeDef definition

class MigrationTaskUpdateTypeDef(TypedDict):
    UpdateDateTime: NotRequired[datetime],
    UpdateType: NotRequired[UpdateTypeType],  # (1)
    MigrationTaskState: NotRequired[TaskTypeDef],  # (2)
```

1. See [:material-code-brackets: UpdateTypeType](./literals.md#updatetypetype) 
2. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
## NotifyApplicationStateRequestRequestTypeDef

```python
# NotifyApplicationStateRequestRequestTypeDef definition

class NotifyApplicationStateRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    Status: ApplicationStatusType,  # (1)
    UpdateDateTime: NotRequired[TimestampTypeDef],
    DryRun: NotRequired[bool],
```

1. See [:material-code-brackets: ApplicationStatusType](./literals.md#applicationstatustype) 
## NotifyMigrationTaskStateRequestRequestTypeDef

```python
# NotifyMigrationTaskStateRequestRequestTypeDef definition

class NotifyMigrationTaskStateRequestRequestTypeDef(TypedDict):
    ProgressUpdateStream: str,
    MigrationTaskName: str,
    Task: TaskTypeDef,  # (1)
    UpdateDateTime: TimestampTypeDef,
    NextUpdateSeconds: int,
    DryRun: NotRequired[bool],
```

1. See [:material-code-braces: TaskTypeDef](./type_defs.md#tasktypedef) 
## DescribeMigrationTaskResultTypeDef

```python
# DescribeMigrationTaskResultTypeDef definition

class DescribeMigrationTaskResultTypeDef(TypedDict):
    MigrationTask: MigrationTaskTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MigrationTaskTypeDef](./type_defs.md#migrationtasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMigrationTaskUpdatesResultTypeDef

```python
# ListMigrationTaskUpdatesResultTypeDef definition

class ListMigrationTaskUpdatesResultTypeDef(TypedDict):
    MigrationTaskUpdateList: List[MigrationTaskUpdateTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MigrationTaskUpdateTypeDef](./type_defs.md#migrationtaskupdatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

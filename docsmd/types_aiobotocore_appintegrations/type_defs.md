# Type definitions

> [Index](../README.md) > [AppIntegrationsService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## ExternalUrlConfigUnionTypeDef

```python
# ExternalUrlConfigUnionTypeDef definition

ExternalUrlConfigUnionTypeDef = Union[
    ExternalUrlConfigTypeDef,  # (1)
    ExternalUrlConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExternalUrlConfigTypeDef](./type_defs.md#externalurlconfigtypedef) 
2. See [:material-code-braces: ExternalUrlConfigOutputTypeDef](./type_defs.md#externalurlconfigoutputtypedef) 



## ApplicationAssociationSummaryTypeDef

```python
# ApplicationAssociationSummaryTypeDef definition

class ApplicationAssociationSummaryTypeDef(TypedDict):
    ApplicationAssociationArn: NotRequired[str],
    ApplicationArn: NotRequired[str],
    ClientId: NotRequired[str],
```

## ExternalUrlConfigOutputTypeDef

```python
# ExternalUrlConfigOutputTypeDef definition

class ExternalUrlConfigOutputTypeDef(TypedDict):
    AccessUrl: str,
    ApprovedOrigins: NotRequired[List[str]],
```

## ApplicationSummaryTypeDef

```python
# ApplicationSummaryTypeDef definition

class ApplicationSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    Namespace: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

## PublicationTypeDef

```python
# PublicationTypeDef definition

class PublicationTypeDef(TypedDict):
    Event: str,
    Schema: str,
    Description: NotRequired[str],
```

## SubscriptionTypeDef

```python
# SubscriptionTypeDef definition

class SubscriptionTypeDef(TypedDict):
    Event: str,
    Description: NotRequired[str],
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

## FileConfigurationTypeDef

```python
# FileConfigurationTypeDef definition

class FileConfigurationTypeDef(TypedDict):
    Folders: Sequence[str],
    Filters: NotRequired[Mapping[str, Sequence[str]]],
```

## ScheduleConfigurationTypeDef

```python
# ScheduleConfigurationTypeDef definition

class ScheduleConfigurationTypeDef(TypedDict):
    ScheduleExpression: str,
    FirstExecutionFrom: NotRequired[str],
    Object: NotRequired[str],
```

## FileConfigurationOutputTypeDef

```python
# FileConfigurationOutputTypeDef definition

class FileConfigurationOutputTypeDef(TypedDict):
    Folders: List[str],
    Filters: NotRequired[Dict[str, List[str]]],
```

## EventFilterTypeDef

```python
# EventFilterTypeDef definition

class EventFilterTypeDef(TypedDict):
    Source: str,
```

## LastExecutionStatusTypeDef

```python
# LastExecutionStatusTypeDef definition

class LastExecutionStatusTypeDef(TypedDict):
    ExecutionStatus: NotRequired[ExecutionStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ExecutionStatusType](./literals.md#executionstatustype) 
## DataIntegrationSummaryTypeDef

```python
# DataIntegrationSummaryTypeDef definition

class DataIntegrationSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    SourceURI: NotRequired[str],
```

## DeleteApplicationRequestRequestTypeDef

```python
# DeleteApplicationRequestRequestTypeDef definition

class DeleteApplicationRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## DeleteDataIntegrationRequestRequestTypeDef

```python
# DeleteDataIntegrationRequestRequestTypeDef definition

class DeleteDataIntegrationRequestRequestTypeDef(TypedDict):
    DataIntegrationIdentifier: str,
```

## DeleteEventIntegrationRequestRequestTypeDef

```python
# DeleteEventIntegrationRequestRequestTypeDef definition

class DeleteEventIntegrationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## EventIntegrationAssociationTypeDef

```python
# EventIntegrationAssociationTypeDef definition

class EventIntegrationAssociationTypeDef(TypedDict):
    EventIntegrationAssociationArn: NotRequired[str],
    EventIntegrationAssociationId: NotRequired[str],
    EventIntegrationName: NotRequired[str],
    ClientId: NotRequired[str],
    EventBridgeRuleName: NotRequired[str],
    ClientAssociationMetadata: NotRequired[Dict[str, str]],
```

## OnDemandConfigurationTypeDef

```python
# OnDemandConfigurationTypeDef definition

class OnDemandConfigurationTypeDef(TypedDict):
    StartTime: str,
    EndTime: NotRequired[str],
```

## ExternalUrlConfigTypeDef

```python
# ExternalUrlConfigTypeDef definition

class ExternalUrlConfigTypeDef(TypedDict):
    AccessUrl: str,
    ApprovedOrigins: NotRequired[Sequence[str]],
```

## GetApplicationRequestRequestTypeDef

```python
# GetApplicationRequestRequestTypeDef definition

class GetApplicationRequestRequestTypeDef(TypedDict):
    Arn: str,
```

## GetDataIntegrationRequestRequestTypeDef

```python
# GetDataIntegrationRequestRequestTypeDef definition

class GetDataIntegrationRequestRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetEventIntegrationRequestRequestTypeDef

```python
# GetEventIntegrationRequestRequestTypeDef definition

class GetEventIntegrationRequestRequestTypeDef(TypedDict):
    Name: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListApplicationAssociationsRequestRequestTypeDef

```python
# ListApplicationAssociationsRequestRequestTypeDef definition

class ListApplicationAssociationsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListApplicationsRequestRequestTypeDef

```python
# ListApplicationsRequestRequestTypeDef definition

class ListApplicationsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDataIntegrationAssociationsRequestRequestTypeDef

```python
# ListDataIntegrationAssociationsRequestRequestTypeDef definition

class ListDataIntegrationAssociationsRequestRequestTypeDef(TypedDict):
    DataIntegrationIdentifier: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDataIntegrationsRequestRequestTypeDef

```python
# ListDataIntegrationsRequestRequestTypeDef definition

class ListDataIntegrationsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListEventIntegrationAssociationsRequestRequestTypeDef

```python
# ListEventIntegrationAssociationsRequestRequestTypeDef definition

class ListEventIntegrationAssociationsRequestRequestTypeDef(TypedDict):
    EventIntegrationName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListEventIntegrationsRequestRequestTypeDef

```python
# ListEventIntegrationsRequestRequestTypeDef definition

class ListEventIntegrationsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateDataIntegrationRequestRequestTypeDef

```python
# UpdateDataIntegrationRequestRequestTypeDef definition

class UpdateDataIntegrationRequestRequestTypeDef(TypedDict):
    Identifier: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
```

## UpdateEventIntegrationRequestRequestTypeDef

```python
# UpdateEventIntegrationRequestRequestTypeDef definition

class UpdateEventIntegrationRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
```

## ApplicationSourceConfigOutputTypeDef

```python
# ApplicationSourceConfigOutputTypeDef definition

class ApplicationSourceConfigOutputTypeDef(TypedDict):
    ExternalUrlConfig: NotRequired[ExternalUrlConfigOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ExternalUrlConfigOutputTypeDef](./type_defs.md#externalurlconfigoutputtypedef) 
## CreateApplicationResponseTypeDef

```python
# CreateApplicationResponseTypeDef definition

class CreateApplicationResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataIntegrationAssociationResponseTypeDef

```python
# CreateDataIntegrationAssociationResponseTypeDef definition

class CreateDataIntegrationAssociationResponseTypeDef(TypedDict):
    DataIntegrationAssociationId: str,
    DataIntegrationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventIntegrationResponseTypeDef

```python
# CreateEventIntegrationResponseTypeDef definition

class CreateEventIntegrationResponseTypeDef(TypedDict):
    EventIntegrationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationAssociationsResponseTypeDef

```python
# ListApplicationAssociationsResponseTypeDef definition

class ListApplicationAssociationsResponseTypeDef(TypedDict):
    ApplicationAssociations: List[ApplicationAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationAssociationSummaryTypeDef](./type_defs.md#applicationassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListApplicationsResponseTypeDef

```python
# ListApplicationsResponseTypeDef definition

class ListApplicationsResponseTypeDef(TypedDict):
    Applications: List[ApplicationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationSummaryTypeDef](./type_defs.md#applicationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataIntegrationRequestRequestTypeDef

```python
# CreateDataIntegrationRequestRequestTypeDef definition

class CreateDataIntegrationRequestRequestTypeDef(TypedDict):
    Name: str,
    KmsKey: str,
    Description: NotRequired[str],
    SourceURI: NotRequired[str],
    ScheduleConfig: NotRequired[ScheduleConfigurationTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
    FileConfiguration: NotRequired[FileConfigurationTypeDef],  # (2)
    ObjectConfiguration: NotRequired[Mapping[str, Mapping[str, Sequence[str]]]],
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: FileConfigurationTypeDef](./type_defs.md#fileconfigurationtypedef) 
## CreateDataIntegrationResponseTypeDef

```python
# CreateDataIntegrationResponseTypeDef definition

class CreateDataIntegrationResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    Description: str,
    KmsKey: str,
    SourceURI: str,
    ScheduleConfiguration: ScheduleConfigurationTypeDef,  # (1)
    Tags: Dict[str, str],
    ClientToken: str,
    FileConfiguration: FileConfigurationOutputTypeDef,  # (2)
    ObjectConfiguration: Dict[str, Dict[str, List[str]]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: FileConfigurationOutputTypeDef](./type_defs.md#fileconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataIntegrationResponseTypeDef

```python
# GetDataIntegrationResponseTypeDef definition

class GetDataIntegrationResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    Description: str,
    KmsKey: str,
    SourceURI: str,
    ScheduleConfiguration: ScheduleConfigurationTypeDef,  # (1)
    Tags: Dict[str, str],
    FileConfiguration: FileConfigurationOutputTypeDef,  # (2)
    ObjectConfiguration: Dict[str, Dict[str, List[str]]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: FileConfigurationOutputTypeDef](./type_defs.md#fileconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventIntegrationRequestRequestTypeDef

```python
# CreateEventIntegrationRequestRequestTypeDef definition

class CreateEventIntegrationRequestRequestTypeDef(TypedDict):
    Name: str,
    EventFilter: EventFilterTypeDef,  # (1)
    EventBridgeBus: str,
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
## EventIntegrationTypeDef

```python
# EventIntegrationTypeDef definition

class EventIntegrationTypeDef(TypedDict):
    EventIntegrationArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    EventFilter: NotRequired[EventFilterTypeDef],  # (1)
    EventBridgeBus: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
## GetEventIntegrationResponseTypeDef

```python
# GetEventIntegrationResponseTypeDef definition

class GetEventIntegrationResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    EventIntegrationArn: str,
    EventBridgeBus: str,
    EventFilter: EventFilterTypeDef,  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataIntegrationsResponseTypeDef

```python
# ListDataIntegrationsResponseTypeDef definition

class ListDataIntegrationsResponseTypeDef(TypedDict):
    DataIntegrations: List[DataIntegrationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataIntegrationSummaryTypeDef](./type_defs.md#dataintegrationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventIntegrationAssociationsResponseTypeDef

```python
# ListEventIntegrationAssociationsResponseTypeDef definition

class ListEventIntegrationAssociationsResponseTypeDef(TypedDict):
    EventIntegrationAssociations: List[EventIntegrationAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EventIntegrationAssociationTypeDef](./type_defs.md#eventintegrationassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecutionConfigurationTypeDef

```python
# ExecutionConfigurationTypeDef definition

class ExecutionConfigurationTypeDef(TypedDict):
    ExecutionMode: ExecutionModeType,  # (1)
    OnDemandConfiguration: NotRequired[OnDemandConfigurationTypeDef],  # (2)
    ScheduleConfiguration: NotRequired[ScheduleConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: ExecutionModeType](./literals.md#executionmodetype) 
2. See [:material-code-braces: OnDemandConfigurationTypeDef](./type_defs.md#ondemandconfigurationtypedef) 
3. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
## ListApplicationAssociationsRequestListApplicationAssociationsPaginateTypeDef

```python
# ListApplicationAssociationsRequestListApplicationAssociationsPaginateTypeDef definition

class ListApplicationAssociationsRequestListApplicationAssociationsPaginateTypeDef(TypedDict):
    ApplicationId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListApplicationsRequestListApplicationsPaginateTypeDef

```python
# ListApplicationsRequestListApplicationsPaginateTypeDef definition

class ListApplicationsRequestListApplicationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataIntegrationAssociationsRequestListDataIntegrationAssociationsPaginateTypeDef

```python
# ListDataIntegrationAssociationsRequestListDataIntegrationAssociationsPaginateTypeDef definition

class ListDataIntegrationAssociationsRequestListDataIntegrationAssociationsPaginateTypeDef(TypedDict):
    DataIntegrationIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataIntegrationsRequestListDataIntegrationsPaginateTypeDef

```python
# ListDataIntegrationsRequestListDataIntegrationsPaginateTypeDef definition

class ListDataIntegrationsRequestListDataIntegrationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventIntegrationAssociationsRequestListEventIntegrationAssociationsPaginateTypeDef

```python
# ListEventIntegrationAssociationsRequestListEventIntegrationAssociationsPaginateTypeDef definition

class ListEventIntegrationAssociationsRequestListEventIntegrationAssociationsPaginateTypeDef(TypedDict):
    EventIntegrationName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEventIntegrationsRequestListEventIntegrationsPaginateTypeDef

```python
# ListEventIntegrationsRequestListEventIntegrationsPaginateTypeDef definition

class ListEventIntegrationsRequestListEventIntegrationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetApplicationResponseTypeDef

```python
# GetApplicationResponseTypeDef definition

class GetApplicationResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    Namespace: str,
    Description: str,
    ApplicationSourceConfig: ApplicationSourceConfigOutputTypeDef,  # (1)
    Subscriptions: List[SubscriptionTypeDef],  # (2)
    Publications: List[PublicationTypeDef],  # (3)
    CreatedTime: datetime,
    LastModifiedTime: datetime,
    Tags: Dict[str, str],
    Permissions: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ApplicationSourceConfigOutputTypeDef](./type_defs.md#applicationsourceconfigoutputtypedef) 
2. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
3. See [:material-code-braces: PublicationTypeDef](./type_defs.md#publicationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventIntegrationsResponseTypeDef

```python
# ListEventIntegrationsResponseTypeDef definition

class ListEventIntegrationsResponseTypeDef(TypedDict):
    EventIntegrations: List[EventIntegrationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EventIntegrationTypeDef](./type_defs.md#eventintegrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataIntegrationAssociationRequestRequestTypeDef

```python
# CreateDataIntegrationAssociationRequestRequestTypeDef definition

class CreateDataIntegrationAssociationRequestRequestTypeDef(TypedDict):
    DataIntegrationIdentifier: str,
    ClientId: NotRequired[str],
    ObjectConfiguration: NotRequired[Mapping[str, Mapping[str, Sequence[str]]]],
    DestinationURI: NotRequired[str],
    ClientAssociationMetadata: NotRequired[Mapping[str, str]],
    ClientToken: NotRequired[str],
    ExecutionConfiguration: NotRequired[ExecutionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: ExecutionConfigurationTypeDef](./type_defs.md#executionconfigurationtypedef) 
## DataIntegrationAssociationSummaryTypeDef

```python
# DataIntegrationAssociationSummaryTypeDef definition

class DataIntegrationAssociationSummaryTypeDef(TypedDict):
    DataIntegrationAssociationArn: NotRequired[str],
    DataIntegrationArn: NotRequired[str],
    ClientId: NotRequired[str],
    DestinationURI: NotRequired[str],
    LastExecutionStatus: NotRequired[LastExecutionStatusTypeDef],  # (1)
    ExecutionConfiguration: NotRequired[ExecutionConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: LastExecutionStatusTypeDef](./type_defs.md#lastexecutionstatustypedef) 
2. See [:material-code-braces: ExecutionConfigurationTypeDef](./type_defs.md#executionconfigurationtypedef) 
## UpdateDataIntegrationAssociationRequestRequestTypeDef

```python
# UpdateDataIntegrationAssociationRequestRequestTypeDef definition

class UpdateDataIntegrationAssociationRequestRequestTypeDef(TypedDict):
    DataIntegrationIdentifier: str,
    DataIntegrationAssociationIdentifier: str,
    ExecutionConfiguration: ExecutionConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: ExecutionConfigurationTypeDef](./type_defs.md#executionconfigurationtypedef) 
## ApplicationSourceConfigTypeDef

```python
# ApplicationSourceConfigTypeDef definition

class ApplicationSourceConfigTypeDef(TypedDict):
    ExternalUrlConfig: NotRequired[ExternalUrlConfigUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ExternalUrlConfigTypeDef](./type_defs.md#externalurlconfigtypedef) [:material-code-braces: ExternalUrlConfigOutputTypeDef](./type_defs.md#externalurlconfigoutputtypedef) 
## ListDataIntegrationAssociationsResponseTypeDef

```python
# ListDataIntegrationAssociationsResponseTypeDef definition

class ListDataIntegrationAssociationsResponseTypeDef(TypedDict):
    DataIntegrationAssociations: List[DataIntegrationAssociationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataIntegrationAssociationSummaryTypeDef](./type_defs.md#dataintegrationassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateApplicationRequestRequestTypeDef

```python
# CreateApplicationRequestRequestTypeDef definition

class CreateApplicationRequestRequestTypeDef(TypedDict):
    Name: str,
    Namespace: str,
    ApplicationSourceConfig: ApplicationSourceConfigTypeDef,  # (1)
    Description: NotRequired[str],
    Subscriptions: NotRequired[Sequence[SubscriptionTypeDef]],  # (2)
    Publications: NotRequired[Sequence[PublicationTypeDef]],  # (3)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    Permissions: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ApplicationSourceConfigTypeDef](./type_defs.md#applicationsourceconfigtypedef) 
2. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
3. See [:material-code-braces: PublicationTypeDef](./type_defs.md#publicationtypedef) 
## UpdateApplicationRequestRequestTypeDef

```python
# UpdateApplicationRequestRequestTypeDef definition

class UpdateApplicationRequestRequestTypeDef(TypedDict):
    Arn: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    ApplicationSourceConfig: NotRequired[ApplicationSourceConfigTypeDef],  # (1)
    Subscriptions: NotRequired[Sequence[SubscriptionTypeDef]],  # (2)
    Publications: NotRequired[Sequence[PublicationTypeDef]],  # (3)
    Permissions: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ApplicationSourceConfigTypeDef](./type_defs.md#applicationsourceconfigtypedef) 
2. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
3. See [:material-code-braces: PublicationTypeDef](./type_defs.md#publicationtypedef) 

# Type definitions

> [Index](../README.md) > [AppIntegrationsService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).



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

## EventFilterTypeDef

```python
# EventFilterTypeDef definition

class EventFilterTypeDef(TypedDict):
    Source: str,
```

## DataIntegrationAssociationSummaryTypeDef

```python
# DataIntegrationAssociationSummaryTypeDef definition

class DataIntegrationAssociationSummaryTypeDef(TypedDict):
    DataIntegrationAssociationArn: NotRequired[str],
    DataIntegrationArn: NotRequired[str],
    ClientId: NotRequired[str],
```

## DataIntegrationSummaryTypeDef

```python
# DataIntegrationSummaryTypeDef definition

class DataIntegrationSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Name: NotRequired[str],
    SourceURI: NotRequired[str],
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

## CreateDataIntegrationRequestRequestTypeDef

```python
# CreateDataIntegrationRequestRequestTypeDef definition

class CreateDataIntegrationRequestRequestTypeDef(TypedDict):
    Name: str,
    KmsKey: str,
    SourceURI: str,
    ScheduleConfig: ScheduleConfigurationTypeDef,  # (1)
    Description: NotRequired[str],
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
    FileConfiguration: FileConfigurationTypeDef,  # (2)
    ObjectConfiguration: Dict[str, Dict[str, List[str]]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: FileConfigurationTypeDef](./type_defs.md#fileconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEventIntegrationResponseTypeDef

```python
# CreateEventIntegrationResponseTypeDef definition

class CreateEventIntegrationResponseTypeDef(TypedDict):
    EventIntegrationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    FileConfiguration: FileConfigurationTypeDef,  # (2)
    ObjectConfiguration: Dict[str, Dict[str, List[str]]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
2. See [:material-code-braces: FileConfigurationTypeDef](./type_defs.md#fileconfigurationtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## ListDataIntegrationAssociationsResponseTypeDef

```python
# ListDataIntegrationAssociationsResponseTypeDef definition

class ListDataIntegrationAssociationsResponseTypeDef(TypedDict):
    DataIntegrationAssociations: List[DataIntegrationAssociationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataIntegrationAssociationSummaryTypeDef](./type_defs.md#dataintegrationassociationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataIntegrationsResponseTypeDef

```python
# ListDataIntegrationsResponseTypeDef definition

class ListDataIntegrationsResponseTypeDef(TypedDict):
    DataIntegrations: List[DataIntegrationSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataIntegrationSummaryTypeDef](./type_defs.md#dataintegrationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventIntegrationAssociationsResponseTypeDef

```python
# ListEventIntegrationAssociationsResponseTypeDef definition

class ListEventIntegrationAssociationsResponseTypeDef(TypedDict):
    EventIntegrationAssociations: List[EventIntegrationAssociationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventIntegrationAssociationTypeDef](./type_defs.md#eventintegrationassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEventIntegrationsResponseTypeDef

```python
# ListEventIntegrationsResponseTypeDef definition

class ListEventIntegrationsResponseTypeDef(TypedDict):
    EventIntegrations: List[EventIntegrationTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventIntegrationTypeDef](./type_defs.md#eventintegrationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

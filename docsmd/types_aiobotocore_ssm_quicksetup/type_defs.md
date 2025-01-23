# Type definitions

> [Index](../README.md) > [SystemsManagerQuickSetup](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SystemsManagerQuickSetup](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-quicksetup.html#systemsmanagerquicksetup)
    type annotations stubs module [types-aiobotocore-ssm-quicksetup](https://pypi.org/project/types-aiobotocore-ssm-quicksetup/).



## ConfigurationDefinitionInputTypeDef

```python
# ConfigurationDefinitionInputTypeDef definition

class ConfigurationDefinitionInputTypeDef(TypedDict):
    Parameters: Mapping[str, str],
    Type: str,
    LocalDeploymentAdministrationRoleArn: NotRequired[str],
    LocalDeploymentExecutionRoleName: NotRequired[str],
    TypeVersion: NotRequired[str],
```

## ConfigurationDefinitionSummaryTypeDef

```python
# ConfigurationDefinitionSummaryTypeDef definition

class ConfigurationDefinitionSummaryTypeDef(TypedDict):
    FirstClassParameters: NotRequired[Dict[str, str]],
    Id: NotRequired[str],
    Type: NotRequired[str],
    TypeVersion: NotRequired[str],
```

## ConfigurationDefinitionTypeDef

```python
# ConfigurationDefinitionTypeDef definition

class ConfigurationDefinitionTypeDef(TypedDict):
    Parameters: Dict[str, str],
    Type: str,
    Id: NotRequired[str],
    LocalDeploymentAdministrationRoleArn: NotRequired[str],
    LocalDeploymentExecutionRoleName: NotRequired[str],
    TypeVersion: NotRequired[str],
```

## StatusSummaryTypeDef

```python
# StatusSummaryTypeDef definition

class StatusSummaryTypeDef(TypedDict):
    LastUpdatedAt: datetime,
    StatusType: StatusTypeType,  # (2)
    Status: NotRequired[StatusType],  # (1)
    StatusDetails: NotRequired[Dict[str, str]],
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
2. See [:material-code-brackets: StatusTypeType](./literals.md#statustypetype) 
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

## DeleteConfigurationManagerInputRequestTypeDef

```python
# DeleteConfigurationManagerInputRequestTypeDef definition

class DeleteConfigurationManagerInputRequestTypeDef(TypedDict):
    ManagerArn: str,
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Key: str,
    Values: Sequence[str],
```

## GetConfigurationInputRequestTypeDef

```python
# GetConfigurationInputRequestTypeDef definition

class GetConfigurationInputRequestTypeDef(TypedDict):
    ConfigurationId: str,
```

## GetConfigurationManagerInputRequestTypeDef

```python
# GetConfigurationManagerInputRequestTypeDef definition

class GetConfigurationManagerInputRequestTypeDef(TypedDict):
    ManagerArn: str,
```

## ServiceSettingsTypeDef

```python
# ServiceSettingsTypeDef definition

class ServiceSettingsTypeDef(TypedDict):
    ExplorerEnablingRoleArn: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## QuickSetupTypeOutputTypeDef

```python
# QuickSetupTypeOutputTypeDef definition

class QuickSetupTypeOutputTypeDef(TypedDict):
    LatestVersion: NotRequired[str],
    Type: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagEntryTypeDef

```python
# TagEntryTypeDef definition

class TagEntryTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateConfigurationDefinitionInputRequestTypeDef

```python
# UpdateConfigurationDefinitionInputRequestTypeDef definition

class UpdateConfigurationDefinitionInputRequestTypeDef(TypedDict):
    Id: str,
    ManagerArn: str,
    LocalDeploymentAdministrationRoleArn: NotRequired[str],
    LocalDeploymentExecutionRoleName: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
    TypeVersion: NotRequired[str],
```

## UpdateConfigurationManagerInputRequestTypeDef

```python
# UpdateConfigurationManagerInputRequestTypeDef definition

class UpdateConfigurationManagerInputRequestTypeDef(TypedDict):
    ManagerArn: str,
    Description: NotRequired[str],
    Name: NotRequired[str],
```

## UpdateServiceSettingsInputRequestTypeDef

```python
# UpdateServiceSettingsInputRequestTypeDef definition

class UpdateServiceSettingsInputRequestTypeDef(TypedDict):
    ExplorerEnablingRoleArn: NotRequired[str],
```

## CreateConfigurationManagerInputRequestTypeDef

```python
# CreateConfigurationManagerInputRequestTypeDef definition

class CreateConfigurationManagerInputRequestTypeDef(TypedDict):
    ConfigurationDefinitions: Sequence[ConfigurationDefinitionInputTypeDef],  # (1)
    Description: NotRequired[str],
    Name: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ConfigurationDefinitionInputTypeDef](./type_defs.md#configurationdefinitioninputtypedef) 
## ConfigurationManagerSummaryTypeDef

```python
# ConfigurationManagerSummaryTypeDef definition

class ConfigurationManagerSummaryTypeDef(TypedDict):
    ManagerArn: str,
    ConfigurationDefinitionSummaries: NotRequired[List[ConfigurationDefinitionSummaryTypeDef]],  # (1)
    Description: NotRequired[str],
    Name: NotRequired[str],
    StatusSummaries: NotRequired[List[StatusSummaryTypeDef]],  # (2)
```

1. See [:material-code-braces: ConfigurationDefinitionSummaryTypeDef](./type_defs.md#configurationdefinitionsummarytypedef) 
2. See [:material-code-braces: StatusSummaryTypeDef](./type_defs.md#statussummarytypedef) 
## ConfigurationSummaryTypeDef

```python
# ConfigurationSummaryTypeDef definition

class ConfigurationSummaryTypeDef(TypedDict):
    Account: NotRequired[str],
    ConfigurationDefinitionId: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    FirstClassParameters: NotRequired[Dict[str, str]],
    Id: NotRequired[str],
    ManagerArn: NotRequired[str],
    Region: NotRequired[str],
    StatusSummaries: NotRequired[List[StatusSummaryTypeDef]],  # (1)
    Type: NotRequired[str],
    TypeVersion: NotRequired[str],
```

1. See [:material-code-braces: StatusSummaryTypeDef](./type_defs.md#statussummarytypedef) 
## CreateConfigurationManagerOutputTypeDef

```python
# CreateConfigurationManagerOutputTypeDef definition

class CreateConfigurationManagerOutputTypeDef(TypedDict):
    ManagerArn: str,
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
## GetConfigurationManagerOutputTypeDef

```python
# GetConfigurationManagerOutputTypeDef definition

class GetConfigurationManagerOutputTypeDef(TypedDict):
    ConfigurationDefinitions: List[ConfigurationDefinitionTypeDef],  # (1)
    CreatedAt: datetime,
    Description: str,
    LastModifiedAt: datetime,
    ManagerArn: str,
    Name: str,
    StatusSummaries: List[StatusSummaryTypeDef],  # (2)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConfigurationDefinitionTypeDef](./type_defs.md#configurationdefinitiontypedef) 
2. See [:material-code-braces: StatusSummaryTypeDef](./type_defs.md#statussummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConfigurationOutputTypeDef

```python
# GetConfigurationOutputTypeDef definition

class GetConfigurationOutputTypeDef(TypedDict):
    Account: str,
    ConfigurationDefinitionId: str,
    CreatedAt: datetime,
    Id: str,
    LastModifiedAt: datetime,
    ManagerArn: str,
    Parameters: Dict[str, str],
    Region: str,
    StatusSummaries: List[StatusSummaryTypeDef],  # (1)
    Type: str,
    TypeVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StatusSummaryTypeDef](./type_defs.md#statussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationManagersInputRequestTypeDef

```python
# ListConfigurationManagersInputRequestTypeDef definition

class ListConfigurationManagersInputRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    MaxItems: NotRequired[int],
    StartingToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListConfigurationsInputRequestTypeDef

```python
# ListConfigurationsInputRequestTypeDef definition

class ListConfigurationsInputRequestTypeDef(TypedDict):
    ConfigurationDefinitionId: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    ManagerArn: NotRequired[str],
    MaxItems: NotRequired[int],
    StartingToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetServiceSettingsOutputTypeDef

```python
# GetServiceSettingsOutputTypeDef definition

class GetServiceSettingsOutputTypeDef(TypedDict):
    ServiceSettings: ServiceSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSettingsTypeDef](./type_defs.md#servicesettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationManagersInputPaginateTypeDef

```python
# ListConfigurationManagersInputPaginateTypeDef definition

class ListConfigurationManagersInputPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationsInputPaginateTypeDef

```python
# ListConfigurationsInputPaginateTypeDef definition

class ListConfigurationsInputPaginateTypeDef(TypedDict):
    ConfigurationDefinitionId: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    ManagerArn: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQuickSetupTypesOutputTypeDef

```python
# ListQuickSetupTypesOutputTypeDef definition

class ListQuickSetupTypesOutputTypeDef(TypedDict):
    QuickSetupTypeList: List[QuickSetupTypeOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QuickSetupTypeOutputTypeDef](./type_defs.md#quicksetuptypeoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagEntryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagEntryTypeDef](./type_defs.md#tagentrytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationManagersOutputTypeDef

```python
# ListConfigurationManagersOutputTypeDef definition

class ListConfigurationManagersOutputTypeDef(TypedDict):
    ConfigurationManagersList: List[ConfigurationManagerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationManagerSummaryTypeDef](./type_defs.md#configurationmanagersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationsOutputTypeDef

```python
# ListConfigurationsOutputTypeDef definition

class ListConfigurationsOutputTypeDef(TypedDict):
    ConfigurationsList: List[ConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationSummaryTypeDef](./type_defs.md#configurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

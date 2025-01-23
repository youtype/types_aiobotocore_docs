# Type definitions

> [Index](../README.md) > [ResourceGroups](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#resourcegroups)
    type annotations stubs module [types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).

## GroupConfigurationParameterUnionTypeDef

```python
# GroupConfigurationParameterUnionTypeDef definition

GroupConfigurationParameterUnionTypeDef = Union[
    GroupConfigurationParameterTypeDef,  # (1)
    GroupConfigurationParameterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GroupConfigurationParameterTypeDef](./type_defs.md#groupconfigurationparametertypedef) 
2. See [:material-code-braces: GroupConfigurationParameterOutputTypeDef](./type_defs.md#groupconfigurationparameteroutputtypedef) 

## GroupConfigurationItemUnionTypeDef

```python
# GroupConfigurationItemUnionTypeDef definition

GroupConfigurationItemUnionTypeDef = Union[
    GroupConfigurationItemTypeDef,  # (1)
    GroupConfigurationItemOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) 
2. See [:material-code-braces: GroupConfigurationItemOutputTypeDef](./type_defs.md#groupconfigurationitemoutputtypedef) 



## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    GroupLifecycleEventsDesiredStatus: NotRequired[GroupLifecycleEventsDesiredStatusType],  # (1)
    GroupLifecycleEventsStatus: NotRequired[GroupLifecycleEventsStatusType],  # (2)
    GroupLifecycleEventsStatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: GroupLifecycleEventsDesiredStatusType](./literals.md#grouplifecycleeventsdesiredstatustype) 
2. See [:material-code-brackets: GroupLifecycleEventsStatusType](./literals.md#grouplifecycleeventsstatustype) 
## CancelTagSyncTaskInputRequestTypeDef

```python
# CancelTagSyncTaskInputRequestTypeDef definition

class CancelTagSyncTaskInputRequestTypeDef(TypedDict):
    TaskArn: str,
```

## ResourceQueryTypeDef

```python
# ResourceQueryTypeDef definition

class ResourceQueryTypeDef(TypedDict):
    Type: QueryTypeType,  # (1)
    Query: str,
```

1. See [:material-code-brackets: QueryTypeType](./literals.md#querytypetype) 
## GroupTypeDef

```python
# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    GroupArn: str,
    Name: str,
    Description: NotRequired[str],
    Criticality: NotRequired[int],
    Owner: NotRequired[str],
    DisplayName: NotRequired[str],
    ApplicationTag: NotRequired[Dict[str, str]],
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

## DeleteGroupInputRequestTypeDef

```python
# DeleteGroupInputRequestTypeDef definition

class DeleteGroupInputRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    Group: NotRequired[str],
```

## FailedResourceTypeDef

```python
# FailedResourceTypeDef definition

class FailedResourceTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    ErrorMessage: NotRequired[str],
    ErrorCode: NotRequired[str],
```

## GetGroupConfigurationInputRequestTypeDef

```python
# GetGroupConfigurationInputRequestTypeDef definition

class GetGroupConfigurationInputRequestTypeDef(TypedDict):
    Group: NotRequired[str],
```

## GetGroupInputRequestTypeDef

```python
# GetGroupInputRequestTypeDef definition

class GetGroupInputRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    Group: NotRequired[str],
```

## GetGroupQueryInputRequestTypeDef

```python
# GetGroupQueryInputRequestTypeDef definition

class GetGroupQueryInputRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    Group: NotRequired[str],
```

## GetTagSyncTaskInputRequestTypeDef

```python
# GetTagSyncTaskInputRequestTypeDef definition

class GetTagSyncTaskInputRequestTypeDef(TypedDict):
    TaskArn: str,
```

## GetTagsInputRequestTypeDef

```python
# GetTagsInputRequestTypeDef definition

class GetTagsInputRequestTypeDef(TypedDict):
    Arn: str,
```

## GroupConfigurationParameterOutputTypeDef

```python
# GroupConfigurationParameterOutputTypeDef definition

class GroupConfigurationParameterOutputTypeDef(TypedDict):
    Name: str,
    Values: NotRequired[List[str]],
```

## GroupConfigurationParameterTypeDef

```python
# GroupConfigurationParameterTypeDef definition

class GroupConfigurationParameterTypeDef(TypedDict):
    Name: str,
    Values: NotRequired[Sequence[str]],
```

## GroupFilterTypeDef

```python
# GroupFilterTypeDef definition

class GroupFilterTypeDef(TypedDict):
    Name: GroupFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: GroupFilterNameType](./literals.md#groupfilternametype) 
## GroupIdentifierTypeDef

```python
# GroupIdentifierTypeDef definition

class GroupIdentifierTypeDef(TypedDict):
    GroupName: NotRequired[str],
    GroupArn: NotRequired[str],
    Description: NotRequired[str],
    Criticality: NotRequired[int],
    Owner: NotRequired[str],
    DisplayName: NotRequired[str],
```

## GroupResourcesInputRequestTypeDef

```python
# GroupResourcesInputRequestTypeDef definition

class GroupResourcesInputRequestTypeDef(TypedDict):
    Group: str,
    ResourceArns: Sequence[str],
```

## PendingResourceTypeDef

```python
# PendingResourceTypeDef definition

class PendingResourceTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
```

## GroupingStatusesItemTypeDef

```python
# GroupingStatusesItemTypeDef definition

class GroupingStatusesItemTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    Action: NotRequired[GroupingTypeType],  # (1)
    Status: NotRequired[GroupingStatusType],  # (2)
    ErrorMessage: NotRequired[str],
    ErrorCode: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: GroupingTypeType](./literals.md#groupingtypetype) 
2. See [:material-code-brackets: GroupingStatusType](./literals.md#groupingstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ResourceFilterTypeDef

```python
# ResourceFilterTypeDef definition

class ResourceFilterTypeDef(TypedDict):
    Name: ResourceFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ResourceFilterNameType](./literals.md#resourcefilternametype) 
## ResourceIdentifierTypeDef

```python
# ResourceIdentifierTypeDef definition

class ResourceIdentifierTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[str],
```

## ResourceStatusTypeDef

```python
# ResourceStatusTypeDef definition

class ResourceStatusTypeDef(TypedDict):
    Name: NotRequired[ResourceStatusValueType],  # (1)
```

1. See [:material-code-brackets: ResourceStatusValueType](./literals.md#resourcestatusvaluetype) 
## QueryErrorTypeDef

```python
# QueryErrorTypeDef definition

class QueryErrorTypeDef(TypedDict):
    ErrorCode: NotRequired[QueryErrorCodeType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: QueryErrorCodeType](./literals.md#queryerrorcodetype) 
## ListGroupingStatusesFilterTypeDef

```python
# ListGroupingStatusesFilterTypeDef definition

class ListGroupingStatusesFilterTypeDef(TypedDict):
    Name: ListGroupingStatusesFilterNameType,  # (1)
    Values: Sequence[str],
```

1. See [:material-code-brackets: ListGroupingStatusesFilterNameType](./literals.md#listgroupingstatusesfilternametype) 
## ListTagSyncTasksFilterTypeDef

```python
# ListTagSyncTasksFilterTypeDef definition

class ListTagSyncTasksFilterTypeDef(TypedDict):
    GroupArn: NotRequired[str],
    GroupName: NotRequired[str],
```

## TagSyncTaskItemTypeDef

```python
# TagSyncTaskItemTypeDef definition

class TagSyncTaskItemTypeDef(TypedDict):
    GroupArn: NotRequired[str],
    GroupName: NotRequired[str],
    TaskArn: NotRequired[str],
    TagKey: NotRequired[str],
    TagValue: NotRequired[str],
    RoleArn: NotRequired[str],
    Status: NotRequired[TagSyncTaskStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    CreatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: TagSyncTaskStatusType](./literals.md#tagsynctaskstatustype) 
## StartTagSyncTaskInputRequestTypeDef

```python
# StartTagSyncTaskInputRequestTypeDef definition

class StartTagSyncTaskInputRequestTypeDef(TypedDict):
    Group: str,
    TagKey: str,
    TagValue: str,
    RoleArn: str,
```

## TagInputRequestTypeDef

```python
# TagInputRequestTypeDef definition

class TagInputRequestTypeDef(TypedDict):
    Arn: str,
    Tags: Mapping[str, str],
```

## UngroupResourcesInputRequestTypeDef

```python
# UngroupResourcesInputRequestTypeDef definition

class UngroupResourcesInputRequestTypeDef(TypedDict):
    Group: str,
    ResourceArns: Sequence[str],
```

## UntagInputRequestTypeDef

```python
# UntagInputRequestTypeDef definition

class UntagInputRequestTypeDef(TypedDict):
    Arn: str,
    Keys: Sequence[str],
```

## UpdateAccountSettingsInputRequestTypeDef

```python
# UpdateAccountSettingsInputRequestTypeDef definition

class UpdateAccountSettingsInputRequestTypeDef(TypedDict):
    GroupLifecycleEventsDesiredStatus: NotRequired[GroupLifecycleEventsDesiredStatusType],  # (1)
```

1. See [:material-code-brackets: GroupLifecycleEventsDesiredStatusType](./literals.md#grouplifecycleeventsdesiredstatustype) 
## UpdateGroupInputRequestTypeDef

```python
# UpdateGroupInputRequestTypeDef definition

class UpdateGroupInputRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    Group: NotRequired[str],
    Description: NotRequired[str],
    Criticality: NotRequired[int],
    Owner: NotRequired[str],
    DisplayName: NotRequired[str],
```

## GroupQueryTypeDef

```python
# GroupQueryTypeDef definition

class GroupQueryTypeDef(TypedDict):
    GroupName: str,
    ResourceQuery: ResourceQueryTypeDef,  # (1)
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
## SearchResourcesInputRequestTypeDef

```python
# SearchResourcesInputRequestTypeDef definition

class SearchResourcesInputRequestTypeDef(TypedDict):
    ResourceQuery: ResourceQueryTypeDef,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
## UpdateGroupQueryInputRequestTypeDef

```python
# UpdateGroupQueryInputRequestTypeDef definition

class UpdateGroupQueryInputRequestTypeDef(TypedDict):
    ResourceQuery: ResourceQueryTypeDef,  # (1)
    GroupName: NotRequired[str],
    Group: NotRequired[str],
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
## DeleteGroupOutputTypeDef

```python
# DeleteGroupOutputTypeDef definition

class DeleteGroupOutputTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountSettingsOutputTypeDef

```python
# GetAccountSettingsOutputTypeDef definition

class GetAccountSettingsOutputTypeDef(TypedDict):
    AccountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupOutputTypeDef

```python
# GetGroupOutputTypeDef definition

class GetGroupOutputTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagSyncTaskOutputTypeDef

```python
# GetTagSyncTaskOutputTypeDef definition

class GetTagSyncTaskOutputTypeDef(TypedDict):
    GroupArn: str,
    GroupName: str,
    TaskArn: str,
    TagKey: str,
    TagValue: str,
    RoleArn: str,
    Status: TagSyncTaskStatusType,  # (1)
    ErrorMessage: str,
    CreatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TagSyncTaskStatusType](./literals.md#tagsynctaskstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTagsOutputTypeDef

```python
# GetTagsOutputTypeDef definition

class GetTagsOutputTypeDef(TypedDict):
    Arn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartTagSyncTaskOutputTypeDef

```python
# StartTagSyncTaskOutputTypeDef definition

class StartTagSyncTaskOutputTypeDef(TypedDict):
    GroupArn: str,
    GroupName: str,
    TaskArn: str,
    TagKey: str,
    TagValue: str,
    RoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagOutputTypeDef

```python
# TagOutputTypeDef definition

class TagOutputTypeDef(TypedDict):
    Arn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagOutputTypeDef

```python
# UntagOutputTypeDef definition

class UntagOutputTypeDef(TypedDict):
    Arn: str,
    Keys: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountSettingsOutputTypeDef

```python
# UpdateAccountSettingsOutputTypeDef definition

class UpdateAccountSettingsOutputTypeDef(TypedDict):
    AccountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGroupOutputTypeDef

```python
# UpdateGroupOutputTypeDef definition

class UpdateGroupOutputTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GroupConfigurationItemOutputTypeDef

```python
# GroupConfigurationItemOutputTypeDef definition

class GroupConfigurationItemOutputTypeDef(TypedDict):
    Type: str,
    Parameters: NotRequired[List[GroupConfigurationParameterOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: GroupConfigurationParameterOutputTypeDef](./type_defs.md#groupconfigurationparameteroutputtypedef) 
## ListGroupsInputRequestTypeDef

```python
# ListGroupsInputRequestTypeDef definition

class ListGroupsInputRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[GroupFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupFilterTypeDef](./type_defs.md#groupfiltertypedef) 
## ListGroupsOutputTypeDef

```python
# ListGroupsOutputTypeDef definition

class ListGroupsOutputTypeDef(TypedDict):
    GroupIdentifiers: List[GroupIdentifierTypeDef],  # (1)
    Groups: List[GroupTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupIdentifierTypeDef](./type_defs.md#groupidentifiertypedef) 
2. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GroupResourcesOutputTypeDef

```python
# GroupResourcesOutputTypeDef definition

class GroupResourcesOutputTypeDef(TypedDict):
    Succeeded: List[str],
    Failed: List[FailedResourceTypeDef],  # (1)
    Pending: List[PendingResourceTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FailedResourceTypeDef](./type_defs.md#failedresourcetypedef) 
2. See [:material-code-braces: PendingResourceTypeDef](./type_defs.md#pendingresourcetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UngroupResourcesOutputTypeDef

```python
# UngroupResourcesOutputTypeDef definition

class UngroupResourcesOutputTypeDef(TypedDict):
    Succeeded: List[str],
    Failed: List[FailedResourceTypeDef],  # (1)
    Pending: List[PendingResourceTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FailedResourceTypeDef](./type_defs.md#failedresourcetypedef) 
2. See [:material-code-braces: PendingResourceTypeDef](./type_defs.md#pendingresourcetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupingStatusesOutputTypeDef

```python
# ListGroupingStatusesOutputTypeDef definition

class ListGroupingStatusesOutputTypeDef(TypedDict):
    Group: str,
    GroupingStatuses: List[GroupingStatusesItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupingStatusesItemTypeDef](./type_defs.md#groupingstatusesitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsInputPaginateTypeDef

```python
# ListGroupsInputPaginateTypeDef definition

class ListGroupsInputPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[GroupFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: GroupFilterTypeDef](./type_defs.md#groupfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchResourcesInputPaginateTypeDef

```python
# SearchResourcesInputPaginateTypeDef definition

class SearchResourcesInputPaginateTypeDef(TypedDict):
    ResourceQuery: ResourceQueryTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupResourcesInputPaginateTypeDef

```python
# ListGroupResourcesInputPaginateTypeDef definition

class ListGroupResourcesInputPaginateTypeDef(TypedDict):
    GroupName: NotRequired[str],
    Group: NotRequired[str],
    Filters: NotRequired[Sequence[ResourceFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupResourcesInputRequestTypeDef

```python
# ListGroupResourcesInputRequestTypeDef definition

class ListGroupResourcesInputRequestTypeDef(TypedDict):
    GroupName: NotRequired[str],
    Group: NotRequired[str],
    Filters: NotRequired[Sequence[ResourceFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceFilterTypeDef](./type_defs.md#resourcefiltertypedef) 
## ListGroupResourcesItemTypeDef

```python
# ListGroupResourcesItemTypeDef definition

class ListGroupResourcesItemTypeDef(TypedDict):
    Identifier: NotRequired[ResourceIdentifierTypeDef],  # (1)
    Status: NotRequired[ResourceStatusTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: ResourceStatusTypeDef](./type_defs.md#resourcestatustypedef) 
## SearchResourcesOutputTypeDef

```python
# SearchResourcesOutputTypeDef definition

class SearchResourcesOutputTypeDef(TypedDict):
    ResourceIdentifiers: List[ResourceIdentifierTypeDef],  # (1)
    QueryErrors: List[QueryErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: QueryErrorTypeDef](./type_defs.md#queryerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupingStatusesInputPaginateTypeDef

```python
# ListGroupingStatusesInputPaginateTypeDef definition

class ListGroupingStatusesInputPaginateTypeDef(TypedDict):
    Group: str,
    Filters: NotRequired[Sequence[ListGroupingStatusesFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListGroupingStatusesFilterTypeDef](./type_defs.md#listgroupingstatusesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupingStatusesInputRequestTypeDef

```python
# ListGroupingStatusesInputRequestTypeDef definition

class ListGroupingStatusesInputRequestTypeDef(TypedDict):
    Group: str,
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[ListGroupingStatusesFilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListGroupingStatusesFilterTypeDef](./type_defs.md#listgroupingstatusesfiltertypedef) 
## ListTagSyncTasksInputPaginateTypeDef

```python
# ListTagSyncTasksInputPaginateTypeDef definition

class ListTagSyncTasksInputPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ListTagSyncTasksFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListTagSyncTasksFilterTypeDef](./type_defs.md#listtagsynctasksfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagSyncTasksInputRequestTypeDef

```python
# ListTagSyncTasksInputRequestTypeDef definition

class ListTagSyncTasksInputRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ListTagSyncTasksFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListTagSyncTasksFilterTypeDef](./type_defs.md#listtagsynctasksfiltertypedef) 
## ListTagSyncTasksOutputTypeDef

```python
# ListTagSyncTasksOutputTypeDef definition

class ListTagSyncTasksOutputTypeDef(TypedDict):
    TagSyncTasks: List[TagSyncTaskItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagSyncTaskItemTypeDef](./type_defs.md#tagsynctaskitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupQueryOutputTypeDef

```python
# GetGroupQueryOutputTypeDef definition

class GetGroupQueryOutputTypeDef(TypedDict):
    GroupQuery: GroupQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupQueryTypeDef](./type_defs.md#groupquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGroupQueryOutputTypeDef

```python
# UpdateGroupQueryOutputTypeDef definition

class UpdateGroupQueryOutputTypeDef(TypedDict):
    GroupQuery: GroupQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupQueryTypeDef](./type_defs.md#groupquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GroupConfigurationTypeDef

```python
# GroupConfigurationTypeDef definition

class GroupConfigurationTypeDef(TypedDict):
    Configuration: NotRequired[List[GroupConfigurationItemOutputTypeDef]],  # (1)
    ProposedConfiguration: NotRequired[List[GroupConfigurationItemOutputTypeDef]],  # (1)
    Status: NotRequired[GroupConfigurationStatusType],  # (3)
    FailureReason: NotRequired[str],
```

1. See [:material-code-braces: GroupConfigurationItemOutputTypeDef](./type_defs.md#groupconfigurationitemoutputtypedef) 
2. See [:material-code-braces: GroupConfigurationItemOutputTypeDef](./type_defs.md#groupconfigurationitemoutputtypedef) 
3. See [:material-code-brackets: GroupConfigurationStatusType](./literals.md#groupconfigurationstatustype) 
## GroupConfigurationItemTypeDef

```python
# GroupConfigurationItemTypeDef definition

class GroupConfigurationItemTypeDef(TypedDict):
    Type: str,
    Parameters: NotRequired[Sequence[GroupConfigurationParameterUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: GroupConfigurationParameterTypeDef](./type_defs.md#groupconfigurationparametertypedef) [:material-code-braces: GroupConfigurationParameterOutputTypeDef](./type_defs.md#groupconfigurationparameteroutputtypedef) 
## ListGroupResourcesOutputTypeDef

```python
# ListGroupResourcesOutputTypeDef definition

class ListGroupResourcesOutputTypeDef(TypedDict):
    Resources: List[ListGroupResourcesItemTypeDef],  # (1)
    ResourceIdentifiers: List[ResourceIdentifierTypeDef],  # (2)
    QueryErrors: List[QueryErrorTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListGroupResourcesItemTypeDef](./type_defs.md#listgroupresourcesitemtypedef) 
2. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
3. See [:material-code-braces: QueryErrorTypeDef](./type_defs.md#queryerrortypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupOutputTypeDef

```python
# CreateGroupOutputTypeDef definition

class CreateGroupOutputTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResourceQuery: ResourceQueryTypeDef,  # (2)
    Tags: Dict[str, str],
    GroupConfiguration: GroupConfigurationTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
3. See [:material-code-braces: GroupConfigurationTypeDef](./type_defs.md#groupconfigurationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupConfigurationOutputTypeDef

```python
# GetGroupConfigurationOutputTypeDef definition

class GetGroupConfigurationOutputTypeDef(TypedDict):
    GroupConfiguration: GroupConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupConfigurationTypeDef](./type_defs.md#groupconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutGroupConfigurationInputRequestTypeDef

```python
# PutGroupConfigurationInputRequestTypeDef definition

class PutGroupConfigurationInputRequestTypeDef(TypedDict):
    Group: NotRequired[str],
    Configuration: NotRequired[Sequence[GroupConfigurationItemTypeDef]],  # (1)
```

1. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) 
## CreateGroupInputRequestTypeDef

```python
# CreateGroupInputRequestTypeDef definition

class CreateGroupInputRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    ResourceQuery: NotRequired[ResourceQueryTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
    Configuration: NotRequired[Sequence[GroupConfigurationItemUnionTypeDef]],  # (2)
    Criticality: NotRequired[int],
    Owner: NotRequired[str],
    DisplayName: NotRequired[str],
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) [:material-code-braces: GroupConfigurationItemOutputTypeDef](./type_defs.md#groupconfigurationitemoutputtypedef) 

# Type definitions

> [Index](../README.md) > [ResourceGroups](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ResourceGroups](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-groups.html#ResourceGroups)
    type annotations stubs module [types-aiobotocore-resource-groups](https://pypi.org/project/types-aiobotocore-resource-groups/).



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

## GetTagsInputRequestTypeDef

```python
# GetTagsInputRequestTypeDef definition

class GetTagsInputRequestTypeDef(TypedDict):
    Arn: str,
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
## GetTagsOutputTypeDef

```python
# GetTagsOutputTypeDef definition

class GetTagsOutputTypeDef(TypedDict):
    Arn: str,
    Tags: Dict[str, str],
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
## GroupConfigurationItemTypeDef

```python
# GroupConfigurationItemTypeDef definition

class GroupConfigurationItemTypeDef(TypedDict):
    Type: str,
    Parameters: NotRequired[Sequence[GroupConfigurationParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: GroupConfigurationParameterTypeDef](./type_defs.md#groupconfigurationparametertypedef) 
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
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
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
## ListGroupsInputListGroupsPaginateTypeDef

```python
# ListGroupsInputListGroupsPaginateTypeDef definition

class ListGroupsInputListGroupsPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[GroupFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: GroupFilterTypeDef](./type_defs.md#groupfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchResourcesInputSearchResourcesPaginateTypeDef

```python
# SearchResourcesInputSearchResourcesPaginateTypeDef definition

class SearchResourcesInputSearchResourcesPaginateTypeDef(TypedDict):
    ResourceQuery: ResourceQueryTypeDef,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListGroupResourcesInputListGroupResourcesPaginateTypeDef

```python
# ListGroupResourcesInputListGroupResourcesPaginateTypeDef definition

class ListGroupResourcesInputListGroupResourcesPaginateTypeDef(TypedDict):
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
    NextToken: str,
    QueryErrors: List[QueryErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: QueryErrorTypeDef](./type_defs.md#queryerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## CreateGroupInputRequestTypeDef

```python
# CreateGroupInputRequestTypeDef definition

class CreateGroupInputRequestTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    ResourceQuery: NotRequired[ResourceQueryTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
    Configuration: NotRequired[Sequence[GroupConfigurationItemTypeDef]],  # (2)
```

1. See [:material-code-braces: ResourceQueryTypeDef](./type_defs.md#resourcequerytypedef) 
2. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) 
## GroupConfigurationTypeDef

```python
# GroupConfigurationTypeDef definition

class GroupConfigurationTypeDef(TypedDict):
    Configuration: NotRequired[List[GroupConfigurationItemTypeDef]],  # (1)
    ProposedConfiguration: NotRequired[List[GroupConfigurationItemTypeDef]],  # (1)
    Status: NotRequired[GroupConfigurationStatusType],  # (3)
    FailureReason: NotRequired[str],
```

1. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) 
2. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) 
3. See [:material-code-brackets: GroupConfigurationStatusType](./literals.md#groupconfigurationstatustype) 
## PutGroupConfigurationInputRequestTypeDef

```python
# PutGroupConfigurationInputRequestTypeDef definition

class PutGroupConfigurationInputRequestTypeDef(TypedDict):
    Group: NotRequired[str],
    Configuration: NotRequired[Sequence[GroupConfigurationItemTypeDef]],  # (1)
```

1. See [:material-code-braces: GroupConfigurationItemTypeDef](./type_defs.md#groupconfigurationitemtypedef) 
## ListGroupResourcesOutputTypeDef

```python
# ListGroupResourcesOutputTypeDef definition

class ListGroupResourcesOutputTypeDef(TypedDict):
    Resources: List[ListGroupResourcesItemTypeDef],  # (1)
    ResourceIdentifiers: List[ResourceIdentifierTypeDef],  # (2)
    NextToken: str,
    QueryErrors: List[QueryErrorTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
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

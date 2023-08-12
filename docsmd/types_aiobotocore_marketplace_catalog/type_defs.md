# Type definitions

> [Index](../README.md) > [MarketplaceCatalog](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MarketplaceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
    type annotations stubs module [types-aiobotocore-marketplace-catalog](https://pypi.org/project/types-aiobotocore-marketplace-catalog/).



## CancelChangeSetRequestRequestTypeDef

```python
# CancelChangeSetRequestRequestTypeDef definition

class CancelChangeSetRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ChangeSetId: str,
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

## ChangeSetSummaryListItemTypeDef

```python
# ChangeSetSummaryListItemTypeDef definition

class ChangeSetSummaryListItemTypeDef(TypedDict):
    ChangeSetId: NotRequired[str],
    ChangeSetArn: NotRequired[str],
    ChangeSetName: NotRequired[str],
    StartTime: NotRequired[str],
    EndTime: NotRequired[str],
    Status: NotRequired[ChangeStatusType],  # (1)
    EntityIdList: NotRequired[List[str]],
    FailureCode: NotRequired[FailureCodeType],  # (2)
```

1. See [:material-code-brackets: ChangeStatusType](./literals.md#changestatustype) 
2. See [:material-code-brackets: FailureCodeType](./literals.md#failurecodetype) 
## EntityTypeDef

```python
# EntityTypeDef definition

class EntityTypeDef(TypedDict):
    Type: str,
    Identifier: NotRequired[str],
```

## ErrorDetailTypeDef

```python
# ErrorDetailTypeDef definition

class ErrorDetailTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteResourcePolicyRequestRequestTypeDef

```python
# DeleteResourcePolicyRequestRequestTypeDef definition

class DeleteResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## DescribeChangeSetRequestRequestTypeDef

```python
# DescribeChangeSetRequestRequestTypeDef definition

class DescribeChangeSetRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ChangeSetId: str,
```

## DescribeEntityRequestRequestTypeDef

```python
# DescribeEntityRequestRequestTypeDef definition

class DescribeEntityRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EntityId: str,
```

## EntitySummaryTypeDef

```python
# EntitySummaryTypeDef definition

class EntitySummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    EntityType: NotRequired[str],
    EntityId: NotRequired[str],
    EntityArn: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Visibility: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    ValueList: NotRequired[Sequence[str]],
```

## GetResourcePolicyRequestRequestTypeDef

```python
# GetResourcePolicyRequestRequestTypeDef definition

class GetResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## SortTypeDef

```python
# SortTypeDef definition

class SortTypeDef(TypedDict):
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PutResourcePolicyRequestRequestTypeDef

```python
# PutResourcePolicyRequestRequestTypeDef definition

class PutResourcePolicyRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Policy: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## CancelChangeSetResponseTypeDef

```python
# CancelChangeSetResponseTypeDef definition

class CancelChangeSetResponseTypeDef(TypedDict):
    ChangeSetId: str,
    ChangeSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEntityResponseTypeDef

```python
# DescribeEntityResponseTypeDef definition

class DescribeEntityResponseTypeDef(TypedDict):
    EntityType: str,
    EntityIdentifier: str,
    EntityArn: str,
    LastModifiedDate: str,
    Details: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePolicyResponseTypeDef

```python
# GetResourcePolicyResponseTypeDef definition

class GetResourcePolicyResponseTypeDef(TypedDict):
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChangeSetResponseTypeDef

```python
# StartChangeSetResponseTypeDef definition

class StartChangeSetResponseTypeDef(TypedDict):
    ChangeSetId: str,
    ChangeSetArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChangeSetsResponseTypeDef

```python
# ListChangeSetsResponseTypeDef definition

class ListChangeSetsResponseTypeDef(TypedDict):
    ChangeSetSummaryList: List[ChangeSetSummaryListItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChangeSetSummaryListItemTypeDef](./type_defs.md#changesetsummarylistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ChangeSummaryTypeDef

```python
# ChangeSummaryTypeDef definition

class ChangeSummaryTypeDef(TypedDict):
    ChangeType: NotRequired[str],
    Entity: NotRequired[EntityTypeDef],  # (1)
    Details: NotRequired[str],
    ErrorDetailList: NotRequired[List[ErrorDetailTypeDef]],  # (2)
    ChangeName: NotRequired[str],
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: ErrorDetailTypeDef](./type_defs.md#errordetailtypedef) 
## ChangeTypeDef

```python
# ChangeTypeDef definition

class ChangeTypeDef(TypedDict):
    ChangeType: str,
    Entity: EntityTypeDef,  # (1)
    Details: str,
    EntityTags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ChangeName: NotRequired[str],
```

1. See [:material-code-braces: EntityTypeDef](./type_defs.md#entitytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    ResourceArn: str,
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListEntitiesResponseTypeDef

```python
# ListEntitiesResponseTypeDef definition

class ListEntitiesResponseTypeDef(TypedDict):
    EntitySummaryList: List[EntitySummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EntitySummaryTypeDef](./type_defs.md#entitysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChangeSetsRequestListChangeSetsPaginateTypeDef

```python
# ListChangeSetsRequestListChangeSetsPaginateTypeDef definition

class ListChangeSetsRequestListChangeSetsPaginateTypeDef(TypedDict):
    Catalog: str,
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Sort: NotRequired[SortTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListChangeSetsRequestRequestTypeDef

```python
# ListChangeSetsRequestRequestTypeDef definition

class ListChangeSetsRequestRequestTypeDef(TypedDict):
    Catalog: str,
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Sort: NotRequired[SortTypeDef],  # (2)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## ListEntitiesRequestListEntitiesPaginateTypeDef

```python
# ListEntitiesRequestListEntitiesPaginateTypeDef definition

class ListEntitiesRequestListEntitiesPaginateTypeDef(TypedDict):
    Catalog: str,
    EntityType: str,
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Sort: NotRequired[SortTypeDef],  # (2)
    OwnershipType: NotRequired[OwnershipTypeType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-brackets: OwnershipTypeType](./literals.md#ownershiptypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntitiesRequestRequestTypeDef

```python
# ListEntitiesRequestRequestTypeDef definition

class ListEntitiesRequestRequestTypeDef(TypedDict):
    Catalog: str,
    EntityType: str,
    FilterList: NotRequired[Sequence[FilterTypeDef]],  # (1)
    Sort: NotRequired[SortTypeDef],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    OwnershipType: NotRequired[OwnershipTypeType],  # (3)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
3. See [:material-code-brackets: OwnershipTypeType](./literals.md#ownershiptypetype) 
## DescribeChangeSetResponseTypeDef

```python
# DescribeChangeSetResponseTypeDef definition

class DescribeChangeSetResponseTypeDef(TypedDict):
    ChangeSetId: str,
    ChangeSetArn: str,
    ChangeSetName: str,
    StartTime: str,
    EndTime: str,
    Status: ChangeStatusType,  # (1)
    FailureCode: FailureCodeType,  # (2)
    FailureDescription: str,
    ChangeSet: List[ChangeSummaryTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ChangeStatusType](./literals.md#changestatustype) 
2. See [:material-code-brackets: FailureCodeType](./literals.md#failurecodetype) 
3. See [:material-code-braces: ChangeSummaryTypeDef](./type_defs.md#changesummarytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartChangeSetRequestRequestTypeDef

```python
# StartChangeSetRequestRequestTypeDef definition

class StartChangeSetRequestRequestTypeDef(TypedDict):
    Catalog: str,
    ChangeSet: Sequence[ChangeTypeDef],  # (1)
    ChangeSetName: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    ChangeSetTags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ChangeTypeDef](./type_defs.md#changetypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 

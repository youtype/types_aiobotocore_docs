# Type definitions

> [Index](../README.md) > [RecycleBin](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RecycleBin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rbin.html#recyclebin)
    type annotations stubs module [types-aiobotocore-rbin](https://pypi.org/project/types-aiobotocore-rbin/).



## ResourceTagTypeDef

```python
# ResourceTagTypeDef definition

class ResourceTagTypeDef(TypedDict):
    ResourceTagKey: str,
    ResourceTagValue: NotRequired[str],
```

## RetentionPeriodTypeDef

```python
# RetentionPeriodTypeDef definition

class RetentionPeriodTypeDef(TypedDict):
    RetentionPeriodValue: int,
    RetentionPeriodUnit: RetentionPeriodUnitType,  # (1)
```

1. See [:material-code-brackets: RetentionPeriodUnitType](./literals.md#retentionperiodunittype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## DeleteRuleRequestRequestTypeDef

```python
# DeleteRuleRequestRequestTypeDef definition

class DeleteRuleRequestRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetRuleRequestRequestTypeDef

```python
# GetRuleRequestRequestTypeDef definition

class GetRuleRequestRequestTypeDef(TypedDict):
    Identifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## UnlockDelayTypeDef

```python
# UnlockDelayTypeDef definition

class UnlockDelayTypeDef(TypedDict):
    UnlockDelayValue: int,
    UnlockDelayUnit: UnlockDelayUnitType,  # (1)
```

1. See [:material-code-brackets: UnlockDelayUnitType](./literals.md#unlockdelayunittype) 
## UnlockRuleRequestRequestTypeDef

```python
# UnlockRuleRequestRequestTypeDef definition

class UnlockRuleRequestRequestTypeDef(TypedDict):
    Identifier: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ListRulesRequestRequestTypeDef

```python
# ListRulesRequestRequestTypeDef definition

class ListRulesRequestRequestTypeDef(TypedDict):
    ResourceType: ResourceTypeType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
    LockState: NotRequired[LockStateType],  # (3)
    ExcludeResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef definition

class RuleSummaryTypeDef(TypedDict):
    Identifier: NotRequired[str],
    Description: NotRequired[str],
    RetentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (1)
    LockState: NotRequired[LockStateType],  # (2)
    RuleArn: NotRequired[str],
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
## UpdateRuleRequestRequestTypeDef

```python
# UpdateRuleRequestRequestTypeDef definition

class UpdateRuleRequestRequestTypeDef(TypedDict):
    Identifier: str,
    RetentionPeriod: NotRequired[RetentionPeriodTypeDef],  # (1)
    Description: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (2)
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (3)
    ExcludeResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (3)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleResponseTypeDef

```python
# UpdateRuleResponseTypeDef definition

class UpdateRuleResponseTypeDef(TypedDict):
    Identifier: str,
    RetentionPeriod: RetentionPeriodTypeDef,  # (1)
    Description: str,
    ResourceType: ResourceTypeType,  # (2)
    ResourceTags: List[ResourceTagTypeDef],  # (3)
    Status: RuleStatusType,  # (4)
    LockState: LockStateType,  # (5)
    LockEndTime: datetime,
    RuleArn: str,
    ExcludeResourceTags: List[ResourceTagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
4. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
5. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
6. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRulesRequestPaginateTypeDef

```python
# ListRulesRequestPaginateTypeDef definition

class ListRulesRequestPaginateTypeDef(TypedDict):
    ResourceType: ResourceTypeType,  # (1)
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
    LockState: NotRequired[LockStateType],  # (3)
    ExcludeResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
3. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## LockConfigurationTypeDef

```python
# LockConfigurationTypeDef definition

class LockConfigurationTypeDef(TypedDict):
    UnlockDelay: UnlockDelayTypeDef,  # (1)
```

1. See [:material-code-braces: UnlockDelayTypeDef](./type_defs.md#unlockdelaytypedef) 
## ListRulesResponseTypeDef

```python
# ListRulesResponseTypeDef definition

class ListRulesResponseTypeDef(TypedDict):
    Rules: List[RuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleRequestRequestTypeDef

```python
# CreateRuleRequestRequestTypeDef definition

class CreateRuleRequestRequestTypeDef(TypedDict):
    RetentionPeriod: RetentionPeriodTypeDef,  # (1)
    ResourceType: ResourceTypeType,  # (2)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    ResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (4)
    LockConfiguration: NotRequired[LockConfigurationTypeDef],  # (5)
    ExcludeResourceTags: NotRequired[Sequence[ResourceTagTypeDef]],  # (4)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
5. See [:material-code-braces: LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef) 
6. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
## CreateRuleResponseTypeDef

```python
# CreateRuleResponseTypeDef definition

class CreateRuleResponseTypeDef(TypedDict):
    Identifier: str,
    RetentionPeriod: RetentionPeriodTypeDef,  # (1)
    Description: str,
    Tags: List[TagTypeDef],  # (2)
    ResourceType: ResourceTypeType,  # (3)
    ResourceTags: List[ResourceTagTypeDef],  # (4)
    Status: RuleStatusType,  # (5)
    LockConfiguration: LockConfigurationTypeDef,  # (6)
    LockState: LockStateType,  # (7)
    RuleArn: str,
    ExcludeResourceTags: List[ResourceTagTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (9)
```

1. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
4. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
5. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
6. See [:material-code-braces: LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef) 
7. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
8. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
9. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuleResponseTypeDef

```python
# GetRuleResponseTypeDef definition

class GetRuleResponseTypeDef(TypedDict):
    Identifier: str,
    Description: str,
    ResourceType: ResourceTypeType,  # (1)
    RetentionPeriod: RetentionPeriodTypeDef,  # (2)
    ResourceTags: List[ResourceTagTypeDef],  # (3)
    Status: RuleStatusType,  # (4)
    LockConfiguration: LockConfigurationTypeDef,  # (5)
    LockState: LockStateType,  # (6)
    LockEndTime: datetime,
    RuleArn: str,
    ExcludeResourceTags: List[ResourceTagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
4. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
5. See [:material-code-braces: LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef) 
6. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
7. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LockRuleRequestRequestTypeDef

```python
# LockRuleRequestRequestTypeDef definition

class LockRuleRequestRequestTypeDef(TypedDict):
    Identifier: str,
    LockConfiguration: LockConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef) 
## LockRuleResponseTypeDef

```python
# LockRuleResponseTypeDef definition

class LockRuleResponseTypeDef(TypedDict):
    Identifier: str,
    Description: str,
    ResourceType: ResourceTypeType,  # (1)
    RetentionPeriod: RetentionPeriodTypeDef,  # (2)
    ResourceTags: List[ResourceTagTypeDef],  # (3)
    Status: RuleStatusType,  # (4)
    LockConfiguration: LockConfigurationTypeDef,  # (5)
    LockState: LockStateType,  # (6)
    RuleArn: str,
    ExcludeResourceTags: List[ResourceTagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
4. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
5. See [:material-code-braces: LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef) 
6. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
7. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UnlockRuleResponseTypeDef

```python
# UnlockRuleResponseTypeDef definition

class UnlockRuleResponseTypeDef(TypedDict):
    Identifier: str,
    Description: str,
    ResourceType: ResourceTypeType,  # (1)
    RetentionPeriod: RetentionPeriodTypeDef,  # (2)
    ResourceTags: List[ResourceTagTypeDef],  # (3)
    Status: RuleStatusType,  # (4)
    LockConfiguration: LockConfigurationTypeDef,  # (5)
    LockState: LockStateType,  # (6)
    LockEndTime: datetime,
    RuleArn: str,
    ExcludeResourceTags: List[ResourceTagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: RetentionPeriodTypeDef](./type_defs.md#retentionperiodtypedef) 
3. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
4. See [:material-code-brackets: RuleStatusType](./literals.md#rulestatustype) 
5. See [:material-code-braces: LockConfigurationTypeDef](./type_defs.md#lockconfigurationtypedef) 
6. See [:material-code-brackets: LockStateType](./literals.md#lockstatetype) 
7. See [:material-code-braces: ResourceTagTypeDef](./type_defs.md#resourcetagtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

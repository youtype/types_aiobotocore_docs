# Type definitions

> [Index](../README.md) > [DLM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DLM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
    type annotations stubs module [types-aiobotocore-dlm](https://pypi.org/project/types-aiobotocore-dlm/).



## RetentionArchiveTierTypeDef

```python
# RetentionArchiveTierTypeDef definition

class RetentionArchiveTierTypeDef(TypedDict):
    Count: NotRequired[int],
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
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

## CreateRuleTypeDef

```python
# CreateRuleTypeDef definition

class CreateRuleTypeDef(TypedDict):
    Location: NotRequired[LocationValuesType],  # (1)
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[IntervalUnitValuesType],  # (2)
    Times: NotRequired[Sequence[str]],
    CronExpression: NotRequired[str],
```

1. See [:material-code-brackets: LocationValuesType](./literals.md#locationvaluestype) 
2. See [:material-code-brackets: IntervalUnitValuesType](./literals.md#intervalunitvaluestype) 
## CrossRegionCopyRetainRuleTypeDef

```python
# CrossRegionCopyRetainRuleTypeDef definition

class CrossRegionCopyRetainRuleTypeDef(TypedDict):
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## EncryptionConfigurationTypeDef

```python
# EncryptionConfigurationTypeDef definition

class EncryptionConfigurationTypeDef(TypedDict):
    Encrypted: bool,
    CmkArn: NotRequired[str],
```

## CrossRegionCopyDeprecateRuleTypeDef

```python
# CrossRegionCopyDeprecateRuleTypeDef definition

class CrossRegionCopyDeprecateRuleTypeDef(TypedDict):
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## DeleteLifecyclePolicyRequestRequestTypeDef

```python
# DeleteLifecyclePolicyRequestRequestTypeDef definition

class DeleteLifecyclePolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
```

## DeprecateRuleTypeDef

```python
# DeprecateRuleTypeDef definition

class DeprecateRuleTypeDef(TypedDict):
    Count: NotRequired[int],
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## EventParametersTypeDef

```python
# EventParametersTypeDef definition

class EventParametersTypeDef(TypedDict):
    EventType: EventTypeValuesType,  # (1)
    SnapshotOwner: Sequence[str],
    DescriptionRegex: str,
```

1. See [:material-code-brackets: EventTypeValuesType](./literals.md#eventtypevaluestype) 
## FastRestoreRuleTypeDef

```python
# FastRestoreRuleTypeDef definition

class FastRestoreRuleTypeDef(TypedDict):
    AvailabilityZones: Sequence[str],
    Count: NotRequired[int],
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## GetLifecyclePoliciesRequestRequestTypeDef

```python
# GetLifecyclePoliciesRequestRequestTypeDef definition

class GetLifecyclePoliciesRequestRequestTypeDef(TypedDict):
    PolicyIds: NotRequired[Sequence[str]],
    State: NotRequired[GettablePolicyStateValuesType],  # (1)
    ResourceTypes: NotRequired[Sequence[ResourceTypeValuesType]],  # (2)
    TargetTags: NotRequired[Sequence[str]],
    TagsToAdd: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: GettablePolicyStateValuesType](./literals.md#gettablepolicystatevaluestype) 
2. See [:material-code-brackets: ResourceTypeValuesType](./literals.md#resourcetypevaluestype) 
## LifecyclePolicySummaryTypeDef

```python
# LifecyclePolicySummaryTypeDef definition

class LifecyclePolicySummaryTypeDef(TypedDict):
    PolicyId: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[GettablePolicyStateValuesType],  # (1)
    Tags: NotRequired[Dict[str, str]],
    PolicyType: NotRequired[PolicyTypeValuesType],  # (2)
```

1. See [:material-code-brackets: GettablePolicyStateValuesType](./literals.md#gettablepolicystatevaluestype) 
2. See [:material-code-brackets: PolicyTypeValuesType](./literals.md#policytypevaluestype) 
## GetLifecyclePolicyRequestRequestTypeDef

```python
# GetLifecyclePolicyRequestRequestTypeDef definition

class GetLifecyclePolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## RetainRuleTypeDef

```python
# RetainRuleTypeDef definition

class RetainRuleTypeDef(TypedDict):
    Count: NotRequired[int],
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## ShareRuleTypeDef

```python
# ShareRuleTypeDef definition

class ShareRuleTypeDef(TypedDict):
    TargetAccounts: Sequence[str],
    UnshareInterval: NotRequired[int],
    UnshareIntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ArchiveRetainRuleTypeDef

```python
# ArchiveRetainRuleTypeDef definition

class ArchiveRetainRuleTypeDef(TypedDict):
    RetentionArchiveTier: RetentionArchiveTierTypeDef,  # (1)
```

1. See [:material-code-braces: RetentionArchiveTierTypeDef](./type_defs.md#retentionarchivetiertypedef) 
## CreateLifecyclePolicyResponseTypeDef

```python
# CreateLifecyclePolicyResponseTypeDef definition

class CreateLifecyclePolicyResponseTypeDef(TypedDict):
    PolicyId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CrossRegionCopyActionTypeDef

```python
# CrossRegionCopyActionTypeDef definition

class CrossRegionCopyActionTypeDef(TypedDict):
    Target: str,
    EncryptionConfiguration: EncryptionConfigurationTypeDef,  # (1)
    RetainRule: NotRequired[CrossRegionCopyRetainRuleTypeDef],  # (2)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
2. See [:material-code-braces: CrossRegionCopyRetainRuleTypeDef](./type_defs.md#crossregioncopyretainruletypedef) 
## CrossRegionCopyRuleTypeDef

```python
# CrossRegionCopyRuleTypeDef definition

class CrossRegionCopyRuleTypeDef(TypedDict):
    Encrypted: bool,
    TargetRegion: NotRequired[str],
    Target: NotRequired[str],
    CmkArn: NotRequired[str],
    CopyTags: NotRequired[bool],
    RetainRule: NotRequired[CrossRegionCopyRetainRuleTypeDef],  # (1)
    DeprecateRule: NotRequired[CrossRegionCopyDeprecateRuleTypeDef],  # (2)
```

1. See [:material-code-braces: CrossRegionCopyRetainRuleTypeDef](./type_defs.md#crossregioncopyretainruletypedef) 
2. See [:material-code-braces: CrossRegionCopyDeprecateRuleTypeDef](./type_defs.md#crossregioncopydeprecateruletypedef) 
## EventSourceTypeDef

```python
# EventSourceTypeDef definition

class EventSourceTypeDef(TypedDict):
    Type: EventSourceValuesType,  # (1)
    Parameters: NotRequired[EventParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: EventSourceValuesType](./literals.md#eventsourcevaluestype) 
2. See [:material-code-braces: EventParametersTypeDef](./type_defs.md#eventparameterstypedef) 
## GetLifecyclePoliciesResponseTypeDef

```python
# GetLifecyclePoliciesResponseTypeDef definition

class GetLifecyclePoliciesResponseTypeDef(TypedDict):
    Policies: List[LifecyclePolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecyclePolicySummaryTypeDef](./type_defs.md#lifecyclepolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ParametersTypeDef

```python
# ParametersTypeDef definition

class ParametersTypeDef(TypedDict):
    ExcludeBootVolume: NotRequired[bool],
    NoReboot: NotRequired[bool],
    ExcludeDataVolumeTags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ArchiveRuleTypeDef

```python
# ArchiveRuleTypeDef definition

class ArchiveRuleTypeDef(TypedDict):
    RetainRule: ArchiveRetainRuleTypeDef,  # (1)
```

1. See [:material-code-braces: ArchiveRetainRuleTypeDef](./type_defs.md#archiveretainruletypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    Name: str,
    CrossRegionCopy: Sequence[CrossRegionCopyActionTypeDef],  # (1)
```

1. See [:material-code-braces: CrossRegionCopyActionTypeDef](./type_defs.md#crossregioncopyactiontypedef) 
## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    Name: NotRequired[str],
    CopyTags: NotRequired[bool],
    TagsToAdd: NotRequired[Sequence[TagTypeDef]],  # (1)
    VariableTags: NotRequired[Sequence[TagTypeDef]],  # (1)
    CreateRule: NotRequired[CreateRuleTypeDef],  # (3)
    RetainRule: NotRequired[RetainRuleTypeDef],  # (4)
    FastRestoreRule: NotRequired[FastRestoreRuleTypeDef],  # (5)
    CrossRegionCopyRules: NotRequired[Sequence[CrossRegionCopyRuleTypeDef]],  # (6)
    ShareRules: NotRequired[Sequence[ShareRuleTypeDef]],  # (7)
    DeprecateRule: NotRequired[DeprecateRuleTypeDef],  # (8)
    ArchiveRule: NotRequired[ArchiveRuleTypeDef],  # (9)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRuleTypeDef](./type_defs.md#createruletypedef) 
4. See [:material-code-braces: RetainRuleTypeDef](./type_defs.md#retainruletypedef) 
5. See [:material-code-braces: FastRestoreRuleTypeDef](./type_defs.md#fastrestoreruletypedef) 
6. See [:material-code-braces: CrossRegionCopyRuleTypeDef](./type_defs.md#crossregioncopyruletypedef) 
7. See [:material-code-braces: ShareRuleTypeDef](./type_defs.md#shareruletypedef) 
8. See [:material-code-braces: DeprecateRuleTypeDef](./type_defs.md#deprecateruletypedef) 
9. See [:material-code-braces: ArchiveRuleTypeDef](./type_defs.md#archiveruletypedef) 
## PolicyDetailsTypeDef

```python
# PolicyDetailsTypeDef definition

class PolicyDetailsTypeDef(TypedDict):
    PolicyType: NotRequired[PolicyTypeValuesType],  # (1)
    ResourceTypes: NotRequired[Sequence[ResourceTypeValuesType]],  # (2)
    ResourceLocations: NotRequired[Sequence[ResourceLocationValuesType]],  # (3)
    TargetTags: NotRequired[Sequence[TagTypeDef]],  # (4)
    Schedules: NotRequired[Sequence[ScheduleTypeDef]],  # (5)
    Parameters: NotRequired[ParametersTypeDef],  # (6)
    EventSource: NotRequired[EventSourceTypeDef],  # (7)
    Actions: NotRequired[Sequence[ActionTypeDef]],  # (8)
```

1. See [:material-code-brackets: PolicyTypeValuesType](./literals.md#policytypevaluestype) 
2. See [:material-code-brackets: ResourceTypeValuesType](./literals.md#resourcetypevaluestype) 
3. See [:material-code-brackets: ResourceLocationValuesType](./literals.md#resourcelocationvaluestype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
6. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
7. See [:material-code-braces: EventSourceTypeDef](./type_defs.md#eventsourcetypedef) 
8. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
## CreateLifecyclePolicyRequestRequestTypeDef

```python
# CreateLifecyclePolicyRequestRequestTypeDef definition

class CreateLifecyclePolicyRequestRequestTypeDef(TypedDict):
    ExecutionRoleArn: str,
    Description: str,
    State: SettablePolicyStateValuesType,  # (1)
    PolicyDetails: PolicyDetailsTypeDef,  # (2)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: SettablePolicyStateValuesType](./literals.md#settablepolicystatevaluestype) 
2. See [:material-code-braces: PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef) 
## LifecyclePolicyTypeDef

```python
# LifecyclePolicyTypeDef definition

class LifecyclePolicyTypeDef(TypedDict):
    PolicyId: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[GettablePolicyStateValuesType],  # (1)
    StatusMessage: NotRequired[str],
    ExecutionRoleArn: NotRequired[str],
    DateCreated: NotRequired[datetime],
    DateModified: NotRequired[datetime],
    PolicyDetails: NotRequired[PolicyDetailsTypeDef],  # (2)
    Tags: NotRequired[Dict[str, str]],
    PolicyArn: NotRequired[str],
```

1. See [:material-code-brackets: GettablePolicyStateValuesType](./literals.md#gettablepolicystatevaluestype) 
2. See [:material-code-braces: PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef) 
## UpdateLifecyclePolicyRequestRequestTypeDef

```python
# UpdateLifecyclePolicyRequestRequestTypeDef definition

class UpdateLifecyclePolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    ExecutionRoleArn: NotRequired[str],
    State: NotRequired[SettablePolicyStateValuesType],  # (1)
    Description: NotRequired[str],
    PolicyDetails: NotRequired[PolicyDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: SettablePolicyStateValuesType](./literals.md#settablepolicystatevaluestype) 
2. See [:material-code-braces: PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef) 
## GetLifecyclePolicyResponseTypeDef

```python
# GetLifecyclePolicyResponseTypeDef definition

class GetLifecyclePolicyResponseTypeDef(TypedDict):
    Policy: LifecyclePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

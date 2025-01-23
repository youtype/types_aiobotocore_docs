# Type definitions

> [Index](../README.md) > [DLM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DLM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#dlm)
    type annotations stubs module [types-aiobotocore-dlm](https://pypi.org/project/types-aiobotocore-dlm/).

## EventParametersUnionTypeDef

```python
# EventParametersUnionTypeDef definition

EventParametersUnionTypeDef = Union[
    EventParametersTypeDef,  # (1)
    EventParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventParametersTypeDef](./type_defs.md#eventparameterstypedef) 
2. See [:material-code-braces: EventParametersOutputTypeDef](./type_defs.md#eventparametersoutputtypedef) 

## FastRestoreRuleUnionTypeDef

```python
# FastRestoreRuleUnionTypeDef definition

FastRestoreRuleUnionTypeDef = Union[
    FastRestoreRuleTypeDef,  # (1)
    FastRestoreRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FastRestoreRuleTypeDef](./type_defs.md#fastrestoreruletypedef) 
2. See [:material-code-braces: FastRestoreRuleOutputTypeDef](./type_defs.md#fastrestoreruleoutputtypedef) 

## ScriptUnionTypeDef

```python
# ScriptUnionTypeDef definition

ScriptUnionTypeDef = Union[
    ScriptTypeDef,  # (1)
    ScriptOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScriptTypeDef](./type_defs.md#scripttypedef) 
2. See [:material-code-braces: ScriptOutputTypeDef](./type_defs.md#scriptoutputtypedef) 

## ShareRuleUnionTypeDef

```python
# ShareRuleUnionTypeDef definition

ShareRuleUnionTypeDef = Union[
    ShareRuleTypeDef,  # (1)
    ShareRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ShareRuleTypeDef](./type_defs.md#shareruletypedef) 
2. See [:material-code-braces: ShareRuleOutputTypeDef](./type_defs.md#shareruleoutputtypedef) 

## ExclusionsUnionTypeDef

```python
# ExclusionsUnionTypeDef definition

ExclusionsUnionTypeDef = Union[
    ExclusionsTypeDef,  # (1)
    ExclusionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ExclusionsTypeDef](./type_defs.md#exclusionstypedef) 
2. See [:material-code-braces: ExclusionsOutputTypeDef](./type_defs.md#exclusionsoutputtypedef) 

## ParametersUnionTypeDef

```python
# ParametersUnionTypeDef definition

ParametersUnionTypeDef = Union[
    ParametersTypeDef,  # (1)
    ParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) 
2. See [:material-code-braces: ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef) 

## ActionUnionTypeDef

```python
# ActionUnionTypeDef definition

ActionUnionTypeDef = Union[
    ActionTypeDef,  # (1)
    ActionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) 
2. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 

## EventSourceUnionTypeDef

```python
# EventSourceUnionTypeDef definition

EventSourceUnionTypeDef = Union[
    EventSourceTypeDef,  # (1)
    EventSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventSourceTypeDef](./type_defs.md#eventsourcetypedef) 
2. See [:material-code-braces: EventSourceOutputTypeDef](./type_defs.md#eventsourceoutputtypedef) 

## CreateRuleUnionTypeDef

```python
# CreateRuleUnionTypeDef definition

CreateRuleUnionTypeDef = Union[
    CreateRuleTypeDef,  # (1)
    CreateRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CreateRuleTypeDef](./type_defs.md#createruletypedef) 
2. See [:material-code-braces: CreateRuleOutputTypeDef](./type_defs.md#createruleoutputtypedef) 

## ScheduleUnionTypeDef

```python
# ScheduleUnionTypeDef definition

ScheduleUnionTypeDef = Union[
    ScheduleTypeDef,  # (1)
    ScheduleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) 
2. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 



## RetentionArchiveTierTypeDef

```python
# RetentionArchiveTierTypeDef definition

class RetentionArchiveTierTypeDef(TypedDict):
    Count: NotRequired[int],
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## CrossRegionCopyTargetTypeDef

```python
# CrossRegionCopyTargetTypeDef definition

class CrossRegionCopyTargetTypeDef(TypedDict):
    TargetRegion: NotRequired[str],
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

## ScriptOutputTypeDef

```python
# ScriptOutputTypeDef definition

class ScriptOutputTypeDef(TypedDict):
    ExecutionHandler: str,
    Stages: NotRequired[List[StageValuesType]],  # (1)
    ExecutionHandlerService: NotRequired[ExecutionHandlerServiceValuesType],  # (2)
    ExecuteOperationOnScriptFailure: NotRequired[bool],
    ExecutionTimeout: NotRequired[int],
    MaximumRetryCount: NotRequired[int],
```

1. See [:material-code-brackets: StageValuesType](./literals.md#stagevaluestype) 
2. See [:material-code-brackets: ExecutionHandlerServiceValuesType](./literals.md#executionhandlerservicevaluestype) 
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
## EventParametersOutputTypeDef

```python
# EventParametersOutputTypeDef definition

class EventParametersOutputTypeDef(TypedDict):
    EventType: EventTypeValuesType,  # (1)
    SnapshotOwner: List[str],
    DescriptionRegex: str,
```

1. See [:material-code-brackets: EventTypeValuesType](./literals.md#eventtypevaluestype) 
## EventParametersTypeDef

```python
# EventParametersTypeDef definition

class EventParametersTypeDef(TypedDict):
    EventType: EventTypeValuesType,  # (1)
    SnapshotOwner: Sequence[str],
    DescriptionRegex: str,
```

1. See [:material-code-brackets: EventTypeValuesType](./literals.md#eventtypevaluestype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## FastRestoreRuleOutputTypeDef

```python
# FastRestoreRuleOutputTypeDef definition

class FastRestoreRuleOutputTypeDef(TypedDict):
    AvailabilityZones: List[str],
    Count: NotRequired[int],
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
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
    DefaultPolicyType: NotRequired[DefaultPoliciesTypeValuesType],  # (3)
```

1. See [:material-code-brackets: GettablePolicyStateValuesType](./literals.md#gettablepolicystatevaluestype) 
2. See [:material-code-brackets: ResourceTypeValuesType](./literals.md#resourcetypevaluestype) 
3. See [:material-code-brackets: DefaultPoliciesTypeValuesType](./literals.md#defaultpoliciestypevaluestype) 
## LifecyclePolicySummaryTypeDef

```python
# LifecyclePolicySummaryTypeDef definition

class LifecyclePolicySummaryTypeDef(TypedDict):
    PolicyId: NotRequired[str],
    Description: NotRequired[str],
    State: NotRequired[GettablePolicyStateValuesType],  # (1)
    Tags: NotRequired[Dict[str, str]],
    PolicyType: NotRequired[PolicyTypeValuesType],  # (2)
    DefaultPolicy: NotRequired[bool],
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

## RetainRuleTypeDef

```python
# RetainRuleTypeDef definition

class RetainRuleTypeDef(TypedDict):
    Count: NotRequired[int],
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## ShareRuleOutputTypeDef

```python
# ShareRuleOutputTypeDef definition

class ShareRuleOutputTypeDef(TypedDict):
    TargetAccounts: List[str],
    UnshareInterval: NotRequired[int],
    UnshareIntervalUnit: NotRequired[RetentionIntervalUnitValuesType],  # (1)
```

1. See [:material-code-brackets: RetentionIntervalUnitValuesType](./literals.md#retentionintervalunitvaluestype) 
## ScriptTypeDef

```python
# ScriptTypeDef definition

class ScriptTypeDef(TypedDict):
    ExecutionHandler: str,
    Stages: NotRequired[Sequence[StageValuesType]],  # (1)
    ExecutionHandlerService: NotRequired[ExecutionHandlerServiceValuesType],  # (2)
    ExecuteOperationOnScriptFailure: NotRequired[bool],
    ExecutionTimeout: NotRequired[int],
    MaximumRetryCount: NotRequired[int],
```

1. See [:material-code-brackets: StageValuesType](./literals.md#stagevaluestype) 
2. See [:material-code-brackets: ExecutionHandlerServiceValuesType](./literals.md#executionhandlerservicevaluestype) 
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
## CreateRuleOutputTypeDef

```python
# CreateRuleOutputTypeDef definition

class CreateRuleOutputTypeDef(TypedDict):
    Location: NotRequired[LocationValuesType],  # (1)
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[IntervalUnitValuesType],  # (2)
    Times: NotRequired[List[str]],
    CronExpression: NotRequired[str],
    Scripts: NotRequired[List[ScriptOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: LocationValuesType](./literals.md#locationvaluestype) 
2. See [:material-code-brackets: IntervalUnitValuesType](./literals.md#intervalunitvaluestype) 
3. See [:material-code-braces: ScriptOutputTypeDef](./type_defs.md#scriptoutputtypedef) 
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
## EventSourceOutputTypeDef

```python
# EventSourceOutputTypeDef definition

class EventSourceOutputTypeDef(TypedDict):
    Type: EventSourceValuesType,  # (1)
    Parameters: NotRequired[EventParametersOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: EventSourceValuesType](./literals.md#eventsourcevaluestype) 
2. See [:material-code-braces: EventParametersOutputTypeDef](./type_defs.md#eventparametersoutputtypedef) 
## ExclusionsOutputTypeDef

```python
# ExclusionsOutputTypeDef definition

class ExclusionsOutputTypeDef(TypedDict):
    ExcludeBootVolumes: NotRequired[bool],
    ExcludeVolumeTypes: NotRequired[List[str]],
    ExcludeTags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ExclusionsTypeDef

```python
# ExclusionsTypeDef definition

class ExclusionsTypeDef(TypedDict):
    ExcludeBootVolumes: NotRequired[bool],
    ExcludeVolumeTypes: NotRequired[Sequence[str]],
    ExcludeTags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ParametersOutputTypeDef

```python
# ParametersOutputTypeDef definition

class ParametersOutputTypeDef(TypedDict):
    ExcludeBootVolume: NotRequired[bool],
    NoReboot: NotRequired[bool],
    ExcludeDataVolumeTags: NotRequired[List[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ParametersTypeDef

```python
# ParametersTypeDef definition

class ParametersTypeDef(TypedDict):
    ExcludeBootVolume: NotRequired[bool],
    NoReboot: NotRequired[bool],
    ExcludeDataVolumeTags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetLifecyclePoliciesResponseTypeDef

```python
# GetLifecyclePoliciesResponseTypeDef definition

class GetLifecyclePoliciesResponseTypeDef(TypedDict):
    Policies: List[LifecyclePolicySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecyclePolicySummaryTypeDef](./type_defs.md#lifecyclepolicysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ArchiveRuleTypeDef

```python
# ArchiveRuleTypeDef definition

class ArchiveRuleTypeDef(TypedDict):
    RetainRule: ArchiveRetainRuleTypeDef,  # (1)
```

1. See [:material-code-braces: ArchiveRetainRuleTypeDef](./type_defs.md#archiveretainruletypedef) 
## ActionOutputTypeDef

```python
# ActionOutputTypeDef definition

class ActionOutputTypeDef(TypedDict):
    Name: str,
    CrossRegionCopy: List[CrossRegionCopyActionTypeDef],  # (1)
```

1. See [:material-code-braces: CrossRegionCopyActionTypeDef](./type_defs.md#crossregioncopyactiontypedef) 
## ActionTypeDef

```python
# ActionTypeDef definition

class ActionTypeDef(TypedDict):
    Name: str,
    CrossRegionCopy: Sequence[CrossRegionCopyActionTypeDef],  # (1)
```

1. See [:material-code-braces: CrossRegionCopyActionTypeDef](./type_defs.md#crossregioncopyactiontypedef) 
## EventSourceTypeDef

```python
# EventSourceTypeDef definition

class EventSourceTypeDef(TypedDict):
    Type: EventSourceValuesType,  # (1)
    Parameters: NotRequired[EventParametersUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: EventSourceValuesType](./literals.md#eventsourcevaluestype) 
2. See [:material-code-braces: EventParametersTypeDef](./type_defs.md#eventparameterstypedef) [:material-code-braces: EventParametersOutputTypeDef](./type_defs.md#eventparametersoutputtypedef) 
## CreateRuleTypeDef

```python
# CreateRuleTypeDef definition

class CreateRuleTypeDef(TypedDict):
    Location: NotRequired[LocationValuesType],  # (1)
    Interval: NotRequired[int],
    IntervalUnit: NotRequired[IntervalUnitValuesType],  # (2)
    Times: NotRequired[Sequence[str]],
    CronExpression: NotRequired[str],
    Scripts: NotRequired[Sequence[ScriptUnionTypeDef]],  # (3)
```

1. See [:material-code-brackets: LocationValuesType](./literals.md#locationvaluestype) 
2. See [:material-code-brackets: IntervalUnitValuesType](./literals.md#intervalunitvaluestype) 
3. See [:material-code-braces: ScriptTypeDef](./type_defs.md#scripttypedef) [:material-code-braces: ScriptOutputTypeDef](./type_defs.md#scriptoutputtypedef) 
## ScheduleOutputTypeDef

```python
# ScheduleOutputTypeDef definition

class ScheduleOutputTypeDef(TypedDict):
    Name: NotRequired[str],
    CopyTags: NotRequired[bool],
    TagsToAdd: NotRequired[List[TagTypeDef]],  # (1)
    VariableTags: NotRequired[List[TagTypeDef]],  # (1)
    CreateRule: NotRequired[CreateRuleOutputTypeDef],  # (3)
    RetainRule: NotRequired[RetainRuleTypeDef],  # (4)
    FastRestoreRule: NotRequired[FastRestoreRuleOutputTypeDef],  # (5)
    CrossRegionCopyRules: NotRequired[List[CrossRegionCopyRuleTypeDef]],  # (6)
    ShareRules: NotRequired[List[ShareRuleOutputTypeDef]],  # (7)
    DeprecateRule: NotRequired[DeprecateRuleTypeDef],  # (8)
    ArchiveRule: NotRequired[ArchiveRuleTypeDef],  # (9)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRuleOutputTypeDef](./type_defs.md#createruleoutputtypedef) 
4. See [:material-code-braces: RetainRuleTypeDef](./type_defs.md#retainruletypedef) 
5. See [:material-code-braces: FastRestoreRuleOutputTypeDef](./type_defs.md#fastrestoreruleoutputtypedef) 
6. See [:material-code-braces: CrossRegionCopyRuleTypeDef](./type_defs.md#crossregioncopyruletypedef) 
7. See [:material-code-braces: ShareRuleOutputTypeDef](./type_defs.md#shareruleoutputtypedef) 
8. See [:material-code-braces: DeprecateRuleTypeDef](./type_defs.md#deprecateruletypedef) 
9. See [:material-code-braces: ArchiveRuleTypeDef](./type_defs.md#archiveruletypedef) 
## PolicyDetailsOutputTypeDef

```python
# PolicyDetailsOutputTypeDef definition

class PolicyDetailsOutputTypeDef(TypedDict):
    PolicyType: NotRequired[PolicyTypeValuesType],  # (1)
    ResourceTypes: NotRequired[List[ResourceTypeValuesType]],  # (2)
    ResourceLocations: NotRequired[List[ResourceLocationValuesType]],  # (3)
    TargetTags: NotRequired[List[TagTypeDef]],  # (4)
    Schedules: NotRequired[List[ScheduleOutputTypeDef]],  # (5)
    Parameters: NotRequired[ParametersOutputTypeDef],  # (6)
    EventSource: NotRequired[EventSourceOutputTypeDef],  # (7)
    Actions: NotRequired[List[ActionOutputTypeDef]],  # (8)
    PolicyLanguage: NotRequired[PolicyLanguageValuesType],  # (9)
    ResourceType: NotRequired[ResourceTypeValuesType],  # (10)
    CreateInterval: NotRequired[int],
    RetainInterval: NotRequired[int],
    CopyTags: NotRequired[bool],
    CrossRegionCopyTargets: NotRequired[List[CrossRegionCopyTargetTypeDef]],  # (11)
    ExtendDeletion: NotRequired[bool],
    Exclusions: NotRequired[ExclusionsOutputTypeDef],  # (12)
```

1. See [:material-code-brackets: PolicyTypeValuesType](./literals.md#policytypevaluestype) 
2. See [:material-code-brackets: ResourceTypeValuesType](./literals.md#resourcetypevaluestype) 
3. See [:material-code-brackets: ResourceLocationValuesType](./literals.md#resourcelocationvaluestype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
6. See [:material-code-braces: ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef) 
7. See [:material-code-braces: EventSourceOutputTypeDef](./type_defs.md#eventsourceoutputtypedef) 
8. See [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
9. See [:material-code-brackets: PolicyLanguageValuesType](./literals.md#policylanguagevaluestype) 
10. See [:material-code-brackets: ResourceTypeValuesType](./literals.md#resourcetypevaluestype) 
11. See [:material-code-braces: CrossRegionCopyTargetTypeDef](./type_defs.md#crossregioncopytargettypedef) 
12. See [:material-code-braces: ExclusionsOutputTypeDef](./type_defs.md#exclusionsoutputtypedef) 
## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    Name: NotRequired[str],
    CopyTags: NotRequired[bool],
    TagsToAdd: NotRequired[Sequence[TagTypeDef]],  # (1)
    VariableTags: NotRequired[Sequence[TagTypeDef]],  # (1)
    CreateRule: NotRequired[CreateRuleUnionTypeDef],  # (3)
    RetainRule: NotRequired[RetainRuleTypeDef],  # (4)
    FastRestoreRule: NotRequired[FastRestoreRuleUnionTypeDef],  # (5)
    CrossRegionCopyRules: NotRequired[Sequence[CrossRegionCopyRuleTypeDef]],  # (6)
    ShareRules: NotRequired[Sequence[ShareRuleUnionTypeDef]],  # (7)
    DeprecateRule: NotRequired[DeprecateRuleTypeDef],  # (8)
    ArchiveRule: NotRequired[ArchiveRuleTypeDef],  # (9)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateRuleTypeDef](./type_defs.md#createruletypedef) [:material-code-braces: CreateRuleOutputTypeDef](./type_defs.md#createruleoutputtypedef) 
4. See [:material-code-braces: RetainRuleTypeDef](./type_defs.md#retainruletypedef) 
5. See [:material-code-braces: FastRestoreRuleTypeDef](./type_defs.md#fastrestoreruletypedef) [:material-code-braces: FastRestoreRuleOutputTypeDef](./type_defs.md#fastrestoreruleoutputtypedef) 
6. See [:material-code-braces: CrossRegionCopyRuleTypeDef](./type_defs.md#crossregioncopyruletypedef) 
7. See [:material-code-braces: ShareRuleTypeDef](./type_defs.md#shareruletypedef) [:material-code-braces: ShareRuleOutputTypeDef](./type_defs.md#shareruleoutputtypedef) 
8. See [:material-code-braces: DeprecateRuleTypeDef](./type_defs.md#deprecateruletypedef) 
9. See [:material-code-braces: ArchiveRuleTypeDef](./type_defs.md#archiveruletypedef) 
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
    PolicyDetails: NotRequired[PolicyDetailsOutputTypeDef],  # (2)
    Tags: NotRequired[Dict[str, str]],
    PolicyArn: NotRequired[str],
    DefaultPolicy: NotRequired[bool],
```

1. See [:material-code-brackets: GettablePolicyStateValuesType](./literals.md#gettablepolicystatevaluestype) 
2. See [:material-code-braces: PolicyDetailsOutputTypeDef](./type_defs.md#policydetailsoutputtypedef) 
## GetLifecyclePolicyResponseTypeDef

```python
# GetLifecyclePolicyResponseTypeDef definition

class GetLifecyclePolicyResponseTypeDef(TypedDict):
    Policy: LifecyclePolicyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LifecyclePolicyTypeDef](./type_defs.md#lifecyclepolicytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyDetailsTypeDef

```python
# PolicyDetailsTypeDef definition

class PolicyDetailsTypeDef(TypedDict):
    PolicyType: NotRequired[PolicyTypeValuesType],  # (1)
    ResourceTypes: NotRequired[Sequence[ResourceTypeValuesType]],  # (2)
    ResourceLocations: NotRequired[Sequence[ResourceLocationValuesType]],  # (3)
    TargetTags: NotRequired[Sequence[TagTypeDef]],  # (4)
    Schedules: NotRequired[Sequence[ScheduleUnionTypeDef]],  # (5)
    Parameters: NotRequired[ParametersUnionTypeDef],  # (6)
    EventSource: NotRequired[EventSourceUnionTypeDef],  # (7)
    Actions: NotRequired[Sequence[ActionUnionTypeDef]],  # (8)
    PolicyLanguage: NotRequired[PolicyLanguageValuesType],  # (9)
    ResourceType: NotRequired[ResourceTypeValuesType],  # (10)
    CreateInterval: NotRequired[int],
    RetainInterval: NotRequired[int],
    CopyTags: NotRequired[bool],
    CrossRegionCopyTargets: NotRequired[Sequence[CrossRegionCopyTargetTypeDef]],  # (11)
    ExtendDeletion: NotRequired[bool],
    Exclusions: NotRequired[ExclusionsUnionTypeDef],  # (12)
```

1. See [:material-code-brackets: PolicyTypeValuesType](./literals.md#policytypevaluestype) 
2. See [:material-code-brackets: ResourceTypeValuesType](./literals.md#resourcetypevaluestype) 
3. See [:material-code-brackets: ResourceLocationValuesType](./literals.md#resourcelocationvaluestype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
6. See [:material-code-braces: ParametersTypeDef](./type_defs.md#parameterstypedef) [:material-code-braces: ParametersOutputTypeDef](./type_defs.md#parametersoutputtypedef) 
7. See [:material-code-braces: EventSourceTypeDef](./type_defs.md#eventsourcetypedef) [:material-code-braces: EventSourceOutputTypeDef](./type_defs.md#eventsourceoutputtypedef) 
8. See [:material-code-braces: ActionTypeDef](./type_defs.md#actiontypedef) [:material-code-braces: ActionOutputTypeDef](./type_defs.md#actionoutputtypedef) 
9. See [:material-code-brackets: PolicyLanguageValuesType](./literals.md#policylanguagevaluestype) 
10. See [:material-code-brackets: ResourceTypeValuesType](./literals.md#resourcetypevaluestype) 
11. See [:material-code-braces: CrossRegionCopyTargetTypeDef](./type_defs.md#crossregioncopytargettypedef) 
12. See [:material-code-braces: ExclusionsTypeDef](./type_defs.md#exclusionstypedef) [:material-code-braces: ExclusionsOutputTypeDef](./type_defs.md#exclusionsoutputtypedef) 
## CreateLifecyclePolicyRequestRequestTypeDef

```python
# CreateLifecyclePolicyRequestRequestTypeDef definition

class CreateLifecyclePolicyRequestRequestTypeDef(TypedDict):
    ExecutionRoleArn: str,
    Description: str,
    State: SettablePolicyStateValuesType,  # (1)
    PolicyDetails: NotRequired[PolicyDetailsTypeDef],  # (2)
    Tags: NotRequired[Mapping[str, str]],
    DefaultPolicy: NotRequired[DefaultPolicyTypeValuesType],  # (3)
    CreateInterval: NotRequired[int],
    RetainInterval: NotRequired[int],
    CopyTags: NotRequired[bool],
    ExtendDeletion: NotRequired[bool],
    CrossRegionCopyTargets: NotRequired[Sequence[CrossRegionCopyTargetTypeDef]],  # (4)
    Exclusions: NotRequired[ExclusionsTypeDef],  # (5)
```

1. See [:material-code-brackets: SettablePolicyStateValuesType](./literals.md#settablepolicystatevaluestype) 
2. See [:material-code-braces: PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef) 
3. See [:material-code-brackets: DefaultPolicyTypeValuesType](./literals.md#defaultpolicytypevaluestype) 
4. See [:material-code-braces: CrossRegionCopyTargetTypeDef](./type_defs.md#crossregioncopytargettypedef) 
5. See [:material-code-braces: ExclusionsTypeDef](./type_defs.md#exclusionstypedef) 
## UpdateLifecyclePolicyRequestRequestTypeDef

```python
# UpdateLifecyclePolicyRequestRequestTypeDef definition

class UpdateLifecyclePolicyRequestRequestTypeDef(TypedDict):
    PolicyId: str,
    ExecutionRoleArn: NotRequired[str],
    State: NotRequired[SettablePolicyStateValuesType],  # (1)
    Description: NotRequired[str],
    PolicyDetails: NotRequired[PolicyDetailsTypeDef],  # (2)
    CreateInterval: NotRequired[int],
    RetainInterval: NotRequired[int],
    CopyTags: NotRequired[bool],
    ExtendDeletion: NotRequired[bool],
    CrossRegionCopyTargets: NotRequired[Sequence[CrossRegionCopyTargetTypeDef]],  # (3)
    Exclusions: NotRequired[ExclusionsTypeDef],  # (4)
```

1. See [:material-code-brackets: SettablePolicyStateValuesType](./literals.md#settablepolicystatevaluestype) 
2. See [:material-code-braces: PolicyDetailsTypeDef](./type_defs.md#policydetailstypedef) 
3. See [:material-code-braces: CrossRegionCopyTargetTypeDef](./type_defs.md#crossregioncopytargettypedef) 
4. See [:material-code-braces: ExclusionsTypeDef](./type_defs.md#exclusionstypedef) 

# Type definitions

> [Index](../README.md) > [Pinpoint](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Pinpoint](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint.html#Pinpoint)
    type annotations stubs module [types-aiobotocore-pinpoint](https://pypi.org/project/types-aiobotocore-pinpoint/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AttributeDimensionUnionTypeDef

```python
# AttributeDimensionUnionTypeDef definition

AttributeDimensionUnionTypeDef = Union[
    AttributeDimensionTypeDef,  # (1)
    AttributeDimensionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AttributeDimensionTypeDef](./type_defs.md#attributedimensiontypedef) 
2. See [:material-code-braces: AttributeDimensionOutputTypeDef](./type_defs.md#attributedimensionoutputtypedef) 

## CustomDeliveryConfigurationUnionTypeDef

```python
# CustomDeliveryConfigurationUnionTypeDef definition

CustomDeliveryConfigurationUnionTypeDef = Union[
    CustomDeliveryConfigurationTypeDef,  # (1)
    CustomDeliveryConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomDeliveryConfigurationTypeDef](./type_defs.md#customdeliveryconfigurationtypedef) 
2. See [:material-code-braces: CustomDeliveryConfigurationOutputTypeDef](./type_defs.md#customdeliveryconfigurationoutputtypedef) 

## EndpointUserUnionTypeDef

```python
# EndpointUserUnionTypeDef definition

EndpointUserUnionTypeDef = Union[
    EndpointUserTypeDef,  # (1)
    EndpointUserOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EndpointUserTypeDef](./type_defs.md#endpointusertypedef) 
2. See [:material-code-braces: EndpointUserOutputTypeDef](./type_defs.md#endpointuseroutputtypedef) 

## SetDimensionUnionTypeDef

```python
# SetDimensionUnionTypeDef definition

SetDimensionUnionTypeDef = Union[
    SetDimensionTypeDef,  # (1)
    SetDimensionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) 
2. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 

## CampaignEmailMessageUnionTypeDef

```python
# CampaignEmailMessageUnionTypeDef definition

CampaignEmailMessageUnionTypeDef = Union[
    CampaignEmailMessageTypeDef,  # (1)
    CampaignEmailMessageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CampaignEmailMessageTypeDef](./type_defs.md#campaignemailmessagetypedef) 
2. See [:material-code-braces: CampaignEmailMessageOutputTypeDef](./type_defs.md#campaignemailmessageoutputtypedef) 

## ClosedDaysUnionTypeDef

```python
# ClosedDaysUnionTypeDef definition

ClosedDaysUnionTypeDef = Union[
    ClosedDaysTypeDef,  # (1)
    ClosedDaysOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ClosedDaysTypeDef](./type_defs.md#closeddaystypedef) 
2. See [:material-code-braces: ClosedDaysOutputTypeDef](./type_defs.md#closeddaysoutputtypedef) 

## CustomMessageActivityUnionTypeDef

```python
# CustomMessageActivityUnionTypeDef definition

CustomMessageActivityUnionTypeDef = Union[
    CustomMessageActivityTypeDef,  # (1)
    CustomMessageActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomMessageActivityTypeDef](./type_defs.md#custommessageactivitytypedef) 
2. See [:material-code-braces: CustomMessageActivityOutputTypeDef](./type_defs.md#custommessageactivityoutputtypedef) 

## JourneyScheduleUnionTypeDef

```python
# JourneyScheduleUnionTypeDef definition

JourneyScheduleUnionTypeDef = Union[
    JourneyScheduleTypeDef,  # (1)
    JourneyScheduleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JourneyScheduleTypeDef](./type_defs.md#journeyscheduletypedef) 
2. See [:material-code-braces: JourneyScheduleOutputTypeDef](./type_defs.md#journeyscheduleoutputtypedef) 

## OpenHoursUnionTypeDef

```python
# OpenHoursUnionTypeDef definition

OpenHoursUnionTypeDef = Union[
    OpenHoursTypeDef,  # (1)
    OpenHoursOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OpenHoursTypeDef](./type_defs.md#openhourstypedef) 
2. See [:material-code-braces: OpenHoursOutputTypeDef](./type_defs.md#openhoursoutputtypedef) 

## RandomSplitActivityUnionTypeDef

```python
# RandomSplitActivityUnionTypeDef definition

RandomSplitActivityUnionTypeDef = Union[
    RandomSplitActivityTypeDef,  # (1)
    RandomSplitActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RandomSplitActivityTypeDef](./type_defs.md#randomsplitactivitytypedef) 
2. See [:material-code-braces: RandomSplitActivityOutputTypeDef](./type_defs.md#randomsplitactivityoutputtypedef) 

## EventDimensionsUnionTypeDef

```python
# EventDimensionsUnionTypeDef definition

EventDimensionsUnionTypeDef = Union[
    EventDimensionsTypeDef,  # (1)
    EventDimensionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventDimensionsTypeDef](./type_defs.md#eventdimensionstypedef) 
2. See [:material-code-braces: EventDimensionsOutputTypeDef](./type_defs.md#eventdimensionsoutputtypedef) 

## SegmentDemographicsUnionTypeDef

```python
# SegmentDemographicsUnionTypeDef definition

SegmentDemographicsUnionTypeDef = Union[
    SegmentDemographicsTypeDef,  # (1)
    SegmentDemographicsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SegmentDemographicsTypeDef](./type_defs.md#segmentdemographicstypedef) 
2. See [:material-code-braces: SegmentDemographicsOutputTypeDef](./type_defs.md#segmentdemographicsoutputtypedef) 

## SegmentLocationUnionTypeDef

```python
# SegmentLocationUnionTypeDef definition

SegmentLocationUnionTypeDef = Union[
    SegmentLocationTypeDef,  # (1)
    SegmentLocationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SegmentLocationTypeDef](./type_defs.md#segmentlocationtypedef) 
2. See [:material-code-braces: SegmentLocationOutputTypeDef](./type_defs.md#segmentlocationoutputtypedef) 

## CampaignInAppMessageUnionTypeDef

```python
# CampaignInAppMessageUnionTypeDef definition

CampaignInAppMessageUnionTypeDef = Union[
    CampaignInAppMessageTypeDef,  # (1)
    CampaignInAppMessageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CampaignInAppMessageTypeDef](./type_defs.md#campaigninappmessagetypedef) 
2. See [:material-code-braces: CampaignInAppMessageOutputTypeDef](./type_defs.md#campaigninappmessageoutputtypedef) 

## CampaignEventFilterUnionTypeDef

```python
# CampaignEventFilterUnionTypeDef definition

CampaignEventFilterUnionTypeDef = Union[
    CampaignEventFilterTypeDef,  # (1)
    CampaignEventFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CampaignEventFilterTypeDef](./type_defs.md#campaigneventfiltertypedef) 
2. See [:material-code-braces: CampaignEventFilterOutputTypeDef](./type_defs.md#campaigneventfilteroutputtypedef) 

## EventConditionUnionTypeDef

```python
# EventConditionUnionTypeDef definition

EventConditionUnionTypeDef = Union[
    EventConditionTypeDef,  # (1)
    EventConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventConditionTypeDef](./type_defs.md#eventconditiontypedef) 
2. See [:material-code-braces: EventConditionOutputTypeDef](./type_defs.md#eventconditionoutputtypedef) 

## EventFilterUnionTypeDef

```python
# EventFilterUnionTypeDef definition

EventFilterUnionTypeDef = Union[
    EventFilterTypeDef,  # (1)
    EventFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) 
2. See [:material-code-braces: EventFilterOutputTypeDef](./type_defs.md#eventfilteroutputtypedef) 

## SegmentDimensionsUnionTypeDef

```python
# SegmentDimensionsUnionTypeDef definition

SegmentDimensionsUnionTypeDef = Union[
    SegmentDimensionsTypeDef,  # (1)
    SegmentDimensionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SegmentDimensionsTypeDef](./type_defs.md#segmentdimensionstypedef) 
2. See [:material-code-braces: SegmentDimensionsOutputTypeDef](./type_defs.md#segmentdimensionsoutputtypedef) 

## MessageConfigurationUnionTypeDef

```python
# MessageConfigurationUnionTypeDef definition

MessageConfigurationUnionTypeDef = Union[
    MessageConfigurationTypeDef,  # (1)
    MessageConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageConfigurationTypeDef](./type_defs.md#messageconfigurationtypedef) 
2. See [:material-code-braces: MessageConfigurationOutputTypeDef](./type_defs.md#messageconfigurationoutputtypedef) 

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

## EventStartConditionUnionTypeDef

```python
# EventStartConditionUnionTypeDef definition

EventStartConditionUnionTypeDef = Union[
    EventStartConditionTypeDef,  # (1)
    EventStartConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventStartConditionTypeDef](./type_defs.md#eventstartconditiontypedef) 
2. See [:material-code-braces: EventStartConditionOutputTypeDef](./type_defs.md#eventstartconditionoutputtypedef) 

## SegmentGroupUnionTypeDef

```python
# SegmentGroupUnionTypeDef definition

SegmentGroupUnionTypeDef = Union[
    SegmentGroupTypeDef,  # (1)
    SegmentGroupOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SegmentGroupTypeDef](./type_defs.md#segmentgrouptypedef) 
2. See [:material-code-braces: SegmentGroupOutputTypeDef](./type_defs.md#segmentgroupoutputtypedef) 

## SimpleConditionUnionTypeDef

```python
# SimpleConditionUnionTypeDef definition

SimpleConditionUnionTypeDef = Union[
    SimpleConditionTypeDef,  # (1)
    SimpleConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SimpleConditionTypeDef](./type_defs.md#simpleconditiontypedef) 
2. See [:material-code-braces: SimpleConditionOutputTypeDef](./type_defs.md#simpleconditionoutputtypedef) 

## StartConditionUnionTypeDef

```python
# StartConditionUnionTypeDef definition

StartConditionUnionTypeDef = Union[
    StartConditionTypeDef,  # (1)
    StartConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StartConditionTypeDef](./type_defs.md#startconditiontypedef) 
2. See [:material-code-braces: StartConditionOutputTypeDef](./type_defs.md#startconditionoutputtypedef) 

## SegmentGroupListUnionTypeDef

```python
# SegmentGroupListUnionTypeDef definition

SegmentGroupListUnionTypeDef = Union[
    SegmentGroupListTypeDef,  # (1)
    SegmentGroupListOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SegmentGroupListTypeDef](./type_defs.md#segmentgrouplisttypedef) 
2. See [:material-code-braces: SegmentGroupListOutputTypeDef](./type_defs.md#segmentgrouplistoutputtypedef) 

## ConditionUnionTypeDef

```python
# ConditionUnionTypeDef definition

ConditionUnionTypeDef = Union[
    ConditionTypeDef,  # (1)
    ConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
2. See [:material-code-braces: ConditionOutputTypeDef](./type_defs.md#conditionoutputtypedef) 

## MultiConditionalBranchUnionTypeDef

```python
# MultiConditionalBranchUnionTypeDef definition

MultiConditionalBranchUnionTypeDef = Union[
    MultiConditionalBranchTypeDef,  # (1)
    MultiConditionalBranchOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MultiConditionalBranchTypeDef](./type_defs.md#multiconditionalbranchtypedef) 
2. See [:material-code-braces: MultiConditionalBranchOutputTypeDef](./type_defs.md#multiconditionalbranchoutputtypedef) 

## ConditionalSplitActivityUnionTypeDef

```python
# ConditionalSplitActivityUnionTypeDef definition

ConditionalSplitActivityUnionTypeDef = Union[
    ConditionalSplitActivityTypeDef,  # (1)
    ConditionalSplitActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConditionalSplitActivityTypeDef](./type_defs.md#conditionalsplitactivitytypedef) 
2. See [:material-code-braces: ConditionalSplitActivityOutputTypeDef](./type_defs.md#conditionalsplitactivityoutputtypedef) 

## MultiConditionalSplitActivityUnionTypeDef

```python
# MultiConditionalSplitActivityUnionTypeDef definition

MultiConditionalSplitActivityUnionTypeDef = Union[
    MultiConditionalSplitActivityTypeDef,  # (1)
    MultiConditionalSplitActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MultiConditionalSplitActivityTypeDef](./type_defs.md#multiconditionalsplitactivitytypedef) 
2. See [:material-code-braces: MultiConditionalSplitActivityOutputTypeDef](./type_defs.md#multiconditionalsplitactivityoutputtypedef) 

## ActivityUnionTypeDef

```python
# ActivityUnionTypeDef definition

ActivityUnionTypeDef = Union[
    ActivityTypeDef,  # (1)
    ActivityOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ActivityTypeDef](./type_defs.md#activitytypedef) 
2. See [:material-code-braces: ActivityOutputTypeDef](./type_defs.md#activityoutputtypedef) 



## ADMChannelRequestTypeDef

```python
# ADMChannelRequestTypeDef definition

class ADMChannelRequestTypeDef(TypedDict):
    ClientId: str,
    ClientSecret: str,
    Enabled: NotRequired[bool],
```

## ADMChannelResponseTypeDef

```python
# ADMChannelResponseTypeDef definition

class ADMChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## ADMMessageTypeDef

```python
# ADMMessageTypeDef definition

class ADMMessageTypeDef(TypedDict):
    Action: NotRequired[ActionType],  # (1)
    Body: NotRequired[str],
    ConsolidationKey: NotRequired[str],
    Data: NotRequired[Mapping[str, str]],
    ExpiresAfter: NotRequired[str],
    IconReference: NotRequired[str],
    ImageIconUrl: NotRequired[str],
    ImageUrl: NotRequired[str],
    MD5: NotRequired[str],
    RawContent: NotRequired[str],
    SilentPush: NotRequired[bool],
    SmallImageIconUrl: NotRequired[str],
    Sound: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## APNSChannelRequestTypeDef

```python
# APNSChannelRequestTypeDef definition

class APNSChannelRequestTypeDef(TypedDict):
    BundleId: NotRequired[str],
    Certificate: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    PrivateKey: NotRequired[str],
    TeamId: NotRequired[str],
    TokenKey: NotRequired[str],
    TokenKeyId: NotRequired[str],
```

## APNSChannelResponseTypeDef

```python
# APNSChannelResponseTypeDef definition

class APNSChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    HasTokenKey: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## APNSMessageTypeDef

```python
# APNSMessageTypeDef definition

class APNSMessageTypeDef(TypedDict):
    APNSPushType: NotRequired[str],
    Action: NotRequired[ActionType],  # (1)
    Badge: NotRequired[int],
    Body: NotRequired[str],
    Category: NotRequired[str],
    CollapseId: NotRequired[str],
    Data: NotRequired[Mapping[str, str]],
    MediaUrl: NotRequired[str],
    PreferredAuthenticationMethod: NotRequired[str],
    Priority: NotRequired[str],
    RawContent: NotRequired[str],
    SilentPush: NotRequired[bool],
    Sound: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    ThreadId: NotRequired[str],
    TimeToLive: NotRequired[int],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## APNSPushNotificationTemplateTypeDef

```python
# APNSPushNotificationTemplateTypeDef definition

class APNSPushNotificationTemplateTypeDef(TypedDict):
    Action: NotRequired[ActionType],  # (1)
    Body: NotRequired[str],
    MediaUrl: NotRequired[str],
    RawContent: NotRequired[str],
    Sound: NotRequired[str],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## APNSSandboxChannelRequestTypeDef

```python
# APNSSandboxChannelRequestTypeDef definition

class APNSSandboxChannelRequestTypeDef(TypedDict):
    BundleId: NotRequired[str],
    Certificate: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    PrivateKey: NotRequired[str],
    TeamId: NotRequired[str],
    TokenKey: NotRequired[str],
    TokenKeyId: NotRequired[str],
```

## APNSSandboxChannelResponseTypeDef

```python
# APNSSandboxChannelResponseTypeDef definition

class APNSSandboxChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    HasTokenKey: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## APNSVoipChannelRequestTypeDef

```python
# APNSVoipChannelRequestTypeDef definition

class APNSVoipChannelRequestTypeDef(TypedDict):
    BundleId: NotRequired[str],
    Certificate: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    PrivateKey: NotRequired[str],
    TeamId: NotRequired[str],
    TokenKey: NotRequired[str],
    TokenKeyId: NotRequired[str],
```

## APNSVoipChannelResponseTypeDef

```python
# APNSVoipChannelResponseTypeDef definition

class APNSVoipChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    HasTokenKey: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## APNSVoipSandboxChannelRequestTypeDef

```python
# APNSVoipSandboxChannelRequestTypeDef definition

class APNSVoipSandboxChannelRequestTypeDef(TypedDict):
    BundleId: NotRequired[str],
    Certificate: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    PrivateKey: NotRequired[str],
    TeamId: NotRequired[str],
    TokenKey: NotRequired[str],
    TokenKeyId: NotRequired[str],
```

## APNSVoipSandboxChannelResponseTypeDef

```python
# APNSVoipSandboxChannelResponseTypeDef definition

class APNSVoipSandboxChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    HasTokenKey: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## ActivityResponseTypeDef

```python
# ActivityResponseTypeDef definition

class ActivityResponseTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
    Id: str,
    End: NotRequired[str],
    Result: NotRequired[str],
    ScheduledStart: NotRequired[str],
    Start: NotRequired[str],
    State: NotRequired[str],
    SuccessfulEndpointCount: NotRequired[int],
    TimezonesCompletedCount: NotRequired[int],
    TimezonesTotalCount: NotRequired[int],
    TotalEndpointCount: NotRequired[int],
    TreatmentId: NotRequired[str],
    ExecutionMetrics: NotRequired[Dict[str, str]],
```

## ContactCenterActivityTypeDef

```python
# ContactCenterActivityTypeDef definition

class ContactCenterActivityTypeDef(TypedDict):
    NextActivity: NotRequired[str],
```

## HoldoutActivityTypeDef

```python
# HoldoutActivityTypeDef definition

class HoldoutActivityTypeDef(TypedDict):
    Percentage: int,
    NextActivity: NotRequired[str],
```

## AddressConfigurationTypeDef

```python
# AddressConfigurationTypeDef definition

class AddressConfigurationTypeDef(TypedDict):
    BodyOverride: NotRequired[str],
    ChannelType: NotRequired[ChannelTypeType],  # (1)
    Context: NotRequired[Mapping[str, str]],
    RawContent: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    TitleOverride: NotRequired[str],
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
## AndroidPushNotificationTemplateTypeDef

```python
# AndroidPushNotificationTemplateTypeDef definition

class AndroidPushNotificationTemplateTypeDef(TypedDict):
    Action: NotRequired[ActionType],  # (1)
    Body: NotRequired[str],
    ImageIconUrl: NotRequired[str],
    ImageUrl: NotRequired[str],
    RawContent: NotRequired[str],
    SmallImageIconUrl: NotRequired[str],
    Sound: NotRequired[str],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## ApplicationResponseTypeDef

```python
# ApplicationResponseTypeDef definition

class ApplicationResponseTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    tags: NotRequired[Dict[str, str]],
    CreationDate: NotRequired[str],
```

## JourneyTimeframeCapTypeDef

```python
# JourneyTimeframeCapTypeDef definition

class JourneyTimeframeCapTypeDef(TypedDict):
    Cap: NotRequired[int],
    Days: NotRequired[int],
```

## CampaignHookTypeDef

```python
# CampaignHookTypeDef definition

class CampaignHookTypeDef(TypedDict):
    LambdaFunctionName: NotRequired[str],
    Mode: NotRequired[ModeType],  # (1)
    WebUrl: NotRequired[str],
```

1. See [:material-code-brackets: ModeType](./literals.md#modetype) 
## CampaignLimitsTypeDef

```python
# CampaignLimitsTypeDef definition

class CampaignLimitsTypeDef(TypedDict):
    Daily: NotRequired[int],
    MaximumDuration: NotRequired[int],
    MessagesPerSecond: NotRequired[int],
    Total: NotRequired[int],
    Session: NotRequired[int],
```

## QuietTimeTypeDef

```python
# QuietTimeTypeDef definition

class QuietTimeTypeDef(TypedDict):
    End: NotRequired[str],
    Start: NotRequired[str],
```

## AttributeDimensionOutputTypeDef

```python
# AttributeDimensionOutputTypeDef definition

class AttributeDimensionOutputTypeDef(TypedDict):
    Values: List[str],
    AttributeType: NotRequired[AttributeTypeType],  # (1)
```

1. See [:material-code-brackets: AttributeTypeType](./literals.md#attributetypetype) 
## AttributeDimensionTypeDef

```python
# AttributeDimensionTypeDef definition

class AttributeDimensionTypeDef(TypedDict):
    Values: Sequence[str],
    AttributeType: NotRequired[AttributeTypeType],  # (1)
```

1. See [:material-code-brackets: AttributeTypeType](./literals.md#attributetypetype) 
## AttributesResourceTypeDef

```python
# AttributesResourceTypeDef definition

class AttributesResourceTypeDef(TypedDict):
    ApplicationId: str,
    AttributeType: str,
    Attributes: NotRequired[List[str]],
```

## BaiduChannelRequestTypeDef

```python
# BaiduChannelRequestTypeDef definition

class BaiduChannelRequestTypeDef(TypedDict):
    ApiKey: str,
    SecretKey: str,
    Enabled: NotRequired[bool],
```

## BaiduChannelResponseTypeDef

```python
# BaiduChannelResponseTypeDef definition

class BaiduChannelResponseTypeDef(TypedDict):
    Credential: str,
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## BaiduMessageTypeDef

```python
# BaiduMessageTypeDef definition

class BaiduMessageTypeDef(TypedDict):
    Action: NotRequired[ActionType],  # (1)
    Body: NotRequired[str],
    Data: NotRequired[Mapping[str, str]],
    IconReference: NotRequired[str],
    ImageIconUrl: NotRequired[str],
    ImageUrl: NotRequired[str],
    RawContent: NotRequired[str],
    SilentPush: NotRequired[bool],
    SmallImageIconUrl: NotRequired[str],
    Sound: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    TimeToLive: NotRequired[int],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## CampaignCustomMessageTypeDef

```python
# CampaignCustomMessageTypeDef definition

class CampaignCustomMessageTypeDef(TypedDict):
    Data: NotRequired[str],
```

## MessageHeaderTypeDef

```python
# MessageHeaderTypeDef definition

class MessageHeaderTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## CampaignStateTypeDef

```python
# CampaignStateTypeDef definition

class CampaignStateTypeDef(TypedDict):
    CampaignStatus: NotRequired[CampaignStatusType],  # (1)
```

1. See [:material-code-brackets: CampaignStatusType](./literals.md#campaignstatustype) 
## CustomDeliveryConfigurationOutputTypeDef

```python
# CustomDeliveryConfigurationOutputTypeDef definition

class CustomDeliveryConfigurationOutputTypeDef(TypedDict):
    DeliveryUri: str,
    EndpointTypes: NotRequired[List[EndpointTypesElementType]],  # (1)
```

1. See [:material-code-brackets: EndpointTypesElementType](./literals.md#endpointtypeselementtype) 
## CampaignSmsMessageTypeDef

```python
# CampaignSmsMessageTypeDef definition

class CampaignSmsMessageTypeDef(TypedDict):
    Body: NotRequired[str],
    MessageType: NotRequired[MessageTypeType],  # (1)
    OriginationNumber: NotRequired[str],
    SenderId: NotRequired[str],
    EntityId: NotRequired[str],
    TemplateId: NotRequired[str],
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## ChannelResponseTypeDef

```python
# ChannelResponseTypeDef definition

class ChannelResponseTypeDef(TypedDict):
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## ClosedDaysRuleTypeDef

```python
# ClosedDaysRuleTypeDef definition

class ClosedDaysRuleTypeDef(TypedDict):
    Name: NotRequired[str],
    StartDateTime: NotRequired[str],
    EndDateTime: NotRequired[str],
```

## WaitTimeTypeDef

```python
# WaitTimeTypeDef definition

class WaitTimeTypeDef(TypedDict):
    WaitFor: NotRequired[str],
    WaitUntil: NotRequired[str],
```

## CreateApplicationRequestTypeDef

```python
# CreateApplicationRequestTypeDef definition

class CreateApplicationRequestTypeDef(TypedDict):
    Name: str,
    tags: NotRequired[Mapping[str, str]],
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

## CreateTemplateMessageBodyTypeDef

```python
# CreateTemplateMessageBodyTypeDef definition

class CreateTemplateMessageBodyTypeDef(TypedDict):
    Arn: NotRequired[str],
    Message: NotRequired[str],
    RequestID: NotRequired[str],
```

## ExportJobRequestTypeDef

```python
# ExportJobRequestTypeDef definition

class ExportJobRequestTypeDef(TypedDict):
    RoleArn: str,
    S3UrlPrefix: str,
    SegmentId: NotRequired[str],
    SegmentVersion: NotRequired[int],
```

## ImportJobRequestTypeDef

```python
# ImportJobRequestTypeDef definition

class ImportJobRequestTypeDef(TypedDict):
    Format: FormatType,  # (1)
    RoleArn: str,
    S3Url: str,
    DefineSegment: NotRequired[bool],
    ExternalId: NotRequired[str],
    RegisterEndpoints: NotRequired[bool],
    SegmentId: NotRequired[str],
    SegmentName: NotRequired[str],
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## TemplateCreateMessageBodyTypeDef

```python
# TemplateCreateMessageBodyTypeDef definition

class TemplateCreateMessageBodyTypeDef(TypedDict):
    Arn: NotRequired[str],
    Message: NotRequired[str],
    RequestID: NotRequired[str],
```

## CreateRecommenderConfigurationTypeDef

```python
# CreateRecommenderConfigurationTypeDef definition

class CreateRecommenderConfigurationTypeDef(TypedDict):
    RecommendationProviderRoleArn: str,
    RecommendationProviderUri: str,
    Attributes: NotRequired[Mapping[str, str]],
    Description: NotRequired[str],
    Name: NotRequired[str],
    RecommendationProviderIdType: NotRequired[str],
    RecommendationTransformerUri: NotRequired[str],
    RecommendationsDisplayName: NotRequired[str],
    RecommendationsPerMessage: NotRequired[int],
```

## RecommenderConfigurationResponseTypeDef

```python
# RecommenderConfigurationResponseTypeDef definition

class RecommenderConfigurationResponseTypeDef(TypedDict):
    CreationDate: str,
    Id: str,
    LastModifiedDate: str,
    RecommendationProviderRoleArn: str,
    RecommendationProviderUri: str,
    Attributes: NotRequired[Dict[str, str]],
    Description: NotRequired[str],
    Name: NotRequired[str],
    RecommendationProviderIdType: NotRequired[str],
    RecommendationTransformerUri: NotRequired[str],
    RecommendationsDisplayName: NotRequired[str],
    RecommendationsPerMessage: NotRequired[int],
```

## SMSTemplateRequestTypeDef

```python
# SMSTemplateRequestTypeDef definition

class SMSTemplateRequestTypeDef(TypedDict):
    Body: NotRequired[str],
    DefaultSubstitutions: NotRequired[str],
    RecommenderId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    TemplateDescription: NotRequired[str],
```

## VoiceTemplateRequestTypeDef

```python
# VoiceTemplateRequestTypeDef definition

class VoiceTemplateRequestTypeDef(TypedDict):
    Body: NotRequired[str],
    DefaultSubstitutions: NotRequired[str],
    LanguageCode: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    TemplateDescription: NotRequired[str],
    VoiceId: NotRequired[str],
```

## CustomDeliveryConfigurationTypeDef

```python
# CustomDeliveryConfigurationTypeDef definition

class CustomDeliveryConfigurationTypeDef(TypedDict):
    DeliveryUri: str,
    EndpointTypes: NotRequired[Sequence[EndpointTypesElementType]],  # (1)
```

1. See [:material-code-brackets: EndpointTypesElementType](./literals.md#endpointtypeselementtype) 
## JourneyCustomMessageTypeDef

```python
# JourneyCustomMessageTypeDef definition

class JourneyCustomMessageTypeDef(TypedDict):
    Data: NotRequired[str],
```

## DefaultButtonConfigurationTypeDef

```python
# DefaultButtonConfigurationTypeDef definition

class DefaultButtonConfigurationTypeDef(TypedDict):
    ButtonAction: ButtonActionType,  # (1)
    Text: str,
    BackgroundColor: NotRequired[str],
    BorderRadius: NotRequired[int],
    Link: NotRequired[str],
    TextColor: NotRequired[str],
```

1. See [:material-code-brackets: ButtonActionType](./literals.md#buttonactiontype) 
## DefaultMessageTypeDef

```python
# DefaultMessageTypeDef definition

class DefaultMessageTypeDef(TypedDict):
    Body: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
```

## DefaultPushNotificationMessageTypeDef

```python
# DefaultPushNotificationMessageTypeDef definition

class DefaultPushNotificationMessageTypeDef(TypedDict):
    Action: NotRequired[ActionType],  # (1)
    Body: NotRequired[str],
    Data: NotRequired[Mapping[str, str]],
    SilentPush: NotRequired[bool],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## DefaultPushNotificationTemplateTypeDef

```python
# DefaultPushNotificationTemplateTypeDef definition

class DefaultPushNotificationTemplateTypeDef(TypedDict):
    Action: NotRequired[ActionType],  # (1)
    Body: NotRequired[str],
    Sound: NotRequired[str],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## DeleteAdmChannelRequestRequestTypeDef

```python
# DeleteAdmChannelRequestRequestTypeDef definition

class DeleteAdmChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteApnsChannelRequestRequestTypeDef

```python
# DeleteApnsChannelRequestRequestTypeDef definition

class DeleteApnsChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteApnsSandboxChannelRequestRequestTypeDef

```python
# DeleteApnsSandboxChannelRequestRequestTypeDef definition

class DeleteApnsSandboxChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteApnsVoipChannelRequestRequestTypeDef

```python
# DeleteApnsVoipChannelRequestRequestTypeDef definition

class DeleteApnsVoipChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteApnsVoipSandboxChannelRequestRequestTypeDef

```python
# DeleteApnsVoipSandboxChannelRequestRequestTypeDef definition

class DeleteApnsVoipSandboxChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteAppRequestRequestTypeDef

```python
# DeleteAppRequestRequestTypeDef definition

class DeleteAppRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteBaiduChannelRequestRequestTypeDef

```python
# DeleteBaiduChannelRequestRequestTypeDef definition

class DeleteBaiduChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## DeleteCampaignRequestRequestTypeDef

```python
# DeleteCampaignRequestRequestTypeDef definition

class DeleteCampaignRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
```

## DeleteEmailChannelRequestRequestTypeDef

```python
# DeleteEmailChannelRequestRequestTypeDef definition

class DeleteEmailChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## EmailChannelResponseTypeDef

```python
# EmailChannelResponseTypeDef definition

class EmailChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    ConfigurationSet: NotRequired[str],
    CreationDate: NotRequired[str],
    Enabled: NotRequired[bool],
    FromAddress: NotRequired[str],
    HasCredential: NotRequired[bool],
    Id: NotRequired[str],
    Identity: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    MessagesPerSecond: NotRequired[int],
    RoleArn: NotRequired[str],
    OrchestrationSendingRoleArn: NotRequired[str],
    Version: NotRequired[int],
```

## DeleteEmailTemplateRequestRequestTypeDef

```python
# DeleteEmailTemplateRequestRequestTypeDef definition

class DeleteEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## MessageBodyTypeDef

```python
# MessageBodyTypeDef definition

class MessageBodyTypeDef(TypedDict):
    Message: NotRequired[str],
    RequestID: NotRequired[str],
```

## DeleteEndpointRequestRequestTypeDef

```python
# DeleteEndpointRequestRequestTypeDef definition

class DeleteEndpointRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EndpointId: str,
```

## DeleteEventStreamRequestRequestTypeDef

```python
# DeleteEventStreamRequestRequestTypeDef definition

class DeleteEventStreamRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## EventStreamTypeDef

```python
# EventStreamTypeDef definition

class EventStreamTypeDef(TypedDict):
    ApplicationId: str,
    DestinationStreamArn: str,
    RoleArn: str,
    ExternalId: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    LastUpdatedBy: NotRequired[str],
```

## DeleteGcmChannelRequestRequestTypeDef

```python
# DeleteGcmChannelRequestRequestTypeDef definition

class DeleteGcmChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GCMChannelResponseTypeDef

```python
# GCMChannelResponseTypeDef definition

class GCMChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    Credential: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    HasFcmServiceCredentials: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## DeleteInAppTemplateRequestRequestTypeDef

```python
# DeleteInAppTemplateRequestRequestTypeDef definition

class DeleteInAppTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## DeleteJourneyRequestRequestTypeDef

```python
# DeleteJourneyRequestRequestTypeDef definition

class DeleteJourneyRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
```

## DeletePushTemplateRequestRequestTypeDef

```python
# DeletePushTemplateRequestRequestTypeDef definition

class DeletePushTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## DeleteRecommenderConfigurationRequestRequestTypeDef

```python
# DeleteRecommenderConfigurationRequestRequestTypeDef definition

class DeleteRecommenderConfigurationRequestRequestTypeDef(TypedDict):
    RecommenderId: str,
```

## DeleteSegmentRequestRequestTypeDef

```python
# DeleteSegmentRequestRequestTypeDef definition

class DeleteSegmentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SegmentId: str,
```

## DeleteSmsChannelRequestRequestTypeDef

```python
# DeleteSmsChannelRequestRequestTypeDef definition

class DeleteSmsChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## SMSChannelResponseTypeDef

```python
# SMSChannelResponseTypeDef definition

class SMSChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    PromotionalMessagesPerSecond: NotRequired[int],
    SenderId: NotRequired[str],
    ShortCode: NotRequired[str],
    TransactionalMessagesPerSecond: NotRequired[int],
    Version: NotRequired[int],
```

## DeleteSmsTemplateRequestRequestTypeDef

```python
# DeleteSmsTemplateRequestRequestTypeDef definition

class DeleteSmsTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## DeleteUserEndpointsRequestRequestTypeDef

```python
# DeleteUserEndpointsRequestRequestTypeDef definition

class DeleteUserEndpointsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    UserId: str,
```

## DeleteVoiceChannelRequestRequestTypeDef

```python
# DeleteVoiceChannelRequestRequestTypeDef definition

class DeleteVoiceChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## VoiceChannelResponseTypeDef

```python
# VoiceChannelResponseTypeDef definition

class VoiceChannelResponseTypeDef(TypedDict):
    Platform: str,
    ApplicationId: NotRequired[str],
    CreationDate: NotRequired[str],
    Enabled: NotRequired[bool],
    HasCredential: NotRequired[bool],
    Id: NotRequired[str],
    IsArchived: NotRequired[bool],
    LastModifiedBy: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Version: NotRequired[int],
```

## DeleteVoiceTemplateRequestRequestTypeDef

```python
# DeleteVoiceTemplateRequestRequestTypeDef definition

class DeleteVoiceTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## GCMMessageTypeDef

```python
# GCMMessageTypeDef definition

class GCMMessageTypeDef(TypedDict):
    Action: NotRequired[ActionType],  # (1)
    Body: NotRequired[str],
    CollapseKey: NotRequired[str],
    Data: NotRequired[Mapping[str, str]],
    IconReference: NotRequired[str],
    ImageIconUrl: NotRequired[str],
    ImageUrl: NotRequired[str],
    PreferredAuthenticationMethod: NotRequired[str],
    Priority: NotRequired[str],
    RawContent: NotRequired[str],
    RestrictedPackageName: NotRequired[str],
    SilentPush: NotRequired[bool],
    SmallImageIconUrl: NotRequired[str],
    Sound: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    TimeToLive: NotRequired[int],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## SMSMessageTypeDef

```python
# SMSMessageTypeDef definition

class SMSMessageTypeDef(TypedDict):
    Body: NotRequired[str],
    Keyword: NotRequired[str],
    MediaUrl: NotRequired[str],
    MessageType: NotRequired[MessageTypeType],  # (1)
    OriginationNumber: NotRequired[str],
    SenderId: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    EntityId: NotRequired[str],
    TemplateId: NotRequired[str],
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## VoiceMessageTypeDef

```python
# VoiceMessageTypeDef definition

class VoiceMessageTypeDef(TypedDict):
    Body: NotRequired[str],
    LanguageCode: NotRequired[str],
    OriginationNumber: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    VoiceId: NotRequired[str],
```

## EmailChannelRequestTypeDef

```python
# EmailChannelRequestTypeDef definition

class EmailChannelRequestTypeDef(TypedDict):
    FromAddress: str,
    Identity: str,
    ConfigurationSet: NotRequired[str],
    Enabled: NotRequired[bool],
    RoleArn: NotRequired[str],
    OrchestrationSendingRoleArn: NotRequired[str],
```

## JourneyEmailMessageTypeDef

```python
# JourneyEmailMessageTypeDef definition

class JourneyEmailMessageTypeDef(TypedDict):
    FromAddress: NotRequired[str],
```

## EndpointDemographicTypeDef

```python
# EndpointDemographicTypeDef definition

class EndpointDemographicTypeDef(TypedDict):
    AppVersion: NotRequired[str],
    Locale: NotRequired[str],
    Make: NotRequired[str],
    Model: NotRequired[str],
    ModelVersion: NotRequired[str],
    Platform: NotRequired[str],
    PlatformVersion: NotRequired[str],
    Timezone: NotRequired[str],
```

## EndpointLocationTypeDef

```python
# EndpointLocationTypeDef definition

class EndpointLocationTypeDef(TypedDict):
    City: NotRequired[str],
    Country: NotRequired[str],
    Latitude: NotRequired[float],
    Longitude: NotRequired[float],
    PostalCode: NotRequired[str],
    Region: NotRequired[str],
```

## EndpointItemResponseTypeDef

```python
# EndpointItemResponseTypeDef definition

class EndpointItemResponseTypeDef(TypedDict):
    Message: NotRequired[str],
    StatusCode: NotRequired[int],
```

## EndpointMessageResultTypeDef

```python
# EndpointMessageResultTypeDef definition

class EndpointMessageResultTypeDef(TypedDict):
    DeliveryStatus: DeliveryStatusType,  # (1)
    StatusCode: int,
    Address: NotRequired[str],
    MessageId: NotRequired[str],
    StatusMessage: NotRequired[str],
    UpdatedToken: NotRequired[str],
```

1. See [:material-code-brackets: DeliveryStatusType](./literals.md#deliverystatustype) 
## EndpointUserOutputTypeDef

```python
# EndpointUserOutputTypeDef definition

class EndpointUserOutputTypeDef(TypedDict):
    UserAttributes: NotRequired[Dict[str, List[str]]],
    UserId: NotRequired[str],
```

## EndpointSendConfigurationTypeDef

```python
# EndpointSendConfigurationTypeDef definition

class EndpointSendConfigurationTypeDef(TypedDict):
    BodyOverride: NotRequired[str],
    Context: NotRequired[Mapping[str, str]],
    RawContent: NotRequired[str],
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
    TitleOverride: NotRequired[str],
```

## EndpointUserTypeDef

```python
# EndpointUserTypeDef definition

class EndpointUserTypeDef(TypedDict):
    UserAttributes: NotRequired[Mapping[str, Sequence[str]]],
    UserId: NotRequired[str],
```

## MetricDimensionTypeDef

```python
# MetricDimensionTypeDef definition

class MetricDimensionTypeDef(TypedDict):
    ComparisonOperator: str,
    Value: float,
```

## SetDimensionOutputTypeDef

```python
# SetDimensionOutputTypeDef definition

class SetDimensionOutputTypeDef(TypedDict):
    Values: List[str],
    DimensionType: NotRequired[DimensionTypeType],  # (1)
```

1. See [:material-code-brackets: DimensionTypeType](./literals.md#dimensiontypetype) 
## EventItemResponseTypeDef

```python
# EventItemResponseTypeDef definition

class EventItemResponseTypeDef(TypedDict):
    Message: NotRequired[str],
    StatusCode: NotRequired[int],
```

## SessionTypeDef

```python
# SessionTypeDef definition

class SessionTypeDef(TypedDict):
    Id: str,
    StartTimestamp: str,
    Duration: NotRequired[int],
    StopTimestamp: NotRequired[str],
```

## ExportJobResourceTypeDef

```python
# ExportJobResourceTypeDef definition

class ExportJobResourceTypeDef(TypedDict):
    RoleArn: str,
    S3UrlPrefix: str,
    SegmentId: NotRequired[str],
    SegmentVersion: NotRequired[int],
```

## GCMChannelRequestTypeDef

```python
# GCMChannelRequestTypeDef definition

class GCMChannelRequestTypeDef(TypedDict):
    ApiKey: NotRequired[str],
    DefaultAuthenticationMethod: NotRequired[str],
    Enabled: NotRequired[bool],
    ServiceJson: NotRequired[str],
```

## GPSCoordinatesTypeDef

```python
# GPSCoordinatesTypeDef definition

class GPSCoordinatesTypeDef(TypedDict):
    Latitude: float,
    Longitude: float,
```

## GetAdmChannelRequestRequestTypeDef

```python
# GetAdmChannelRequestRequestTypeDef definition

class GetAdmChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetApnsChannelRequestRequestTypeDef

```python
# GetApnsChannelRequestRequestTypeDef definition

class GetApnsChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetApnsSandboxChannelRequestRequestTypeDef

```python
# GetApnsSandboxChannelRequestRequestTypeDef definition

class GetApnsSandboxChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetApnsVoipChannelRequestRequestTypeDef

```python
# GetApnsVoipChannelRequestRequestTypeDef definition

class GetApnsVoipChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetApnsVoipSandboxChannelRequestRequestTypeDef

```python
# GetApnsVoipSandboxChannelRequestRequestTypeDef definition

class GetApnsVoipSandboxChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetAppRequestRequestTypeDef

```python
# GetAppRequestRequestTypeDef definition

class GetAppRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetApplicationSettingsRequestRequestTypeDef

```python
# GetApplicationSettingsRequestRequestTypeDef definition

class GetApplicationSettingsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetAppsRequestRequestTypeDef

```python
# GetAppsRequestRequestTypeDef definition

class GetAppsRequestRequestTypeDef(TypedDict):
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetBaiduChannelRequestRequestTypeDef

```python
# GetBaiduChannelRequestRequestTypeDef definition

class GetBaiduChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetCampaignActivitiesRequestRequestTypeDef

```python
# GetCampaignActivitiesRequestRequestTypeDef definition

class GetCampaignActivitiesRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetCampaignRequestRequestTypeDef

```python
# GetCampaignRequestRequestTypeDef definition

class GetCampaignRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
```

## GetCampaignVersionRequestRequestTypeDef

```python
# GetCampaignVersionRequestRequestTypeDef definition

class GetCampaignVersionRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
    Version: str,
```

## GetCampaignVersionsRequestRequestTypeDef

```python
# GetCampaignVersionsRequestRequestTypeDef definition

class GetCampaignVersionsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetCampaignsRequestRequestTypeDef

```python
# GetCampaignsRequestRequestTypeDef definition

class GetCampaignsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetChannelsRequestRequestTypeDef

```python
# GetChannelsRequestRequestTypeDef definition

class GetChannelsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetEmailChannelRequestRequestTypeDef

```python
# GetEmailChannelRequestRequestTypeDef definition

class GetEmailChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetEmailTemplateRequestRequestTypeDef

```python
# GetEmailTemplateRequestRequestTypeDef definition

class GetEmailTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## GetEndpointRequestRequestTypeDef

```python
# GetEndpointRequestRequestTypeDef definition

class GetEndpointRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EndpointId: str,
```

## GetEventStreamRequestRequestTypeDef

```python
# GetEventStreamRequestRequestTypeDef definition

class GetEventStreamRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetExportJobRequestRequestTypeDef

```python
# GetExportJobRequestRequestTypeDef definition

class GetExportJobRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JobId: str,
```

## GetExportJobsRequestRequestTypeDef

```python
# GetExportJobsRequestRequestTypeDef definition

class GetExportJobsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetGcmChannelRequestRequestTypeDef

```python
# GetGcmChannelRequestRequestTypeDef definition

class GetGcmChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetImportJobRequestRequestTypeDef

```python
# GetImportJobRequestRequestTypeDef definition

class GetImportJobRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JobId: str,
```

## GetImportJobsRequestRequestTypeDef

```python
# GetImportJobsRequestRequestTypeDef definition

class GetImportJobsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetInAppMessagesRequestRequestTypeDef

```python
# GetInAppMessagesRequestRequestTypeDef definition

class GetInAppMessagesRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EndpointId: str,
```

## GetInAppTemplateRequestRequestTypeDef

```python
# GetInAppTemplateRequestRequestTypeDef definition

class GetInAppTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## GetJourneyExecutionActivityMetricsRequestRequestTypeDef

```python
# GetJourneyExecutionActivityMetricsRequestRequestTypeDef definition

class GetJourneyExecutionActivityMetricsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyActivityId: str,
    JourneyId: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
```

## JourneyExecutionActivityMetricsResponseTypeDef

```python
# JourneyExecutionActivityMetricsResponseTypeDef definition

class JourneyExecutionActivityMetricsResponseTypeDef(TypedDict):
    ActivityType: str,
    ApplicationId: str,
    JourneyActivityId: str,
    JourneyId: str,
    LastEvaluatedTime: str,
    Metrics: Dict[str, str],
```

## GetJourneyExecutionMetricsRequestRequestTypeDef

```python
# GetJourneyExecutionMetricsRequestRequestTypeDef definition

class GetJourneyExecutionMetricsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
```

## JourneyExecutionMetricsResponseTypeDef

```python
# JourneyExecutionMetricsResponseTypeDef definition

class JourneyExecutionMetricsResponseTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
    LastEvaluatedTime: str,
    Metrics: Dict[str, str],
```

## GetJourneyRequestRequestTypeDef

```python
# GetJourneyRequestRequestTypeDef definition

class GetJourneyRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
```

## GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef

```python
# GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef definition

class GetJourneyRunExecutionActivityMetricsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyActivityId: str,
    JourneyId: str,
    RunId: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
```

## JourneyRunExecutionActivityMetricsResponseTypeDef

```python
# JourneyRunExecutionActivityMetricsResponseTypeDef definition

class JourneyRunExecutionActivityMetricsResponseTypeDef(TypedDict):
    ActivityType: str,
    ApplicationId: str,
    JourneyActivityId: str,
    JourneyId: str,
    LastEvaluatedTime: str,
    Metrics: Dict[str, str],
    RunId: str,
```

## GetJourneyRunExecutionMetricsRequestRequestTypeDef

```python
# GetJourneyRunExecutionMetricsRequestRequestTypeDef definition

class GetJourneyRunExecutionMetricsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
    RunId: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
```

## JourneyRunExecutionMetricsResponseTypeDef

```python
# JourneyRunExecutionMetricsResponseTypeDef definition

class JourneyRunExecutionMetricsResponseTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
    LastEvaluatedTime: str,
    Metrics: Dict[str, str],
    RunId: str,
```

## GetJourneyRunsRequestRequestTypeDef

```python
# GetJourneyRunsRequestRequestTypeDef definition

class GetJourneyRunsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetPushTemplateRequestRequestTypeDef

```python
# GetPushTemplateRequestRequestTypeDef definition

class GetPushTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## GetRecommenderConfigurationRequestRequestTypeDef

```python
# GetRecommenderConfigurationRequestRequestTypeDef definition

class GetRecommenderConfigurationRequestRequestTypeDef(TypedDict):
    RecommenderId: str,
```

## GetRecommenderConfigurationsRequestRequestTypeDef

```python
# GetRecommenderConfigurationsRequestRequestTypeDef definition

class GetRecommenderConfigurationsRequestRequestTypeDef(TypedDict):
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetSegmentExportJobsRequestRequestTypeDef

```python
# GetSegmentExportJobsRequestRequestTypeDef definition

class GetSegmentExportJobsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SegmentId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetSegmentImportJobsRequestRequestTypeDef

```python
# GetSegmentImportJobsRequestRequestTypeDef definition

class GetSegmentImportJobsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SegmentId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetSegmentRequestRequestTypeDef

```python
# GetSegmentRequestRequestTypeDef definition

class GetSegmentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SegmentId: str,
```

## GetSegmentVersionRequestRequestTypeDef

```python
# GetSegmentVersionRequestRequestTypeDef definition

class GetSegmentVersionRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SegmentId: str,
    Version: str,
```

## GetSegmentVersionsRequestRequestTypeDef

```python
# GetSegmentVersionsRequestRequestTypeDef definition

class GetSegmentVersionsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SegmentId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetSegmentsRequestRequestTypeDef

```python
# GetSegmentsRequestRequestTypeDef definition

class GetSegmentsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## GetSmsChannelRequestRequestTypeDef

```python
# GetSmsChannelRequestRequestTypeDef definition

class GetSmsChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetSmsTemplateRequestRequestTypeDef

```python
# GetSmsTemplateRequestRequestTypeDef definition

class GetSmsTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## SMSTemplateResponseTypeDef

```python
# SMSTemplateResponseTypeDef definition

class SMSTemplateResponseTypeDef(TypedDict):
    CreationDate: str,
    LastModifiedDate: str,
    TemplateName: str,
    TemplateType: TemplateTypeType,  # (1)
    Arn: NotRequired[str],
    Body: NotRequired[str],
    DefaultSubstitutions: NotRequired[str],
    RecommenderId: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    TemplateDescription: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## GetUserEndpointsRequestRequestTypeDef

```python
# GetUserEndpointsRequestRequestTypeDef definition

class GetUserEndpointsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    UserId: str,
```

## GetVoiceChannelRequestRequestTypeDef

```python
# GetVoiceChannelRequestRequestTypeDef definition

class GetVoiceChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
```

## GetVoiceTemplateRequestRequestTypeDef

```python
# GetVoiceTemplateRequestRequestTypeDef definition

class GetVoiceTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    Version: NotRequired[str],
```

## VoiceTemplateResponseTypeDef

```python
# VoiceTemplateResponseTypeDef definition

class VoiceTemplateResponseTypeDef(TypedDict):
    CreationDate: str,
    LastModifiedDate: str,
    TemplateName: str,
    TemplateType: TemplateTypeType,  # (1)
    Arn: NotRequired[str],
    Body: NotRequired[str],
    DefaultSubstitutions: NotRequired[str],
    LanguageCode: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    TemplateDescription: NotRequired[str],
    Version: NotRequired[str],
    VoiceId: NotRequired[str],
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## ImportJobResourceTypeDef

```python
# ImportJobResourceTypeDef definition

class ImportJobResourceTypeDef(TypedDict):
    Format: FormatType,  # (1)
    RoleArn: str,
    S3Url: str,
    DefineSegment: NotRequired[bool],
    ExternalId: NotRequired[str],
    RegisterEndpoints: NotRequired[bool],
    SegmentId: NotRequired[str],
    SegmentName: NotRequired[str],
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## InAppMessageBodyConfigTypeDef

```python
# InAppMessageBodyConfigTypeDef definition

class InAppMessageBodyConfigTypeDef(TypedDict):
    Alignment: AlignmentType,  # (1)
    Body: str,
    TextColor: str,
```

1. See [:material-code-brackets: AlignmentType](./literals.md#alignmenttype) 
## OverrideButtonConfigurationTypeDef

```python
# OverrideButtonConfigurationTypeDef definition

class OverrideButtonConfigurationTypeDef(TypedDict):
    ButtonAction: ButtonActionType,  # (1)
    Link: NotRequired[str],
```

1. See [:material-code-brackets: ButtonActionType](./literals.md#buttonactiontype) 
## InAppMessageHeaderConfigTypeDef

```python
# InAppMessageHeaderConfigTypeDef definition

class InAppMessageHeaderConfigTypeDef(TypedDict):
    Alignment: AlignmentType,  # (1)
    Header: str,
    TextColor: str,
```

1. See [:material-code-brackets: AlignmentType](./literals.md#alignmenttype) 
## JourneyChannelSettingsTypeDef

```python
# JourneyChannelSettingsTypeDef definition

class JourneyChannelSettingsTypeDef(TypedDict):
    ConnectCampaignArn: NotRequired[str],
    ConnectCampaignExecutionRoleArn: NotRequired[str],
```

## JourneyPushMessageTypeDef

```python
# JourneyPushMessageTypeDef definition

class JourneyPushMessageTypeDef(TypedDict):
    TimeToLive: NotRequired[str],
```

## JourneyScheduleOutputTypeDef

```python
# JourneyScheduleOutputTypeDef definition

class JourneyScheduleOutputTypeDef(TypedDict):
    EndTime: NotRequired[datetime],
    StartTime: NotRequired[datetime],
    Timezone: NotRequired[str],
```

## JourneyRunResponseTypeDef

```python
# JourneyRunResponseTypeDef definition

class JourneyRunResponseTypeDef(TypedDict):
    CreationTime: str,
    LastUpdateTime: str,
    RunId: str,
    Status: JourneyRunStatusType,  # (1)
```

1. See [:material-code-brackets: JourneyRunStatusType](./literals.md#journeyrunstatustype) 
## JourneySMSMessageTypeDef

```python
# JourneySMSMessageTypeDef definition

class JourneySMSMessageTypeDef(TypedDict):
    MessageType: NotRequired[MessageTypeType],  # (1)
    OriginationNumber: NotRequired[str],
    SenderId: NotRequired[str],
    EntityId: NotRequired[str],
    TemplateId: NotRequired[str],
```

1. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
## JourneyStateRequestTypeDef

```python
# JourneyStateRequestTypeDef definition

class JourneyStateRequestTypeDef(TypedDict):
    State: NotRequired[StateType],  # (1)
```

1. See [:material-code-brackets: StateType](./literals.md#statetype) 
## ListJourneysRequestRequestTypeDef

```python
# ListJourneysRequestRequestTypeDef definition

class ListJourneysRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    PageSize: NotRequired[str],
    Token: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagsModelOutputTypeDef

```python
# TagsModelOutputTypeDef definition

class TagsModelOutputTypeDef(TypedDict):
    tags: Dict[str, str],
```

## ListTemplateVersionsRequestRequestTypeDef

```python
# ListTemplateVersionsRequestRequestTypeDef definition

class ListTemplateVersionsRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    TemplateType: str,
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
```

## ListTemplatesRequestRequestTypeDef

```python
# ListTemplatesRequestRequestTypeDef definition

class ListTemplatesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
    Prefix: NotRequired[str],
    TemplateType: NotRequired[str],
```

## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    Action: NotRequired[ActionType],  # (1)
    Body: NotRequired[str],
    ImageIconUrl: NotRequired[str],
    ImageSmallIconUrl: NotRequired[str],
    ImageUrl: NotRequired[str],
    JsonBody: NotRequired[str],
    MediaUrl: NotRequired[str],
    RawContent: NotRequired[str],
    SilentPush: NotRequired[bool],
    TimeToLive: NotRequired[int],
    Title: NotRequired[str],
    Url: NotRequired[str],
```

1. See [:material-code-brackets: ActionType](./literals.md#actiontype) 
## MessageResultTypeDef

```python
# MessageResultTypeDef definition

class MessageResultTypeDef(TypedDict):
    DeliveryStatus: DeliveryStatusType,  # (1)
    StatusCode: int,
    MessageId: NotRequired[str],
    StatusMessage: NotRequired[str],
    UpdatedToken: NotRequired[str],
```

1. See [:material-code-brackets: DeliveryStatusType](./literals.md#deliverystatustype) 
## NumberValidateRequestTypeDef

```python
# NumberValidateRequestTypeDef definition

class NumberValidateRequestTypeDef(TypedDict):
    IsoCountryCode: NotRequired[str],
    PhoneNumber: NotRequired[str],
```

## NumberValidateResponseTypeDef

```python
# NumberValidateResponseTypeDef definition

class NumberValidateResponseTypeDef(TypedDict):
    Carrier: NotRequired[str],
    City: NotRequired[str],
    CleansedPhoneNumberE164: NotRequired[str],
    CleansedPhoneNumberNational: NotRequired[str],
    Country: NotRequired[str],
    CountryCodeIso2: NotRequired[str],
    CountryCodeNumeric: NotRequired[str],
    County: NotRequired[str],
    OriginalCountryCodeIso2: NotRequired[str],
    OriginalPhoneNumber: NotRequired[str],
    PhoneType: NotRequired[str],
    PhoneTypeCode: NotRequired[int],
    Timezone: NotRequired[str],
    ZipCode: NotRequired[str],
```

## OpenHoursRuleTypeDef

```python
# OpenHoursRuleTypeDef definition

class OpenHoursRuleTypeDef(TypedDict):
    StartTime: NotRequired[str],
    EndTime: NotRequired[str],
```

## WriteEventStreamTypeDef

```python
# WriteEventStreamTypeDef definition

class WriteEventStreamTypeDef(TypedDict):
    DestinationStreamArn: str,
    RoleArn: str,
```

## RandomSplitEntryTypeDef

```python
# RandomSplitEntryTypeDef definition

class RandomSplitEntryTypeDef(TypedDict):
    NextActivity: NotRequired[str],
    Percentage: NotRequired[int],
```

## RecencyDimensionTypeDef

```python
# RecencyDimensionTypeDef definition

class RecencyDimensionTypeDef(TypedDict):
    Duration: DurationType,  # (1)
    RecencyType: RecencyTypeType,  # (2)
```

1. See [:material-code-brackets: DurationType](./literals.md#durationtype) 
2. See [:material-code-brackets: RecencyTypeType](./literals.md#recencytypetype) 
## UpdateAttributesRequestTypeDef

```python
# UpdateAttributesRequestTypeDef definition

class UpdateAttributesRequestTypeDef(TypedDict):
    Blacklist: NotRequired[Sequence[str]],
```

## ResultRowValueTypeDef

```python
# ResultRowValueTypeDef definition

class ResultRowValueTypeDef(TypedDict):
    Key: str,
    Type: str,
    Value: str,
```

## SMSChannelRequestTypeDef

```python
# SMSChannelRequestTypeDef definition

class SMSChannelRequestTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    SenderId: NotRequired[str],
    ShortCode: NotRequired[str],
```

## SegmentConditionTypeDef

```python
# SegmentConditionTypeDef definition

class SegmentConditionTypeDef(TypedDict):
    SegmentId: str,
```

## SegmentReferenceTypeDef

```python
# SegmentReferenceTypeDef definition

class SegmentReferenceTypeDef(TypedDict):
    Id: str,
    Version: NotRequired[int],
```

## SegmentImportResourceTypeDef

```python
# SegmentImportResourceTypeDef definition

class SegmentImportResourceTypeDef(TypedDict):
    ExternalId: str,
    Format: FormatType,  # (1)
    RoleArn: str,
    S3Url: str,
    Size: int,
    ChannelCounts: NotRequired[Dict[str, int]],
```

1. See [:material-code-brackets: FormatType](./literals.md#formattype) 
## SendOTPMessageRequestParametersTypeDef

```python
# SendOTPMessageRequestParametersTypeDef definition

class SendOTPMessageRequestParametersTypeDef(TypedDict):
    BrandName: str,
    Channel: str,
    DestinationIdentity: str,
    OriginationIdentity: str,
    ReferenceId: str,
    AllowedAttempts: NotRequired[int],
    CodeLength: NotRequired[int],
    EntityId: NotRequired[str],
    Language: NotRequired[str],
    TemplateId: NotRequired[str],
    ValidityPeriod: NotRequired[int],
```

## SetDimensionTypeDef

```python
# SetDimensionTypeDef definition

class SetDimensionTypeDef(TypedDict):
    Values: Sequence[str],
    DimensionType: NotRequired[DimensionTypeType],  # (1)
```

1. See [:material-code-brackets: DimensionTypeType](./literals.md#dimensiontypetype) 
## SimpleEmailPartTypeDef

```python
# SimpleEmailPartTypeDef definition

class SimpleEmailPartTypeDef(TypedDict):
    Charset: NotRequired[str],
    Data: NotRequired[str],
```

## TagsModelTypeDef

```python
# TagsModelTypeDef definition

class TagsModelTypeDef(TypedDict):
    tags: Mapping[str, str],
```

## TemplateActiveVersionRequestTypeDef

```python
# TemplateActiveVersionRequestTypeDef definition

class TemplateActiveVersionRequestTypeDef(TypedDict):
    Version: NotRequired[str],
```

## TemplateTypeDef

```python
# TemplateTypeDef definition

class TemplateTypeDef(TypedDict):
    Name: NotRequired[str],
    Version: NotRequired[str],
```

## TemplateResponseTypeDef

```python
# TemplateResponseTypeDef definition

class TemplateResponseTypeDef(TypedDict):
    CreationDate: str,
    LastModifiedDate: str,
    TemplateName: str,
    TemplateType: TemplateTypeType,  # (1)
    Arn: NotRequired[str],
    DefaultSubstitutions: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    TemplateDescription: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## TemplateVersionResponseTypeDef

```python
# TemplateVersionResponseTypeDef definition

class TemplateVersionResponseTypeDef(TypedDict):
    CreationDate: str,
    LastModifiedDate: str,
    TemplateName: str,
    TemplateType: str,
    DefaultSubstitutions: NotRequired[str],
    TemplateDescription: NotRequired[str],
    Version: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateRecommenderConfigurationTypeDef

```python
# UpdateRecommenderConfigurationTypeDef definition

class UpdateRecommenderConfigurationTypeDef(TypedDict):
    RecommendationProviderRoleArn: str,
    RecommendationProviderUri: str,
    Attributes: NotRequired[Mapping[str, str]],
    Description: NotRequired[str],
    Name: NotRequired[str],
    RecommendationProviderIdType: NotRequired[str],
    RecommendationTransformerUri: NotRequired[str],
    RecommendationsDisplayName: NotRequired[str],
    RecommendationsPerMessage: NotRequired[int],
```

## VoiceChannelRequestTypeDef

```python
# VoiceChannelRequestTypeDef definition

class VoiceChannelRequestTypeDef(TypedDict):
    Enabled: NotRequired[bool],
```

## VerificationResponseTypeDef

```python
# VerificationResponseTypeDef definition

class VerificationResponseTypeDef(TypedDict):
    Valid: NotRequired[bool],
```

## VerifyOTPMessageRequestParametersTypeDef

```python
# VerifyOTPMessageRequestParametersTypeDef definition

class VerifyOTPMessageRequestParametersTypeDef(TypedDict):
    DestinationIdentity: str,
    Otp: str,
    ReferenceId: str,
```

## UpdateAdmChannelRequestRequestTypeDef

```python
# UpdateAdmChannelRequestRequestTypeDef definition

class UpdateAdmChannelRequestRequestTypeDef(TypedDict):
    ADMChannelRequest: ADMChannelRequestTypeDef,  # (1)
    ApplicationId: str,
```

1. See [:material-code-braces: ADMChannelRequestTypeDef](./type_defs.md#admchannelrequesttypedef) 
## UpdateApnsChannelRequestRequestTypeDef

```python
# UpdateApnsChannelRequestRequestTypeDef definition

class UpdateApnsChannelRequestRequestTypeDef(TypedDict):
    APNSChannelRequest: APNSChannelRequestTypeDef,  # (1)
    ApplicationId: str,
```

1. See [:material-code-braces: APNSChannelRequestTypeDef](./type_defs.md#apnschannelrequesttypedef) 
## UpdateApnsSandboxChannelRequestRequestTypeDef

```python
# UpdateApnsSandboxChannelRequestRequestTypeDef definition

class UpdateApnsSandboxChannelRequestRequestTypeDef(TypedDict):
    APNSSandboxChannelRequest: APNSSandboxChannelRequestTypeDef,  # (1)
    ApplicationId: str,
```

1. See [:material-code-braces: APNSSandboxChannelRequestTypeDef](./type_defs.md#apnssandboxchannelrequesttypedef) 
## UpdateApnsVoipChannelRequestRequestTypeDef

```python
# UpdateApnsVoipChannelRequestRequestTypeDef definition

class UpdateApnsVoipChannelRequestRequestTypeDef(TypedDict):
    APNSVoipChannelRequest: APNSVoipChannelRequestTypeDef,  # (1)
    ApplicationId: str,
```

1. See [:material-code-braces: APNSVoipChannelRequestTypeDef](./type_defs.md#apnsvoipchannelrequesttypedef) 
## UpdateApnsVoipSandboxChannelRequestRequestTypeDef

```python
# UpdateApnsVoipSandboxChannelRequestRequestTypeDef definition

class UpdateApnsVoipSandboxChannelRequestRequestTypeDef(TypedDict):
    APNSVoipSandboxChannelRequest: APNSVoipSandboxChannelRequestTypeDef,  # (1)
    ApplicationId: str,
```

1. See [:material-code-braces: APNSVoipSandboxChannelRequestTypeDef](./type_defs.md#apnsvoipsandboxchannelrequesttypedef) 
## ActivitiesResponseTypeDef

```python
# ActivitiesResponseTypeDef definition

class ActivitiesResponseTypeDef(TypedDict):
    Item: List[ActivityResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ActivityResponseTypeDef](./type_defs.md#activityresponsetypedef) 
## ApplicationsResponseTypeDef

```python
# ApplicationsResponseTypeDef definition

class ApplicationsResponseTypeDef(TypedDict):
    Item: NotRequired[List[ApplicationResponseTypeDef]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 
## ApplicationSettingsJourneyLimitsTypeDef

```python
# ApplicationSettingsJourneyLimitsTypeDef definition

class ApplicationSettingsJourneyLimitsTypeDef(TypedDict):
    DailyCap: NotRequired[int],
    TimeframeCap: NotRequired[JourneyTimeframeCapTypeDef],  # (1)
    TotalCap: NotRequired[int],
```

1. See [:material-code-braces: JourneyTimeframeCapTypeDef](./type_defs.md#journeytimeframecaptypedef) 
## JourneyLimitsTypeDef

```python
# JourneyLimitsTypeDef definition

class JourneyLimitsTypeDef(TypedDict):
    DailyCap: NotRequired[int],
    EndpointReentryCap: NotRequired[int],
    MessagesPerSecond: NotRequired[int],
    EndpointReentryInterval: NotRequired[str],
    TimeframeCap: NotRequired[JourneyTimeframeCapTypeDef],  # (1)
    TotalCap: NotRequired[int],
```

1. See [:material-code-braces: JourneyTimeframeCapTypeDef](./type_defs.md#journeytimeframecaptypedef) 
## UpdateBaiduChannelRequestRequestTypeDef

```python
# UpdateBaiduChannelRequestRequestTypeDef definition

class UpdateBaiduChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    BaiduChannelRequest: BaiduChannelRequestTypeDef,  # (1)
```

1. See [:material-code-braces: BaiduChannelRequestTypeDef](./type_defs.md#baiduchannelrequesttypedef) 
## RawEmailTypeDef

```python
# RawEmailTypeDef definition

class RawEmailTypeDef(TypedDict):
    Data: NotRequired[BlobTypeDef],
```

## CampaignEmailMessageOutputTypeDef

```python
# CampaignEmailMessageOutputTypeDef definition

class CampaignEmailMessageOutputTypeDef(TypedDict):
    Body: NotRequired[str],
    FromAddress: NotRequired[str],
    Headers: NotRequired[List[MessageHeaderTypeDef]],  # (1)
    HtmlBody: NotRequired[str],
    Title: NotRequired[str],
```

1. See [:material-code-braces: MessageHeaderTypeDef](./type_defs.md#messageheadertypedef) 
## CampaignEmailMessageTypeDef

```python
# CampaignEmailMessageTypeDef definition

class CampaignEmailMessageTypeDef(TypedDict):
    Body: NotRequired[str],
    FromAddress: NotRequired[str],
    Headers: NotRequired[Sequence[MessageHeaderTypeDef]],  # (1)
    HtmlBody: NotRequired[str],
    Title: NotRequired[str],
```

1. See [:material-code-braces: MessageHeaderTypeDef](./type_defs.md#messageheadertypedef) 
## EmailTemplateRequestTypeDef

```python
# EmailTemplateRequestTypeDef definition

class EmailTemplateRequestTypeDef(TypedDict):
    DefaultSubstitutions: NotRequired[str],
    HtmlPart: NotRequired[str],
    RecommenderId: NotRequired[str],
    Subject: NotRequired[str],
    Headers: NotRequired[Sequence[MessageHeaderTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
    TemplateDescription: NotRequired[str],
    TextPart: NotRequired[str],
```

1. See [:material-code-braces: MessageHeaderTypeDef](./type_defs.md#messageheadertypedef) 
## EmailTemplateResponseTypeDef

```python
# EmailTemplateResponseTypeDef definition

class EmailTemplateResponseTypeDef(TypedDict):
    CreationDate: str,
    LastModifiedDate: str,
    TemplateName: str,
    TemplateType: TemplateTypeType,  # (2)
    Arn: NotRequired[str],
    DefaultSubstitutions: NotRequired[str],
    HtmlPart: NotRequired[str],
    RecommenderId: NotRequired[str],
    Subject: NotRequired[str],
    Headers: NotRequired[List[MessageHeaderTypeDef]],  # (1)
    tags: NotRequired[Dict[str, str]],
    TemplateDescription: NotRequired[str],
    TextPart: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-braces: MessageHeaderTypeDef](./type_defs.md#messageheadertypedef) 
2. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## ChannelsResponseTypeDef

```python
# ChannelsResponseTypeDef definition

class ChannelsResponseTypeDef(TypedDict):
    Channels: Dict[str, ChannelResponseTypeDef],  # (1)
```

1. See [:material-code-braces: ChannelResponseTypeDef](./type_defs.md#channelresponsetypedef) 
## ClosedDaysOutputTypeDef

```python
# ClosedDaysOutputTypeDef definition

class ClosedDaysOutputTypeDef(TypedDict):
    EMAIL: NotRequired[List[ClosedDaysRuleTypeDef]],  # (1)
    SMS: NotRequired[List[ClosedDaysRuleTypeDef]],  # (1)
    PUSH: NotRequired[List[ClosedDaysRuleTypeDef]],  # (1)
    VOICE: NotRequired[List[ClosedDaysRuleTypeDef]],  # (1)
    CUSTOM: NotRequired[List[ClosedDaysRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
2. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
3. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
4. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
5. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
## ClosedDaysTypeDef

```python
# ClosedDaysTypeDef definition

class ClosedDaysTypeDef(TypedDict):
    EMAIL: NotRequired[Sequence[ClosedDaysRuleTypeDef]],  # (1)
    SMS: NotRequired[Sequence[ClosedDaysRuleTypeDef]],  # (1)
    PUSH: NotRequired[Sequence[ClosedDaysRuleTypeDef]],  # (1)
    VOICE: NotRequired[Sequence[ClosedDaysRuleTypeDef]],  # (1)
    CUSTOM: NotRequired[Sequence[ClosedDaysRuleTypeDef]],  # (1)
```

1. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
2. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
3. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
4. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
5. See [:material-code-braces: ClosedDaysRuleTypeDef](./type_defs.md#closeddaysruletypedef) 
## WaitActivityTypeDef

```python
# WaitActivityTypeDef definition

class WaitActivityTypeDef(TypedDict):
    NextActivity: NotRequired[str],
    WaitTime: NotRequired[WaitTimeTypeDef],  # (1)
```

1. See [:material-code-braces: WaitTimeTypeDef](./type_defs.md#waittimetypedef) 
## CreateAppRequestRequestTypeDef

```python
# CreateAppRequestRequestTypeDef definition

class CreateAppRequestRequestTypeDef(TypedDict):
    CreateApplicationRequest: CreateApplicationRequestTypeDef,  # (1)
```

1. See [:material-code-braces: CreateApplicationRequestTypeDef](./type_defs.md#createapplicationrequesttypedef) 
## CreateAppResponseTypeDef

```python
# CreateAppResponseTypeDef definition

class CreateAppResponseTypeDef(TypedDict):
    ApplicationResponse: ApplicationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAdmChannelResponseTypeDef

```python
# DeleteAdmChannelResponseTypeDef definition

class DeleteAdmChannelResponseTypeDef(TypedDict):
    ADMChannelResponse: ADMChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ADMChannelResponseTypeDef](./type_defs.md#admchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApnsChannelResponseTypeDef

```python
# DeleteApnsChannelResponseTypeDef definition

class DeleteApnsChannelResponseTypeDef(TypedDict):
    APNSChannelResponse: APNSChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSChannelResponseTypeDef](./type_defs.md#apnschannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApnsSandboxChannelResponseTypeDef

```python
# DeleteApnsSandboxChannelResponseTypeDef definition

class DeleteApnsSandboxChannelResponseTypeDef(TypedDict):
    APNSSandboxChannelResponse: APNSSandboxChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSSandboxChannelResponseTypeDef](./type_defs.md#apnssandboxchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApnsVoipChannelResponseTypeDef

```python
# DeleteApnsVoipChannelResponseTypeDef definition

class DeleteApnsVoipChannelResponseTypeDef(TypedDict):
    APNSVoipChannelResponse: APNSVoipChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSVoipChannelResponseTypeDef](./type_defs.md#apnsvoipchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteApnsVoipSandboxChannelResponseTypeDef

```python
# DeleteApnsVoipSandboxChannelResponseTypeDef definition

class DeleteApnsVoipSandboxChannelResponseTypeDef(TypedDict):
    APNSVoipSandboxChannelResponse: APNSVoipSandboxChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSVoipSandboxChannelResponseTypeDef](./type_defs.md#apnsvoipsandboxchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAppResponseTypeDef

```python
# DeleteAppResponseTypeDef definition

class DeleteAppResponseTypeDef(TypedDict):
    ApplicationResponse: ApplicationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBaiduChannelResponseTypeDef

```python
# DeleteBaiduChannelResponseTypeDef definition

class DeleteBaiduChannelResponseTypeDef(TypedDict):
    BaiduChannelResponse: BaiduChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BaiduChannelResponseTypeDef](./type_defs.md#baiduchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAdmChannelResponseTypeDef

```python
# GetAdmChannelResponseTypeDef definition

class GetAdmChannelResponseTypeDef(TypedDict):
    ADMChannelResponse: ADMChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ADMChannelResponseTypeDef](./type_defs.md#admchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApnsChannelResponseTypeDef

```python
# GetApnsChannelResponseTypeDef definition

class GetApnsChannelResponseTypeDef(TypedDict):
    APNSChannelResponse: APNSChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSChannelResponseTypeDef](./type_defs.md#apnschannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApnsSandboxChannelResponseTypeDef

```python
# GetApnsSandboxChannelResponseTypeDef definition

class GetApnsSandboxChannelResponseTypeDef(TypedDict):
    APNSSandboxChannelResponse: APNSSandboxChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSSandboxChannelResponseTypeDef](./type_defs.md#apnssandboxchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApnsVoipChannelResponseTypeDef

```python
# GetApnsVoipChannelResponseTypeDef definition

class GetApnsVoipChannelResponseTypeDef(TypedDict):
    APNSVoipChannelResponse: APNSVoipChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSVoipChannelResponseTypeDef](./type_defs.md#apnsvoipchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApnsVoipSandboxChannelResponseTypeDef

```python
# GetApnsVoipSandboxChannelResponseTypeDef definition

class GetApnsVoipSandboxChannelResponseTypeDef(TypedDict):
    APNSVoipSandboxChannelResponse: APNSVoipSandboxChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSVoipSandboxChannelResponseTypeDef](./type_defs.md#apnsvoipsandboxchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppResponseTypeDef

```python
# GetAppResponseTypeDef definition

class GetAppResponseTypeDef(TypedDict):
    ApplicationResponse: ApplicationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationResponseTypeDef](./type_defs.md#applicationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBaiduChannelResponseTypeDef

```python
# GetBaiduChannelResponseTypeDef definition

class GetBaiduChannelResponseTypeDef(TypedDict):
    BaiduChannelResponse: BaiduChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BaiduChannelResponseTypeDef](./type_defs.md#baiduchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemoveAttributesResponseTypeDef

```python
# RemoveAttributesResponseTypeDef definition

class RemoveAttributesResponseTypeDef(TypedDict):
    AttributesResource: AttributesResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributesResourceTypeDef](./type_defs.md#attributesresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAdmChannelResponseTypeDef

```python
# UpdateAdmChannelResponseTypeDef definition

class UpdateAdmChannelResponseTypeDef(TypedDict):
    ADMChannelResponse: ADMChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ADMChannelResponseTypeDef](./type_defs.md#admchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApnsChannelResponseTypeDef

```python
# UpdateApnsChannelResponseTypeDef definition

class UpdateApnsChannelResponseTypeDef(TypedDict):
    APNSChannelResponse: APNSChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSChannelResponseTypeDef](./type_defs.md#apnschannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApnsSandboxChannelResponseTypeDef

```python
# UpdateApnsSandboxChannelResponseTypeDef definition

class UpdateApnsSandboxChannelResponseTypeDef(TypedDict):
    APNSSandboxChannelResponse: APNSSandboxChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSSandboxChannelResponseTypeDef](./type_defs.md#apnssandboxchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApnsVoipChannelResponseTypeDef

```python
# UpdateApnsVoipChannelResponseTypeDef definition

class UpdateApnsVoipChannelResponseTypeDef(TypedDict):
    APNSVoipChannelResponse: APNSVoipChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSVoipChannelResponseTypeDef](./type_defs.md#apnsvoipchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApnsVoipSandboxChannelResponseTypeDef

```python
# UpdateApnsVoipSandboxChannelResponseTypeDef definition

class UpdateApnsVoipSandboxChannelResponseTypeDef(TypedDict):
    APNSVoipSandboxChannelResponse: APNSVoipSandboxChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: APNSVoipSandboxChannelResponseTypeDef](./type_defs.md#apnsvoipsandboxchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBaiduChannelResponseTypeDef

```python
# UpdateBaiduChannelResponseTypeDef definition

class UpdateBaiduChannelResponseTypeDef(TypedDict):
    BaiduChannelResponse: BaiduChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BaiduChannelResponseTypeDef](./type_defs.md#baiduchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEmailTemplateResponseTypeDef

```python
# CreateEmailTemplateResponseTypeDef definition

class CreateEmailTemplateResponseTypeDef(TypedDict):
    CreateTemplateMessageBody: CreateTemplateMessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateTemplateMessageBodyTypeDef](./type_defs.md#createtemplatemessagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePushTemplateResponseTypeDef

```python
# CreatePushTemplateResponseTypeDef definition

class CreatePushTemplateResponseTypeDef(TypedDict):
    CreateTemplateMessageBody: CreateTemplateMessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateTemplateMessageBodyTypeDef](./type_defs.md#createtemplatemessagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSmsTemplateResponseTypeDef

```python
# CreateSmsTemplateResponseTypeDef definition

class CreateSmsTemplateResponseTypeDef(TypedDict):
    CreateTemplateMessageBody: CreateTemplateMessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateTemplateMessageBodyTypeDef](./type_defs.md#createtemplatemessagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateVoiceTemplateResponseTypeDef

```python
# CreateVoiceTemplateResponseTypeDef definition

class CreateVoiceTemplateResponseTypeDef(TypedDict):
    CreateTemplateMessageBody: CreateTemplateMessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CreateTemplateMessageBodyTypeDef](./type_defs.md#createtemplatemessagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExportJobRequestRequestTypeDef

```python
# CreateExportJobRequestRequestTypeDef definition

class CreateExportJobRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ExportJobRequest: ExportJobRequestTypeDef,  # (1)
```

1. See [:material-code-braces: ExportJobRequestTypeDef](./type_defs.md#exportjobrequesttypedef) 
## CreateImportJobRequestRequestTypeDef

```python
# CreateImportJobRequestRequestTypeDef definition

class CreateImportJobRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    ImportJobRequest: ImportJobRequestTypeDef,  # (1)
```

1. See [:material-code-braces: ImportJobRequestTypeDef](./type_defs.md#importjobrequesttypedef) 
## CreateInAppTemplateResponseTypeDef

```python
# CreateInAppTemplateResponseTypeDef definition

class CreateInAppTemplateResponseTypeDef(TypedDict):
    TemplateCreateMessageBody: TemplateCreateMessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateCreateMessageBodyTypeDef](./type_defs.md#templatecreatemessagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecommenderConfigurationRequestRequestTypeDef

```python
# CreateRecommenderConfigurationRequestRequestTypeDef definition

class CreateRecommenderConfigurationRequestRequestTypeDef(TypedDict):
    CreateRecommenderConfiguration: CreateRecommenderConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: CreateRecommenderConfigurationTypeDef](./type_defs.md#createrecommenderconfigurationtypedef) 
## CreateRecommenderConfigurationResponseTypeDef

```python
# CreateRecommenderConfigurationResponseTypeDef definition

class CreateRecommenderConfigurationResponseTypeDef(TypedDict):
    RecommenderConfigurationResponse: RecommenderConfigurationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommenderConfigurationResponseTypeDef](./type_defs.md#recommenderconfigurationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRecommenderConfigurationResponseTypeDef

```python
# DeleteRecommenderConfigurationResponseTypeDef definition

class DeleteRecommenderConfigurationResponseTypeDef(TypedDict):
    RecommenderConfigurationResponse: RecommenderConfigurationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommenderConfigurationResponseTypeDef](./type_defs.md#recommenderconfigurationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecommenderConfigurationResponseTypeDef

```python
# GetRecommenderConfigurationResponseTypeDef definition

class GetRecommenderConfigurationResponseTypeDef(TypedDict):
    RecommenderConfigurationResponse: RecommenderConfigurationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommenderConfigurationResponseTypeDef](./type_defs.md#recommenderconfigurationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecommenderConfigurationsResponseTypeDef

```python
# ListRecommenderConfigurationsResponseTypeDef definition

class ListRecommenderConfigurationsResponseTypeDef(TypedDict):
    Item: List[RecommenderConfigurationResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommenderConfigurationResponseTypeDef](./type_defs.md#recommenderconfigurationresponsetypedef) 
## UpdateRecommenderConfigurationResponseTypeDef

```python
# UpdateRecommenderConfigurationResponseTypeDef definition

class UpdateRecommenderConfigurationResponseTypeDef(TypedDict):
    RecommenderConfigurationResponse: RecommenderConfigurationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommenderConfigurationResponseTypeDef](./type_defs.md#recommenderconfigurationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSmsTemplateRequestRequestTypeDef

```python
# CreateSmsTemplateRequestRequestTypeDef definition

class CreateSmsTemplateRequestRequestTypeDef(TypedDict):
    SMSTemplateRequest: SMSTemplateRequestTypeDef,  # (1)
    TemplateName: str,
```

1. See [:material-code-braces: SMSTemplateRequestTypeDef](./type_defs.md#smstemplaterequesttypedef) 
## UpdateSmsTemplateRequestRequestTypeDef

```python
# UpdateSmsTemplateRequestRequestTypeDef definition

class UpdateSmsTemplateRequestRequestTypeDef(TypedDict):
    SMSTemplateRequest: SMSTemplateRequestTypeDef,  # (1)
    TemplateName: str,
    CreateNewVersion: NotRequired[bool],
    Version: NotRequired[str],
```

1. See [:material-code-braces: SMSTemplateRequestTypeDef](./type_defs.md#smstemplaterequesttypedef) 
## CreateVoiceTemplateRequestRequestTypeDef

```python
# CreateVoiceTemplateRequestRequestTypeDef definition

class CreateVoiceTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    VoiceTemplateRequest: VoiceTemplateRequestTypeDef,  # (1)
```

1. See [:material-code-braces: VoiceTemplateRequestTypeDef](./type_defs.md#voicetemplaterequesttypedef) 
## UpdateVoiceTemplateRequestRequestTypeDef

```python
# UpdateVoiceTemplateRequestRequestTypeDef definition

class UpdateVoiceTemplateRequestRequestTypeDef(TypedDict):
    TemplateName: str,
    VoiceTemplateRequest: VoiceTemplateRequestTypeDef,  # (1)
    CreateNewVersion: NotRequired[bool],
    Version: NotRequired[str],
```

1. See [:material-code-braces: VoiceTemplateRequestTypeDef](./type_defs.md#voicetemplaterequesttypedef) 
## CustomMessageActivityOutputTypeDef

```python
# CustomMessageActivityOutputTypeDef definition

class CustomMessageActivityOutputTypeDef(TypedDict):
    DeliveryUri: NotRequired[str],
    EndpointTypes: NotRequired[List[EndpointTypesElementType]],  # (1)
    MessageConfig: NotRequired[JourneyCustomMessageTypeDef],  # (2)
    NextActivity: NotRequired[str],
    TemplateName: NotRequired[str],
    TemplateVersion: NotRequired[str],
```

1. See [:material-code-brackets: EndpointTypesElementType](./literals.md#endpointtypeselementtype) 
2. See [:material-code-braces: JourneyCustomMessageTypeDef](./type_defs.md#journeycustommessagetypedef) 
## CustomMessageActivityTypeDef

```python
# CustomMessageActivityTypeDef definition

class CustomMessageActivityTypeDef(TypedDict):
    DeliveryUri: NotRequired[str],
    EndpointTypes: NotRequired[Sequence[EndpointTypesElementType]],  # (1)
    MessageConfig: NotRequired[JourneyCustomMessageTypeDef],  # (2)
    NextActivity: NotRequired[str],
    TemplateName: NotRequired[str],
    TemplateVersion: NotRequired[str],
```

1. See [:material-code-brackets: EndpointTypesElementType](./literals.md#endpointtypeselementtype) 
2. See [:material-code-braces: JourneyCustomMessageTypeDef](./type_defs.md#journeycustommessagetypedef) 
## PushNotificationTemplateRequestTypeDef

```python
# PushNotificationTemplateRequestTypeDef definition

class PushNotificationTemplateRequestTypeDef(TypedDict):
    ADM: NotRequired[AndroidPushNotificationTemplateTypeDef],  # (1)
    APNS: NotRequired[APNSPushNotificationTemplateTypeDef],  # (2)
    Baidu: NotRequired[AndroidPushNotificationTemplateTypeDef],  # (1)
    Default: NotRequired[DefaultPushNotificationTemplateTypeDef],  # (4)
    DefaultSubstitutions: NotRequired[str],
    GCM: NotRequired[AndroidPushNotificationTemplateTypeDef],  # (1)
    RecommenderId: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    TemplateDescription: NotRequired[str],
```

1. See [:material-code-braces: AndroidPushNotificationTemplateTypeDef](./type_defs.md#androidpushnotificationtemplatetypedef) 
2. See [:material-code-braces: APNSPushNotificationTemplateTypeDef](./type_defs.md#apnspushnotificationtemplatetypedef) 
3. See [:material-code-braces: AndroidPushNotificationTemplateTypeDef](./type_defs.md#androidpushnotificationtemplatetypedef) 
4. See [:material-code-braces: DefaultPushNotificationTemplateTypeDef](./type_defs.md#defaultpushnotificationtemplatetypedef) 
5. See [:material-code-braces: AndroidPushNotificationTemplateTypeDef](./type_defs.md#androidpushnotificationtemplatetypedef) 
## PushNotificationTemplateResponseTypeDef

```python
# PushNotificationTemplateResponseTypeDef definition

class PushNotificationTemplateResponseTypeDef(TypedDict):
    CreationDate: str,
    LastModifiedDate: str,
    TemplateName: str,
    TemplateType: TemplateTypeType,  # (6)
    ADM: NotRequired[AndroidPushNotificationTemplateTypeDef],  # (1)
    APNS: NotRequired[APNSPushNotificationTemplateTypeDef],  # (2)
    Arn: NotRequired[str],
    Baidu: NotRequired[AndroidPushNotificationTemplateTypeDef],  # (1)
    Default: NotRequired[DefaultPushNotificationTemplateTypeDef],  # (4)
    DefaultSubstitutions: NotRequired[str],
    GCM: NotRequired[AndroidPushNotificationTemplateTypeDef],  # (1)
    RecommenderId: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    TemplateDescription: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-braces: AndroidPushNotificationTemplateTypeDef](./type_defs.md#androidpushnotificationtemplatetypedef) 
2. See [:material-code-braces: APNSPushNotificationTemplateTypeDef](./type_defs.md#apnspushnotificationtemplatetypedef) 
3. See [:material-code-braces: AndroidPushNotificationTemplateTypeDef](./type_defs.md#androidpushnotificationtemplatetypedef) 
4. See [:material-code-braces: DefaultPushNotificationTemplateTypeDef](./type_defs.md#defaultpushnotificationtemplatetypedef) 
5. See [:material-code-braces: AndroidPushNotificationTemplateTypeDef](./type_defs.md#androidpushnotificationtemplatetypedef) 
6. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## DeleteEmailChannelResponseTypeDef

```python
# DeleteEmailChannelResponseTypeDef definition

class DeleteEmailChannelResponseTypeDef(TypedDict):
    EmailChannelResponse: EmailChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmailChannelResponseTypeDef](./type_defs.md#emailchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEmailChannelResponseTypeDef

```python
# GetEmailChannelResponseTypeDef definition

class GetEmailChannelResponseTypeDef(TypedDict):
    EmailChannelResponse: EmailChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmailChannelResponseTypeDef](./type_defs.md#emailchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEmailChannelResponseTypeDef

```python
# UpdateEmailChannelResponseTypeDef definition

class UpdateEmailChannelResponseTypeDef(TypedDict):
    EmailChannelResponse: EmailChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmailChannelResponseTypeDef](./type_defs.md#emailchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEmailTemplateResponseTypeDef

```python
# DeleteEmailTemplateResponseTypeDef definition

class DeleteEmailTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteInAppTemplateResponseTypeDef

```python
# DeleteInAppTemplateResponseTypeDef definition

class DeleteInAppTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePushTemplateResponseTypeDef

```python
# DeletePushTemplateResponseTypeDef definition

class DeletePushTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSmsTemplateResponseTypeDef

```python
# DeleteSmsTemplateResponseTypeDef definition

class DeleteSmsTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVoiceTemplateResponseTypeDef

```python
# DeleteVoiceTemplateResponseTypeDef definition

class DeleteVoiceTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEmailTemplateResponseTypeDef

```python
# UpdateEmailTemplateResponseTypeDef definition

class UpdateEmailTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEndpointResponseTypeDef

```python
# UpdateEndpointResponseTypeDef definition

class UpdateEndpointResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEndpointsBatchResponseTypeDef

```python
# UpdateEndpointsBatchResponseTypeDef definition

class UpdateEndpointsBatchResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateInAppTemplateResponseTypeDef

```python
# UpdateInAppTemplateResponseTypeDef definition

class UpdateInAppTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePushTemplateResponseTypeDef

```python
# UpdatePushTemplateResponseTypeDef definition

class UpdatePushTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSmsTemplateResponseTypeDef

```python
# UpdateSmsTemplateResponseTypeDef definition

class UpdateSmsTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplateActiveVersionResponseTypeDef

```python
# UpdateTemplateActiveVersionResponseTypeDef definition

class UpdateTemplateActiveVersionResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVoiceTemplateResponseTypeDef

```python
# UpdateVoiceTemplateResponseTypeDef definition

class UpdateVoiceTemplateResponseTypeDef(TypedDict):
    MessageBody: MessageBodyTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageBodyTypeDef](./type_defs.md#messagebodytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEventStreamResponseTypeDef

```python
# DeleteEventStreamResponseTypeDef definition

class DeleteEventStreamResponseTypeDef(TypedDict):
    EventStream: EventStreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventStreamTypeDef](./type_defs.md#eventstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEventStreamResponseTypeDef

```python
# GetEventStreamResponseTypeDef definition

class GetEventStreamResponseTypeDef(TypedDict):
    EventStream: EventStreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventStreamTypeDef](./type_defs.md#eventstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEventStreamResponseTypeDef

```python
# PutEventStreamResponseTypeDef definition

class PutEventStreamResponseTypeDef(TypedDict):
    EventStream: EventStreamTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventStreamTypeDef](./type_defs.md#eventstreamtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGcmChannelResponseTypeDef

```python
# DeleteGcmChannelResponseTypeDef definition

class DeleteGcmChannelResponseTypeDef(TypedDict):
    GCMChannelResponse: GCMChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GCMChannelResponseTypeDef](./type_defs.md#gcmchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGcmChannelResponseTypeDef

```python
# GetGcmChannelResponseTypeDef definition

class GetGcmChannelResponseTypeDef(TypedDict):
    GCMChannelResponse: GCMChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GCMChannelResponseTypeDef](./type_defs.md#gcmchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGcmChannelResponseTypeDef

```python
# UpdateGcmChannelResponseTypeDef definition

class UpdateGcmChannelResponseTypeDef(TypedDict):
    GCMChannelResponse: GCMChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GCMChannelResponseTypeDef](./type_defs.md#gcmchannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSmsChannelResponseTypeDef

```python
# DeleteSmsChannelResponseTypeDef definition

class DeleteSmsChannelResponseTypeDef(TypedDict):
    SMSChannelResponse: SMSChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SMSChannelResponseTypeDef](./type_defs.md#smschannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSmsChannelResponseTypeDef

```python
# GetSmsChannelResponseTypeDef definition

class GetSmsChannelResponseTypeDef(TypedDict):
    SMSChannelResponse: SMSChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SMSChannelResponseTypeDef](./type_defs.md#smschannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSmsChannelResponseTypeDef

```python
# UpdateSmsChannelResponseTypeDef definition

class UpdateSmsChannelResponseTypeDef(TypedDict):
    SMSChannelResponse: SMSChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SMSChannelResponseTypeDef](./type_defs.md#smschannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteVoiceChannelResponseTypeDef

```python
# DeleteVoiceChannelResponseTypeDef definition

class DeleteVoiceChannelResponseTypeDef(TypedDict):
    VoiceChannelResponse: VoiceChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceChannelResponseTypeDef](./type_defs.md#voicechannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceChannelResponseTypeDef

```python
# GetVoiceChannelResponseTypeDef definition

class GetVoiceChannelResponseTypeDef(TypedDict):
    VoiceChannelResponse: VoiceChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceChannelResponseTypeDef](./type_defs.md#voicechannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateVoiceChannelResponseTypeDef

```python
# UpdateVoiceChannelResponseTypeDef definition

class UpdateVoiceChannelResponseTypeDef(TypedDict):
    VoiceChannelResponse: VoiceChannelResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceChannelResponseTypeDef](./type_defs.md#voicechannelresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEmailChannelRequestRequestTypeDef

```python
# UpdateEmailChannelRequestRequestTypeDef definition

class UpdateEmailChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EmailChannelRequest: EmailChannelRequestTypeDef,  # (1)
```

1. See [:material-code-braces: EmailChannelRequestTypeDef](./type_defs.md#emailchannelrequesttypedef) 
## EmailMessageActivityTypeDef

```python
# EmailMessageActivityTypeDef definition

class EmailMessageActivityTypeDef(TypedDict):
    MessageConfig: NotRequired[JourneyEmailMessageTypeDef],  # (1)
    NextActivity: NotRequired[str],
    TemplateName: NotRequired[str],
    TemplateVersion: NotRequired[str],
```

1. See [:material-code-braces: JourneyEmailMessageTypeDef](./type_defs.md#journeyemailmessagetypedef) 
## SendUsersMessageResponseTypeDef

```python
# SendUsersMessageResponseTypeDef definition

class SendUsersMessageResponseTypeDef(TypedDict):
    ApplicationId: str,
    RequestId: NotRequired[str],
    Result: NotRequired[Dict[str, Dict[str, EndpointMessageResultTypeDef]]],  # (1)
```

1. See [:material-code-braces: EndpointMessageResultTypeDef](./type_defs.md#endpointmessageresulttypedef) 
## EndpointResponseTypeDef

```python
# EndpointResponseTypeDef definition

class EndpointResponseTypeDef(TypedDict):
    Address: NotRequired[str],
    ApplicationId: NotRequired[str],
    Attributes: NotRequired[Dict[str, List[str]]],
    ChannelType: NotRequired[ChannelTypeType],  # (1)
    CohortId: NotRequired[str],
    CreationDate: NotRequired[str],
    Demographic: NotRequired[EndpointDemographicTypeDef],  # (2)
    EffectiveDate: NotRequired[str],
    EndpointStatus: NotRequired[str],
    Id: NotRequired[str],
    Location: NotRequired[EndpointLocationTypeDef],  # (3)
    Metrics: NotRequired[Dict[str, float]],
    OptOut: NotRequired[str],
    RequestId: NotRequired[str],
    User: NotRequired[EndpointUserOutputTypeDef],  # (4)
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: EndpointDemographicTypeDef](./type_defs.md#endpointdemographictypedef) 
3. See [:material-code-braces: EndpointLocationTypeDef](./type_defs.md#endpointlocationtypedef) 
4. See [:material-code-braces: EndpointUserOutputTypeDef](./type_defs.md#endpointuseroutputtypedef) 
## EventDimensionsOutputTypeDef

```python
# EventDimensionsOutputTypeDef definition

class EventDimensionsOutputTypeDef(TypedDict):
    Attributes: NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],  # (1)
    EventType: NotRequired[SetDimensionOutputTypeDef],  # (2)
    Metrics: NotRequired[Dict[str, MetricDimensionTypeDef]],  # (3)
```

1. See [:material-code-braces: AttributeDimensionOutputTypeDef](./type_defs.md#attributedimensionoutputtypedef) 
2. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
3. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
## SegmentDemographicsOutputTypeDef

```python
# SegmentDemographicsOutputTypeDef definition

class SegmentDemographicsOutputTypeDef(TypedDict):
    AppVersion: NotRequired[SetDimensionOutputTypeDef],  # (1)
    Channel: NotRequired[SetDimensionOutputTypeDef],  # (1)
    DeviceType: NotRequired[SetDimensionOutputTypeDef],  # (1)
    Make: NotRequired[SetDimensionOutputTypeDef],  # (1)
    Model: NotRequired[SetDimensionOutputTypeDef],  # (1)
    Platform: NotRequired[SetDimensionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
2. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
3. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
4. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
5. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
6. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
## ItemResponseTypeDef

```python
# ItemResponseTypeDef definition

class ItemResponseTypeDef(TypedDict):
    EndpointItemResponse: NotRequired[EndpointItemResponseTypeDef],  # (1)
    EventsItemResponse: NotRequired[Dict[str, EventItemResponseTypeDef]],  # (2)
```

1. See [:material-code-braces: EndpointItemResponseTypeDef](./type_defs.md#endpointitemresponsetypedef) 
2. See [:material-code-braces: EventItemResponseTypeDef](./type_defs.md#eventitemresponsetypedef) 
## EventTypeDef

```python
# EventTypeDef definition

class EventTypeDef(TypedDict):
    EventType: str,
    Timestamp: str,
    AppPackageName: NotRequired[str],
    AppTitle: NotRequired[str],
    AppVersionCode: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    ClientSdkVersion: NotRequired[str],
    Metrics: NotRequired[Mapping[str, float]],
    SdkName: NotRequired[str],
    Session: NotRequired[SessionTypeDef],  # (1)
```

1. See [:material-code-braces: SessionTypeDef](./type_defs.md#sessiontypedef) 
## ExportJobResponseTypeDef

```python
# ExportJobResponseTypeDef definition

class ExportJobResponseTypeDef(TypedDict):
    ApplicationId: str,
    CreationDate: str,
    Definition: ExportJobResourceTypeDef,  # (1)
    Id: str,
    JobStatus: JobStatusType,  # (2)
    Type: str,
    CompletedPieces: NotRequired[int],
    CompletionDate: NotRequired[str],
    FailedPieces: NotRequired[int],
    Failures: NotRequired[List[str]],
    TotalFailures: NotRequired[int],
    TotalPieces: NotRequired[int],
    TotalProcessed: NotRequired[int],
```

1. See [:material-code-braces: ExportJobResourceTypeDef](./type_defs.md#exportjobresourcetypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## UpdateGcmChannelRequestRequestTypeDef

```python
# UpdateGcmChannelRequestRequestTypeDef definition

class UpdateGcmChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    GCMChannelRequest: GCMChannelRequestTypeDef,  # (1)
```

1. See [:material-code-braces: GCMChannelRequestTypeDef](./type_defs.md#gcmchannelrequesttypedef) 
## GPSPointDimensionTypeDef

```python
# GPSPointDimensionTypeDef definition

class GPSPointDimensionTypeDef(TypedDict):
    Coordinates: GPSCoordinatesTypeDef,  # (1)
    RangeInKilometers: NotRequired[float],
```

1. See [:material-code-braces: GPSCoordinatesTypeDef](./type_defs.md#gpscoordinatestypedef) 
## GetApplicationDateRangeKpiRequestRequestTypeDef

```python
# GetApplicationDateRangeKpiRequestRequestTypeDef definition

class GetApplicationDateRangeKpiRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    KpiName: str,
    EndTime: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
```

## GetCampaignDateRangeKpiRequestRequestTypeDef

```python
# GetCampaignDateRangeKpiRequestRequestTypeDef definition

class GetCampaignDateRangeKpiRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
    KpiName: str,
    EndTime: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
```

## GetJourneyDateRangeKpiRequestRequestTypeDef

```python
# GetJourneyDateRangeKpiRequestRequestTypeDef definition

class GetJourneyDateRangeKpiRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
    KpiName: str,
    EndTime: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    PageSize: NotRequired[str],
    StartTime: NotRequired[TimestampTypeDef],
```

## JourneyScheduleTypeDef

```python
# JourneyScheduleTypeDef definition

class JourneyScheduleTypeDef(TypedDict):
    EndTime: NotRequired[TimestampTypeDef],
    StartTime: NotRequired[TimestampTypeDef],
    Timezone: NotRequired[str],
```

## GetJourneyExecutionActivityMetricsResponseTypeDef

```python
# GetJourneyExecutionActivityMetricsResponseTypeDef definition

class GetJourneyExecutionActivityMetricsResponseTypeDef(TypedDict):
    JourneyExecutionActivityMetricsResponse: JourneyExecutionActivityMetricsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyExecutionActivityMetricsResponseTypeDef](./type_defs.md#journeyexecutionactivitymetricsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJourneyExecutionMetricsResponseTypeDef

```python
# GetJourneyExecutionMetricsResponseTypeDef definition

class GetJourneyExecutionMetricsResponseTypeDef(TypedDict):
    JourneyExecutionMetricsResponse: JourneyExecutionMetricsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyExecutionMetricsResponseTypeDef](./type_defs.md#journeyexecutionmetricsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJourneyRunExecutionActivityMetricsResponseTypeDef

```python
# GetJourneyRunExecutionActivityMetricsResponseTypeDef definition

class GetJourneyRunExecutionActivityMetricsResponseTypeDef(TypedDict):
    JourneyRunExecutionActivityMetricsResponse: JourneyRunExecutionActivityMetricsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyRunExecutionActivityMetricsResponseTypeDef](./type_defs.md#journeyrunexecutionactivitymetricsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJourneyRunExecutionMetricsResponseTypeDef

```python
# GetJourneyRunExecutionMetricsResponseTypeDef definition

class GetJourneyRunExecutionMetricsResponseTypeDef(TypedDict):
    JourneyRunExecutionMetricsResponse: JourneyRunExecutionMetricsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyRunExecutionMetricsResponseTypeDef](./type_defs.md#journeyrunexecutionmetricsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSmsTemplateResponseTypeDef

```python
# GetSmsTemplateResponseTypeDef definition

class GetSmsTemplateResponseTypeDef(TypedDict):
    SMSTemplateResponse: SMSTemplateResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SMSTemplateResponseTypeDef](./type_defs.md#smstemplateresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetVoiceTemplateResponseTypeDef

```python
# GetVoiceTemplateResponseTypeDef definition

class GetVoiceTemplateResponseTypeDef(TypedDict):
    VoiceTemplateResponse: VoiceTemplateResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VoiceTemplateResponseTypeDef](./type_defs.md#voicetemplateresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportJobResponseTypeDef

```python
# ImportJobResponseTypeDef definition

class ImportJobResponseTypeDef(TypedDict):
    ApplicationId: str,
    CreationDate: str,
    Definition: ImportJobResourceTypeDef,  # (1)
    Id: str,
    JobStatus: JobStatusType,  # (2)
    Type: str,
    CompletedPieces: NotRequired[int],
    CompletionDate: NotRequired[str],
    FailedPieces: NotRequired[int],
    Failures: NotRequired[List[str]],
    TotalFailures: NotRequired[int],
    TotalPieces: NotRequired[int],
    TotalProcessed: NotRequired[int],
```

1. See [:material-code-braces: ImportJobResourceTypeDef](./type_defs.md#importjobresourcetypedef) 
2. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## InAppMessageButtonTypeDef

```python
# InAppMessageButtonTypeDef definition

class InAppMessageButtonTypeDef(TypedDict):
    Android: NotRequired[OverrideButtonConfigurationTypeDef],  # (1)
    DefaultConfig: NotRequired[DefaultButtonConfigurationTypeDef],  # (2)
    IOS: NotRequired[OverrideButtonConfigurationTypeDef],  # (1)
    Web: NotRequired[OverrideButtonConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: OverrideButtonConfigurationTypeDef](./type_defs.md#overridebuttonconfigurationtypedef) 
2. See [:material-code-braces: DefaultButtonConfigurationTypeDef](./type_defs.md#defaultbuttonconfigurationtypedef) 
3. See [:material-code-braces: OverrideButtonConfigurationTypeDef](./type_defs.md#overridebuttonconfigurationtypedef) 
4. See [:material-code-braces: OverrideButtonConfigurationTypeDef](./type_defs.md#overridebuttonconfigurationtypedef) 
## PushMessageActivityTypeDef

```python
# PushMessageActivityTypeDef definition

class PushMessageActivityTypeDef(TypedDict):
    MessageConfig: NotRequired[JourneyPushMessageTypeDef],  # (1)
    NextActivity: NotRequired[str],
    TemplateName: NotRequired[str],
    TemplateVersion: NotRequired[str],
```

1. See [:material-code-braces: JourneyPushMessageTypeDef](./type_defs.md#journeypushmessagetypedef) 
## JourneyRunsResponseTypeDef

```python
# JourneyRunsResponseTypeDef definition

class JourneyRunsResponseTypeDef(TypedDict):
    Item: List[JourneyRunResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JourneyRunResponseTypeDef](./type_defs.md#journeyrunresponsetypedef) 
## SMSMessageActivityTypeDef

```python
# SMSMessageActivityTypeDef definition

class SMSMessageActivityTypeDef(TypedDict):
    MessageConfig: NotRequired[JourneySMSMessageTypeDef],  # (1)
    NextActivity: NotRequired[str],
    TemplateName: NotRequired[str],
    TemplateVersion: NotRequired[str],
```

1. See [:material-code-braces: JourneySMSMessageTypeDef](./type_defs.md#journeysmsmessagetypedef) 
## UpdateJourneyStateRequestRequestTypeDef

```python
# UpdateJourneyStateRequestRequestTypeDef definition

class UpdateJourneyStateRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
    JourneyStateRequest: JourneyStateRequestTypeDef,  # (1)
```

1. See [:material-code-braces: JourneyStateRequestTypeDef](./type_defs.md#journeystaterequesttypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    TagsModel: TagsModelOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagsModelOutputTypeDef](./type_defs.md#tagsmodeloutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MessageResponseTypeDef

```python
# MessageResponseTypeDef definition

class MessageResponseTypeDef(TypedDict):
    ApplicationId: str,
    EndpointResult: NotRequired[Dict[str, EndpointMessageResultTypeDef]],  # (1)
    RequestId: NotRequired[str],
    Result: NotRequired[Dict[str, MessageResultTypeDef]],  # (2)
```

1. See [:material-code-braces: EndpointMessageResultTypeDef](./type_defs.md#endpointmessageresulttypedef) 
2. See [:material-code-braces: MessageResultTypeDef](./type_defs.md#messageresulttypedef) 
## PhoneNumberValidateRequestRequestTypeDef

```python
# PhoneNumberValidateRequestRequestTypeDef definition

class PhoneNumberValidateRequestRequestTypeDef(TypedDict):
    NumberValidateRequest: NumberValidateRequestTypeDef,  # (1)
```

1. See [:material-code-braces: NumberValidateRequestTypeDef](./type_defs.md#numbervalidaterequesttypedef) 
## PhoneNumberValidateResponseTypeDef

```python
# PhoneNumberValidateResponseTypeDef definition

class PhoneNumberValidateResponseTypeDef(TypedDict):
    NumberValidateResponse: NumberValidateResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NumberValidateResponseTypeDef](./type_defs.md#numbervalidateresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OpenHoursOutputTypeDef

```python
# OpenHoursOutputTypeDef definition

class OpenHoursOutputTypeDef(TypedDict):
    EMAIL: NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],  # (1)
    SMS: NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],  # (1)
    PUSH: NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],  # (1)
    VOICE: NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],  # (1)
    CUSTOM: NotRequired[Dict[DayOfWeekType, List[OpenHoursRuleTypeDef]]],  # (1)
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
3. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
4. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
5. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
## OpenHoursTypeDef

```python
# OpenHoursTypeDef definition

class OpenHoursTypeDef(TypedDict):
    EMAIL: NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],  # (1)
    SMS: NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],  # (1)
    PUSH: NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],  # (1)
    VOICE: NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],  # (1)
    CUSTOM: NotRequired[Mapping[DayOfWeekType, Sequence[OpenHoursRuleTypeDef]]],  # (1)
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
2. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
3. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
4. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
5. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: OpenHoursRuleTypeDef](./type_defs.md#openhoursruletypedef) 
## PutEventStreamRequestRequestTypeDef

```python
# PutEventStreamRequestRequestTypeDef definition

class PutEventStreamRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    WriteEventStream: WriteEventStreamTypeDef,  # (1)
```

1. See [:material-code-braces: WriteEventStreamTypeDef](./type_defs.md#writeeventstreamtypedef) 
## RandomSplitActivityOutputTypeDef

```python
# RandomSplitActivityOutputTypeDef definition

class RandomSplitActivityOutputTypeDef(TypedDict):
    Branches: NotRequired[List[RandomSplitEntryTypeDef]],  # (1)
```

1. See [:material-code-braces: RandomSplitEntryTypeDef](./type_defs.md#randomsplitentrytypedef) 
## RandomSplitActivityTypeDef

```python
# RandomSplitActivityTypeDef definition

class RandomSplitActivityTypeDef(TypedDict):
    Branches: NotRequired[Sequence[RandomSplitEntryTypeDef]],  # (1)
```

1. See [:material-code-braces: RandomSplitEntryTypeDef](./type_defs.md#randomsplitentrytypedef) 
## SegmentBehaviorsTypeDef

```python
# SegmentBehaviorsTypeDef definition

class SegmentBehaviorsTypeDef(TypedDict):
    Recency: NotRequired[RecencyDimensionTypeDef],  # (1)
```

1. See [:material-code-braces: RecencyDimensionTypeDef](./type_defs.md#recencydimensiontypedef) 
## RemoveAttributesRequestRequestTypeDef

```python
# RemoveAttributesRequestRequestTypeDef definition

class RemoveAttributesRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    AttributeType: str,
    UpdateAttributesRequest: UpdateAttributesRequestTypeDef,  # (1)
```

1. See [:material-code-braces: UpdateAttributesRequestTypeDef](./type_defs.md#updateattributesrequesttypedef) 
## ResultRowTypeDef

```python
# ResultRowTypeDef definition

class ResultRowTypeDef(TypedDict):
    GroupedBys: List[ResultRowValueTypeDef],  # (1)
    Values: List[ResultRowValueTypeDef],  # (1)
```

1. See [:material-code-braces: ResultRowValueTypeDef](./type_defs.md#resultrowvaluetypedef) 
2. See [:material-code-braces: ResultRowValueTypeDef](./type_defs.md#resultrowvaluetypedef) 
## UpdateSmsChannelRequestRequestTypeDef

```python
# UpdateSmsChannelRequestRequestTypeDef definition

class UpdateSmsChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SMSChannelRequest: SMSChannelRequestTypeDef,  # (1)
```

1. See [:material-code-braces: SMSChannelRequestTypeDef](./type_defs.md#smschannelrequesttypedef) 
## SendOTPMessageRequestRequestTypeDef

```python
# SendOTPMessageRequestRequestTypeDef definition

class SendOTPMessageRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SendOTPMessageRequestParameters: SendOTPMessageRequestParametersTypeDef,  # (1)
```

1. See [:material-code-braces: SendOTPMessageRequestParametersTypeDef](./type_defs.md#sendotpmessagerequestparameterstypedef) 
## SimpleEmailTypeDef

```python
# SimpleEmailTypeDef definition

class SimpleEmailTypeDef(TypedDict):
    HtmlPart: NotRequired[SimpleEmailPartTypeDef],  # (1)
    Subject: NotRequired[SimpleEmailPartTypeDef],  # (1)
    TextPart: NotRequired[SimpleEmailPartTypeDef],  # (1)
    Headers: NotRequired[Sequence[MessageHeaderTypeDef]],  # (4)
```

1. See [:material-code-braces: SimpleEmailPartTypeDef](./type_defs.md#simpleemailparttypedef) 
2. See [:material-code-braces: SimpleEmailPartTypeDef](./type_defs.md#simpleemailparttypedef) 
3. See [:material-code-braces: SimpleEmailPartTypeDef](./type_defs.md#simpleemailparttypedef) 
4. See [:material-code-braces: MessageHeaderTypeDef](./type_defs.md#messageheadertypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagsModel: TagsModelTypeDef,  # (1)
```

1. See [:material-code-braces: TagsModelTypeDef](./type_defs.md#tagsmodeltypedef) 
## UpdateTemplateActiveVersionRequestRequestTypeDef

```python
# UpdateTemplateActiveVersionRequestRequestTypeDef definition

class UpdateTemplateActiveVersionRequestRequestTypeDef(TypedDict):
    TemplateActiveVersionRequest: TemplateActiveVersionRequestTypeDef,  # (1)
    TemplateName: str,
    TemplateType: str,
```

1. See [:material-code-braces: TemplateActiveVersionRequestTypeDef](./type_defs.md#templateactiveversionrequesttypedef) 
## TemplateConfigurationTypeDef

```python
# TemplateConfigurationTypeDef definition

class TemplateConfigurationTypeDef(TypedDict):
    EmailTemplate: NotRequired[TemplateTypeDef],  # (1)
    PushTemplate: NotRequired[TemplateTypeDef],  # (1)
    SMSTemplate: NotRequired[TemplateTypeDef],  # (1)
    VoiceTemplate: NotRequired[TemplateTypeDef],  # (1)
    InAppTemplate: NotRequired[TemplateTypeDef],  # (1)
```

1. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
2. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
3. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
4. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
5. See [:material-code-braces: TemplateTypeDef](./type_defs.md#templatetypedef) 
## TemplatesResponseTypeDef

```python
# TemplatesResponseTypeDef definition

class TemplatesResponseTypeDef(TypedDict):
    Item: List[TemplateResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateResponseTypeDef](./type_defs.md#templateresponsetypedef) 
## TemplateVersionsResponseTypeDef

```python
# TemplateVersionsResponseTypeDef definition

class TemplateVersionsResponseTypeDef(TypedDict):
    Item: List[TemplateVersionResponseTypeDef],  # (1)
    Message: NotRequired[str],
    NextToken: NotRequired[str],
    RequestID: NotRequired[str],
```

1. See [:material-code-braces: TemplateVersionResponseTypeDef](./type_defs.md#templateversionresponsetypedef) 
## UpdateRecommenderConfigurationRequestRequestTypeDef

```python
# UpdateRecommenderConfigurationRequestRequestTypeDef definition

class UpdateRecommenderConfigurationRequestRequestTypeDef(TypedDict):
    RecommenderId: str,
    UpdateRecommenderConfiguration: UpdateRecommenderConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: UpdateRecommenderConfigurationTypeDef](./type_defs.md#updaterecommenderconfigurationtypedef) 
## UpdateVoiceChannelRequestRequestTypeDef

```python
# UpdateVoiceChannelRequestRequestTypeDef definition

class UpdateVoiceChannelRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    VoiceChannelRequest: VoiceChannelRequestTypeDef,  # (1)
```

1. See [:material-code-braces: VoiceChannelRequestTypeDef](./type_defs.md#voicechannelrequesttypedef) 
## VerifyOTPMessageResponseTypeDef

```python
# VerifyOTPMessageResponseTypeDef definition

class VerifyOTPMessageResponseTypeDef(TypedDict):
    VerificationResponse: VerificationResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: VerificationResponseTypeDef](./type_defs.md#verificationresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VerifyOTPMessageRequestRequestTypeDef

```python
# VerifyOTPMessageRequestRequestTypeDef definition

class VerifyOTPMessageRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    VerifyOTPMessageRequestParameters: VerifyOTPMessageRequestParametersTypeDef,  # (1)
```

1. See [:material-code-braces: VerifyOTPMessageRequestParametersTypeDef](./type_defs.md#verifyotpmessagerequestparameterstypedef) 
## GetCampaignActivitiesResponseTypeDef

```python
# GetCampaignActivitiesResponseTypeDef definition

class GetCampaignActivitiesResponseTypeDef(TypedDict):
    ActivitiesResponse: ActivitiesResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActivitiesResponseTypeDef](./type_defs.md#activitiesresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppsResponseTypeDef

```python
# GetAppsResponseTypeDef definition

class GetAppsResponseTypeDef(TypedDict):
    ApplicationsResponse: ApplicationsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationsResponseTypeDef](./type_defs.md#applicationsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ApplicationSettingsResourceTypeDef

```python
# ApplicationSettingsResourceTypeDef definition

class ApplicationSettingsResourceTypeDef(TypedDict):
    ApplicationId: str,
    CampaignHook: NotRequired[CampaignHookTypeDef],  # (1)
    LastModifiedDate: NotRequired[str],
    Limits: NotRequired[CampaignLimitsTypeDef],  # (2)
    QuietTime: NotRequired[QuietTimeTypeDef],  # (3)
    JourneyLimits: NotRequired[ApplicationSettingsJourneyLimitsTypeDef],  # (4)
```

1. See [:material-code-braces: CampaignHookTypeDef](./type_defs.md#campaignhooktypedef) 
2. See [:material-code-braces: CampaignLimitsTypeDef](./type_defs.md#campaignlimitstypedef) 
3. See [:material-code-braces: QuietTimeTypeDef](./type_defs.md#quiettimetypedef) 
4. See [:material-code-braces: ApplicationSettingsJourneyLimitsTypeDef](./type_defs.md#applicationsettingsjourneylimitstypedef) 
## WriteApplicationSettingsRequestTypeDef

```python
# WriteApplicationSettingsRequestTypeDef definition

class WriteApplicationSettingsRequestTypeDef(TypedDict):
    CampaignHook: NotRequired[CampaignHookTypeDef],  # (1)
    CloudWatchMetricsEnabled: NotRequired[bool],
    EventTaggingEnabled: NotRequired[bool],
    Limits: NotRequired[CampaignLimitsTypeDef],  # (2)
    QuietTime: NotRequired[QuietTimeTypeDef],  # (3)
    JourneyLimits: NotRequired[ApplicationSettingsJourneyLimitsTypeDef],  # (4)
```

1. See [:material-code-braces: CampaignHookTypeDef](./type_defs.md#campaignhooktypedef) 
2. See [:material-code-braces: CampaignLimitsTypeDef](./type_defs.md#campaignlimitstypedef) 
3. See [:material-code-braces: QuietTimeTypeDef](./type_defs.md#quiettimetypedef) 
4. See [:material-code-braces: ApplicationSettingsJourneyLimitsTypeDef](./type_defs.md#applicationsettingsjourneylimitstypedef) 
## CreateEmailTemplateRequestRequestTypeDef

```python
# CreateEmailTemplateRequestRequestTypeDef definition

class CreateEmailTemplateRequestRequestTypeDef(TypedDict):
    EmailTemplateRequest: EmailTemplateRequestTypeDef,  # (1)
    TemplateName: str,
```

1. See [:material-code-braces: EmailTemplateRequestTypeDef](./type_defs.md#emailtemplaterequesttypedef) 
## UpdateEmailTemplateRequestRequestTypeDef

```python
# UpdateEmailTemplateRequestRequestTypeDef definition

class UpdateEmailTemplateRequestRequestTypeDef(TypedDict):
    EmailTemplateRequest: EmailTemplateRequestTypeDef,  # (1)
    TemplateName: str,
    CreateNewVersion: NotRequired[bool],
    Version: NotRequired[str],
```

1. See [:material-code-braces: EmailTemplateRequestTypeDef](./type_defs.md#emailtemplaterequesttypedef) 
## GetEmailTemplateResponseTypeDef

```python
# GetEmailTemplateResponseTypeDef definition

class GetEmailTemplateResponseTypeDef(TypedDict):
    EmailTemplateResponse: EmailTemplateResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmailTemplateResponseTypeDef](./type_defs.md#emailtemplateresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetChannelsResponseTypeDef

```python
# GetChannelsResponseTypeDef definition

class GetChannelsResponseTypeDef(TypedDict):
    ChannelsResponse: ChannelsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ChannelsResponseTypeDef](./type_defs.md#channelsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecommenderConfigurationsResponseTypeDef

```python
# GetRecommenderConfigurationsResponseTypeDef definition

class GetRecommenderConfigurationsResponseTypeDef(TypedDict):
    ListRecommenderConfigurationsResponse: ListRecommenderConfigurationsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListRecommenderConfigurationsResponseTypeDef](./type_defs.md#listrecommenderconfigurationsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePushTemplateRequestRequestTypeDef

```python
# CreatePushTemplateRequestRequestTypeDef definition

class CreatePushTemplateRequestRequestTypeDef(TypedDict):
    PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,  # (1)
    TemplateName: str,
```

1. See [:material-code-braces: PushNotificationTemplateRequestTypeDef](./type_defs.md#pushnotificationtemplaterequesttypedef) 
## UpdatePushTemplateRequestRequestTypeDef

```python
# UpdatePushTemplateRequestRequestTypeDef definition

class UpdatePushTemplateRequestRequestTypeDef(TypedDict):
    PushNotificationTemplateRequest: PushNotificationTemplateRequestTypeDef,  # (1)
    TemplateName: str,
    CreateNewVersion: NotRequired[bool],
    Version: NotRequired[str],
```

1. See [:material-code-braces: PushNotificationTemplateRequestTypeDef](./type_defs.md#pushnotificationtemplaterequesttypedef) 
## GetPushTemplateResponseTypeDef

```python
# GetPushTemplateResponseTypeDef definition

class GetPushTemplateResponseTypeDef(TypedDict):
    PushNotificationTemplateResponse: PushNotificationTemplateResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PushNotificationTemplateResponseTypeDef](./type_defs.md#pushnotificationtemplateresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendUsersMessagesResponseTypeDef

```python
# SendUsersMessagesResponseTypeDef definition

class SendUsersMessagesResponseTypeDef(TypedDict):
    SendUsersMessageResponse: SendUsersMessageResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SendUsersMessageResponseTypeDef](./type_defs.md#sendusersmessageresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEndpointResponseTypeDef

```python
# DeleteEndpointResponseTypeDef definition

class DeleteEndpointResponseTypeDef(TypedDict):
    EndpointResponse: EndpointResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointResponseTypeDef](./type_defs.md#endpointresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointsResponseTypeDef

```python
# EndpointsResponseTypeDef definition

class EndpointsResponseTypeDef(TypedDict):
    Item: List[EndpointResponseTypeDef],  # (1)
```

1. See [:material-code-braces: EndpointResponseTypeDef](./type_defs.md#endpointresponsetypedef) 
## GetEndpointResponseTypeDef

```python
# GetEndpointResponseTypeDef definition

class GetEndpointResponseTypeDef(TypedDict):
    EndpointResponse: EndpointResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointResponseTypeDef](./type_defs.md#endpointresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointBatchItemTypeDef

```python
# EndpointBatchItemTypeDef definition

class EndpointBatchItemTypeDef(TypedDict):
    Address: NotRequired[str],
    Attributes: NotRequired[Mapping[str, Sequence[str]]],
    ChannelType: NotRequired[ChannelTypeType],  # (1)
    Demographic: NotRequired[EndpointDemographicTypeDef],  # (2)
    EffectiveDate: NotRequired[str],
    EndpointStatus: NotRequired[str],
    Id: NotRequired[str],
    Location: NotRequired[EndpointLocationTypeDef],  # (3)
    Metrics: NotRequired[Mapping[str, float]],
    OptOut: NotRequired[str],
    RequestId: NotRequired[str],
    User: NotRequired[EndpointUserUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: EndpointDemographicTypeDef](./type_defs.md#endpointdemographictypedef) 
3. See [:material-code-braces: EndpointLocationTypeDef](./type_defs.md#endpointlocationtypedef) 
4. See [:material-code-braces: EndpointUserTypeDef](./type_defs.md#endpointusertypedef) [:material-code-braces: EndpointUserOutputTypeDef](./type_defs.md#endpointuseroutputtypedef) 
## EndpointRequestTypeDef

```python
# EndpointRequestTypeDef definition

class EndpointRequestTypeDef(TypedDict):
    Address: NotRequired[str],
    Attributes: NotRequired[Mapping[str, Sequence[str]]],
    ChannelType: NotRequired[ChannelTypeType],  # (1)
    Demographic: NotRequired[EndpointDemographicTypeDef],  # (2)
    EffectiveDate: NotRequired[str],
    EndpointStatus: NotRequired[str],
    Location: NotRequired[EndpointLocationTypeDef],  # (3)
    Metrics: NotRequired[Mapping[str, float]],
    OptOut: NotRequired[str],
    RequestId: NotRequired[str],
    User: NotRequired[EndpointUserUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: EndpointDemographicTypeDef](./type_defs.md#endpointdemographictypedef) 
3. See [:material-code-braces: EndpointLocationTypeDef](./type_defs.md#endpointlocationtypedef) 
4. See [:material-code-braces: EndpointUserTypeDef](./type_defs.md#endpointusertypedef) [:material-code-braces: EndpointUserOutputTypeDef](./type_defs.md#endpointuseroutputtypedef) 
## PublicEndpointTypeDef

```python
# PublicEndpointTypeDef definition

class PublicEndpointTypeDef(TypedDict):
    Address: NotRequired[str],
    Attributes: NotRequired[Mapping[str, Sequence[str]]],
    ChannelType: NotRequired[ChannelTypeType],  # (1)
    Demographic: NotRequired[EndpointDemographicTypeDef],  # (2)
    EffectiveDate: NotRequired[str],
    EndpointStatus: NotRequired[str],
    Location: NotRequired[EndpointLocationTypeDef],  # (3)
    Metrics: NotRequired[Mapping[str, float]],
    OptOut: NotRequired[str],
    RequestId: NotRequired[str],
    User: NotRequired[EndpointUserUnionTypeDef],  # (4)
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: EndpointDemographicTypeDef](./type_defs.md#endpointdemographictypedef) 
3. See [:material-code-braces: EndpointLocationTypeDef](./type_defs.md#endpointlocationtypedef) 
4. See [:material-code-braces: EndpointUserTypeDef](./type_defs.md#endpointusertypedef) [:material-code-braces: EndpointUserOutputTypeDef](./type_defs.md#endpointuseroutputtypedef) 
## CampaignEventFilterOutputTypeDef

```python
# CampaignEventFilterOutputTypeDef definition

class CampaignEventFilterOutputTypeDef(TypedDict):
    Dimensions: EventDimensionsOutputTypeDef,  # (1)
    FilterType: FilterTypeType,  # (2)
```

1. See [:material-code-braces: EventDimensionsOutputTypeDef](./type_defs.md#eventdimensionsoutputtypedef) 
2. See [:material-code-brackets: FilterTypeType](./literals.md#filtertypetype) 
## EventConditionOutputTypeDef

```python
# EventConditionOutputTypeDef definition

class EventConditionOutputTypeDef(TypedDict):
    Dimensions: NotRequired[EventDimensionsOutputTypeDef],  # (1)
    MessageActivity: NotRequired[str],
```

1. See [:material-code-braces: EventDimensionsOutputTypeDef](./type_defs.md#eventdimensionsoutputtypedef) 
## EventFilterOutputTypeDef

```python
# EventFilterOutputTypeDef definition

class EventFilterOutputTypeDef(TypedDict):
    Dimensions: EventDimensionsOutputTypeDef,  # (1)
    FilterType: FilterTypeType,  # (2)
```

1. See [:material-code-braces: EventDimensionsOutputTypeDef](./type_defs.md#eventdimensionsoutputtypedef) 
2. See [:material-code-brackets: FilterTypeType](./literals.md#filtertypetype) 
## EventsResponseTypeDef

```python
# EventsResponseTypeDef definition

class EventsResponseTypeDef(TypedDict):
    Results: NotRequired[Dict[str, ItemResponseTypeDef]],  # (1)
```

1. See [:material-code-braces: ItemResponseTypeDef](./type_defs.md#itemresponsetypedef) 
## CreateExportJobResponseTypeDef

```python
# CreateExportJobResponseTypeDef definition

class CreateExportJobResponseTypeDef(TypedDict):
    ExportJobResponse: ExportJobResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportJobResponseTypeDef](./type_defs.md#exportjobresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExportJobsResponseTypeDef

```python
# ExportJobsResponseTypeDef definition

class ExportJobsResponseTypeDef(TypedDict):
    Item: List[ExportJobResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExportJobResponseTypeDef](./type_defs.md#exportjobresponsetypedef) 
## GetExportJobResponseTypeDef

```python
# GetExportJobResponseTypeDef definition

class GetExportJobResponseTypeDef(TypedDict):
    ExportJobResponse: ExportJobResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportJobResponseTypeDef](./type_defs.md#exportjobresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SegmentLocationOutputTypeDef

```python
# SegmentLocationOutputTypeDef definition

class SegmentLocationOutputTypeDef(TypedDict):
    Country: NotRequired[SetDimensionOutputTypeDef],  # (1)
    GPSPoint: NotRequired[GPSPointDimensionTypeDef],  # (2)
```

1. See [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
2. See [:material-code-braces: GPSPointDimensionTypeDef](./type_defs.md#gpspointdimensiontypedef) 
## CreateImportJobResponseTypeDef

```python
# CreateImportJobResponseTypeDef definition

class CreateImportJobResponseTypeDef(TypedDict):
    ImportJobResponse: ImportJobResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportJobResponseTypeDef](./type_defs.md#importjobresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetImportJobResponseTypeDef

```python
# GetImportJobResponseTypeDef definition

class GetImportJobResponseTypeDef(TypedDict):
    ImportJobResponse: ImportJobResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportJobResponseTypeDef](./type_defs.md#importjobresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportJobsResponseTypeDef

```python
# ImportJobsResponseTypeDef definition

class ImportJobsResponseTypeDef(TypedDict):
    Item: List[ImportJobResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ImportJobResponseTypeDef](./type_defs.md#importjobresponsetypedef) 
## InAppMessageContentTypeDef

```python
# InAppMessageContentTypeDef definition

class InAppMessageContentTypeDef(TypedDict):
    BackgroundColor: NotRequired[str],
    BodyConfig: NotRequired[InAppMessageBodyConfigTypeDef],  # (1)
    HeaderConfig: NotRequired[InAppMessageHeaderConfigTypeDef],  # (2)
    ImageUrl: NotRequired[str],
    PrimaryBtn: NotRequired[InAppMessageButtonTypeDef],  # (3)
    SecondaryBtn: NotRequired[InAppMessageButtonTypeDef],  # (3)
```

1. See [:material-code-braces: InAppMessageBodyConfigTypeDef](./type_defs.md#inappmessagebodyconfigtypedef) 
2. See [:material-code-braces: InAppMessageHeaderConfigTypeDef](./type_defs.md#inappmessageheaderconfigtypedef) 
3. See [:material-code-braces: InAppMessageButtonTypeDef](./type_defs.md#inappmessagebuttontypedef) 
4. See [:material-code-braces: InAppMessageButtonTypeDef](./type_defs.md#inappmessagebuttontypedef) 
## GetJourneyRunsResponseTypeDef

```python
# GetJourneyRunsResponseTypeDef definition

class GetJourneyRunsResponseTypeDef(TypedDict):
    JourneyRunsResponse: JourneyRunsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyRunsResponseTypeDef](./type_defs.md#journeyrunsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendMessagesResponseTypeDef

```python
# SendMessagesResponseTypeDef definition

class SendMessagesResponseTypeDef(TypedDict):
    MessageResponse: MessageResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageResponseTypeDef](./type_defs.md#messageresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SendOTPMessageResponseTypeDef

```python
# SendOTPMessageResponseTypeDef definition

class SendOTPMessageResponseTypeDef(TypedDict):
    MessageResponse: MessageResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: MessageResponseTypeDef](./type_defs.md#messageresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BaseKpiResultTypeDef

```python
# BaseKpiResultTypeDef definition

class BaseKpiResultTypeDef(TypedDict):
    Rows: List[ResultRowTypeDef],  # (1)
```

1. See [:material-code-braces: ResultRowTypeDef](./type_defs.md#resultrowtypedef) 
## EventDimensionsTypeDef

```python
# EventDimensionsTypeDef definition

class EventDimensionsTypeDef(TypedDict):
    Attributes: NotRequired[Mapping[str, AttributeDimensionUnionTypeDef]],  # (1)
    EventType: NotRequired[SetDimensionUnionTypeDef],  # (2)
    Metrics: NotRequired[Mapping[str, MetricDimensionTypeDef]],  # (3)
```

1. See [:material-code-braces: AttributeDimensionTypeDef](./type_defs.md#attributedimensiontypedef) [:material-code-braces: AttributeDimensionOutputTypeDef](./type_defs.md#attributedimensionoutputtypedef) 
2. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
3. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
## SegmentDemographicsTypeDef

```python
# SegmentDemographicsTypeDef definition

class SegmentDemographicsTypeDef(TypedDict):
    AppVersion: NotRequired[SetDimensionUnionTypeDef],  # (1)
    Channel: NotRequired[SetDimensionUnionTypeDef],  # (1)
    DeviceType: NotRequired[SetDimensionUnionTypeDef],  # (1)
    Make: NotRequired[SetDimensionUnionTypeDef],  # (1)
    Model: NotRequired[SetDimensionUnionTypeDef],  # (1)
    Platform: NotRequired[SetDimensionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
2. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
3. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
4. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
5. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
6. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
## SegmentLocationTypeDef

```python
# SegmentLocationTypeDef definition

class SegmentLocationTypeDef(TypedDict):
    Country: NotRequired[SetDimensionUnionTypeDef],  # (1)
    GPSPoint: NotRequired[GPSPointDimensionTypeDef],  # (2)
```

1. See [:material-code-braces: SetDimensionTypeDef](./type_defs.md#setdimensiontypedef) [:material-code-braces: SetDimensionOutputTypeDef](./type_defs.md#setdimensionoutputtypedef) 
2. See [:material-code-braces: GPSPointDimensionTypeDef](./type_defs.md#gpspointdimensiontypedef) 
## EmailMessageTypeDef

```python
# EmailMessageTypeDef definition

class EmailMessageTypeDef(TypedDict):
    Body: NotRequired[str],
    FeedbackForwardingAddress: NotRequired[str],
    FromAddress: NotRequired[str],
    RawEmail: NotRequired[RawEmailTypeDef],  # (1)
    ReplyToAddresses: NotRequired[Sequence[str]],
    SimpleEmail: NotRequired[SimpleEmailTypeDef],  # (2)
    Substitutions: NotRequired[Mapping[str, Sequence[str]]],
```

1. See [:material-code-braces: RawEmailTypeDef](./type_defs.md#rawemailtypedef) 
2. See [:material-code-braces: SimpleEmailTypeDef](./type_defs.md#simpleemailtypedef) 
## ListTemplatesResponseTypeDef

```python
# ListTemplatesResponseTypeDef definition

class ListTemplatesResponseTypeDef(TypedDict):
    TemplatesResponse: TemplatesResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplatesResponseTypeDef](./type_defs.md#templatesresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplateVersionsResponseTypeDef

```python
# ListTemplateVersionsResponseTypeDef definition

class ListTemplateVersionsResponseTypeDef(TypedDict):
    TemplateVersionsResponse: TemplateVersionsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateVersionsResponseTypeDef](./type_defs.md#templateversionsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationSettingsResponseTypeDef

```python
# GetApplicationSettingsResponseTypeDef definition

class GetApplicationSettingsResponseTypeDef(TypedDict):
    ApplicationSettingsResource: ApplicationSettingsResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationSettingsResourceTypeDef](./type_defs.md#applicationsettingsresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationSettingsResponseTypeDef

```python
# UpdateApplicationSettingsResponseTypeDef definition

class UpdateApplicationSettingsResponseTypeDef(TypedDict):
    ApplicationSettingsResource: ApplicationSettingsResourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationSettingsResourceTypeDef](./type_defs.md#applicationsettingsresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateApplicationSettingsRequestRequestTypeDef

```python
# UpdateApplicationSettingsRequestRequestTypeDef definition

class UpdateApplicationSettingsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    WriteApplicationSettingsRequest: WriteApplicationSettingsRequestTypeDef,  # (1)
```

1. See [:material-code-braces: WriteApplicationSettingsRequestTypeDef](./type_defs.md#writeapplicationsettingsrequesttypedef) 
## DeleteUserEndpointsResponseTypeDef

```python
# DeleteUserEndpointsResponseTypeDef definition

class DeleteUserEndpointsResponseTypeDef(TypedDict):
    EndpointsResponse: EndpointsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointsResponseTypeDef](./type_defs.md#endpointsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserEndpointsResponseTypeDef

```python
# GetUserEndpointsResponseTypeDef definition

class GetUserEndpointsResponseTypeDef(TypedDict):
    EndpointsResponse: EndpointsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointsResponseTypeDef](./type_defs.md#endpointsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointBatchRequestTypeDef

```python
# EndpointBatchRequestTypeDef definition

class EndpointBatchRequestTypeDef(TypedDict):
    Item: Sequence[EndpointBatchItemTypeDef],  # (1)
```

1. See [:material-code-braces: EndpointBatchItemTypeDef](./type_defs.md#endpointbatchitemtypedef) 
## UpdateEndpointRequestRequestTypeDef

```python
# UpdateEndpointRequestRequestTypeDef definition

class UpdateEndpointRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EndpointId: str,
    EndpointRequest: EndpointRequestTypeDef,  # (1)
```

1. See [:material-code-braces: EndpointRequestTypeDef](./type_defs.md#endpointrequesttypedef) 
## EventsBatchTypeDef

```python
# EventsBatchTypeDef definition

class EventsBatchTypeDef(TypedDict):
    Endpoint: PublicEndpointTypeDef,  # (1)
    Events: Mapping[str, EventTypeDef],  # (2)
```

1. See [:material-code-braces: PublicEndpointTypeDef](./type_defs.md#publicendpointtypedef) 
2. See [:material-code-braces: EventTypeDef](./type_defs.md#eventtypedef) 
## InAppCampaignScheduleTypeDef

```python
# InAppCampaignScheduleTypeDef definition

class InAppCampaignScheduleTypeDef(TypedDict):
    EndDate: NotRequired[str],
    EventFilter: NotRequired[CampaignEventFilterOutputTypeDef],  # (1)
    QuietTime: NotRequired[QuietTimeTypeDef],  # (2)
```

1. See [:material-code-braces: CampaignEventFilterOutputTypeDef](./type_defs.md#campaigneventfilteroutputtypedef) 
2. See [:material-code-braces: QuietTimeTypeDef](./type_defs.md#quiettimetypedef) 
## ScheduleOutputTypeDef

```python
# ScheduleOutputTypeDef definition

class ScheduleOutputTypeDef(TypedDict):
    StartTime: str,
    EndTime: NotRequired[str],
    EventFilter: NotRequired[CampaignEventFilterOutputTypeDef],  # (1)
    Frequency: NotRequired[FrequencyType],  # (2)
    IsLocalTime: NotRequired[bool],
    QuietTime: NotRequired[QuietTimeTypeDef],  # (3)
    Timezone: NotRequired[str],
```

1. See [:material-code-braces: CampaignEventFilterOutputTypeDef](./type_defs.md#campaigneventfilteroutputtypedef) 
2. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
3. See [:material-code-braces: QuietTimeTypeDef](./type_defs.md#quiettimetypedef) 
## EventStartConditionOutputTypeDef

```python
# EventStartConditionOutputTypeDef definition

class EventStartConditionOutputTypeDef(TypedDict):
    EventFilter: NotRequired[EventFilterOutputTypeDef],  # (1)
    SegmentId: NotRequired[str],
```

1. See [:material-code-braces: EventFilterOutputTypeDef](./type_defs.md#eventfilteroutputtypedef) 
## PutEventsResponseTypeDef

```python
# PutEventsResponseTypeDef definition

class PutEventsResponseTypeDef(TypedDict):
    EventsResponse: EventsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventsResponseTypeDef](./type_defs.md#eventsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetExportJobsResponseTypeDef

```python
# GetExportJobsResponseTypeDef definition

class GetExportJobsResponseTypeDef(TypedDict):
    ExportJobsResponse: ExportJobsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportJobsResponseTypeDef](./type_defs.md#exportjobsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentExportJobsResponseTypeDef

```python
# GetSegmentExportJobsResponseTypeDef definition

class GetSegmentExportJobsResponseTypeDef(TypedDict):
    ExportJobsResponse: ExportJobsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportJobsResponseTypeDef](./type_defs.md#exportjobsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SegmentDimensionsOutputTypeDef

```python
# SegmentDimensionsOutputTypeDef definition

class SegmentDimensionsOutputTypeDef(TypedDict):
    Attributes: NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],  # (1)
    Behavior: NotRequired[SegmentBehaviorsTypeDef],  # (2)
    Demographic: NotRequired[SegmentDemographicsOutputTypeDef],  # (3)
    Location: NotRequired[SegmentLocationOutputTypeDef],  # (4)
    Metrics: NotRequired[Dict[str, MetricDimensionTypeDef]],  # (5)
    UserAttributes: NotRequired[Dict[str, AttributeDimensionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeDimensionOutputTypeDef](./type_defs.md#attributedimensionoutputtypedef) 
2. See [:material-code-braces: SegmentBehaviorsTypeDef](./type_defs.md#segmentbehaviorstypedef) 
3. See [:material-code-braces: SegmentDemographicsOutputTypeDef](./type_defs.md#segmentdemographicsoutputtypedef) 
4. See [:material-code-braces: SegmentLocationOutputTypeDef](./type_defs.md#segmentlocationoutputtypedef) 
5. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
6. See [:material-code-braces: AttributeDimensionOutputTypeDef](./type_defs.md#attributedimensionoutputtypedef) 
## GetImportJobsResponseTypeDef

```python
# GetImportJobsResponseTypeDef definition

class GetImportJobsResponseTypeDef(TypedDict):
    ImportJobsResponse: ImportJobsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportJobsResponseTypeDef](./type_defs.md#importjobsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentImportJobsResponseTypeDef

```python
# GetSegmentImportJobsResponseTypeDef definition

class GetSegmentImportJobsResponseTypeDef(TypedDict):
    ImportJobsResponse: ImportJobsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ImportJobsResponseTypeDef](./type_defs.md#importjobsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CampaignInAppMessageOutputTypeDef

```python
# CampaignInAppMessageOutputTypeDef definition

class CampaignInAppMessageOutputTypeDef(TypedDict):
    Body: NotRequired[str],
    Content: NotRequired[List[InAppMessageContentTypeDef]],  # (1)
    CustomConfig: NotRequired[Dict[str, str]],
    Layout: NotRequired[LayoutType],  # (2)
```

1. See [:material-code-braces: InAppMessageContentTypeDef](./type_defs.md#inappmessagecontenttypedef) 
2. See [:material-code-brackets: LayoutType](./literals.md#layouttype) 
## CampaignInAppMessageTypeDef

```python
# CampaignInAppMessageTypeDef definition

class CampaignInAppMessageTypeDef(TypedDict):
    Body: NotRequired[str],
    Content: NotRequired[Sequence[InAppMessageContentTypeDef]],  # (1)
    CustomConfig: NotRequired[Mapping[str, str]],
    Layout: NotRequired[LayoutType],  # (2)
```

1. See [:material-code-braces: InAppMessageContentTypeDef](./type_defs.md#inappmessagecontenttypedef) 
2. See [:material-code-brackets: LayoutType](./literals.md#layouttype) 
## InAppMessageTypeDef

```python
# InAppMessageTypeDef definition

class InAppMessageTypeDef(TypedDict):
    Content: NotRequired[List[InAppMessageContentTypeDef]],  # (1)
    CustomConfig: NotRequired[Dict[str, str]],
    Layout: NotRequired[LayoutType],  # (2)
```

1. See [:material-code-braces: InAppMessageContentTypeDef](./type_defs.md#inappmessagecontenttypedef) 
2. See [:material-code-brackets: LayoutType](./literals.md#layouttype) 
## InAppTemplateRequestTypeDef

```python
# InAppTemplateRequestTypeDef definition

class InAppTemplateRequestTypeDef(TypedDict):
    Content: NotRequired[Sequence[InAppMessageContentTypeDef]],  # (1)
    CustomConfig: NotRequired[Mapping[str, str]],
    Layout: NotRequired[LayoutType],  # (2)
    tags: NotRequired[Mapping[str, str]],
    TemplateDescription: NotRequired[str],
```

1. See [:material-code-braces: InAppMessageContentTypeDef](./type_defs.md#inappmessagecontenttypedef) 
2. See [:material-code-brackets: LayoutType](./literals.md#layouttype) 
## InAppTemplateResponseTypeDef

```python
# InAppTemplateResponseTypeDef definition

class InAppTemplateResponseTypeDef(TypedDict):
    CreationDate: str,
    LastModifiedDate: str,
    TemplateName: str,
    TemplateType: TemplateTypeType,  # (3)
    Arn: NotRequired[str],
    Content: NotRequired[List[InAppMessageContentTypeDef]],  # (1)
    CustomConfig: NotRequired[Dict[str, str]],
    Layout: NotRequired[LayoutType],  # (2)
    tags: NotRequired[Dict[str, str]],
    TemplateDescription: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-braces: InAppMessageContentTypeDef](./type_defs.md#inappmessagecontenttypedef) 
2. See [:material-code-brackets: LayoutType](./literals.md#layouttype) 
3. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## ApplicationDateRangeKpiResponseTypeDef

```python
# ApplicationDateRangeKpiResponseTypeDef definition

class ApplicationDateRangeKpiResponseTypeDef(TypedDict):
    ApplicationId: str,
    EndTime: datetime,
    KpiName: str,
    KpiResult: BaseKpiResultTypeDef,  # (1)
    StartTime: datetime,
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BaseKpiResultTypeDef](./type_defs.md#basekpiresulttypedef) 
## CampaignDateRangeKpiResponseTypeDef

```python
# CampaignDateRangeKpiResponseTypeDef definition

class CampaignDateRangeKpiResponseTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
    EndTime: datetime,
    KpiName: str,
    KpiResult: BaseKpiResultTypeDef,  # (1)
    StartTime: datetime,
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BaseKpiResultTypeDef](./type_defs.md#basekpiresulttypedef) 
## JourneyDateRangeKpiResponseTypeDef

```python
# JourneyDateRangeKpiResponseTypeDef definition

class JourneyDateRangeKpiResponseTypeDef(TypedDict):
    ApplicationId: str,
    EndTime: datetime,
    JourneyId: str,
    KpiName: str,
    KpiResult: BaseKpiResultTypeDef,  # (1)
    StartTime: datetime,
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BaseKpiResultTypeDef](./type_defs.md#basekpiresulttypedef) 
## DirectMessageConfigurationTypeDef

```python
# DirectMessageConfigurationTypeDef definition

class DirectMessageConfigurationTypeDef(TypedDict):
    ADMMessage: NotRequired[ADMMessageTypeDef],  # (1)
    APNSMessage: NotRequired[APNSMessageTypeDef],  # (2)
    BaiduMessage: NotRequired[BaiduMessageTypeDef],  # (3)
    DefaultMessage: NotRequired[DefaultMessageTypeDef],  # (4)
    DefaultPushNotificationMessage: NotRequired[DefaultPushNotificationMessageTypeDef],  # (5)
    EmailMessage: NotRequired[EmailMessageTypeDef],  # (6)
    GCMMessage: NotRequired[GCMMessageTypeDef],  # (7)
    SMSMessage: NotRequired[SMSMessageTypeDef],  # (8)
    VoiceMessage: NotRequired[VoiceMessageTypeDef],  # (9)
```

1. See [:material-code-braces: ADMMessageTypeDef](./type_defs.md#admmessagetypedef) 
2. See [:material-code-braces: APNSMessageTypeDef](./type_defs.md#apnsmessagetypedef) 
3. See [:material-code-braces: BaiduMessageTypeDef](./type_defs.md#baidumessagetypedef) 
4. See [:material-code-braces: DefaultMessageTypeDef](./type_defs.md#defaultmessagetypedef) 
5. See [:material-code-braces: DefaultPushNotificationMessageTypeDef](./type_defs.md#defaultpushnotificationmessagetypedef) 
6. See [:material-code-braces: EmailMessageTypeDef](./type_defs.md#emailmessagetypedef) 
7. See [:material-code-braces: GCMMessageTypeDef](./type_defs.md#gcmmessagetypedef) 
8. See [:material-code-braces: SMSMessageTypeDef](./type_defs.md#smsmessagetypedef) 
9. See [:material-code-braces: VoiceMessageTypeDef](./type_defs.md#voicemessagetypedef) 
## UpdateEndpointsBatchRequestRequestTypeDef

```python
# UpdateEndpointsBatchRequestRequestTypeDef definition

class UpdateEndpointsBatchRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EndpointBatchRequest: EndpointBatchRequestTypeDef,  # (1)
```

1. See [:material-code-braces: EndpointBatchRequestTypeDef](./type_defs.md#endpointbatchrequesttypedef) 
## EventsRequestTypeDef

```python
# EventsRequestTypeDef definition

class EventsRequestTypeDef(TypedDict):
    BatchItem: Mapping[str, EventsBatchTypeDef],  # (1)
```

1. See [:material-code-braces: EventsBatchTypeDef](./type_defs.md#eventsbatchtypedef) 
## StartConditionOutputTypeDef

```python
# StartConditionOutputTypeDef definition

class StartConditionOutputTypeDef(TypedDict):
    Description: NotRequired[str],
    EventStartCondition: NotRequired[EventStartConditionOutputTypeDef],  # (1)
    SegmentStartCondition: NotRequired[SegmentConditionTypeDef],  # (2)
```

1. See [:material-code-braces: EventStartConditionOutputTypeDef](./type_defs.md#eventstartconditionoutputtypedef) 
2. See [:material-code-braces: SegmentConditionTypeDef](./type_defs.md#segmentconditiontypedef) 
## SegmentGroupOutputTypeDef

```python
# SegmentGroupOutputTypeDef definition

class SegmentGroupOutputTypeDef(TypedDict):
    Dimensions: NotRequired[List[SegmentDimensionsOutputTypeDef]],  # (1)
    SourceSegments: NotRequired[List[SegmentReferenceTypeDef]],  # (2)
    SourceType: NotRequired[SourceTypeType],  # (3)
    Type: NotRequired[TypeType],  # (4)
```

1. See [:material-code-braces: SegmentDimensionsOutputTypeDef](./type_defs.md#segmentdimensionsoutputtypedef) 
2. See [:material-code-braces: SegmentReferenceTypeDef](./type_defs.md#segmentreferencetypedef) 
3. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
4. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## SimpleConditionOutputTypeDef

```python
# SimpleConditionOutputTypeDef definition

class SimpleConditionOutputTypeDef(TypedDict):
    EventCondition: NotRequired[EventConditionOutputTypeDef],  # (1)
    SegmentCondition: NotRequired[SegmentConditionTypeDef],  # (2)
    SegmentDimensions: NotRequired[SegmentDimensionsOutputTypeDef],  # (3)
```

1. See [:material-code-braces: EventConditionOutputTypeDef](./type_defs.md#eventconditionoutputtypedef) 
2. See [:material-code-braces: SegmentConditionTypeDef](./type_defs.md#segmentconditiontypedef) 
3. See [:material-code-braces: SegmentDimensionsOutputTypeDef](./type_defs.md#segmentdimensionsoutputtypedef) 
## MessageConfigurationOutputTypeDef

```python
# MessageConfigurationOutputTypeDef definition

class MessageConfigurationOutputTypeDef(TypedDict):
    ADMMessage: NotRequired[MessageTypeDef],  # (1)
    APNSMessage: NotRequired[MessageTypeDef],  # (1)
    BaiduMessage: NotRequired[MessageTypeDef],  # (1)
    CustomMessage: NotRequired[CampaignCustomMessageTypeDef],  # (4)
    DefaultMessage: NotRequired[MessageTypeDef],  # (1)
    EmailMessage: NotRequired[CampaignEmailMessageOutputTypeDef],  # (6)
    GCMMessage: NotRequired[MessageTypeDef],  # (1)
    SMSMessage: NotRequired[CampaignSmsMessageTypeDef],  # (8)
    InAppMessage: NotRequired[CampaignInAppMessageOutputTypeDef],  # (9)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
3. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
4. See [:material-code-braces: CampaignCustomMessageTypeDef](./type_defs.md#campaigncustommessagetypedef) 
5. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
6. See [:material-code-braces: CampaignEmailMessageOutputTypeDef](./type_defs.md#campaignemailmessageoutputtypedef) 
7. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
8. See [:material-code-braces: CampaignSmsMessageTypeDef](./type_defs.md#campaignsmsmessagetypedef) 
9. See [:material-code-braces: CampaignInAppMessageOutputTypeDef](./type_defs.md#campaigninappmessageoutputtypedef) 
## InAppMessageCampaignTypeDef

```python
# InAppMessageCampaignTypeDef definition

class InAppMessageCampaignTypeDef(TypedDict):
    CampaignId: NotRequired[str],
    DailyCap: NotRequired[int],
    InAppMessage: NotRequired[InAppMessageTypeDef],  # (1)
    Priority: NotRequired[int],
    Schedule: NotRequired[InAppCampaignScheduleTypeDef],  # (2)
    SessionCap: NotRequired[int],
    TotalCap: NotRequired[int],
    TreatmentId: NotRequired[str],
```

1. See [:material-code-braces: InAppMessageTypeDef](./type_defs.md#inappmessagetypedef) 
2. See [:material-code-braces: InAppCampaignScheduleTypeDef](./type_defs.md#inappcampaignscheduletypedef) 
## CreateInAppTemplateRequestRequestTypeDef

```python
# CreateInAppTemplateRequestRequestTypeDef definition

class CreateInAppTemplateRequestRequestTypeDef(TypedDict):
    InAppTemplateRequest: InAppTemplateRequestTypeDef,  # (1)
    TemplateName: str,
```

1. See [:material-code-braces: InAppTemplateRequestTypeDef](./type_defs.md#inapptemplaterequesttypedef) 
## UpdateInAppTemplateRequestRequestTypeDef

```python
# UpdateInAppTemplateRequestRequestTypeDef definition

class UpdateInAppTemplateRequestRequestTypeDef(TypedDict):
    InAppTemplateRequest: InAppTemplateRequestTypeDef,  # (1)
    TemplateName: str,
    CreateNewVersion: NotRequired[bool],
    Version: NotRequired[str],
```

1. See [:material-code-braces: InAppTemplateRequestTypeDef](./type_defs.md#inapptemplaterequesttypedef) 
## GetInAppTemplateResponseTypeDef

```python
# GetInAppTemplateResponseTypeDef definition

class GetInAppTemplateResponseTypeDef(TypedDict):
    InAppTemplateResponse: InAppTemplateResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InAppTemplateResponseTypeDef](./type_defs.md#inapptemplateresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetApplicationDateRangeKpiResponseTypeDef

```python
# GetApplicationDateRangeKpiResponseTypeDef definition

class GetApplicationDateRangeKpiResponseTypeDef(TypedDict):
    ApplicationDateRangeKpiResponse: ApplicationDateRangeKpiResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ApplicationDateRangeKpiResponseTypeDef](./type_defs.md#applicationdaterangekpiresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCampaignDateRangeKpiResponseTypeDef

```python
# GetCampaignDateRangeKpiResponseTypeDef definition

class GetCampaignDateRangeKpiResponseTypeDef(TypedDict):
    CampaignDateRangeKpiResponse: CampaignDateRangeKpiResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignDateRangeKpiResponseTypeDef](./type_defs.md#campaigndaterangekpiresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJourneyDateRangeKpiResponseTypeDef

```python
# GetJourneyDateRangeKpiResponseTypeDef definition

class GetJourneyDateRangeKpiResponseTypeDef(TypedDict):
    JourneyDateRangeKpiResponse: JourneyDateRangeKpiResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyDateRangeKpiResponseTypeDef](./type_defs.md#journeydaterangekpiresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CampaignEventFilterTypeDef

```python
# CampaignEventFilterTypeDef definition

class CampaignEventFilterTypeDef(TypedDict):
    Dimensions: EventDimensionsUnionTypeDef,  # (1)
    FilterType: FilterTypeType,  # (2)
```

1. See [:material-code-braces: EventDimensionsTypeDef](./type_defs.md#eventdimensionstypedef) [:material-code-braces: EventDimensionsOutputTypeDef](./type_defs.md#eventdimensionsoutputtypedef) 
2. See [:material-code-brackets: FilterTypeType](./literals.md#filtertypetype) 
## EventConditionTypeDef

```python
# EventConditionTypeDef definition

class EventConditionTypeDef(TypedDict):
    Dimensions: NotRequired[EventDimensionsUnionTypeDef],  # (1)
    MessageActivity: NotRequired[str],
```

1. See [:material-code-braces: EventDimensionsTypeDef](./type_defs.md#eventdimensionstypedef) [:material-code-braces: EventDimensionsOutputTypeDef](./type_defs.md#eventdimensionsoutputtypedef) 
## EventFilterTypeDef

```python
# EventFilterTypeDef definition

class EventFilterTypeDef(TypedDict):
    Dimensions: EventDimensionsUnionTypeDef,  # (1)
    FilterType: FilterTypeType,  # (2)
```

1. See [:material-code-braces: EventDimensionsTypeDef](./type_defs.md#eventdimensionstypedef) [:material-code-braces: EventDimensionsOutputTypeDef](./type_defs.md#eventdimensionsoutputtypedef) 
2. See [:material-code-brackets: FilterTypeType](./literals.md#filtertypetype) 
## SegmentDimensionsTypeDef

```python
# SegmentDimensionsTypeDef definition

class SegmentDimensionsTypeDef(TypedDict):
    Attributes: NotRequired[Mapping[str, AttributeDimensionUnionTypeDef]],  # (1)
    Behavior: NotRequired[SegmentBehaviorsTypeDef],  # (2)
    Demographic: NotRequired[SegmentDemographicsUnionTypeDef],  # (3)
    Location: NotRequired[SegmentLocationUnionTypeDef],  # (4)
    Metrics: NotRequired[Mapping[str, MetricDimensionTypeDef]],  # (5)
    UserAttributes: NotRequired[Mapping[str, AttributeDimensionUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeDimensionTypeDef](./type_defs.md#attributedimensiontypedef) [:material-code-braces: AttributeDimensionOutputTypeDef](./type_defs.md#attributedimensionoutputtypedef) 
2. See [:material-code-braces: SegmentBehaviorsTypeDef](./type_defs.md#segmentbehaviorstypedef) 
3. See [:material-code-braces: SegmentDemographicsTypeDef](./type_defs.md#segmentdemographicstypedef) [:material-code-braces: SegmentDemographicsOutputTypeDef](./type_defs.md#segmentdemographicsoutputtypedef) 
4. See [:material-code-braces: SegmentLocationTypeDef](./type_defs.md#segmentlocationtypedef) [:material-code-braces: SegmentLocationOutputTypeDef](./type_defs.md#segmentlocationoutputtypedef) 
5. See [:material-code-braces: MetricDimensionTypeDef](./type_defs.md#metricdimensiontypedef) 
6. See [:material-code-braces: AttributeDimensionTypeDef](./type_defs.md#attributedimensiontypedef) [:material-code-braces: AttributeDimensionOutputTypeDef](./type_defs.md#attributedimensionoutputtypedef) 
## MessageRequestTypeDef

```python
# MessageRequestTypeDef definition

class MessageRequestTypeDef(TypedDict):
    MessageConfiguration: DirectMessageConfigurationTypeDef,  # (3)
    Addresses: NotRequired[Mapping[str, AddressConfigurationTypeDef]],  # (1)
    Context: NotRequired[Mapping[str, str]],
    Endpoints: NotRequired[Mapping[str, EndpointSendConfigurationTypeDef]],  # (2)
    TemplateConfiguration: NotRequired[TemplateConfigurationTypeDef],  # (4)
    TraceId: NotRequired[str],
```

1. See [:material-code-braces: AddressConfigurationTypeDef](./type_defs.md#addressconfigurationtypedef) 
2. See [:material-code-braces: EndpointSendConfigurationTypeDef](./type_defs.md#endpointsendconfigurationtypedef) 
3. See [:material-code-braces: DirectMessageConfigurationTypeDef](./type_defs.md#directmessageconfigurationtypedef) 
4. See [:material-code-braces: TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef) 
## SendUsersMessageRequestTypeDef

```python
# SendUsersMessageRequestTypeDef definition

class SendUsersMessageRequestTypeDef(TypedDict):
    MessageConfiguration: DirectMessageConfigurationTypeDef,  # (1)
    Users: Mapping[str, EndpointSendConfigurationTypeDef],  # (3)
    Context: NotRequired[Mapping[str, str]],
    TemplateConfiguration: NotRequired[TemplateConfigurationTypeDef],  # (2)
    TraceId: NotRequired[str],
```

1. See [:material-code-braces: DirectMessageConfigurationTypeDef](./type_defs.md#directmessageconfigurationtypedef) 
2. See [:material-code-braces: TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef) 
3. See [:material-code-braces: EndpointSendConfigurationTypeDef](./type_defs.md#endpointsendconfigurationtypedef) 
## PutEventsRequestRequestTypeDef

```python
# PutEventsRequestRequestTypeDef definition

class PutEventsRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    EventsRequest: EventsRequestTypeDef,  # (1)
```

1. See [:material-code-braces: EventsRequestTypeDef](./type_defs.md#eventsrequesttypedef) 
## SegmentGroupListOutputTypeDef

```python
# SegmentGroupListOutputTypeDef definition

class SegmentGroupListOutputTypeDef(TypedDict):
    Groups: NotRequired[List[SegmentGroupOutputTypeDef]],  # (1)
    Include: NotRequired[IncludeType],  # (2)
```

1. See [:material-code-braces: SegmentGroupOutputTypeDef](./type_defs.md#segmentgroupoutputtypedef) 
2. See [:material-code-brackets: IncludeType](./literals.md#includetype) 
## ConditionOutputTypeDef

```python
# ConditionOutputTypeDef definition

class ConditionOutputTypeDef(TypedDict):
    Conditions: NotRequired[List[SimpleConditionOutputTypeDef]],  # (1)
    Operator: NotRequired[OperatorType],  # (2)
```

1. See [:material-code-braces: SimpleConditionOutputTypeDef](./type_defs.md#simpleconditionoutputtypedef) 
2. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## MultiConditionalBranchOutputTypeDef

```python
# MultiConditionalBranchOutputTypeDef definition

class MultiConditionalBranchOutputTypeDef(TypedDict):
    Condition: NotRequired[SimpleConditionOutputTypeDef],  # (1)
    NextActivity: NotRequired[str],
```

1. See [:material-code-braces: SimpleConditionOutputTypeDef](./type_defs.md#simpleconditionoutputtypedef) 
## TreatmentResourceTypeDef

```python
# TreatmentResourceTypeDef definition

class TreatmentResourceTypeDef(TypedDict):
    Id: str,
    SizePercent: int,
    CustomDeliveryConfiguration: NotRequired[CustomDeliveryConfigurationOutputTypeDef],  # (1)
    MessageConfiguration: NotRequired[MessageConfigurationOutputTypeDef],  # (2)
    Schedule: NotRequired[ScheduleOutputTypeDef],  # (3)
    State: NotRequired[CampaignStateTypeDef],  # (4)
    TemplateConfiguration: NotRequired[TemplateConfigurationTypeDef],  # (5)
    TreatmentDescription: NotRequired[str],
    TreatmentName: NotRequired[str],
```

1. See [:material-code-braces: CustomDeliveryConfigurationOutputTypeDef](./type_defs.md#customdeliveryconfigurationoutputtypedef) 
2. See [:material-code-braces: MessageConfigurationOutputTypeDef](./type_defs.md#messageconfigurationoutputtypedef) 
3. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
4. See [:material-code-braces: CampaignStateTypeDef](./type_defs.md#campaignstatetypedef) 
5. See [:material-code-braces: TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef) 
## MessageConfigurationTypeDef

```python
# MessageConfigurationTypeDef definition

class MessageConfigurationTypeDef(TypedDict):
    ADMMessage: NotRequired[MessageTypeDef],  # (1)
    APNSMessage: NotRequired[MessageTypeDef],  # (1)
    BaiduMessage: NotRequired[MessageTypeDef],  # (1)
    CustomMessage: NotRequired[CampaignCustomMessageTypeDef],  # (4)
    DefaultMessage: NotRequired[MessageTypeDef],  # (1)
    EmailMessage: NotRequired[CampaignEmailMessageUnionTypeDef],  # (6)
    GCMMessage: NotRequired[MessageTypeDef],  # (1)
    SMSMessage: NotRequired[CampaignSmsMessageTypeDef],  # (8)
    InAppMessage: NotRequired[CampaignInAppMessageUnionTypeDef],  # (9)
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
3. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
4. See [:material-code-braces: CampaignCustomMessageTypeDef](./type_defs.md#campaigncustommessagetypedef) 
5. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
6. See [:material-code-braces: CampaignEmailMessageTypeDef](./type_defs.md#campaignemailmessagetypedef) [:material-code-braces: CampaignEmailMessageOutputTypeDef](./type_defs.md#campaignemailmessageoutputtypedef) 
7. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
8. See [:material-code-braces: CampaignSmsMessageTypeDef](./type_defs.md#campaignsmsmessagetypedef) 
9. See [:material-code-braces: CampaignInAppMessageTypeDef](./type_defs.md#campaigninappmessagetypedef) [:material-code-braces: CampaignInAppMessageOutputTypeDef](./type_defs.md#campaigninappmessageoutputtypedef) 
## InAppMessagesResponseTypeDef

```python
# InAppMessagesResponseTypeDef definition

class InAppMessagesResponseTypeDef(TypedDict):
    InAppMessageCampaigns: NotRequired[List[InAppMessageCampaignTypeDef]],  # (1)
```

1. See [:material-code-braces: InAppMessageCampaignTypeDef](./type_defs.md#inappmessagecampaigntypedef) 
## SendMessagesRequestRequestTypeDef

```python
# SendMessagesRequestRequestTypeDef definition

class SendMessagesRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    MessageRequest: MessageRequestTypeDef,  # (1)
```

1. See [:material-code-braces: MessageRequestTypeDef](./type_defs.md#messagerequesttypedef) 
## SendUsersMessagesRequestRequestTypeDef

```python
# SendUsersMessagesRequestRequestTypeDef definition

class SendUsersMessagesRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SendUsersMessageRequest: SendUsersMessageRequestTypeDef,  # (1)
```

1. See [:material-code-braces: SendUsersMessageRequestTypeDef](./type_defs.md#sendusersmessagerequesttypedef) 
## SegmentResponseTypeDef

```python
# SegmentResponseTypeDef definition

class SegmentResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    CreationDate: str,
    Id: str,
    SegmentType: SegmentTypeType,  # (4)
    Dimensions: NotRequired[SegmentDimensionsOutputTypeDef],  # (1)
    ImportDefinition: NotRequired[SegmentImportResourceTypeDef],  # (2)
    LastModifiedDate: NotRequired[str],
    Name: NotRequired[str],
    SegmentGroups: NotRequired[SegmentGroupListOutputTypeDef],  # (3)
    tags: NotRequired[Dict[str, str]],
    Version: NotRequired[int],
```

1. See [:material-code-braces: SegmentDimensionsOutputTypeDef](./type_defs.md#segmentdimensionsoutputtypedef) 
2. See [:material-code-braces: SegmentImportResourceTypeDef](./type_defs.md#segmentimportresourcetypedef) 
3. See [:material-code-braces: SegmentGroupListOutputTypeDef](./type_defs.md#segmentgrouplistoutputtypedef) 
4. See [:material-code-brackets: SegmentTypeType](./literals.md#segmenttypetype) 
## ConditionalSplitActivityOutputTypeDef

```python
# ConditionalSplitActivityOutputTypeDef definition

class ConditionalSplitActivityOutputTypeDef(TypedDict):
    Condition: NotRequired[ConditionOutputTypeDef],  # (1)
    EvaluationWaitTime: NotRequired[WaitTimeTypeDef],  # (2)
    FalseActivity: NotRequired[str],
    TrueActivity: NotRequired[str],
```

1. See [:material-code-braces: ConditionOutputTypeDef](./type_defs.md#conditionoutputtypedef) 
2. See [:material-code-braces: WaitTimeTypeDef](./type_defs.md#waittimetypedef) 
## MultiConditionalSplitActivityOutputTypeDef

```python
# MultiConditionalSplitActivityOutputTypeDef definition

class MultiConditionalSplitActivityOutputTypeDef(TypedDict):
    Branches: NotRequired[List[MultiConditionalBranchOutputTypeDef]],  # (1)
    DefaultActivity: NotRequired[str],
    EvaluationWaitTime: NotRequired[WaitTimeTypeDef],  # (2)
```

1. See [:material-code-braces: MultiConditionalBranchOutputTypeDef](./type_defs.md#multiconditionalbranchoutputtypedef) 
2. See [:material-code-braces: WaitTimeTypeDef](./type_defs.md#waittimetypedef) 
## CampaignResponseTypeDef

```python
# CampaignResponseTypeDef definition

class CampaignResponseTypeDef(TypedDict):
    ApplicationId: str,
    Arn: str,
    CreationDate: str,
    Id: str,
    LastModifiedDate: str,
    SegmentId: str,
    SegmentVersion: int,
    AdditionalTreatments: NotRequired[List[TreatmentResourceTypeDef]],  # (1)
    CustomDeliveryConfiguration: NotRequired[CustomDeliveryConfigurationOutputTypeDef],  # (2)
    DefaultState: NotRequired[CampaignStateTypeDef],  # (3)
    Description: NotRequired[str],
    HoldoutPercent: NotRequired[int],
    Hook: NotRequired[CampaignHookTypeDef],  # (4)
    IsPaused: NotRequired[bool],
    Limits: NotRequired[CampaignLimitsTypeDef],  # (5)
    MessageConfiguration: NotRequired[MessageConfigurationOutputTypeDef],  # (6)
    Name: NotRequired[str],
    Schedule: NotRequired[ScheduleOutputTypeDef],  # (7)
    State: NotRequired[CampaignStateTypeDef],  # (3)
    tags: NotRequired[Dict[str, str]],
    TemplateConfiguration: NotRequired[TemplateConfigurationTypeDef],  # (9)
    TreatmentDescription: NotRequired[str],
    TreatmentName: NotRequired[str],
    Version: NotRequired[int],
    Priority: NotRequired[int],
```

1. See [:material-code-braces: TreatmentResourceTypeDef](./type_defs.md#treatmentresourcetypedef) 
2. See [:material-code-braces: CustomDeliveryConfigurationOutputTypeDef](./type_defs.md#customdeliveryconfigurationoutputtypedef) 
3. See [:material-code-braces: CampaignStateTypeDef](./type_defs.md#campaignstatetypedef) 
4. See [:material-code-braces: CampaignHookTypeDef](./type_defs.md#campaignhooktypedef) 
5. See [:material-code-braces: CampaignLimitsTypeDef](./type_defs.md#campaignlimitstypedef) 
6. See [:material-code-braces: MessageConfigurationOutputTypeDef](./type_defs.md#messageconfigurationoutputtypedef) 
7. See [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
8. See [:material-code-braces: CampaignStateTypeDef](./type_defs.md#campaignstatetypedef) 
9. See [:material-code-braces: TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef) 
## GetInAppMessagesResponseTypeDef

```python
# GetInAppMessagesResponseTypeDef definition

class GetInAppMessagesResponseTypeDef(TypedDict):
    InAppMessagesResponse: InAppMessagesResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InAppMessagesResponseTypeDef](./type_defs.md#inappmessagesresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScheduleTypeDef

```python
# ScheduleTypeDef definition

class ScheduleTypeDef(TypedDict):
    StartTime: str,
    EndTime: NotRequired[str],
    EventFilter: NotRequired[CampaignEventFilterUnionTypeDef],  # (1)
    Frequency: NotRequired[FrequencyType],  # (2)
    IsLocalTime: NotRequired[bool],
    QuietTime: NotRequired[QuietTimeTypeDef],  # (3)
    Timezone: NotRequired[str],
```

1. See [:material-code-braces: CampaignEventFilterTypeDef](./type_defs.md#campaigneventfiltertypedef) [:material-code-braces: CampaignEventFilterOutputTypeDef](./type_defs.md#campaigneventfilteroutputtypedef) 
2. See [:material-code-brackets: FrequencyType](./literals.md#frequencytype) 
3. See [:material-code-braces: QuietTimeTypeDef](./type_defs.md#quiettimetypedef) 
## EventStartConditionTypeDef

```python
# EventStartConditionTypeDef definition

class EventStartConditionTypeDef(TypedDict):
    EventFilter: NotRequired[EventFilterUnionTypeDef],  # (1)
    SegmentId: NotRequired[str],
```

1. See [:material-code-braces: EventFilterTypeDef](./type_defs.md#eventfiltertypedef) [:material-code-braces: EventFilterOutputTypeDef](./type_defs.md#eventfilteroutputtypedef) 
## SegmentGroupTypeDef

```python
# SegmentGroupTypeDef definition

class SegmentGroupTypeDef(TypedDict):
    Dimensions: NotRequired[Sequence[SegmentDimensionsUnionTypeDef]],  # (1)
    SourceSegments: NotRequired[Sequence[SegmentReferenceTypeDef]],  # (2)
    SourceType: NotRequired[SourceTypeType],  # (3)
    Type: NotRequired[TypeType],  # (4)
```

1. See [:material-code-braces: SegmentDimensionsTypeDef](./type_defs.md#segmentdimensionstypedef) [:material-code-braces: SegmentDimensionsOutputTypeDef](./type_defs.md#segmentdimensionsoutputtypedef) 
2. See [:material-code-braces: SegmentReferenceTypeDef](./type_defs.md#segmentreferencetypedef) 
3. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
4. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## SimpleConditionTypeDef

```python
# SimpleConditionTypeDef definition

class SimpleConditionTypeDef(TypedDict):
    EventCondition: NotRequired[EventConditionUnionTypeDef],  # (1)
    SegmentCondition: NotRequired[SegmentConditionTypeDef],  # (2)
    SegmentDimensions: NotRequired[SegmentDimensionsUnionTypeDef],  # (3)
```

1. See [:material-code-braces: EventConditionTypeDef](./type_defs.md#eventconditiontypedef) [:material-code-braces: EventConditionOutputTypeDef](./type_defs.md#eventconditionoutputtypedef) 
2. See [:material-code-braces: SegmentConditionTypeDef](./type_defs.md#segmentconditiontypedef) 
3. See [:material-code-braces: SegmentDimensionsTypeDef](./type_defs.md#segmentdimensionstypedef) [:material-code-braces: SegmentDimensionsOutputTypeDef](./type_defs.md#segmentdimensionsoutputtypedef) 
## CreateSegmentResponseTypeDef

```python
# CreateSegmentResponseTypeDef definition

class CreateSegmentResponseTypeDef(TypedDict):
    SegmentResponse: SegmentResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentResponseTypeDef](./type_defs.md#segmentresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSegmentResponseTypeDef

```python
# DeleteSegmentResponseTypeDef definition

class DeleteSegmentResponseTypeDef(TypedDict):
    SegmentResponse: SegmentResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentResponseTypeDef](./type_defs.md#segmentresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentResponseTypeDef

```python
# GetSegmentResponseTypeDef definition

class GetSegmentResponseTypeDef(TypedDict):
    SegmentResponse: SegmentResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentResponseTypeDef](./type_defs.md#segmentresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentVersionResponseTypeDef

```python
# GetSegmentVersionResponseTypeDef definition

class GetSegmentVersionResponseTypeDef(TypedDict):
    SegmentResponse: SegmentResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentResponseTypeDef](./type_defs.md#segmentresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SegmentsResponseTypeDef

```python
# SegmentsResponseTypeDef definition

class SegmentsResponseTypeDef(TypedDict):
    Item: List[SegmentResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SegmentResponseTypeDef](./type_defs.md#segmentresponsetypedef) 
## UpdateSegmentResponseTypeDef

```python
# UpdateSegmentResponseTypeDef definition

class UpdateSegmentResponseTypeDef(TypedDict):
    SegmentResponse: SegmentResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentResponseTypeDef](./type_defs.md#segmentresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ActivityOutputTypeDef

```python
# ActivityOutputTypeDef definition

class ActivityOutputTypeDef(TypedDict):
    CUSTOM: NotRequired[CustomMessageActivityOutputTypeDef],  # (1)
    ConditionalSplit: NotRequired[ConditionalSplitActivityOutputTypeDef],  # (2)
    Description: NotRequired[str],
    EMAIL: NotRequired[EmailMessageActivityTypeDef],  # (3)
    Holdout: NotRequired[HoldoutActivityTypeDef],  # (4)
    MultiCondition: NotRequired[MultiConditionalSplitActivityOutputTypeDef],  # (5)
    PUSH: NotRequired[PushMessageActivityTypeDef],  # (6)
    RandomSplit: NotRequired[RandomSplitActivityOutputTypeDef],  # (7)
    SMS: NotRequired[SMSMessageActivityTypeDef],  # (8)
    Wait: NotRequired[WaitActivityTypeDef],  # (9)
    ContactCenter: NotRequired[ContactCenterActivityTypeDef],  # (10)
```

1. See [:material-code-braces: CustomMessageActivityOutputTypeDef](./type_defs.md#custommessageactivityoutputtypedef) 
2. See [:material-code-braces: ConditionalSplitActivityOutputTypeDef](./type_defs.md#conditionalsplitactivityoutputtypedef) 
3. See [:material-code-braces: EmailMessageActivityTypeDef](./type_defs.md#emailmessageactivitytypedef) 
4. See [:material-code-braces: HoldoutActivityTypeDef](./type_defs.md#holdoutactivitytypedef) 
5. See [:material-code-braces: MultiConditionalSplitActivityOutputTypeDef](./type_defs.md#multiconditionalsplitactivityoutputtypedef) 
6. See [:material-code-braces: PushMessageActivityTypeDef](./type_defs.md#pushmessageactivitytypedef) 
7. See [:material-code-braces: RandomSplitActivityOutputTypeDef](./type_defs.md#randomsplitactivityoutputtypedef) 
8. See [:material-code-braces: SMSMessageActivityTypeDef](./type_defs.md#smsmessageactivitytypedef) 
9. See [:material-code-braces: WaitActivityTypeDef](./type_defs.md#waitactivitytypedef) 
10. See [:material-code-braces: ContactCenterActivityTypeDef](./type_defs.md#contactcenteractivitytypedef) 
## CampaignsResponseTypeDef

```python
# CampaignsResponseTypeDef definition

class CampaignsResponseTypeDef(TypedDict):
    Item: List[CampaignResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CampaignResponseTypeDef](./type_defs.md#campaignresponsetypedef) 
## CreateCampaignResponseTypeDef

```python
# CreateCampaignResponseTypeDef definition

class CreateCampaignResponseTypeDef(TypedDict):
    CampaignResponse: CampaignResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignResponseTypeDef](./type_defs.md#campaignresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteCampaignResponseTypeDef

```python
# DeleteCampaignResponseTypeDef definition

class DeleteCampaignResponseTypeDef(TypedDict):
    CampaignResponse: CampaignResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignResponseTypeDef](./type_defs.md#campaignresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCampaignResponseTypeDef

```python
# GetCampaignResponseTypeDef definition

class GetCampaignResponseTypeDef(TypedDict):
    CampaignResponse: CampaignResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignResponseTypeDef](./type_defs.md#campaignresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCampaignVersionResponseTypeDef

```python
# GetCampaignVersionResponseTypeDef definition

class GetCampaignVersionResponseTypeDef(TypedDict):
    CampaignResponse: CampaignResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignResponseTypeDef](./type_defs.md#campaignresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCampaignResponseTypeDef

```python
# UpdateCampaignResponseTypeDef definition

class UpdateCampaignResponseTypeDef(TypedDict):
    CampaignResponse: CampaignResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignResponseTypeDef](./type_defs.md#campaignresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentVersionsResponseTypeDef

```python
# GetSegmentVersionsResponseTypeDef definition

class GetSegmentVersionsResponseTypeDef(TypedDict):
    SegmentsResponse: SegmentsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentsResponseTypeDef](./type_defs.md#segmentsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSegmentsResponseTypeDef

```python
# GetSegmentsResponseTypeDef definition

class GetSegmentsResponseTypeDef(TypedDict):
    SegmentsResponse: SegmentsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SegmentsResponseTypeDef](./type_defs.md#segmentsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JourneyResponseTypeDef

```python
# JourneyResponseTypeDef definition

class JourneyResponseTypeDef(TypedDict):
    ApplicationId: str,
    Id: str,
    Name: str,
    Activities: NotRequired[Dict[str, ActivityOutputTypeDef]],  # (1)
    CreationDate: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Limits: NotRequired[JourneyLimitsTypeDef],  # (2)
    LocalTime: NotRequired[bool],
    QuietTime: NotRequired[QuietTimeTypeDef],  # (3)
    RefreshFrequency: NotRequired[str],
    Schedule: NotRequired[JourneyScheduleOutputTypeDef],  # (4)
    StartActivity: NotRequired[str],
    StartCondition: NotRequired[StartConditionOutputTypeDef],  # (5)
    State: NotRequired[StateType],  # (6)
    tags: NotRequired[Dict[str, str]],
    WaitForQuietTime: NotRequired[bool],
    RefreshOnSegmentUpdate: NotRequired[bool],
    JourneyChannelSettings: NotRequired[JourneyChannelSettingsTypeDef],  # (7)
    SendingSchedule: NotRequired[bool],
    OpenHours: NotRequired[OpenHoursOutputTypeDef],  # (8)
    ClosedDays: NotRequired[ClosedDaysOutputTypeDef],  # (9)
    TimezoneEstimationMethods: NotRequired[List[TimezoneEstimationMethodsElementType]],  # (10)
```

1. See [:material-code-braces: ActivityOutputTypeDef](./type_defs.md#activityoutputtypedef) 
2. See [:material-code-braces: JourneyLimitsTypeDef](./type_defs.md#journeylimitstypedef) 
3. See [:material-code-braces: QuietTimeTypeDef](./type_defs.md#quiettimetypedef) 
4. See [:material-code-braces: JourneyScheduleOutputTypeDef](./type_defs.md#journeyscheduleoutputtypedef) 
5. See [:material-code-braces: StartConditionOutputTypeDef](./type_defs.md#startconditionoutputtypedef) 
6. See [:material-code-brackets: StateType](./literals.md#statetype) 
7. See [:material-code-braces: JourneyChannelSettingsTypeDef](./type_defs.md#journeychannelsettingstypedef) 
8. See [:material-code-braces: OpenHoursOutputTypeDef](./type_defs.md#openhoursoutputtypedef) 
9. See [:material-code-braces: ClosedDaysOutputTypeDef](./type_defs.md#closeddaysoutputtypedef) 
10. See [:material-code-brackets: TimezoneEstimationMethodsElementType](./literals.md#timezoneestimationmethodselementtype) 
## GetCampaignVersionsResponseTypeDef

```python
# GetCampaignVersionsResponseTypeDef definition

class GetCampaignVersionsResponseTypeDef(TypedDict):
    CampaignsResponse: CampaignsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignsResponseTypeDef](./type_defs.md#campaignsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCampaignsResponseTypeDef

```python
# GetCampaignsResponseTypeDef definition

class GetCampaignsResponseTypeDef(TypedDict):
    CampaignsResponse: CampaignsResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignsResponseTypeDef](./type_defs.md#campaignsresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WriteTreatmentResourceTypeDef

```python
# WriteTreatmentResourceTypeDef definition

class WriteTreatmentResourceTypeDef(TypedDict):
    SizePercent: int,
    CustomDeliveryConfiguration: NotRequired[CustomDeliveryConfigurationUnionTypeDef],  # (1)
    MessageConfiguration: NotRequired[MessageConfigurationUnionTypeDef],  # (2)
    Schedule: NotRequired[ScheduleUnionTypeDef],  # (3)
    TemplateConfiguration: NotRequired[TemplateConfigurationTypeDef],  # (4)
    TreatmentDescription: NotRequired[str],
    TreatmentName: NotRequired[str],
```

1. See [:material-code-braces: CustomDeliveryConfigurationTypeDef](./type_defs.md#customdeliveryconfigurationtypedef) [:material-code-braces: CustomDeliveryConfigurationOutputTypeDef](./type_defs.md#customdeliveryconfigurationoutputtypedef) 
2. See [:material-code-braces: MessageConfigurationTypeDef](./type_defs.md#messageconfigurationtypedef) [:material-code-braces: MessageConfigurationOutputTypeDef](./type_defs.md#messageconfigurationoutputtypedef) 
3. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
4. See [:material-code-braces: TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef) 
## StartConditionTypeDef

```python
# StartConditionTypeDef definition

class StartConditionTypeDef(TypedDict):
    Description: NotRequired[str],
    EventStartCondition: NotRequired[EventStartConditionUnionTypeDef],  # (1)
    SegmentStartCondition: NotRequired[SegmentConditionTypeDef],  # (2)
```

1. See [:material-code-braces: EventStartConditionTypeDef](./type_defs.md#eventstartconditiontypedef) [:material-code-braces: EventStartConditionOutputTypeDef](./type_defs.md#eventstartconditionoutputtypedef) 
2. See [:material-code-braces: SegmentConditionTypeDef](./type_defs.md#segmentconditiontypedef) 
## SegmentGroupListTypeDef

```python
# SegmentGroupListTypeDef definition

class SegmentGroupListTypeDef(TypedDict):
    Groups: NotRequired[Sequence[SegmentGroupUnionTypeDef]],  # (1)
    Include: NotRequired[IncludeType],  # (2)
```

1. See [:material-code-braces: SegmentGroupTypeDef](./type_defs.md#segmentgrouptypedef) [:material-code-braces: SegmentGroupOutputTypeDef](./type_defs.md#segmentgroupoutputtypedef) 
2. See [:material-code-brackets: IncludeType](./literals.md#includetype) 
## ConditionTypeDef

```python
# ConditionTypeDef definition

class ConditionTypeDef(TypedDict):
    Conditions: NotRequired[Sequence[SimpleConditionUnionTypeDef]],  # (1)
    Operator: NotRequired[OperatorType],  # (2)
```

1. See [:material-code-braces: SimpleConditionTypeDef](./type_defs.md#simpleconditiontypedef) [:material-code-braces: SimpleConditionOutputTypeDef](./type_defs.md#simpleconditionoutputtypedef) 
2. See [:material-code-brackets: OperatorType](./literals.md#operatortype) 
## MultiConditionalBranchTypeDef

```python
# MultiConditionalBranchTypeDef definition

class MultiConditionalBranchTypeDef(TypedDict):
    Condition: NotRequired[SimpleConditionUnionTypeDef],  # (1)
    NextActivity: NotRequired[str],
```

1. See [:material-code-braces: SimpleConditionTypeDef](./type_defs.md#simpleconditiontypedef) [:material-code-braces: SimpleConditionOutputTypeDef](./type_defs.md#simpleconditionoutputtypedef) 
## CreateJourneyResponseTypeDef

```python
# CreateJourneyResponseTypeDef definition

class CreateJourneyResponseTypeDef(TypedDict):
    JourneyResponse: JourneyResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyResponseTypeDef](./type_defs.md#journeyresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteJourneyResponseTypeDef

```python
# DeleteJourneyResponseTypeDef definition

class DeleteJourneyResponseTypeDef(TypedDict):
    JourneyResponse: JourneyResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyResponseTypeDef](./type_defs.md#journeyresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJourneyResponseTypeDef

```python
# GetJourneyResponseTypeDef definition

class GetJourneyResponseTypeDef(TypedDict):
    JourneyResponse: JourneyResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyResponseTypeDef](./type_defs.md#journeyresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JourneysResponseTypeDef

```python
# JourneysResponseTypeDef definition

class JourneysResponseTypeDef(TypedDict):
    Item: List[JourneyResponseTypeDef],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: JourneyResponseTypeDef](./type_defs.md#journeyresponsetypedef) 
## UpdateJourneyResponseTypeDef

```python
# UpdateJourneyResponseTypeDef definition

class UpdateJourneyResponseTypeDef(TypedDict):
    JourneyResponse: JourneyResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyResponseTypeDef](./type_defs.md#journeyresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJourneyStateResponseTypeDef

```python
# UpdateJourneyStateResponseTypeDef definition

class UpdateJourneyStateResponseTypeDef(TypedDict):
    JourneyResponse: JourneyResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneyResponseTypeDef](./type_defs.md#journeyresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WriteCampaignRequestTypeDef

```python
# WriteCampaignRequestTypeDef definition

class WriteCampaignRequestTypeDef(TypedDict):
    AdditionalTreatments: NotRequired[Sequence[WriteTreatmentResourceTypeDef]],  # (1)
    CustomDeliveryConfiguration: NotRequired[CustomDeliveryConfigurationUnionTypeDef],  # (2)
    Description: NotRequired[str],
    HoldoutPercent: NotRequired[int],
    Hook: NotRequired[CampaignHookTypeDef],  # (3)
    IsPaused: NotRequired[bool],
    Limits: NotRequired[CampaignLimitsTypeDef],  # (4)
    MessageConfiguration: NotRequired[MessageConfigurationUnionTypeDef],  # (5)
    Name: NotRequired[str],
    Schedule: NotRequired[ScheduleUnionTypeDef],  # (6)
    SegmentId: NotRequired[str],
    SegmentVersion: NotRequired[int],
    tags: NotRequired[Mapping[str, str]],
    TemplateConfiguration: NotRequired[TemplateConfigurationTypeDef],  # (7)
    TreatmentDescription: NotRequired[str],
    TreatmentName: NotRequired[str],
    Priority: NotRequired[int],
```

1. See [:material-code-braces: WriteTreatmentResourceTypeDef](./type_defs.md#writetreatmentresourcetypedef) 
2. See [:material-code-braces: CustomDeliveryConfigurationTypeDef](./type_defs.md#customdeliveryconfigurationtypedef) [:material-code-braces: CustomDeliveryConfigurationOutputTypeDef](./type_defs.md#customdeliveryconfigurationoutputtypedef) 
3. See [:material-code-braces: CampaignHookTypeDef](./type_defs.md#campaignhooktypedef) 
4. See [:material-code-braces: CampaignLimitsTypeDef](./type_defs.md#campaignlimitstypedef) 
5. See [:material-code-braces: MessageConfigurationTypeDef](./type_defs.md#messageconfigurationtypedef) [:material-code-braces: MessageConfigurationOutputTypeDef](./type_defs.md#messageconfigurationoutputtypedef) 
6. See [:material-code-braces: ScheduleTypeDef](./type_defs.md#scheduletypedef) [:material-code-braces: ScheduleOutputTypeDef](./type_defs.md#scheduleoutputtypedef) 
7. See [:material-code-braces: TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef) 
## ListJourneysResponseTypeDef

```python
# ListJourneysResponseTypeDef definition

class ListJourneysResponseTypeDef(TypedDict):
    JourneysResponse: JourneysResponseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JourneysResponseTypeDef](./type_defs.md#journeysresponsetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCampaignRequestRequestTypeDef

```python
# CreateCampaignRequestRequestTypeDef definition

class CreateCampaignRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    WriteCampaignRequest: WriteCampaignRequestTypeDef,  # (1)
```

1. See [:material-code-braces: WriteCampaignRequestTypeDef](./type_defs.md#writecampaignrequesttypedef) 
## UpdateCampaignRequestRequestTypeDef

```python
# UpdateCampaignRequestRequestTypeDef definition

class UpdateCampaignRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    CampaignId: str,
    WriteCampaignRequest: WriteCampaignRequestTypeDef,  # (1)
```

1. See [:material-code-braces: WriteCampaignRequestTypeDef](./type_defs.md#writecampaignrequesttypedef) 
## WriteSegmentRequestTypeDef

```python
# WriteSegmentRequestTypeDef definition

class WriteSegmentRequestTypeDef(TypedDict):
    Dimensions: NotRequired[SegmentDimensionsUnionTypeDef],  # (1)
    Name: NotRequired[str],
    SegmentGroups: NotRequired[SegmentGroupListUnionTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SegmentDimensionsTypeDef](./type_defs.md#segmentdimensionstypedef) [:material-code-braces: SegmentDimensionsOutputTypeDef](./type_defs.md#segmentdimensionsoutputtypedef) 
2. See [:material-code-braces: SegmentGroupListTypeDef](./type_defs.md#segmentgrouplisttypedef) [:material-code-braces: SegmentGroupListOutputTypeDef](./type_defs.md#segmentgrouplistoutputtypedef) 
## ConditionalSplitActivityTypeDef

```python
# ConditionalSplitActivityTypeDef definition

class ConditionalSplitActivityTypeDef(TypedDict):
    Condition: NotRequired[ConditionUnionTypeDef],  # (1)
    EvaluationWaitTime: NotRequired[WaitTimeTypeDef],  # (2)
    FalseActivity: NotRequired[str],
    TrueActivity: NotRequired[str],
```

1. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) [:material-code-braces: ConditionOutputTypeDef](./type_defs.md#conditionoutputtypedef) 
2. See [:material-code-braces: WaitTimeTypeDef](./type_defs.md#waittimetypedef) 
## MultiConditionalSplitActivityTypeDef

```python
# MultiConditionalSplitActivityTypeDef definition

class MultiConditionalSplitActivityTypeDef(TypedDict):
    Branches: NotRequired[Sequence[MultiConditionalBranchUnionTypeDef]],  # (1)
    DefaultActivity: NotRequired[str],
    EvaluationWaitTime: NotRequired[WaitTimeTypeDef],  # (2)
```

1. See [:material-code-braces: MultiConditionalBranchTypeDef](./type_defs.md#multiconditionalbranchtypedef) [:material-code-braces: MultiConditionalBranchOutputTypeDef](./type_defs.md#multiconditionalbranchoutputtypedef) 
2. See [:material-code-braces: WaitTimeTypeDef](./type_defs.md#waittimetypedef) 
## CreateSegmentRequestRequestTypeDef

```python
# CreateSegmentRequestRequestTypeDef definition

class CreateSegmentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    WriteSegmentRequest: WriteSegmentRequestTypeDef,  # (1)
```

1. See [:material-code-braces: WriteSegmentRequestTypeDef](./type_defs.md#writesegmentrequesttypedef) 
## UpdateSegmentRequestRequestTypeDef

```python
# UpdateSegmentRequestRequestTypeDef definition

class UpdateSegmentRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    SegmentId: str,
    WriteSegmentRequest: WriteSegmentRequestTypeDef,  # (1)
```

1. See [:material-code-braces: WriteSegmentRequestTypeDef](./type_defs.md#writesegmentrequesttypedef) 
## ActivityTypeDef

```python
# ActivityTypeDef definition

class ActivityTypeDef(TypedDict):
    CUSTOM: NotRequired[CustomMessageActivityUnionTypeDef],  # (1)
    ConditionalSplit: NotRequired[ConditionalSplitActivityUnionTypeDef],  # (2)
    Description: NotRequired[str],
    EMAIL: NotRequired[EmailMessageActivityTypeDef],  # (3)
    Holdout: NotRequired[HoldoutActivityTypeDef],  # (4)
    MultiCondition: NotRequired[MultiConditionalSplitActivityUnionTypeDef],  # (5)
    PUSH: NotRequired[PushMessageActivityTypeDef],  # (6)
    RandomSplit: NotRequired[RandomSplitActivityUnionTypeDef],  # (7)
    SMS: NotRequired[SMSMessageActivityTypeDef],  # (8)
    Wait: NotRequired[WaitActivityTypeDef],  # (9)
    ContactCenter: NotRequired[ContactCenterActivityTypeDef],  # (10)
```

1. See [:material-code-braces: CustomMessageActivityTypeDef](./type_defs.md#custommessageactivitytypedef) [:material-code-braces: CustomMessageActivityOutputTypeDef](./type_defs.md#custommessageactivityoutputtypedef) 
2. See [:material-code-braces: ConditionalSplitActivityTypeDef](./type_defs.md#conditionalsplitactivitytypedef) [:material-code-braces: ConditionalSplitActivityOutputTypeDef](./type_defs.md#conditionalsplitactivityoutputtypedef) 
3. See [:material-code-braces: EmailMessageActivityTypeDef](./type_defs.md#emailmessageactivitytypedef) 
4. See [:material-code-braces: HoldoutActivityTypeDef](./type_defs.md#holdoutactivitytypedef) 
5. See [:material-code-braces: MultiConditionalSplitActivityTypeDef](./type_defs.md#multiconditionalsplitactivitytypedef) [:material-code-braces: MultiConditionalSplitActivityOutputTypeDef](./type_defs.md#multiconditionalsplitactivityoutputtypedef) 
6. See [:material-code-braces: PushMessageActivityTypeDef](./type_defs.md#pushmessageactivitytypedef) 
7. See [:material-code-braces: RandomSplitActivityTypeDef](./type_defs.md#randomsplitactivitytypedef) [:material-code-braces: RandomSplitActivityOutputTypeDef](./type_defs.md#randomsplitactivityoutputtypedef) 
8. See [:material-code-braces: SMSMessageActivityTypeDef](./type_defs.md#smsmessageactivitytypedef) 
9. See [:material-code-braces: WaitActivityTypeDef](./type_defs.md#waitactivitytypedef) 
10. See [:material-code-braces: ContactCenterActivityTypeDef](./type_defs.md#contactcenteractivitytypedef) 
## WriteJourneyRequestTypeDef

```python
# WriteJourneyRequestTypeDef definition

class WriteJourneyRequestTypeDef(TypedDict):
    Name: str,
    Activities: NotRequired[Mapping[str, ActivityUnionTypeDef]],  # (1)
    CreationDate: NotRequired[str],
    LastModifiedDate: NotRequired[str],
    Limits: NotRequired[JourneyLimitsTypeDef],  # (2)
    LocalTime: NotRequired[bool],
    QuietTime: NotRequired[QuietTimeTypeDef],  # (3)
    RefreshFrequency: NotRequired[str],
    Schedule: NotRequired[JourneyScheduleUnionTypeDef],  # (4)
    StartActivity: NotRequired[str],
    StartCondition: NotRequired[StartConditionUnionTypeDef],  # (5)
    State: NotRequired[StateType],  # (6)
    WaitForQuietTime: NotRequired[bool],
    RefreshOnSegmentUpdate: NotRequired[bool],
    JourneyChannelSettings: NotRequired[JourneyChannelSettingsTypeDef],  # (7)
    SendingSchedule: NotRequired[bool],
    OpenHours: NotRequired[OpenHoursUnionTypeDef],  # (8)
    ClosedDays: NotRequired[ClosedDaysUnionTypeDef],  # (9)
    TimezoneEstimationMethods: NotRequired[Sequence[TimezoneEstimationMethodsElementType]],  # (10)
```

1. See [:material-code-braces: ActivityTypeDef](./type_defs.md#activitytypedef) [:material-code-braces: ActivityOutputTypeDef](./type_defs.md#activityoutputtypedef) 
2. See [:material-code-braces: JourneyLimitsTypeDef](./type_defs.md#journeylimitstypedef) 
3. See [:material-code-braces: QuietTimeTypeDef](./type_defs.md#quiettimetypedef) 
4. See [:material-code-braces: JourneyScheduleTypeDef](./type_defs.md#journeyscheduletypedef) [:material-code-braces: JourneyScheduleOutputTypeDef](./type_defs.md#journeyscheduleoutputtypedef) 
5. See [:material-code-braces: StartConditionTypeDef](./type_defs.md#startconditiontypedef) [:material-code-braces: StartConditionOutputTypeDef](./type_defs.md#startconditionoutputtypedef) 
6. See [:material-code-brackets: StateType](./literals.md#statetype) 
7. See [:material-code-braces: JourneyChannelSettingsTypeDef](./type_defs.md#journeychannelsettingstypedef) 
8. See [:material-code-braces: OpenHoursTypeDef](./type_defs.md#openhourstypedef) [:material-code-braces: OpenHoursOutputTypeDef](./type_defs.md#openhoursoutputtypedef) 
9. See [:material-code-braces: ClosedDaysTypeDef](./type_defs.md#closeddaystypedef) [:material-code-braces: ClosedDaysOutputTypeDef](./type_defs.md#closeddaysoutputtypedef) 
10. See [:material-code-brackets: TimezoneEstimationMethodsElementType](./literals.md#timezoneestimationmethodselementtype) 
## CreateJourneyRequestRequestTypeDef

```python
# CreateJourneyRequestRequestTypeDef definition

class CreateJourneyRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    WriteJourneyRequest: WriteJourneyRequestTypeDef,  # (1)
```

1. See [:material-code-braces: WriteJourneyRequestTypeDef](./type_defs.md#writejourneyrequesttypedef) 
## UpdateJourneyRequestRequestTypeDef

```python
# UpdateJourneyRequestRequestTypeDef definition

class UpdateJourneyRequestRequestTypeDef(TypedDict):
    ApplicationId: str,
    JourneyId: str,
    WriteJourneyRequest: WriteJourneyRequestTypeDef,  # (1)
```

1. See [:material-code-braces: WriteJourneyRequestTypeDef](./type_defs.md#writejourneyrequesttypedef) 

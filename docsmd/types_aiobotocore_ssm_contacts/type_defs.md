# Type definitions

> [Index](../README.md) > [SSMContacts](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SSMContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#ssmcontacts)
    type annotations stubs module [types-aiobotocore-ssm-contacts](https://pypi.org/project/types-aiobotocore-ssm-contacts/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## StageUnionTypeDef

```python
# StageUnionTypeDef definition

StageUnionTypeDef = Union[
    StageTypeDef,  # (1)
    StageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) 
2. See [:material-code-braces: StageOutputTypeDef](./type_defs.md#stageoutputtypedef) 



## AcceptPageRequestRequestTypeDef

```python
# AcceptPageRequestRequestTypeDef definition

class AcceptPageRequestRequestTypeDef(TypedDict):
    PageId: str,
    AcceptType: AcceptTypeType,  # (1)
    AcceptCode: str,
    ContactChannelId: NotRequired[str],
    Note: NotRequired[str],
    AcceptCodeValidation: NotRequired[AcceptCodeValidationType],  # (2)
```

1. See [:material-code-brackets: AcceptTypeType](./literals.md#accepttypetype) 
2. See [:material-code-brackets: AcceptCodeValidationType](./literals.md#acceptcodevalidationtype) 
## ActivateContactChannelRequestRequestTypeDef

```python
# ActivateContactChannelRequestRequestTypeDef definition

class ActivateContactChannelRequestRequestTypeDef(TypedDict):
    ContactChannelId: str,
    ActivationCode: str,
```

## ChannelTargetInfoTypeDef

```python
# ChannelTargetInfoTypeDef definition

class ChannelTargetInfoTypeDef(TypedDict):
    ContactChannelId: str,
    RetryIntervalInMinutes: NotRequired[int],
```

## ContactChannelAddressTypeDef

```python
# ContactChannelAddressTypeDef definition

class ContactChannelAddressTypeDef(TypedDict):
    SimpleAddress: NotRequired[str],
```

## ContactTargetInfoTypeDef

```python
# ContactTargetInfoTypeDef definition

class ContactTargetInfoTypeDef(TypedDict):
    IsEssential: bool,
    ContactId: NotRequired[str],
```

## ContactTypeDef

```python
# ContactTypeDef definition

class ContactTypeDef(TypedDict):
    ContactArn: str,
    Alias: str,
    Type: ContactTypeType,  # (1)
    DisplayName: NotRequired[str],
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
## HandOffTimeTypeDef

```python
# HandOffTimeTypeDef definition

class HandOffTimeTypeDef(TypedDict):
    HourOfDay: int,
    MinuteOfHour: int,
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

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## DeactivateContactChannelRequestRequestTypeDef

```python
# DeactivateContactChannelRequestRequestTypeDef definition

class DeactivateContactChannelRequestRequestTypeDef(TypedDict):
    ContactChannelId: str,
```

## DeleteContactChannelRequestRequestTypeDef

```python
# DeleteContactChannelRequestRequestTypeDef definition

class DeleteContactChannelRequestRequestTypeDef(TypedDict):
    ContactChannelId: str,
```

## DeleteContactRequestRequestTypeDef

```python
# DeleteContactRequestRequestTypeDef definition

class DeleteContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
```

## DeleteRotationOverrideRequestRequestTypeDef

```python
# DeleteRotationOverrideRequestRequestTypeDef definition

class DeleteRotationOverrideRequestRequestTypeDef(TypedDict):
    RotationId: str,
    RotationOverrideId: str,
```

## DeleteRotationRequestRequestTypeDef

```python
# DeleteRotationRequestRequestTypeDef definition

class DeleteRotationRequestRequestTypeDef(TypedDict):
    RotationId: str,
```

## DescribeEngagementRequestRequestTypeDef

```python
# DescribeEngagementRequestRequestTypeDef definition

class DescribeEngagementRequestRequestTypeDef(TypedDict):
    EngagementId: str,
```

## DescribePageRequestRequestTypeDef

```python
# DescribePageRequestRequestTypeDef definition

class DescribePageRequestRequestTypeDef(TypedDict):
    PageId: str,
```

## EngagementTypeDef

```python
# EngagementTypeDef definition

class EngagementTypeDef(TypedDict):
    EngagementArn: str,
    ContactArn: str,
    Sender: str,
    IncidentId: NotRequired[str],
    StartTime: NotRequired[datetime],
    StopTime: NotRequired[datetime],
```

## GetContactChannelRequestRequestTypeDef

```python
# GetContactChannelRequestRequestTypeDef definition

class GetContactChannelRequestRequestTypeDef(TypedDict):
    ContactChannelId: str,
```

## GetContactPolicyRequestRequestTypeDef

```python
# GetContactPolicyRequestRequestTypeDef definition

class GetContactPolicyRequestRequestTypeDef(TypedDict):
    ContactArn: str,
```

## GetContactRequestRequestTypeDef

```python
# GetContactRequestRequestTypeDef definition

class GetContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
```

## GetRotationOverrideRequestRequestTypeDef

```python
# GetRotationOverrideRequestRequestTypeDef definition

class GetRotationOverrideRequestRequestTypeDef(TypedDict):
    RotationId: str,
    RotationOverrideId: str,
```

## GetRotationRequestRequestTypeDef

```python
# GetRotationRequestRequestTypeDef definition

class GetRotationRequestRequestTypeDef(TypedDict):
    RotationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListContactChannelsRequestRequestTypeDef

```python
# ListContactChannelsRequestRequestTypeDef definition

class ListContactChannelsRequestRequestTypeDef(TypedDict):
    ContactId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListContactsRequestRequestTypeDef

```python
# ListContactsRequestRequestTypeDef definition

class ListContactsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    AliasPrefix: NotRequired[str],
    Type: NotRequired[ContactTypeType],  # (1)
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
## ListPageReceiptsRequestRequestTypeDef

```python
# ListPageReceiptsRequestRequestTypeDef definition

class ListPageReceiptsRequestRequestTypeDef(TypedDict):
    PageId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ReceiptTypeDef

```python
# ReceiptTypeDef definition

class ReceiptTypeDef(TypedDict):
    ReceiptType: ReceiptTypeType,  # (1)
    ReceiptTime: datetime,
    ContactChannelArn: NotRequired[str],
    ReceiptInfo: NotRequired[str],
```

1. See [:material-code-brackets: ReceiptTypeType](./literals.md#receipttypetype) 
## ListPageResolutionsRequestRequestTypeDef

```python
# ListPageResolutionsRequestRequestTypeDef definition

class ListPageResolutionsRequestRequestTypeDef(TypedDict):
    PageId: str,
    NextToken: NotRequired[str],
```

## ResolutionContactTypeDef

```python
# ResolutionContactTypeDef definition

class ResolutionContactTypeDef(TypedDict):
    ContactArn: str,
    Type: ContactTypeType,  # (1)
    StageIndex: NotRequired[int],
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
## ListPagesByContactRequestRequestTypeDef

```python
# ListPagesByContactRequestRequestTypeDef definition

class ListPagesByContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PageTypeDef

```python
# PageTypeDef definition

class PageTypeDef(TypedDict):
    PageArn: str,
    EngagementArn: str,
    ContactArn: str,
    Sender: str,
    IncidentId: NotRequired[str],
    SentTime: NotRequired[datetime],
    DeliveryTime: NotRequired[datetime],
    ReadTime: NotRequired[datetime],
```

## ListPagesByEngagementRequestRequestTypeDef

```python
# ListPagesByEngagementRequestRequestTypeDef definition

class ListPagesByEngagementRequestRequestTypeDef(TypedDict):
    EngagementId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RotationOverrideTypeDef

```python
# RotationOverrideTypeDef definition

class RotationOverrideTypeDef(TypedDict):
    RotationOverrideId: str,
    NewContactIds: List[str],
    StartTime: datetime,
    EndTime: datetime,
    CreateTime: datetime,
```

## ListRotationsRequestRequestTypeDef

```python
# ListRotationsRequestRequestTypeDef definition

class ListRotationsRequestRequestTypeDef(TypedDict):
    RotationNamePrefix: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## PutContactPolicyRequestRequestTypeDef

```python
# PutContactPolicyRequestRequestTypeDef definition

class PutContactPolicyRequestRequestTypeDef(TypedDict):
    ContactArn: str,
    Policy: str,
```

## ShiftDetailsTypeDef

```python
# ShiftDetailsTypeDef definition

class ShiftDetailsTypeDef(TypedDict):
    OverriddenContactIds: List[str],
```

## SendActivationCodeRequestRequestTypeDef

```python
# SendActivationCodeRequestRequestTypeDef definition

class SendActivationCodeRequestRequestTypeDef(TypedDict):
    ContactChannelId: str,
```

## StartEngagementRequestRequestTypeDef

```python
# StartEngagementRequestRequestTypeDef definition

class StartEngagementRequestRequestTypeDef(TypedDict):
    ContactId: str,
    Sender: str,
    Subject: str,
    Content: str,
    PublicSubject: NotRequired[str],
    PublicContent: NotRequired[str],
    IncidentId: NotRequired[str],
    IdempotencyToken: NotRequired[str],
```

## StopEngagementRequestRequestTypeDef

```python
# StopEngagementRequestRequestTypeDef definition

class StopEngagementRequestRequestTypeDef(TypedDict):
    EngagementId: str,
    Reason: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## ContactChannelTypeDef

```python
# ContactChannelTypeDef definition

class ContactChannelTypeDef(TypedDict):
    ContactChannelArn: str,
    ContactArn: str,
    Name: str,
    DeliveryAddress: ContactChannelAddressTypeDef,  # (2)
    ActivationStatus: ActivationStatusType,  # (3)
    Type: NotRequired[ChannelTypeType],  # (1)
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: ContactChannelAddressTypeDef](./type_defs.md#contactchanneladdresstypedef) 
3. See [:material-code-brackets: ActivationStatusType](./literals.md#activationstatustype) 
## CreateContactChannelRequestRequestTypeDef

```python
# CreateContactChannelRequestRequestTypeDef definition

class CreateContactChannelRequestRequestTypeDef(TypedDict):
    ContactId: str,
    Name: str,
    Type: ChannelTypeType,  # (1)
    DeliveryAddress: ContactChannelAddressTypeDef,  # (2)
    DeferActivation: NotRequired[bool],
    IdempotencyToken: NotRequired[str],
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: ContactChannelAddressTypeDef](./type_defs.md#contactchanneladdresstypedef) 
## UpdateContactChannelRequestRequestTypeDef

```python
# UpdateContactChannelRequestRequestTypeDef definition

class UpdateContactChannelRequestRequestTypeDef(TypedDict):
    ContactChannelId: str,
    Name: NotRequired[str],
    DeliveryAddress: NotRequired[ContactChannelAddressTypeDef],  # (1)
```

1. See [:material-code-braces: ContactChannelAddressTypeDef](./type_defs.md#contactchanneladdresstypedef) 
## TargetTypeDef

```python
# TargetTypeDef definition

class TargetTypeDef(TypedDict):
    ChannelTargetInfo: NotRequired[ChannelTargetInfoTypeDef],  # (1)
    ContactTargetInfo: NotRequired[ContactTargetInfoTypeDef],  # (2)
```

1. See [:material-code-braces: ChannelTargetInfoTypeDef](./type_defs.md#channeltargetinfotypedef) 
2. See [:material-code-braces: ContactTargetInfoTypeDef](./type_defs.md#contacttargetinfotypedef) 
## CoverageTimeTypeDef

```python
# CoverageTimeTypeDef definition

class CoverageTimeTypeDef(TypedDict):
    Start: NotRequired[HandOffTimeTypeDef],  # (1)
    End: NotRequired[HandOffTimeTypeDef],  # (1)
```

1. See [:material-code-braces: HandOffTimeTypeDef](./type_defs.md#handofftimetypedef) 
2. See [:material-code-braces: HandOffTimeTypeDef](./type_defs.md#handofftimetypedef) 
## MonthlySettingTypeDef

```python
# MonthlySettingTypeDef definition

class MonthlySettingTypeDef(TypedDict):
    DayOfMonth: int,
    HandOffTime: HandOffTimeTypeDef,  # (1)
```

1. See [:material-code-braces: HandOffTimeTypeDef](./type_defs.md#handofftimetypedef) 
## WeeklySettingTypeDef

```python
# WeeklySettingTypeDef definition

class WeeklySettingTypeDef(TypedDict):
    DayOfWeek: DayOfWeekType,  # (1)
    HandOffTime: HandOffTimeTypeDef,  # (2)
```

1. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) 
2. See [:material-code-braces: HandOffTimeTypeDef](./type_defs.md#handofftimetypedef) 
## CreateContactChannelResultTypeDef

```python
# CreateContactChannelResultTypeDef definition

class CreateContactChannelResultTypeDef(TypedDict):
    ContactChannelArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactResultTypeDef

```python
# CreateContactResultTypeDef definition

class CreateContactResultTypeDef(TypedDict):
    ContactArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRotationOverrideResultTypeDef

```python
# CreateRotationOverrideResultTypeDef definition

class CreateRotationOverrideResultTypeDef(TypedDict):
    RotationOverrideId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRotationResultTypeDef

```python
# CreateRotationResultTypeDef definition

class CreateRotationResultTypeDef(TypedDict):
    RotationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEngagementResultTypeDef

```python
# DescribeEngagementResultTypeDef definition

class DescribeEngagementResultTypeDef(TypedDict):
    ContactArn: str,
    EngagementArn: str,
    Sender: str,
    Subject: str,
    Content: str,
    PublicSubject: str,
    PublicContent: str,
    IncidentId: str,
    StartTime: datetime,
    StopTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePageResultTypeDef

```python
# DescribePageResultTypeDef definition

class DescribePageResultTypeDef(TypedDict):
    PageArn: str,
    EngagementArn: str,
    ContactArn: str,
    Sender: str,
    Subject: str,
    Content: str,
    PublicSubject: str,
    PublicContent: str,
    IncidentId: str,
    SentTime: datetime,
    ReadTime: datetime,
    DeliveryTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContactChannelResultTypeDef

```python
# GetContactChannelResultTypeDef definition

class GetContactChannelResultTypeDef(TypedDict):
    ContactArn: str,
    ContactChannelArn: str,
    Name: str,
    Type: ChannelTypeType,  # (1)
    DeliveryAddress: ContactChannelAddressTypeDef,  # (2)
    ActivationStatus: ActivationStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ChannelTypeType](./literals.md#channeltypetype) 
2. See [:material-code-braces: ContactChannelAddressTypeDef](./type_defs.md#contactchanneladdresstypedef) 
3. See [:material-code-brackets: ActivationStatusType](./literals.md#activationstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetContactPolicyResultTypeDef

```python
# GetContactPolicyResultTypeDef definition

class GetContactPolicyResultTypeDef(TypedDict):
    ContactArn: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRotationOverrideResultTypeDef

```python
# GetRotationOverrideResultTypeDef definition

class GetRotationOverrideResultTypeDef(TypedDict):
    RotationOverrideId: str,
    RotationArn: str,
    NewContactIds: List[str],
    StartTime: datetime,
    EndTime: datetime,
    CreateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContactsResultTypeDef

```python
# ListContactsResultTypeDef definition

class ListContactsResultTypeDef(TypedDict):
    Contacts: List[ContactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartEngagementResultTypeDef

```python
# StartEngagementResultTypeDef definition

class StartEngagementResultTypeDef(TypedDict):
    EngagementArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResultTypeDef

```python
# ListTagsForResourceResultTypeDef definition

class ListTagsForResourceResultTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRotationOverrideRequestRequestTypeDef

```python
# CreateRotationOverrideRequestRequestTypeDef definition

class CreateRotationOverrideRequestRequestTypeDef(TypedDict):
    RotationId: str,
    NewContactIds: Sequence[str],
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    IdempotencyToken: NotRequired[str],
```

## ListRotationOverridesRequestRequestTypeDef

```python
# ListRotationOverridesRequestRequestTypeDef definition

class ListRotationOverridesRequestRequestTypeDef(TypedDict):
    RotationId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListRotationShiftsRequestRequestTypeDef

```python
# ListRotationShiftsRequestRequestTypeDef definition

class ListRotationShiftsRequestRequestTypeDef(TypedDict):
    RotationId: str,
    EndTime: TimestampTypeDef,
    StartTime: NotRequired[TimestampTypeDef],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PreviewOverrideTypeDef

```python
# PreviewOverrideTypeDef definition

class PreviewOverrideTypeDef(TypedDict):
    NewMembers: NotRequired[Sequence[str]],
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
```

## TimeRangeTypeDef

```python
# TimeRangeTypeDef definition

class TimeRangeTypeDef(TypedDict):
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
```

## ListEngagementsResultTypeDef

```python
# ListEngagementsResultTypeDef definition

class ListEngagementsResultTypeDef(TypedDict):
    Engagements: List[EngagementTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EngagementTypeDef](./type_defs.md#engagementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContactChannelsRequestPaginateTypeDef

```python
# ListContactChannelsRequestPaginateTypeDef definition

class ListContactChannelsRequestPaginateTypeDef(TypedDict):
    ContactId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListContactsRequestPaginateTypeDef

```python
# ListContactsRequestPaginateTypeDef definition

class ListContactsRequestPaginateTypeDef(TypedDict):
    AliasPrefix: NotRequired[str],
    Type: NotRequired[ContactTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPageReceiptsRequestPaginateTypeDef

```python
# ListPageReceiptsRequestPaginateTypeDef definition

class ListPageReceiptsRequestPaginateTypeDef(TypedDict):
    PageId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPageResolutionsRequestPaginateTypeDef

```python
# ListPageResolutionsRequestPaginateTypeDef definition

class ListPageResolutionsRequestPaginateTypeDef(TypedDict):
    PageId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPagesByContactRequestPaginateTypeDef

```python
# ListPagesByContactRequestPaginateTypeDef definition

class ListPagesByContactRequestPaginateTypeDef(TypedDict):
    ContactId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPagesByEngagementRequestPaginateTypeDef

```python
# ListPagesByEngagementRequestPaginateTypeDef definition

class ListPagesByEngagementRequestPaginateTypeDef(TypedDict):
    EngagementId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRotationOverridesRequestPaginateTypeDef

```python
# ListRotationOverridesRequestPaginateTypeDef definition

class ListRotationOverridesRequestPaginateTypeDef(TypedDict):
    RotationId: str,
    StartTime: TimestampTypeDef,
    EndTime: TimestampTypeDef,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRotationShiftsRequestPaginateTypeDef

```python
# ListRotationShiftsRequestPaginateTypeDef definition

class ListRotationShiftsRequestPaginateTypeDef(TypedDict):
    RotationId: str,
    EndTime: TimestampTypeDef,
    StartTime: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRotationsRequestPaginateTypeDef

```python
# ListRotationsRequestPaginateTypeDef definition

class ListRotationsRequestPaginateTypeDef(TypedDict):
    RotationNamePrefix: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPageReceiptsResultTypeDef

```python
# ListPageReceiptsResultTypeDef definition

class ListPageReceiptsResultTypeDef(TypedDict):
    Receipts: List[ReceiptTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReceiptTypeDef](./type_defs.md#receipttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPageResolutionsResultTypeDef

```python
# ListPageResolutionsResultTypeDef definition

class ListPageResolutionsResultTypeDef(TypedDict):
    PageResolutions: List[ResolutionContactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResolutionContactTypeDef](./type_defs.md#resolutioncontacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPagesByContactResultTypeDef

```python
# ListPagesByContactResultTypeDef definition

class ListPagesByContactResultTypeDef(TypedDict):
    Pages: List[PageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PageTypeDef](./type_defs.md#pagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPagesByEngagementResultTypeDef

```python
# ListPagesByEngagementResultTypeDef definition

class ListPagesByEngagementResultTypeDef(TypedDict):
    Pages: List[PageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PageTypeDef](./type_defs.md#pagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRotationOverridesResultTypeDef

```python
# ListRotationOverridesResultTypeDef definition

class ListRotationOverridesResultTypeDef(TypedDict):
    RotationOverrides: List[RotationOverrideTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RotationOverrideTypeDef](./type_defs.md#rotationoverridetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotationShiftTypeDef

```python
# RotationShiftTypeDef definition

class RotationShiftTypeDef(TypedDict):
    StartTime: datetime,
    EndTime: datetime,
    ContactIds: NotRequired[List[str]],
    Type: NotRequired[ShiftTypeType],  # (1)
    ShiftDetails: NotRequired[ShiftDetailsTypeDef],  # (2)
```

1. See [:material-code-brackets: ShiftTypeType](./literals.md#shifttypetype) 
2. See [:material-code-braces: ShiftDetailsTypeDef](./type_defs.md#shiftdetailstypedef) 
## ListContactChannelsResultTypeDef

```python
# ListContactChannelsResultTypeDef definition

class ListContactChannelsResultTypeDef(TypedDict):
    ContactChannels: List[ContactChannelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ContactChannelTypeDef](./type_defs.md#contactchanneltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StageOutputTypeDef

```python
# StageOutputTypeDef definition

class StageOutputTypeDef(TypedDict):
    DurationInMinutes: int,
    Targets: List[TargetTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## StageTypeDef

```python
# StageTypeDef definition

class StageTypeDef(TypedDict):
    DurationInMinutes: int,
    Targets: Sequence[TargetTypeDef],  # (1)
```

1. See [:material-code-braces: TargetTypeDef](./type_defs.md#targettypedef) 
## RecurrenceSettingsOutputTypeDef

```python
# RecurrenceSettingsOutputTypeDef definition

class RecurrenceSettingsOutputTypeDef(TypedDict):
    NumberOfOnCalls: int,
    RecurrenceMultiplier: int,
    MonthlySettings: NotRequired[List[MonthlySettingTypeDef]],  # (1)
    WeeklySettings: NotRequired[List[WeeklySettingTypeDef]],  # (2)
    DailySettings: NotRequired[List[HandOffTimeTypeDef]],  # (3)
    ShiftCoverages: NotRequired[Dict[DayOfWeekType, List[CoverageTimeTypeDef]]],  # (4)
```

1. See [:material-code-braces: MonthlySettingTypeDef](./type_defs.md#monthlysettingtypedef) 
2. See [:material-code-braces: WeeklySettingTypeDef](./type_defs.md#weeklysettingtypedef) 
3. See [:material-code-braces: HandOffTimeTypeDef](./type_defs.md#handofftimetypedef) 
4. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: CoverageTimeTypeDef](./type_defs.md#coveragetimetypedef) 
## RecurrenceSettingsTypeDef

```python
# RecurrenceSettingsTypeDef definition

class RecurrenceSettingsTypeDef(TypedDict):
    NumberOfOnCalls: int,
    RecurrenceMultiplier: int,
    MonthlySettings: NotRequired[Sequence[MonthlySettingTypeDef]],  # (1)
    WeeklySettings: NotRequired[Sequence[WeeklySettingTypeDef]],  # (2)
    DailySettings: NotRequired[Sequence[HandOffTimeTypeDef]],  # (3)
    ShiftCoverages: NotRequired[Mapping[DayOfWeekType, Sequence[CoverageTimeTypeDef]]],  # (4)
```

1. See [:material-code-braces: MonthlySettingTypeDef](./type_defs.md#monthlysettingtypedef) 
2. See [:material-code-braces: WeeklySettingTypeDef](./type_defs.md#weeklysettingtypedef) 
3. See [:material-code-braces: HandOffTimeTypeDef](./type_defs.md#handofftimetypedef) 
4. See [:material-code-brackets: DayOfWeekType](./literals.md#dayofweektype) [:material-code-braces: CoverageTimeTypeDef](./type_defs.md#coveragetimetypedef) 
## ListEngagementsRequestPaginateTypeDef

```python
# ListEngagementsRequestPaginateTypeDef definition

class ListEngagementsRequestPaginateTypeDef(TypedDict):
    IncidentId: NotRequired[str],
    TimeRangeValue: NotRequired[TimeRangeTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEngagementsRequestRequestTypeDef

```python
# ListEngagementsRequestRequestTypeDef definition

class ListEngagementsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    IncidentId: NotRequired[str],
    TimeRangeValue: NotRequired[TimeRangeTypeDef],  # (1)
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
## ListPreviewRotationShiftsResultTypeDef

```python
# ListPreviewRotationShiftsResultTypeDef definition

class ListPreviewRotationShiftsResultTypeDef(TypedDict):
    RotationShifts: List[RotationShiftTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RotationShiftTypeDef](./type_defs.md#rotationshifttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRotationShiftsResultTypeDef

```python
# ListRotationShiftsResultTypeDef definition

class ListRotationShiftsResultTypeDef(TypedDict):
    RotationShifts: List[RotationShiftTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RotationShiftTypeDef](./type_defs.md#rotationshifttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PlanOutputTypeDef

```python
# PlanOutputTypeDef definition

class PlanOutputTypeDef(TypedDict):
    Stages: NotRequired[List[StageOutputTypeDef]],  # (1)
    RotationIds: NotRequired[List[str]],
```

1. See [:material-code-braces: StageOutputTypeDef](./type_defs.md#stageoutputtypedef) 
## GetRotationResultTypeDef

```python
# GetRotationResultTypeDef definition

class GetRotationResultTypeDef(TypedDict):
    RotationArn: str,
    Name: str,
    ContactIds: List[str],
    StartTime: datetime,
    TimeZoneId: str,
    Recurrence: RecurrenceSettingsOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecurrenceSettingsOutputTypeDef](./type_defs.md#recurrencesettingsoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RotationTypeDef

```python
# RotationTypeDef definition

class RotationTypeDef(TypedDict):
    RotationArn: str,
    Name: str,
    ContactIds: NotRequired[List[str]],
    StartTime: NotRequired[datetime],
    TimeZoneId: NotRequired[str],
    Recurrence: NotRequired[RecurrenceSettingsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: RecurrenceSettingsOutputTypeDef](./type_defs.md#recurrencesettingsoutputtypedef) 
## CreateRotationRequestRequestTypeDef

```python
# CreateRotationRequestRequestTypeDef definition

class CreateRotationRequestRequestTypeDef(TypedDict):
    Name: str,
    ContactIds: Sequence[str],
    TimeZoneId: str,
    Recurrence: RecurrenceSettingsTypeDef,  # (1)
    StartTime: NotRequired[TimestampTypeDef],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    IdempotencyToken: NotRequired[str],
```

1. See [:material-code-braces: RecurrenceSettingsTypeDef](./type_defs.md#recurrencesettingstypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListPreviewRotationShiftsRequestPaginateTypeDef

```python
# ListPreviewRotationShiftsRequestPaginateTypeDef definition

class ListPreviewRotationShiftsRequestPaginateTypeDef(TypedDict):
    EndTime: TimestampTypeDef,
    Members: Sequence[str],
    TimeZoneId: str,
    Recurrence: RecurrenceSettingsTypeDef,  # (1)
    RotationStartTime: NotRequired[TimestampTypeDef],
    StartTime: NotRequired[TimestampTypeDef],
    Overrides: NotRequired[Sequence[PreviewOverrideTypeDef]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: RecurrenceSettingsTypeDef](./type_defs.md#recurrencesettingstypedef) 
2. See [:material-code-braces: PreviewOverrideTypeDef](./type_defs.md#previewoverridetypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPreviewRotationShiftsRequestRequestTypeDef

```python
# ListPreviewRotationShiftsRequestRequestTypeDef definition

class ListPreviewRotationShiftsRequestRequestTypeDef(TypedDict):
    EndTime: TimestampTypeDef,
    Members: Sequence[str],
    TimeZoneId: str,
    Recurrence: RecurrenceSettingsTypeDef,  # (1)
    RotationStartTime: NotRequired[TimestampTypeDef],
    StartTime: NotRequired[TimestampTypeDef],
    Overrides: NotRequired[Sequence[PreviewOverrideTypeDef]],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: RecurrenceSettingsTypeDef](./type_defs.md#recurrencesettingstypedef) 
2. See [:material-code-braces: PreviewOverrideTypeDef](./type_defs.md#previewoverridetypedef) 
## UpdateRotationRequestRequestTypeDef

```python
# UpdateRotationRequestRequestTypeDef definition

class UpdateRotationRequestRequestTypeDef(TypedDict):
    RotationId: str,
    Recurrence: RecurrenceSettingsTypeDef,  # (1)
    ContactIds: NotRequired[Sequence[str]],
    StartTime: NotRequired[TimestampTypeDef],
    TimeZoneId: NotRequired[str],
```

1. See [:material-code-braces: RecurrenceSettingsTypeDef](./type_defs.md#recurrencesettingstypedef) 
## GetContactResultTypeDef

```python
# GetContactResultTypeDef definition

class GetContactResultTypeDef(TypedDict):
    ContactArn: str,
    Alias: str,
    DisplayName: str,
    Type: ContactTypeType,  # (1)
    Plan: PlanOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
2. See [:material-code-braces: PlanOutputTypeDef](./type_defs.md#planoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PlanTypeDef

```python
# PlanTypeDef definition

class PlanTypeDef(TypedDict):
    Stages: NotRequired[Sequence[StageUnionTypeDef]],  # (1)
    RotationIds: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: StageTypeDef](./type_defs.md#stagetypedef) [:material-code-braces: StageOutputTypeDef](./type_defs.md#stageoutputtypedef) 
## ListRotationsResultTypeDef

```python
# ListRotationsResultTypeDef definition

class ListRotationsResultTypeDef(TypedDict):
    Rotations: List[RotationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RotationTypeDef](./type_defs.md#rotationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateContactRequestRequestTypeDef

```python
# CreateContactRequestRequestTypeDef definition

class CreateContactRequestRequestTypeDef(TypedDict):
    Alias: str,
    Type: ContactTypeType,  # (1)
    Plan: PlanTypeDef,  # (2)
    DisplayName: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    IdempotencyToken: NotRequired[str],
```

1. See [:material-code-brackets: ContactTypeType](./literals.md#contacttypetype) 
2. See [:material-code-braces: PlanTypeDef](./type_defs.md#plantypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateContactRequestRequestTypeDef

```python
# UpdateContactRequestRequestTypeDef definition

class UpdateContactRequestRequestTypeDef(TypedDict):
    ContactId: str,
    DisplayName: NotRequired[str],
    Plan: NotRequired[PlanTypeDef],  # (1)
```

1. See [:material-code-braces: PlanTypeDef](./type_defs.md#plantypedef) 

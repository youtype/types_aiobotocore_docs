# Type definitions

> [Index](../README.md) > [VoiceID](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [VoiceID](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/voice-id.html#VoiceID)
    type annotations stubs module [types-aiobotocore-voice-id](https://pypi.org/project/types-aiobotocore-voice-id/).

## EnrollmentJobFraudDetectionConfigUnionTypeDef

```python
# EnrollmentJobFraudDetectionConfigUnionTypeDef definition

EnrollmentJobFraudDetectionConfigUnionTypeDef = Union[
    EnrollmentJobFraudDetectionConfigTypeDef,  # (1)
    EnrollmentJobFraudDetectionConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EnrollmentJobFraudDetectionConfigTypeDef](./type_defs.md#enrollmentjobfrauddetectionconfigtypedef) 
2. See [:material-code-braces: EnrollmentJobFraudDetectionConfigOutputTypeDef](./type_defs.md#enrollmentjobfrauddetectionconfigoutputtypedef) 



## AssociateFraudsterRequestRequestTypeDef

```python
# AssociateFraudsterRequestRequestTypeDef definition

class AssociateFraudsterRequestRequestTypeDef(TypedDict):
    DomainId: str,
    FraudsterId: str,
    WatchlistId: str,
```

## FraudsterTypeDef

```python
# FraudsterTypeDef definition

class FraudsterTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    DomainId: NotRequired[str],
    GeneratedFraudsterId: NotRequired[str],
    WatchlistIds: NotRequired[List[str]],
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

## AuthenticationConfigurationTypeDef

```python
# AuthenticationConfigurationTypeDef definition

class AuthenticationConfigurationTypeDef(TypedDict):
    AcceptanceThreshold: int,
```

## ServerSideEncryptionConfigurationTypeDef

```python
# ServerSideEncryptionConfigurationTypeDef definition

class ServerSideEncryptionConfigurationTypeDef(TypedDict):
    KmsKeyId: str,
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## CreateWatchlistRequestRequestTypeDef

```python
# CreateWatchlistRequestRequestTypeDef definition

class CreateWatchlistRequestRequestTypeDef(TypedDict):
    DomainId: str,
    Name: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
```

## WatchlistTypeDef

```python
# WatchlistTypeDef definition

class WatchlistTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    DefaultWatchlist: NotRequired[bool],
    Description: NotRequired[str],
    DomainId: NotRequired[str],
    Name: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
    WatchlistId: NotRequired[str],
```

## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    DomainId: str,
```

## DeleteFraudsterRequestRequestTypeDef

```python
# DeleteFraudsterRequestRequestTypeDef definition

class DeleteFraudsterRequestRequestTypeDef(TypedDict):
    DomainId: str,
    FraudsterId: str,
```

## DeleteSpeakerRequestRequestTypeDef

```python
# DeleteSpeakerRequestRequestTypeDef definition

class DeleteSpeakerRequestRequestTypeDef(TypedDict):
    DomainId: str,
    SpeakerId: str,
```

## DeleteWatchlistRequestRequestTypeDef

```python
# DeleteWatchlistRequestRequestTypeDef definition

class DeleteWatchlistRequestRequestTypeDef(TypedDict):
    DomainId: str,
    WatchlistId: str,
```

## DescribeDomainRequestRequestTypeDef

```python
# DescribeDomainRequestRequestTypeDef definition

class DescribeDomainRequestRequestTypeDef(TypedDict):
    DomainId: str,
```

## DescribeFraudsterRegistrationJobRequestRequestTypeDef

```python
# DescribeFraudsterRegistrationJobRequestRequestTypeDef definition

class DescribeFraudsterRegistrationJobRequestRequestTypeDef(TypedDict):
    DomainId: str,
    JobId: str,
```

## DescribeFraudsterRequestRequestTypeDef

```python
# DescribeFraudsterRequestRequestTypeDef definition

class DescribeFraudsterRequestRequestTypeDef(TypedDict):
    DomainId: str,
    FraudsterId: str,
```

## DescribeSpeakerEnrollmentJobRequestRequestTypeDef

```python
# DescribeSpeakerEnrollmentJobRequestRequestTypeDef definition

class DescribeSpeakerEnrollmentJobRequestRequestTypeDef(TypedDict):
    DomainId: str,
    JobId: str,
```

## DescribeSpeakerRequestRequestTypeDef

```python
# DescribeSpeakerRequestRequestTypeDef definition

class DescribeSpeakerRequestRequestTypeDef(TypedDict):
    DomainId: str,
    SpeakerId: str,
```

## SpeakerTypeDef

```python
# SpeakerTypeDef definition

class SpeakerTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    CustomerSpeakerId: NotRequired[str],
    DomainId: NotRequired[str],
    GeneratedSpeakerId: NotRequired[str],
    LastAccessedAt: NotRequired[datetime],
    Status: NotRequired[SpeakerStatusType],  # (1)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: SpeakerStatusType](./literals.md#speakerstatustype) 
## DescribeWatchlistRequestRequestTypeDef

```python
# DescribeWatchlistRequestRequestTypeDef definition

class DescribeWatchlistRequestRequestTypeDef(TypedDict):
    DomainId: str,
    WatchlistId: str,
```

## DisassociateFraudsterRequestRequestTypeDef

```python
# DisassociateFraudsterRequestRequestTypeDef definition

class DisassociateFraudsterRequestRequestTypeDef(TypedDict):
    DomainId: str,
    FraudsterId: str,
    WatchlistId: str,
```

## ServerSideEncryptionUpdateDetailsTypeDef

```python
# ServerSideEncryptionUpdateDetailsTypeDef definition

class ServerSideEncryptionUpdateDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
    OldKmsKeyId: NotRequired[str],
    UpdateStatus: NotRequired[ServerSideEncryptionUpdateStatusType],  # (1)
```

1. See [:material-code-brackets: ServerSideEncryptionUpdateStatusType](./literals.md#serversideencryptionupdatestatustype) 
## WatchlistDetailsTypeDef

```python
# WatchlistDetailsTypeDef definition

class WatchlistDetailsTypeDef(TypedDict):
    DefaultWatchlistId: str,
```

## EnrollmentJobFraudDetectionConfigOutputTypeDef

```python
# EnrollmentJobFraudDetectionConfigOutputTypeDef definition

class EnrollmentJobFraudDetectionConfigOutputTypeDef(TypedDict):
    FraudDetectionAction: NotRequired[FraudDetectionActionType],  # (1)
    RiskThreshold: NotRequired[int],
    WatchlistIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: FraudDetectionActionType](./literals.md#frauddetectionactiontype) 
## EnrollmentJobFraudDetectionConfigTypeDef

```python
# EnrollmentJobFraudDetectionConfigTypeDef definition

class EnrollmentJobFraudDetectionConfigTypeDef(TypedDict):
    FraudDetectionAction: NotRequired[FraudDetectionActionType],  # (1)
    RiskThreshold: NotRequired[int],
    WatchlistIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: FraudDetectionActionType](./literals.md#frauddetectionactiontype) 
## EvaluateSessionRequestRequestTypeDef

```python
# EvaluateSessionRequestRequestTypeDef definition

class EvaluateSessionRequestRequestTypeDef(TypedDict):
    DomainId: str,
    SessionNameOrId: str,
```

## FailureDetailsTypeDef

```python
# FailureDetailsTypeDef definition

class FailureDetailsTypeDef(TypedDict):
    Message: NotRequired[str],
    StatusCode: NotRequired[int],
```

## FraudDetectionConfigurationTypeDef

```python
# FraudDetectionConfigurationTypeDef definition

class FraudDetectionConfigurationTypeDef(TypedDict):
    RiskThreshold: NotRequired[int],
    WatchlistId: NotRequired[str],
```

## KnownFraudsterRiskTypeDef

```python
# KnownFraudsterRiskTypeDef definition

class KnownFraudsterRiskTypeDef(TypedDict):
    RiskScore: int,
    GeneratedFraudsterId: NotRequired[str],
```

## VoiceSpoofingRiskTypeDef

```python
# VoiceSpoofingRiskTypeDef definition

class VoiceSpoofingRiskTypeDef(TypedDict):
    RiskScore: int,
```

## JobProgressTypeDef

```python
# JobProgressTypeDef definition

class JobProgressTypeDef(TypedDict):
    PercentComplete: NotRequired[int],
```

## InputDataConfigTypeDef

```python
# InputDataConfigTypeDef definition

class InputDataConfigTypeDef(TypedDict):
    S3Uri: str,
```

## OutputDataConfigTypeDef

```python
# OutputDataConfigTypeDef definition

class OutputDataConfigTypeDef(TypedDict):
    S3Uri: str,
    KmsKeyId: NotRequired[str],
```

## RegistrationConfigOutputTypeDef

```python
# RegistrationConfigOutputTypeDef definition

class RegistrationConfigOutputTypeDef(TypedDict):
    DuplicateRegistrationAction: NotRequired[DuplicateRegistrationActionType],  # (1)
    FraudsterSimilarityThreshold: NotRequired[int],
    WatchlistIds: NotRequired[List[str]],
```

1. See [:material-code-brackets: DuplicateRegistrationActionType](./literals.md#duplicateregistrationactiontype) 
## FraudsterSummaryTypeDef

```python
# FraudsterSummaryTypeDef definition

class FraudsterSummaryTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    DomainId: NotRequired[str],
    GeneratedFraudsterId: NotRequired[str],
    WatchlistIds: NotRequired[List[str]],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFraudsterRegistrationJobsRequestRequestTypeDef

```python
# ListFraudsterRegistrationJobsRequestRequestTypeDef definition

class ListFraudsterRegistrationJobsRequestRequestTypeDef(TypedDict):
    DomainId: str,
    JobStatus: NotRequired[FraudsterRegistrationJobStatusType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: FraudsterRegistrationJobStatusType](./literals.md#fraudsterregistrationjobstatustype) 
## ListFraudstersRequestRequestTypeDef

```python
# ListFraudstersRequestRequestTypeDef definition

class ListFraudstersRequestRequestTypeDef(TypedDict):
    DomainId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    WatchlistId: NotRequired[str],
```

## ListSpeakerEnrollmentJobsRequestRequestTypeDef

```python
# ListSpeakerEnrollmentJobsRequestRequestTypeDef definition

class ListSpeakerEnrollmentJobsRequestRequestTypeDef(TypedDict):
    DomainId: str,
    JobStatus: NotRequired[SpeakerEnrollmentJobStatusType],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: SpeakerEnrollmentJobStatusType](./literals.md#speakerenrollmentjobstatustype) 
## ListSpeakersRequestRequestTypeDef

```python
# ListSpeakersRequestRequestTypeDef definition

class ListSpeakersRequestRequestTypeDef(TypedDict):
    DomainId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SpeakerSummaryTypeDef

```python
# SpeakerSummaryTypeDef definition

class SpeakerSummaryTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    CustomerSpeakerId: NotRequired[str],
    DomainId: NotRequired[str],
    GeneratedSpeakerId: NotRequired[str],
    LastAccessedAt: NotRequired[datetime],
    Status: NotRequired[SpeakerStatusType],  # (1)
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: SpeakerStatusType](./literals.md#speakerstatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListWatchlistsRequestRequestTypeDef

```python
# ListWatchlistsRequestRequestTypeDef definition

class ListWatchlistsRequestRequestTypeDef(TypedDict):
    DomainId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## WatchlistSummaryTypeDef

```python
# WatchlistSummaryTypeDef definition

class WatchlistSummaryTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    DefaultWatchlist: NotRequired[bool],
    Description: NotRequired[str],
    DomainId: NotRequired[str],
    Name: NotRequired[str],
    UpdatedAt: NotRequired[datetime],
    WatchlistId: NotRequired[str],
```

## OptOutSpeakerRequestRequestTypeDef

```python
# OptOutSpeakerRequestRequestTypeDef definition

class OptOutSpeakerRequestRequestTypeDef(TypedDict):
    DomainId: str,
    SpeakerId: str,
```

## RegistrationConfigTypeDef

```python
# RegistrationConfigTypeDef definition

class RegistrationConfigTypeDef(TypedDict):
    DuplicateRegistrationAction: NotRequired[DuplicateRegistrationActionType],  # (1)
    FraudsterSimilarityThreshold: NotRequired[int],
    WatchlistIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DuplicateRegistrationActionType](./literals.md#duplicateregistrationactiontype) 
## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateWatchlistRequestRequestTypeDef

```python
# UpdateWatchlistRequestRequestTypeDef definition

class UpdateWatchlistRequestRequestTypeDef(TypedDict):
    DomainId: str,
    WatchlistId: str,
    Description: NotRequired[str],
    Name: NotRequired[str],
```

## AssociateFraudsterResponseTypeDef

```python
# AssociateFraudsterResponseTypeDef definition

class AssociateFraudsterResponseTypeDef(TypedDict):
    Fraudster: FraudsterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FraudsterTypeDef](./type_defs.md#fraudstertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFraudsterResponseTypeDef

```python
# DescribeFraudsterResponseTypeDef definition

class DescribeFraudsterResponseTypeDef(TypedDict):
    Fraudster: FraudsterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FraudsterTypeDef](./type_defs.md#fraudstertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateFraudsterResponseTypeDef

```python
# DisassociateFraudsterResponseTypeDef definition

class DisassociateFraudsterResponseTypeDef(TypedDict):
    Fraudster: FraudsterTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FraudsterTypeDef](./type_defs.md#fraudstertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuthenticationResultTypeDef

```python
# AuthenticationResultTypeDef definition

class AuthenticationResultTypeDef(TypedDict):
    AudioAggregationEndedAt: NotRequired[datetime],
    AudioAggregationStartedAt: NotRequired[datetime],
    AuthenticationResultId: NotRequired[str],
    Configuration: NotRequired[AuthenticationConfigurationTypeDef],  # (1)
    CustomerSpeakerId: NotRequired[str],
    Decision: NotRequired[AuthenticationDecisionType],  # (2)
    GeneratedSpeakerId: NotRequired[str],
    Score: NotRequired[int],
```

1. See [:material-code-braces: AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef) 
2. See [:material-code-brackets: AuthenticationDecisionType](./literals.md#authenticationdecisiontype) 
## UpdateDomainRequestRequestTypeDef

```python
# UpdateDomainRequestRequestTypeDef definition

class UpdateDomainRequestRequestTypeDef(TypedDict):
    DomainId: str,
    Name: str,
    ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
## CreateDomainRequestRequestTypeDef

```python
# CreateDomainRequestRequestTypeDef definition

class CreateDomainRequestRequestTypeDef(TypedDict):
    Name: str,
    ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,  # (1)
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
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
## CreateWatchlistResponseTypeDef

```python
# CreateWatchlistResponseTypeDef definition

class CreateWatchlistResponseTypeDef(TypedDict):
    Watchlist: WatchlistTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WatchlistTypeDef](./type_defs.md#watchlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeWatchlistResponseTypeDef

```python
# DescribeWatchlistResponseTypeDef definition

class DescribeWatchlistResponseTypeDef(TypedDict):
    Watchlist: WatchlistTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WatchlistTypeDef](./type_defs.md#watchlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWatchlistResponseTypeDef

```python
# UpdateWatchlistResponseTypeDef definition

class UpdateWatchlistResponseTypeDef(TypedDict):
    Watchlist: WatchlistTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WatchlistTypeDef](./type_defs.md#watchlisttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSpeakerResponseTypeDef

```python
# DescribeSpeakerResponseTypeDef definition

class DescribeSpeakerResponseTypeDef(TypedDict):
    Speaker: SpeakerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SpeakerTypeDef](./type_defs.md#speakertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OptOutSpeakerResponseTypeDef

```python
# OptOutSpeakerResponseTypeDef definition

class OptOutSpeakerResponseTypeDef(TypedDict):
    Speaker: SpeakerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SpeakerTypeDef](./type_defs.md#speakertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Description: NotRequired[str],
    DomainId: NotRequired[str],
    DomainStatus: NotRequired[DomainStatusType],  # (1)
    Name: NotRequired[str],
    ServerSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (2)
    ServerSideEncryptionUpdateDetails: NotRequired[ServerSideEncryptionUpdateDetailsTypeDef],  # (3)
    UpdatedAt: NotRequired[datetime],
    WatchlistDetails: NotRequired[WatchlistDetailsTypeDef],  # (4)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-braces: ServerSideEncryptionUpdateDetailsTypeDef](./type_defs.md#serversideencryptionupdatedetailstypedef) 
4. See [:material-code-braces: WatchlistDetailsTypeDef](./type_defs.md#watchlistdetailstypedef) 
## DomainTypeDef

```python
# DomainTypeDef definition

class DomainTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Description: NotRequired[str],
    DomainId: NotRequired[str],
    DomainStatus: NotRequired[DomainStatusType],  # (1)
    Name: NotRequired[str],
    ServerSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (2)
    ServerSideEncryptionUpdateDetails: NotRequired[ServerSideEncryptionUpdateDetailsTypeDef],  # (3)
    UpdatedAt: NotRequired[datetime],
    WatchlistDetails: NotRequired[WatchlistDetailsTypeDef],  # (4)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-braces: ServerSideEncryptionUpdateDetailsTypeDef](./type_defs.md#serversideencryptionupdatedetailstypedef) 
4. See [:material-code-braces: WatchlistDetailsTypeDef](./type_defs.md#watchlistdetailstypedef) 
## EnrollmentConfigOutputTypeDef

```python
# EnrollmentConfigOutputTypeDef definition

class EnrollmentConfigOutputTypeDef(TypedDict):
    ExistingEnrollmentAction: NotRequired[ExistingEnrollmentActionType],  # (1)
    FraudDetectionConfig: NotRequired[EnrollmentJobFraudDetectionConfigOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: ExistingEnrollmentActionType](./literals.md#existingenrollmentactiontype) 
2. See [:material-code-braces: EnrollmentJobFraudDetectionConfigOutputTypeDef](./type_defs.md#enrollmentjobfrauddetectionconfigoutputtypedef) 
## FraudRiskDetailsTypeDef

```python
# FraudRiskDetailsTypeDef definition

class FraudRiskDetailsTypeDef(TypedDict):
    KnownFraudsterRisk: KnownFraudsterRiskTypeDef,  # (1)
    VoiceSpoofingRisk: VoiceSpoofingRiskTypeDef,  # (2)
```

1. See [:material-code-braces: KnownFraudsterRiskTypeDef](./type_defs.md#knownfraudsterrisktypedef) 
2. See [:material-code-braces: VoiceSpoofingRiskTypeDef](./type_defs.md#voicespoofingrisktypedef) 
## FraudsterRegistrationJobSummaryTypeDef

```python
# FraudsterRegistrationJobSummaryTypeDef definition

class FraudsterRegistrationJobSummaryTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    DomainId: NotRequired[str],
    EndedAt: NotRequired[datetime],
    FailureDetails: NotRequired[FailureDetailsTypeDef],  # (1)
    JobId: NotRequired[str],
    JobName: NotRequired[str],
    JobProgress: NotRequired[JobProgressTypeDef],  # (2)
    JobStatus: NotRequired[FraudsterRegistrationJobStatusType],  # (3)
```

1. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
2. See [:material-code-braces: JobProgressTypeDef](./type_defs.md#jobprogresstypedef) 
3. See [:material-code-brackets: FraudsterRegistrationJobStatusType](./literals.md#fraudsterregistrationjobstatustype) 
## SpeakerEnrollmentJobSummaryTypeDef

```python
# SpeakerEnrollmentJobSummaryTypeDef definition

class SpeakerEnrollmentJobSummaryTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    DomainId: NotRequired[str],
    EndedAt: NotRequired[datetime],
    FailureDetails: NotRequired[FailureDetailsTypeDef],  # (1)
    JobId: NotRequired[str],
    JobName: NotRequired[str],
    JobProgress: NotRequired[JobProgressTypeDef],  # (2)
    JobStatus: NotRequired[SpeakerEnrollmentJobStatusType],  # (3)
```

1. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
2. See [:material-code-braces: JobProgressTypeDef](./type_defs.md#jobprogresstypedef) 
3. See [:material-code-brackets: SpeakerEnrollmentJobStatusType](./literals.md#speakerenrollmentjobstatustype) 
## FraudsterRegistrationJobTypeDef

```python
# FraudsterRegistrationJobTypeDef definition

class FraudsterRegistrationJobTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    DataAccessRoleArn: NotRequired[str],
    DomainId: NotRequired[str],
    EndedAt: NotRequired[datetime],
    FailureDetails: NotRequired[FailureDetailsTypeDef],  # (1)
    InputDataConfig: NotRequired[InputDataConfigTypeDef],  # (2)
    JobId: NotRequired[str],
    JobName: NotRequired[str],
    JobProgress: NotRequired[JobProgressTypeDef],  # (3)
    JobStatus: NotRequired[FraudsterRegistrationJobStatusType],  # (4)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (5)
    RegistrationConfig: NotRequired[RegistrationConfigOutputTypeDef],  # (6)
```

1. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
2. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
3. See [:material-code-braces: JobProgressTypeDef](./type_defs.md#jobprogresstypedef) 
4. See [:material-code-brackets: FraudsterRegistrationJobStatusType](./literals.md#fraudsterregistrationjobstatustype) 
5. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
6. See [:material-code-braces: RegistrationConfigOutputTypeDef](./type_defs.md#registrationconfigoutputtypedef) 
## ListFraudstersResponseTypeDef

```python
# ListFraudstersResponseTypeDef definition

class ListFraudstersResponseTypeDef(TypedDict):
    FraudsterSummaries: List[FraudsterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FraudsterSummaryTypeDef](./type_defs.md#fraudstersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainsRequestListDomainsPaginateTypeDef

```python
# ListDomainsRequestListDomainsPaginateTypeDef definition

class ListDomainsRequestListDomainsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef

```python
# ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef definition

class ListFraudsterRegistrationJobsRequestListFraudsterRegistrationJobsPaginateTypeDef(TypedDict):
    DomainId: str,
    JobStatus: NotRequired[FraudsterRegistrationJobStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FraudsterRegistrationJobStatusType](./literals.md#fraudsterregistrationjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFraudstersRequestListFraudstersPaginateTypeDef

```python
# ListFraudstersRequestListFraudstersPaginateTypeDef definition

class ListFraudstersRequestListFraudstersPaginateTypeDef(TypedDict):
    DomainId: str,
    WatchlistId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef

```python
# ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef definition

class ListSpeakerEnrollmentJobsRequestListSpeakerEnrollmentJobsPaginateTypeDef(TypedDict):
    DomainId: str,
    JobStatus: NotRequired[SpeakerEnrollmentJobStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SpeakerEnrollmentJobStatusType](./literals.md#speakerenrollmentjobstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSpeakersRequestListSpeakersPaginateTypeDef

```python
# ListSpeakersRequestListSpeakersPaginateTypeDef definition

class ListSpeakersRequestListSpeakersPaginateTypeDef(TypedDict):
    DomainId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWatchlistsRequestListWatchlistsPaginateTypeDef

```python
# ListWatchlistsRequestListWatchlistsPaginateTypeDef definition

class ListWatchlistsRequestListWatchlistsPaginateTypeDef(TypedDict):
    DomainId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSpeakersResponseTypeDef

```python
# ListSpeakersResponseTypeDef definition

class ListSpeakersResponseTypeDef(TypedDict):
    SpeakerSummaries: List[SpeakerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SpeakerSummaryTypeDef](./type_defs.md#speakersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWatchlistsResponseTypeDef

```python
# ListWatchlistsResponseTypeDef definition

class ListWatchlistsResponseTypeDef(TypedDict):
    WatchlistSummaries: List[WatchlistSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WatchlistSummaryTypeDef](./type_defs.md#watchlistsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartFraudsterRegistrationJobRequestRequestTypeDef

```python
# StartFraudsterRegistrationJobRequestRequestTypeDef definition

class StartFraudsterRegistrationJobRequestRequestTypeDef(TypedDict):
    DataAccessRoleArn: str,
    DomainId: str,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    ClientToken: NotRequired[str],
    JobName: NotRequired[str],
    RegistrationConfig: NotRequired[RegistrationConfigTypeDef],  # (3)
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: RegistrationConfigTypeDef](./type_defs.md#registrationconfigtypedef) 
## ListDomainsResponseTypeDef

```python
# ListDomainsResponseTypeDef definition

class ListDomainsResponseTypeDef(TypedDict):
    DomainSummaries: List[DomainSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainResponseTypeDef

```python
# CreateDomainResponseTypeDef definition

class CreateDomainResponseTypeDef(TypedDict):
    Domain: DomainTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainTypeDef](./type_defs.md#domaintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDomainResponseTypeDef

```python
# DescribeDomainResponseTypeDef definition

class DescribeDomainResponseTypeDef(TypedDict):
    Domain: DomainTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainTypeDef](./type_defs.md#domaintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainResponseTypeDef

```python
# UpdateDomainResponseTypeDef definition

class UpdateDomainResponseTypeDef(TypedDict):
    Domain: DomainTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainTypeDef](./type_defs.md#domaintypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SpeakerEnrollmentJobTypeDef

```python
# SpeakerEnrollmentJobTypeDef definition

class SpeakerEnrollmentJobTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    DataAccessRoleArn: NotRequired[str],
    DomainId: NotRequired[str],
    EndedAt: NotRequired[datetime],
    EnrollmentConfig: NotRequired[EnrollmentConfigOutputTypeDef],  # (1)
    FailureDetails: NotRequired[FailureDetailsTypeDef],  # (2)
    InputDataConfig: NotRequired[InputDataConfigTypeDef],  # (3)
    JobId: NotRequired[str],
    JobName: NotRequired[str],
    JobProgress: NotRequired[JobProgressTypeDef],  # (4)
    JobStatus: NotRequired[SpeakerEnrollmentJobStatusType],  # (5)
    OutputDataConfig: NotRequired[OutputDataConfigTypeDef],  # (6)
```

1. See [:material-code-braces: EnrollmentConfigOutputTypeDef](./type_defs.md#enrollmentconfigoutputtypedef) 
2. See [:material-code-braces: FailureDetailsTypeDef](./type_defs.md#failuredetailstypedef) 
3. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
4. See [:material-code-braces: JobProgressTypeDef](./type_defs.md#jobprogresstypedef) 
5. See [:material-code-brackets: SpeakerEnrollmentJobStatusType](./literals.md#speakerenrollmentjobstatustype) 
6. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
## EnrollmentConfigTypeDef

```python
# EnrollmentConfigTypeDef definition

class EnrollmentConfigTypeDef(TypedDict):
    ExistingEnrollmentAction: NotRequired[ExistingEnrollmentActionType],  # (1)
    FraudDetectionConfig: NotRequired[EnrollmentJobFraudDetectionConfigUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: ExistingEnrollmentActionType](./literals.md#existingenrollmentactiontype) 
2. See [:material-code-braces: EnrollmentJobFraudDetectionConfigTypeDef](./type_defs.md#enrollmentjobfrauddetectionconfigtypedef) [:material-code-braces: EnrollmentJobFraudDetectionConfigOutputTypeDef](./type_defs.md#enrollmentjobfrauddetectionconfigoutputtypedef) 
## FraudDetectionResultTypeDef

```python
# FraudDetectionResultTypeDef definition

class FraudDetectionResultTypeDef(TypedDict):
    AudioAggregationEndedAt: NotRequired[datetime],
    AudioAggregationStartedAt: NotRequired[datetime],
    Configuration: NotRequired[FraudDetectionConfigurationTypeDef],  # (1)
    Decision: NotRequired[FraudDetectionDecisionType],  # (2)
    FraudDetectionResultId: NotRequired[str],
    Reasons: NotRequired[List[FraudDetectionReasonType]],  # (3)
    RiskDetails: NotRequired[FraudRiskDetailsTypeDef],  # (4)
```

1. See [:material-code-braces: FraudDetectionConfigurationTypeDef](./type_defs.md#frauddetectionconfigurationtypedef) 
2. See [:material-code-brackets: FraudDetectionDecisionType](./literals.md#frauddetectiondecisiontype) 
3. See [:material-code-brackets: FraudDetectionReasonType](./literals.md#frauddetectionreasontype) 
4. See [:material-code-braces: FraudRiskDetailsTypeDef](./type_defs.md#fraudriskdetailstypedef) 
## ListFraudsterRegistrationJobsResponseTypeDef

```python
# ListFraudsterRegistrationJobsResponseTypeDef definition

class ListFraudsterRegistrationJobsResponseTypeDef(TypedDict):
    JobSummaries: List[FraudsterRegistrationJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FraudsterRegistrationJobSummaryTypeDef](./type_defs.md#fraudsterregistrationjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSpeakerEnrollmentJobsResponseTypeDef

```python
# ListSpeakerEnrollmentJobsResponseTypeDef definition

class ListSpeakerEnrollmentJobsResponseTypeDef(TypedDict):
    JobSummaries: List[SpeakerEnrollmentJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SpeakerEnrollmentJobSummaryTypeDef](./type_defs.md#speakerenrollmentjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFraudsterRegistrationJobResponseTypeDef

```python
# DescribeFraudsterRegistrationJobResponseTypeDef definition

class DescribeFraudsterRegistrationJobResponseTypeDef(TypedDict):
    Job: FraudsterRegistrationJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FraudsterRegistrationJobTypeDef](./type_defs.md#fraudsterregistrationjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartFraudsterRegistrationJobResponseTypeDef

```python
# StartFraudsterRegistrationJobResponseTypeDef definition

class StartFraudsterRegistrationJobResponseTypeDef(TypedDict):
    Job: FraudsterRegistrationJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FraudsterRegistrationJobTypeDef](./type_defs.md#fraudsterregistrationjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSpeakerEnrollmentJobResponseTypeDef

```python
# DescribeSpeakerEnrollmentJobResponseTypeDef definition

class DescribeSpeakerEnrollmentJobResponseTypeDef(TypedDict):
    Job: SpeakerEnrollmentJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SpeakerEnrollmentJobTypeDef](./type_defs.md#speakerenrollmentjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSpeakerEnrollmentJobResponseTypeDef

```python
# StartSpeakerEnrollmentJobResponseTypeDef definition

class StartSpeakerEnrollmentJobResponseTypeDef(TypedDict):
    Job: SpeakerEnrollmentJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SpeakerEnrollmentJobTypeDef](./type_defs.md#speakerenrollmentjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSpeakerEnrollmentJobRequestRequestTypeDef

```python
# StartSpeakerEnrollmentJobRequestRequestTypeDef definition

class StartSpeakerEnrollmentJobRequestRequestTypeDef(TypedDict):
    DataAccessRoleArn: str,
    DomainId: str,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    ClientToken: NotRequired[str],
    EnrollmentConfig: NotRequired[EnrollmentConfigTypeDef],  # (3)
    JobName: NotRequired[str],
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: EnrollmentConfigTypeDef](./type_defs.md#enrollmentconfigtypedef) 
## EvaluateSessionResponseTypeDef

```python
# EvaluateSessionResponseTypeDef definition

class EvaluateSessionResponseTypeDef(TypedDict):
    AuthenticationResult: AuthenticationResultTypeDef,  # (1)
    DomainId: str,
    FraudDetectionResult: FraudDetectionResultTypeDef,  # (2)
    SessionId: str,
    SessionName: str,
    StreamingStatus: StreamingStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AuthenticationResultTypeDef](./type_defs.md#authenticationresulttypedef) 
2. See [:material-code-braces: FraudDetectionResultTypeDef](./type_defs.md#frauddetectionresulttypedef) 
3. See [:material-code-brackets: StreamingStatusType](./literals.md#streamingstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

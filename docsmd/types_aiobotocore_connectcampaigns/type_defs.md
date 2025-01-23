# Type definitions

> [Index](../README.md) > [ConnectCampaignService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ConnectCampaignService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#connectcampaignservice)
    type annotations stubs module [types-aiobotocore-connectcampaigns](https://pypi.org/project/types-aiobotocore-connectcampaigns/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AgentlessDialerConfigTypeDef

```python
# AgentlessDialerConfigTypeDef definition

class AgentlessDialerConfigTypeDef(TypedDict):
    dialingCapacity: NotRequired[float],
```

## AnswerMachineDetectionConfigTypeDef

```python
# AnswerMachineDetectionConfigTypeDef definition

class AnswerMachineDetectionConfigTypeDef(TypedDict):
    enableAnswerMachineDetection: bool,
    awaitAnswerMachinePrompt: NotRequired[bool],
```

## InstanceIdFilterTypeDef

```python
# InstanceIdFilterTypeDef definition

class InstanceIdFilterTypeDef(TypedDict):
    value: str,
    operator: InstanceIdFilterOperatorType,  # (1)
```

1. See [:material-code-brackets: InstanceIdFilterOperatorType](./literals.md#instanceidfilteroperatortype) 
## CampaignSummaryTypeDef

```python
# CampaignSummaryTypeDef definition

class CampaignSummaryTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    connectInstanceId: str,
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

## DeleteCampaignRequestRequestTypeDef

```python
# DeleteCampaignRequestRequestTypeDef definition

class DeleteCampaignRequestRequestTypeDef(TypedDict):
    id: str,
```

## DeleteConnectInstanceConfigRequestRequestTypeDef

```python
# DeleteConnectInstanceConfigRequestRequestTypeDef definition

class DeleteConnectInstanceConfigRequestRequestTypeDef(TypedDict):
    connectInstanceId: str,
```

## DeleteInstanceOnboardingJobRequestRequestTypeDef

```python
# DeleteInstanceOnboardingJobRequestRequestTypeDef definition

class DeleteInstanceOnboardingJobRequestRequestTypeDef(TypedDict):
    connectInstanceId: str,
```

## DescribeCampaignRequestRequestTypeDef

```python
# DescribeCampaignRequestRequestTypeDef definition

class DescribeCampaignRequestRequestTypeDef(TypedDict):
    id: str,
```

## PredictiveDialerConfigTypeDef

```python
# PredictiveDialerConfigTypeDef definition

class PredictiveDialerConfigTypeDef(TypedDict):
    bandwidthAllocation: float,
    dialingCapacity: NotRequired[float],
```

## ProgressiveDialerConfigTypeDef

```python
# ProgressiveDialerConfigTypeDef definition

class ProgressiveDialerConfigTypeDef(TypedDict):
    bandwidthAllocation: float,
    dialingCapacity: NotRequired[float],
```

## EncryptionConfigTypeDef

```python
# EncryptionConfigTypeDef definition

class EncryptionConfigTypeDef(TypedDict):
    enabled: bool,
    encryptionType: NotRequired[EncryptionTypeType],  # (1)
    keyArn: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype) 
## FailedCampaignStateResponseTypeDef

```python
# FailedCampaignStateResponseTypeDef definition

class FailedCampaignStateResponseTypeDef(TypedDict):
    campaignId: NotRequired[str],
    failureCode: NotRequired[GetCampaignStateBatchFailureCodeType],  # (1)
```

1. See [:material-code-brackets: GetCampaignStateBatchFailureCodeType](./literals.md#getcampaignstatebatchfailurecodetype) 
## FailedRequestTypeDef

```python
# FailedRequestTypeDef definition

class FailedRequestTypeDef(TypedDict):
    clientToken: NotRequired[str],
    id: NotRequired[str],
    failureCode: NotRequired[FailureCodeType],  # (1)
```

1. See [:material-code-brackets: FailureCodeType](./literals.md#failurecodetype) 
## GetCampaignStateBatchRequestRequestTypeDef

```python
# GetCampaignStateBatchRequestRequestTypeDef definition

class GetCampaignStateBatchRequestRequestTypeDef(TypedDict):
    campaignIds: Sequence[str],
```

## SuccessfulCampaignStateResponseTypeDef

```python
# SuccessfulCampaignStateResponseTypeDef definition

class SuccessfulCampaignStateResponseTypeDef(TypedDict):
    campaignId: NotRequired[str],
    state: NotRequired[CampaignStateType],  # (1)
```

1. See [:material-code-brackets: CampaignStateType](./literals.md#campaignstatetype) 
## GetCampaignStateRequestRequestTypeDef

```python
# GetCampaignStateRequestRequestTypeDef definition

class GetCampaignStateRequestRequestTypeDef(TypedDict):
    id: str,
```

## GetConnectInstanceConfigRequestRequestTypeDef

```python
# GetConnectInstanceConfigRequestRequestTypeDef definition

class GetConnectInstanceConfigRequestRequestTypeDef(TypedDict):
    connectInstanceId: str,
```

## GetInstanceOnboardingJobStatusRequestRequestTypeDef

```python
# GetInstanceOnboardingJobStatusRequestRequestTypeDef definition

class GetInstanceOnboardingJobStatusRequestRequestTypeDef(TypedDict):
    connectInstanceId: str,
```

## InstanceOnboardingJobStatusTypeDef

```python
# InstanceOnboardingJobStatusTypeDef definition

class InstanceOnboardingJobStatusTypeDef(TypedDict):
    connectInstanceId: str,
    status: InstanceOnboardingJobStatusCodeType,  # (1)
    failureCode: NotRequired[InstanceOnboardingJobFailureCodeType],  # (2)
```

1. See [:material-code-brackets: InstanceOnboardingJobStatusCodeType](./literals.md#instanceonboardingjobstatuscodetype) 
2. See [:material-code-brackets: InstanceOnboardingJobFailureCodeType](./literals.md#instanceonboardingjobfailurecodetype) 
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
    arn: str,
```

## PauseCampaignRequestRequestTypeDef

```python
# PauseCampaignRequestRequestTypeDef definition

class PauseCampaignRequestRequestTypeDef(TypedDict):
    id: str,
```

## SuccessfulRequestTypeDef

```python
# SuccessfulRequestTypeDef definition

class SuccessfulRequestTypeDef(TypedDict):
    clientToken: NotRequired[str],
    id: NotRequired[str],
```

## ResumeCampaignRequestRequestTypeDef

```python
# ResumeCampaignRequestRequestTypeDef definition

class ResumeCampaignRequestRequestTypeDef(TypedDict):
    id: str,
```

## StartCampaignRequestRequestTypeDef

```python
# StartCampaignRequestRequestTypeDef definition

class StartCampaignRequestRequestTypeDef(TypedDict):
    id: str,
```

## StopCampaignRequestRequestTypeDef

```python
# StopCampaignRequestRequestTypeDef definition

class StopCampaignRequestRequestTypeDef(TypedDict):
    id: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    arn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    arn: str,
    tagKeys: Sequence[str],
```

## UpdateCampaignNameRequestRequestTypeDef

```python
# UpdateCampaignNameRequestRequestTypeDef definition

class UpdateCampaignNameRequestRequestTypeDef(TypedDict):
    id: str,
    name: str,
```

## OutboundCallConfigTypeDef

```python
# OutboundCallConfigTypeDef definition

class OutboundCallConfigTypeDef(TypedDict):
    connectContactFlowId: str,
    connectSourcePhoneNumber: NotRequired[str],
    connectQueueId: NotRequired[str],
    answerMachineDetectionConfig: NotRequired[AnswerMachineDetectionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef) 
## UpdateCampaignOutboundCallConfigRequestRequestTypeDef

```python
# UpdateCampaignOutboundCallConfigRequestRequestTypeDef definition

class UpdateCampaignOutboundCallConfigRequestRequestTypeDef(TypedDict):
    id: str,
    connectContactFlowId: NotRequired[str],
    connectSourcePhoneNumber: NotRequired[str],
    answerMachineDetectionConfig: NotRequired[AnswerMachineDetectionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef) 
## CampaignFiltersTypeDef

```python
# CampaignFiltersTypeDef definition

class CampaignFiltersTypeDef(TypedDict):
    instanceIdFilter: NotRequired[InstanceIdFilterTypeDef],  # (1)
```

1. See [:material-code-braces: InstanceIdFilterTypeDef](./type_defs.md#instanceidfiltertypedef) 
## CreateCampaignResponseTypeDef

```python
# CreateCampaignResponseTypeDef definition

class CreateCampaignResponseTypeDef(TypedDict):
    id: str,
    arn: str,
    tags: Dict[str, str],
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
## GetCampaignStateResponseTypeDef

```python
# GetCampaignStateResponseTypeDef definition

class GetCampaignStateResponseTypeDef(TypedDict):
    state: CampaignStateType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CampaignStateType](./literals.md#campaignstatetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCampaignsResponseTypeDef

```python
# ListCampaignsResponseTypeDef definition

class ListCampaignsResponseTypeDef(TypedDict):
    campaignSummaryList: List[CampaignSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CampaignSummaryTypeDef](./type_defs.md#campaignsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DialRequestTypeDef

```python
# DialRequestTypeDef definition

class DialRequestTypeDef(TypedDict):
    clientToken: str,
    phoneNumber: str,
    expirationTime: TimestampTypeDef,
    attributes: Mapping[str, str],
```

## DialerConfigTypeDef

```python
# DialerConfigTypeDef definition

class DialerConfigTypeDef(TypedDict):
    progressiveDialerConfig: NotRequired[ProgressiveDialerConfigTypeDef],  # (1)
    predictiveDialerConfig: NotRequired[PredictiveDialerConfigTypeDef],  # (2)
    agentlessDialerConfig: NotRequired[AgentlessDialerConfigTypeDef],  # (3)
```

1. See [:material-code-braces: ProgressiveDialerConfigTypeDef](./type_defs.md#progressivedialerconfigtypedef) 
2. See [:material-code-braces: PredictiveDialerConfigTypeDef](./type_defs.md#predictivedialerconfigtypedef) 
3. See [:material-code-braces: AgentlessDialerConfigTypeDef](./type_defs.md#agentlessdialerconfigtypedef) 
## InstanceConfigTypeDef

```python
# InstanceConfigTypeDef definition

class InstanceConfigTypeDef(TypedDict):
    connectInstanceId: str,
    serviceLinkedRoleArn: str,
    encryptionConfig: EncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## StartInstanceOnboardingJobRequestRequestTypeDef

```python
# StartInstanceOnboardingJobRequestRequestTypeDef definition

class StartInstanceOnboardingJobRequestRequestTypeDef(TypedDict):
    connectInstanceId: str,
    encryptionConfig: EncryptionConfigTypeDef,  # (1)
```

1. See [:material-code-braces: EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef) 
## GetCampaignStateBatchResponseTypeDef

```python
# GetCampaignStateBatchResponseTypeDef definition

class GetCampaignStateBatchResponseTypeDef(TypedDict):
    successfulRequests: List[SuccessfulCampaignStateResponseTypeDef],  # (1)
    failedRequests: List[FailedCampaignStateResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulCampaignStateResponseTypeDef](./type_defs.md#successfulcampaignstateresponsetypedef) 
2. See [:material-code-braces: FailedCampaignStateResponseTypeDef](./type_defs.md#failedcampaignstateresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInstanceOnboardingJobStatusResponseTypeDef

```python
# GetInstanceOnboardingJobStatusResponseTypeDef definition

class GetInstanceOnboardingJobStatusResponseTypeDef(TypedDict):
    connectInstanceOnboardingJobStatus: InstanceOnboardingJobStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceOnboardingJobStatusTypeDef](./type_defs.md#instanceonboardingjobstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartInstanceOnboardingJobResponseTypeDef

```python
# StartInstanceOnboardingJobResponseTypeDef definition

class StartInstanceOnboardingJobResponseTypeDef(TypedDict):
    connectInstanceOnboardingJobStatus: InstanceOnboardingJobStatusTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceOnboardingJobStatusTypeDef](./type_defs.md#instanceonboardingjobstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDialRequestBatchResponseTypeDef

```python
# PutDialRequestBatchResponseTypeDef definition

class PutDialRequestBatchResponseTypeDef(TypedDict):
    successfulRequests: List[SuccessfulRequestTypeDef],  # (1)
    failedRequests: List[FailedRequestTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuccessfulRequestTypeDef](./type_defs.md#successfulrequesttypedef) 
2. See [:material-code-braces: FailedRequestTypeDef](./type_defs.md#failedrequesttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCampaignsRequestPaginateTypeDef

```python
# ListCampaignsRequestPaginateTypeDef definition

class ListCampaignsRequestPaginateTypeDef(TypedDict):
    filters: NotRequired[CampaignFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: CampaignFiltersTypeDef](./type_defs.md#campaignfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCampaignsRequestRequestTypeDef

```python
# ListCampaignsRequestRequestTypeDef definition

class ListCampaignsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    filters: NotRequired[CampaignFiltersTypeDef],  # (1)
```

1. See [:material-code-braces: CampaignFiltersTypeDef](./type_defs.md#campaignfilterstypedef) 
## PutDialRequestBatchRequestRequestTypeDef

```python
# PutDialRequestBatchRequestRequestTypeDef definition

class PutDialRequestBatchRequestRequestTypeDef(TypedDict):
    id: str,
    dialRequests: Sequence[DialRequestTypeDef],  # (1)
```

1. See [:material-code-braces: DialRequestTypeDef](./type_defs.md#dialrequesttypedef) 
## CampaignTypeDef

```python
# CampaignTypeDef definition

class CampaignTypeDef(TypedDict):
    id: str,
    arn: str,
    name: str,
    connectInstanceId: str,
    dialerConfig: DialerConfigTypeDef,  # (1)
    outboundCallConfig: OutboundCallConfigTypeDef,  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: DialerConfigTypeDef](./type_defs.md#dialerconfigtypedef) 
2. See [:material-code-braces: OutboundCallConfigTypeDef](./type_defs.md#outboundcallconfigtypedef) 
## CreateCampaignRequestRequestTypeDef

```python
# CreateCampaignRequestRequestTypeDef definition

class CreateCampaignRequestRequestTypeDef(TypedDict):
    name: str,
    connectInstanceId: str,
    dialerConfig: DialerConfigTypeDef,  # (1)
    outboundCallConfig: OutboundCallConfigTypeDef,  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: DialerConfigTypeDef](./type_defs.md#dialerconfigtypedef) 
2. See [:material-code-braces: OutboundCallConfigTypeDef](./type_defs.md#outboundcallconfigtypedef) 
## UpdateCampaignDialerConfigRequestRequestTypeDef

```python
# UpdateCampaignDialerConfigRequestRequestTypeDef definition

class UpdateCampaignDialerConfigRequestRequestTypeDef(TypedDict):
    id: str,
    dialerConfig: DialerConfigTypeDef,  # (1)
```

1. See [:material-code-braces: DialerConfigTypeDef](./type_defs.md#dialerconfigtypedef) 
## GetConnectInstanceConfigResponseTypeDef

```python
# GetConnectInstanceConfigResponseTypeDef definition

class GetConnectInstanceConfigResponseTypeDef(TypedDict):
    connectInstanceConfig: InstanceConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InstanceConfigTypeDef](./type_defs.md#instanceconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCampaignResponseTypeDef

```python
# DescribeCampaignResponseTypeDef definition

class DescribeCampaignResponseTypeDef(TypedDict):
    campaign: CampaignTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CampaignTypeDef](./type_defs.md#campaigntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

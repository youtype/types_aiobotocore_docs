# Type definitions

> [Index](../README.md) > [MTurk](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [MTurk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#mturk)
    type annotations stubs module [types-aiobotocore-mturk](https://pypi.org/project/types-aiobotocore-mturk/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ParameterMapEntryUnionTypeDef

```python
# ParameterMapEntryUnionTypeDef definition

ParameterMapEntryUnionTypeDef = Union[
    ParameterMapEntryTypeDef,  # (1)
    ParameterMapEntryOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ParameterMapEntryTypeDef](./type_defs.md#parametermapentrytypedef) 
2. See [:material-code-braces: ParameterMapEntryOutputTypeDef](./type_defs.md#parametermapentryoutputtypedef) 

## QualificationRequirementUnionTypeDef

```python
# QualificationRequirementUnionTypeDef definition

QualificationRequirementUnionTypeDef = Union[
    QualificationRequirementTypeDef,  # (1)
    QualificationRequirementOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QualificationRequirementTypeDef](./type_defs.md#qualificationrequirementtypedef) 
2. See [:material-code-braces: QualificationRequirementOutputTypeDef](./type_defs.md#qualificationrequirementoutputtypedef) 

## PolicyParameterUnionTypeDef

```python
# PolicyParameterUnionTypeDef definition

PolicyParameterUnionTypeDef = Union[
    PolicyParameterTypeDef,  # (1)
    PolicyParameterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PolicyParameterTypeDef](./type_defs.md#policyparametertypedef) 
2. See [:material-code-braces: PolicyParameterOutputTypeDef](./type_defs.md#policyparameteroutputtypedef) 



## AcceptQualificationRequestRequestRequestTypeDef

```python
# AcceptQualificationRequestRequestRequestTypeDef definition

class AcceptQualificationRequestRequestRequestTypeDef(TypedDict):
    QualificationRequestId: str,
    IntegerValue: NotRequired[int],
```

## ApproveAssignmentRequestRequestTypeDef

```python
# ApproveAssignmentRequestRequestTypeDef definition

class ApproveAssignmentRequestRequestTypeDef(TypedDict):
    AssignmentId: str,
    RequesterFeedback: NotRequired[str],
    OverrideRejection: NotRequired[bool],
```

## AssignmentTypeDef

```python
# AssignmentTypeDef definition

class AssignmentTypeDef(TypedDict):
    AssignmentId: NotRequired[str],
    WorkerId: NotRequired[str],
    HITId: NotRequired[str],
    AssignmentStatus: NotRequired[AssignmentStatusType],  # (1)
    AutoApprovalTime: NotRequired[datetime],
    AcceptTime: NotRequired[datetime],
    SubmitTime: NotRequired[datetime],
    ApprovalTime: NotRequired[datetime],
    RejectionTime: NotRequired[datetime],
    Deadline: NotRequired[datetime],
    Answer: NotRequired[str],
    RequesterFeedback: NotRequired[str],
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
## AssociateQualificationWithWorkerRequestRequestTypeDef

```python
# AssociateQualificationWithWorkerRequestRequestTypeDef definition

class AssociateQualificationWithWorkerRequestRequestTypeDef(TypedDict):
    QualificationTypeId: str,
    WorkerId: str,
    IntegerValue: NotRequired[int],
    SendNotification: NotRequired[bool],
```

## BonusPaymentTypeDef

```python
# BonusPaymentTypeDef definition

class BonusPaymentTypeDef(TypedDict):
    WorkerId: NotRequired[str],
    BonusAmount: NotRequired[str],
    AssignmentId: NotRequired[str],
    Reason: NotRequired[str],
    GrantTime: NotRequired[datetime],
```

## CreateAdditionalAssignmentsForHITRequestRequestTypeDef

```python
# CreateAdditionalAssignmentsForHITRequestRequestTypeDef definition

class CreateAdditionalAssignmentsForHITRequestRequestTypeDef(TypedDict):
    HITId: str,
    NumberOfAdditionalAssignments: int,
    UniqueRequestToken: NotRequired[str],
```

## HITLayoutParameterTypeDef

```python
# HITLayoutParameterTypeDef definition

class HITLayoutParameterTypeDef(TypedDict):
    Name: str,
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

## CreateQualificationTypeRequestRequestTypeDef

```python
# CreateQualificationTypeRequestRequestTypeDef definition

class CreateQualificationTypeRequestRequestTypeDef(TypedDict):
    Name: str,
    Description: str,
    QualificationTypeStatus: QualificationTypeStatusType,  # (1)
    Keywords: NotRequired[str],
    RetryDelayInSeconds: NotRequired[int],
    Test: NotRequired[str],
    AnswerKey: NotRequired[str],
    TestDurationInSeconds: NotRequired[int],
    AutoGranted: NotRequired[bool],
    AutoGrantedValue: NotRequired[int],
```

1. See [:material-code-brackets: QualificationTypeStatusType](./literals.md#qualificationtypestatustype) 
## QualificationTypeTypeDef

```python
# QualificationTypeTypeDef definition

class QualificationTypeTypeDef(TypedDict):
    QualificationTypeId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Keywords: NotRequired[str],
    QualificationTypeStatus: NotRequired[QualificationTypeStatusType],  # (1)
    Test: NotRequired[str],
    TestDurationInSeconds: NotRequired[int],
    AnswerKey: NotRequired[str],
    RetryDelayInSeconds: NotRequired[int],
    IsRequestable: NotRequired[bool],
    AutoGranted: NotRequired[bool],
    AutoGrantedValue: NotRequired[int],
```

1. See [:material-code-brackets: QualificationTypeStatusType](./literals.md#qualificationtypestatustype) 
## CreateWorkerBlockRequestRequestTypeDef

```python
# CreateWorkerBlockRequestRequestTypeDef definition

class CreateWorkerBlockRequestRequestTypeDef(TypedDict):
    WorkerId: str,
    Reason: str,
```

## DeleteHITRequestRequestTypeDef

```python
# DeleteHITRequestRequestTypeDef definition

class DeleteHITRequestRequestTypeDef(TypedDict):
    HITId: str,
```

## DeleteQualificationTypeRequestRequestTypeDef

```python
# DeleteQualificationTypeRequestRequestTypeDef definition

class DeleteQualificationTypeRequestRequestTypeDef(TypedDict):
    QualificationTypeId: str,
```

## DeleteWorkerBlockRequestRequestTypeDef

```python
# DeleteWorkerBlockRequestRequestTypeDef definition

class DeleteWorkerBlockRequestRequestTypeDef(TypedDict):
    WorkerId: str,
    Reason: NotRequired[str],
```

## DisassociateQualificationFromWorkerRequestRequestTypeDef

```python
# DisassociateQualificationFromWorkerRequestRequestTypeDef definition

class DisassociateQualificationFromWorkerRequestRequestTypeDef(TypedDict):
    WorkerId: str,
    QualificationTypeId: str,
    Reason: NotRequired[str],
```

## GetAssignmentRequestRequestTypeDef

```python
# GetAssignmentRequestRequestTypeDef definition

class GetAssignmentRequestRequestTypeDef(TypedDict):
    AssignmentId: str,
```

## GetFileUploadURLRequestRequestTypeDef

```python
# GetFileUploadURLRequestRequestTypeDef definition

class GetFileUploadURLRequestRequestTypeDef(TypedDict):
    AssignmentId: str,
    QuestionIdentifier: str,
```

## GetHITRequestRequestTypeDef

```python
# GetHITRequestRequestTypeDef definition

class GetHITRequestRequestTypeDef(TypedDict):
    HITId: str,
```

## GetQualificationScoreRequestRequestTypeDef

```python
# GetQualificationScoreRequestRequestTypeDef definition

class GetQualificationScoreRequestRequestTypeDef(TypedDict):
    QualificationTypeId: str,
    WorkerId: str,
```

## GetQualificationTypeRequestRequestTypeDef

```python
# GetQualificationTypeRequestRequestTypeDef definition

class GetQualificationTypeRequestRequestTypeDef(TypedDict):
    QualificationTypeId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAssignmentsForHITRequestRequestTypeDef

```python
# ListAssignmentsForHITRequestRequestTypeDef definition

class ListAssignmentsForHITRequestRequestTypeDef(TypedDict):
    HITId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    AssignmentStatuses: NotRequired[Sequence[AssignmentStatusType]],  # (1)
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
## ListBonusPaymentsRequestRequestTypeDef

```python
# ListBonusPaymentsRequestRequestTypeDef definition

class ListBonusPaymentsRequestRequestTypeDef(TypedDict):
    HITId: NotRequired[str],
    AssignmentId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListHITsForQualificationTypeRequestRequestTypeDef

```python
# ListHITsForQualificationTypeRequestRequestTypeDef definition

class ListHITsForQualificationTypeRequestRequestTypeDef(TypedDict):
    QualificationTypeId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListHITsRequestRequestTypeDef

```python
# ListHITsRequestRequestTypeDef definition

class ListHITsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListQualificationRequestsRequestRequestTypeDef

```python
# ListQualificationRequestsRequestRequestTypeDef definition

class ListQualificationRequestsRequestRequestTypeDef(TypedDict):
    QualificationTypeId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## QualificationRequestTypeDef

```python
# QualificationRequestTypeDef definition

class QualificationRequestTypeDef(TypedDict):
    QualificationRequestId: NotRequired[str],
    QualificationTypeId: NotRequired[str],
    WorkerId: NotRequired[str],
    Test: NotRequired[str],
    Answer: NotRequired[str],
    SubmitTime: NotRequired[datetime],
```

## ListQualificationTypesRequestRequestTypeDef

```python
# ListQualificationTypesRequestRequestTypeDef definition

class ListQualificationTypesRequestRequestTypeDef(TypedDict):
    MustBeRequestable: bool,
    Query: NotRequired[str],
    MustBeOwnedByCaller: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListReviewPolicyResultsForHITRequestRequestTypeDef

```python
# ListReviewPolicyResultsForHITRequestRequestTypeDef definition

class ListReviewPolicyResultsForHITRequestRequestTypeDef(TypedDict):
    HITId: str,
    PolicyLevels: NotRequired[Sequence[ReviewPolicyLevelType]],  # (1)
    RetrieveActions: NotRequired[bool],
    RetrieveResults: NotRequired[bool],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ReviewPolicyLevelType](./literals.md#reviewpolicyleveltype) 
## ListReviewableHITsRequestRequestTypeDef

```python
# ListReviewableHITsRequestRequestTypeDef definition

class ListReviewableHITsRequestRequestTypeDef(TypedDict):
    HITTypeId: NotRequired[str],
    Status: NotRequired[ReviewableHITStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: ReviewableHITStatusType](./literals.md#reviewablehitstatustype) 
## ListWorkerBlocksRequestRequestTypeDef

```python
# ListWorkerBlocksRequestRequestTypeDef definition

class ListWorkerBlocksRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## WorkerBlockTypeDef

```python
# WorkerBlockTypeDef definition

class WorkerBlockTypeDef(TypedDict):
    WorkerId: NotRequired[str],
    Reason: NotRequired[str],
```

## ListWorkersWithQualificationTypeRequestRequestTypeDef

```python
# ListWorkersWithQualificationTypeRequestRequestTypeDef definition

class ListWorkersWithQualificationTypeRequestRequestTypeDef(TypedDict):
    QualificationTypeId: str,
    Status: NotRequired[QualificationStatusType],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: QualificationStatusType](./literals.md#qualificationstatustype) 
## LocaleTypeDef

```python
# LocaleTypeDef definition

class LocaleTypeDef(TypedDict):
    Country: str,
    Subdivision: NotRequired[str],
```

## NotificationSpecificationTypeDef

```python
# NotificationSpecificationTypeDef definition

class NotificationSpecificationTypeDef(TypedDict):
    Destination: str,
    Transport: NotificationTransportType,  # (1)
    Version: str,
    EventTypes: Sequence[EventTypeType],  # (2)
```

1. See [:material-code-brackets: NotificationTransportType](./literals.md#notificationtransporttype) 
2. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## NotifyWorkersFailureStatusTypeDef

```python
# NotifyWorkersFailureStatusTypeDef definition

class NotifyWorkersFailureStatusTypeDef(TypedDict):
    NotifyWorkersFailureCode: NotRequired[NotifyWorkersFailureCodeType],  # (1)
    NotifyWorkersFailureMessage: NotRequired[str],
    WorkerId: NotRequired[str],
```

1. See [:material-code-brackets: NotifyWorkersFailureCodeType](./literals.md#notifyworkersfailurecodetype) 
## NotifyWorkersRequestRequestTypeDef

```python
# NotifyWorkersRequestRequestTypeDef definition

class NotifyWorkersRequestRequestTypeDef(TypedDict):
    Subject: str,
    MessageText: str,
    WorkerIds: Sequence[str],
```

## ParameterMapEntryOutputTypeDef

```python
# ParameterMapEntryOutputTypeDef definition

class ParameterMapEntryOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[List[str]],
```

## ParameterMapEntryTypeDef

```python
# ParameterMapEntryTypeDef definition

class ParameterMapEntryTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## RejectAssignmentRequestRequestTypeDef

```python
# RejectAssignmentRequestRequestTypeDef definition

class RejectAssignmentRequestRequestTypeDef(TypedDict):
    AssignmentId: str,
    RequesterFeedback: str,
```

## RejectQualificationRequestRequestRequestTypeDef

```python
# RejectQualificationRequestRequestRequestTypeDef definition

class RejectQualificationRequestRequestRequestTypeDef(TypedDict):
    QualificationRequestId: str,
    Reason: NotRequired[str],
```

## ReviewActionDetailTypeDef

```python
# ReviewActionDetailTypeDef definition

class ReviewActionDetailTypeDef(TypedDict):
    ActionId: NotRequired[str],
    ActionName: NotRequired[str],
    TargetId: NotRequired[str],
    TargetType: NotRequired[str],
    Status: NotRequired[ReviewActionStatusType],  # (1)
    CompleteTime: NotRequired[datetime],
    Result: NotRequired[str],
    ErrorCode: NotRequired[str],
```

1. See [:material-code-brackets: ReviewActionStatusType](./literals.md#reviewactionstatustype) 
## ReviewResultDetailTypeDef

```python
# ReviewResultDetailTypeDef definition

class ReviewResultDetailTypeDef(TypedDict):
    ActionId: NotRequired[str],
    SubjectId: NotRequired[str],
    SubjectType: NotRequired[str],
    QuestionId: NotRequired[str],
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## SendBonusRequestRequestTypeDef

```python
# SendBonusRequestRequestTypeDef definition

class SendBonusRequestRequestTypeDef(TypedDict):
    WorkerId: str,
    BonusAmount: str,
    AssignmentId: str,
    Reason: str,
    UniqueRequestToken: NotRequired[str],
```

## UpdateHITReviewStatusRequestRequestTypeDef

```python
# UpdateHITReviewStatusRequestRequestTypeDef definition

class UpdateHITReviewStatusRequestRequestTypeDef(TypedDict):
    HITId: str,
    Revert: NotRequired[bool],
```

## UpdateHITTypeOfHITRequestRequestTypeDef

```python
# UpdateHITTypeOfHITRequestRequestTypeDef definition

class UpdateHITTypeOfHITRequestRequestTypeDef(TypedDict):
    HITId: str,
    HITTypeId: str,
```

## UpdateQualificationTypeRequestRequestTypeDef

```python
# UpdateQualificationTypeRequestRequestTypeDef definition

class UpdateQualificationTypeRequestRequestTypeDef(TypedDict):
    QualificationTypeId: str,
    Description: NotRequired[str],
    QualificationTypeStatus: NotRequired[QualificationTypeStatusType],  # (1)
    Test: NotRequired[str],
    AnswerKey: NotRequired[str],
    TestDurationInSeconds: NotRequired[int],
    RetryDelayInSeconds: NotRequired[int],
    AutoGranted: NotRequired[bool],
    AutoGrantedValue: NotRequired[int],
```

1. See [:material-code-brackets: QualificationTypeStatusType](./literals.md#qualificationtypestatustype) 
## CreateHITTypeResponseTypeDef

```python
# CreateHITTypeResponseTypeDef definition

class CreateHITTypeResponseTypeDef(TypedDict):
    HITTypeId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountBalanceResponseTypeDef

```python
# GetAccountBalanceResponseTypeDef definition

class GetAccountBalanceResponseTypeDef(TypedDict):
    AvailableBalance: str,
    OnHoldBalance: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFileUploadURLResponseTypeDef

```python
# GetFileUploadURLResponseTypeDef definition

class GetFileUploadURLResponseTypeDef(TypedDict):
    FileUploadURL: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssignmentsForHITResponseTypeDef

```python
# ListAssignmentsForHITResponseTypeDef definition

class ListAssignmentsForHITResponseTypeDef(TypedDict):
    NumResults: int,
    Assignments: List[AssignmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AssignmentTypeDef](./type_defs.md#assignmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBonusPaymentsResponseTypeDef

```python
# ListBonusPaymentsResponseTypeDef definition

class ListBonusPaymentsResponseTypeDef(TypedDict):
    NumResults: int,
    BonusPayments: List[BonusPaymentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: BonusPaymentTypeDef](./type_defs.md#bonuspaymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQualificationTypeResponseTypeDef

```python
# CreateQualificationTypeResponseTypeDef definition

class CreateQualificationTypeResponseTypeDef(TypedDict):
    QualificationType: QualificationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QualificationTypeTypeDef](./type_defs.md#qualificationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQualificationTypeResponseTypeDef

```python
# GetQualificationTypeResponseTypeDef definition

class GetQualificationTypeResponseTypeDef(TypedDict):
    QualificationType: QualificationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QualificationTypeTypeDef](./type_defs.md#qualificationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQualificationTypesResponseTypeDef

```python
# ListQualificationTypesResponseTypeDef definition

class ListQualificationTypesResponseTypeDef(TypedDict):
    NumResults: int,
    QualificationTypes: List[QualificationTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QualificationTypeTypeDef](./type_defs.md#qualificationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQualificationTypeResponseTypeDef

```python
# UpdateQualificationTypeResponseTypeDef definition

class UpdateQualificationTypeResponseTypeDef(TypedDict):
    QualificationType: QualificationTypeTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QualificationTypeTypeDef](./type_defs.md#qualificationtypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssignmentsForHITRequestPaginateTypeDef

```python
# ListAssignmentsForHITRequestPaginateTypeDef definition

class ListAssignmentsForHITRequestPaginateTypeDef(TypedDict):
    HITId: str,
    AssignmentStatuses: NotRequired[Sequence[AssignmentStatusType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AssignmentStatusType](./literals.md#assignmentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBonusPaymentsRequestPaginateTypeDef

```python
# ListBonusPaymentsRequestPaginateTypeDef definition

class ListBonusPaymentsRequestPaginateTypeDef(TypedDict):
    HITId: NotRequired[str],
    AssignmentId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHITsForQualificationTypeRequestPaginateTypeDef

```python
# ListHITsForQualificationTypeRequestPaginateTypeDef definition

class ListHITsForQualificationTypeRequestPaginateTypeDef(TypedDict):
    QualificationTypeId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListHITsRequestPaginateTypeDef

```python
# ListHITsRequestPaginateTypeDef definition

class ListHITsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQualificationRequestsRequestPaginateTypeDef

```python
# ListQualificationRequestsRequestPaginateTypeDef definition

class ListQualificationRequestsRequestPaginateTypeDef(TypedDict):
    QualificationTypeId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQualificationTypesRequestPaginateTypeDef

```python
# ListQualificationTypesRequestPaginateTypeDef definition

class ListQualificationTypesRequestPaginateTypeDef(TypedDict):
    MustBeRequestable: bool,
    Query: NotRequired[str],
    MustBeOwnedByCaller: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReviewableHITsRequestPaginateTypeDef

```python
# ListReviewableHITsRequestPaginateTypeDef definition

class ListReviewableHITsRequestPaginateTypeDef(TypedDict):
    HITTypeId: NotRequired[str],
    Status: NotRequired[ReviewableHITStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ReviewableHITStatusType](./literals.md#reviewablehitstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkerBlocksRequestPaginateTypeDef

```python
# ListWorkerBlocksRequestPaginateTypeDef definition

class ListWorkerBlocksRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkersWithQualificationTypeRequestPaginateTypeDef

```python
# ListWorkersWithQualificationTypeRequestPaginateTypeDef definition

class ListWorkersWithQualificationTypeRequestPaginateTypeDef(TypedDict):
    QualificationTypeId: str,
    Status: NotRequired[QualificationStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: QualificationStatusType](./literals.md#qualificationstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQualificationRequestsResponseTypeDef

```python
# ListQualificationRequestsResponseTypeDef definition

class ListQualificationRequestsResponseTypeDef(TypedDict):
    NumResults: int,
    QualificationRequests: List[QualificationRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QualificationRequestTypeDef](./type_defs.md#qualificationrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkerBlocksResponseTypeDef

```python
# ListWorkerBlocksResponseTypeDef definition

class ListWorkerBlocksResponseTypeDef(TypedDict):
    NumResults: int,
    WorkerBlocks: List[WorkerBlockTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkerBlockTypeDef](./type_defs.md#workerblocktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## QualificationRequirementOutputTypeDef

```python
# QualificationRequirementOutputTypeDef definition

class QualificationRequirementOutputTypeDef(TypedDict):
    QualificationTypeId: str,
    Comparator: ComparatorType,  # (1)
    IntegerValues: NotRequired[List[int]],
    LocaleValues: NotRequired[List[LocaleTypeDef]],  # (2)
    RequiredToPreview: NotRequired[bool],
    ActionsGuarded: NotRequired[HITAccessActionsType],  # (3)
```

1. See [:material-code-brackets: ComparatorType](./literals.md#comparatortype) 
2. See [:material-code-braces: LocaleTypeDef](./type_defs.md#localetypedef) 
3. See [:material-code-brackets: HITAccessActionsType](./literals.md#hitaccessactionstype) 
## QualificationRequirementTypeDef

```python
# QualificationRequirementTypeDef definition

class QualificationRequirementTypeDef(TypedDict):
    QualificationTypeId: str,
    Comparator: ComparatorType,  # (1)
    IntegerValues: NotRequired[Sequence[int]],
    LocaleValues: NotRequired[Sequence[LocaleTypeDef]],  # (2)
    RequiredToPreview: NotRequired[bool],
    ActionsGuarded: NotRequired[HITAccessActionsType],  # (3)
```

1. See [:material-code-brackets: ComparatorType](./literals.md#comparatortype) 
2. See [:material-code-braces: LocaleTypeDef](./type_defs.md#localetypedef) 
3. See [:material-code-brackets: HITAccessActionsType](./literals.md#hitaccessactionstype) 
## QualificationTypeDef

```python
# QualificationTypeDef definition

class QualificationTypeDef(TypedDict):
    QualificationTypeId: NotRequired[str],
    WorkerId: NotRequired[str],
    GrantTime: NotRequired[datetime],
    IntegerValue: NotRequired[int],
    LocaleValue: NotRequired[LocaleTypeDef],  # (1)
    Status: NotRequired[QualificationStatusType],  # (2)
```

1. See [:material-code-braces: LocaleTypeDef](./type_defs.md#localetypedef) 
2. See [:material-code-brackets: QualificationStatusType](./literals.md#qualificationstatustype) 
## SendTestEventNotificationRequestRequestTypeDef

```python
# SendTestEventNotificationRequestRequestTypeDef definition

class SendTestEventNotificationRequestRequestTypeDef(TypedDict):
    Notification: NotificationSpecificationTypeDef,  # (1)
    TestEventType: EventTypeType,  # (2)
```

1. See [:material-code-braces: NotificationSpecificationTypeDef](./type_defs.md#notificationspecificationtypedef) 
2. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype) 
## UpdateNotificationSettingsRequestRequestTypeDef

```python
# UpdateNotificationSettingsRequestRequestTypeDef definition

class UpdateNotificationSettingsRequestRequestTypeDef(TypedDict):
    HITTypeId: str,
    Notification: NotRequired[NotificationSpecificationTypeDef],  # (1)
    Active: NotRequired[bool],
```

1. See [:material-code-braces: NotificationSpecificationTypeDef](./type_defs.md#notificationspecificationtypedef) 
## NotifyWorkersResponseTypeDef

```python
# NotifyWorkersResponseTypeDef definition

class NotifyWorkersResponseTypeDef(TypedDict):
    NotifyWorkersFailureStatuses: List[NotifyWorkersFailureStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NotifyWorkersFailureStatusTypeDef](./type_defs.md#notifyworkersfailurestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyParameterOutputTypeDef

```python
# PolicyParameterOutputTypeDef definition

class PolicyParameterOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[List[str]],
    MapEntries: NotRequired[List[ParameterMapEntryOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterMapEntryOutputTypeDef](./type_defs.md#parametermapentryoutputtypedef) 
## ReviewReportTypeDef

```python
# ReviewReportTypeDef definition

class ReviewReportTypeDef(TypedDict):
    ReviewResults: NotRequired[List[ReviewResultDetailTypeDef]],  # (1)
    ReviewActions: NotRequired[List[ReviewActionDetailTypeDef]],  # (2)
```

1. See [:material-code-braces: ReviewResultDetailTypeDef](./type_defs.md#reviewresultdetailtypedef) 
2. See [:material-code-braces: ReviewActionDetailTypeDef](./type_defs.md#reviewactiondetailtypedef) 
## UpdateExpirationForHITRequestRequestTypeDef

```python
# UpdateExpirationForHITRequestRequestTypeDef definition

class UpdateExpirationForHITRequestRequestTypeDef(TypedDict):
    HITId: str,
    ExpireAt: TimestampTypeDef,
```

## HITTypeDef

```python
# HITTypeDef definition

class HITTypeDef(TypedDict):
    HITId: NotRequired[str],
    HITTypeId: NotRequired[str],
    HITGroupId: NotRequired[str],
    HITLayoutId: NotRequired[str],
    CreationTime: NotRequired[datetime],
    Title: NotRequired[str],
    Description: NotRequired[str],
    Question: NotRequired[str],
    Keywords: NotRequired[str],
    HITStatus: NotRequired[HITStatusType],  # (1)
    MaxAssignments: NotRequired[int],
    Reward: NotRequired[str],
    AutoApprovalDelayInSeconds: NotRequired[int],
    Expiration: NotRequired[datetime],
    AssignmentDurationInSeconds: NotRequired[int],
    RequesterAnnotation: NotRequired[str],
    QualificationRequirements: NotRequired[List[QualificationRequirementOutputTypeDef]],  # (2)
    HITReviewStatus: NotRequired[HITReviewStatusType],  # (3)
    NumberOfAssignmentsPending: NotRequired[int],
    NumberOfAssignmentsAvailable: NotRequired[int],
    NumberOfAssignmentsCompleted: NotRequired[int],
```

1. See [:material-code-brackets: HITStatusType](./literals.md#hitstatustype) 
2. See [:material-code-braces: QualificationRequirementOutputTypeDef](./type_defs.md#qualificationrequirementoutputtypedef) 
3. See [:material-code-brackets: HITReviewStatusType](./literals.md#hitreviewstatustype) 
## CreateHITTypeRequestRequestTypeDef

```python
# CreateHITTypeRequestRequestTypeDef definition

class CreateHITTypeRequestRequestTypeDef(TypedDict):
    AssignmentDurationInSeconds: int,
    Reward: str,
    Title: str,
    Description: str,
    AutoApprovalDelayInSeconds: NotRequired[int],
    Keywords: NotRequired[str],
    QualificationRequirements: NotRequired[Sequence[QualificationRequirementTypeDef]],  # (1)
```

1. See [:material-code-braces: QualificationRequirementTypeDef](./type_defs.md#qualificationrequirementtypedef) 
## GetQualificationScoreResponseTypeDef

```python
# GetQualificationScoreResponseTypeDef definition

class GetQualificationScoreResponseTypeDef(TypedDict):
    Qualification: QualificationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QualificationTypeDef](./type_defs.md#qualificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkersWithQualificationTypeResponseTypeDef

```python
# ListWorkersWithQualificationTypeResponseTypeDef definition

class ListWorkersWithQualificationTypeResponseTypeDef(TypedDict):
    NumResults: int,
    Qualifications: List[QualificationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QualificationTypeDef](./type_defs.md#qualificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReviewPolicyOutputTypeDef

```python
# ReviewPolicyOutputTypeDef definition

class ReviewPolicyOutputTypeDef(TypedDict):
    PolicyName: str,
    Parameters: NotRequired[List[PolicyParameterOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyParameterOutputTypeDef](./type_defs.md#policyparameteroutputtypedef) 
## PolicyParameterTypeDef

```python
# PolicyParameterTypeDef definition

class PolicyParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[Sequence[str]],
    MapEntries: NotRequired[Sequence[ParameterMapEntryUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ParameterMapEntryTypeDef](./type_defs.md#parametermapentrytypedef) [:material-code-braces: ParameterMapEntryOutputTypeDef](./type_defs.md#parametermapentryoutputtypedef) 
## CreateHITResponseTypeDef

```python
# CreateHITResponseTypeDef definition

class CreateHITResponseTypeDef(TypedDict):
    HIT: HITTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HITTypeDef](./type_defs.md#hittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateHITWithHITTypeResponseTypeDef

```python
# CreateHITWithHITTypeResponseTypeDef definition

class CreateHITWithHITTypeResponseTypeDef(TypedDict):
    HIT: HITTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HITTypeDef](./type_defs.md#hittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssignmentResponseTypeDef

```python
# GetAssignmentResponseTypeDef definition

class GetAssignmentResponseTypeDef(TypedDict):
    Assignment: AssignmentTypeDef,  # (1)
    HIT: HITTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssignmentTypeDef](./type_defs.md#assignmenttypedef) 
2. See [:material-code-braces: HITTypeDef](./type_defs.md#hittypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetHITResponseTypeDef

```python
# GetHITResponseTypeDef definition

class GetHITResponseTypeDef(TypedDict):
    HIT: HITTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: HITTypeDef](./type_defs.md#hittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHITsForQualificationTypeResponseTypeDef

```python
# ListHITsForQualificationTypeResponseTypeDef definition

class ListHITsForQualificationTypeResponseTypeDef(TypedDict):
    NumResults: int,
    HITs: List[HITTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HITTypeDef](./type_defs.md#hittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListHITsResponseTypeDef

```python
# ListHITsResponseTypeDef definition

class ListHITsResponseTypeDef(TypedDict):
    NumResults: int,
    HITs: List[HITTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HITTypeDef](./type_defs.md#hittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReviewableHITsResponseTypeDef

```python
# ListReviewableHITsResponseTypeDef definition

class ListReviewableHITsResponseTypeDef(TypedDict):
    NumResults: int,
    HITs: List[HITTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: HITTypeDef](./type_defs.md#hittypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReviewPolicyResultsForHITResponseTypeDef

```python
# ListReviewPolicyResultsForHITResponseTypeDef definition

class ListReviewPolicyResultsForHITResponseTypeDef(TypedDict):
    HITId: str,
    AssignmentReviewPolicy: ReviewPolicyOutputTypeDef,  # (1)
    HITReviewPolicy: ReviewPolicyOutputTypeDef,  # (1)
    AssignmentReviewReport: ReviewReportTypeDef,  # (3)
    HITReviewReport: ReviewReportTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReviewPolicyOutputTypeDef](./type_defs.md#reviewpolicyoutputtypedef) 
2. See [:material-code-braces: ReviewPolicyOutputTypeDef](./type_defs.md#reviewpolicyoutputtypedef) 
3. See [:material-code-braces: ReviewReportTypeDef](./type_defs.md#reviewreporttypedef) 
4. See [:material-code-braces: ReviewReportTypeDef](./type_defs.md#reviewreporttypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReviewPolicyTypeDef

```python
# ReviewPolicyTypeDef definition

class ReviewPolicyTypeDef(TypedDict):
    PolicyName: str,
    Parameters: NotRequired[Sequence[PolicyParameterUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: PolicyParameterTypeDef](./type_defs.md#policyparametertypedef) [:material-code-braces: PolicyParameterOutputTypeDef](./type_defs.md#policyparameteroutputtypedef) 
## CreateHITRequestRequestTypeDef

```python
# CreateHITRequestRequestTypeDef definition

class CreateHITRequestRequestTypeDef(TypedDict):
    LifetimeInSeconds: int,
    AssignmentDurationInSeconds: int,
    Reward: str,
    Title: str,
    Description: str,
    MaxAssignments: NotRequired[int],
    AutoApprovalDelayInSeconds: NotRequired[int],
    Keywords: NotRequired[str],
    Question: NotRequired[str],
    RequesterAnnotation: NotRequired[str],
    QualificationRequirements: NotRequired[Sequence[QualificationRequirementUnionTypeDef]],  # (1)
    UniqueRequestToken: NotRequired[str],
    AssignmentReviewPolicy: NotRequired[ReviewPolicyTypeDef],  # (2)
    HITReviewPolicy: NotRequired[ReviewPolicyTypeDef],  # (2)
    HITLayoutId: NotRequired[str],
    HITLayoutParameters: NotRequired[Sequence[HITLayoutParameterTypeDef]],  # (4)
```

1. See [:material-code-braces: QualificationRequirementTypeDef](./type_defs.md#qualificationrequirementtypedef) [:material-code-braces: QualificationRequirementOutputTypeDef](./type_defs.md#qualificationrequirementoutputtypedef) 
2. See [:material-code-braces: ReviewPolicyTypeDef](./type_defs.md#reviewpolicytypedef) 
3. See [:material-code-braces: ReviewPolicyTypeDef](./type_defs.md#reviewpolicytypedef) 
4. See [:material-code-braces: HITLayoutParameterTypeDef](./type_defs.md#hitlayoutparametertypedef) 
## CreateHITWithHITTypeRequestRequestTypeDef

```python
# CreateHITWithHITTypeRequestRequestTypeDef definition

class CreateHITWithHITTypeRequestRequestTypeDef(TypedDict):
    HITTypeId: str,
    LifetimeInSeconds: int,
    MaxAssignments: NotRequired[int],
    Question: NotRequired[str],
    RequesterAnnotation: NotRequired[str],
    UniqueRequestToken: NotRequired[str],
    AssignmentReviewPolicy: NotRequired[ReviewPolicyTypeDef],  # (1)
    HITReviewPolicy: NotRequired[ReviewPolicyTypeDef],  # (1)
    HITLayoutId: NotRequired[str],
    HITLayoutParameters: NotRequired[Sequence[HITLayoutParameterTypeDef]],  # (3)
```

1. See [:material-code-braces: ReviewPolicyTypeDef](./type_defs.md#reviewpolicytypedef) 
2. See [:material-code-braces: ReviewPolicyTypeDef](./type_defs.md#reviewpolicytypedef) 
3. See [:material-code-braces: HITLayoutParameterTypeDef](./type_defs.md#hitlayoutparametertypedef) 

# Type definitions

> [Index](../README.md) > [SecurityIncidentResponse](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SecurityIncidentResponse](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#securityincidentresponse)
    type annotations stubs module [types-aiobotocore-security-ir](https://pypi.org/project/types-aiobotocore-security-ir/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## BatchGetMemberAccountDetailsRequestRequestTypeDef

```python
# BatchGetMemberAccountDetailsRequestRequestTypeDef definition

class BatchGetMemberAccountDetailsRequestRequestTypeDef(TypedDict):
    membershipId: str,
    accountIds: Sequence[str],
```

## GetMembershipAccountDetailErrorTypeDef

```python
# GetMembershipAccountDetailErrorTypeDef definition

class GetMembershipAccountDetailErrorTypeDef(TypedDict):
    accountId: str,
    error: str,
    message: str,
```

## GetMembershipAccountDetailItemTypeDef

```python
# GetMembershipAccountDetailItemTypeDef definition

class GetMembershipAccountDetailItemTypeDef(TypedDict):
    accountId: NotRequired[str],
    relationshipStatus: NotRequired[MembershipAccountRelationshipStatusType],  # (1)
    relationshipType: NotRequired[MembershipAccountRelationshipTypeType],  # (2)
```

1. See [:material-code-brackets: MembershipAccountRelationshipStatusType](./literals.md#membershipaccountrelationshipstatustype) 
2. See [:material-code-brackets: MembershipAccountRelationshipTypeType](./literals.md#membershipaccountrelationshiptypetype) 
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

## CancelMembershipRequestRequestTypeDef

```python
# CancelMembershipRequestRequestTypeDef definition

class CancelMembershipRequestRequestTypeDef(TypedDict):
    membershipId: str,
```

## CaseAttachmentAttributesTypeDef

```python
# CaseAttachmentAttributesTypeDef definition

class CaseAttachmentAttributesTypeDef(TypedDict):
    attachmentId: str,
    fileName: str,
    attachmentStatus: CaseAttachmentStatusType,  # (1)
    creator: str,
    createdDate: datetime,
```

1. See [:material-code-brackets: CaseAttachmentStatusType](./literals.md#caseattachmentstatustype) 
## CaseEditItemTypeDef

```python
# CaseEditItemTypeDef definition

class CaseEditItemTypeDef(TypedDict):
    eventTimestamp: NotRequired[datetime],
    principal: NotRequired[str],
    action: NotRequired[str],
    message: NotRequired[str],
```

## CloseCaseRequestRequestTypeDef

```python
# CloseCaseRequestRequestTypeDef definition

class CloseCaseRequestRequestTypeDef(TypedDict):
    caseId: str,
```

## CreateCaseCommentRequestRequestTypeDef

```python
# CreateCaseCommentRequestRequestTypeDef definition

class CreateCaseCommentRequestRequestTypeDef(TypedDict):
    caseId: str,
    body: str,
    clientToken: NotRequired[str],
```

## ImpactedAwsRegionTypeDef

```python
# ImpactedAwsRegionTypeDef definition

class ImpactedAwsRegionTypeDef(TypedDict):
    region: AwsRegionType,  # (1)
```

1. See [:material-code-brackets: AwsRegionType](./literals.md#awsregiontype) 
## ThreatActorIpTypeDef

```python
# ThreatActorIpTypeDef definition

class ThreatActorIpTypeDef(TypedDict):
    ipAddress: str,
    userAgent: NotRequired[str],
```

## WatcherTypeDef

```python
# WatcherTypeDef definition

class WatcherTypeDef(TypedDict):
    email: str,
    name: NotRequired[str],
    jobTitle: NotRequired[str],
```

## IncidentResponderTypeDef

```python
# IncidentResponderTypeDef definition

class IncidentResponderTypeDef(TypedDict):
    name: str,
    jobTitle: str,
    email: str,
```

## OptInFeatureTypeDef

```python
# OptInFeatureTypeDef definition

class OptInFeatureTypeDef(TypedDict):
    featureName: OptInFeatureNameType,  # (1)
    isEnabled: bool,
```

1. See [:material-code-brackets: OptInFeatureNameType](./literals.md#optinfeaturenametype) 
## GetCaseAttachmentDownloadUrlRequestRequestTypeDef

```python
# GetCaseAttachmentDownloadUrlRequestRequestTypeDef definition

class GetCaseAttachmentDownloadUrlRequestRequestTypeDef(TypedDict):
    caseId: str,
    attachmentId: str,
```

## GetCaseAttachmentUploadUrlRequestRequestTypeDef

```python
# GetCaseAttachmentUploadUrlRequestRequestTypeDef definition

class GetCaseAttachmentUploadUrlRequestRequestTypeDef(TypedDict):
    caseId: str,
    fileName: str,
    contentLength: int,
    clientToken: NotRequired[str],
```

## GetCaseRequestRequestTypeDef

```python
# GetCaseRequestRequestTypeDef definition

class GetCaseRequestRequestTypeDef(TypedDict):
    caseId: str,
```

## GetMembershipRequestRequestTypeDef

```python
# GetMembershipRequestRequestTypeDef definition

class GetMembershipRequestRequestTypeDef(TypedDict):
    membershipId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListCaseEditsRequestRequestTypeDef

```python
# ListCaseEditsRequestRequestTypeDef definition

class ListCaseEditsRequestRequestTypeDef(TypedDict):
    caseId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCasesItemTypeDef

```python
# ListCasesItemTypeDef definition

class ListCasesItemTypeDef(TypedDict):
    caseId: str,
    lastUpdatedDate: NotRequired[datetime],
    title: NotRequired[str],
    caseArn: NotRequired[str],
    engagementType: NotRequired[EngagementTypeType],  # (1)
    caseStatus: NotRequired[CaseStatusType],  # (2)
    createdDate: NotRequired[datetime],
    closedDate: NotRequired[datetime],
    resolverType: NotRequired[ResolverTypeType],  # (3)
    pendingAction: NotRequired[PendingActionType],  # (4)
```

1. See [:material-code-brackets: EngagementTypeType](./literals.md#engagementtypetype) 
2. See [:material-code-brackets: CaseStatusType](./literals.md#casestatustype) 
3. See [:material-code-brackets: ResolverTypeType](./literals.md#resolvertypetype) 
4. See [:material-code-brackets: PendingActionType](./literals.md#pendingactiontype) 
## ListCasesRequestRequestTypeDef

```python
# ListCasesRequestRequestTypeDef definition

class ListCasesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListCommentsItemTypeDef

```python
# ListCommentsItemTypeDef definition

class ListCommentsItemTypeDef(TypedDict):
    commentId: str,
    createdDate: NotRequired[datetime],
    lastUpdatedDate: NotRequired[datetime],
    creator: NotRequired[str],
    lastUpdatedBy: NotRequired[str],
    body: NotRequired[str],
```

## ListCommentsRequestRequestTypeDef

```python
# ListCommentsRequestRequestTypeDef definition

class ListCommentsRequestRequestTypeDef(TypedDict):
    caseId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListMembershipItemTypeDef

```python
# ListMembershipItemTypeDef definition

class ListMembershipItemTypeDef(TypedDict):
    membershipId: str,
    accountId: NotRequired[str],
    region: NotRequired[AwsRegionType],  # (1)
    membershipArn: NotRequired[str],
    membershipStatus: NotRequired[MembershipStatusType],  # (2)
```

1. See [:material-code-brackets: AwsRegionType](./literals.md#awsregiontype) 
2. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
## ListMembershipsRequestRequestTypeDef

```python
# ListMembershipsRequestRequestTypeDef definition

class ListMembershipsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateCaseCommentRequestRequestTypeDef

```python
# UpdateCaseCommentRequestRequestTypeDef definition

class UpdateCaseCommentRequestRequestTypeDef(TypedDict):
    caseId: str,
    commentId: str,
    body: str,
```

## UpdateCaseStatusRequestRequestTypeDef

```python
# UpdateCaseStatusRequestRequestTypeDef definition

class UpdateCaseStatusRequestRequestTypeDef(TypedDict):
    caseId: str,
    caseStatus: SelfManagedCaseStatusType,  # (1)
```

1. See [:material-code-brackets: SelfManagedCaseStatusType](./literals.md#selfmanagedcasestatustype) 
## UpdateResolverTypeRequestRequestTypeDef

```python
# UpdateResolverTypeRequestRequestTypeDef definition

class UpdateResolverTypeRequestRequestTypeDef(TypedDict):
    caseId: str,
    resolverType: ResolverTypeType,  # (1)
```

1. See [:material-code-brackets: ResolverTypeType](./literals.md#resolvertypetype) 
## BatchGetMemberAccountDetailsResponseTypeDef

```python
# BatchGetMemberAccountDetailsResponseTypeDef definition

class BatchGetMemberAccountDetailsResponseTypeDef(TypedDict):
    items: List[GetMembershipAccountDetailItemTypeDef],  # (1)
    errors: List[GetMembershipAccountDetailErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: GetMembershipAccountDetailItemTypeDef](./type_defs.md#getmembershipaccountdetailitemtypedef) 
2. See [:material-code-braces: GetMembershipAccountDetailErrorTypeDef](./type_defs.md#getmembershipaccountdetailerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelMembershipResponseTypeDef

```python
# CancelMembershipResponseTypeDef definition

class CancelMembershipResponseTypeDef(TypedDict):
    membershipId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CloseCaseResponseTypeDef

```python
# CloseCaseResponseTypeDef definition

class CloseCaseResponseTypeDef(TypedDict):
    caseStatus: CaseStatusType,  # (1)
    closedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CaseStatusType](./literals.md#casestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseCommentResponseTypeDef

```python
# CreateCaseCommentResponseTypeDef definition

class CreateCaseCommentResponseTypeDef(TypedDict):
    commentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseResponseTypeDef

```python
# CreateCaseResponseTypeDef definition

class CreateCaseResponseTypeDef(TypedDict):
    caseId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateMembershipResponseTypeDef

```python
# CreateMembershipResponseTypeDef definition

class CreateMembershipResponseTypeDef(TypedDict):
    membershipId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCaseAttachmentDownloadUrlResponseTypeDef

```python
# GetCaseAttachmentDownloadUrlResponseTypeDef definition

class GetCaseAttachmentDownloadUrlResponseTypeDef(TypedDict):
    attachmentPresignedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCaseAttachmentUploadUrlResponseTypeDef

```python
# GetCaseAttachmentUploadUrlResponseTypeDef definition

class GetCaseAttachmentUploadUrlResponseTypeDef(TypedDict):
    attachmentPresignedUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCaseCommentResponseTypeDef

```python
# UpdateCaseCommentResponseTypeDef definition

class UpdateCaseCommentResponseTypeDef(TypedDict):
    commentId: str,
    body: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCaseStatusResponseTypeDef

```python
# UpdateCaseStatusResponseTypeDef definition

class UpdateCaseStatusResponseTypeDef(TypedDict):
    caseStatus: SelfManagedCaseStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: SelfManagedCaseStatusType](./literals.md#selfmanagedcasestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResolverTypeResponseTypeDef

```python
# UpdateResolverTypeResponseTypeDef definition

class UpdateResolverTypeResponseTypeDef(TypedDict):
    caseId: str,
    caseStatus: CaseStatusType,  # (1)
    resolverType: ResolverTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: CaseStatusType](./literals.md#casestatustype) 
2. See [:material-code-brackets: ResolverTypeType](./literals.md#resolvertypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCaseEditsResponseTypeDef

```python
# ListCaseEditsResponseTypeDef definition

class ListCaseEditsResponseTypeDef(TypedDict):
    items: List[CaseEditItemTypeDef],  # (1)
    total: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CaseEditItemTypeDef](./type_defs.md#caseedititemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseRequestRequestTypeDef

```python
# CreateCaseRequestRequestTypeDef definition

class CreateCaseRequestRequestTypeDef(TypedDict):
    resolverType: ResolverTypeType,  # (1)
    title: str,
    description: str,
    engagementType: EngagementTypeType,  # (2)
    reportedIncidentStartDate: TimestampTypeDef,
    impactedAccounts: Sequence[str],
    watchers: Sequence[WatcherTypeDef],  # (3)
    clientToken: NotRequired[str],
    threatActorIpAddresses: NotRequired[Sequence[ThreatActorIpTypeDef]],  # (4)
    impactedServices: NotRequired[Sequence[str]],
    impactedAwsRegions: NotRequired[Sequence[ImpactedAwsRegionTypeDef]],  # (5)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ResolverTypeType](./literals.md#resolvertypetype) 
2. See [:material-code-brackets: EngagementTypeType](./literals.md#engagementtypetype) 
3. See [:material-code-braces: WatcherTypeDef](./type_defs.md#watchertypedef) 
4. See [:material-code-braces: ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef) 
5. See [:material-code-braces: ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef) 
## GetCaseResponseTypeDef

```python
# GetCaseResponseTypeDef definition

class GetCaseResponseTypeDef(TypedDict):
    title: str,
    caseArn: str,
    description: str,
    caseStatus: CaseStatusType,  # (1)
    engagementType: EngagementTypeType,  # (2)
    reportedIncidentStartDate: datetime,
    actualIncidentStartDate: datetime,
    impactedAwsRegions: List[ImpactedAwsRegionTypeDef],  # (3)
    threatActorIpAddresses: List[ThreatActorIpTypeDef],  # (4)
    pendingAction: PendingActionType,  # (5)
    impactedAccounts: List[str],
    watchers: List[WatcherTypeDef],  # (6)
    createdDate: datetime,
    lastUpdatedDate: datetime,
    closureCode: ClosureCodeType,  # (7)
    resolverType: ResolverTypeType,  # (8)
    impactedServices: List[str],
    caseAttachments: List[CaseAttachmentAttributesTypeDef],  # (9)
    closedDate: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-brackets: CaseStatusType](./literals.md#casestatustype) 
2. See [:material-code-brackets: EngagementTypeType](./literals.md#engagementtypetype) 
3. See [:material-code-braces: ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef) 
4. See [:material-code-braces: ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef) 
5. See [:material-code-brackets: PendingActionType](./literals.md#pendingactiontype) 
6. See [:material-code-braces: WatcherTypeDef](./type_defs.md#watchertypedef) 
7. See [:material-code-brackets: ClosureCodeType](./literals.md#closurecodetype) 
8. See [:material-code-brackets: ResolverTypeType](./literals.md#resolvertypetype) 
9. See [:material-code-braces: CaseAttachmentAttributesTypeDef](./type_defs.md#caseattachmentattributestypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCaseRequestRequestTypeDef

```python
# UpdateCaseRequestRequestTypeDef definition

class UpdateCaseRequestRequestTypeDef(TypedDict):
    caseId: str,
    title: NotRequired[str],
    description: NotRequired[str],
    reportedIncidentStartDate: NotRequired[TimestampTypeDef],
    actualIncidentStartDate: NotRequired[TimestampTypeDef],
    engagementType: NotRequired[EngagementTypeType],  # (1)
    watchersToAdd: NotRequired[Sequence[WatcherTypeDef]],  # (2)
    watchersToDelete: NotRequired[Sequence[WatcherTypeDef]],  # (2)
    threatActorIpAddressesToAdd: NotRequired[Sequence[ThreatActorIpTypeDef]],  # (4)
    threatActorIpAddressesToDelete: NotRequired[Sequence[ThreatActorIpTypeDef]],  # (4)
    impactedServicesToAdd: NotRequired[Sequence[str]],
    impactedServicesToDelete: NotRequired[Sequence[str]],
    impactedAwsRegionsToAdd: NotRequired[Sequence[ImpactedAwsRegionTypeDef]],  # (6)
    impactedAwsRegionsToDelete: NotRequired[Sequence[ImpactedAwsRegionTypeDef]],  # (6)
    impactedAccountsToAdd: NotRequired[Sequence[str]],
    impactedAccountsToDelete: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: EngagementTypeType](./literals.md#engagementtypetype) 
2. See [:material-code-braces: WatcherTypeDef](./type_defs.md#watchertypedef) 
3. See [:material-code-braces: WatcherTypeDef](./type_defs.md#watchertypedef) 
4. See [:material-code-braces: ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef) 
5. See [:material-code-braces: ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef) 
6. See [:material-code-braces: ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef) 
7. See [:material-code-braces: ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef) 
## CreateMembershipRequestRequestTypeDef

```python
# CreateMembershipRequestRequestTypeDef definition

class CreateMembershipRequestRequestTypeDef(TypedDict):
    membershipName: str,
    incidentResponseTeam: Sequence[IncidentResponderTypeDef],  # (1)
    clientToken: NotRequired[str],
    optInFeatures: NotRequired[Sequence[OptInFeatureTypeDef]],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: IncidentResponderTypeDef](./type_defs.md#incidentrespondertypedef) 
2. See [:material-code-braces: OptInFeatureTypeDef](./type_defs.md#optinfeaturetypedef) 
## GetMembershipResponseTypeDef

```python
# GetMembershipResponseTypeDef definition

class GetMembershipResponseTypeDef(TypedDict):
    membershipId: str,
    accountId: str,
    region: AwsRegionType,  # (1)
    membershipName: str,
    membershipArn: str,
    membershipStatus: MembershipStatusType,  # (2)
    membershipActivationTimestamp: datetime,
    membershipDeactivationTimestamp: datetime,
    customerType: CustomerTypeType,  # (3)
    numberOfAccountsCovered: int,
    incidentResponseTeam: List[IncidentResponderTypeDef],  # (4)
    optInFeatures: List[OptInFeatureTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: AwsRegionType](./literals.md#awsregiontype) 
2. See [:material-code-brackets: MembershipStatusType](./literals.md#membershipstatustype) 
3. See [:material-code-brackets: CustomerTypeType](./literals.md#customertypetype) 
4. See [:material-code-braces: IncidentResponderTypeDef](./type_defs.md#incidentrespondertypedef) 
5. See [:material-code-braces: OptInFeatureTypeDef](./type_defs.md#optinfeaturetypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateMembershipRequestRequestTypeDef

```python
# UpdateMembershipRequestRequestTypeDef definition

class UpdateMembershipRequestRequestTypeDef(TypedDict):
    membershipId: str,
    membershipName: NotRequired[str],
    incidentResponseTeam: NotRequired[Sequence[IncidentResponderTypeDef]],  # (1)
    optInFeatures: NotRequired[Sequence[OptInFeatureTypeDef]],  # (2)
```

1. See [:material-code-braces: IncidentResponderTypeDef](./type_defs.md#incidentrespondertypedef) 
2. See [:material-code-braces: OptInFeatureTypeDef](./type_defs.md#optinfeaturetypedef) 
## ListCaseEditsRequestPaginateTypeDef

```python
# ListCaseEditsRequestPaginateTypeDef definition

class ListCaseEditsRequestPaginateTypeDef(TypedDict):
    caseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCasesRequestPaginateTypeDef

```python
# ListCasesRequestPaginateTypeDef definition

class ListCasesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCommentsRequestPaginateTypeDef

```python
# ListCommentsRequestPaginateTypeDef definition

class ListCommentsRequestPaginateTypeDef(TypedDict):
    caseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMembershipsRequestPaginateTypeDef

```python
# ListMembershipsRequestPaginateTypeDef definition

class ListMembershipsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCasesResponseTypeDef

```python
# ListCasesResponseTypeDef definition

class ListCasesResponseTypeDef(TypedDict):
    items: List[ListCasesItemTypeDef],  # (1)
    total: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListCasesItemTypeDef](./type_defs.md#listcasesitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCommentsResponseTypeDef

```python
# ListCommentsResponseTypeDef definition

class ListCommentsResponseTypeDef(TypedDict):
    items: List[ListCommentsItemTypeDef],  # (1)
    total: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListCommentsItemTypeDef](./type_defs.md#listcommentsitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListMembershipsResponseTypeDef

```python
# ListMembershipsResponseTypeDef definition

class ListMembershipsResponseTypeDef(TypedDict):
    items: List[ListMembershipItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ListMembershipItemTypeDef](./type_defs.md#listmembershipitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

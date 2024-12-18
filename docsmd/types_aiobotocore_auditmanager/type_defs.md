# Type definitions

> [Index](../README.md) > [AuditManager](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AuditManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/auditmanager.html#auditmanager)
    type annotations stubs module [types-aiobotocore-auditmanager](https://pypi.org/project/types-aiobotocore-auditmanager/).



## AWSAccountTypeDef

```python
# AWSAccountTypeDef definition

class AWSAccountTypeDef(TypedDict):
    id: NotRequired[str],
    emailAddress: NotRequired[str],
    name: NotRequired[str],
```

## AWSServiceTypeDef

```python
# AWSServiceTypeDef definition

class AWSServiceTypeDef(TypedDict):
    serviceName: NotRequired[str],
```

## DelegationTypeDef

```python
# DelegationTypeDef definition

class DelegationTypeDef(TypedDict):
    id: NotRequired[str],
    assessmentName: NotRequired[str],
    assessmentId: NotRequired[str],
    status: NotRequired[DelegationStatusType],  # (1)
    roleArn: NotRequired[str],
    roleType: NotRequired[RoleTypeType],  # (2)
    creationTime: NotRequired[datetime],
    lastUpdated: NotRequired[datetime],
    controlSetId: NotRequired[str],
    comment: NotRequired[str],
    createdBy: NotRequired[str],
```

1. See [:material-code-brackets: DelegationStatusType](./literals.md#delegationstatustype) 
2. See [:material-code-brackets: RoleTypeType](./literals.md#roletypetype) 
## RoleTypeDef

```python
# RoleTypeDef definition

class RoleTypeDef(TypedDict):
    roleType: RoleTypeType,  # (1)
    roleArn: str,
```

1. See [:material-code-brackets: RoleTypeType](./literals.md#roletypetype) 
## ControlCommentTypeDef

```python
# ControlCommentTypeDef definition

class ControlCommentTypeDef(TypedDict):
    authorName: NotRequired[str],
    commentBody: NotRequired[str],
    postedDate: NotRequired[datetime],
```

## AssessmentEvidenceFolderTypeDef

```python
# AssessmentEvidenceFolderTypeDef definition

class AssessmentEvidenceFolderTypeDef(TypedDict):
    name: NotRequired[str],
    date: NotRequired[datetime],
    assessmentId: NotRequired[str],
    controlSetId: NotRequired[str],
    controlId: NotRequired[str],
    id: NotRequired[str],
    dataSource: NotRequired[str],
    author: NotRequired[str],
    totalEvidence: NotRequired[int],
    assessmentReportSelectionCount: NotRequired[int],
    controlName: NotRequired[str],
    evidenceResourcesIncludedCount: NotRequired[int],
    evidenceByTypeConfigurationDataCount: NotRequired[int],
    evidenceByTypeManualCount: NotRequired[int],
    evidenceByTypeComplianceCheckCount: NotRequired[int],
    evidenceByTypeComplianceCheckIssuesCount: NotRequired[int],
    evidenceByTypeUserActivityCount: NotRequired[int],
    evidenceAwsServiceSourceCount: NotRequired[int],
```

## AssessmentFrameworkMetadataTypeDef

```python
# AssessmentFrameworkMetadataTypeDef definition

class AssessmentFrameworkMetadataTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    type: NotRequired[FrameworkTypeType],  # (1)
    name: NotRequired[str],
    description: NotRequired[str],
    logo: NotRequired[str],
    complianceType: NotRequired[str],
    controlsCount: NotRequired[int],
    controlSetsCount: NotRequired[int],
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: FrameworkTypeType](./literals.md#frameworktypetype) 
## AssessmentFrameworkShareRequestTypeDef

```python
# AssessmentFrameworkShareRequestTypeDef definition

class AssessmentFrameworkShareRequestTypeDef(TypedDict):
    id: NotRequired[str],
    frameworkId: NotRequired[str],
    frameworkName: NotRequired[str],
    frameworkDescription: NotRequired[str],
    status: NotRequired[ShareRequestStatusType],  # (1)
    sourceAccount: NotRequired[str],
    destinationAccount: NotRequired[str],
    destinationRegion: NotRequired[str],
    expirationTime: NotRequired[datetime],
    creationTime: NotRequired[datetime],
    lastUpdated: NotRequired[datetime],
    comment: NotRequired[str],
    standardControlsCount: NotRequired[int],
    customControlsCount: NotRequired[int],
    complianceType: NotRequired[str],
```

1. See [:material-code-brackets: ShareRequestStatusType](./literals.md#sharerequeststatustype) 
## FrameworkMetadataTypeDef

```python
# FrameworkMetadataTypeDef definition

class FrameworkMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    logo: NotRequired[str],
    complianceType: NotRequired[str],
```

## AssessmentReportsDestinationTypeDef

```python
# AssessmentReportsDestinationTypeDef definition

class AssessmentReportsDestinationTypeDef(TypedDict):
    destinationType: NotRequired[AssessmentReportDestinationTypeType],  # (1)
    destination: NotRequired[str],
```

1. See [:material-code-brackets: AssessmentReportDestinationTypeType](./literals.md#assessmentreportdestinationtypetype) 
## AssessmentReportEvidenceErrorTypeDef

```python
# AssessmentReportEvidenceErrorTypeDef definition

class AssessmentReportEvidenceErrorTypeDef(TypedDict):
    evidenceId: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## AssessmentReportMetadataTypeDef

```python
# AssessmentReportMetadataTypeDef definition

class AssessmentReportMetadataTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    assessmentId: NotRequired[str],
    assessmentName: NotRequired[str],
    author: NotRequired[str],
    status: NotRequired[AssessmentReportStatusType],  # (1)
    creationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AssessmentReportStatusType](./literals.md#assessmentreportstatustype) 
## AssessmentReportTypeDef

```python
# AssessmentReportTypeDef definition

class AssessmentReportTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    awsAccountId: NotRequired[str],
    assessmentId: NotRequired[str],
    assessmentName: NotRequired[str],
    author: NotRequired[str],
    status: NotRequired[AssessmentReportStatusType],  # (1)
    creationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: AssessmentReportStatusType](./literals.md#assessmentreportstatustype) 
## AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef

```python
# AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef definition

class AssociateAssessmentReportEvidenceFolderRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    evidenceFolderId: str,
```

## BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef

```python
# BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef definition

class BatchAssociateAssessmentReportEvidenceRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    evidenceFolderId: str,
    evidenceIds: Sequence[str],
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

## CreateDelegationRequestTypeDef

```python
# CreateDelegationRequestTypeDef definition

class CreateDelegationRequestTypeDef(TypedDict):
    comment: NotRequired[str],
    controlSetId: NotRequired[str],
    roleArn: NotRequired[str],
    roleType: NotRequired[RoleTypeType],  # (1)
```

1. See [:material-code-brackets: RoleTypeType](./literals.md#roletypetype) 
## BatchDeleteDelegationByAssessmentErrorTypeDef

```python
# BatchDeleteDelegationByAssessmentErrorTypeDef definition

class BatchDeleteDelegationByAssessmentErrorTypeDef(TypedDict):
    delegationId: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## BatchDeleteDelegationByAssessmentRequestRequestTypeDef

```python
# BatchDeleteDelegationByAssessmentRequestRequestTypeDef definition

class BatchDeleteDelegationByAssessmentRequestRequestTypeDef(TypedDict):
    delegationIds: Sequence[str],
    assessmentId: str,
```

## BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef

```python
# BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef definition

class BatchDisassociateAssessmentReportEvidenceRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    evidenceFolderId: str,
    evidenceIds: Sequence[str],
```

## ManualEvidenceTypeDef

```python
# ManualEvidenceTypeDef definition

class ManualEvidenceTypeDef(TypedDict):
    s3ResourcePath: NotRequired[str],
    textResponse: NotRequired[str],
    evidenceFileName: NotRequired[str],
```

## ChangeLogTypeDef

```python
# ChangeLogTypeDef definition

class ChangeLogTypeDef(TypedDict):
    objectType: NotRequired[ObjectTypeEnumType],  # (1)
    objectName: NotRequired[str],
    action: NotRequired[ActionEnumType],  # (2)
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
```

1. See [:material-code-brackets: ObjectTypeEnumType](./literals.md#objecttypeenumtype) 
2. See [:material-code-brackets: ActionEnumType](./literals.md#actionenumtype) 
## EvidenceInsightsTypeDef

```python
# EvidenceInsightsTypeDef definition

class EvidenceInsightsTypeDef(TypedDict):
    noncompliantEvidenceCount: NotRequired[int],
    compliantEvidenceCount: NotRequired[int],
    inconclusiveEvidenceCount: NotRequired[int],
```

## SourceKeywordTypeDef

```python
# SourceKeywordTypeDef definition

class SourceKeywordTypeDef(TypedDict):
    keywordInputType: NotRequired[KeywordInputTypeType],  # (1)
    keywordValue: NotRequired[str],
```

1. See [:material-code-brackets: KeywordInputTypeType](./literals.md#keywordinputtypetype) 
## ControlMetadataTypeDef

```python
# ControlMetadataTypeDef definition

class ControlMetadataTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    controlSources: NotRequired[str],
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
```

## CreateAssessmentFrameworkControlTypeDef

```python
# CreateAssessmentFrameworkControlTypeDef definition

class CreateAssessmentFrameworkControlTypeDef(TypedDict):
    id: str,
```

## CreateAssessmentReportRequestRequestTypeDef

```python
# CreateAssessmentReportRequestRequestTypeDef definition

class CreateAssessmentReportRequestRequestTypeDef(TypedDict):
    name: str,
    assessmentId: str,
    description: NotRequired[str],
    queryStatement: NotRequired[str],
```

## DefaultExportDestinationTypeDef

```python
# DefaultExportDestinationTypeDef definition

class DefaultExportDestinationTypeDef(TypedDict):
    destinationType: NotRequired[ExportDestinationTypeType],  # (1)
    destination: NotRequired[str],
```

1. See [:material-code-brackets: ExportDestinationTypeType](./literals.md#exportdestinationtypetype) 
## DelegationMetadataTypeDef

```python
# DelegationMetadataTypeDef definition

class DelegationMetadataTypeDef(TypedDict):
    id: NotRequired[str],
    assessmentName: NotRequired[str],
    assessmentId: NotRequired[str],
    status: NotRequired[DelegationStatusType],  # (1)
    roleArn: NotRequired[str],
    creationTime: NotRequired[datetime],
    controlSetName: NotRequired[str],
```

1. See [:material-code-brackets: DelegationStatusType](./literals.md#delegationstatustype) 
## DeleteAssessmentFrameworkRequestRequestTypeDef

```python
# DeleteAssessmentFrameworkRequestRequestTypeDef definition

class DeleteAssessmentFrameworkRequestRequestTypeDef(TypedDict):
    frameworkId: str,
```

## DeleteAssessmentFrameworkShareRequestRequestTypeDef

```python
# DeleteAssessmentFrameworkShareRequestRequestTypeDef definition

class DeleteAssessmentFrameworkShareRequestRequestTypeDef(TypedDict):
    requestId: str,
    requestType: ShareRequestTypeType,  # (1)
```

1. See [:material-code-brackets: ShareRequestTypeType](./literals.md#sharerequesttypetype) 
## DeleteAssessmentReportRequestRequestTypeDef

```python
# DeleteAssessmentReportRequestRequestTypeDef definition

class DeleteAssessmentReportRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    assessmentReportId: str,
```

## DeleteAssessmentRequestRequestTypeDef

```python
# DeleteAssessmentRequestRequestTypeDef definition

class DeleteAssessmentRequestRequestTypeDef(TypedDict):
    assessmentId: str,
```

## DeleteControlRequestRequestTypeDef

```python
# DeleteControlRequestRequestTypeDef definition

class DeleteControlRequestRequestTypeDef(TypedDict):
    controlId: str,
```

## DeregisterOrganizationAdminAccountRequestRequestTypeDef

```python
# DeregisterOrganizationAdminAccountRequestRequestTypeDef definition

class DeregisterOrganizationAdminAccountRequestRequestTypeDef(TypedDict):
    adminAccountId: NotRequired[str],
```

## DeregistrationPolicyTypeDef

```python
# DeregistrationPolicyTypeDef definition

class DeregistrationPolicyTypeDef(TypedDict):
    deleteResources: NotRequired[DeleteResourcesType],  # (1)
```

1. See [:material-code-brackets: DeleteResourcesType](./literals.md#deleteresourcestype) 
## DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef

```python
# DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef definition

class DisassociateAssessmentReportEvidenceFolderRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    evidenceFolderId: str,
```

## EvidenceFinderEnablementTypeDef

```python
# EvidenceFinderEnablementTypeDef definition

class EvidenceFinderEnablementTypeDef(TypedDict):
    eventDataStoreArn: NotRequired[str],
    enablementStatus: NotRequired[EvidenceFinderEnablementStatusType],  # (1)
    backfillStatus: NotRequired[EvidenceFinderBackfillStatusType],  # (2)
    error: NotRequired[str],
```

1. See [:material-code-brackets: EvidenceFinderEnablementStatusType](./literals.md#evidencefinderenablementstatustype) 
2. See [:material-code-brackets: EvidenceFinderBackfillStatusType](./literals.md#evidencefinderbackfillstatustype) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    arn: NotRequired[str],
    value: NotRequired[str],
    complianceCheck: NotRequired[str],
```

## GetAssessmentFrameworkRequestRequestTypeDef

```python
# GetAssessmentFrameworkRequestRequestTypeDef definition

class GetAssessmentFrameworkRequestRequestTypeDef(TypedDict):
    frameworkId: str,
```

## GetAssessmentReportUrlRequestRequestTypeDef

```python
# GetAssessmentReportUrlRequestRequestTypeDef definition

class GetAssessmentReportUrlRequestRequestTypeDef(TypedDict):
    assessmentReportId: str,
    assessmentId: str,
```

## URLTypeDef

```python
# URLTypeDef definition

class URLTypeDef(TypedDict):
    hyperlinkName: NotRequired[str],
    link: NotRequired[str],
```

## GetAssessmentRequestRequestTypeDef

```python
# GetAssessmentRequestRequestTypeDef definition

class GetAssessmentRequestRequestTypeDef(TypedDict):
    assessmentId: str,
```

## GetChangeLogsRequestRequestTypeDef

```python
# GetChangeLogsRequestRequestTypeDef definition

class GetChangeLogsRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    controlSetId: NotRequired[str],
    controlId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetControlRequestRequestTypeDef

```python
# GetControlRequestRequestTypeDef definition

class GetControlRequestRequestTypeDef(TypedDict):
    controlId: str,
```

## GetDelegationsRequestRequestTypeDef

```python
# GetDelegationsRequestRequestTypeDef definition

class GetDelegationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetEvidenceByEvidenceFolderRequestRequestTypeDef

```python
# GetEvidenceByEvidenceFolderRequestRequestTypeDef definition

class GetEvidenceByEvidenceFolderRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    controlSetId: str,
    evidenceFolderId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetEvidenceFileUploadUrlRequestRequestTypeDef

```python
# GetEvidenceFileUploadUrlRequestRequestTypeDef definition

class GetEvidenceFileUploadUrlRequestRequestTypeDef(TypedDict):
    fileName: str,
```

## GetEvidenceFolderRequestRequestTypeDef

```python
# GetEvidenceFolderRequestRequestTypeDef definition

class GetEvidenceFolderRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    controlSetId: str,
    evidenceFolderId: str,
```

## GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef

```python
# GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef definition

class GetEvidenceFoldersByAssessmentControlRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    controlSetId: str,
    controlId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetEvidenceFoldersByAssessmentRequestRequestTypeDef

```python
# GetEvidenceFoldersByAssessmentRequestRequestTypeDef definition

class GetEvidenceFoldersByAssessmentRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetEvidenceRequestRequestTypeDef

```python
# GetEvidenceRequestRequestTypeDef definition

class GetEvidenceRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    controlSetId: str,
    evidenceFolderId: str,
    evidenceId: str,
```

## GetInsightsByAssessmentRequestRequestTypeDef

```python
# GetInsightsByAssessmentRequestRequestTypeDef definition

class GetInsightsByAssessmentRequestRequestTypeDef(TypedDict):
    assessmentId: str,
```

## InsightsByAssessmentTypeDef

```python
# InsightsByAssessmentTypeDef definition

class InsightsByAssessmentTypeDef(TypedDict):
    noncompliantEvidenceCount: NotRequired[int],
    compliantEvidenceCount: NotRequired[int],
    inconclusiveEvidenceCount: NotRequired[int],
    assessmentControlsCountByNoncompliantEvidence: NotRequired[int],
    totalAssessmentControlsCount: NotRequired[int],
    lastUpdated: NotRequired[datetime],
```

## InsightsTypeDef

```python
# InsightsTypeDef definition

class InsightsTypeDef(TypedDict):
    activeAssessmentsCount: NotRequired[int],
    noncompliantEvidenceCount: NotRequired[int],
    compliantEvidenceCount: NotRequired[int],
    inconclusiveEvidenceCount: NotRequired[int],
    assessmentControlsCountByNoncompliantEvidence: NotRequired[int],
    totalAssessmentControlsCount: NotRequired[int],
    lastUpdated: NotRequired[datetime],
```

## ServiceMetadataTypeDef

```python
# ServiceMetadataTypeDef definition

class ServiceMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    displayName: NotRequired[str],
    description: NotRequired[str],
    category: NotRequired[str],
```

## GetSettingsRequestRequestTypeDef

```python
# GetSettingsRequestRequestTypeDef definition

class GetSettingsRequestRequestTypeDef(TypedDict):
    attribute: SettingAttributeType,  # (1)
```

1. See [:material-code-brackets: SettingAttributeType](./literals.md#settingattributetype) 
## ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef

```python
# ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef definition

class ListAssessmentControlInsightsByControlDomainRequestRequestTypeDef(TypedDict):
    controlDomainId: str,
    assessmentId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAssessmentFrameworkShareRequestsRequestRequestTypeDef

```python
# ListAssessmentFrameworkShareRequestsRequestRequestTypeDef definition

class ListAssessmentFrameworkShareRequestsRequestRequestTypeDef(TypedDict):
    requestType: ShareRequestTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ShareRequestTypeType](./literals.md#sharerequesttypetype) 
## ListAssessmentFrameworksRequestRequestTypeDef

```python
# ListAssessmentFrameworksRequestRequestTypeDef definition

class ListAssessmentFrameworksRequestRequestTypeDef(TypedDict):
    frameworkType: FrameworkTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: FrameworkTypeType](./literals.md#frameworktypetype) 
## ListAssessmentReportsRequestRequestTypeDef

```python
# ListAssessmentReportsRequestRequestTypeDef definition

class ListAssessmentReportsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListAssessmentsRequestRequestTypeDef

```python
# ListAssessmentsRequestRequestTypeDef definition

class ListAssessmentsRequestRequestTypeDef(TypedDict):
    status: NotRequired[AssessmentStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
## ListControlDomainInsightsByAssessmentRequestRequestTypeDef

```python
# ListControlDomainInsightsByAssessmentRequestRequestTypeDef definition

class ListControlDomainInsightsByAssessmentRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListControlDomainInsightsRequestRequestTypeDef

```python
# ListControlDomainInsightsRequestRequestTypeDef definition

class ListControlDomainInsightsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListControlInsightsByControlDomainRequestRequestTypeDef

```python
# ListControlInsightsByControlDomainRequestRequestTypeDef definition

class ListControlInsightsByControlDomainRequestRequestTypeDef(TypedDict):
    controlDomainId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListControlsRequestRequestTypeDef

```python
# ListControlsRequestRequestTypeDef definition

class ListControlsRequestRequestTypeDef(TypedDict):
    controlType: ControlTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    controlCatalogId: NotRequired[str],
```

1. See [:material-code-brackets: ControlTypeType](./literals.md#controltypetype) 
## ListKeywordsForDataSourceRequestRequestTypeDef

```python
# ListKeywordsForDataSourceRequestRequestTypeDef definition

class ListKeywordsForDataSourceRequestRequestTypeDef(TypedDict):
    source: DataSourceTypeType,  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
## ListNotificationsRequestRequestTypeDef

```python
# ListNotificationsRequestRequestTypeDef definition

class ListNotificationsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## NotificationTypeDef

```python
# NotificationTypeDef definition

class NotificationTypeDef(TypedDict):
    id: NotRequired[str],
    assessmentId: NotRequired[str],
    assessmentName: NotRequired[str],
    controlSetId: NotRequired[str],
    controlSetName: NotRequired[str],
    description: NotRequired[str],
    eventTime: NotRequired[datetime],
    source: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RegisterAccountRequestRequestTypeDef

```python
# RegisterAccountRequestRequestTypeDef definition

class RegisterAccountRequestRequestTypeDef(TypedDict):
    kmsKey: NotRequired[str],
    delegatedAdminAccount: NotRequired[str],
```

## RegisterOrganizationAdminAccountRequestRequestTypeDef

```python
# RegisterOrganizationAdminAccountRequestRequestTypeDef definition

class RegisterOrganizationAdminAccountRequestRequestTypeDef(TypedDict):
    adminAccountId: str,
```

## StartAssessmentFrameworkShareRequestRequestTypeDef

```python
# StartAssessmentFrameworkShareRequestRequestTypeDef definition

class StartAssessmentFrameworkShareRequestRequestTypeDef(TypedDict):
    frameworkId: str,
    destinationAccount: str,
    destinationRegion: str,
    comment: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAssessmentControlRequestRequestTypeDef

```python
# UpdateAssessmentControlRequestRequestTypeDef definition

class UpdateAssessmentControlRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    controlSetId: str,
    controlId: str,
    controlStatus: NotRequired[ControlStatusType],  # (1)
    commentBody: NotRequired[str],
```

1. See [:material-code-brackets: ControlStatusType](./literals.md#controlstatustype) 
## UpdateAssessmentControlSetStatusRequestRequestTypeDef

```python
# UpdateAssessmentControlSetStatusRequestRequestTypeDef definition

class UpdateAssessmentControlSetStatusRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    controlSetId: str,
    status: ControlSetStatusType,  # (1)
    comment: str,
```

1. See [:material-code-brackets: ControlSetStatusType](./literals.md#controlsetstatustype) 
## UpdateAssessmentFrameworkShareRequestRequestTypeDef

```python
# UpdateAssessmentFrameworkShareRequestRequestTypeDef definition

class UpdateAssessmentFrameworkShareRequestRequestTypeDef(TypedDict):
    requestId: str,
    requestType: ShareRequestTypeType,  # (1)
    action: ShareRequestActionType,  # (2)
```

1. See [:material-code-brackets: ShareRequestTypeType](./literals.md#sharerequesttypetype) 
2. See [:material-code-brackets: ShareRequestActionType](./literals.md#sharerequestactiontype) 
## UpdateAssessmentStatusRequestRequestTypeDef

```python
# UpdateAssessmentStatusRequestRequestTypeDef definition

class UpdateAssessmentStatusRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    status: AssessmentStatusType,  # (1)
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
## ValidateAssessmentReportIntegrityRequestRequestTypeDef

```python
# ValidateAssessmentReportIntegrityRequestRequestTypeDef definition

class ValidateAssessmentReportIntegrityRequestRequestTypeDef(TypedDict):
    s3RelativePath: str,
```

## ScopeOutputTypeDef

```python
# ScopeOutputTypeDef definition

class ScopeOutputTypeDef(TypedDict):
    awsAccounts: NotRequired[List[AWSAccountTypeDef]],  # (1)
    awsServices: NotRequired[List[AWSServiceTypeDef]],  # (2)
```

1. See [:material-code-braces: AWSAccountTypeDef](./type_defs.md#awsaccounttypedef) 
2. See [:material-code-braces: AWSServiceTypeDef](./type_defs.md#awsservicetypedef) 
## ScopeTypeDef

```python
# ScopeTypeDef definition

class ScopeTypeDef(TypedDict):
    awsAccounts: NotRequired[Sequence[AWSAccountTypeDef]],  # (1)
    awsServices: NotRequired[Sequence[AWSServiceTypeDef]],  # (2)
```

1. See [:material-code-braces: AWSAccountTypeDef](./type_defs.md#awsaccounttypedef) 
2. See [:material-code-braces: AWSServiceTypeDef](./type_defs.md#awsservicetypedef) 
## AssessmentMetadataItemTypeDef

```python
# AssessmentMetadataItemTypeDef definition

class AssessmentMetadataItemTypeDef(TypedDict):
    name: NotRequired[str],
    id: NotRequired[str],
    complianceType: NotRequired[str],
    status: NotRequired[AssessmentStatusType],  # (1)
    roles: NotRequired[List[RoleTypeDef]],  # (2)
    delegations: NotRequired[List[DelegationTypeDef]],  # (3)
    creationTime: NotRequired[datetime],
    lastUpdated: NotRequired[datetime],
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
3. See [:material-code-braces: DelegationTypeDef](./type_defs.md#delegationtypedef) 
## AssessmentControlTypeDef

```python
# AssessmentControlTypeDef definition

class AssessmentControlTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[ControlStatusType],  # (1)
    response: NotRequired[ControlResponseType],  # (2)
    comments: NotRequired[List[ControlCommentTypeDef]],  # (3)
    evidenceSources: NotRequired[List[str]],
    evidenceCount: NotRequired[int],
    assessmentReportEvidenceCount: NotRequired[int],
```

1. See [:material-code-brackets: ControlStatusType](./literals.md#controlstatustype) 
2. See [:material-code-brackets: ControlResponseType](./literals.md#controlresponsetype) 
3. See [:material-code-braces: ControlCommentTypeDef](./type_defs.md#controlcommenttypedef) 
## BatchAssociateAssessmentReportEvidenceResponseTypeDef

```python
# BatchAssociateAssessmentReportEvidenceResponseTypeDef definition

class BatchAssociateAssessmentReportEvidenceResponseTypeDef(TypedDict):
    evidenceIds: List[str],
    errors: List[AssessmentReportEvidenceErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentReportEvidenceErrorTypeDef](./type_defs.md#assessmentreportevidenceerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateAssessmentReportEvidenceResponseTypeDef

```python
# BatchDisassociateAssessmentReportEvidenceResponseTypeDef definition

class BatchDisassociateAssessmentReportEvidenceResponseTypeDef(TypedDict):
    evidenceIds: List[str],
    errors: List[AssessmentReportEvidenceErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentReportEvidenceErrorTypeDef](./type_defs.md#assessmentreportevidenceerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssessmentReportResponseTypeDef

```python
# CreateAssessmentReportResponseTypeDef definition

class CreateAssessmentReportResponseTypeDef(TypedDict):
    assessmentReport: AssessmentReportTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentReportTypeDef](./type_defs.md#assessmentreporttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeregisterAccountResponseTypeDef

```python
# DeregisterAccountResponseTypeDef definition

class DeregisterAccountResponseTypeDef(TypedDict):
    status: AccountStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AccountStatusType](./literals.md#accountstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccountStatusResponseTypeDef

```python
# GetAccountStatusResponseTypeDef definition

class GetAccountStatusResponseTypeDef(TypedDict):
    status: AccountStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AccountStatusType](./literals.md#accountstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEvidenceFileUploadUrlResponseTypeDef

```python
# GetEvidenceFileUploadUrlResponseTypeDef definition

class GetEvidenceFileUploadUrlResponseTypeDef(TypedDict):
    evidenceFileName: str,
    uploadUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEvidenceFolderResponseTypeDef

```python
# GetEvidenceFolderResponseTypeDef definition

class GetEvidenceFolderResponseTypeDef(TypedDict):
    evidenceFolder: AssessmentEvidenceFolderTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentEvidenceFolderTypeDef](./type_defs.md#assessmentevidencefoldertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEvidenceFoldersByAssessmentControlResponseTypeDef

```python
# GetEvidenceFoldersByAssessmentControlResponseTypeDef definition

class GetEvidenceFoldersByAssessmentControlResponseTypeDef(TypedDict):
    evidenceFolders: List[AssessmentEvidenceFolderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssessmentEvidenceFolderTypeDef](./type_defs.md#assessmentevidencefoldertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEvidenceFoldersByAssessmentResponseTypeDef

```python
# GetEvidenceFoldersByAssessmentResponseTypeDef definition

class GetEvidenceFoldersByAssessmentResponseTypeDef(TypedDict):
    evidenceFolders: List[AssessmentEvidenceFolderTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssessmentEvidenceFolderTypeDef](./type_defs.md#assessmentevidencefoldertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOrganizationAdminAccountResponseTypeDef

```python
# GetOrganizationAdminAccountResponseTypeDef definition

class GetOrganizationAdminAccountResponseTypeDef(TypedDict):
    adminAccountId: str,
    organizationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentFrameworkShareRequestsResponseTypeDef

```python
# ListAssessmentFrameworkShareRequestsResponseTypeDef definition

class ListAssessmentFrameworkShareRequestsResponseTypeDef(TypedDict):
    assessmentFrameworkShareRequests: List[AssessmentFrameworkShareRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssessmentFrameworkShareRequestTypeDef](./type_defs.md#assessmentframeworksharerequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentFrameworksResponseTypeDef

```python
# ListAssessmentFrameworksResponseTypeDef definition

class ListAssessmentFrameworksResponseTypeDef(TypedDict):
    frameworkMetadataList: List[AssessmentFrameworkMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssessmentFrameworkMetadataTypeDef](./type_defs.md#assessmentframeworkmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentReportsResponseTypeDef

```python
# ListAssessmentReportsResponseTypeDef definition

class ListAssessmentReportsResponseTypeDef(TypedDict):
    assessmentReports: List[AssessmentReportMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssessmentReportMetadataTypeDef](./type_defs.md#assessmentreportmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKeywordsForDataSourceResponseTypeDef

```python
# ListKeywordsForDataSourceResponseTypeDef definition

class ListKeywordsForDataSourceResponseTypeDef(TypedDict):
    keywords: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterAccountResponseTypeDef

```python
# RegisterAccountResponseTypeDef definition

class RegisterAccountResponseTypeDef(TypedDict):
    status: AccountStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AccountStatusType](./literals.md#accountstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RegisterOrganizationAdminAccountResponseTypeDef

```python
# RegisterOrganizationAdminAccountResponseTypeDef definition

class RegisterOrganizationAdminAccountResponseTypeDef(TypedDict):
    adminAccountId: str,
    organizationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAssessmentFrameworkShareResponseTypeDef

```python
# StartAssessmentFrameworkShareResponseTypeDef definition

class StartAssessmentFrameworkShareResponseTypeDef(TypedDict):
    assessmentFrameworkShareRequest: AssessmentFrameworkShareRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentFrameworkShareRequestTypeDef](./type_defs.md#assessmentframeworksharerequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssessmentFrameworkShareResponseTypeDef

```python
# UpdateAssessmentFrameworkShareResponseTypeDef definition

class UpdateAssessmentFrameworkShareResponseTypeDef(TypedDict):
    assessmentFrameworkShareRequest: AssessmentFrameworkShareRequestTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentFrameworkShareRequestTypeDef](./type_defs.md#assessmentframeworksharerequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ValidateAssessmentReportIntegrityResponseTypeDef

```python
# ValidateAssessmentReportIntegrityResponseTypeDef definition

class ValidateAssessmentReportIntegrityResponseTypeDef(TypedDict):
    signatureValid: bool,
    signatureAlgorithm: str,
    signatureDateTime: str,
    signatureKeyId: str,
    validationErrors: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateDelegationByAssessmentErrorTypeDef

```python
# BatchCreateDelegationByAssessmentErrorTypeDef definition

class BatchCreateDelegationByAssessmentErrorTypeDef(TypedDict):
    createDelegationRequest: NotRequired[CreateDelegationRequestTypeDef],  # (1)
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

1. See [:material-code-braces: CreateDelegationRequestTypeDef](./type_defs.md#createdelegationrequesttypedef) 
## BatchCreateDelegationByAssessmentRequestRequestTypeDef

```python
# BatchCreateDelegationByAssessmentRequestRequestTypeDef definition

class BatchCreateDelegationByAssessmentRequestRequestTypeDef(TypedDict):
    createDelegationRequests: Sequence[CreateDelegationRequestTypeDef],  # (1)
    assessmentId: str,
```

1. See [:material-code-braces: CreateDelegationRequestTypeDef](./type_defs.md#createdelegationrequesttypedef) 
## BatchDeleteDelegationByAssessmentResponseTypeDef

```python
# BatchDeleteDelegationByAssessmentResponseTypeDef definition

class BatchDeleteDelegationByAssessmentResponseTypeDef(TypedDict):
    errors: List[BatchDeleteDelegationByAssessmentErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteDelegationByAssessmentErrorTypeDef](./type_defs.md#batchdeletedelegationbyassessmenterrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchImportEvidenceToAssessmentControlErrorTypeDef

```python
# BatchImportEvidenceToAssessmentControlErrorTypeDef definition

class BatchImportEvidenceToAssessmentControlErrorTypeDef(TypedDict):
    manualEvidence: NotRequired[ManualEvidenceTypeDef],  # (1)
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

1. See [:material-code-braces: ManualEvidenceTypeDef](./type_defs.md#manualevidencetypedef) 
## BatchImportEvidenceToAssessmentControlRequestRequestTypeDef

```python
# BatchImportEvidenceToAssessmentControlRequestRequestTypeDef definition

class BatchImportEvidenceToAssessmentControlRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    controlSetId: str,
    controlId: str,
    manualEvidence: Sequence[ManualEvidenceTypeDef],  # (1)
```

1. See [:material-code-braces: ManualEvidenceTypeDef](./type_defs.md#manualevidencetypedef) 
## GetChangeLogsResponseTypeDef

```python
# GetChangeLogsResponseTypeDef definition

class GetChangeLogsResponseTypeDef(TypedDict):
    changeLogs: List[ChangeLogTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ChangeLogTypeDef](./type_defs.md#changelogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ControlDomainInsightsTypeDef

```python
# ControlDomainInsightsTypeDef definition

class ControlDomainInsightsTypeDef(TypedDict):
    name: NotRequired[str],
    id: NotRequired[str],
    controlsCountByNoncompliantEvidence: NotRequired[int],
    totalControlsCount: NotRequired[int],
    evidenceInsights: NotRequired[EvidenceInsightsTypeDef],  # (1)
    lastUpdated: NotRequired[datetime],
```

1. See [:material-code-braces: EvidenceInsightsTypeDef](./type_defs.md#evidenceinsightstypedef) 
## ControlInsightsMetadataByAssessmentItemTypeDef

```python
# ControlInsightsMetadataByAssessmentItemTypeDef definition

class ControlInsightsMetadataByAssessmentItemTypeDef(TypedDict):
    name: NotRequired[str],
    id: NotRequired[str],
    evidenceInsights: NotRequired[EvidenceInsightsTypeDef],  # (1)
    controlSetName: NotRequired[str],
    lastUpdated: NotRequired[datetime],
```

1. See [:material-code-braces: EvidenceInsightsTypeDef](./type_defs.md#evidenceinsightstypedef) 
## ControlInsightsMetadataItemTypeDef

```python
# ControlInsightsMetadataItemTypeDef definition

class ControlInsightsMetadataItemTypeDef(TypedDict):
    name: NotRequired[str],
    id: NotRequired[str],
    evidenceInsights: NotRequired[EvidenceInsightsTypeDef],  # (1)
    lastUpdated: NotRequired[datetime],
```

1. See [:material-code-braces: EvidenceInsightsTypeDef](./type_defs.md#evidenceinsightstypedef) 
## ControlMappingSourceTypeDef

```python
# ControlMappingSourceTypeDef definition

class ControlMappingSourceTypeDef(TypedDict):
    sourceId: NotRequired[str],
    sourceName: NotRequired[str],
    sourceDescription: NotRequired[str],
    sourceSetUpOption: NotRequired[SourceSetUpOptionType],  # (1)
    sourceType: NotRequired[SourceTypeType],  # (2)
    sourceKeyword: NotRequired[SourceKeywordTypeDef],  # (3)
    sourceFrequency: NotRequired[SourceFrequencyType],  # (4)
    troubleshootingText: NotRequired[str],
```

1. See [:material-code-brackets: SourceSetUpOptionType](./literals.md#sourcesetupoptiontype) 
2. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
3. See [:material-code-braces: SourceKeywordTypeDef](./type_defs.md#sourcekeywordtypedef) 
4. See [:material-code-brackets: SourceFrequencyType](./literals.md#sourcefrequencytype) 
## CreateControlMappingSourceTypeDef

```python
# CreateControlMappingSourceTypeDef definition

class CreateControlMappingSourceTypeDef(TypedDict):
    sourceName: NotRequired[str],
    sourceDescription: NotRequired[str],
    sourceSetUpOption: NotRequired[SourceSetUpOptionType],  # (1)
    sourceType: NotRequired[SourceTypeType],  # (2)
    sourceKeyword: NotRequired[SourceKeywordTypeDef],  # (3)
    sourceFrequency: NotRequired[SourceFrequencyType],  # (4)
    troubleshootingText: NotRequired[str],
```

1. See [:material-code-brackets: SourceSetUpOptionType](./literals.md#sourcesetupoptiontype) 
2. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
3. See [:material-code-braces: SourceKeywordTypeDef](./type_defs.md#sourcekeywordtypedef) 
4. See [:material-code-brackets: SourceFrequencyType](./literals.md#sourcefrequencytype) 
## ListControlsResponseTypeDef

```python
# ListControlsResponseTypeDef definition

class ListControlsResponseTypeDef(TypedDict):
    controlMetadataList: List[ControlMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlMetadataTypeDef](./type_defs.md#controlmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssessmentFrameworkControlSetTypeDef

```python
# CreateAssessmentFrameworkControlSetTypeDef definition

class CreateAssessmentFrameworkControlSetTypeDef(TypedDict):
    name: str,
    controls: NotRequired[Sequence[CreateAssessmentFrameworkControlTypeDef]],  # (1)
```

1. See [:material-code-braces: CreateAssessmentFrameworkControlTypeDef](./type_defs.md#createassessmentframeworkcontroltypedef) 
## UpdateAssessmentFrameworkControlSetTypeDef

```python
# UpdateAssessmentFrameworkControlSetTypeDef definition

class UpdateAssessmentFrameworkControlSetTypeDef(TypedDict):
    name: str,
    controls: Sequence[CreateAssessmentFrameworkControlTypeDef],  # (1)
    id: NotRequired[str],
```

1. See [:material-code-braces: CreateAssessmentFrameworkControlTypeDef](./type_defs.md#createassessmentframeworkcontroltypedef) 
## GetDelegationsResponseTypeDef

```python
# GetDelegationsResponseTypeDef definition

class GetDelegationsResponseTypeDef(TypedDict):
    delegations: List[DelegationMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DelegationMetadataTypeDef](./type_defs.md#delegationmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSettingsRequestRequestTypeDef

```python
# UpdateSettingsRequestRequestTypeDef definition

class UpdateSettingsRequestRequestTypeDef(TypedDict):
    snsTopic: NotRequired[str],
    defaultAssessmentReportsDestination: NotRequired[AssessmentReportsDestinationTypeDef],  # (1)
    defaultProcessOwners: NotRequired[Sequence[RoleTypeDef]],  # (2)
    kmsKey: NotRequired[str],
    evidenceFinderEnabled: NotRequired[bool],
    deregistrationPolicy: NotRequired[DeregistrationPolicyTypeDef],  # (3)
    defaultExportDestination: NotRequired[DefaultExportDestinationTypeDef],  # (4)
```

1. See [:material-code-braces: AssessmentReportsDestinationTypeDef](./type_defs.md#assessmentreportsdestinationtypedef) 
2. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
3. See [:material-code-braces: DeregistrationPolicyTypeDef](./type_defs.md#deregistrationpolicytypedef) 
4. See [:material-code-braces: DefaultExportDestinationTypeDef](./type_defs.md#defaultexportdestinationtypedef) 
## SettingsTypeDef

```python
# SettingsTypeDef definition

class SettingsTypeDef(TypedDict):
    isAwsOrgEnabled: NotRequired[bool],
    snsTopic: NotRequired[str],
    defaultAssessmentReportsDestination: NotRequired[AssessmentReportsDestinationTypeDef],  # (1)
    defaultProcessOwners: NotRequired[List[RoleTypeDef]],  # (2)
    kmsKey: NotRequired[str],
    evidenceFinderEnablement: NotRequired[EvidenceFinderEnablementTypeDef],  # (3)
    deregistrationPolicy: NotRequired[DeregistrationPolicyTypeDef],  # (4)
    defaultExportDestination: NotRequired[DefaultExportDestinationTypeDef],  # (5)
```

1. See [:material-code-braces: AssessmentReportsDestinationTypeDef](./type_defs.md#assessmentreportsdestinationtypedef) 
2. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
3. See [:material-code-braces: EvidenceFinderEnablementTypeDef](./type_defs.md#evidencefinderenablementtypedef) 
4. See [:material-code-braces: DeregistrationPolicyTypeDef](./type_defs.md#deregistrationpolicytypedef) 
5. See [:material-code-braces: DefaultExportDestinationTypeDef](./type_defs.md#defaultexportdestinationtypedef) 
## EvidenceTypeDef

```python
# EvidenceTypeDef definition

class EvidenceTypeDef(TypedDict):
    dataSource: NotRequired[str],
    evidenceAwsAccountId: NotRequired[str],
    time: NotRequired[datetime],
    eventSource: NotRequired[str],
    eventName: NotRequired[str],
    evidenceByType: NotRequired[str],
    resourcesIncluded: NotRequired[List[ResourceTypeDef]],  # (1)
    attributes: NotRequired[Dict[str, str]],
    iamId: NotRequired[str],
    complianceCheck: NotRequired[str],
    awsOrganization: NotRequired[str],
    awsAccountId: NotRequired[str],
    evidenceFolderId: NotRequired[str],
    id: NotRequired[str],
    assessmentReportSelection: NotRequired[str],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## GetAssessmentReportUrlResponseTypeDef

```python
# GetAssessmentReportUrlResponseTypeDef definition

class GetAssessmentReportUrlResponseTypeDef(TypedDict):
    preSignedUrl: URLTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: URLTypeDef](./type_defs.md#urltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInsightsByAssessmentResponseTypeDef

```python
# GetInsightsByAssessmentResponseTypeDef definition

class GetInsightsByAssessmentResponseTypeDef(TypedDict):
    insights: InsightsByAssessmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightsByAssessmentTypeDef](./type_defs.md#insightsbyassessmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetInsightsResponseTypeDef

```python
# GetInsightsResponseTypeDef definition

class GetInsightsResponseTypeDef(TypedDict):
    insights: InsightsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: InsightsTypeDef](./type_defs.md#insightstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServicesInScopeResponseTypeDef

```python
# GetServicesInScopeResponseTypeDef definition

class GetServicesInScopeResponseTypeDef(TypedDict):
    serviceMetadata: List[ServiceMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceMetadataTypeDef](./type_defs.md#servicemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNotificationsResponseTypeDef

```python
# ListNotificationsResponseTypeDef definition

class ListNotificationsResponseTypeDef(TypedDict):
    notifications: List[NotificationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationTypeDef](./type_defs.md#notificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssessmentMetadataTypeDef

```python
# AssessmentMetadataTypeDef definition

class AssessmentMetadataTypeDef(TypedDict):
    name: NotRequired[str],
    id: NotRequired[str],
    description: NotRequired[str],
    complianceType: NotRequired[str],
    status: NotRequired[AssessmentStatusType],  # (1)
    assessmentReportsDestination: NotRequired[AssessmentReportsDestinationTypeDef],  # (2)
    scope: NotRequired[ScopeOutputTypeDef],  # (3)
    roles: NotRequired[List[RoleTypeDef]],  # (4)
    delegations: NotRequired[List[DelegationTypeDef]],  # (5)
    creationTime: NotRequired[datetime],
    lastUpdated: NotRequired[datetime],
```

1. See [:material-code-brackets: AssessmentStatusType](./literals.md#assessmentstatustype) 
2. See [:material-code-braces: AssessmentReportsDestinationTypeDef](./type_defs.md#assessmentreportsdestinationtypedef) 
3. See [:material-code-braces: ScopeOutputTypeDef](./type_defs.md#scopeoutputtypedef) 
4. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
5. See [:material-code-braces: DelegationTypeDef](./type_defs.md#delegationtypedef) 
## CreateAssessmentRequestRequestTypeDef

```python
# CreateAssessmentRequestRequestTypeDef definition

class CreateAssessmentRequestRequestTypeDef(TypedDict):
    name: str,
    assessmentReportsDestination: AssessmentReportsDestinationTypeDef,  # (1)
    scope: ScopeTypeDef,  # (2)
    roles: Sequence[RoleTypeDef],  # (3)
    frameworkId: str,
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AssessmentReportsDestinationTypeDef](./type_defs.md#assessmentreportsdestinationtypedef) 
2. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
3. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
## UpdateAssessmentRequestRequestTypeDef

```python
# UpdateAssessmentRequestRequestTypeDef definition

class UpdateAssessmentRequestRequestTypeDef(TypedDict):
    assessmentId: str,
    scope: ScopeTypeDef,  # (1)
    assessmentName: NotRequired[str],
    assessmentDescription: NotRequired[str],
    assessmentReportsDestination: NotRequired[AssessmentReportsDestinationTypeDef],  # (2)
    roles: NotRequired[Sequence[RoleTypeDef]],  # (3)
```

1. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
2. See [:material-code-braces: AssessmentReportsDestinationTypeDef](./type_defs.md#assessmentreportsdestinationtypedef) 
3. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
## ListAssessmentsResponseTypeDef

```python
# ListAssessmentsResponseTypeDef definition

class ListAssessmentsResponseTypeDef(TypedDict):
    assessmentMetadata: List[AssessmentMetadataItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssessmentMetadataItemTypeDef](./type_defs.md#assessmentmetadataitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssessmentControlSetTypeDef

```python
# AssessmentControlSetTypeDef definition

class AssessmentControlSetTypeDef(TypedDict):
    id: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[ControlSetStatusType],  # (1)
    roles: NotRequired[List[RoleTypeDef]],  # (2)
    controls: NotRequired[List[AssessmentControlTypeDef]],  # (3)
    delegations: NotRequired[List[DelegationTypeDef]],  # (4)
    systemEvidenceCount: NotRequired[int],
    manualEvidenceCount: NotRequired[int],
```

1. See [:material-code-brackets: ControlSetStatusType](./literals.md#controlsetstatustype) 
2. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
3. See [:material-code-braces: AssessmentControlTypeDef](./type_defs.md#assessmentcontroltypedef) 
4. See [:material-code-braces: DelegationTypeDef](./type_defs.md#delegationtypedef) 
## UpdateAssessmentControlResponseTypeDef

```python
# UpdateAssessmentControlResponseTypeDef definition

class UpdateAssessmentControlResponseTypeDef(TypedDict):
    control: AssessmentControlTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentControlTypeDef](./type_defs.md#assessmentcontroltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchCreateDelegationByAssessmentResponseTypeDef

```python
# BatchCreateDelegationByAssessmentResponseTypeDef definition

class BatchCreateDelegationByAssessmentResponseTypeDef(TypedDict):
    delegations: List[DelegationTypeDef],  # (1)
    errors: List[BatchCreateDelegationByAssessmentErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: DelegationTypeDef](./type_defs.md#delegationtypedef) 
2. See [:material-code-braces: BatchCreateDelegationByAssessmentErrorTypeDef](./type_defs.md#batchcreatedelegationbyassessmenterrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchImportEvidenceToAssessmentControlResponseTypeDef

```python
# BatchImportEvidenceToAssessmentControlResponseTypeDef definition

class BatchImportEvidenceToAssessmentControlResponseTypeDef(TypedDict):
    errors: List[BatchImportEvidenceToAssessmentControlErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchImportEvidenceToAssessmentControlErrorTypeDef](./type_defs.md#batchimportevidencetoassessmentcontrolerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListControlDomainInsightsByAssessmentResponseTypeDef

```python
# ListControlDomainInsightsByAssessmentResponseTypeDef definition

class ListControlDomainInsightsByAssessmentResponseTypeDef(TypedDict):
    controlDomainInsights: List[ControlDomainInsightsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlDomainInsightsTypeDef](./type_defs.md#controldomaininsightstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListControlDomainInsightsResponseTypeDef

```python
# ListControlDomainInsightsResponseTypeDef definition

class ListControlDomainInsightsResponseTypeDef(TypedDict):
    controlDomainInsights: List[ControlDomainInsightsTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlDomainInsightsTypeDef](./type_defs.md#controldomaininsightstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssessmentControlInsightsByControlDomainResponseTypeDef

```python
# ListAssessmentControlInsightsByControlDomainResponseTypeDef definition

class ListAssessmentControlInsightsByControlDomainResponseTypeDef(TypedDict):
    controlInsightsByAssessment: List[ControlInsightsMetadataByAssessmentItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlInsightsMetadataByAssessmentItemTypeDef](./type_defs.md#controlinsightsmetadatabyassessmentitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListControlInsightsByControlDomainResponseTypeDef

```python
# ListControlInsightsByControlDomainResponseTypeDef definition

class ListControlInsightsByControlDomainResponseTypeDef(TypedDict):
    controlInsightsMetadata: List[ControlInsightsMetadataItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ControlInsightsMetadataItemTypeDef](./type_defs.md#controlinsightsmetadataitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ControlTypeDef

```python
# ControlTypeDef definition

class ControlTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    type: NotRequired[ControlTypeType],  # (1)
    name: NotRequired[str],
    description: NotRequired[str],
    testingInformation: NotRequired[str],
    actionPlanTitle: NotRequired[str],
    actionPlanInstructions: NotRequired[str],
    controlSources: NotRequired[str],
    controlMappingSources: NotRequired[List[ControlMappingSourceTypeDef]],  # (2)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    lastUpdatedBy: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
    state: NotRequired[ControlStateType],  # (3)
```

1. See [:material-code-brackets: ControlTypeType](./literals.md#controltypetype) 
2. See [:material-code-braces: ControlMappingSourceTypeDef](./type_defs.md#controlmappingsourcetypedef) 
3. See [:material-code-brackets: ControlStateType](./literals.md#controlstatetype) 
## UpdateControlRequestRequestTypeDef

```python
# UpdateControlRequestRequestTypeDef definition

class UpdateControlRequestRequestTypeDef(TypedDict):
    controlId: str,
    name: str,
    controlMappingSources: Sequence[ControlMappingSourceTypeDef],  # (1)
    description: NotRequired[str],
    testingInformation: NotRequired[str],
    actionPlanTitle: NotRequired[str],
    actionPlanInstructions: NotRequired[str],
```

1. See [:material-code-braces: ControlMappingSourceTypeDef](./type_defs.md#controlmappingsourcetypedef) 
## CreateControlRequestRequestTypeDef

```python
# CreateControlRequestRequestTypeDef definition

class CreateControlRequestRequestTypeDef(TypedDict):
    name: str,
    controlMappingSources: Sequence[CreateControlMappingSourceTypeDef],  # (1)
    description: NotRequired[str],
    testingInformation: NotRequired[str],
    actionPlanTitle: NotRequired[str],
    actionPlanInstructions: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CreateControlMappingSourceTypeDef](./type_defs.md#createcontrolmappingsourcetypedef) 
## CreateAssessmentFrameworkRequestRequestTypeDef

```python
# CreateAssessmentFrameworkRequestRequestTypeDef definition

class CreateAssessmentFrameworkRequestRequestTypeDef(TypedDict):
    name: str,
    controlSets: Sequence[CreateAssessmentFrameworkControlSetTypeDef],  # (1)
    description: NotRequired[str],
    complianceType: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CreateAssessmentFrameworkControlSetTypeDef](./type_defs.md#createassessmentframeworkcontrolsettypedef) 
## UpdateAssessmentFrameworkRequestRequestTypeDef

```python
# UpdateAssessmentFrameworkRequestRequestTypeDef definition

class UpdateAssessmentFrameworkRequestRequestTypeDef(TypedDict):
    frameworkId: str,
    name: str,
    controlSets: Sequence[UpdateAssessmentFrameworkControlSetTypeDef],  # (1)
    description: NotRequired[str],
    complianceType: NotRequired[str],
```

1. See [:material-code-braces: UpdateAssessmentFrameworkControlSetTypeDef](./type_defs.md#updateassessmentframeworkcontrolsettypedef) 
## GetSettingsResponseTypeDef

```python
# GetSettingsResponseTypeDef definition

class GetSettingsResponseTypeDef(TypedDict):
    settings: SettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateSettingsResponseTypeDef

```python
# UpdateSettingsResponseTypeDef definition

class UpdateSettingsResponseTypeDef(TypedDict):
    settings: SettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SettingsTypeDef](./type_defs.md#settingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEvidenceByEvidenceFolderResponseTypeDef

```python
# GetEvidenceByEvidenceFolderResponseTypeDef definition

class GetEvidenceByEvidenceFolderResponseTypeDef(TypedDict):
    evidence: List[EvidenceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EvidenceTypeDef](./type_defs.md#evidencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEvidenceResponseTypeDef

```python
# GetEvidenceResponseTypeDef definition

class GetEvidenceResponseTypeDef(TypedDict):
    evidence: EvidenceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvidenceTypeDef](./type_defs.md#evidencetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssessmentFrameworkTypeDef

```python
# AssessmentFrameworkTypeDef definition

class AssessmentFrameworkTypeDef(TypedDict):
    id: NotRequired[str],
    arn: NotRequired[str],
    metadata: NotRequired[FrameworkMetadataTypeDef],  # (1)
    controlSets: NotRequired[List[AssessmentControlSetTypeDef]],  # (2)
```

1. See [:material-code-braces: FrameworkMetadataTypeDef](./type_defs.md#frameworkmetadatatypedef) 
2. See [:material-code-braces: AssessmentControlSetTypeDef](./type_defs.md#assessmentcontrolsettypedef) 
## UpdateAssessmentControlSetStatusResponseTypeDef

```python
# UpdateAssessmentControlSetStatusResponseTypeDef definition

class UpdateAssessmentControlSetStatusResponseTypeDef(TypedDict):
    controlSet: AssessmentControlSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentControlSetTypeDef](./type_defs.md#assessmentcontrolsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ControlSetTypeDef

```python
# ControlSetTypeDef definition

class ControlSetTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
    controls: NotRequired[List[ControlTypeDef]],  # (1)
```

1. See [:material-code-braces: ControlTypeDef](./type_defs.md#controltypedef) 
## CreateControlResponseTypeDef

```python
# CreateControlResponseTypeDef definition

class CreateControlResponseTypeDef(TypedDict):
    control: ControlTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ControlTypeDef](./type_defs.md#controltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetControlResponseTypeDef

```python
# GetControlResponseTypeDef definition

class GetControlResponseTypeDef(TypedDict):
    control: ControlTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ControlTypeDef](./type_defs.md#controltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateControlResponseTypeDef

```python
# UpdateControlResponseTypeDef definition

class UpdateControlResponseTypeDef(TypedDict):
    control: ControlTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ControlTypeDef](./type_defs.md#controltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssessmentTypeDef

```python
# AssessmentTypeDef definition

class AssessmentTypeDef(TypedDict):
    arn: NotRequired[str],
    awsAccount: NotRequired[AWSAccountTypeDef],  # (1)
    metadata: NotRequired[AssessmentMetadataTypeDef],  # (2)
    framework: NotRequired[AssessmentFrameworkTypeDef],  # (3)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AWSAccountTypeDef](./type_defs.md#awsaccounttypedef) 
2. See [:material-code-braces: AssessmentMetadataTypeDef](./type_defs.md#assessmentmetadatatypedef) 
3. See [:material-code-braces: AssessmentFrameworkTypeDef](./type_defs.md#assessmentframeworktypedef) 
## FrameworkTypeDef

```python
# FrameworkTypeDef definition

class FrameworkTypeDef(TypedDict):
    arn: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    type: NotRequired[FrameworkTypeType],  # (1)
    complianceType: NotRequired[str],
    description: NotRequired[str],
    logo: NotRequired[str],
    controlSources: NotRequired[str],
    controlSets: NotRequired[List[ControlSetTypeDef]],  # (2)
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    lastUpdatedBy: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FrameworkTypeType](./literals.md#frameworktypetype) 
2. See [:material-code-braces: ControlSetTypeDef](./type_defs.md#controlsettypedef) 
## CreateAssessmentResponseTypeDef

```python
# CreateAssessmentResponseTypeDef definition

class CreateAssessmentResponseTypeDef(TypedDict):
    assessment: AssessmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentTypeDef](./type_defs.md#assessmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssessmentResponseTypeDef

```python
# GetAssessmentResponseTypeDef definition

class GetAssessmentResponseTypeDef(TypedDict):
    assessment: AssessmentTypeDef,  # (1)
    userRole: RoleTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssessmentTypeDef](./type_defs.md#assessmenttypedef) 
2. See [:material-code-braces: RoleTypeDef](./type_defs.md#roletypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssessmentResponseTypeDef

```python
# UpdateAssessmentResponseTypeDef definition

class UpdateAssessmentResponseTypeDef(TypedDict):
    assessment: AssessmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentTypeDef](./type_defs.md#assessmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssessmentStatusResponseTypeDef

```python
# UpdateAssessmentStatusResponseTypeDef definition

class UpdateAssessmentStatusResponseTypeDef(TypedDict):
    assessment: AssessmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssessmentTypeDef](./type_defs.md#assessmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssessmentFrameworkResponseTypeDef

```python
# CreateAssessmentFrameworkResponseTypeDef definition

class CreateAssessmentFrameworkResponseTypeDef(TypedDict):
    framework: FrameworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FrameworkTypeDef](./type_defs.md#frameworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssessmentFrameworkResponseTypeDef

```python
# GetAssessmentFrameworkResponseTypeDef definition

class GetAssessmentFrameworkResponseTypeDef(TypedDict):
    framework: FrameworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FrameworkTypeDef](./type_defs.md#frameworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssessmentFrameworkResponseTypeDef

```python
# UpdateAssessmentFrameworkResponseTypeDef definition

class UpdateAssessmentFrameworkResponseTypeDef(TypedDict):
    framework: FrameworkTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FrameworkTypeDef](./type_defs.md#frameworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

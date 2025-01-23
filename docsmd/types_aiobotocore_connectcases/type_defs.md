# Type definitions

> [Index](../README.md) > [ConnectCases](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#connectcases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## FieldValueUnionUnionTypeDef

```python
# FieldValueUnionUnionTypeDef definition

FieldValueUnionUnionTypeDef = Union[
    FieldValueUnionTypeDef,  # (1)
    FieldValueUnionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef) 
2. See [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 

## CaseEventIncludedDataUnionTypeDef

```python
# CaseEventIncludedDataUnionTypeDef definition

CaseEventIncludedDataUnionTypeDef = Union[
    CaseEventIncludedDataTypeDef,  # (1)
    CaseEventIncludedDataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CaseEventIncludedDataTypeDef](./type_defs.md#caseeventincludeddatatypedef) 
2. See [:material-code-braces: CaseEventIncludedDataOutputTypeDef](./type_defs.md#caseeventincludeddataoutputtypedef) 

## FieldGroupUnionTypeDef

```python
# FieldGroupUnionTypeDef definition

FieldGroupUnionTypeDef = Union[
    FieldGroupTypeDef,  # (1)
    FieldGroupOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldGroupTypeDef](./type_defs.md#fieldgrouptypedef) 
2. See [:material-code-braces: FieldGroupOutputTypeDef](./type_defs.md#fieldgroupoutputtypedef) 

## FieldValueExtraUnionTypeDef

```python
# FieldValueExtraUnionTypeDef definition

FieldValueExtraUnionTypeDef = Union[
    FieldValueTypeDef,  # (1)
    FieldValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
2. See [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 

## EventIncludedDataUnionTypeDef

```python
# EventIncludedDataUnionTypeDef definition

EventIncludedDataUnionTypeDef = Union[
    EventIncludedDataTypeDef,  # (1)
    EventIncludedDataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventIncludedDataTypeDef](./type_defs.md#eventincludeddatatypedef) 
2. See [:material-code-braces: EventIncludedDataOutputTypeDef](./type_defs.md#eventincludeddataoutputtypedef) 

## SectionUnionTypeDef

```python
# SectionUnionTypeDef definition

SectionUnionTypeDef = Union[
    SectionTypeDef,  # (1)
    SectionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SectionTypeDef](./type_defs.md#sectiontypedef) 
2. See [:material-code-braces: SectionOutputTypeDef](./type_defs.md#sectionoutputtypedef) 

## LayoutSectionsUnionTypeDef

```python
# LayoutSectionsUnionTypeDef definition

LayoutSectionsUnionTypeDef = Union[
    LayoutSectionsTypeDef,  # (1)
    LayoutSectionsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef) 
2. See [:material-code-braces: LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef) 

## BasicLayoutUnionTypeDef

```python
# BasicLayoutUnionTypeDef definition

BasicLayoutUnionTypeDef = Union[
    BasicLayoutTypeDef,  # (1)
    BasicLayoutOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BasicLayoutTypeDef](./type_defs.md#basiclayouttypedef) 
2. See [:material-code-braces: BasicLayoutOutputTypeDef](./type_defs.md#basiclayoutoutputtypedef) 



## AuditEventFieldValueUnionTypeDef

```python
# AuditEventFieldValueUnionTypeDef definition

class AuditEventFieldValueUnionTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    emptyValue: NotRequired[Dict[str, Any]],
    stringValue: NotRequired[str],
    userArnValue: NotRequired[str],
```

## UserUnionTypeDef

```python
# UserUnionTypeDef definition

class UserUnionTypeDef(TypedDict):
    userArn: NotRequired[str],
```

## FieldIdentifierTypeDef

```python
# FieldIdentifierTypeDef definition

class FieldIdentifierTypeDef(TypedDict):
    id: str,
```

## FieldErrorTypeDef

```python
# FieldErrorTypeDef definition

class FieldErrorTypeDef(TypedDict):
    errorCode: str,
    id: str,
    message: NotRequired[str],
```

## GetFieldResponseTypeDef

```python
# GetFieldResponseTypeDef definition

class GetFieldResponseTypeDef(TypedDict):
    fieldArn: str,
    fieldId: str,
    name: str,
    namespace: FieldNamespaceType,  # (1)
    type: FieldTypeType,  # (2)
    createdTime: NotRequired[datetime],
    deleted: NotRequired[bool],
    description: NotRequired[str],
    lastModifiedTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FieldNamespaceType](./literals.md#fieldnamespacetype) 
2. See [:material-code-brackets: FieldTypeType](./literals.md#fieldtypetype) 
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

## FieldOptionTypeDef

```python
# FieldOptionTypeDef definition

class FieldOptionTypeDef(TypedDict):
    active: bool,
    name: str,
    value: str,
```

## FieldOptionErrorTypeDef

```python
# FieldOptionErrorTypeDef definition

class FieldOptionErrorTypeDef(TypedDict):
    errorCode: str,
    message: str,
    value: str,
```

## CaseSummaryTypeDef

```python
# CaseSummaryTypeDef definition

class CaseSummaryTypeDef(TypedDict):
    caseId: str,
    templateId: str,
```

## CommentContentTypeDef

```python
# CommentContentTypeDef definition

class CommentContentTypeDef(TypedDict):
    body: str,
    contentType: CommentBodyTextTypeType,  # (1)
```

1. See [:material-code-brackets: CommentBodyTextTypeType](./literals.md#commentbodytexttypetype) 
## ContactContentTypeDef

```python
# ContactContentTypeDef definition

class ContactContentTypeDef(TypedDict):
    channel: str,
    connectedToSystemTime: datetime,
    contactArn: str,
```

## ContactFilterTypeDef

```python
# ContactFilterTypeDef definition

class ContactFilterTypeDef(TypedDict):
    channel: NotRequired[Sequence[str]],
    contactArn: NotRequired[str],
```

## ContactTypeDef

```python
# ContactTypeDef definition

class ContactTypeDef(TypedDict):
    contactArn: str,
```

## CreateDomainRequestRequestTypeDef

```python
# CreateDomainRequestRequestTypeDef definition

class CreateDomainRequestRequestTypeDef(TypedDict):
    name: str,
```

## CreateFieldRequestRequestTypeDef

```python
# CreateFieldRequestRequestTypeDef definition

class CreateFieldRequestRequestTypeDef(TypedDict):
    domainId: str,
    name: str,
    type: FieldTypeType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: FieldTypeType](./literals.md#fieldtypetype) 
## LayoutConfigurationTypeDef

```python
# LayoutConfigurationTypeDef definition

class LayoutConfigurationTypeDef(TypedDict):
    defaultLayout: NotRequired[str],
```

## RequiredFieldTypeDef

```python
# RequiredFieldTypeDef definition

class RequiredFieldTypeDef(TypedDict):
    fieldId: str,
```

## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    domainId: str,
```

## DeleteFieldRequestRequestTypeDef

```python
# DeleteFieldRequestRequestTypeDef definition

class DeleteFieldRequestRequestTypeDef(TypedDict):
    domainId: str,
    fieldId: str,
```

## DeleteLayoutRequestRequestTypeDef

```python
# DeleteLayoutRequestRequestTypeDef definition

class DeleteLayoutRequestRequestTypeDef(TypedDict):
    domainId: str,
    layoutId: str,
```

## DeleteTemplateRequestRequestTypeDef

```python
# DeleteTemplateRequestRequestTypeDef definition

class DeleteTemplateRequestRequestTypeDef(TypedDict):
    domainId: str,
    templateId: str,
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    domainArn: str,
    domainId: str,
    name: str,
```

## RelatedItemEventIncludedDataTypeDef

```python
# RelatedItemEventIncludedDataTypeDef definition

class RelatedItemEventIncludedDataTypeDef(TypedDict):
    includeContent: bool,
```

## FieldItemTypeDef

```python
# FieldItemTypeDef definition

class FieldItemTypeDef(TypedDict):
    id: str,
```

## FieldSummaryTypeDef

```python
# FieldSummaryTypeDef definition

class FieldSummaryTypeDef(TypedDict):
    fieldArn: str,
    fieldId: str,
    name: str,
    namespace: FieldNamespaceType,  # (1)
    type: FieldTypeType,  # (2)
```

1. See [:material-code-brackets: FieldNamespaceType](./literals.md#fieldnamespacetype) 
2. See [:material-code-brackets: FieldTypeType](./literals.md#fieldtypetype) 
## FieldValueUnionOutputTypeDef

```python
# FieldValueUnionOutputTypeDef definition

class FieldValueUnionOutputTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    emptyValue: NotRequired[Dict[str, Any]],
    stringValue: NotRequired[str],
    userArnValue: NotRequired[str],
```

## FieldValueUnionTypeDef

```python
# FieldValueUnionTypeDef definition

class FieldValueUnionTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    emptyValue: NotRequired[Mapping[str, Any]],
    stringValue: NotRequired[str],
    userArnValue: NotRequired[str],
```

## FileContentTypeDef

```python
# FileContentTypeDef definition

class FileContentTypeDef(TypedDict):
    fileArn: str,
```

## FileFilterTypeDef

```python
# FileFilterTypeDef definition

class FileFilterTypeDef(TypedDict):
    fileArn: NotRequired[str],
```

## GetCaseAuditEventsRequestRequestTypeDef

```python
# GetCaseAuditEventsRequestRequestTypeDef definition

class GetCaseAuditEventsRequestRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetCaseEventConfigurationRequestRequestTypeDef

```python
# GetCaseEventConfigurationRequestRequestTypeDef definition

class GetCaseEventConfigurationRequestRequestTypeDef(TypedDict):
    domainId: str,
```

## GetDomainRequestRequestTypeDef

```python
# GetDomainRequestRequestTypeDef definition

class GetDomainRequestRequestTypeDef(TypedDict):
    domainId: str,
```

## GetLayoutRequestRequestTypeDef

```python
# GetLayoutRequestRequestTypeDef definition

class GetLayoutRequestRequestTypeDef(TypedDict):
    domainId: str,
    layoutId: str,
```

## GetTemplateRequestRequestTypeDef

```python
# GetTemplateRequestRequestTypeDef definition

class GetTemplateRequestRequestTypeDef(TypedDict):
    domainId: str,
    templateId: str,
```

## LayoutSummaryTypeDef

```python
# LayoutSummaryTypeDef definition

class LayoutSummaryTypeDef(TypedDict):
    layoutArn: str,
    layoutId: str,
    name: str,
```

## ListCasesForContactRequestRequestTypeDef

```python
# ListCasesForContactRequestRequestTypeDef definition

class ListCasesForContactRequestRequestTypeDef(TypedDict):
    contactArn: str,
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListFieldOptionsRequestRequestTypeDef

```python
# ListFieldOptionsRequestRequestTypeDef definition

class ListFieldOptionsRequestRequestTypeDef(TypedDict):
    domainId: str,
    fieldId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## ListFieldsRequestRequestTypeDef

```python
# ListFieldsRequestRequestTypeDef definition

class ListFieldsRequestRequestTypeDef(TypedDict):
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListLayoutsRequestRequestTypeDef

```python
# ListLayoutsRequestRequestTypeDef definition

class ListLayoutsRequestRequestTypeDef(TypedDict):
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    arn: str,
```

## ListTemplatesRequestRequestTypeDef

```python
# ListTemplatesRequestRequestTypeDef definition

class ListTemplatesRequestRequestTypeDef(TypedDict):
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[Sequence[TemplateStatusType]],  # (1)
```

1. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## TemplateSummaryTypeDef

```python
# TemplateSummaryTypeDef definition

class TemplateSummaryTypeDef(TypedDict):
    name: str,
    status: TemplateStatusType,  # (1)
    templateArn: str,
    templateId: str,
```

1. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## SortTypeDef

```python
# SortTypeDef definition

class SortTypeDef(TypedDict):
    fieldId: str,
    sortOrder: OrderType,  # (1)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
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

## UpdateFieldRequestRequestTypeDef

```python
# UpdateFieldRequestRequestTypeDef definition

class UpdateFieldRequestRequestTypeDef(TypedDict):
    domainId: str,
    fieldId: str,
    description: NotRequired[str],
    name: NotRequired[str],
```

## AuditEventFieldTypeDef

```python
# AuditEventFieldTypeDef definition

class AuditEventFieldTypeDef(TypedDict):
    eventFieldId: str,
    newValue: AuditEventFieldValueUnionTypeDef,  # (1)
    oldValue: NotRequired[AuditEventFieldValueUnionTypeDef],  # (1)
```

1. See [:material-code-braces: AuditEventFieldValueUnionTypeDef](./type_defs.md#auditeventfieldvalueuniontypedef) 
2. See [:material-code-braces: AuditEventFieldValueUnionTypeDef](./type_defs.md#auditeventfieldvalueuniontypedef) 
## AuditEventPerformedByTypeDef

```python
# AuditEventPerformedByTypeDef definition

class AuditEventPerformedByTypeDef(TypedDict):
    iamPrincipalArn: str,
    user: NotRequired[UserUnionTypeDef],  # (1)
```

1. See [:material-code-braces: UserUnionTypeDef](./type_defs.md#useruniontypedef) 
## BatchGetFieldRequestRequestTypeDef

```python
# BatchGetFieldRequestRequestTypeDef definition

class BatchGetFieldRequestRequestTypeDef(TypedDict):
    domainId: str,
    fields: Sequence[FieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## CaseEventIncludedDataOutputTypeDef

```python
# CaseEventIncludedDataOutputTypeDef definition

class CaseEventIncludedDataOutputTypeDef(TypedDict):
    fields: List[FieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## CaseEventIncludedDataTypeDef

```python
# CaseEventIncludedDataTypeDef definition

class CaseEventIncludedDataTypeDef(TypedDict):
    fields: Sequence[FieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## GetCaseRequestRequestTypeDef

```python
# GetCaseRequestRequestTypeDef definition

class GetCaseRequestRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    fields: Sequence[FieldIdentifierTypeDef],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## BatchGetFieldResponseTypeDef

```python
# BatchGetFieldResponseTypeDef definition

class BatchGetFieldResponseTypeDef(TypedDict):
    errors: List[FieldErrorTypeDef],  # (1)
    fields: List[GetFieldResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FieldErrorTypeDef](./type_defs.md#fielderrortypedef) 
2. See [:material-code-braces: GetFieldResponseTypeDef](./type_defs.md#getfieldresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseResponseTypeDef

```python
# CreateCaseResponseTypeDef definition

class CreateCaseResponseTypeDef(TypedDict):
    caseArn: str,
    caseId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainResponseTypeDef

```python
# CreateDomainResponseTypeDef definition

class CreateDomainResponseTypeDef(TypedDict):
    domainArn: str,
    domainId: str,
    domainStatus: DomainStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFieldResponseTypeDef

```python
# CreateFieldResponseTypeDef definition

class CreateFieldResponseTypeDef(TypedDict):
    fieldArn: str,
    fieldId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLayoutResponseTypeDef

```python
# CreateLayoutResponseTypeDef definition

class CreateLayoutResponseTypeDef(TypedDict):
    layoutArn: str,
    layoutId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRelatedItemResponseTypeDef

```python
# CreateRelatedItemResponseTypeDef definition

class CreateRelatedItemResponseTypeDef(TypedDict):
    relatedItemArn: str,
    relatedItemId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateResponseTypeDef

```python
# CreateTemplateResponseTypeDef definition

class CreateTemplateResponseTypeDef(TypedDict):
    templateArn: str,
    templateId: str,
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
## GetDomainResponseTypeDef

```python
# GetDomainResponseTypeDef definition

class GetDomainResponseTypeDef(TypedDict):
    createdTime: datetime,
    domainArn: str,
    domainId: str,
    domainStatus: DomainStatusType,  # (1)
    name: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutFieldOptionsRequestRequestTypeDef

```python
# BatchPutFieldOptionsRequestRequestTypeDef definition

class BatchPutFieldOptionsRequestRequestTypeDef(TypedDict):
    domainId: str,
    fieldId: str,
    options: Sequence[FieldOptionTypeDef],  # (1)
```

1. See [:material-code-braces: FieldOptionTypeDef](./type_defs.md#fieldoptiontypedef) 
## ListFieldOptionsResponseTypeDef

```python
# ListFieldOptionsResponseTypeDef definition

class ListFieldOptionsResponseTypeDef(TypedDict):
    options: List[FieldOptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FieldOptionTypeDef](./type_defs.md#fieldoptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutFieldOptionsResponseTypeDef

```python
# BatchPutFieldOptionsResponseTypeDef definition

class BatchPutFieldOptionsResponseTypeDef(TypedDict):
    errors: List[FieldOptionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldOptionErrorTypeDef](./type_defs.md#fieldoptionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCasesForContactResponseTypeDef

```python
# ListCasesForContactResponseTypeDef definition

class ListCasesForContactResponseTypeDef(TypedDict):
    cases: List[CaseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CaseSummaryTypeDef](./type_defs.md#casesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateRequestRequestTypeDef

```python
# CreateTemplateRequestRequestTypeDef definition

class CreateTemplateRequestRequestTypeDef(TypedDict):
    domainId: str,
    name: str,
    description: NotRequired[str],
    layoutConfiguration: NotRequired[LayoutConfigurationTypeDef],  # (1)
    requiredFields: NotRequired[Sequence[RequiredFieldTypeDef]],  # (2)
    status: NotRequired[TemplateStatusType],  # (3)
```

1. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
2. See [:material-code-braces: RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef) 
3. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## GetTemplateResponseTypeDef

```python
# GetTemplateResponseTypeDef definition

class GetTemplateResponseTypeDef(TypedDict):
    createdTime: datetime,
    deleted: bool,
    description: str,
    lastModifiedTime: datetime,
    layoutConfiguration: LayoutConfigurationTypeDef,  # (1)
    name: str,
    requiredFields: List[RequiredFieldTypeDef],  # (2)
    status: TemplateStatusType,  # (3)
    tags: Dict[str, str],
    templateArn: str,
    templateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
2. See [:material-code-braces: RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef) 
3. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplateRequestRequestTypeDef

```python
# UpdateTemplateRequestRequestTypeDef definition

class UpdateTemplateRequestRequestTypeDef(TypedDict):
    domainId: str,
    templateId: str,
    description: NotRequired[str],
    layoutConfiguration: NotRequired[LayoutConfigurationTypeDef],  # (1)
    name: NotRequired[str],
    requiredFields: NotRequired[Sequence[RequiredFieldTypeDef]],  # (2)
    status: NotRequired[TemplateStatusType],  # (3)
```

1. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
2. See [:material-code-braces: RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef) 
3. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## ListDomainsResponseTypeDef

```python
# ListDomainsResponseTypeDef definition

class ListDomainsResponseTypeDef(TypedDict):
    domains: List[DomainSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FieldGroupOutputTypeDef

```python
# FieldGroupOutputTypeDef definition

class FieldGroupOutputTypeDef(TypedDict):
    fields: List[FieldItemTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: FieldItemTypeDef](./type_defs.md#fielditemtypedef) 
## FieldGroupTypeDef

```python
# FieldGroupTypeDef definition

class FieldGroupTypeDef(TypedDict):
    fields: Sequence[FieldItemTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: FieldItemTypeDef](./type_defs.md#fielditemtypedef) 
## ListFieldsResponseTypeDef

```python
# ListFieldsResponseTypeDef definition

class ListFieldsResponseTypeDef(TypedDict):
    fields: List[FieldSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FieldSummaryTypeDef](./type_defs.md#fieldsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FieldValueOutputTypeDef

```python
# FieldValueOutputTypeDef definition

class FieldValueOutputTypeDef(TypedDict):
    id: str,
    value: FieldValueUnionOutputTypeDef,  # (1)
```

1. See [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 
## RelatedItemContentTypeDef

```python
# RelatedItemContentTypeDef definition

class RelatedItemContentTypeDef(TypedDict):
    comment: NotRequired[CommentContentTypeDef],  # (1)
    contact: NotRequired[ContactContentTypeDef],  # (2)
    file: NotRequired[FileContentTypeDef],  # (3)
```

1. See [:material-code-braces: CommentContentTypeDef](./type_defs.md#commentcontenttypedef) 
2. See [:material-code-braces: ContactContentTypeDef](./type_defs.md#contactcontenttypedef) 
3. See [:material-code-braces: FileContentTypeDef](./type_defs.md#filecontenttypedef) 
## RelatedItemInputContentTypeDef

```python
# RelatedItemInputContentTypeDef definition

class RelatedItemInputContentTypeDef(TypedDict):
    comment: NotRequired[CommentContentTypeDef],  # (1)
    contact: NotRequired[ContactTypeDef],  # (2)
    file: NotRequired[FileContentTypeDef],  # (3)
```

1. See [:material-code-braces: CommentContentTypeDef](./type_defs.md#commentcontenttypedef) 
2. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
3. See [:material-code-braces: FileContentTypeDef](./type_defs.md#filecontenttypedef) 
## RelatedItemTypeFilterTypeDef

```python
# RelatedItemTypeFilterTypeDef definition

class RelatedItemTypeFilterTypeDef(TypedDict):
    comment: NotRequired[Mapping[str, Any]],
    contact: NotRequired[ContactFilterTypeDef],  # (1)
    file: NotRequired[FileFilterTypeDef],  # (2)
```

1. See [:material-code-braces: ContactFilterTypeDef](./type_defs.md#contactfiltertypedef) 
2. See [:material-code-braces: FileFilterTypeDef](./type_defs.md#filefiltertypedef) 
## ListLayoutsResponseTypeDef

```python
# ListLayoutsResponseTypeDef definition

class ListLayoutsResponseTypeDef(TypedDict):
    layouts: List[LayoutSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LayoutSummaryTypeDef](./type_defs.md#layoutsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplatesResponseTypeDef

```python
# ListTemplatesResponseTypeDef definition

class ListTemplatesResponseTypeDef(TypedDict):
    templates: List[TemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AuditEventTypeDef

```python
# AuditEventTypeDef definition

class AuditEventTypeDef(TypedDict):
    eventId: str,
    fields: List[AuditEventFieldTypeDef],  # (1)
    performedTime: datetime,
    type: AuditEventTypeType,  # (4)
    performedBy: NotRequired[AuditEventPerformedByTypeDef],  # (2)
    relatedItemType: NotRequired[RelatedItemTypeType],  # (3)
```

1. See [:material-code-braces: AuditEventFieldTypeDef](./type_defs.md#auditeventfieldtypedef) 
2. See [:material-code-braces: AuditEventPerformedByTypeDef](./type_defs.md#auditeventperformedbytypedef) 
3. See [:material-code-brackets: RelatedItemTypeType](./literals.md#relateditemtypetype) 
4. See [:material-code-brackets: AuditEventTypeType](./literals.md#auditeventtypetype) 
## EventIncludedDataOutputTypeDef

```python
# EventIncludedDataOutputTypeDef definition

class EventIncludedDataOutputTypeDef(TypedDict):
    caseData: NotRequired[CaseEventIncludedDataOutputTypeDef],  # (1)
    relatedItemData: NotRequired[RelatedItemEventIncludedDataTypeDef],  # (2)
```

1. See [:material-code-braces: CaseEventIncludedDataOutputTypeDef](./type_defs.md#caseeventincludeddataoutputtypedef) 
2. See [:material-code-braces: RelatedItemEventIncludedDataTypeDef](./type_defs.md#relateditemeventincludeddatatypedef) 
## SectionOutputTypeDef

```python
# SectionOutputTypeDef definition

class SectionOutputTypeDef(TypedDict):
    fieldGroup: NotRequired[FieldGroupOutputTypeDef],  # (1)
```

1. See [:material-code-braces: FieldGroupOutputTypeDef](./type_defs.md#fieldgroupoutputtypedef) 
## GetCaseResponseTypeDef

```python
# GetCaseResponseTypeDef definition

class GetCaseResponseTypeDef(TypedDict):
    fields: List[FieldValueOutputTypeDef],  # (1)
    tags: Dict[str, str],
    templateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchCasesResponseItemTypeDef

```python
# SearchCasesResponseItemTypeDef definition

class SearchCasesResponseItemTypeDef(TypedDict):
    caseId: str,
    fields: List[FieldValueOutputTypeDef],  # (1)
    templateId: str,
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
## FieldValueTypeDef

```python
# FieldValueTypeDef definition

class FieldValueTypeDef(TypedDict):
    id: str,
    value: FieldValueUnionUnionTypeDef,  # (1)
```

1. See [:material-code-braces: FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef) [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 
## SearchRelatedItemsResponseItemTypeDef

```python
# SearchRelatedItemsResponseItemTypeDef definition

class SearchRelatedItemsResponseItemTypeDef(TypedDict):
    associationTime: datetime,
    content: RelatedItemContentTypeDef,  # (1)
    relatedItemId: str,
    type: RelatedItemTypeType,  # (3)
    performedBy: NotRequired[UserUnionTypeDef],  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RelatedItemContentTypeDef](./type_defs.md#relateditemcontenttypedef) 
2. See [:material-code-braces: UserUnionTypeDef](./type_defs.md#useruniontypedef) 
3. See [:material-code-brackets: RelatedItemTypeType](./literals.md#relateditemtypetype) 
## CreateRelatedItemRequestRequestTypeDef

```python
# CreateRelatedItemRequestRequestTypeDef definition

class CreateRelatedItemRequestRequestTypeDef(TypedDict):
    caseId: str,
    content: RelatedItemInputContentTypeDef,  # (1)
    domainId: str,
    type: RelatedItemTypeType,  # (2)
    performedBy: NotRequired[UserUnionTypeDef],  # (3)
```

1. See [:material-code-braces: RelatedItemInputContentTypeDef](./type_defs.md#relatediteminputcontenttypedef) 
2. See [:material-code-brackets: RelatedItemTypeType](./literals.md#relateditemtypetype) 
3. See [:material-code-braces: UserUnionTypeDef](./type_defs.md#useruniontypedef) 
## SearchRelatedItemsRequestPaginateTypeDef

```python
# SearchRelatedItemsRequestPaginateTypeDef definition

class SearchRelatedItemsRequestPaginateTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    filters: NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RelatedItemTypeFilterTypeDef](./type_defs.md#relateditemtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchRelatedItemsRequestRequestTypeDef

```python
# SearchRelatedItemsRequestRequestTypeDef definition

class SearchRelatedItemsRequestRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    filters: NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RelatedItemTypeFilterTypeDef](./type_defs.md#relateditemtypefiltertypedef) 
## GetCaseAuditEventsResponseTypeDef

```python
# GetCaseAuditEventsResponseTypeDef definition

class GetCaseAuditEventsResponseTypeDef(TypedDict):
    auditEvents: List[AuditEventTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AuditEventTypeDef](./type_defs.md#auditeventtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EventBridgeConfigurationOutputTypeDef

```python
# EventBridgeConfigurationOutputTypeDef definition

class EventBridgeConfigurationOutputTypeDef(TypedDict):
    enabled: bool,
    includedData: NotRequired[EventIncludedDataOutputTypeDef],  # (1)
```

1. See [:material-code-braces: EventIncludedDataOutputTypeDef](./type_defs.md#eventincludeddataoutputtypedef) 
## EventIncludedDataTypeDef

```python
# EventIncludedDataTypeDef definition

class EventIncludedDataTypeDef(TypedDict):
    caseData: NotRequired[CaseEventIncludedDataUnionTypeDef],  # (1)
    relatedItemData: NotRequired[RelatedItemEventIncludedDataTypeDef],  # (2)
```

1. See [:material-code-braces: CaseEventIncludedDataTypeDef](./type_defs.md#caseeventincludeddatatypedef) [:material-code-braces: CaseEventIncludedDataOutputTypeDef](./type_defs.md#caseeventincludeddataoutputtypedef) 
2. See [:material-code-braces: RelatedItemEventIncludedDataTypeDef](./type_defs.md#relateditemeventincludeddatatypedef) 
## LayoutSectionsOutputTypeDef

```python
# LayoutSectionsOutputTypeDef definition

class LayoutSectionsOutputTypeDef(TypedDict):
    sections: NotRequired[List[SectionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: SectionOutputTypeDef](./type_defs.md#sectionoutputtypedef) 
## SectionTypeDef

```python
# SectionTypeDef definition

class SectionTypeDef(TypedDict):
    fieldGroup: NotRequired[FieldGroupUnionTypeDef],  # (1)
```

1. See [:material-code-braces: FieldGroupTypeDef](./type_defs.md#fieldgrouptypedef) [:material-code-braces: FieldGroupOutputTypeDef](./type_defs.md#fieldgroupoutputtypedef) 
## SearchCasesResponseTypeDef

```python
# SearchCasesResponseTypeDef definition

class SearchCasesResponseTypeDef(TypedDict):
    cases: List[SearchCasesResponseItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchCasesResponseItemTypeDef](./type_defs.md#searchcasesresponseitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCaseRequestRequestTypeDef

```python
# UpdateCaseRequestRequestTypeDef definition

class UpdateCaseRequestRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    fields: Sequence[FieldValueTypeDef],  # (1)
    performedBy: NotRequired[UserUnionTypeDef],  # (2)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
2. See [:material-code-braces: UserUnionTypeDef](./type_defs.md#useruniontypedef) 
## SearchRelatedItemsResponseTypeDef

```python
# SearchRelatedItemsResponseTypeDef definition

class SearchRelatedItemsResponseTypeDef(TypedDict):
    relatedItems: List[SearchRelatedItemsResponseItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchRelatedItemsResponseItemTypeDef](./type_defs.md#searchrelateditemsresponseitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCaseEventConfigurationResponseTypeDef

```python
# GetCaseEventConfigurationResponseTypeDef definition

class GetCaseEventConfigurationResponseTypeDef(TypedDict):
    eventBridge: EventBridgeConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventBridgeConfigurationOutputTypeDef](./type_defs.md#eventbridgeconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BasicLayoutOutputTypeDef

```python
# BasicLayoutOutputTypeDef definition

class BasicLayoutOutputTypeDef(TypedDict):
    moreInfo: NotRequired[LayoutSectionsOutputTypeDef],  # (1)
    topPanel: NotRequired[LayoutSectionsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef) 
2. See [:material-code-braces: LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef) 
## CreateCaseRequestRequestTypeDef

```python
# CreateCaseRequestRequestTypeDef definition

class CreateCaseRequestRequestTypeDef(TypedDict):
    domainId: str,
    fields: Sequence[FieldValueExtraUnionTypeDef],  # (1)
    templateId: str,
    clientToken: NotRequired[str],
    performedBy: NotRequired[UserUnionTypeDef],  # (2)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
2. See [:material-code-braces: UserUnionTypeDef](./type_defs.md#useruniontypedef) 
## FieldFilterTypeDef

```python
# FieldFilterTypeDef definition

class FieldFilterTypeDef(TypedDict):
    contains: NotRequired[FieldValueExtraUnionTypeDef],  # (1)
    equalTo: NotRequired[FieldValueExtraUnionTypeDef],  # (1)
    greaterThan: NotRequired[FieldValueExtraUnionTypeDef],  # (1)
    greaterThanOrEqualTo: NotRequired[FieldValueExtraUnionTypeDef],  # (1)
    lessThan: NotRequired[FieldValueExtraUnionTypeDef],  # (1)
    lessThanOrEqualTo: NotRequired[FieldValueExtraUnionTypeDef],  # (1)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
2. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
3. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
4. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
5. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
6. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
## EventBridgeConfigurationTypeDef

```python
# EventBridgeConfigurationTypeDef definition

class EventBridgeConfigurationTypeDef(TypedDict):
    enabled: bool,
    includedData: NotRequired[EventIncludedDataUnionTypeDef],  # (1)
```

1. See [:material-code-braces: EventIncludedDataTypeDef](./type_defs.md#eventincludeddatatypedef) [:material-code-braces: EventIncludedDataOutputTypeDef](./type_defs.md#eventincludeddataoutputtypedef) 
## LayoutContentOutputTypeDef

```python
# LayoutContentOutputTypeDef definition

class LayoutContentOutputTypeDef(TypedDict):
    basic: NotRequired[BasicLayoutOutputTypeDef],  # (1)
```

1. See [:material-code-braces: BasicLayoutOutputTypeDef](./type_defs.md#basiclayoutoutputtypedef) 
## LayoutSectionsTypeDef

```python
# LayoutSectionsTypeDef definition

class LayoutSectionsTypeDef(TypedDict):
    sections: NotRequired[Sequence[SectionUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: SectionTypeDef](./type_defs.md#sectiontypedef) [:material-code-braces: SectionOutputTypeDef](./type_defs.md#sectionoutputtypedef) 
## CaseFilterPaginatorTypeDef

```python
# CaseFilterPaginatorTypeDef definition

class CaseFilterPaginatorTypeDef(TypedDict):
    andAll: NotRequired[Sequence[Mapping[str, Any]]],
    field: NotRequired[FieldFilterTypeDef],  # (1)
    not: NotRequired[Mapping[str, Any]],
    orAll: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: FieldFilterTypeDef](./type_defs.md#fieldfiltertypedef) 
## CaseFilterTypeDef

```python
# CaseFilterTypeDef definition

class CaseFilterTypeDef(TypedDict):
    andAll: NotRequired[Sequence[Mapping[str, Any]]],
    field: NotRequired[FieldFilterTypeDef],  # (1)
    not: NotRequired[Mapping[str, Any]],
    orAll: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: FieldFilterTypeDef](./type_defs.md#fieldfiltertypedef) 
## PutCaseEventConfigurationRequestRequestTypeDef

```python
# PutCaseEventConfigurationRequestRequestTypeDef definition

class PutCaseEventConfigurationRequestRequestTypeDef(TypedDict):
    domainId: str,
    eventBridge: EventBridgeConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef) 
## GetLayoutResponseTypeDef

```python
# GetLayoutResponseTypeDef definition

class GetLayoutResponseTypeDef(TypedDict):
    content: LayoutContentOutputTypeDef,  # (1)
    createdTime: datetime,
    deleted: bool,
    lastModifiedTime: datetime,
    layoutArn: str,
    layoutId: str,
    name: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LayoutContentOutputTypeDef](./type_defs.md#layoutcontentoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchCasesRequestPaginateTypeDef

```python
# SearchCasesRequestPaginateTypeDef definition

class SearchCasesRequestPaginateTypeDef(TypedDict):
    domainId: str,
    fields: NotRequired[Sequence[FieldIdentifierTypeDef]],  # (1)
    filter: NotRequired[CaseFilterPaginatorTypeDef],  # (2)
    searchTerm: NotRequired[str],
    sorts: NotRequired[Sequence[SortTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
2. See [:material-code-braces: CaseFilterPaginatorTypeDef](./type_defs.md#casefilterpaginatortypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchCasesRequestRequestTypeDef

```python
# SearchCasesRequestRequestTypeDef definition

class SearchCasesRequestRequestTypeDef(TypedDict):
    domainId: str,
    fields: NotRequired[Sequence[FieldIdentifierTypeDef]],  # (1)
    filter: NotRequired[CaseFilterTypeDef],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    searchTerm: NotRequired[str],
    sorts: NotRequired[Sequence[SortTypeDef]],  # (3)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
2. See [:material-code-braces: CaseFilterTypeDef](./type_defs.md#casefiltertypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
## BasicLayoutTypeDef

```python
# BasicLayoutTypeDef definition

class BasicLayoutTypeDef(TypedDict):
    moreInfo: NotRequired[LayoutSectionsUnionTypeDef],  # (1)
    topPanel: NotRequired[LayoutSectionsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef) [:material-code-braces: LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef) 
2. See [:material-code-braces: LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef) [:material-code-braces: LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef) 
## LayoutContentTypeDef

```python
# LayoutContentTypeDef definition

class LayoutContentTypeDef(TypedDict):
    basic: NotRequired[BasicLayoutUnionTypeDef],  # (1)
```

1. See [:material-code-braces: BasicLayoutTypeDef](./type_defs.md#basiclayouttypedef) [:material-code-braces: BasicLayoutOutputTypeDef](./type_defs.md#basiclayoutoutputtypedef) 
## CreateLayoutRequestRequestTypeDef

```python
# CreateLayoutRequestRequestTypeDef definition

class CreateLayoutRequestRequestTypeDef(TypedDict):
    content: LayoutContentTypeDef,  # (1)
    domainId: str,
    name: str,
```

1. See [:material-code-braces: LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef) 
## UpdateLayoutRequestRequestTypeDef

```python
# UpdateLayoutRequestRequestTypeDef definition

class UpdateLayoutRequestRequestTypeDef(TypedDict):
    domainId: str,
    layoutId: str,
    content: NotRequired[LayoutContentTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef) 

# Type definitions

> [Index](../README.md) > [ConnectCases](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).



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
    description: NotRequired[str],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: FieldNamespaceType](./literals.md#fieldnamespacetype) 
2. See [:material-code-brackets: FieldTypeType](./literals.md#fieldtypetype) 
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
## FieldValueUnionTypeDef

```python
# FieldValueUnionTypeDef definition

class FieldValueUnionTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    emptyValue: NotRequired[Mapping[str, Any]],
    stringValue: NotRequired[str],
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

## BatchGetFieldRequestRequestTypeDef

```python
# BatchGetFieldRequestRequestTypeDef definition

class BatchGetFieldRequestRequestTypeDef(TypedDict):
    domainId: str,
    fields: Sequence[FieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## CaseEventIncludedDataTypeDef

```python
# CaseEventIncludedDataTypeDef definition

class CaseEventIncludedDataTypeDef(TypedDict):
    fields: List[FieldIdentifierTypeDef],  # (1)
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
    nextToken: str,
    options: List[FieldOptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CaseSummaryTypeDef](./type_defs.md#casesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RelatedItemContentTypeDef

```python
# RelatedItemContentTypeDef definition

class RelatedItemContentTypeDef(TypedDict):
    comment: NotRequired[CommentContentTypeDef],  # (1)
    contact: NotRequired[ContactContentTypeDef],  # (2)
```

1. See [:material-code-braces: CommentContentTypeDef](./type_defs.md#commentcontenttypedef) 
2. See [:material-code-braces: ContactContentTypeDef](./type_defs.md#contactcontenttypedef) 
## RelatedItemTypeFilterTypeDef

```python
# RelatedItemTypeFilterTypeDef definition

class RelatedItemTypeFilterTypeDef(TypedDict):
    comment: NotRequired[Mapping[str, Any]],
    contact: NotRequired[ContactFilterTypeDef],  # (1)
```

1. See [:material-code-braces: ContactFilterTypeDef](./type_defs.md#contactfiltertypedef) 
## RelatedItemInputContentTypeDef

```python
# RelatedItemInputContentTypeDef definition

class RelatedItemInputContentTypeDef(TypedDict):
    comment: NotRequired[CommentContentTypeDef],  # (1)
    contact: NotRequired[ContactTypeDef],  # (2)
```

1. See [:material-code-braces: CommentContentTypeDef](./type_defs.md#commentcontenttypedef) 
2. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
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
    description: str,
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldSummaryTypeDef](./type_defs.md#fieldsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FieldValueTypeDef

```python
# FieldValueTypeDef definition

class FieldValueTypeDef(TypedDict):
    id: str,
    value: FieldValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef) 
## ListLayoutsResponseTypeDef

```python
# ListLayoutsResponseTypeDef definition

class ListLayoutsResponseTypeDef(TypedDict):
    layouts: List[LayoutSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LayoutSummaryTypeDef](./type_defs.md#layoutsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTemplatesResponseTypeDef

```python
# ListTemplatesResponseTypeDef definition

class ListTemplatesResponseTypeDef(TypedDict):
    nextToken: str,
    templates: List[TemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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
## SearchCasesRequestSearchCasesPaginateTypeDef

```python
# SearchCasesRequestSearchCasesPaginateTypeDef definition

class SearchCasesRequestSearchCasesPaginateTypeDef(TypedDict):
    domainId: str,
    fields: NotRequired[Sequence[FieldIdentifierTypeDef]],  # (1)
    filter: NotRequired[CaseFilterTypeDef],  # (2)
    searchTerm: NotRequired[str],
    sorts: NotRequired[Sequence[SortTypeDef]],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
2. See [:material-code-braces: CaseFilterTypeDef](./type_defs.md#casefiltertypedef) 
3. See [:material-code-braces: SortTypeDef](./type_defs.md#sorttypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## EventIncludedDataTypeDef

```python
# EventIncludedDataTypeDef definition

class EventIncludedDataTypeDef(TypedDict):
    caseData: NotRequired[CaseEventIncludedDataTypeDef],  # (1)
    relatedItemData: NotRequired[RelatedItemEventIncludedDataTypeDef],  # (2)
```

1. See [:material-code-braces: CaseEventIncludedDataTypeDef](./type_defs.md#caseeventincludeddatatypedef) 
2. See [:material-code-braces: RelatedItemEventIncludedDataTypeDef](./type_defs.md#relateditemeventincludeddatatypedef) 
## SearchRelatedItemsResponseItemTypeDef

```python
# SearchRelatedItemsResponseItemTypeDef definition

class SearchRelatedItemsResponseItemTypeDef(TypedDict):
    associationTime: datetime,
    content: RelatedItemContentTypeDef,  # (1)
    relatedItemId: str,
    type: RelatedItemTypeType,  # (2)
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: RelatedItemContentTypeDef](./type_defs.md#relateditemcontenttypedef) 
2. See [:material-code-brackets: RelatedItemTypeType](./literals.md#relateditemtypetype) 
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
## SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef

```python
# SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef definition

class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    filters: NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RelatedItemTypeFilterTypeDef](./type_defs.md#relateditemtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## CreateRelatedItemRequestRequestTypeDef

```python
# CreateRelatedItemRequestRequestTypeDef definition

class CreateRelatedItemRequestRequestTypeDef(TypedDict):
    caseId: str,
    content: RelatedItemInputContentTypeDef,  # (1)
    domainId: str,
    type: RelatedItemTypeType,  # (2)
```

1. See [:material-code-braces: RelatedItemInputContentTypeDef](./type_defs.md#relatediteminputcontenttypedef) 
2. See [:material-code-brackets: RelatedItemTypeType](./literals.md#relateditemtypetype) 
## SectionTypeDef

```python
# SectionTypeDef definition

class SectionTypeDef(TypedDict):
    fieldGroup: NotRequired[FieldGroupTypeDef],  # (1)
```

1. See [:material-code-braces: FieldGroupTypeDef](./type_defs.md#fieldgrouptypedef) 
## CreateCaseRequestRequestTypeDef

```python
# CreateCaseRequestRequestTypeDef definition

class CreateCaseRequestRequestTypeDef(TypedDict):
    domainId: str,
    fields: Sequence[FieldValueTypeDef],  # (1)
    templateId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
## FieldFilterTypeDef

```python
# FieldFilterTypeDef definition

class FieldFilterTypeDef(TypedDict):
    contains: NotRequired[FieldValueTypeDef],  # (1)
    equalTo: NotRequired[FieldValueTypeDef],  # (1)
    greaterThan: NotRequired[FieldValueTypeDef],  # (1)
    greaterThanOrEqualTo: NotRequired[FieldValueTypeDef],  # (1)
    lessThan: NotRequired[FieldValueTypeDef],  # (1)
    lessThanOrEqualTo: NotRequired[FieldValueTypeDef],  # (1)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
2. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
3. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
4. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
5. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
6. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
## GetCaseResponseTypeDef

```python
# GetCaseResponseTypeDef definition

class GetCaseResponseTypeDef(TypedDict):
    fields: List[FieldValueTypeDef],  # (1)
    nextToken: str,
    tags: Dict[str, str],
    templateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchCasesResponseItemTypeDef

```python
# SearchCasesResponseItemTypeDef definition

class SearchCasesResponseItemTypeDef(TypedDict):
    caseId: str,
    fields: List[FieldValueTypeDef],  # (1)
    templateId: str,
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
## UpdateCaseRequestRequestTypeDef

```python
# UpdateCaseRequestRequestTypeDef definition

class UpdateCaseRequestRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    fields: Sequence[FieldValueTypeDef],  # (1)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
## EventBridgeConfigurationTypeDef

```python
# EventBridgeConfigurationTypeDef definition

class EventBridgeConfigurationTypeDef(TypedDict):
    enabled: bool,
    includedData: NotRequired[EventIncludedDataTypeDef],  # (1)
```

1. See [:material-code-braces: EventIncludedDataTypeDef](./type_defs.md#eventincludeddatatypedef) 
## SearchRelatedItemsResponseTypeDef

```python
# SearchRelatedItemsResponseTypeDef definition

class SearchRelatedItemsResponseTypeDef(TypedDict):
    nextToken: str,
    relatedItems: List[SearchRelatedItemsResponseItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SearchRelatedItemsResponseItemTypeDef](./type_defs.md#searchrelateditemsresponseitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LayoutSectionsTypeDef

```python
# LayoutSectionsTypeDef definition

class LayoutSectionsTypeDef(TypedDict):
    sections: NotRequired[Sequence[SectionTypeDef]],  # (1)
```

1. See [:material-code-braces: SectionTypeDef](./type_defs.md#sectiontypedef) 
## CaseFilterTypeDef

```python
# CaseFilterTypeDef definition

class CaseFilterTypeDef(TypedDict):
    andAll: NotRequired[Sequence[CaseFilterTypeDef]],  # (1)
    field: NotRequired[FieldFilterTypeDef],  # (2)
    not: NotRequired[CaseFilterTypeDef],  # (3)
    orAll: NotRequired[Sequence[CaseFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: CaseFilterTypeDef](./type_defs.md#casefiltertypedef) 
2. See [:material-code-braces: FieldFilterTypeDef](./type_defs.md#fieldfiltertypedef) 
3. See [:material-code-braces: CaseFilterTypeDef](./type_defs.md#casefiltertypedef) 
4. See [:material-code-braces: CaseFilterTypeDef](./type_defs.md#casefiltertypedef) 
## SearchCasesResponseTypeDef

```python
# SearchCasesResponseTypeDef definition

class SearchCasesResponseTypeDef(TypedDict):
    cases: List[SearchCasesResponseItemTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SearchCasesResponseItemTypeDef](./type_defs.md#searchcasesresponseitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCaseEventConfigurationResponseTypeDef

```python
# GetCaseEventConfigurationResponseTypeDef definition

class GetCaseEventConfigurationResponseTypeDef(TypedDict):
    eventBridge: EventBridgeConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutCaseEventConfigurationRequestRequestTypeDef

```python
# PutCaseEventConfigurationRequestRequestTypeDef definition

class PutCaseEventConfigurationRequestRequestTypeDef(TypedDict):
    domainId: str,
    eventBridge: EventBridgeConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef) 
## BasicLayoutTypeDef

```python
# BasicLayoutTypeDef definition

class BasicLayoutTypeDef(TypedDict):
    moreInfo: NotRequired[LayoutSectionsTypeDef],  # (1)
    topPanel: NotRequired[LayoutSectionsTypeDef],  # (1)
```

1. See [:material-code-braces: LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef) 
2. See [:material-code-braces: LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef) 
## LayoutContentTypeDef

```python
# LayoutContentTypeDef definition

class LayoutContentTypeDef(TypedDict):
    basic: NotRequired[BasicLayoutTypeDef],  # (1)
```

1. See [:material-code-braces: BasicLayoutTypeDef](./type_defs.md#basiclayouttypedef) 
## CreateLayoutRequestRequestTypeDef

```python
# CreateLayoutRequestRequestTypeDef definition

class CreateLayoutRequestRequestTypeDef(TypedDict):
    content: LayoutContentTypeDef,  # (1)
    domainId: str,
    name: str,
```

1. See [:material-code-braces: LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef) 
## GetLayoutResponseTypeDef

```python
# GetLayoutResponseTypeDef definition

class GetLayoutResponseTypeDef(TypedDict):
    content: LayoutContentTypeDef,  # (1)
    layoutArn: str,
    layoutId: str,
    name: str,
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
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

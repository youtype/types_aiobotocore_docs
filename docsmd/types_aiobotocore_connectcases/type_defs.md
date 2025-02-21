# Type definitions

> [Index](../README.md) > [ConnectCases](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#connectcases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## FieldValueUnionUnionTypeDef

```python
# FieldValueUnionUnionTypeDef Union usage example

from types_aiobotocore_connectcases.type_defs import FieldValueUnionUnionTypeDef


def get_value() -> FieldValueUnionUnionTypeDef:
    return ...


# FieldValueUnionUnionTypeDef definition

FieldValueUnionUnionTypeDef = Union[
    FieldValueUnionTypeDef,  # (1)
    FieldValueUnionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef) 
2. See [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 

## FieldValueUnionExtraTypeDef

```python
# FieldValueUnionExtraTypeDef Union usage example

from types_aiobotocore_connectcases.type_defs import FieldValueUnionExtraTypeDef


def get_value() -> FieldValueUnionExtraTypeDef:
    return ...


# FieldValueUnionExtraTypeDef definition

FieldValueUnionExtraTypeDef = Union[
    FieldValueTypeDef,  # (1)
    FieldValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) 
2. See [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 

## EventBridgeConfigurationUnionTypeDef

```python
# EventBridgeConfigurationUnionTypeDef Union usage example

from types_aiobotocore_connectcases.type_defs import EventBridgeConfigurationUnionTypeDef


def get_value() -> EventBridgeConfigurationUnionTypeDef:
    return ...


# EventBridgeConfigurationUnionTypeDef definition

EventBridgeConfigurationUnionTypeDef = Union[
    EventBridgeConfigurationTypeDef,  # (1)
    EventBridgeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef) 
2. See [:material-code-braces: EventBridgeConfigurationOutputTypeDef](./type_defs.md#eventbridgeconfigurationoutputtypedef) 

## CaseRuleDetailsUnionTypeDef

```python
# CaseRuleDetailsUnionTypeDef Union usage example

from types_aiobotocore_connectcases.type_defs import CaseRuleDetailsUnionTypeDef


def get_value() -> CaseRuleDetailsUnionTypeDef:
    return ...


# CaseRuleDetailsUnionTypeDef definition

CaseRuleDetailsUnionTypeDef = Union[
    CaseRuleDetailsTypeDef,  # (1)
    CaseRuleDetailsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CaseRuleDetailsTypeDef](./type_defs.md#caseruledetailstypedef) 
2. See [:material-code-braces: CaseRuleDetailsOutputTypeDef](./type_defs.md#caseruledetailsoutputtypedef) 

## LayoutContentUnionTypeDef

```python
# LayoutContentUnionTypeDef Union usage example

from types_aiobotocore_connectcases.type_defs import LayoutContentUnionTypeDef


def get_value() -> LayoutContentUnionTypeDef:
    return ...


# LayoutContentUnionTypeDef definition

LayoutContentUnionTypeDef = Union[
    LayoutContentTypeDef,  # (1)
    LayoutContentOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef) 
2. See [:material-code-braces: LayoutContentOutputTypeDef](./type_defs.md#layoutcontentoutputtypedef) 



## AuditEventFieldValueUnionTypeDef

```python
# AuditEventFieldValueUnionTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import AuditEventFieldValueUnionTypeDef


def get_value() -> AuditEventFieldValueUnionTypeDef:
    return {
        "booleanValue": ...,
    }


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
# UserUnionTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import UserUnionTypeDef


def get_value() -> UserUnionTypeDef:
    return {
        "userArn": ...,
    }


# UserUnionTypeDef definition

class UserUnionTypeDef(TypedDict):
    userArn: NotRequired[str],
```

## CaseRuleIdentifierTypeDef

```python
# CaseRuleIdentifierTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseRuleIdentifierTypeDef


def get_value() -> CaseRuleIdentifierTypeDef:
    return {
        "id": ...,
    }


# CaseRuleIdentifierTypeDef definition

class CaseRuleIdentifierTypeDef(TypedDict):
    id: str,
```

## CaseRuleErrorTypeDef

```python
# CaseRuleErrorTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseRuleErrorTypeDef


def get_value() -> CaseRuleErrorTypeDef:
    return {
        "errorCode": ...,
    }


# CaseRuleErrorTypeDef definition

class CaseRuleErrorTypeDef(TypedDict):
    errorCode: str,
    id: str,
    message: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## FieldIdentifierTypeDef

```python
# FieldIdentifierTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldIdentifierTypeDef


def get_value() -> FieldIdentifierTypeDef:
    return {
        "id": ...,
    }


# FieldIdentifierTypeDef definition

class FieldIdentifierTypeDef(TypedDict):
    id: str,
```

## FieldErrorTypeDef

```python
# FieldErrorTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldErrorTypeDef


def get_value() -> FieldErrorTypeDef:
    return {
        "errorCode": ...,
    }


# FieldErrorTypeDef definition

class FieldErrorTypeDef(TypedDict):
    errorCode: str,
    id: str,
    message: NotRequired[str],
```

## GetFieldResponseTypeDef

```python
# GetFieldResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetFieldResponseTypeDef


def get_value() -> GetFieldResponseTypeDef:
    return {
        "createdTime": ...,
    }


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
## FieldOptionTypeDef

```python
# FieldOptionTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldOptionTypeDef


def get_value() -> FieldOptionTypeDef:
    return {
        "active": ...,
    }


# FieldOptionTypeDef definition

class FieldOptionTypeDef(TypedDict):
    active: bool,
    name: str,
    value: str,
```

## FieldOptionErrorTypeDef

```python
# FieldOptionErrorTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldOptionErrorTypeDef


def get_value() -> FieldOptionErrorTypeDef:
    return {
        "errorCode": ...,
    }


# FieldOptionErrorTypeDef definition

class FieldOptionErrorTypeDef(TypedDict):
    errorCode: str,
    message: str,
    value: str,
```

## OperandOneTypeDef

```python
# OperandOneTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import OperandOneTypeDef


def get_value() -> OperandOneTypeDef:
    return {
        "fieldId": ...,
    }


# OperandOneTypeDef definition

class OperandOneTypeDef(TypedDict):
    fieldId: NotRequired[str],
```

## OperandTwoOutputTypeDef

```python
# OperandTwoOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import OperandTwoOutputTypeDef


def get_value() -> OperandTwoOutputTypeDef:
    return {
        "booleanValue": ...,
    }


# OperandTwoOutputTypeDef definition

class OperandTwoOutputTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    emptyValue: NotRequired[Dict[str, Any]],
    stringValue: NotRequired[str],
```

## OperandTwoTypeDef

```python
# OperandTwoTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import OperandTwoTypeDef


def get_value() -> OperandTwoTypeDef:
    return {
        "booleanValue": ...,
    }


# OperandTwoTypeDef definition

class OperandTwoTypeDef(TypedDict):
    booleanValue: NotRequired[bool],
    doubleValue: NotRequired[float],
    emptyValue: NotRequired[Mapping[str, Any]],
    stringValue: NotRequired[str],
```

## CaseRuleSummaryTypeDef

```python
# CaseRuleSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseRuleSummaryTypeDef


def get_value() -> CaseRuleSummaryTypeDef:
    return {
        "caseRuleArn": ...,
    }


# CaseRuleSummaryTypeDef definition

class CaseRuleSummaryTypeDef(TypedDict):
    caseRuleArn: str,
    caseRuleId: str,
    name: str,
    ruleType: RuleTypeType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
## CaseSummaryTypeDef

```python
# CaseSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseSummaryTypeDef


def get_value() -> CaseSummaryTypeDef:
    return {
        "caseId": ...,
    }


# CaseSummaryTypeDef definition

class CaseSummaryTypeDef(TypedDict):
    caseId: str,
    templateId: str,
```

## CommentContentTypeDef

```python
# CommentContentTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CommentContentTypeDef


def get_value() -> CommentContentTypeDef:
    return {
        "body": ...,
    }


# CommentContentTypeDef definition

class CommentContentTypeDef(TypedDict):
    body: str,
    contentType: CommentBodyTextTypeType,  # (1)
```

1. See [:material-code-brackets: CommentBodyTextTypeType](./literals.md#commentbodytexttypetype) 
## ContactContentTypeDef

```python
# ContactContentTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ContactContentTypeDef


def get_value() -> ContactContentTypeDef:
    return {
        "channel": ...,
    }


# ContactContentTypeDef definition

class ContactContentTypeDef(TypedDict):
    channel: str,
    connectedToSystemTime: datetime,
    contactArn: str,
```

## ContactFilterTypeDef

```python
# ContactFilterTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ContactFilterTypeDef


def get_value() -> ContactFilterTypeDef:
    return {
        "channel": ...,
    }


# ContactFilterTypeDef definition

class ContactFilterTypeDef(TypedDict):
    channel: NotRequired[Sequence[str]],
    contactArn: NotRequired[str],
```

## ContactTypeDef

```python
# ContactTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ContactTypeDef


def get_value() -> ContactTypeDef:
    return {
        "contactArn": ...,
    }


# ContactTypeDef definition

class ContactTypeDef(TypedDict):
    contactArn: str,
```

## CreateDomainRequestTypeDef

```python
# CreateDomainRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateDomainRequestTypeDef


def get_value() -> CreateDomainRequestTypeDef:
    return {
        "name": ...,
    }


# CreateDomainRequestTypeDef definition

class CreateDomainRequestTypeDef(TypedDict):
    name: str,
```

## CreateFieldRequestTypeDef

```python
# CreateFieldRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateFieldRequestTypeDef


def get_value() -> CreateFieldRequestTypeDef:
    return {
        "domainId": ...,
    }


# CreateFieldRequestTypeDef definition

class CreateFieldRequestTypeDef(TypedDict):
    domainId: str,
    name: str,
    type: FieldTypeType,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-brackets: FieldTypeType](./literals.md#fieldtypetype) 
## LayoutConfigurationTypeDef

```python
# LayoutConfigurationTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import LayoutConfigurationTypeDef


def get_value() -> LayoutConfigurationTypeDef:
    return {
        "defaultLayout": ...,
    }


# LayoutConfigurationTypeDef definition

class LayoutConfigurationTypeDef(TypedDict):
    defaultLayout: NotRequired[str],
```

## RequiredFieldTypeDef

```python
# RequiredFieldTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import RequiredFieldTypeDef


def get_value() -> RequiredFieldTypeDef:
    return {
        "fieldId": ...,
    }


# RequiredFieldTypeDef definition

class RequiredFieldTypeDef(TypedDict):
    fieldId: str,
```

## TemplateRuleTypeDef

```python
# TemplateRuleTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import TemplateRuleTypeDef


def get_value() -> TemplateRuleTypeDef:
    return {
        "caseRuleId": ...,
    }


# TemplateRuleTypeDef definition

class TemplateRuleTypeDef(TypedDict):
    caseRuleId: str,
    fieldId: str,
```

## DeleteCaseRuleRequestTypeDef

```python
# DeleteCaseRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import DeleteCaseRuleRequestTypeDef


def get_value() -> DeleteCaseRuleRequestTypeDef:
    return {
        "caseRuleId": ...,
    }


# DeleteCaseRuleRequestTypeDef definition

class DeleteCaseRuleRequestTypeDef(TypedDict):
    caseRuleId: str,
    domainId: str,
```

## DeleteDomainRequestTypeDef

```python
# DeleteDomainRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import DeleteDomainRequestTypeDef


def get_value() -> DeleteDomainRequestTypeDef:
    return {
        "domainId": ...,
    }


# DeleteDomainRequestTypeDef definition

class DeleteDomainRequestTypeDef(TypedDict):
    domainId: str,
```

## DeleteFieldRequestTypeDef

```python
# DeleteFieldRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import DeleteFieldRequestTypeDef


def get_value() -> DeleteFieldRequestTypeDef:
    return {
        "domainId": ...,
    }


# DeleteFieldRequestTypeDef definition

class DeleteFieldRequestTypeDef(TypedDict):
    domainId: str,
    fieldId: str,
```

## DeleteLayoutRequestTypeDef

```python
# DeleteLayoutRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import DeleteLayoutRequestTypeDef


def get_value() -> DeleteLayoutRequestTypeDef:
    return {
        "domainId": ...,
    }


# DeleteLayoutRequestTypeDef definition

class DeleteLayoutRequestTypeDef(TypedDict):
    domainId: str,
    layoutId: str,
```

## DeleteTemplateRequestTypeDef

```python
# DeleteTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import DeleteTemplateRequestTypeDef


def get_value() -> DeleteTemplateRequestTypeDef:
    return {
        "domainId": ...,
    }


# DeleteTemplateRequestTypeDef definition

class DeleteTemplateRequestTypeDef(TypedDict):
    domainId: str,
    templateId: str,
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import DomainSummaryTypeDef


def get_value() -> DomainSummaryTypeDef:
    return {
        "domainArn": ...,
    }


# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    domainArn: str,
    domainId: str,
    name: str,
```

## RelatedItemEventIncludedDataTypeDef

```python
# RelatedItemEventIncludedDataTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import RelatedItemEventIncludedDataTypeDef


def get_value() -> RelatedItemEventIncludedDataTypeDef:
    return {
        "includeContent": ...,
    }


# RelatedItemEventIncludedDataTypeDef definition

class RelatedItemEventIncludedDataTypeDef(TypedDict):
    includeContent: bool,
```

## FieldItemTypeDef

```python
# FieldItemTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldItemTypeDef


def get_value() -> FieldItemTypeDef:
    return {
        "id": ...,
    }


# FieldItemTypeDef definition

class FieldItemTypeDef(TypedDict):
    id: str,
```

## FieldSummaryTypeDef

```python
# FieldSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldSummaryTypeDef


def get_value() -> FieldSummaryTypeDef:
    return {
        "fieldArn": ...,
    }


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
# FieldValueUnionOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldValueUnionOutputTypeDef


def get_value() -> FieldValueUnionOutputTypeDef:
    return {
        "booleanValue": ...,
    }


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
# FieldValueUnionTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldValueUnionTypeDef


def get_value() -> FieldValueUnionTypeDef:
    return {
        "booleanValue": ...,
    }


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
# FileContentTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FileContentTypeDef


def get_value() -> FileContentTypeDef:
    return {
        "fileArn": ...,
    }


# FileContentTypeDef definition

class FileContentTypeDef(TypedDict):
    fileArn: str,
```

## FileFilterTypeDef

```python
# FileFilterTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FileFilterTypeDef


def get_value() -> FileFilterTypeDef:
    return {
        "fileArn": ...,
    }


# FileFilterTypeDef definition

class FileFilterTypeDef(TypedDict):
    fileArn: NotRequired[str],
```

## GetCaseAuditEventsRequestTypeDef

```python
# GetCaseAuditEventsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetCaseAuditEventsRequestTypeDef


def get_value() -> GetCaseAuditEventsRequestTypeDef:
    return {
        "caseId": ...,
    }


# GetCaseAuditEventsRequestTypeDef definition

class GetCaseAuditEventsRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## GetCaseEventConfigurationRequestTypeDef

```python
# GetCaseEventConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetCaseEventConfigurationRequestTypeDef


def get_value() -> GetCaseEventConfigurationRequestTypeDef:
    return {
        "domainId": ...,
    }


# GetCaseEventConfigurationRequestTypeDef definition

class GetCaseEventConfigurationRequestTypeDef(TypedDict):
    domainId: str,
```

## GetDomainRequestTypeDef

```python
# GetDomainRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetDomainRequestTypeDef


def get_value() -> GetDomainRequestTypeDef:
    return {
        "domainId": ...,
    }


# GetDomainRequestTypeDef definition

class GetDomainRequestTypeDef(TypedDict):
    domainId: str,
```

## GetLayoutRequestTypeDef

```python
# GetLayoutRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetLayoutRequestTypeDef


def get_value() -> GetLayoutRequestTypeDef:
    return {
        "domainId": ...,
    }


# GetLayoutRequestTypeDef definition

class GetLayoutRequestTypeDef(TypedDict):
    domainId: str,
    layoutId: str,
```

## GetTemplateRequestTypeDef

```python
# GetTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetTemplateRequestTypeDef


def get_value() -> GetTemplateRequestTypeDef:
    return {
        "domainId": ...,
    }


# GetTemplateRequestTypeDef definition

class GetTemplateRequestTypeDef(TypedDict):
    domainId: str,
    templateId: str,
```

## LayoutSummaryTypeDef

```python
# LayoutSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import LayoutSummaryTypeDef


def get_value() -> LayoutSummaryTypeDef:
    return {
        "layoutArn": ...,
    }


# LayoutSummaryTypeDef definition

class LayoutSummaryTypeDef(TypedDict):
    layoutArn: str,
    layoutId: str,
    name: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListCaseRulesRequestTypeDef

```python
# ListCaseRulesRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListCaseRulesRequestTypeDef


def get_value() -> ListCaseRulesRequestTypeDef:
    return {
        "domainId": ...,
    }


# ListCaseRulesRequestTypeDef definition

class ListCaseRulesRequestTypeDef(TypedDict):
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListCasesForContactRequestTypeDef

```python
# ListCasesForContactRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListCasesForContactRequestTypeDef


def get_value() -> ListCasesForContactRequestTypeDef:
    return {
        "contactArn": ...,
    }


# ListCasesForContactRequestTypeDef definition

class ListCasesForContactRequestTypeDef(TypedDict):
    contactArn: str,
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDomainsRequestTypeDef

```python
# ListDomainsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListDomainsRequestTypeDef


def get_value() -> ListDomainsRequestTypeDef:
    return {
        "maxResults": ...,
    }


# ListDomainsRequestTypeDef definition

class ListDomainsRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListFieldOptionsRequestTypeDef

```python
# ListFieldOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListFieldOptionsRequestTypeDef


def get_value() -> ListFieldOptionsRequestTypeDef:
    return {
        "domainId": ...,
    }


# ListFieldOptionsRequestTypeDef definition

class ListFieldOptionsRequestTypeDef(TypedDict):
    domainId: str,
    fieldId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    values: NotRequired[Sequence[str]],
```

## ListFieldsRequestTypeDef

```python
# ListFieldsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListFieldsRequestTypeDef


def get_value() -> ListFieldsRequestTypeDef:
    return {
        "domainId": ...,
    }


# ListFieldsRequestTypeDef definition

class ListFieldsRequestTypeDef(TypedDict):
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListLayoutsRequestTypeDef

```python
# ListLayoutsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListLayoutsRequestTypeDef


def get_value() -> ListLayoutsRequestTypeDef:
    return {
        "domainId": ...,
    }


# ListLayoutsRequestTypeDef definition

class ListLayoutsRequestTypeDef(TypedDict):
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "arn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    arn: str,
```

## ListTemplatesRequestTypeDef

```python
# ListTemplatesRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListTemplatesRequestTypeDef


def get_value() -> ListTemplatesRequestTypeDef:
    return {
        "domainId": ...,
    }


# ListTemplatesRequestTypeDef definition

class ListTemplatesRequestTypeDef(TypedDict):
    domainId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[Sequence[TemplateStatusType]],  # (1)
```

1. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## TemplateSummaryTypeDef

```python
# TemplateSummaryTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import TemplateSummaryTypeDef


def get_value() -> TemplateSummaryTypeDef:
    return {
        "name": ...,
    }


# TemplateSummaryTypeDef definition

class TemplateSummaryTypeDef(TypedDict):
    name: str,
    status: TemplateStatusType,  # (1)
    templateArn: str,
    templateId: str,
```

1. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## SortTypeDef

```python
# SortTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SortTypeDef


def get_value() -> SortTypeDef:
    return {
        "fieldId": ...,
    }


# SortTypeDef definition

class SortTypeDef(TypedDict):
    fieldId: str,
    sortOrder: OrderType,  # (1)
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "arn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    arn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "arn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    arn: str,
    tagKeys: Sequence[str],
```

## UpdateFieldRequestTypeDef

```python
# UpdateFieldRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import UpdateFieldRequestTypeDef


def get_value() -> UpdateFieldRequestTypeDef:
    return {
        "domainId": ...,
    }


# UpdateFieldRequestTypeDef definition

class UpdateFieldRequestTypeDef(TypedDict):
    domainId: str,
    fieldId: str,
    description: NotRequired[str],
    name: NotRequired[str],
```

## AuditEventFieldTypeDef

```python
# AuditEventFieldTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import AuditEventFieldTypeDef


def get_value() -> AuditEventFieldTypeDef:
    return {
        "eventFieldId": ...,
    }


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
# AuditEventPerformedByTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import AuditEventPerformedByTypeDef


def get_value() -> AuditEventPerformedByTypeDef:
    return {
        "iamPrincipalArn": ...,
    }


# AuditEventPerformedByTypeDef definition

class AuditEventPerformedByTypeDef(TypedDict):
    iamPrincipalArn: str,
    user: NotRequired[UserUnionTypeDef],  # (1)
```

1. See [:material-code-braces: UserUnionTypeDef](./type_defs.md#useruniontypedef) 
## BatchGetCaseRuleRequestTypeDef

```python
# BatchGetCaseRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BatchGetCaseRuleRequestTypeDef


def get_value() -> BatchGetCaseRuleRequestTypeDef:
    return {
        "caseRules": ...,
    }


# BatchGetCaseRuleRequestTypeDef definition

class BatchGetCaseRuleRequestTypeDef(TypedDict):
    caseRules: Sequence[CaseRuleIdentifierTypeDef],  # (1)
    domainId: str,
```

1. See [:material-code-braces: CaseRuleIdentifierTypeDef](./type_defs.md#caseruleidentifiertypedef) 
## CreateCaseResponseTypeDef

```python
# CreateCaseResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateCaseResponseTypeDef


def get_value() -> CreateCaseResponseTypeDef:
    return {
        "caseArn": ...,
    }


# CreateCaseResponseTypeDef definition

class CreateCaseResponseTypeDef(TypedDict):
    caseArn: str,
    caseId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseRuleResponseTypeDef

```python
# CreateCaseRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateCaseRuleResponseTypeDef


def get_value() -> CreateCaseRuleResponseTypeDef:
    return {
        "caseRuleArn": ...,
    }


# CreateCaseRuleResponseTypeDef definition

class CreateCaseRuleResponseTypeDef(TypedDict):
    caseRuleArn: str,
    caseRuleId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainResponseTypeDef

```python
# CreateDomainResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateDomainResponseTypeDef


def get_value() -> CreateDomainResponseTypeDef:
    return {
        "domainArn": ...,
    }


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
# CreateFieldResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateFieldResponseTypeDef


def get_value() -> CreateFieldResponseTypeDef:
    return {
        "fieldArn": ...,
    }


# CreateFieldResponseTypeDef definition

class CreateFieldResponseTypeDef(TypedDict):
    fieldArn: str,
    fieldId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLayoutResponseTypeDef

```python
# CreateLayoutResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateLayoutResponseTypeDef


def get_value() -> CreateLayoutResponseTypeDef:
    return {
        "layoutArn": ...,
    }


# CreateLayoutResponseTypeDef definition

class CreateLayoutResponseTypeDef(TypedDict):
    layoutArn: str,
    layoutId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRelatedItemResponseTypeDef

```python
# CreateRelatedItemResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateRelatedItemResponseTypeDef


def get_value() -> CreateRelatedItemResponseTypeDef:
    return {
        "relatedItemArn": ...,
    }


# CreateRelatedItemResponseTypeDef definition

class CreateRelatedItemResponseTypeDef(TypedDict):
    relatedItemArn: str,
    relatedItemId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateResponseTypeDef

```python
# CreateTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateTemplateResponseTypeDef


def get_value() -> CreateTemplateResponseTypeDef:
    return {
        "templateArn": ...,
    }


# CreateTemplateResponseTypeDef definition

class CreateTemplateResponseTypeDef(TypedDict):
    templateArn: str,
    templateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainResponseTypeDef

```python
# GetDomainResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetDomainResponseTypeDef


def get_value() -> GetDomainResponseTypeDef:
    return {
        "createdTime": ...,
    }


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
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetFieldRequestTypeDef

```python
# BatchGetFieldRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BatchGetFieldRequestTypeDef


def get_value() -> BatchGetFieldRequestTypeDef:
    return {
        "domainId": ...,
    }


# BatchGetFieldRequestTypeDef definition

class BatchGetFieldRequestTypeDef(TypedDict):
    domainId: str,
    fields: Sequence[FieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## CaseEventIncludedDataOutputTypeDef

```python
# CaseEventIncludedDataOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseEventIncludedDataOutputTypeDef


def get_value() -> CaseEventIncludedDataOutputTypeDef:
    return {
        "fields": ...,
    }


# CaseEventIncludedDataOutputTypeDef definition

class CaseEventIncludedDataOutputTypeDef(TypedDict):
    fields: List[FieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## CaseEventIncludedDataTypeDef

```python
# CaseEventIncludedDataTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseEventIncludedDataTypeDef


def get_value() -> CaseEventIncludedDataTypeDef:
    return {
        "fields": ...,
    }


# CaseEventIncludedDataTypeDef definition

class CaseEventIncludedDataTypeDef(TypedDict):
    fields: Sequence[FieldIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## GetCaseRequestTypeDef

```python
# GetCaseRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetCaseRequestTypeDef


def get_value() -> GetCaseRequestTypeDef:
    return {
        "caseId": ...,
    }


# GetCaseRequestTypeDef definition

class GetCaseRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    fields: Sequence[FieldIdentifierTypeDef],  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef) 
## BatchGetFieldResponseTypeDef

```python
# BatchGetFieldResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BatchGetFieldResponseTypeDef


def get_value() -> BatchGetFieldResponseTypeDef:
    return {
        "errors": ...,
    }


# BatchGetFieldResponseTypeDef definition

class BatchGetFieldResponseTypeDef(TypedDict):
    errors: List[FieldErrorTypeDef],  # (1)
    fields: List[GetFieldResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FieldErrorTypeDef](./type_defs.md#fielderrortypedef) 
2. See [:material-code-braces: GetFieldResponseTypeDef](./type_defs.md#getfieldresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutFieldOptionsRequestTypeDef

```python
# BatchPutFieldOptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BatchPutFieldOptionsRequestTypeDef


def get_value() -> BatchPutFieldOptionsRequestTypeDef:
    return {
        "domainId": ...,
    }


# BatchPutFieldOptionsRequestTypeDef definition

class BatchPutFieldOptionsRequestTypeDef(TypedDict):
    domainId: str,
    fieldId: str,
    options: Sequence[FieldOptionTypeDef],  # (1)
```

1. See [:material-code-braces: FieldOptionTypeDef](./type_defs.md#fieldoptiontypedef) 
## ListFieldOptionsResponseTypeDef

```python
# ListFieldOptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListFieldOptionsResponseTypeDef


def get_value() -> ListFieldOptionsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# BatchPutFieldOptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BatchPutFieldOptionsResponseTypeDef


def get_value() -> BatchPutFieldOptionsResponseTypeDef:
    return {
        "errors": ...,
    }


# BatchPutFieldOptionsResponseTypeDef definition

class BatchPutFieldOptionsResponseTypeDef(TypedDict):
    errors: List[FieldOptionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FieldOptionErrorTypeDef](./type_defs.md#fieldoptionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BooleanOperandsOutputTypeDef

```python
# BooleanOperandsOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BooleanOperandsOutputTypeDef


def get_value() -> BooleanOperandsOutputTypeDef:
    return {
        "operandOne": ...,
    }


# BooleanOperandsOutputTypeDef definition

class BooleanOperandsOutputTypeDef(TypedDict):
    operandOne: OperandOneTypeDef,  # (1)
    operandTwo: OperandTwoOutputTypeDef,  # (2)
    result: bool,
```

1. See [:material-code-braces: OperandOneTypeDef](./type_defs.md#operandonetypedef) 
2. See [:material-code-braces: OperandTwoOutputTypeDef](./type_defs.md#operandtwooutputtypedef) 
## BooleanOperandsTypeDef

```python
# BooleanOperandsTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BooleanOperandsTypeDef


def get_value() -> BooleanOperandsTypeDef:
    return {
        "operandOne": ...,
    }


# BooleanOperandsTypeDef definition

class BooleanOperandsTypeDef(TypedDict):
    operandOne: OperandOneTypeDef,  # (1)
    operandTwo: OperandTwoTypeDef,  # (2)
    result: bool,
```

1. See [:material-code-braces: OperandOneTypeDef](./type_defs.md#operandonetypedef) 
2. See [:material-code-braces: OperandTwoTypeDef](./type_defs.md#operandtwotypedef) 
## ListCaseRulesResponseTypeDef

```python
# ListCaseRulesResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListCaseRulesResponseTypeDef


def get_value() -> ListCaseRulesResponseTypeDef:
    return {
        "caseRules": ...,
    }


# ListCaseRulesResponseTypeDef definition

class ListCaseRulesResponseTypeDef(TypedDict):
    caseRules: List[CaseRuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CaseRuleSummaryTypeDef](./type_defs.md#caserulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCasesForContactResponseTypeDef

```python
# ListCasesForContactResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListCasesForContactResponseTypeDef


def get_value() -> ListCasesForContactResponseTypeDef:
    return {
        "cases": ...,
    }


# ListCasesForContactResponseTypeDef definition

class ListCasesForContactResponseTypeDef(TypedDict):
    cases: List[CaseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CaseSummaryTypeDef](./type_defs.md#casesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateRequestTypeDef

```python
# CreateTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateTemplateRequestTypeDef


def get_value() -> CreateTemplateRequestTypeDef:
    return {
        "domainId": ...,
    }


# CreateTemplateRequestTypeDef definition

class CreateTemplateRequestTypeDef(TypedDict):
    domainId: str,
    name: str,
    description: NotRequired[str],
    layoutConfiguration: NotRequired[LayoutConfigurationTypeDef],  # (1)
    requiredFields: NotRequired[Sequence[RequiredFieldTypeDef]],  # (2)
    rules: NotRequired[Sequence[TemplateRuleTypeDef]],  # (3)
    status: NotRequired[TemplateStatusType],  # (4)
```

1. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
2. See [:material-code-braces: RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef) 
3. See [:material-code-braces: TemplateRuleTypeDef](./type_defs.md#templateruletypedef) 
4. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## GetTemplateResponseTypeDef

```python
# GetTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetTemplateResponseTypeDef


def get_value() -> GetTemplateResponseTypeDef:
    return {
        "createdTime": ...,
    }


# GetTemplateResponseTypeDef definition

class GetTemplateResponseTypeDef(TypedDict):
    createdTime: datetime,
    deleted: bool,
    description: str,
    lastModifiedTime: datetime,
    layoutConfiguration: LayoutConfigurationTypeDef,  # (1)
    name: str,
    requiredFields: List[RequiredFieldTypeDef],  # (2)
    rules: List[TemplateRuleTypeDef],  # (3)
    status: TemplateStatusType,  # (4)
    tags: Dict[str, str],
    templateArn: str,
    templateId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
2. See [:material-code-braces: RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef) 
3. See [:material-code-braces: TemplateRuleTypeDef](./type_defs.md#templateruletypedef) 
4. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplateRequestTypeDef

```python
# UpdateTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import UpdateTemplateRequestTypeDef


def get_value() -> UpdateTemplateRequestTypeDef:
    return {
        "domainId": ...,
    }


# UpdateTemplateRequestTypeDef definition

class UpdateTemplateRequestTypeDef(TypedDict):
    domainId: str,
    templateId: str,
    description: NotRequired[str],
    layoutConfiguration: NotRequired[LayoutConfigurationTypeDef],  # (1)
    name: NotRequired[str],
    requiredFields: NotRequired[Sequence[RequiredFieldTypeDef]],  # (2)
    rules: NotRequired[Sequence[TemplateRuleTypeDef]],  # (3)
    status: NotRequired[TemplateStatusType],  # (4)
```

1. See [:material-code-braces: LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef) 
2. See [:material-code-braces: RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef) 
3. See [:material-code-braces: TemplateRuleTypeDef](./type_defs.md#templateruletypedef) 
4. See [:material-code-brackets: TemplateStatusType](./literals.md#templatestatustype) 
## ListDomainsResponseTypeDef

```python
# ListDomainsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListDomainsResponseTypeDef


def get_value() -> ListDomainsResponseTypeDef:
    return {
        "domains": ...,
    }


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
# FieldGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldGroupOutputTypeDef


def get_value() -> FieldGroupOutputTypeDef:
    return {
        "fields": ...,
    }


# FieldGroupOutputTypeDef definition

class FieldGroupOutputTypeDef(TypedDict):
    fields: List[FieldItemTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: FieldItemTypeDef](./type_defs.md#fielditemtypedef) 
## FieldGroupTypeDef

```python
# FieldGroupTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldGroupTypeDef


def get_value() -> FieldGroupTypeDef:
    return {
        "fields": ...,
    }


# FieldGroupTypeDef definition

class FieldGroupTypeDef(TypedDict):
    fields: Sequence[FieldItemTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: FieldItemTypeDef](./type_defs.md#fielditemtypedef) 
## ListFieldsResponseTypeDef

```python
# ListFieldsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListFieldsResponseTypeDef


def get_value() -> ListFieldsResponseTypeDef:
    return {
        "fields": ...,
    }


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
# FieldValueOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldValueOutputTypeDef


def get_value() -> FieldValueOutputTypeDef:
    return {
        "id": ...,
    }


# FieldValueOutputTypeDef definition

class FieldValueOutputTypeDef(TypedDict):
    id: str,
    value: FieldValueUnionOutputTypeDef,  # (1)
```

1. See [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 
## RelatedItemContentTypeDef

```python
# RelatedItemContentTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import RelatedItemContentTypeDef


def get_value() -> RelatedItemContentTypeDef:
    return {
        "comment": ...,
    }


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
# RelatedItemInputContentTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import RelatedItemInputContentTypeDef


def get_value() -> RelatedItemInputContentTypeDef:
    return {
        "comment": ...,
    }


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
# RelatedItemTypeFilterTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import RelatedItemTypeFilterTypeDef


def get_value() -> RelatedItemTypeFilterTypeDef:
    return {
        "comment": ...,
    }


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
# ListLayoutsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListLayoutsResponseTypeDef


def get_value() -> ListLayoutsResponseTypeDef:
    return {
        "layouts": ...,
    }


# ListLayoutsResponseTypeDef definition

class ListLayoutsResponseTypeDef(TypedDict):
    layouts: List[LayoutSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LayoutSummaryTypeDef](./type_defs.md#layoutsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCaseRulesRequestPaginateTypeDef

```python
# ListCaseRulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListCaseRulesRequestPaginateTypeDef


def get_value() -> ListCaseRulesRequestPaginateTypeDef:
    return {
        "domainId": ...,
    }


# ListCaseRulesRequestPaginateTypeDef definition

class ListCaseRulesRequestPaginateTypeDef(TypedDict):
    domainId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTemplatesResponseTypeDef

```python
# ListTemplatesResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import ListTemplatesResponseTypeDef


def get_value() -> ListTemplatesResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# AuditEventTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import AuditEventTypeDef


def get_value() -> AuditEventTypeDef:
    return {
        "eventId": ...,
    }


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
# EventIncludedDataOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import EventIncludedDataOutputTypeDef


def get_value() -> EventIncludedDataOutputTypeDef:
    return {
        "caseData": ...,
    }


# EventIncludedDataOutputTypeDef definition

class EventIncludedDataOutputTypeDef(TypedDict):
    caseData: NotRequired[CaseEventIncludedDataOutputTypeDef],  # (1)
    relatedItemData: NotRequired[RelatedItemEventIncludedDataTypeDef],  # (2)
```

1. See [:material-code-braces: CaseEventIncludedDataOutputTypeDef](./type_defs.md#caseeventincludeddataoutputtypedef) 
2. See [:material-code-braces: RelatedItemEventIncludedDataTypeDef](./type_defs.md#relateditemeventincludeddatatypedef) 
## EventIncludedDataTypeDef

```python
# EventIncludedDataTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import EventIncludedDataTypeDef


def get_value() -> EventIncludedDataTypeDef:
    return {
        "caseData": ...,
    }


# EventIncludedDataTypeDef definition

class EventIncludedDataTypeDef(TypedDict):
    caseData: NotRequired[CaseEventIncludedDataTypeDef],  # (1)
    relatedItemData: NotRequired[RelatedItemEventIncludedDataTypeDef],  # (2)
```

1. See [:material-code-braces: CaseEventIncludedDataTypeDef](./type_defs.md#caseeventincludeddatatypedef) 
2. See [:material-code-braces: RelatedItemEventIncludedDataTypeDef](./type_defs.md#relateditemeventincludeddatatypedef) 
## BooleanConditionOutputTypeDef

```python
# BooleanConditionOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BooleanConditionOutputTypeDef


def get_value() -> BooleanConditionOutputTypeDef:
    return {
        "equalTo": ...,
    }


# BooleanConditionOutputTypeDef definition

class BooleanConditionOutputTypeDef(TypedDict):
    equalTo: NotRequired[BooleanOperandsOutputTypeDef],  # (1)
    notEqualTo: NotRequired[BooleanOperandsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: BooleanOperandsOutputTypeDef](./type_defs.md#booleanoperandsoutputtypedef) 
2. See [:material-code-braces: BooleanOperandsOutputTypeDef](./type_defs.md#booleanoperandsoutputtypedef) 
## BooleanConditionTypeDef

```python
# BooleanConditionTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BooleanConditionTypeDef


def get_value() -> BooleanConditionTypeDef:
    return {
        "equalTo": ...,
    }


# BooleanConditionTypeDef definition

class BooleanConditionTypeDef(TypedDict):
    equalTo: NotRequired[BooleanOperandsTypeDef],  # (1)
    notEqualTo: NotRequired[BooleanOperandsTypeDef],  # (1)
```

1. See [:material-code-braces: BooleanOperandsTypeDef](./type_defs.md#booleanoperandstypedef) 
2. See [:material-code-braces: BooleanOperandsTypeDef](./type_defs.md#booleanoperandstypedef) 
## SectionOutputTypeDef

```python
# SectionOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SectionOutputTypeDef


def get_value() -> SectionOutputTypeDef:
    return {
        "fieldGroup": ...,
    }


# SectionOutputTypeDef definition

class SectionOutputTypeDef(TypedDict):
    fieldGroup: NotRequired[FieldGroupOutputTypeDef],  # (1)
```

1. See [:material-code-braces: FieldGroupOutputTypeDef](./type_defs.md#fieldgroupoutputtypedef) 
## SectionTypeDef

```python
# SectionTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SectionTypeDef


def get_value() -> SectionTypeDef:
    return {
        "fieldGroup": ...,
    }


# SectionTypeDef definition

class SectionTypeDef(TypedDict):
    fieldGroup: NotRequired[FieldGroupTypeDef],  # (1)
```

1. See [:material-code-braces: FieldGroupTypeDef](./type_defs.md#fieldgrouptypedef) 
## GetCaseResponseTypeDef

```python
# GetCaseResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetCaseResponseTypeDef


def get_value() -> GetCaseResponseTypeDef:
    return {
        "fields": ...,
    }


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
# SearchCasesResponseItemTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SearchCasesResponseItemTypeDef


def get_value() -> SearchCasesResponseItemTypeDef:
    return {
        "caseId": ...,
    }


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
# FieldValueTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldValueTypeDef


def get_value() -> FieldValueTypeDef:
    return {
        "id": ...,
    }


# FieldValueTypeDef definition

class FieldValueTypeDef(TypedDict):
    id: str,
    value: FieldValueUnionUnionTypeDef,  # (1)
```

1. See [:material-code-braces: FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef) [:material-code-braces: FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef) 
## SearchRelatedItemsResponseItemTypeDef

```python
# SearchRelatedItemsResponseItemTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SearchRelatedItemsResponseItemTypeDef


def get_value() -> SearchRelatedItemsResponseItemTypeDef:
    return {
        "associationTime": ...,
    }


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
## CreateRelatedItemRequestTypeDef

```python
# CreateRelatedItemRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateRelatedItemRequestTypeDef


def get_value() -> CreateRelatedItemRequestTypeDef:
    return {
        "caseId": ...,
    }


# CreateRelatedItemRequestTypeDef definition

class CreateRelatedItemRequestTypeDef(TypedDict):
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
# SearchRelatedItemsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SearchRelatedItemsRequestPaginateTypeDef


def get_value() -> SearchRelatedItemsRequestPaginateTypeDef:
    return {
        "caseId": ...,
    }


# SearchRelatedItemsRequestPaginateTypeDef definition

class SearchRelatedItemsRequestPaginateTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    filters: NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: RelatedItemTypeFilterTypeDef](./type_defs.md#relateditemtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchRelatedItemsRequestTypeDef

```python
# SearchRelatedItemsRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SearchRelatedItemsRequestTypeDef


def get_value() -> SearchRelatedItemsRequestTypeDef:
    return {
        "caseId": ...,
    }


# SearchRelatedItemsRequestTypeDef definition

class SearchRelatedItemsRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    filters: NotRequired[Sequence[RelatedItemTypeFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RelatedItemTypeFilterTypeDef](./type_defs.md#relateditemtypefiltertypedef) 
## GetCaseAuditEventsResponseTypeDef

```python
# GetCaseAuditEventsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetCaseAuditEventsResponseTypeDef


def get_value() -> GetCaseAuditEventsResponseTypeDef:
    return {
        "auditEvents": ...,
    }


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
# EventBridgeConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import EventBridgeConfigurationOutputTypeDef


def get_value() -> EventBridgeConfigurationOutputTypeDef:
    return {
        "enabled": ...,
    }


# EventBridgeConfigurationOutputTypeDef definition

class EventBridgeConfigurationOutputTypeDef(TypedDict):
    enabled: bool,
    includedData: NotRequired[EventIncludedDataOutputTypeDef],  # (1)
```

1. See [:material-code-braces: EventIncludedDataOutputTypeDef](./type_defs.md#eventincludeddataoutputtypedef) 
## EventBridgeConfigurationTypeDef

```python
# EventBridgeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import EventBridgeConfigurationTypeDef


def get_value() -> EventBridgeConfigurationTypeDef:
    return {
        "enabled": ...,
    }


# EventBridgeConfigurationTypeDef definition

class EventBridgeConfigurationTypeDef(TypedDict):
    enabled: bool,
    includedData: NotRequired[EventIncludedDataTypeDef],  # (1)
```

1. See [:material-code-braces: EventIncludedDataTypeDef](./type_defs.md#eventincludeddatatypedef) 
## RequiredCaseRuleOutputTypeDef

```python
# RequiredCaseRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import RequiredCaseRuleOutputTypeDef


def get_value() -> RequiredCaseRuleOutputTypeDef:
    return {
        "conditions": ...,
    }


# RequiredCaseRuleOutputTypeDef definition

class RequiredCaseRuleOutputTypeDef(TypedDict):
    conditions: List[BooleanConditionOutputTypeDef],  # (1)
    defaultValue: bool,
```

1. See [:material-code-braces: BooleanConditionOutputTypeDef](./type_defs.md#booleanconditionoutputtypedef) 
## RequiredCaseRuleTypeDef

```python
# RequiredCaseRuleTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import RequiredCaseRuleTypeDef


def get_value() -> RequiredCaseRuleTypeDef:
    return {
        "conditions": ...,
    }


# RequiredCaseRuleTypeDef definition

class RequiredCaseRuleTypeDef(TypedDict):
    conditions: Sequence[BooleanConditionTypeDef],  # (1)
    defaultValue: bool,
```

1. See [:material-code-braces: BooleanConditionTypeDef](./type_defs.md#booleanconditiontypedef) 
## LayoutSectionsOutputTypeDef

```python
# LayoutSectionsOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import LayoutSectionsOutputTypeDef


def get_value() -> LayoutSectionsOutputTypeDef:
    return {
        "sections": ...,
    }


# LayoutSectionsOutputTypeDef definition

class LayoutSectionsOutputTypeDef(TypedDict):
    sections: NotRequired[List[SectionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: SectionOutputTypeDef](./type_defs.md#sectionoutputtypedef) 
## LayoutSectionsTypeDef

```python
# LayoutSectionsTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import LayoutSectionsTypeDef


def get_value() -> LayoutSectionsTypeDef:
    return {
        "sections": ...,
    }


# LayoutSectionsTypeDef definition

class LayoutSectionsTypeDef(TypedDict):
    sections: NotRequired[Sequence[SectionTypeDef]],  # (1)
```

1. See [:material-code-braces: SectionTypeDef](./type_defs.md#sectiontypedef) 
## SearchCasesResponseTypeDef

```python
# SearchCasesResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SearchCasesResponseTypeDef


def get_value() -> SearchCasesResponseTypeDef:
    return {
        "cases": ...,
    }


# SearchCasesResponseTypeDef definition

class SearchCasesResponseTypeDef(TypedDict):
    cases: List[SearchCasesResponseItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchCasesResponseItemTypeDef](./type_defs.md#searchcasesresponseitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchRelatedItemsResponseTypeDef

```python
# SearchRelatedItemsResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SearchRelatedItemsResponseTypeDef


def get_value() -> SearchRelatedItemsResponseTypeDef:
    return {
        "nextToken": ...,
    }


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
# GetCaseEventConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetCaseEventConfigurationResponseTypeDef


def get_value() -> GetCaseEventConfigurationResponseTypeDef:
    return {
        "eventBridge": ...,
    }


# GetCaseEventConfigurationResponseTypeDef definition

class GetCaseEventConfigurationResponseTypeDef(TypedDict):
    eventBridge: EventBridgeConfigurationOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EventBridgeConfigurationOutputTypeDef](./type_defs.md#eventbridgeconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CaseRuleDetailsOutputTypeDef

```python
# CaseRuleDetailsOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseRuleDetailsOutputTypeDef


def get_value() -> CaseRuleDetailsOutputTypeDef:
    return {
        "required": ...,
    }


# CaseRuleDetailsOutputTypeDef definition

class CaseRuleDetailsOutputTypeDef(TypedDict):
    required: NotRequired[RequiredCaseRuleOutputTypeDef],  # (1)
```

1. See [:material-code-braces: RequiredCaseRuleOutputTypeDef](./type_defs.md#requiredcaseruleoutputtypedef) 
## CaseRuleDetailsTypeDef

```python
# CaseRuleDetailsTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseRuleDetailsTypeDef


def get_value() -> CaseRuleDetailsTypeDef:
    return {
        "required": ...,
    }


# CaseRuleDetailsTypeDef definition

class CaseRuleDetailsTypeDef(TypedDict):
    required: NotRequired[RequiredCaseRuleTypeDef],  # (1)
```

1. See [:material-code-braces: RequiredCaseRuleTypeDef](./type_defs.md#requiredcaseruletypedef) 
## BasicLayoutOutputTypeDef

```python
# BasicLayoutOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BasicLayoutOutputTypeDef


def get_value() -> BasicLayoutOutputTypeDef:
    return {
        "moreInfo": ...,
    }


# BasicLayoutOutputTypeDef definition

class BasicLayoutOutputTypeDef(TypedDict):
    moreInfo: NotRequired[LayoutSectionsOutputTypeDef],  # (1)
    topPanel: NotRequired[LayoutSectionsOutputTypeDef],  # (1)
```

1. See [:material-code-braces: LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef) 
2. See [:material-code-braces: LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef) 
## BasicLayoutTypeDef

```python
# BasicLayoutTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BasicLayoutTypeDef


def get_value() -> BasicLayoutTypeDef:
    return {
        "moreInfo": ...,
    }


# BasicLayoutTypeDef definition

class BasicLayoutTypeDef(TypedDict):
    moreInfo: NotRequired[LayoutSectionsTypeDef],  # (1)
    topPanel: NotRequired[LayoutSectionsTypeDef],  # (1)
```

1. See [:material-code-braces: LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef) 
2. See [:material-code-braces: LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef) 
## CreateCaseRequestTypeDef

```python
# CreateCaseRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateCaseRequestTypeDef


def get_value() -> CreateCaseRequestTypeDef:
    return {
        "domainId": ...,
    }


# CreateCaseRequestTypeDef definition

class CreateCaseRequestTypeDef(TypedDict):
    domainId: str,
    fields: Sequence[FieldValueUnionExtraTypeDef],  # (1)
    templateId: str,
    clientToken: NotRequired[str],
    performedBy: NotRequired[UserUnionTypeDef],  # (2)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
2. See [:material-code-braces: UserUnionTypeDef](./type_defs.md#useruniontypedef) 
## FieldFilterTypeDef

```python
# FieldFilterTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import FieldFilterTypeDef


def get_value() -> FieldFilterTypeDef:
    return {
        "contains": ...,
    }


# FieldFilterTypeDef definition

class FieldFilterTypeDef(TypedDict):
    contains: NotRequired[FieldValueUnionExtraTypeDef],  # (1)
    equalTo: NotRequired[FieldValueUnionExtraTypeDef],  # (1)
    greaterThan: NotRequired[FieldValueUnionExtraTypeDef],  # (1)
    greaterThanOrEqualTo: NotRequired[FieldValueUnionExtraTypeDef],  # (1)
    lessThan: NotRequired[FieldValueUnionExtraTypeDef],  # (1)
    lessThanOrEqualTo: NotRequired[FieldValueUnionExtraTypeDef],  # (1)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
2. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
3. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
4. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
5. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
6. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
## UpdateCaseRequestTypeDef

```python
# UpdateCaseRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import UpdateCaseRequestTypeDef


def get_value() -> UpdateCaseRequestTypeDef:
    return {
        "caseId": ...,
    }


# UpdateCaseRequestTypeDef definition

class UpdateCaseRequestTypeDef(TypedDict):
    caseId: str,
    domainId: str,
    fields: Sequence[FieldValueUnionExtraTypeDef],  # (1)
    performedBy: NotRequired[UserUnionTypeDef],  # (2)
```

1. See [:material-code-braces: FieldValueTypeDef](./type_defs.md#fieldvaluetypedef) [:material-code-braces: FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef) 
2. See [:material-code-braces: UserUnionTypeDef](./type_defs.md#useruniontypedef) 
## PutCaseEventConfigurationRequestTypeDef

```python
# PutCaseEventConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import PutCaseEventConfigurationRequestTypeDef


def get_value() -> PutCaseEventConfigurationRequestTypeDef:
    return {
        "domainId": ...,
    }


# PutCaseEventConfigurationRequestTypeDef definition

class PutCaseEventConfigurationRequestTypeDef(TypedDict):
    domainId: str,
    eventBridge: EventBridgeConfigurationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef) [:material-code-braces: EventBridgeConfigurationOutputTypeDef](./type_defs.md#eventbridgeconfigurationoutputtypedef) 
## GetCaseRuleResponseTypeDef

```python
# GetCaseRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetCaseRuleResponseTypeDef


def get_value() -> GetCaseRuleResponseTypeDef:
    return {
        "caseRuleArn": ...,
    }


# GetCaseRuleResponseTypeDef definition

class GetCaseRuleResponseTypeDef(TypedDict):
    caseRuleArn: str,
    caseRuleId: str,
    name: str,
    rule: CaseRuleDetailsOutputTypeDef,  # (1)
    createdTime: NotRequired[datetime],
    deleted: NotRequired[bool],
    description: NotRequired[str],
    lastModifiedTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: CaseRuleDetailsOutputTypeDef](./type_defs.md#caseruledetailsoutputtypedef) 
## LayoutContentOutputTypeDef

```python
# LayoutContentOutputTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import LayoutContentOutputTypeDef


def get_value() -> LayoutContentOutputTypeDef:
    return {
        "basic": ...,
    }


# LayoutContentOutputTypeDef definition

class LayoutContentOutputTypeDef(TypedDict):
    basic: NotRequired[BasicLayoutOutputTypeDef],  # (1)
```

1. See [:material-code-braces: BasicLayoutOutputTypeDef](./type_defs.md#basiclayoutoutputtypedef) 
## LayoutContentTypeDef

```python
# LayoutContentTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import LayoutContentTypeDef


def get_value() -> LayoutContentTypeDef:
    return {
        "basic": ...,
    }


# LayoutContentTypeDef definition

class LayoutContentTypeDef(TypedDict):
    basic: NotRequired[BasicLayoutTypeDef],  # (1)
```

1. See [:material-code-braces: BasicLayoutTypeDef](./type_defs.md#basiclayouttypedef) 
## CaseFilterPaginatorTypeDef

```python
# CaseFilterPaginatorTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseFilterPaginatorTypeDef


def get_value() -> CaseFilterPaginatorTypeDef:
    return {
        "andAll": ...,
    }


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
# CaseFilterTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CaseFilterTypeDef


def get_value() -> CaseFilterTypeDef:
    return {
        "andAll": ...,
    }


# CaseFilterTypeDef definition

class CaseFilterTypeDef(TypedDict):
    andAll: NotRequired[Sequence[Mapping[str, Any]]],
    field: NotRequired[FieldFilterTypeDef],  # (1)
    not: NotRequired[Mapping[str, Any]],
    orAll: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: FieldFilterTypeDef](./type_defs.md#fieldfiltertypedef) 
## BatchGetCaseRuleResponseTypeDef

```python
# BatchGetCaseRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import BatchGetCaseRuleResponseTypeDef


def get_value() -> BatchGetCaseRuleResponseTypeDef:
    return {
        "caseRules": ...,
    }


# BatchGetCaseRuleResponseTypeDef definition

class BatchGetCaseRuleResponseTypeDef(TypedDict):
    caseRules: List[GetCaseRuleResponseTypeDef],  # (1)
    errors: List[CaseRuleErrorTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: GetCaseRuleResponseTypeDef](./type_defs.md#getcaseruleresponsetypedef) 
2. See [:material-code-braces: CaseRuleErrorTypeDef](./type_defs.md#caseruleerrortypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCaseRuleRequestTypeDef

```python
# CreateCaseRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateCaseRuleRequestTypeDef


def get_value() -> CreateCaseRuleRequestTypeDef:
    return {
        "domainId": ...,
    }


# CreateCaseRuleRequestTypeDef definition

class CreateCaseRuleRequestTypeDef(TypedDict):
    domainId: str,
    name: str,
    rule: CaseRuleDetailsUnionTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: CaseRuleDetailsTypeDef](./type_defs.md#caseruledetailstypedef) [:material-code-braces: CaseRuleDetailsOutputTypeDef](./type_defs.md#caseruledetailsoutputtypedef) 
## UpdateCaseRuleRequestTypeDef

```python
# UpdateCaseRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import UpdateCaseRuleRequestTypeDef


def get_value() -> UpdateCaseRuleRequestTypeDef:
    return {
        "caseRuleId": ...,
    }


# UpdateCaseRuleRequestTypeDef definition

class UpdateCaseRuleRequestTypeDef(TypedDict):
    caseRuleId: str,
    domainId: str,
    description: NotRequired[str],
    name: NotRequired[str],
    rule: NotRequired[CaseRuleDetailsUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CaseRuleDetailsTypeDef](./type_defs.md#caseruledetailstypedef) [:material-code-braces: CaseRuleDetailsOutputTypeDef](./type_defs.md#caseruledetailsoutputtypedef) 
## GetLayoutResponseTypeDef

```python
# GetLayoutResponseTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import GetLayoutResponseTypeDef


def get_value() -> GetLayoutResponseTypeDef:
    return {
        "content": ...,
    }


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
# SearchCasesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SearchCasesRequestPaginateTypeDef


def get_value() -> SearchCasesRequestPaginateTypeDef:
    return {
        "domainId": ...,
    }


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
## SearchCasesRequestTypeDef

```python
# SearchCasesRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import SearchCasesRequestTypeDef


def get_value() -> SearchCasesRequestTypeDef:
    return {
        "domainId": ...,
    }


# SearchCasesRequestTypeDef definition

class SearchCasesRequestTypeDef(TypedDict):
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
## CreateLayoutRequestTypeDef

```python
# CreateLayoutRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import CreateLayoutRequestTypeDef


def get_value() -> CreateLayoutRequestTypeDef:
    return {
        "content": ...,
    }


# CreateLayoutRequestTypeDef definition

class CreateLayoutRequestTypeDef(TypedDict):
    content: LayoutContentUnionTypeDef,  # (1)
    domainId: str,
    name: str,
```

1. See [:material-code-braces: LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef) [:material-code-braces: LayoutContentOutputTypeDef](./type_defs.md#layoutcontentoutputtypedef) 
## UpdateLayoutRequestTypeDef

```python
# UpdateLayoutRequestTypeDef TypedDict usage example

from types_aiobotocore_connectcases.type_defs import UpdateLayoutRequestTypeDef


def get_value() -> UpdateLayoutRequestTypeDef:
    return {
        "domainId": ...,
    }


# UpdateLayoutRequestTypeDef definition

class UpdateLayoutRequestTypeDef(TypedDict):
    domainId: str,
    layoutId: str,
    content: NotRequired[LayoutContentUnionTypeDef],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-braces: LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef) [:material-code-braces: LayoutContentOutputTypeDef](./type_defs.md#layoutcontentoutputtypedef) 

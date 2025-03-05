# ConnectCases module

> [Index](../README.md) > ConnectCases


!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#connectcases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.21.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ConnectCases` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `ConnectCases` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[connectcases]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[connectcases]'

# standalone installation
python -m pip install types-aiobotocore-connectcases
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-connectcases
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ConnectCasesClient

Type annotations and code completion for  `#!python session.create_client("connectcases")` as [ConnectCasesClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client)

```python
# ConnectCasesClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcases.client import ConnectCasesClient


session = get_session()
async with session.create_client("connectcases") as client:
    client: ConnectCasesClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("connectcases").get_paginator("...")`.

```python
# ListCaseRulesPaginator usage example

from types_aiobotocore_connectcases.paginator import ListCaseRulesPaginator

def get_list_case_rules_paginator() -> ListCaseRulesPaginator:
    return client.get_paginator("list_case_rules"))
```

- [ListCaseRulesPaginator](./paginators.md#listcaserulespaginator)
- [SearchCasesPaginator](./paginators.md#searchcasespaginator)
- [SearchRelatedItemsPaginator](./paginators.md#searchrelateditemspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AuditEventTypeType usage example

from types_aiobotocore_connectcases.literals import AuditEventTypeType

def get_value() -> AuditEventTypeType:
    return "Case.Created"
```

- [AuditEventTypeType](./literals.md#auditeventtypetype)
- [CommentBodyTextTypeType](./literals.md#commentbodytexttypetype)
- [DomainStatusType](./literals.md#domainstatustype)
- [FieldNamespaceType](./literals.md#fieldnamespacetype)
- [FieldTypeType](./literals.md#fieldtypetype)
- [ListCaseRulesPaginatorName](./literals.md#listcaserulespaginatorname)
- [OrderType](./literals.md#ordertype)
- [RelatedItemTypeType](./literals.md#relateditemtypetype)
- [RuleTypeType](./literals.md#ruletypetype)
- [SearchCasesPaginatorName](./literals.md#searchcasespaginatorname)
- [SearchRelatedItemsPaginatorName](./literals.md#searchrelateditemspaginatorname)
- [TemplateStatusType](./literals.md#templatestatustype)
- [ConnectCasesServiceName](./literals.md#connectcasesservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AuditEventFieldValueUnionTypeDef](./type_defs.md#auditeventfieldvalueuniontypedef)
- [UserUnionTypeDef](./type_defs.md#useruniontypedef)
- [CaseRuleIdentifierTypeDef](./type_defs.md#caseruleidentifiertypedef)
- [CaseRuleErrorTypeDef](./type_defs.md#caseruleerrortypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef)
- [FieldErrorTypeDef](./type_defs.md#fielderrortypedef)
- [GetFieldResponseTypeDef](./type_defs.md#getfieldresponsetypedef)
- [FieldOptionTypeDef](./type_defs.md#fieldoptiontypedef)
- [FieldOptionErrorTypeDef](./type_defs.md#fieldoptionerrortypedef)
- [OperandOneTypeDef](./type_defs.md#operandonetypedef)
- [OperandTwoOutputTypeDef](./type_defs.md#operandtwooutputtypedef)
- [OperandTwoTypeDef](./type_defs.md#operandtwotypedef)
- [CaseRuleSummaryTypeDef](./type_defs.md#caserulesummarytypedef)
- [CaseSummaryTypeDef](./type_defs.md#casesummarytypedef)
- [CommentContentTypeDef](./type_defs.md#commentcontenttypedef)
- [ContactContentTypeDef](./type_defs.md#contactcontenttypedef)
- [ContactFilterTypeDef](./type_defs.md#contactfiltertypedef)
- [ContactTypeDef](./type_defs.md#contacttypedef)
- [CreateDomainRequestTypeDef](./type_defs.md#createdomainrequesttypedef)
- [CreateFieldRequestTypeDef](./type_defs.md#createfieldrequesttypedef)
- [LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef)
- [RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef)
- [TemplateRuleTypeDef](./type_defs.md#templateruletypedef)
- [DeleteCaseRuleRequestTypeDef](./type_defs.md#deletecaserulerequesttypedef)
- [DeleteDomainRequestTypeDef](./type_defs.md#deletedomainrequesttypedef)
- [DeleteFieldRequestTypeDef](./type_defs.md#deletefieldrequesttypedef)
- [DeleteLayoutRequestTypeDef](./type_defs.md#deletelayoutrequesttypedef)
- [DeleteTemplateRequestTypeDef](./type_defs.md#deletetemplaterequesttypedef)
- [DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef)
- [RelatedItemEventIncludedDataTypeDef](./type_defs.md#relateditemeventincludeddatatypedef)
- [FieldItemTypeDef](./type_defs.md#fielditemtypedef)
- [FieldSummaryTypeDef](./type_defs.md#fieldsummarytypedef)
- [FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef)
- [FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef)
- [FileContentTypeDef](./type_defs.md#filecontenttypedef)
- [FileFilterTypeDef](./type_defs.md#filefiltertypedef)
- [GetCaseAuditEventsRequestTypeDef](./type_defs.md#getcaseauditeventsrequesttypedef)
- [GetCaseEventConfigurationRequestTypeDef](./type_defs.md#getcaseeventconfigurationrequesttypedef)
- [GetDomainRequestTypeDef](./type_defs.md#getdomainrequesttypedef)
- [GetLayoutRequestTypeDef](./type_defs.md#getlayoutrequesttypedef)
- [GetTemplateRequestTypeDef](./type_defs.md#gettemplaterequesttypedef)
- [LayoutSummaryTypeDef](./type_defs.md#layoutsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCaseRulesRequestTypeDef](./type_defs.md#listcaserulesrequesttypedef)
- [ListCasesForContactRequestTypeDef](./type_defs.md#listcasesforcontactrequesttypedef)
- [ListDomainsRequestTypeDef](./type_defs.md#listdomainsrequesttypedef)
- [ListFieldOptionsRequestTypeDef](./type_defs.md#listfieldoptionsrequesttypedef)
- [ListFieldsRequestTypeDef](./type_defs.md#listfieldsrequesttypedef)
- [ListLayoutsRequestTypeDef](./type_defs.md#listlayoutsrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [ListTemplatesRequestTypeDef](./type_defs.md#listtemplatesrequesttypedef)
- [TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef)
- [SortTypeDef](./type_defs.md#sorttypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateFieldRequestTypeDef](./type_defs.md#updatefieldrequesttypedef)
- [AuditEventFieldTypeDef](./type_defs.md#auditeventfieldtypedef)
- [AuditEventPerformedByTypeDef](./type_defs.md#auditeventperformedbytypedef)
- [BatchGetCaseRuleRequestTypeDef](./type_defs.md#batchgetcaserulerequesttypedef)
- [CreateCaseResponseTypeDef](./type_defs.md#createcaseresponsetypedef)
- [CreateCaseRuleResponseTypeDef](./type_defs.md#createcaseruleresponsetypedef)
- [CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef)
- [CreateFieldResponseTypeDef](./type_defs.md#createfieldresponsetypedef)
- [CreateLayoutResponseTypeDef](./type_defs.md#createlayoutresponsetypedef)
- [CreateRelatedItemResponseTypeDef](./type_defs.md#createrelateditemresponsetypedef)
- [CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDomainResponseTypeDef](./type_defs.md#getdomainresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [BatchGetFieldRequestTypeDef](./type_defs.md#batchgetfieldrequesttypedef)
- [CaseEventIncludedDataOutputTypeDef](./type_defs.md#caseeventincludeddataoutputtypedef)
- [CaseEventIncludedDataTypeDef](./type_defs.md#caseeventincludeddatatypedef)
- [GetCaseRequestTypeDef](./type_defs.md#getcaserequesttypedef)
- [BatchGetFieldResponseTypeDef](./type_defs.md#batchgetfieldresponsetypedef)
- [BatchPutFieldOptionsRequestTypeDef](./type_defs.md#batchputfieldoptionsrequesttypedef)
- [ListFieldOptionsResponseTypeDef](./type_defs.md#listfieldoptionsresponsetypedef)
- [BatchPutFieldOptionsResponseTypeDef](./type_defs.md#batchputfieldoptionsresponsetypedef)
- [BooleanOperandsOutputTypeDef](./type_defs.md#booleanoperandsoutputtypedef)
- [BooleanOperandsTypeDef](./type_defs.md#booleanoperandstypedef)
- [ListCaseRulesResponseTypeDef](./type_defs.md#listcaserulesresponsetypedef)
- [ListCasesForContactResponseTypeDef](./type_defs.md#listcasesforcontactresponsetypedef)
- [CreateTemplateRequestTypeDef](./type_defs.md#createtemplaterequesttypedef)
- [GetTemplateResponseTypeDef](./type_defs.md#gettemplateresponsetypedef)
- [UpdateTemplateRequestTypeDef](./type_defs.md#updatetemplaterequesttypedef)
- [ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef)
- [FieldGroupOutputTypeDef](./type_defs.md#fieldgroupoutputtypedef)
- [FieldGroupTypeDef](./type_defs.md#fieldgrouptypedef)
- [ListFieldsResponseTypeDef](./type_defs.md#listfieldsresponsetypedef)
- [FieldValueOutputTypeDef](./type_defs.md#fieldvalueoutputtypedef)
- [FieldValueUnionUnionTypeDef](./type_defs.md#fieldvalueunionuniontypedef)
- [RelatedItemContentTypeDef](./type_defs.md#relateditemcontenttypedef)
- [RelatedItemInputContentTypeDef](./type_defs.md#relatediteminputcontenttypedef)
- [RelatedItemTypeFilterTypeDef](./type_defs.md#relateditemtypefiltertypedef)
- [ListLayoutsResponseTypeDef](./type_defs.md#listlayoutsresponsetypedef)
- [ListCaseRulesRequestPaginateTypeDef](./type_defs.md#listcaserulesrequestpaginatetypedef)
- [ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef)
- [AuditEventTypeDef](./type_defs.md#auditeventtypedef)
- [EventIncludedDataOutputTypeDef](./type_defs.md#eventincludeddataoutputtypedef)
- [EventIncludedDataTypeDef](./type_defs.md#eventincludeddatatypedef)
- [BooleanConditionOutputTypeDef](./type_defs.md#booleanconditionoutputtypedef)
- [BooleanConditionTypeDef](./type_defs.md#booleanconditiontypedef)
- [SectionOutputTypeDef](./type_defs.md#sectionoutputtypedef)
- [SectionTypeDef](./type_defs.md#sectiontypedef)
- [GetCaseResponseTypeDef](./type_defs.md#getcaseresponsetypedef)
- [SearchCasesResponseItemTypeDef](./type_defs.md#searchcasesresponseitemtypedef)
- [FieldValueTypeDef](./type_defs.md#fieldvaluetypedef)
- [SearchRelatedItemsResponseItemTypeDef](./type_defs.md#searchrelateditemsresponseitemtypedef)
- [CreateRelatedItemRequestTypeDef](./type_defs.md#createrelateditemrequesttypedef)
- [SearchRelatedItemsRequestPaginateTypeDef](./type_defs.md#searchrelateditemsrequestpaginatetypedef)
- [SearchRelatedItemsRequestTypeDef](./type_defs.md#searchrelateditemsrequesttypedef)
- [GetCaseAuditEventsResponseTypeDef](./type_defs.md#getcaseauditeventsresponsetypedef)
- [EventBridgeConfigurationOutputTypeDef](./type_defs.md#eventbridgeconfigurationoutputtypedef)
- [EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef)
- [RequiredCaseRuleOutputTypeDef](./type_defs.md#requiredcaseruleoutputtypedef)
- [RequiredCaseRuleTypeDef](./type_defs.md#requiredcaseruletypedef)
- [LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef)
- [LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef)
- [SearchCasesResponseTypeDef](./type_defs.md#searchcasesresponsetypedef)
- [FieldValueUnionExtraTypeDef](./type_defs.md#fieldvalueunionextratypedef)
- [SearchRelatedItemsResponseTypeDef](./type_defs.md#searchrelateditemsresponsetypedef)
- [GetCaseEventConfigurationResponseTypeDef](./type_defs.md#getcaseeventconfigurationresponsetypedef)
- [EventBridgeConfigurationUnionTypeDef](./type_defs.md#eventbridgeconfigurationuniontypedef)
- [CaseRuleDetailsOutputTypeDef](./type_defs.md#caseruledetailsoutputtypedef)
- [CaseRuleDetailsTypeDef](./type_defs.md#caseruledetailstypedef)
- [BasicLayoutOutputTypeDef](./type_defs.md#basiclayoutoutputtypedef)
- [BasicLayoutTypeDef](./type_defs.md#basiclayouttypedef)
- [CreateCaseRequestTypeDef](./type_defs.md#createcaserequesttypedef)
- [FieldFilterTypeDef](./type_defs.md#fieldfiltertypedef)
- [UpdateCaseRequestTypeDef](./type_defs.md#updatecaserequesttypedef)
- [PutCaseEventConfigurationRequestTypeDef](./type_defs.md#putcaseeventconfigurationrequesttypedef)
- [GetCaseRuleResponseTypeDef](./type_defs.md#getcaseruleresponsetypedef)
- [CaseRuleDetailsUnionTypeDef](./type_defs.md#caseruledetailsuniontypedef)
- [LayoutContentOutputTypeDef](./type_defs.md#layoutcontentoutputtypedef)
- [LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef)
- [CaseFilterPaginatorTypeDef](./type_defs.md#casefilterpaginatortypedef)
- [CaseFilterTypeDef](./type_defs.md#casefiltertypedef)
- [BatchGetCaseRuleResponseTypeDef](./type_defs.md#batchgetcaseruleresponsetypedef)
- [CreateCaseRuleRequestTypeDef](./type_defs.md#createcaserulerequesttypedef)
- [UpdateCaseRuleRequestTypeDef](./type_defs.md#updatecaserulerequesttypedef)
- [GetLayoutResponseTypeDef](./type_defs.md#getlayoutresponsetypedef)
- [LayoutContentUnionTypeDef](./type_defs.md#layoutcontentuniontypedef)
- [SearchCasesRequestPaginateTypeDef](./type_defs.md#searchcasesrequestpaginatetypedef)
- [SearchCasesRequestTypeDef](./type_defs.md#searchcasesrequesttypedef)
- [CreateLayoutRequestTypeDef](./type_defs.md#createlayoutrequesttypedef)
- [UpdateLayoutRequestTypeDef](./type_defs.md#updatelayoutrequesttypedef)


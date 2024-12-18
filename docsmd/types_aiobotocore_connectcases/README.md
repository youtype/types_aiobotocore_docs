# ConnectCases module

> [Index](../README.md) > ConnectCases


!!! note ""

    Auto-generated documentation for [ConnectCases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#connectcases)
    type annotations stubs module [types-aiobotocore-connectcases](https://pypi.org/project/types-aiobotocore-connectcases/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.16.0' mypy_boto3_builder`
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
# SearchCasesPaginator usage example

from types_aiobotocore_connectcases.paginator import SearchCasesPaginator

def get_search_cases_paginator() -> SearchCasesPaginator:
    return client.get_paginator("search_cases"))
```

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
- [OrderType](./literals.md#ordertype)
- [RelatedItemTypeType](./literals.md#relateditemtypetype)
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
- [FieldIdentifierTypeDef](./type_defs.md#fieldidentifiertypedef)
- [FieldErrorTypeDef](./type_defs.md#fielderrortypedef)
- [GetFieldResponseTypeDef](./type_defs.md#getfieldresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [FieldOptionTypeDef](./type_defs.md#fieldoptiontypedef)
- [FieldOptionErrorTypeDef](./type_defs.md#fieldoptionerrortypedef)
- [CaseSummaryTypeDef](./type_defs.md#casesummarytypedef)
- [CommentContentTypeDef](./type_defs.md#commentcontenttypedef)
- [ContactContentTypeDef](./type_defs.md#contactcontenttypedef)
- [ContactFilterTypeDef](./type_defs.md#contactfiltertypedef)
- [ContactTypeDef](./type_defs.md#contacttypedef)
- [CreateDomainRequestRequestTypeDef](./type_defs.md#createdomainrequestrequesttypedef)
- [CreateFieldRequestRequestTypeDef](./type_defs.md#createfieldrequestrequesttypedef)
- [LayoutConfigurationTypeDef](./type_defs.md#layoutconfigurationtypedef)
- [RequiredFieldTypeDef](./type_defs.md#requiredfieldtypedef)
- [DeleteDomainRequestRequestTypeDef](./type_defs.md#deletedomainrequestrequesttypedef)
- [DeleteFieldRequestRequestTypeDef](./type_defs.md#deletefieldrequestrequesttypedef)
- [DeleteLayoutRequestRequestTypeDef](./type_defs.md#deletelayoutrequestrequesttypedef)
- [DeleteTemplateRequestRequestTypeDef](./type_defs.md#deletetemplaterequestrequesttypedef)
- [DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef)
- [RelatedItemEventIncludedDataTypeDef](./type_defs.md#relateditemeventincludeddatatypedef)
- [FieldItemTypeDef](./type_defs.md#fielditemtypedef)
- [FieldSummaryTypeDef](./type_defs.md#fieldsummarytypedef)
- [FieldValueUnionOutputTypeDef](./type_defs.md#fieldvalueunionoutputtypedef)
- [FieldValueUnionTypeDef](./type_defs.md#fieldvalueuniontypedef)
- [FileContentTypeDef](./type_defs.md#filecontenttypedef)
- [FileFilterTypeDef](./type_defs.md#filefiltertypedef)
- [GetCaseAuditEventsRequestRequestTypeDef](./type_defs.md#getcaseauditeventsrequestrequesttypedef)
- [GetCaseEventConfigurationRequestRequestTypeDef](./type_defs.md#getcaseeventconfigurationrequestrequesttypedef)
- [GetDomainRequestRequestTypeDef](./type_defs.md#getdomainrequestrequesttypedef)
- [GetLayoutRequestRequestTypeDef](./type_defs.md#getlayoutrequestrequesttypedef)
- [GetTemplateRequestRequestTypeDef](./type_defs.md#gettemplaterequestrequesttypedef)
- [LayoutSummaryTypeDef](./type_defs.md#layoutsummarytypedef)
- [ListCasesForContactRequestRequestTypeDef](./type_defs.md#listcasesforcontactrequestrequesttypedef)
- [ListDomainsRequestRequestTypeDef](./type_defs.md#listdomainsrequestrequesttypedef)
- [ListFieldOptionsRequestRequestTypeDef](./type_defs.md#listfieldoptionsrequestrequesttypedef)
- [ListFieldsRequestRequestTypeDef](./type_defs.md#listfieldsrequestrequesttypedef)
- [ListLayoutsRequestRequestTypeDef](./type_defs.md#listlayoutsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTemplatesRequestRequestTypeDef](./type_defs.md#listtemplatesrequestrequesttypedef)
- [TemplateSummaryTypeDef](./type_defs.md#templatesummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [SortTypeDef](./type_defs.md#sorttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateFieldRequestRequestTypeDef](./type_defs.md#updatefieldrequestrequesttypedef)
- [AuditEventFieldTypeDef](./type_defs.md#auditeventfieldtypedef)
- [AuditEventPerformedByTypeDef](./type_defs.md#auditeventperformedbytypedef)
- [BatchGetFieldRequestRequestTypeDef](./type_defs.md#batchgetfieldrequestrequesttypedef)
- [CaseEventIncludedDataOutputTypeDef](./type_defs.md#caseeventincludeddataoutputtypedef)
- [CaseEventIncludedDataTypeDef](./type_defs.md#caseeventincludeddatatypedef)
- [GetCaseRequestRequestTypeDef](./type_defs.md#getcaserequestrequesttypedef)
- [BatchGetFieldResponseTypeDef](./type_defs.md#batchgetfieldresponsetypedef)
- [CreateCaseResponseTypeDef](./type_defs.md#createcaseresponsetypedef)
- [CreateDomainResponseTypeDef](./type_defs.md#createdomainresponsetypedef)
- [CreateFieldResponseTypeDef](./type_defs.md#createfieldresponsetypedef)
- [CreateLayoutResponseTypeDef](./type_defs.md#createlayoutresponsetypedef)
- [CreateRelatedItemResponseTypeDef](./type_defs.md#createrelateditemresponsetypedef)
- [CreateTemplateResponseTypeDef](./type_defs.md#createtemplateresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetDomainResponseTypeDef](./type_defs.md#getdomainresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [BatchPutFieldOptionsRequestRequestTypeDef](./type_defs.md#batchputfieldoptionsrequestrequesttypedef)
- [ListFieldOptionsResponseTypeDef](./type_defs.md#listfieldoptionsresponsetypedef)
- [BatchPutFieldOptionsResponseTypeDef](./type_defs.md#batchputfieldoptionsresponsetypedef)
- [ListCasesForContactResponseTypeDef](./type_defs.md#listcasesforcontactresponsetypedef)
- [CreateTemplateRequestRequestTypeDef](./type_defs.md#createtemplaterequestrequesttypedef)
- [GetTemplateResponseTypeDef](./type_defs.md#gettemplateresponsetypedef)
- [UpdateTemplateRequestRequestTypeDef](./type_defs.md#updatetemplaterequestrequesttypedef)
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
- [ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef)
- [AuditEventTypeDef](./type_defs.md#auditeventtypedef)
- [EventIncludedDataOutputTypeDef](./type_defs.md#eventincludeddataoutputtypedef)
- [CaseEventIncludedDataUnionTypeDef](./type_defs.md#caseeventincludeddatauniontypedef)
- [SectionOutputTypeDef](./type_defs.md#sectionoutputtypedef)
- [FieldGroupUnionTypeDef](./type_defs.md#fieldgroupuniontypedef)
- [GetCaseResponseTypeDef](./type_defs.md#getcaseresponsetypedef)
- [SearchCasesResponseItemTypeDef](./type_defs.md#searchcasesresponseitemtypedef)
- [FieldValueTypeDef](./type_defs.md#fieldvaluetypedef)
- [SearchRelatedItemsResponseItemTypeDef](./type_defs.md#searchrelateditemsresponseitemtypedef)
- [CreateRelatedItemRequestRequestTypeDef](./type_defs.md#createrelateditemrequestrequesttypedef)
- [SearchRelatedItemsRequestRequestTypeDef](./type_defs.md#searchrelateditemsrequestrequesttypedef)
- [SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef](./type_defs.md#searchrelateditemsrequestsearchrelateditemspaginatetypedef)
- [GetCaseAuditEventsResponseTypeDef](./type_defs.md#getcaseauditeventsresponsetypedef)
- [EventBridgeConfigurationOutputTypeDef](./type_defs.md#eventbridgeconfigurationoutputtypedef)
- [EventIncludedDataTypeDef](./type_defs.md#eventincludeddatatypedef)
- [LayoutSectionsOutputTypeDef](./type_defs.md#layoutsectionsoutputtypedef)
- [SectionTypeDef](./type_defs.md#sectiontypedef)
- [SearchCasesResponseTypeDef](./type_defs.md#searchcasesresponsetypedef)
- [FieldValueExtraUnionTypeDef](./type_defs.md#fieldvalueextrauniontypedef)
- [UpdateCaseRequestRequestTypeDef](./type_defs.md#updatecaserequestrequesttypedef)
- [SearchRelatedItemsResponseTypeDef](./type_defs.md#searchrelateditemsresponsetypedef)
- [GetCaseEventConfigurationResponseTypeDef](./type_defs.md#getcaseeventconfigurationresponsetypedef)
- [EventIncludedDataUnionTypeDef](./type_defs.md#eventincludeddatauniontypedef)
- [BasicLayoutOutputTypeDef](./type_defs.md#basiclayoutoutputtypedef)
- [SectionUnionTypeDef](./type_defs.md#sectionuniontypedef)
- [CreateCaseRequestRequestTypeDef](./type_defs.md#createcaserequestrequesttypedef)
- [FieldFilterTypeDef](./type_defs.md#fieldfiltertypedef)
- [EventBridgeConfigurationTypeDef](./type_defs.md#eventbridgeconfigurationtypedef)
- [LayoutContentOutputTypeDef](./type_defs.md#layoutcontentoutputtypedef)
- [LayoutSectionsTypeDef](./type_defs.md#layoutsectionstypedef)
- [CaseFilterPaginatorTypeDef](./type_defs.md#casefilterpaginatortypedef)
- [CaseFilterTypeDef](./type_defs.md#casefiltertypedef)
- [PutCaseEventConfigurationRequestRequestTypeDef](./type_defs.md#putcaseeventconfigurationrequestrequesttypedef)
- [GetLayoutResponseTypeDef](./type_defs.md#getlayoutresponsetypedef)
- [LayoutSectionsUnionTypeDef](./type_defs.md#layoutsectionsuniontypedef)
- [SearchCasesRequestSearchCasesPaginateTypeDef](./type_defs.md#searchcasesrequestsearchcasespaginatetypedef)
- [SearchCasesRequestRequestTypeDef](./type_defs.md#searchcasesrequestrequesttypedef)
- [BasicLayoutTypeDef](./type_defs.md#basiclayouttypedef)
- [BasicLayoutUnionTypeDef](./type_defs.md#basiclayoutuniontypedef)
- [LayoutContentTypeDef](./type_defs.md#layoutcontenttypedef)
- [CreateLayoutRequestRequestTypeDef](./type_defs.md#createlayoutrequestrequesttypedef)
- [UpdateLayoutRequestRequestTypeDef](./type_defs.md#updatelayoutrequestrequesttypedef)


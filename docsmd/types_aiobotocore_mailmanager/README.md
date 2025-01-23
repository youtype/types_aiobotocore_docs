# MailManager module

> [Index](../README.md) > MailManager


!!! note ""

    Auto-generated documentation for [MailManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#mailmanager)
    type annotations stubs module [types-aiobotocore-mailmanager](https://pypi.org/project/types-aiobotocore-mailmanager/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MailManager` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MailManager` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mailmanager]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mailmanager]'

# standalone installation
python -m pip install types-aiobotocore-mailmanager
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mailmanager
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MailManagerClient

Type annotations and code completion for  `#!python session.create_client("mailmanager")` as [MailManagerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mailmanager.html#MailManager.Client)

```python
# MailManagerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_mailmanager.client import MailManagerClient


session = get_session()
async with session.create_client("mailmanager") as client:
    client: MailManagerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mailmanager").get_paginator("...")`.

```python
# ListAddonInstancesPaginator usage example

from types_aiobotocore_mailmanager.paginator import ListAddonInstancesPaginator

def get_list_addon_instances_paginator() -> ListAddonInstancesPaginator:
    return client.get_paginator("list_addon_instances"))
```

- [ListAddonInstancesPaginator](./paginators.md#listaddoninstancespaginator)
- [ListAddonSubscriptionsPaginator](./paginators.md#listaddonsubscriptionspaginator)
- [ListArchiveExportsPaginator](./paginators.md#listarchiveexportspaginator)
- [ListArchiveSearchesPaginator](./paginators.md#listarchivesearchespaginator)
- [ListArchivesPaginator](./paginators.md#listarchivespaginator)
- [ListIngressPointsPaginator](./paginators.md#listingresspointspaginator)
- [ListRelaysPaginator](./paginators.md#listrelayspaginator)
- [ListRuleSetsPaginator](./paginators.md#listrulesetspaginator)
- [ListTrafficPoliciesPaginator](./paginators.md#listtrafficpoliciespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AcceptActionType usage example

from types_aiobotocore_mailmanager.literals import AcceptActionType

def get_value() -> AcceptActionType:
    return "ALLOW"
```

- [AcceptActionType](./literals.md#acceptactiontype)
- [ActionFailurePolicyType](./literals.md#actionfailurepolicytype)
- [ArchiveBooleanEmailAttributeType](./literals.md#archivebooleanemailattributetype)
- [ArchiveBooleanOperatorType](./literals.md#archivebooleanoperatortype)
- [ArchiveStateType](./literals.md#archivestatetype)
- [ArchiveStringEmailAttributeType](./literals.md#archivestringemailattributetype)
- [ArchiveStringOperatorType](./literals.md#archivestringoperatortype)
- [ExportStateType](./literals.md#exportstatetype)
- [IngressBooleanOperatorType](./literals.md#ingressbooleanoperatortype)
- [IngressIpOperatorType](./literals.md#ingressipoperatortype)
- [IngressIpv4AttributeType](./literals.md#ingressipv4attributetype)
- [IngressPointStatusToUpdateType](./literals.md#ingresspointstatustoupdatetype)
- [IngressPointStatusType](./literals.md#ingresspointstatustype)
- [IngressPointTypeType](./literals.md#ingresspointtypetype)
- [IngressStringEmailAttributeType](./literals.md#ingressstringemailattributetype)
- [IngressStringOperatorType](./literals.md#ingressstringoperatortype)
- [IngressTlsAttributeType](./literals.md#ingresstlsattributetype)
- [IngressTlsProtocolAttributeType](./literals.md#ingresstlsprotocolattributetype)
- [IngressTlsProtocolOperatorType](./literals.md#ingresstlsprotocoloperatortype)
- [ListAddonInstancesPaginatorName](./literals.md#listaddoninstancespaginatorname)
- [ListAddonSubscriptionsPaginatorName](./literals.md#listaddonsubscriptionspaginatorname)
- [ListArchiveExportsPaginatorName](./literals.md#listarchiveexportspaginatorname)
- [ListArchiveSearchesPaginatorName](./literals.md#listarchivesearchespaginatorname)
- [ListArchivesPaginatorName](./literals.md#listarchivespaginatorname)
- [ListIngressPointsPaginatorName](./literals.md#listingresspointspaginatorname)
- [ListRelaysPaginatorName](./literals.md#listrelayspaginatorname)
- [ListRuleSetsPaginatorName](./literals.md#listrulesetspaginatorname)
- [ListTrafficPoliciesPaginatorName](./literals.md#listtrafficpoliciespaginatorname)
- [MailFromType](./literals.md#mailfromtype)
- [RetentionPeriodType](./literals.md#retentionperiodtype)
- [RuleBooleanEmailAttributeType](./literals.md#rulebooleanemailattributetype)
- [RuleBooleanOperatorType](./literals.md#rulebooleanoperatortype)
- [RuleDmarcOperatorType](./literals.md#ruledmarcoperatortype)
- [RuleDmarcPolicyType](./literals.md#ruledmarcpolicytype)
- [RuleIpEmailAttributeType](./literals.md#ruleipemailattributetype)
- [RuleIpOperatorType](./literals.md#ruleipoperatortype)
- [RuleNumberEmailAttributeType](./literals.md#rulenumberemailattributetype)
- [RuleNumberOperatorType](./literals.md#rulenumberoperatortype)
- [RuleStringEmailAttributeType](./literals.md#rulestringemailattributetype)
- [RuleStringOperatorType](./literals.md#rulestringoperatortype)
- [RuleVerdictAttributeType](./literals.md#ruleverdictattributetype)
- [RuleVerdictOperatorType](./literals.md#ruleverdictoperatortype)
- [RuleVerdictType](./literals.md#ruleverdicttype)
- [SearchStateType](./literals.md#searchstatetype)
- [MailManagerServiceName](./literals.md#mailmanagerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddHeaderActionTypeDef](./type_defs.md#addheaderactiontypedef)
- [AddonInstanceTypeDef](./type_defs.md#addoninstancetypedef)
- [AddonSubscriptionTypeDef](./type_defs.md#addonsubscriptiontypedef)
- [AnalysisTypeDef](./type_defs.md#analysistypedef)
- [ArchiveActionTypeDef](./type_defs.md#archiveactiontypedef)
- [ArchiveBooleanToEvaluateTypeDef](./type_defs.md#archivebooleantoevaluatetypedef)
- [ArchiveRetentionTypeDef](./type_defs.md#archiveretentiontypedef)
- [ArchiveStringToEvaluateTypeDef](./type_defs.md#archivestringtoevaluatetypedef)
- [ArchiveTypeDef](./type_defs.md#archivetypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [IngressPointConfigurationTypeDef](./type_defs.md#ingresspointconfigurationtypedef)
- [RelayAuthenticationTypeDef](./type_defs.md#relayauthenticationtypedef)
- [DeleteAddonInstanceRequestRequestTypeDef](./type_defs.md#deleteaddoninstancerequestrequesttypedef)
- [DeleteAddonSubscriptionRequestRequestTypeDef](./type_defs.md#deleteaddonsubscriptionrequestrequesttypedef)
- [DeleteArchiveRequestRequestTypeDef](./type_defs.md#deletearchiverequestrequesttypedef)
- [DeleteIngressPointRequestRequestTypeDef](./type_defs.md#deleteingresspointrequestrequesttypedef)
- [DeleteRelayRequestRequestTypeDef](./type_defs.md#deleterelayrequestrequesttypedef)
- [DeleteRuleSetRequestRequestTypeDef](./type_defs.md#deleterulesetrequestrequesttypedef)
- [DeleteTrafficPolicyRequestRequestTypeDef](./type_defs.md#deletetrafficpolicyrequestrequesttypedef)
- [DeliverToMailboxActionTypeDef](./type_defs.md#delivertomailboxactiontypedef)
- [DeliverToQBusinessActionTypeDef](./type_defs.md#delivertoqbusinessactiontypedef)
- [EnvelopeTypeDef](./type_defs.md#envelopetypedef)
- [S3ExportDestinationConfigurationTypeDef](./type_defs.md#s3exportdestinationconfigurationtypedef)
- [ExportStatusTypeDef](./type_defs.md#exportstatustypedef)
- [GetAddonInstanceRequestRequestTypeDef](./type_defs.md#getaddoninstancerequestrequesttypedef)
- [GetAddonSubscriptionRequestRequestTypeDef](./type_defs.md#getaddonsubscriptionrequestrequesttypedef)
- [GetArchiveExportRequestRequestTypeDef](./type_defs.md#getarchiveexportrequestrequesttypedef)
- [GetArchiveMessageContentRequestRequestTypeDef](./type_defs.md#getarchivemessagecontentrequestrequesttypedef)
- [MessageBodyTypeDef](./type_defs.md#messagebodytypedef)
- [GetArchiveMessageRequestRequestTypeDef](./type_defs.md#getarchivemessagerequestrequesttypedef)
- [MetadataTypeDef](./type_defs.md#metadatatypedef)
- [GetArchiveRequestRequestTypeDef](./type_defs.md#getarchiverequestrequesttypedef)
- [GetArchiveSearchRequestRequestTypeDef](./type_defs.md#getarchivesearchrequestrequesttypedef)
- [SearchStatusTypeDef](./type_defs.md#searchstatustypedef)
- [GetArchiveSearchResultsRequestRequestTypeDef](./type_defs.md#getarchivesearchresultsrequestrequesttypedef)
- [GetIngressPointRequestRequestTypeDef](./type_defs.md#getingresspointrequestrequesttypedef)
- [GetRelayRequestRequestTypeDef](./type_defs.md#getrelayrequestrequesttypedef)
- [RelayAuthenticationOutputTypeDef](./type_defs.md#relayauthenticationoutputtypedef)
- [GetRuleSetRequestRequestTypeDef](./type_defs.md#getrulesetrequestrequesttypedef)
- [GetTrafficPolicyRequestRequestTypeDef](./type_defs.md#gettrafficpolicyrequestrequesttypedef)
- [IngressAnalysisTypeDef](./type_defs.md#ingressanalysistypedef)
- [IngressIpToEvaluateTypeDef](./type_defs.md#ingressiptoevaluatetypedef)
- [IngressPointPasswordConfigurationTypeDef](./type_defs.md#ingresspointpasswordconfigurationtypedef)
- [IngressPointTypeDef](./type_defs.md#ingresspointtypedef)
- [IngressStringToEvaluateTypeDef](./type_defs.md#ingressstringtoevaluatetypedef)
- [IngressTlsProtocolToEvaluateTypeDef](./type_defs.md#ingresstlsprotocoltoevaluatetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAddonInstancesRequestRequestTypeDef](./type_defs.md#listaddoninstancesrequestrequesttypedef)
- [ListAddonSubscriptionsRequestRequestTypeDef](./type_defs.md#listaddonsubscriptionsrequestrequesttypedef)
- [ListArchiveExportsRequestRequestTypeDef](./type_defs.md#listarchiveexportsrequestrequesttypedef)
- [ListArchiveSearchesRequestRequestTypeDef](./type_defs.md#listarchivesearchesrequestrequesttypedef)
- [ListArchivesRequestRequestTypeDef](./type_defs.md#listarchivesrequestrequesttypedef)
- [ListIngressPointsRequestRequestTypeDef](./type_defs.md#listingresspointsrequestrequesttypedef)
- [ListRelaysRequestRequestTypeDef](./type_defs.md#listrelaysrequestrequesttypedef)
- [RelayTypeDef](./type_defs.md#relaytypedef)
- [ListRuleSetsRequestRequestTypeDef](./type_defs.md#listrulesetsrequestrequesttypedef)
- [RuleSetTypeDef](./type_defs.md#rulesettypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTrafficPoliciesRequestRequestTypeDef](./type_defs.md#listtrafficpoliciesrequestrequesttypedef)
- [TrafficPolicyTypeDef](./type_defs.md#trafficpolicytypedef)
- [RelayActionTypeDef](./type_defs.md#relayactiontypedef)
- [ReplaceRecipientActionOutputTypeDef](./type_defs.md#replacerecipientactionoutputtypedef)
- [ReplaceRecipientActionTypeDef](./type_defs.md#replacerecipientactiontypedef)
- [S3ActionTypeDef](./type_defs.md#s3actiontypedef)
- [SendActionTypeDef](./type_defs.md#sendactiontypedef)
- [RuleBooleanToEvaluateTypeDef](./type_defs.md#rulebooleantoevaluatetypedef)
- [RuleDmarcExpressionOutputTypeDef](./type_defs.md#ruledmarcexpressionoutputtypedef)
- [RuleDmarcExpressionTypeDef](./type_defs.md#ruledmarcexpressiontypedef)
- [RuleIpToEvaluateTypeDef](./type_defs.md#ruleiptoevaluatetypedef)
- [RuleNumberToEvaluateTypeDef](./type_defs.md#rulenumbertoevaluatetypedef)
- [RuleStringToEvaluateTypeDef](./type_defs.md#rulestringtoevaluatetypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [StopArchiveExportRequestRequestTypeDef](./type_defs.md#stoparchiveexportrequestrequesttypedef)
- [StopArchiveSearchRequestRequestTypeDef](./type_defs.md#stoparchivesearchrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [RuleVerdictToEvaluateTypeDef](./type_defs.md#ruleverdicttoevaluatetypedef)
- [ArchiveBooleanExpressionTypeDef](./type_defs.md#archivebooleanexpressiontypedef)
- [UpdateArchiveRequestRequestTypeDef](./type_defs.md#updatearchiverequestrequesttypedef)
- [ArchiveStringExpressionOutputTypeDef](./type_defs.md#archivestringexpressionoutputtypedef)
- [ArchiveStringExpressionTypeDef](./type_defs.md#archivestringexpressiontypedef)
- [CreateAddonInstanceRequestRequestTypeDef](./type_defs.md#createaddoninstancerequestrequesttypedef)
- [CreateAddonSubscriptionRequestRequestTypeDef](./type_defs.md#createaddonsubscriptionrequestrequesttypedef)
- [CreateArchiveRequestRequestTypeDef](./type_defs.md#createarchiverequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateAddonInstanceResponseTypeDef](./type_defs.md#createaddoninstanceresponsetypedef)
- [CreateAddonSubscriptionResponseTypeDef](./type_defs.md#createaddonsubscriptionresponsetypedef)
- [CreateArchiveResponseTypeDef](./type_defs.md#createarchiveresponsetypedef)
- [CreateIngressPointResponseTypeDef](./type_defs.md#createingresspointresponsetypedef)
- [CreateRelayResponseTypeDef](./type_defs.md#createrelayresponsetypedef)
- [CreateRuleSetResponseTypeDef](./type_defs.md#createrulesetresponsetypedef)
- [CreateTrafficPolicyResponseTypeDef](./type_defs.md#createtrafficpolicyresponsetypedef)
- [GetAddonInstanceResponseTypeDef](./type_defs.md#getaddoninstanceresponsetypedef)
- [GetAddonSubscriptionResponseTypeDef](./type_defs.md#getaddonsubscriptionresponsetypedef)
- [GetArchiveResponseTypeDef](./type_defs.md#getarchiveresponsetypedef)
- [ListAddonInstancesResponseTypeDef](./type_defs.md#listaddoninstancesresponsetypedef)
- [ListAddonSubscriptionsResponseTypeDef](./type_defs.md#listaddonsubscriptionsresponsetypedef)
- [ListArchivesResponseTypeDef](./type_defs.md#listarchivesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [StartArchiveExportResponseTypeDef](./type_defs.md#startarchiveexportresponsetypedef)
- [StartArchiveSearchResponseTypeDef](./type_defs.md#startarchivesearchresponsetypedef)
- [CreateIngressPointRequestRequestTypeDef](./type_defs.md#createingresspointrequestrequesttypedef)
- [UpdateIngressPointRequestRequestTypeDef](./type_defs.md#updateingresspointrequestrequesttypedef)
- [CreateRelayRequestRequestTypeDef](./type_defs.md#createrelayrequestrequesttypedef)
- [UpdateRelayRequestRequestTypeDef](./type_defs.md#updaterelayrequestrequesttypedef)
- [RowTypeDef](./type_defs.md#rowtypedef)
- [ExportDestinationConfigurationTypeDef](./type_defs.md#exportdestinationconfigurationtypedef)
- [ExportSummaryTypeDef](./type_defs.md#exportsummarytypedef)
- [GetArchiveMessageContentResponseTypeDef](./type_defs.md#getarchivemessagecontentresponsetypedef)
- [GetArchiveMessageResponseTypeDef](./type_defs.md#getarchivemessageresponsetypedef)
- [SearchSummaryTypeDef](./type_defs.md#searchsummarytypedef)
- [GetRelayResponseTypeDef](./type_defs.md#getrelayresponsetypedef)
- [IngressBooleanToEvaluateTypeDef](./type_defs.md#ingressbooleantoevaluatetypedef)
- [IngressIpv4ExpressionOutputTypeDef](./type_defs.md#ingressipv4expressionoutputtypedef)
- [IngressIpv4ExpressionTypeDef](./type_defs.md#ingressipv4expressiontypedef)
- [IngressPointAuthConfigurationTypeDef](./type_defs.md#ingresspointauthconfigurationtypedef)
- [ListIngressPointsResponseTypeDef](./type_defs.md#listingresspointsresponsetypedef)
- [IngressStringExpressionOutputTypeDef](./type_defs.md#ingressstringexpressionoutputtypedef)
- [IngressStringExpressionTypeDef](./type_defs.md#ingressstringexpressiontypedef)
- [IngressTlsProtocolExpressionTypeDef](./type_defs.md#ingresstlsprotocolexpressiontypedef)
- [ListAddonInstancesRequestPaginateTypeDef](./type_defs.md#listaddoninstancesrequestpaginatetypedef)
- [ListAddonSubscriptionsRequestPaginateTypeDef](./type_defs.md#listaddonsubscriptionsrequestpaginatetypedef)
- [ListArchiveExportsRequestPaginateTypeDef](./type_defs.md#listarchiveexportsrequestpaginatetypedef)
- [ListArchiveSearchesRequestPaginateTypeDef](./type_defs.md#listarchivesearchesrequestpaginatetypedef)
- [ListArchivesRequestPaginateTypeDef](./type_defs.md#listarchivesrequestpaginatetypedef)
- [ListIngressPointsRequestPaginateTypeDef](./type_defs.md#listingresspointsrequestpaginatetypedef)
- [ListRelaysRequestPaginateTypeDef](./type_defs.md#listrelaysrequestpaginatetypedef)
- [ListRuleSetsRequestPaginateTypeDef](./type_defs.md#listrulesetsrequestpaginatetypedef)
- [ListTrafficPoliciesRequestPaginateTypeDef](./type_defs.md#listtrafficpoliciesrequestpaginatetypedef)
- [ListRelaysResponseTypeDef](./type_defs.md#listrelaysresponsetypedef)
- [ListRuleSetsResponseTypeDef](./type_defs.md#listrulesetsresponsetypedef)
- [ListTrafficPoliciesResponseTypeDef](./type_defs.md#listtrafficpoliciesresponsetypedef)
- [ReplaceRecipientActionUnionTypeDef](./type_defs.md#replacerecipientactionuniontypedef)
- [RuleActionOutputTypeDef](./type_defs.md#ruleactionoutputtypedef)
- [RuleBooleanExpressionTypeDef](./type_defs.md#rulebooleanexpressiontypedef)
- [RuleDmarcExpressionUnionTypeDef](./type_defs.md#ruledmarcexpressionuniontypedef)
- [RuleIpExpressionOutputTypeDef](./type_defs.md#ruleipexpressionoutputtypedef)
- [RuleIpExpressionTypeDef](./type_defs.md#ruleipexpressiontypedef)
- [RuleNumberExpressionTypeDef](./type_defs.md#rulenumberexpressiontypedef)
- [RuleStringExpressionOutputTypeDef](./type_defs.md#rulestringexpressionoutputtypedef)
- [RuleStringExpressionTypeDef](./type_defs.md#rulestringexpressiontypedef)
- [RuleVerdictExpressionOutputTypeDef](./type_defs.md#ruleverdictexpressionoutputtypedef)
- [RuleVerdictExpressionTypeDef](./type_defs.md#ruleverdictexpressiontypedef)
- [ArchiveFilterConditionOutputTypeDef](./type_defs.md#archivefilterconditionoutputtypedef)
- [ArchiveStringExpressionUnionTypeDef](./type_defs.md#archivestringexpressionuniontypedef)
- [GetArchiveSearchResultsResponseTypeDef](./type_defs.md#getarchivesearchresultsresponsetypedef)
- [ListArchiveExportsResponseTypeDef](./type_defs.md#listarchiveexportsresponsetypedef)
- [ListArchiveSearchesResponseTypeDef](./type_defs.md#listarchivesearchesresponsetypedef)
- [IngressBooleanExpressionTypeDef](./type_defs.md#ingressbooleanexpressiontypedef)
- [IngressIpv4ExpressionUnionTypeDef](./type_defs.md#ingressipv4expressionuniontypedef)
- [GetIngressPointResponseTypeDef](./type_defs.md#getingresspointresponsetypedef)
- [IngressStringExpressionUnionTypeDef](./type_defs.md#ingressstringexpressionuniontypedef)
- [RuleActionTypeDef](./type_defs.md#ruleactiontypedef)
- [RuleIpExpressionUnionTypeDef](./type_defs.md#ruleipexpressionuniontypedef)
- [RuleStringExpressionUnionTypeDef](./type_defs.md#rulestringexpressionuniontypedef)
- [RuleConditionOutputTypeDef](./type_defs.md#ruleconditionoutputtypedef)
- [RuleVerdictExpressionUnionTypeDef](./type_defs.md#ruleverdictexpressionuniontypedef)
- [ArchiveFiltersOutputTypeDef](./type_defs.md#archivefiltersoutputtypedef)
- [ArchiveFilterConditionTypeDef](./type_defs.md#archivefilterconditiontypedef)
- [PolicyConditionOutputTypeDef](./type_defs.md#policyconditionoutputtypedef)
- [PolicyConditionTypeDef](./type_defs.md#policyconditiontypedef)
- [RuleActionUnionTypeDef](./type_defs.md#ruleactionuniontypedef)
- [RuleOutputTypeDef](./type_defs.md#ruleoutputtypedef)
- [RuleConditionTypeDef](./type_defs.md#ruleconditiontypedef)
- [GetArchiveExportResponseTypeDef](./type_defs.md#getarchiveexportresponsetypedef)
- [GetArchiveSearchResponseTypeDef](./type_defs.md#getarchivesearchresponsetypedef)
- [ArchiveFilterConditionUnionTypeDef](./type_defs.md#archivefilterconditionuniontypedef)
- [PolicyStatementOutputTypeDef](./type_defs.md#policystatementoutputtypedef)
- [PolicyConditionUnionTypeDef](./type_defs.md#policyconditionuniontypedef)
- [GetRuleSetResponseTypeDef](./type_defs.md#getrulesetresponsetypedef)
- [RuleConditionUnionTypeDef](./type_defs.md#ruleconditionuniontypedef)
- [ArchiveFiltersTypeDef](./type_defs.md#archivefilterstypedef)
- [GetTrafficPolicyResponseTypeDef](./type_defs.md#gettrafficpolicyresponsetypedef)
- [PolicyStatementTypeDef](./type_defs.md#policystatementtypedef)
- [RuleTypeDef](./type_defs.md#ruletypedef)
- [StartArchiveExportRequestRequestTypeDef](./type_defs.md#startarchiveexportrequestrequesttypedef)
- [StartArchiveSearchRequestRequestTypeDef](./type_defs.md#startarchivesearchrequestrequesttypedef)
- [PolicyStatementUnionTypeDef](./type_defs.md#policystatementuniontypedef)
- [UpdateTrafficPolicyRequestRequestTypeDef](./type_defs.md#updatetrafficpolicyrequestrequesttypedef)
- [RuleUnionTypeDef](./type_defs.md#ruleuniontypedef)
- [UpdateRuleSetRequestRequestTypeDef](./type_defs.md#updaterulesetrequestrequesttypedef)
- [CreateTrafficPolicyRequestRequestTypeDef](./type_defs.md#createtrafficpolicyrequestrequesttypedef)
- [CreateRuleSetRequestRequestTypeDef](./type_defs.md#createrulesetrequestrequesttypedef)


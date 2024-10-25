# QConnect module

> [Index](../README.md) > QConnect


!!! note ""

    Auto-generated documentation for [QConnect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect)
    type annotations stubs module [types-aiobotocore-qconnect](https://pypi.org/project/types-aiobotocore-qconnect/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `QConnect` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[qconnect]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[qconnect]'


# standalone installation
python -m pip install types-aiobotocore-qconnect
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-qconnect
```

## Usage

Code samples can be found in [Examples](./usage.md).

## QConnectClient

Type annotations and code completion for  `#!python session.create_client("qconnect")` as [QConnectClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qconnect.html#QConnect.Client)

```python
# QConnectClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_qconnect.client import QConnectClient


session = get_session()
async with session.create_client("qconnect") as client:
    client: QConnectClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("qconnect").get_paginator("...")`.

```python
# ListAIAgentVersionsPaginator usage example

from types_aiobotocore_qconnect.paginator import ListAIAgentVersionsPaginator

def get_list_ai_agent_versions_paginator() -> ListAIAgentVersionsPaginator:
    return client.get_paginator("list_ai_agent_versions"))
```

- [ListAIAgentVersionsPaginator](./paginators.md#listaiagentversionspaginator)
- [ListAIAgentsPaginator](./paginators.md#listaiagentspaginator)
- [ListAIPromptVersionsPaginator](./paginators.md#listaipromptversionspaginator)
- [ListAIPromptsPaginator](./paginators.md#listaipromptspaginator)
- [ListAssistantAssociationsPaginator](./paginators.md#listassistantassociationspaginator)
- [ListAssistantsPaginator](./paginators.md#listassistantspaginator)
- [ListContentAssociationsPaginator](./paginators.md#listcontentassociationspaginator)
- [ListContentsPaginator](./paginators.md#listcontentspaginator)
- [ListImportJobsPaginator](./paginators.md#listimportjobspaginator)
- [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)
- [ListQuickResponsesPaginator](./paginators.md#listquickresponsespaginator)
- [QueryAssistantPaginator](./paginators.md#queryassistantpaginator)
- [SearchContentPaginator](./paginators.md#searchcontentpaginator)
- [SearchQuickResponsesPaginator](./paginators.md#searchquickresponsespaginator)
- [SearchSessionsPaginator](./paginators.md#searchsessionspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AIAgentAssociationConfigurationTypeType usage example

from types_aiobotocore_qconnect.literals import AIAgentAssociationConfigurationTypeType

def get_value() -> AIAgentAssociationConfigurationTypeType:
    return "KNOWLEDGE_BASE"
```

- [AIAgentAssociationConfigurationTypeType](./literals.md#aiagentassociationconfigurationtypetype)
- [AIAgentTypeType](./literals.md#aiagenttypetype)
- [AIPromptAPIFormatType](./literals.md#aipromptapiformattype)
- [AIPromptTemplateTypeType](./literals.md#aiprompttemplatetypetype)
- [AIPromptTypeType](./literals.md#aiprompttypetype)
- [AssistantCapabilityTypeType](./literals.md#assistantcapabilitytypetype)
- [AssistantStatusType](./literals.md#assistantstatustype)
- [AssistantTypeType](./literals.md#assistanttypetype)
- [AssociationTypeType](./literals.md#associationtypetype)
- [ChunkingStrategyType](./literals.md#chunkingstrategytype)
- [ContentAssociationTypeType](./literals.md#contentassociationtypetype)
- [ContentStatusType](./literals.md#contentstatustype)
- [ExternalSourceType](./literals.md#externalsourcetype)
- [FilterFieldType](./literals.md#filterfieldtype)
- [FilterOperatorType](./literals.md#filteroperatortype)
- [ImportJobStatusType](./literals.md#importjobstatustype)
- [ImportJobTypeType](./literals.md#importjobtypetype)
- [KnowledgeBaseSearchTypeType](./literals.md#knowledgebasesearchtypetype)
- [KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype)
- [KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype)
- [ListAIAgentVersionsPaginatorName](./literals.md#listaiagentversionspaginatorname)
- [ListAIAgentsPaginatorName](./literals.md#listaiagentspaginatorname)
- [ListAIPromptVersionsPaginatorName](./literals.md#listaipromptversionspaginatorname)
- [ListAIPromptsPaginatorName](./literals.md#listaipromptspaginatorname)
- [ListAssistantAssociationsPaginatorName](./literals.md#listassistantassociationspaginatorname)
- [ListAssistantsPaginatorName](./literals.md#listassistantspaginatorname)
- [ListContentAssociationsPaginatorName](./literals.md#listcontentassociationspaginatorname)
- [ListContentsPaginatorName](./literals.md#listcontentspaginatorname)
- [ListImportJobsPaginatorName](./literals.md#listimportjobspaginatorname)
- [ListKnowledgeBasesPaginatorName](./literals.md#listknowledgebasespaginatorname)
- [ListQuickResponsesPaginatorName](./literals.md#listquickresponsespaginatorname)
- [OrderType](./literals.md#ordertype)
- [OriginType](./literals.md#origintype)
- [ParsingStrategyType](./literals.md#parsingstrategytype)
- [PriorityType](./literals.md#prioritytype)
- [QueryAssistantPaginatorName](./literals.md#queryassistantpaginatorname)
- [QueryConditionComparisonOperatorType](./literals.md#queryconditioncomparisonoperatortype)
- [QueryConditionFieldNameType](./literals.md#queryconditionfieldnametype)
- [QueryResultTypeType](./literals.md#queryresulttypetype)
- [QuickResponseFilterOperatorType](./literals.md#quickresponsefilteroperatortype)
- [QuickResponseQueryOperatorType](./literals.md#quickresponsequeryoperatortype)
- [QuickResponseStatusType](./literals.md#quickresponsestatustype)
- [RecommendationSourceTypeType](./literals.md#recommendationsourcetypetype)
- [RecommendationTriggerTypeType](./literals.md#recommendationtriggertypetype)
- [RecommendationTypeType](./literals.md#recommendationtypetype)
- [ReferenceTypeType](./literals.md#referencetypetype)
- [RelevanceLevelType](./literals.md#relevanceleveltype)
- [RelevanceType](./literals.md#relevancetype)
- [SearchContentPaginatorName](./literals.md#searchcontentpaginatorname)
- [SearchQuickResponsesPaginatorName](./literals.md#searchquickresponsespaginatorname)
- [SearchSessionsPaginatorName](./literals.md#searchsessionspaginatorname)
- [SessionDataNamespaceType](./literals.md#sessiondatanamespacetype)
- [SourceContentTypeType](./literals.md#sourcecontenttypetype)
- [StatusType](./literals.md#statustype)
- [SyncStatusType](./literals.md#syncstatustype)
- [TargetTypeType](./literals.md#targettypetype)
- [VisibilityStatusType](./literals.md#visibilitystatustype)
- [WebScopeTypeType](./literals.md#webscopetypetype)
- [QConnectServiceName](./literals.md#qconnectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AIAgentConfigurationDataTypeDef](./type_defs.md#aiagentconfigurationdatatypedef)
- [AIPromptSummaryTypeDef](./type_defs.md#aipromptsummarytypedef)
- [TextFullAIPromptEditTemplateConfigurationTypeDef](./type_defs.md#textfullaipromptedittemplateconfigurationtypedef)
- [AmazonConnectGuideAssociationDataTypeDef](./type_defs.md#amazonconnectguideassociationdatatypedef)
- [AppIntegrationsConfigurationOutputTypeDef](./type_defs.md#appintegrationsconfigurationoutputtypedef)
- [AppIntegrationsConfigurationTypeDef](./type_defs.md#appintegrationsconfigurationtypedef)
- [AssistantAssociationInputDataTypeDef](./type_defs.md#assistantassociationinputdatatypedef)
- [KnowledgeBaseAssociationDataTypeDef](./type_defs.md#knowledgebaseassociationdatatypedef)
- [AssistantCapabilityConfigurationTypeDef](./type_defs.md#assistantcapabilityconfigurationtypedef)
- [AssistantIntegrationConfigurationTypeDef](./type_defs.md#assistantintegrationconfigurationtypedef)
- [ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
- [ParsingPromptTypeDef](./type_defs.md#parsingprompttypedef)
- [FixedSizeChunkingConfigurationTypeDef](./type_defs.md#fixedsizechunkingconfigurationtypedef)
- [SemanticChunkingConfigurationTypeDef](./type_defs.md#semanticchunkingconfigurationtypedef)
- [CitationSpanTypeDef](./type_defs.md#citationspantypedef)
- [ConnectConfigurationTypeDef](./type_defs.md#connectconfigurationtypedef)
- [RankingDataTypeDef](./type_defs.md#rankingdatatypedef)
- [ContentDataTypeDef](./type_defs.md#contentdatatypedef)
- [GenerativeContentFeedbackDataTypeDef](./type_defs.md#generativecontentfeedbackdatatypedef)
- [ContentReferenceTypeDef](./type_defs.md#contentreferencetypedef)
- [ContentSummaryTypeDef](./type_defs.md#contentsummarytypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [CreateContentRequestRequestTypeDef](./type_defs.md#createcontentrequestrequesttypedef)
- [RenderingConfigurationTypeDef](./type_defs.md#renderingconfigurationtypedef)
- [GroupingConfigurationTypeDef](./type_defs.md#groupingconfigurationtypedef)
- [QuickResponseDataProviderTypeDef](./type_defs.md#quickresponsedataprovidertypedef)
- [IntentDetectedDataDetailsTypeDef](./type_defs.md#intentdetecteddatadetailstypedef)
- [GenerativeReferenceTypeDef](./type_defs.md#generativereferencetypedef)
- [DeleteAIAgentRequestRequestTypeDef](./type_defs.md#deleteaiagentrequestrequesttypedef)
- [DeleteAIAgentVersionRequestRequestTypeDef](./type_defs.md#deleteaiagentversionrequestrequesttypedef)
- [DeleteAIPromptRequestRequestTypeDef](./type_defs.md#deleteaipromptrequestrequesttypedef)
- [DeleteAIPromptVersionRequestRequestTypeDef](./type_defs.md#deleteaipromptversionrequestrequesttypedef)
- [DeleteAssistantAssociationRequestRequestTypeDef](./type_defs.md#deleteassistantassociationrequestrequesttypedef)
- [DeleteAssistantRequestRequestTypeDef](./type_defs.md#deleteassistantrequestrequesttypedef)
- [DeleteContentAssociationRequestRequestTypeDef](./type_defs.md#deletecontentassociationrequestrequesttypedef)
- [DeleteContentRequestRequestTypeDef](./type_defs.md#deletecontentrequestrequesttypedef)
- [DeleteImportJobRequestRequestTypeDef](./type_defs.md#deleteimportjobrequestrequesttypedef)
- [DeleteKnowledgeBaseRequestRequestTypeDef](./type_defs.md#deleteknowledgebaserequestrequesttypedef)
- [DeleteQuickResponseRequestRequestTypeDef](./type_defs.md#deletequickresponserequestrequesttypedef)
- [HighlightTypeDef](./type_defs.md#highlighttypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GetAIAgentRequestRequestTypeDef](./type_defs.md#getaiagentrequestrequesttypedef)
- [GetAIPromptRequestRequestTypeDef](./type_defs.md#getaipromptrequestrequesttypedef)
- [GetAssistantAssociationRequestRequestTypeDef](./type_defs.md#getassistantassociationrequestrequesttypedef)
- [GetAssistantRequestRequestTypeDef](./type_defs.md#getassistantrequestrequesttypedef)
- [GetContentAssociationRequestRequestTypeDef](./type_defs.md#getcontentassociationrequestrequesttypedef)
- [GetContentRequestRequestTypeDef](./type_defs.md#getcontentrequestrequesttypedef)
- [GetContentSummaryRequestRequestTypeDef](./type_defs.md#getcontentsummaryrequestrequesttypedef)
- [GetImportJobRequestRequestTypeDef](./type_defs.md#getimportjobrequestrequesttypedef)
- [GetKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getknowledgebaserequestrequesttypedef)
- [GetQuickResponseRequestRequestTypeDef](./type_defs.md#getquickresponserequestrequesttypedef)
- [GetRecommendationsRequestRequestTypeDef](./type_defs.md#getrecommendationsrequestrequesttypedef)
- [GetSessionRequestRequestTypeDef](./type_defs.md#getsessionrequestrequesttypedef)
- [GroupingConfigurationOutputTypeDef](./type_defs.md#groupingconfigurationoutputtypedef)
- [HierarchicalChunkingLevelConfigurationTypeDef](./type_defs.md#hierarchicalchunkinglevelconfigurationtypedef)
- [IntentInputDataTypeDef](./type_defs.md#intentinputdatatypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAIAgentVersionsRequestRequestTypeDef](./type_defs.md#listaiagentversionsrequestrequesttypedef)
- [ListAIAgentsRequestRequestTypeDef](./type_defs.md#listaiagentsrequestrequesttypedef)
- [ListAIPromptVersionsRequestRequestTypeDef](./type_defs.md#listaipromptversionsrequestrequesttypedef)
- [ListAIPromptsRequestRequestTypeDef](./type_defs.md#listaipromptsrequestrequesttypedef)
- [ListAssistantAssociationsRequestRequestTypeDef](./type_defs.md#listassistantassociationsrequestrequesttypedef)
- [ListAssistantsRequestRequestTypeDef](./type_defs.md#listassistantsrequestrequesttypedef)
- [ListContentAssociationsRequestRequestTypeDef](./type_defs.md#listcontentassociationsrequestrequesttypedef)
- [ListContentsRequestRequestTypeDef](./type_defs.md#listcontentsrequestrequesttypedef)
- [ListImportJobsRequestRequestTypeDef](./type_defs.md#listimportjobsrequestrequesttypedef)
- [ListKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listknowledgebasesrequestrequesttypedef)
- [ListQuickResponsesRequestRequestTypeDef](./type_defs.md#listquickresponsesrequestrequesttypedef)
- [QuickResponseSummaryTypeDef](./type_defs.md#quickresponsesummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [NotifyRecommendationsReceivedErrorTypeDef](./type_defs.md#notifyrecommendationsreceivederrortypedef)
- [NotifyRecommendationsReceivedRequestRequestTypeDef](./type_defs.md#notifyrecommendationsreceivedrequestrequesttypedef)
- [TagConditionTypeDef](./type_defs.md#tagconditiontypedef)
- [QueryConditionItemTypeDef](./type_defs.md#queryconditionitemtypedef)
- [QueryTextInputDataTypeDef](./type_defs.md#querytextinputdatatypedef)
- [QueryRecommendationTriggerDataTypeDef](./type_defs.md#queryrecommendationtriggerdatatypedef)
- [QuickResponseContentProviderTypeDef](./type_defs.md#quickresponsecontentprovidertypedef)
- [QuickResponseFilterFieldTypeDef](./type_defs.md#quickresponsefilterfieldtypedef)
- [QuickResponseOrderFieldTypeDef](./type_defs.md#quickresponseorderfieldtypedef)
- [QuickResponseQueryFieldTypeDef](./type_defs.md#quickresponsequeryfieldtypedef)
- [RemoveAssistantAIAgentRequestRequestTypeDef](./type_defs.md#removeassistantaiagentrequestrequesttypedef)
- [RemoveKnowledgeBaseTemplateUriRequestRequestTypeDef](./type_defs.md#removeknowledgebasetemplateurirequestrequesttypedef)
- [RuntimeSessionDataValueTypeDef](./type_defs.md#runtimesessiondatavaluetypedef)
- [SessionSummaryTypeDef](./type_defs.md#sessionsummarytypedef)
- [SeedUrlTypeDef](./type_defs.md#seedurltypedef)
- [SessionIntegrationConfigurationTypeDef](./type_defs.md#sessionintegrationconfigurationtypedef)
- [StartContentUploadRequestRequestTypeDef](./type_defs.md#startcontentuploadrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateContentRequestRequestTypeDef](./type_defs.md#updatecontentrequestrequesttypedef)
- [UpdateKnowledgeBaseTemplateUriRequestRequestTypeDef](./type_defs.md#updateknowledgebasetemplateurirequestrequesttypedef)
- [WebCrawlerLimitsTypeDef](./type_defs.md#webcrawlerlimitstypedef)
- [UpdateAssistantAIAgentRequestRequestTypeDef](./type_defs.md#updateassistantaiagentrequestrequesttypedef)
- [AIPromptVersionSummaryTypeDef](./type_defs.md#aipromptversionsummarytypedef)
- [AIPromptTemplateConfigurationTypeDef](./type_defs.md#aiprompttemplateconfigurationtypedef)
- [ContentAssociationContentsTypeDef](./type_defs.md#contentassociationcontentstypedef)
- [AppIntegrationsConfigurationUnionTypeDef](./type_defs.md#appintegrationsconfigurationuniontypedef)
- [CreateAssistantAssociationRequestRequestTypeDef](./type_defs.md#createassistantassociationrequestrequesttypedef)
- [AssistantAssociationOutputDataTypeDef](./type_defs.md#assistantassociationoutputdatatypedef)
- [AssistantDataTypeDef](./type_defs.md#assistantdatatypedef)
- [AssistantSummaryTypeDef](./type_defs.md#assistantsummarytypedef)
- [CreateAssistantRequestRequestTypeDef](./type_defs.md#createassistantrequestrequesttypedef)
- [BedrockFoundationModelConfigurationForParsingTypeDef](./type_defs.md#bedrockfoundationmodelconfigurationforparsingtypedef)
- [ConfigurationTypeDef](./type_defs.md#configurationtypedef)
- [GenerativeDataDetailsPaginatorTypeDef](./type_defs.md#generativedatadetailspaginatortypedef)
- [GenerativeDataDetailsTypeDef](./type_defs.md#generativedatadetailstypedef)
- [ContentFeedbackDataTypeDef](./type_defs.md#contentfeedbackdatatypedef)
- [CreateContentResponseTypeDef](./type_defs.md#createcontentresponsetypedef)
- [GetContentResponseTypeDef](./type_defs.md#getcontentresponsetypedef)
- [GetContentSummaryResponseTypeDef](./type_defs.md#getcontentsummaryresponsetypedef)
- [ListAIPromptsResponseTypeDef](./type_defs.md#listaipromptsresponsetypedef)
- [ListContentsResponseTypeDef](./type_defs.md#listcontentsresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [SearchContentResponseTypeDef](./type_defs.md#searchcontentresponsetypedef)
- [StartContentUploadResponseTypeDef](./type_defs.md#startcontentuploadresponsetypedef)
- [UpdateContentResponseTypeDef](./type_defs.md#updatecontentresponsetypedef)
- [CreateAIAgentVersionRequestRequestTypeDef](./type_defs.md#createaiagentversionrequestrequesttypedef)
- [CreateAIPromptVersionRequestRequestTypeDef](./type_defs.md#createaipromptversionrequestrequesttypedef)
- [CreateQuickResponseRequestRequestTypeDef](./type_defs.md#createquickresponserequestrequesttypedef)
- [UpdateQuickResponseRequestRequestTypeDef](./type_defs.md#updatequickresponserequestrequesttypedef)
- [DataReferenceTypeDef](./type_defs.md#datareferencetypedef)
- [DocumentTextTypeDef](./type_defs.md#documenttexttypedef)
- [SearchExpressionTypeDef](./type_defs.md#searchexpressiontypedef)
- [HierarchicalChunkingConfigurationOutputTypeDef](./type_defs.md#hierarchicalchunkingconfigurationoutputtypedef)
- [HierarchicalChunkingConfigurationTypeDef](./type_defs.md#hierarchicalchunkingconfigurationtypedef)
- [ListAIAgentVersionsRequestListAIAgentVersionsPaginateTypeDef](./type_defs.md#listaiagentversionsrequestlistaiagentversionspaginatetypedef)
- [ListAIAgentsRequestListAIAgentsPaginateTypeDef](./type_defs.md#listaiagentsrequestlistaiagentspaginatetypedef)
- [ListAIPromptVersionsRequestListAIPromptVersionsPaginateTypeDef](./type_defs.md#listaipromptversionsrequestlistaipromptversionspaginatetypedef)
- [ListAIPromptsRequestListAIPromptsPaginateTypeDef](./type_defs.md#listaipromptsrequestlistaipromptspaginatetypedef)
- [ListAssistantAssociationsRequestListAssistantAssociationsPaginateTypeDef](./type_defs.md#listassistantassociationsrequestlistassistantassociationspaginatetypedef)
- [ListAssistantsRequestListAssistantsPaginateTypeDef](./type_defs.md#listassistantsrequestlistassistantspaginatetypedef)
- [ListContentAssociationsRequestListContentAssociationsPaginateTypeDef](./type_defs.md#listcontentassociationsrequestlistcontentassociationspaginatetypedef)
- [ListContentsRequestListContentsPaginateTypeDef](./type_defs.md#listcontentsrequestlistcontentspaginatetypedef)
- [ListImportJobsRequestListImportJobsPaginateTypeDef](./type_defs.md#listimportjobsrequestlistimportjobspaginatetypedef)
- [ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef](./type_defs.md#listknowledgebasesrequestlistknowledgebasespaginatetypedef)
- [ListQuickResponsesRequestListQuickResponsesPaginateTypeDef](./type_defs.md#listquickresponsesrequestlistquickresponsespaginatetypedef)
- [ListQuickResponsesResponseTypeDef](./type_defs.md#listquickresponsesresponsetypedef)
- [NotifyRecommendationsReceivedResponseTypeDef](./type_defs.md#notifyrecommendationsreceivedresponsetypedef)
- [OrConditionOutputTypeDef](./type_defs.md#orconditionoutputtypedef)
- [OrConditionTypeDef](./type_defs.md#orconditiontypedef)
- [QueryConditionTypeDef](./type_defs.md#queryconditiontypedef)
- [QueryInputDataTypeDef](./type_defs.md#queryinputdatatypedef)
- [RecommendationTriggerDataTypeDef](./type_defs.md#recommendationtriggerdatatypedef)
- [QuickResponseContentsTypeDef](./type_defs.md#quickresponsecontentstypedef)
- [QuickResponseSearchExpressionTypeDef](./type_defs.md#quickresponsesearchexpressiontypedef)
- [RuntimeSessionDataTypeDef](./type_defs.md#runtimesessiondatatypedef)
- [SearchSessionsResponseTypeDef](./type_defs.md#searchsessionsresponsetypedef)
- [UrlConfigurationOutputTypeDef](./type_defs.md#urlconfigurationoutputtypedef)
- [UrlConfigurationTypeDef](./type_defs.md#urlconfigurationtypedef)
- [ListAIPromptVersionsResponseTypeDef](./type_defs.md#listaipromptversionsresponsetypedef)
- [AIPromptDataTypeDef](./type_defs.md#aipromptdatatypedef)
- [CreateAIPromptRequestRequestTypeDef](./type_defs.md#createaipromptrequestrequesttypedef)
- [UpdateAIPromptRequestRequestTypeDef](./type_defs.md#updateaipromptrequestrequesttypedef)
- [ContentAssociationDataTypeDef](./type_defs.md#contentassociationdatatypedef)
- [ContentAssociationSummaryTypeDef](./type_defs.md#contentassociationsummarytypedef)
- [CreateContentAssociationRequestRequestTypeDef](./type_defs.md#createcontentassociationrequestrequesttypedef)
- [AssistantAssociationDataTypeDef](./type_defs.md#assistantassociationdatatypedef)
- [AssistantAssociationSummaryTypeDef](./type_defs.md#assistantassociationsummarytypedef)
- [CreateAssistantResponseTypeDef](./type_defs.md#createassistantresponsetypedef)
- [GetAssistantResponseTypeDef](./type_defs.md#getassistantresponsetypedef)
- [UpdateAssistantAIAgentResponseTypeDef](./type_defs.md#updateassistantaiagentresponsetypedef)
- [ListAssistantsResponseTypeDef](./type_defs.md#listassistantsresponsetypedef)
- [ParsingConfigurationTypeDef](./type_defs.md#parsingconfigurationtypedef)
- [ExternalSourceConfigurationTypeDef](./type_defs.md#externalsourceconfigurationtypedef)
- [PutFeedbackRequestRequestTypeDef](./type_defs.md#putfeedbackrequestrequesttypedef)
- [PutFeedbackResponseTypeDef](./type_defs.md#putfeedbackresponsetypedef)
- [DocumentTypeDef](./type_defs.md#documenttypedef)
- [TextDataTypeDef](./type_defs.md#textdatatypedef)
- [SearchContentRequestRequestTypeDef](./type_defs.md#searchcontentrequestrequesttypedef)
- [SearchContentRequestSearchContentPaginateTypeDef](./type_defs.md#searchcontentrequestsearchcontentpaginatetypedef)
- [SearchSessionsRequestRequestTypeDef](./type_defs.md#searchsessionsrequestrequesttypedef)
- [SearchSessionsRequestSearchSessionsPaginateTypeDef](./type_defs.md#searchsessionsrequestsearchsessionspaginatetypedef)
- [ChunkingConfigurationOutputTypeDef](./type_defs.md#chunkingconfigurationoutputtypedef)
- [HierarchicalChunkingConfigurationUnionTypeDef](./type_defs.md#hierarchicalchunkingconfigurationuniontypedef)
- [TagFilterOutputTypeDef](./type_defs.md#tagfilteroutputtypedef)
- [OrConditionUnionTypeDef](./type_defs.md#orconditionuniontypedef)
- [QueryAssistantRequestQueryAssistantPaginateTypeDef](./type_defs.md#queryassistantrequestqueryassistantpaginatetypedef)
- [QueryAssistantRequestRequestTypeDef](./type_defs.md#queryassistantrequestrequesttypedef)
- [RecommendationTriggerTypeDef](./type_defs.md#recommendationtriggertypedef)
- [QuickResponseDataTypeDef](./type_defs.md#quickresponsedatatypedef)
- [QuickResponseSearchResultDataTypeDef](./type_defs.md#quickresponsesearchresultdatatypedef)
- [SearchQuickResponsesRequestRequestTypeDef](./type_defs.md#searchquickresponsesrequestrequesttypedef)
- [SearchQuickResponsesRequestSearchQuickResponsesPaginateTypeDef](./type_defs.md#searchquickresponsesrequestsearchquickresponsespaginatetypedef)
- [UpdateSessionDataRequestRequestTypeDef](./type_defs.md#updatesessiondatarequestrequesttypedef)
- [UpdateSessionDataResponseTypeDef](./type_defs.md#updatesessiondataresponsetypedef)
- [WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef)
- [UrlConfigurationUnionTypeDef](./type_defs.md#urlconfigurationuniontypedef)
- [CreateAIPromptResponseTypeDef](./type_defs.md#createaipromptresponsetypedef)
- [CreateAIPromptVersionResponseTypeDef](./type_defs.md#createaipromptversionresponsetypedef)
- [GetAIPromptResponseTypeDef](./type_defs.md#getaipromptresponsetypedef)
- [UpdateAIPromptResponseTypeDef](./type_defs.md#updateaipromptresponsetypedef)
- [CreateContentAssociationResponseTypeDef](./type_defs.md#createcontentassociationresponsetypedef)
- [GetContentAssociationResponseTypeDef](./type_defs.md#getcontentassociationresponsetypedef)
- [ListContentAssociationsResponseTypeDef](./type_defs.md#listcontentassociationsresponsetypedef)
- [CreateAssistantAssociationResponseTypeDef](./type_defs.md#createassistantassociationresponsetypedef)
- [GetAssistantAssociationResponseTypeDef](./type_defs.md#getassistantassociationresponsetypedef)
- [ListAssistantAssociationsResponseTypeDef](./type_defs.md#listassistantassociationsresponsetypedef)
- [ImportJobDataTypeDef](./type_defs.md#importjobdatatypedef)
- [ImportJobSummaryTypeDef](./type_defs.md#importjobsummarytypedef)
- [StartImportJobRequestRequestTypeDef](./type_defs.md#startimportjobrequestrequesttypedef)
- [ContentDataDetailsTypeDef](./type_defs.md#contentdatadetailstypedef)
- [SourceContentDataDetailsTypeDef](./type_defs.md#sourcecontentdatadetailstypedef)
- [VectorIngestionConfigurationOutputTypeDef](./type_defs.md#vectoringestionconfigurationoutputtypedef)
- [ChunkingConfigurationTypeDef](./type_defs.md#chunkingconfigurationtypedef)
- [KnowledgeBaseAssociationConfigurationDataOutputTypeDef](./type_defs.md#knowledgebaseassociationconfigurationdataoutputtypedef)
- [SessionDataTypeDef](./type_defs.md#sessiondatatypedef)
- [TagFilterTypeDef](./type_defs.md#tagfiltertypedef)
- [CreateQuickResponseResponseTypeDef](./type_defs.md#createquickresponseresponsetypedef)
- [GetQuickResponseResponseTypeDef](./type_defs.md#getquickresponseresponsetypedef)
- [UpdateQuickResponseResponseTypeDef](./type_defs.md#updatequickresponseresponsetypedef)
- [SearchQuickResponsesResponseTypeDef](./type_defs.md#searchquickresponsesresponsetypedef)
- [ManagedSourceConfigurationOutputTypeDef](./type_defs.md#managedsourceconfigurationoutputtypedef)
- [WebCrawlerConfigurationTypeDef](./type_defs.md#webcrawlerconfigurationtypedef)
- [GetImportJobResponseTypeDef](./type_defs.md#getimportjobresponsetypedef)
- [StartImportJobResponseTypeDef](./type_defs.md#startimportjobresponsetypedef)
- [ListImportJobsResponseTypeDef](./type_defs.md#listimportjobsresponsetypedef)
- [DataDetailsPaginatorTypeDef](./type_defs.md#datadetailspaginatortypedef)
- [DataDetailsTypeDef](./type_defs.md#datadetailstypedef)
- [ChunkingConfigurationUnionTypeDef](./type_defs.md#chunkingconfigurationuniontypedef)
- [AssociationConfigurationDataOutputTypeDef](./type_defs.md#associationconfigurationdataoutputtypedef)
- [CreateSessionResponseTypeDef](./type_defs.md#createsessionresponsetypedef)
- [GetSessionResponseTypeDef](./type_defs.md#getsessionresponsetypedef)
- [UpdateSessionResponseTypeDef](./type_defs.md#updatesessionresponsetypedef)
- [CreateSessionRequestRequestTypeDef](./type_defs.md#createsessionrequestrequesttypedef)
- [TagFilterUnionTypeDef](./type_defs.md#tagfilteruniontypedef)
- [UpdateSessionRequestRequestTypeDef](./type_defs.md#updatesessionrequestrequesttypedef)
- [SourceConfigurationOutputTypeDef](./type_defs.md#sourceconfigurationoutputtypedef)
- [WebCrawlerConfigurationUnionTypeDef](./type_defs.md#webcrawlerconfigurationuniontypedef)
- [DataSummaryPaginatorTypeDef](./type_defs.md#datasummarypaginatortypedef)
- [DataSummaryTypeDef](./type_defs.md#datasummarytypedef)
- [VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef)
- [AssociationConfigurationOutputTypeDef](./type_defs.md#associationconfigurationoutputtypedef)
- [KnowledgeBaseAssociationConfigurationDataTypeDef](./type_defs.md#knowledgebaseassociationconfigurationdatatypedef)
- [KnowledgeBaseDataTypeDef](./type_defs.md#knowledgebasedatatypedef)
- [KnowledgeBaseSummaryTypeDef](./type_defs.md#knowledgebasesummarytypedef)
- [ManagedSourceConfigurationTypeDef](./type_defs.md#managedsourceconfigurationtypedef)
- [ResultDataPaginatorTypeDef](./type_defs.md#resultdatapaginatortypedef)
- [RecommendationDataTypeDef](./type_defs.md#recommendationdatatypedef)
- [ResultDataTypeDef](./type_defs.md#resultdatatypedef)
- [AnswerRecommendationAIAgentConfigurationOutputTypeDef](./type_defs.md#answerrecommendationaiagentconfigurationoutputtypedef)
- [ManualSearchAIAgentConfigurationOutputTypeDef](./type_defs.md#manualsearchaiagentconfigurationoutputtypedef)
- [KnowledgeBaseAssociationConfigurationDataUnionTypeDef](./type_defs.md#knowledgebaseassociationconfigurationdatauniontypedef)
- [CreateKnowledgeBaseResponseTypeDef](./type_defs.md#createknowledgebaseresponsetypedef)
- [GetKnowledgeBaseResponseTypeDef](./type_defs.md#getknowledgebaseresponsetypedef)
- [UpdateKnowledgeBaseTemplateUriResponseTypeDef](./type_defs.md#updateknowledgebasetemplateuriresponsetypedef)
- [ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef)
- [ManagedSourceConfigurationUnionTypeDef](./type_defs.md#managedsourceconfigurationuniontypedef)
- [QueryAssistantResponsePaginatorTypeDef](./type_defs.md#queryassistantresponsepaginatortypedef)
- [GetRecommendationsResponseTypeDef](./type_defs.md#getrecommendationsresponsetypedef)
- [QueryAssistantResponseTypeDef](./type_defs.md#queryassistantresponsetypedef)
- [AIAgentConfigurationOutputTypeDef](./type_defs.md#aiagentconfigurationoutputtypedef)
- [AssociationConfigurationDataTypeDef](./type_defs.md#associationconfigurationdatatypedef)
- [SourceConfigurationTypeDef](./type_defs.md#sourceconfigurationtypedef)
- [AIAgentDataTypeDef](./type_defs.md#aiagentdatatypedef)
- [AIAgentSummaryTypeDef](./type_defs.md#aiagentsummarytypedef)
- [AssociationConfigurationDataUnionTypeDef](./type_defs.md#associationconfigurationdatauniontypedef)
- [CreateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#createknowledgebaserequestrequesttypedef)
- [CreateAIAgentResponseTypeDef](./type_defs.md#createaiagentresponsetypedef)
- [CreateAIAgentVersionResponseTypeDef](./type_defs.md#createaiagentversionresponsetypedef)
- [GetAIAgentResponseTypeDef](./type_defs.md#getaiagentresponsetypedef)
- [UpdateAIAgentResponseTypeDef](./type_defs.md#updateaiagentresponsetypedef)
- [AIAgentVersionSummaryTypeDef](./type_defs.md#aiagentversionsummarytypedef)
- [ListAIAgentsResponseTypeDef](./type_defs.md#listaiagentsresponsetypedef)
- [AssociationConfigurationTypeDef](./type_defs.md#associationconfigurationtypedef)
- [ListAIAgentVersionsResponseTypeDef](./type_defs.md#listaiagentversionsresponsetypedef)
- [AssociationConfigurationUnionTypeDef](./type_defs.md#associationconfigurationuniontypedef)
- [ManualSearchAIAgentConfigurationTypeDef](./type_defs.md#manualsearchaiagentconfigurationtypedef)
- [AnswerRecommendationAIAgentConfigurationTypeDef](./type_defs.md#answerrecommendationaiagentconfigurationtypedef)
- [ManualSearchAIAgentConfigurationUnionTypeDef](./type_defs.md#manualsearchaiagentconfigurationuniontypedef)
- [AnswerRecommendationAIAgentConfigurationUnionTypeDef](./type_defs.md#answerrecommendationaiagentconfigurationuniontypedef)
- [AIAgentConfigurationTypeDef](./type_defs.md#aiagentconfigurationtypedef)
- [CreateAIAgentRequestRequestTypeDef](./type_defs.md#createaiagentrequestrequesttypedef)
- [UpdateAIAgentRequestRequestTypeDef](./type_defs.md#updateaiagentrequestrequesttypedef)


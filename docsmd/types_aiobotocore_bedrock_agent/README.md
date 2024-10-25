# AgentsforBedrock module

> [Index](../README.md) > AgentsforBedrock


!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `AgentsforBedrock` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[bedrock-agent]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[bedrock-agent]'


# standalone installation
python -m pip install types-aiobotocore-bedrock-agent
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-bedrock-agent
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AgentsforBedrockClient

Type annotations and code completion for  `#!python session.create_client("bedrock-agent")` as [AgentsforBedrockClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#AgentsforBedrock.Client)

```python
# AgentsforBedrockClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_bedrock_agent.client import AgentsforBedrockClient


session = get_session()
async with session.create_client("bedrock-agent") as client:
    client: AgentsforBedrockClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("bedrock-agent").get_paginator("...")`.

```python
# ListAgentActionGroupsPaginator usage example

from types_aiobotocore_bedrock_agent.paginator import ListAgentActionGroupsPaginator

def get_list_agent_action_groups_paginator() -> ListAgentActionGroupsPaginator:
    return client.get_paginator("list_agent_action_groups"))
```

- [ListAgentActionGroupsPaginator](./paginators.md#listagentactiongroupspaginator)
- [ListAgentAliasesPaginator](./paginators.md#listagentaliasespaginator)
- [ListAgentKnowledgeBasesPaginator](./paginators.md#listagentknowledgebasespaginator)
- [ListAgentVersionsPaginator](./paginators.md#listagentversionspaginator)
- [ListAgentsPaginator](./paginators.md#listagentspaginator)
- [ListDataSourcesPaginator](./paginators.md#listdatasourcespaginator)
- [ListFlowAliasesPaginator](./paginators.md#listflowaliasespaginator)
- [ListFlowVersionsPaginator](./paginators.md#listflowversionspaginator)
- [ListFlowsPaginator](./paginators.md#listflowspaginator)
- [ListIngestionJobsPaginator](./paginators.md#listingestionjobspaginator)
- [ListKnowledgeBasesPaginator](./paginators.md#listknowledgebasespaginator)
- [ListPromptsPaginator](./paginators.md#listpromptspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionGroupSignatureType usage example

from types_aiobotocore_bedrock_agent.literals import ActionGroupSignatureType

def get_value() -> ActionGroupSignatureType:
    return "AMAZON.CodeInterpreter"
```

- [ActionGroupSignatureType](./literals.md#actiongroupsignaturetype)
- [ActionGroupStateType](./literals.md#actiongroupstatetype)
- [AgentAliasStatusType](./literals.md#agentaliasstatustype)
- [AgentStatusType](./literals.md#agentstatustype)
- [ChunkingStrategyType](./literals.md#chunkingstrategytype)
- [ConfluenceAuthTypeType](./literals.md#confluenceauthtypetype)
- [ConfluenceHostTypeType](./literals.md#confluencehosttypetype)
- [CrawlFilterConfigurationTypeType](./literals.md#crawlfilterconfigurationtypetype)
- [CreationModeType](./literals.md#creationmodetype)
- [CustomControlMethodType](./literals.md#customcontrolmethodtype)
- [DataDeletionPolicyType](./literals.md#datadeletionpolicytype)
- [DataSourceStatusType](./literals.md#datasourcestatustype)
- [DataSourceTypeType](./literals.md#datasourcetypetype)
- [FlowConnectionTypeType](./literals.md#flowconnectiontypetype)
- [FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype)
- [FlowNodeTypeType](./literals.md#flownodetypetype)
- [FlowStatusType](./literals.md#flowstatustype)
- [FlowValidationSeverityType](./literals.md#flowvalidationseveritytype)
- [IngestionJobFilterAttributeType](./literals.md#ingestionjobfilterattributetype)
- [IngestionJobFilterOperatorType](./literals.md#ingestionjobfilteroperatortype)
- [IngestionJobSortByAttributeType](./literals.md#ingestionjobsortbyattributetype)
- [IngestionJobStatusType](./literals.md#ingestionjobstatustype)
- [KnowledgeBaseStateType](./literals.md#knowledgebasestatetype)
- [KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype)
- [KnowledgeBaseStorageTypeType](./literals.md#knowledgebasestoragetypetype)
- [KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype)
- [ListAgentActionGroupsPaginatorName](./literals.md#listagentactiongroupspaginatorname)
- [ListAgentAliasesPaginatorName](./literals.md#listagentaliasespaginatorname)
- [ListAgentKnowledgeBasesPaginatorName](./literals.md#listagentknowledgebasespaginatorname)
- [ListAgentVersionsPaginatorName](./literals.md#listagentversionspaginatorname)
- [ListAgentsPaginatorName](./literals.md#listagentspaginatorname)
- [ListDataSourcesPaginatorName](./literals.md#listdatasourcespaginatorname)
- [ListFlowAliasesPaginatorName](./literals.md#listflowaliasespaginatorname)
- [ListFlowVersionsPaginatorName](./literals.md#listflowversionspaginatorname)
- [ListFlowsPaginatorName](./literals.md#listflowspaginatorname)
- [ListIngestionJobsPaginatorName](./literals.md#listingestionjobspaginatorname)
- [ListKnowledgeBasesPaginatorName](./literals.md#listknowledgebasespaginatorname)
- [ListPromptsPaginatorName](./literals.md#listpromptspaginatorname)
- [MemoryTypeType](./literals.md#memorytypetype)
- [ParsingStrategyType](./literals.md#parsingstrategytype)
- [PromptStateType](./literals.md#promptstatetype)
- [PromptTemplateTypeType](./literals.md#prompttemplatetypetype)
- [PromptTypeType](./literals.md#prompttypetype)
- [RequireConfirmationType](./literals.md#requireconfirmationtype)
- [SalesforceAuthTypeType](./literals.md#salesforceauthtypetype)
- [SharePointAuthTypeType](./literals.md#sharepointauthtypetype)
- [SharePointHostTypeType](./literals.md#sharepointhosttypetype)
- [SortOrderType](./literals.md#sortordertype)
- [StepTypeType](./literals.md#steptypetype)
- [TypeType](./literals.md#typetype)
- [WebScopeTypeType](./literals.md#webscopetypetype)
- [AgentsforBedrockServiceName](./literals.md#agentsforbedrockservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [S3IdentifierTypeDef](./type_defs.md#s3identifiertypedef)
- [ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef)
- [ActionGroupSummaryTypeDef](./type_defs.md#actiongroupsummarytypedef)
- [AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef)
- [AgentFlowNodeConfigurationTypeDef](./type_defs.md#agentflownodeconfigurationtypedef)
- [AgentKnowledgeBaseSummaryTypeDef](./type_defs.md#agentknowledgebasesummarytypedef)
- [AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef)
- [GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef)
- [MemoryConfigurationOutputTypeDef](./type_defs.md#memoryconfigurationoutputtypedef)
- [AssociateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#associateagentknowledgebaserequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BedrockEmbeddingModelConfigurationTypeDef](./type_defs.md#bedrockembeddingmodelconfigurationtypedef)
- [ParsingPromptTypeDef](./type_defs.md#parsingprompttypedef)
- [FixedSizeChunkingConfigurationTypeDef](./type_defs.md#fixedsizechunkingconfigurationtypedef)
- [SemanticChunkingConfigurationTypeDef](./type_defs.md#semanticchunkingconfigurationtypedef)
- [FlowConditionTypeDef](./type_defs.md#flowconditiontypedef)
- [ConfluenceSourceConfigurationTypeDef](./type_defs.md#confluencesourceconfigurationtypedef)
- [MemoryConfigurationTypeDef](./type_defs.md#memoryconfigurationtypedef)
- [ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef)
- [FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef)
- [CreateFlowVersionRequestRequestTypeDef](./type_defs.md#createflowversionrequestrequesttypedef)
- [CreatePromptVersionRequestRequestTypeDef](./type_defs.md#createpromptversionrequestrequesttypedef)
- [S3DataSourceConfigurationOutputTypeDef](./type_defs.md#s3datasourceconfigurationoutputtypedef)
- [DataSourceSummaryTypeDef](./type_defs.md#datasourcesummarytypedef)
- [DeleteAgentActionGroupRequestRequestTypeDef](./type_defs.md#deleteagentactiongrouprequestrequesttypedef)
- [DeleteAgentAliasRequestRequestTypeDef](./type_defs.md#deleteagentaliasrequestrequesttypedef)
- [DeleteAgentRequestRequestTypeDef](./type_defs.md#deleteagentrequestrequesttypedef)
- [DeleteAgentVersionRequestRequestTypeDef](./type_defs.md#deleteagentversionrequestrequesttypedef)
- [DeleteDataSourceRequestRequestTypeDef](./type_defs.md#deletedatasourcerequestrequesttypedef)
- [DeleteFlowAliasRequestRequestTypeDef](./type_defs.md#deleteflowaliasrequestrequesttypedef)
- [DeleteFlowRequestRequestTypeDef](./type_defs.md#deleteflowrequestrequesttypedef)
- [DeleteFlowVersionRequestRequestTypeDef](./type_defs.md#deleteflowversionrequestrequesttypedef)
- [DeleteKnowledgeBaseRequestRequestTypeDef](./type_defs.md#deleteknowledgebaserequestrequesttypedef)
- [DeletePromptRequestRequestTypeDef](./type_defs.md#deletepromptrequestrequesttypedef)
- [DisassociateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#disassociateagentknowledgebaserequestrequesttypedef)
- [FlowConditionalConnectionConfigurationTypeDef](./type_defs.md#flowconditionalconnectionconfigurationtypedef)
- [FlowDataConnectionConfigurationTypeDef](./type_defs.md#flowdataconnectionconfigurationtypedef)
- [KnowledgeBaseFlowNodeConfigurationTypeDef](./type_defs.md#knowledgebaseflownodeconfigurationtypedef)
- [LambdaFunctionFlowNodeConfigurationTypeDef](./type_defs.md#lambdafunctionflownodeconfigurationtypedef)
- [LexFlowNodeConfigurationTypeDef](./type_defs.md#lexflownodeconfigurationtypedef)
- [FlowNodeInputTypeDef](./type_defs.md#flownodeinputtypedef)
- [FlowNodeOutputTypeDef](./type_defs.md#flownodeoutputtypedef)
- [FlowSummaryTypeDef](./type_defs.md#flowsummarytypedef)
- [FlowValidationTypeDef](./type_defs.md#flowvalidationtypedef)
- [FlowVersionSummaryTypeDef](./type_defs.md#flowversionsummarytypedef)
- [ParameterDetailTypeDef](./type_defs.md#parameterdetailtypedef)
- [GetAgentActionGroupRequestRequestTypeDef](./type_defs.md#getagentactiongrouprequestrequesttypedef)
- [GetAgentAliasRequestRequestTypeDef](./type_defs.md#getagentaliasrequestrequesttypedef)
- [GetAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getagentknowledgebaserequestrequesttypedef)
- [GetAgentRequestRequestTypeDef](./type_defs.md#getagentrequestrequesttypedef)
- [GetAgentVersionRequestRequestTypeDef](./type_defs.md#getagentversionrequestrequesttypedef)
- [GetDataSourceRequestRequestTypeDef](./type_defs.md#getdatasourcerequestrequesttypedef)
- [GetFlowAliasRequestRequestTypeDef](./type_defs.md#getflowaliasrequestrequesttypedef)
- [GetFlowRequestRequestTypeDef](./type_defs.md#getflowrequestrequesttypedef)
- [GetFlowVersionRequestRequestTypeDef](./type_defs.md#getflowversionrequestrequesttypedef)
- [GetIngestionJobRequestRequestTypeDef](./type_defs.md#getingestionjobrequestrequesttypedef)
- [GetKnowledgeBaseRequestRequestTypeDef](./type_defs.md#getknowledgebaserequestrequesttypedef)
- [GetPromptRequestRequestTypeDef](./type_defs.md#getpromptrequestrequesttypedef)
- [HierarchicalChunkingLevelConfigurationTypeDef](./type_defs.md#hierarchicalchunkinglevelconfigurationtypedef)
- [InferenceConfigurationOutputTypeDef](./type_defs.md#inferenceconfigurationoutputtypedef)
- [InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef)
- [IngestionJobFilterTypeDef](./type_defs.md#ingestionjobfiltertypedef)
- [IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef)
- [IngestionJobStatisticsTypeDef](./type_defs.md#ingestionjobstatisticstypedef)
- [S3LocationTypeDef](./type_defs.md#s3locationtypedef)
- [KnowledgeBaseSummaryTypeDef](./type_defs.md#knowledgebasesummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAgentActionGroupsRequestRequestTypeDef](./type_defs.md#listagentactiongroupsrequestrequesttypedef)
- [ListAgentAliasesRequestRequestTypeDef](./type_defs.md#listagentaliasesrequestrequesttypedef)
- [ListAgentKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listagentknowledgebasesrequestrequesttypedef)
- [ListAgentVersionsRequestRequestTypeDef](./type_defs.md#listagentversionsrequestrequesttypedef)
- [ListAgentsRequestRequestTypeDef](./type_defs.md#listagentsrequestrequesttypedef)
- [ListDataSourcesRequestRequestTypeDef](./type_defs.md#listdatasourcesrequestrequesttypedef)
- [ListFlowAliasesRequestRequestTypeDef](./type_defs.md#listflowaliasesrequestrequesttypedef)
- [ListFlowVersionsRequestRequestTypeDef](./type_defs.md#listflowversionsrequestrequesttypedef)
- [ListFlowsRequestRequestTypeDef](./type_defs.md#listflowsrequestrequesttypedef)
- [ListKnowledgeBasesRequestRequestTypeDef](./type_defs.md#listknowledgebasesrequestrequesttypedef)
- [ListPromptsRequestRequestTypeDef](./type_defs.md#listpromptsrequestrequesttypedef)
- [PromptSummaryTypeDef](./type_defs.md#promptsummarytypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [MongoDbAtlasFieldMappingTypeDef](./type_defs.md#mongodbatlasfieldmappingtypedef)
- [OpenSearchServerlessFieldMappingTypeDef](./type_defs.md#opensearchserverlessfieldmappingtypedef)
- [PatternObjectFilterOutputTypeDef](./type_defs.md#patternobjectfilteroutputtypedef)
- [PatternObjectFilterTypeDef](./type_defs.md#patternobjectfiltertypedef)
- [PineconeFieldMappingTypeDef](./type_defs.md#pineconefieldmappingtypedef)
- [PrepareAgentRequestRequestTypeDef](./type_defs.md#prepareagentrequestrequesttypedef)
- [PrepareFlowRequestRequestTypeDef](./type_defs.md#prepareflowrequestrequesttypedef)
- [PromptFlowNodeResourceConfigurationTypeDef](./type_defs.md#promptflownoderesourceconfigurationtypedef)
- [PromptModelInferenceConfigurationOutputTypeDef](./type_defs.md#promptmodelinferenceconfigurationoutputtypedef)
- [PromptInputVariableTypeDef](./type_defs.md#promptinputvariabletypedef)
- [PromptMetadataEntryTypeDef](./type_defs.md#promptmetadataentrytypedef)
- [PromptModelInferenceConfigurationTypeDef](./type_defs.md#promptmodelinferenceconfigurationtypedef)
- [RdsFieldMappingTypeDef](./type_defs.md#rdsfieldmappingtypedef)
- [RedisEnterpriseCloudFieldMappingTypeDef](./type_defs.md#redisenterprisecloudfieldmappingtypedef)
- [RetrievalFlowNodeS3ConfigurationTypeDef](./type_defs.md#retrievalflownodes3configurationtypedef)
- [S3DataSourceConfigurationTypeDef](./type_defs.md#s3datasourceconfigurationtypedef)
- [SalesforceSourceConfigurationTypeDef](./type_defs.md#salesforcesourceconfigurationtypedef)
- [SeedUrlTypeDef](./type_defs.md#seedurltypedef)
- [SharePointSourceConfigurationOutputTypeDef](./type_defs.md#sharepointsourceconfigurationoutputtypedef)
- [SharePointSourceConfigurationTypeDef](./type_defs.md#sharepointsourceconfigurationtypedef)
- [StartIngestionJobRequestRequestTypeDef](./type_defs.md#startingestionjobrequestrequesttypedef)
- [StopIngestionJobRequestRequestTypeDef](./type_defs.md#stopingestionjobrequestrequesttypedef)
- [StorageFlowNodeS3ConfigurationTypeDef](./type_defs.md#storageflownodes3configurationtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [TransformationLambdaConfigurationTypeDef](./type_defs.md#transformationlambdaconfigurationtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAgentKnowledgeBaseRequestRequestTypeDef](./type_defs.md#updateagentknowledgebaserequestrequesttypedef)
- [WebCrawlerLimitsTypeDef](./type_defs.md#webcrawlerlimitstypedef)
- [APISchemaTypeDef](./type_defs.md#apischematypedef)
- [AgentAliasHistoryEventTypeDef](./type_defs.md#agentaliashistoryeventtypedef)
- [AgentAliasSummaryTypeDef](./type_defs.md#agentaliassummarytypedef)
- [CreateAgentAliasRequestRequestTypeDef](./type_defs.md#createagentaliasrequestrequesttypedef)
- [UpdateAgentAliasRequestRequestTypeDef](./type_defs.md#updateagentaliasrequestrequesttypedef)
- [AgentSummaryTypeDef](./type_defs.md#agentsummarytypedef)
- [AgentVersionSummaryTypeDef](./type_defs.md#agentversionsummarytypedef)
- [AssociateAgentKnowledgeBaseResponseTypeDef](./type_defs.md#associateagentknowledgebaseresponsetypedef)
- [DeleteAgentAliasResponseTypeDef](./type_defs.md#deleteagentaliasresponsetypedef)
- [DeleteAgentResponseTypeDef](./type_defs.md#deleteagentresponsetypedef)
- [DeleteAgentVersionResponseTypeDef](./type_defs.md#deleteagentversionresponsetypedef)
- [DeleteDataSourceResponseTypeDef](./type_defs.md#deletedatasourceresponsetypedef)
- [DeleteFlowAliasResponseTypeDef](./type_defs.md#deleteflowaliasresponsetypedef)
- [DeleteFlowResponseTypeDef](./type_defs.md#deleteflowresponsetypedef)
- [DeleteFlowVersionResponseTypeDef](./type_defs.md#deleteflowversionresponsetypedef)
- [DeleteKnowledgeBaseResponseTypeDef](./type_defs.md#deleteknowledgebaseresponsetypedef)
- [DeletePromptResponseTypeDef](./type_defs.md#deletepromptresponsetypedef)
- [GetAgentKnowledgeBaseResponseTypeDef](./type_defs.md#getagentknowledgebaseresponsetypedef)
- [ListAgentActionGroupsResponseTypeDef](./type_defs.md#listagentactiongroupsresponsetypedef)
- [ListAgentKnowledgeBasesResponseTypeDef](./type_defs.md#listagentknowledgebasesresponsetypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [PrepareAgentResponseTypeDef](./type_defs.md#prepareagentresponsetypedef)
- [PrepareFlowResponseTypeDef](./type_defs.md#prepareflowresponsetypedef)
- [UpdateAgentKnowledgeBaseResponseTypeDef](./type_defs.md#updateagentknowledgebaseresponsetypedef)
- [EmbeddingModelConfigurationTypeDef](./type_defs.md#embeddingmodelconfigurationtypedef)
- [BedrockFoundationModelConfigurationTypeDef](./type_defs.md#bedrockfoundationmodelconfigurationtypedef)
- [ConditionFlowNodeConfigurationOutputTypeDef](./type_defs.md#conditionflownodeconfigurationoutputtypedef)
- [ConditionFlowNodeConfigurationTypeDef](./type_defs.md#conditionflownodeconfigurationtypedef)
- [CreateFlowAliasRequestRequestTypeDef](./type_defs.md#createflowaliasrequestrequesttypedef)
- [CreateFlowAliasResponseTypeDef](./type_defs.md#createflowaliasresponsetypedef)
- [FlowAliasSummaryTypeDef](./type_defs.md#flowaliassummarytypedef)
- [GetFlowAliasResponseTypeDef](./type_defs.md#getflowaliasresponsetypedef)
- [UpdateFlowAliasRequestRequestTypeDef](./type_defs.md#updateflowaliasrequestrequesttypedef)
- [UpdateFlowAliasResponseTypeDef](./type_defs.md#updateflowaliasresponsetypedef)
- [ListDataSourcesResponseTypeDef](./type_defs.md#listdatasourcesresponsetypedef)
- [FlowConnectionConfigurationTypeDef](./type_defs.md#flowconnectionconfigurationtypedef)
- [ListFlowsResponseTypeDef](./type_defs.md#listflowsresponsetypedef)
- [ListFlowVersionsResponseTypeDef](./type_defs.md#listflowversionsresponsetypedef)
- [FunctionOutputTypeDef](./type_defs.md#functionoutputtypedef)
- [FunctionTypeDef](./type_defs.md#functiontypedef)
- [HierarchicalChunkingConfigurationOutputTypeDef](./type_defs.md#hierarchicalchunkingconfigurationoutputtypedef)
- [HierarchicalChunkingConfigurationTypeDef](./type_defs.md#hierarchicalchunkingconfigurationtypedef)
- [PromptConfigurationOutputTypeDef](./type_defs.md#promptconfigurationoutputtypedef)
- [InferenceConfigurationUnionTypeDef](./type_defs.md#inferenceconfigurationuniontypedef)
- [ListIngestionJobsRequestRequestTypeDef](./type_defs.md#listingestionjobsrequestrequesttypedef)
- [IngestionJobSummaryTypeDef](./type_defs.md#ingestionjobsummarytypedef)
- [IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef)
- [IntermediateStorageTypeDef](./type_defs.md#intermediatestoragetypedef)
- [ListKnowledgeBasesResponseTypeDef](./type_defs.md#listknowledgebasesresponsetypedef)
- [ListAgentActionGroupsRequestListAgentActionGroupsPaginateTypeDef](./type_defs.md#listagentactiongroupsrequestlistagentactiongroupspaginatetypedef)
- [ListAgentAliasesRequestListAgentAliasesPaginateTypeDef](./type_defs.md#listagentaliasesrequestlistagentaliasespaginatetypedef)
- [ListAgentKnowledgeBasesRequestListAgentKnowledgeBasesPaginateTypeDef](./type_defs.md#listagentknowledgebasesrequestlistagentknowledgebasespaginatetypedef)
- [ListAgentVersionsRequestListAgentVersionsPaginateTypeDef](./type_defs.md#listagentversionsrequestlistagentversionspaginatetypedef)
- [ListAgentsRequestListAgentsPaginateTypeDef](./type_defs.md#listagentsrequestlistagentspaginatetypedef)
- [ListDataSourcesRequestListDataSourcesPaginateTypeDef](./type_defs.md#listdatasourcesrequestlistdatasourcespaginatetypedef)
- [ListFlowAliasesRequestListFlowAliasesPaginateTypeDef](./type_defs.md#listflowaliasesrequestlistflowaliasespaginatetypedef)
- [ListFlowVersionsRequestListFlowVersionsPaginateTypeDef](./type_defs.md#listflowversionsrequestlistflowversionspaginatetypedef)
- [ListFlowsRequestListFlowsPaginateTypeDef](./type_defs.md#listflowsrequestlistflowspaginatetypedef)
- [ListIngestionJobsRequestListIngestionJobsPaginateTypeDef](./type_defs.md#listingestionjobsrequestlistingestionjobspaginatetypedef)
- [ListKnowledgeBasesRequestListKnowledgeBasesPaginateTypeDef](./type_defs.md#listknowledgebasesrequestlistknowledgebasespaginatetypedef)
- [ListPromptsRequestListPromptsPaginateTypeDef](./type_defs.md#listpromptsrequestlistpromptspaginatetypedef)
- [ListPromptsResponseTypeDef](./type_defs.md#listpromptsresponsetypedef)
- [MongoDbAtlasConfigurationTypeDef](./type_defs.md#mongodbatlasconfigurationtypedef)
- [OpenSearchServerlessConfigurationTypeDef](./type_defs.md#opensearchserverlessconfigurationtypedef)
- [PatternObjectFilterConfigurationOutputTypeDef](./type_defs.md#patternobjectfilterconfigurationoutputtypedef)
- [PatternObjectFilterUnionTypeDef](./type_defs.md#patternobjectfilteruniontypedef)
- [PineconeConfigurationTypeDef](./type_defs.md#pineconeconfigurationtypedef)
- [PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef)
- [TextPromptTemplateConfigurationOutputTypeDef](./type_defs.md#textprompttemplateconfigurationoutputtypedef)
- [TextPromptTemplateConfigurationTypeDef](./type_defs.md#textprompttemplateconfigurationtypedef)
- [PromptModelInferenceConfigurationUnionTypeDef](./type_defs.md#promptmodelinferenceconfigurationuniontypedef)
- [RdsConfigurationTypeDef](./type_defs.md#rdsconfigurationtypedef)
- [RedisEnterpriseCloudConfigurationTypeDef](./type_defs.md#redisenterprisecloudconfigurationtypedef)
- [RetrievalFlowNodeServiceConfigurationTypeDef](./type_defs.md#retrievalflownodeserviceconfigurationtypedef)
- [S3DataSourceConfigurationUnionTypeDef](./type_defs.md#s3datasourceconfigurationuniontypedef)
- [UrlConfigurationOutputTypeDef](./type_defs.md#urlconfigurationoutputtypedef)
- [UrlConfigurationTypeDef](./type_defs.md#urlconfigurationtypedef)
- [SharePointSourceConfigurationUnionTypeDef](./type_defs.md#sharepointsourceconfigurationuniontypedef)
- [StorageFlowNodeServiceConfigurationTypeDef](./type_defs.md#storageflownodeserviceconfigurationtypedef)
- [TransformationFunctionTypeDef](./type_defs.md#transformationfunctiontypedef)
- [WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef)
- [WebCrawlerConfigurationTypeDef](./type_defs.md#webcrawlerconfigurationtypedef)
- [AgentAliasTypeDef](./type_defs.md#agentaliastypedef)
- [ListAgentAliasesResponseTypeDef](./type_defs.md#listagentaliasesresponsetypedef)
- [ListAgentsResponseTypeDef](./type_defs.md#listagentsresponsetypedef)
- [ListAgentVersionsResponseTypeDef](./type_defs.md#listagentversionsresponsetypedef)
- [VectorKnowledgeBaseConfigurationTypeDef](./type_defs.md#vectorknowledgebaseconfigurationtypedef)
- [ParsingConfigurationTypeDef](./type_defs.md#parsingconfigurationtypedef)
- [ConditionFlowNodeConfigurationUnionTypeDef](./type_defs.md#conditionflownodeconfigurationuniontypedef)
- [ListFlowAliasesResponseTypeDef](./type_defs.md#listflowaliasesresponsetypedef)
- [FlowConnectionTypeDef](./type_defs.md#flowconnectiontypedef)
- [FunctionSchemaOutputTypeDef](./type_defs.md#functionschemaoutputtypedef)
- [FunctionUnionTypeDef](./type_defs.md#functionuniontypedef)
- [ChunkingConfigurationOutputTypeDef](./type_defs.md#chunkingconfigurationoutputtypedef)
- [HierarchicalChunkingConfigurationUnionTypeDef](./type_defs.md#hierarchicalchunkingconfigurationuniontypedef)
- [PromptOverrideConfigurationOutputTypeDef](./type_defs.md#promptoverrideconfigurationoutputtypedef)
- [PromptConfigurationTypeDef](./type_defs.md#promptconfigurationtypedef)
- [ListIngestionJobsResponseTypeDef](./type_defs.md#listingestionjobsresponsetypedef)
- [GetIngestionJobResponseTypeDef](./type_defs.md#getingestionjobresponsetypedef)
- [StartIngestionJobResponseTypeDef](./type_defs.md#startingestionjobresponsetypedef)
- [StopIngestionJobResponseTypeDef](./type_defs.md#stopingestionjobresponsetypedef)
- [CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef)
- [PatternObjectFilterConfigurationTypeDef](./type_defs.md#patternobjectfilterconfigurationtypedef)
- [PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef)
- [TextPromptTemplateConfigurationUnionTypeDef](./type_defs.md#textprompttemplateconfigurationuniontypedef)
- [PromptInferenceConfigurationTypeDef](./type_defs.md#promptinferenceconfigurationtypedef)
- [StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef)
- [RetrievalFlowNodeConfigurationTypeDef](./type_defs.md#retrievalflownodeconfigurationtypedef)
- [WebSourceConfigurationOutputTypeDef](./type_defs.md#websourceconfigurationoutputtypedef)
- [UrlConfigurationUnionTypeDef](./type_defs.md#urlconfigurationuniontypedef)
- [StorageFlowNodeConfigurationTypeDef](./type_defs.md#storageflownodeconfigurationtypedef)
- [TransformationTypeDef](./type_defs.md#transformationtypedef)
- [WebCrawlerConfigurationUnionTypeDef](./type_defs.md#webcrawlerconfigurationuniontypedef)
- [CreateAgentAliasResponseTypeDef](./type_defs.md#createagentaliasresponsetypedef)
- [GetAgentAliasResponseTypeDef](./type_defs.md#getagentaliasresponsetypedef)
- [UpdateAgentAliasResponseTypeDef](./type_defs.md#updateagentaliasresponsetypedef)
- [KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef)
- [AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef)
- [FunctionSchemaTypeDef](./type_defs.md#functionschematypedef)
- [ChunkingConfigurationTypeDef](./type_defs.md#chunkingconfigurationtypedef)
- [AgentTypeDef](./type_defs.md#agenttypedef)
- [AgentVersionTypeDef](./type_defs.md#agentversiontypedef)
- [PromptConfigurationUnionTypeDef](./type_defs.md#promptconfigurationuniontypedef)
- [ConfluenceCrawlerConfigurationOutputTypeDef](./type_defs.md#confluencecrawlerconfigurationoutputtypedef)
- [SalesforceCrawlerConfigurationOutputTypeDef](./type_defs.md#salesforcecrawlerconfigurationoutputtypedef)
- [SharePointCrawlerConfigurationOutputTypeDef](./type_defs.md#sharepointcrawlerconfigurationoutputtypedef)
- [PatternObjectFilterConfigurationUnionTypeDef](./type_defs.md#patternobjectfilterconfigurationuniontypedef)
- [PromptFlowNodeInlineConfigurationOutputTypeDef](./type_defs.md#promptflownodeinlineconfigurationoutputtypedef)
- [PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef)
- [PromptTemplateConfigurationTypeDef](./type_defs.md#prompttemplateconfigurationtypedef)
- [PromptInferenceConfigurationUnionTypeDef](./type_defs.md#promptinferenceconfigurationuniontypedef)
- [WebDataSourceConfigurationOutputTypeDef](./type_defs.md#webdatasourceconfigurationoutputtypedef)
- [WebSourceConfigurationTypeDef](./type_defs.md#websourceconfigurationtypedef)
- [CustomTransformationConfigurationOutputTypeDef](./type_defs.md#customtransformationconfigurationoutputtypedef)
- [CustomTransformationConfigurationTypeDef](./type_defs.md#customtransformationconfigurationtypedef)
- [CreateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#createknowledgebaserequestrequesttypedef)
- [KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef)
- [UpdateKnowledgeBaseRequestRequestTypeDef](./type_defs.md#updateknowledgebaserequestrequesttypedef)
- [CreateAgentActionGroupResponseTypeDef](./type_defs.md#createagentactiongroupresponsetypedef)
- [GetAgentActionGroupResponseTypeDef](./type_defs.md#getagentactiongroupresponsetypedef)
- [UpdateAgentActionGroupResponseTypeDef](./type_defs.md#updateagentactiongroupresponsetypedef)
- [CreateAgentActionGroupRequestRequestTypeDef](./type_defs.md#createagentactiongrouprequestrequesttypedef)
- [UpdateAgentActionGroupRequestRequestTypeDef](./type_defs.md#updateagentactiongrouprequestrequesttypedef)
- [ChunkingConfigurationUnionTypeDef](./type_defs.md#chunkingconfigurationuniontypedef)
- [CreateAgentResponseTypeDef](./type_defs.md#createagentresponsetypedef)
- [GetAgentResponseTypeDef](./type_defs.md#getagentresponsetypedef)
- [UpdateAgentResponseTypeDef](./type_defs.md#updateagentresponsetypedef)
- [GetAgentVersionResponseTypeDef](./type_defs.md#getagentversionresponsetypedef)
- [PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef)
- [ConfluenceDataSourceConfigurationOutputTypeDef](./type_defs.md#confluencedatasourceconfigurationoutputtypedef)
- [SalesforceDataSourceConfigurationOutputTypeDef](./type_defs.md#salesforcedatasourceconfigurationoutputtypedef)
- [SharePointDataSourceConfigurationOutputTypeDef](./type_defs.md#sharepointdatasourceconfigurationoutputtypedef)
- [CrawlFilterConfigurationTypeDef](./type_defs.md#crawlfilterconfigurationtypedef)
- [PromptFlowNodeSourceConfigurationOutputTypeDef](./type_defs.md#promptflownodesourceconfigurationoutputtypedef)
- [CreatePromptResponseTypeDef](./type_defs.md#createpromptresponsetypedef)
- [CreatePromptVersionResponseTypeDef](./type_defs.md#createpromptversionresponsetypedef)
- [GetPromptResponseTypeDef](./type_defs.md#getpromptresponsetypedef)
- [UpdatePromptResponseTypeDef](./type_defs.md#updatepromptresponsetypedef)
- [PromptTemplateConfigurationUnionTypeDef](./type_defs.md#prompttemplateconfigurationuniontypedef)
- [WebSourceConfigurationUnionTypeDef](./type_defs.md#websourceconfigurationuniontypedef)
- [VectorIngestionConfigurationOutputTypeDef](./type_defs.md#vectoringestionconfigurationoutputtypedef)
- [CustomTransformationConfigurationUnionTypeDef](./type_defs.md#customtransformationconfigurationuniontypedef)
- [CreateKnowledgeBaseResponseTypeDef](./type_defs.md#createknowledgebaseresponsetypedef)
- [GetKnowledgeBaseResponseTypeDef](./type_defs.md#getknowledgebaseresponsetypedef)
- [UpdateKnowledgeBaseResponseTypeDef](./type_defs.md#updateknowledgebaseresponsetypedef)
- [CreateAgentRequestRequestTypeDef](./type_defs.md#createagentrequestrequesttypedef)
- [UpdateAgentRequestRequestTypeDef](./type_defs.md#updateagentrequestrequesttypedef)
- [DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef)
- [CrawlFilterConfigurationUnionTypeDef](./type_defs.md#crawlfilterconfigurationuniontypedef)
- [PromptFlowNodeConfigurationOutputTypeDef](./type_defs.md#promptflownodeconfigurationoutputtypedef)
- [PromptFlowNodeInlineConfigurationTypeDef](./type_defs.md#promptflownodeinlineconfigurationtypedef)
- [PromptVariantTypeDef](./type_defs.md#promptvarianttypedef)
- [WebDataSourceConfigurationTypeDef](./type_defs.md#webdatasourceconfigurationtypedef)
- [VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef)
- [DataSourceTypeDef](./type_defs.md#datasourcetypedef)
- [ConfluenceCrawlerConfigurationTypeDef](./type_defs.md#confluencecrawlerconfigurationtypedef)
- [SalesforceCrawlerConfigurationTypeDef](./type_defs.md#salesforcecrawlerconfigurationtypedef)
- [SharePointCrawlerConfigurationTypeDef](./type_defs.md#sharepointcrawlerconfigurationtypedef)
- [FlowNodeConfigurationOutputTypeDef](./type_defs.md#flownodeconfigurationoutputtypedef)
- [PromptFlowNodeInlineConfigurationUnionTypeDef](./type_defs.md#promptflownodeinlineconfigurationuniontypedef)
- [PromptVariantUnionTypeDef](./type_defs.md#promptvariantuniontypedef)
- [UpdatePromptRequestRequestTypeDef](./type_defs.md#updatepromptrequestrequesttypedef)
- [WebDataSourceConfigurationUnionTypeDef](./type_defs.md#webdatasourceconfigurationuniontypedef)
- [CreateDataSourceResponseTypeDef](./type_defs.md#createdatasourceresponsetypedef)
- [GetDataSourceResponseTypeDef](./type_defs.md#getdatasourceresponsetypedef)
- [UpdateDataSourceResponseTypeDef](./type_defs.md#updatedatasourceresponsetypedef)
- [ConfluenceCrawlerConfigurationUnionTypeDef](./type_defs.md#confluencecrawlerconfigurationuniontypedef)
- [SalesforceCrawlerConfigurationUnionTypeDef](./type_defs.md#salesforcecrawlerconfigurationuniontypedef)
- [SharePointCrawlerConfigurationUnionTypeDef](./type_defs.md#sharepointcrawlerconfigurationuniontypedef)
- [FlowNodeExtraOutputTypeDef](./type_defs.md#flownodeextraoutputtypedef)
- [PromptFlowNodeSourceConfigurationTypeDef](./type_defs.md#promptflownodesourceconfigurationtypedef)
- [CreatePromptRequestRequestTypeDef](./type_defs.md#createpromptrequestrequesttypedef)
- [ConfluenceDataSourceConfigurationTypeDef](./type_defs.md#confluencedatasourceconfigurationtypedef)
- [SalesforceDataSourceConfigurationTypeDef](./type_defs.md#salesforcedatasourceconfigurationtypedef)
- [SharePointDataSourceConfigurationTypeDef](./type_defs.md#sharepointdatasourceconfigurationtypedef)
- [FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef)
- [PromptFlowNodeSourceConfigurationUnionTypeDef](./type_defs.md#promptflownodesourceconfigurationuniontypedef)
- [ConfluenceDataSourceConfigurationUnionTypeDef](./type_defs.md#confluencedatasourceconfigurationuniontypedef)
- [SalesforceDataSourceConfigurationUnionTypeDef](./type_defs.md#salesforcedatasourceconfigurationuniontypedef)
- [SharePointDataSourceConfigurationUnionTypeDef](./type_defs.md#sharepointdatasourceconfigurationuniontypedef)
- [CreateFlowResponseTypeDef](./type_defs.md#createflowresponsetypedef)
- [CreateFlowVersionResponseTypeDef](./type_defs.md#createflowversionresponsetypedef)
- [GetFlowResponseTypeDef](./type_defs.md#getflowresponsetypedef)
- [GetFlowVersionResponseTypeDef](./type_defs.md#getflowversionresponsetypedef)
- [UpdateFlowResponseTypeDef](./type_defs.md#updateflowresponsetypedef)
- [PromptFlowNodeConfigurationTypeDef](./type_defs.md#promptflownodeconfigurationtypedef)
- [DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef)
- [PromptFlowNodeConfigurationUnionTypeDef](./type_defs.md#promptflownodeconfigurationuniontypedef)
- [CreateDataSourceRequestRequestTypeDef](./type_defs.md#createdatasourcerequestrequesttypedef)
- [UpdateDataSourceRequestRequestTypeDef](./type_defs.md#updatedatasourcerequestrequesttypedef)
- [FlowNodeConfigurationTypeDef](./type_defs.md#flownodeconfigurationtypedef)
- [FlowNodeConfigurationUnionTypeDef](./type_defs.md#flownodeconfigurationuniontypedef)
- [FlowNodeTypeDef](./type_defs.md#flownodetypedef)
- [FlowNodeUnionTypeDef](./type_defs.md#flownodeuniontypedef)
- [FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef)
- [CreateFlowRequestRequestTypeDef](./type_defs.md#createflowrequestrequesttypedef)
- [UpdateFlowRequestRequestTypeDef](./type_defs.md#updateflowrequestrequesttypedef)


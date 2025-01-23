# Type definitions

> [Index](../README.md) > [AgentsforBedrock](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AgentsforBedrock](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bedrock-agent.html#agentsforbedrock)
    type annotations stubs module [types-aiobotocore-bedrock-agent](https://pypi.org/project/types-aiobotocore-bedrock-agent/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## InferenceConfigurationUnionTypeDef

```python
# InferenceConfigurationUnionTypeDef definition

InferenceConfigurationUnionTypeDef = Union[
    InferenceConfigurationTypeDef,  # (1)
    InferenceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) 
2. See [:material-code-braces: InferenceConfigurationOutputTypeDef](./type_defs.md#inferenceconfigurationoutputtypedef) 

## PatternObjectFilterUnionTypeDef

```python
# PatternObjectFilterUnionTypeDef definition

PatternObjectFilterUnionTypeDef = Union[
    PatternObjectFilterTypeDef,  # (1)
    PatternObjectFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PatternObjectFilterTypeDef](./type_defs.md#patternobjectfiltertypedef) 
2. See [:material-code-braces: PatternObjectFilterOutputTypeDef](./type_defs.md#patternobjectfilteroutputtypedef) 

## PromptModelInferenceConfigurationUnionTypeDef

```python
# PromptModelInferenceConfigurationUnionTypeDef definition

PromptModelInferenceConfigurationUnionTypeDef = Union[
    PromptModelInferenceConfigurationTypeDef,  # (1)
    PromptModelInferenceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptModelInferenceConfigurationTypeDef](./type_defs.md#promptmodelinferenceconfigurationtypedef) 
2. See [:material-code-braces: PromptModelInferenceConfigurationOutputTypeDef](./type_defs.md#promptmodelinferenceconfigurationoutputtypedef) 

## RedshiftQueryEngineAwsDataCatalogStorageConfigurationUnionTypeDef

```python
# RedshiftQueryEngineAwsDataCatalogStorageConfigurationUnionTypeDef definition

RedshiftQueryEngineAwsDataCatalogStorageConfigurationUnionTypeDef = Union[
    RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef,  # (1)
    RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef](./type_defs.md#redshiftqueryengineawsdatacatalogstorageconfigurationtypedef) 
2. See [:material-code-braces: RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef](./type_defs.md#redshiftqueryengineawsdatacatalogstorageconfigurationoutputtypedef) 

## S3DataSourceConfigurationUnionTypeDef

```python
# S3DataSourceConfigurationUnionTypeDef definition

S3DataSourceConfigurationUnionTypeDef = Union[
    S3DataSourceConfigurationTypeDef,  # (1)
    S3DataSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: S3DataSourceConfigurationTypeDef](./type_defs.md#s3datasourceconfigurationtypedef) 
2. See [:material-code-braces: S3DataSourceConfigurationOutputTypeDef](./type_defs.md#s3datasourceconfigurationoutputtypedef) 

## SharePointSourceConfigurationUnionTypeDef

```python
# SharePointSourceConfigurationUnionTypeDef definition

SharePointSourceConfigurationUnionTypeDef = Union[
    SharePointSourceConfigurationTypeDef,  # (1)
    SharePointSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SharePointSourceConfigurationTypeDef](./type_defs.md#sharepointsourceconfigurationtypedef) 
2. See [:material-code-braces: SharePointSourceConfigurationOutputTypeDef](./type_defs.md#sharepointsourceconfigurationoutputtypedef) 

## ToolInputSchemaUnionTypeDef

```python
# ToolInputSchemaUnionTypeDef definition

ToolInputSchemaUnionTypeDef = Union[
    ToolInputSchemaTypeDef,  # (1)
    ToolInputSchemaOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolInputSchemaTypeDef](./type_defs.md#toolinputschematypedef) 
2. See [:material-code-braces: ToolInputSchemaOutputTypeDef](./type_defs.md#toolinputschemaoutputtypedef) 

## TextPromptTemplateConfigurationUnionTypeDef

```python
# TextPromptTemplateConfigurationUnionTypeDef definition

TextPromptTemplateConfigurationUnionTypeDef = Union[
    TextPromptTemplateConfigurationTypeDef,  # (1)
    TextPromptTemplateConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TextPromptTemplateConfigurationTypeDef](./type_defs.md#textprompttemplateconfigurationtypedef) 
2. See [:material-code-braces: TextPromptTemplateConfigurationOutputTypeDef](./type_defs.md#textprompttemplateconfigurationoutputtypedef) 

## ConditionFlowNodeConfigurationUnionTypeDef

```python
# ConditionFlowNodeConfigurationUnionTypeDef definition

ConditionFlowNodeConfigurationUnionTypeDef = Union[
    ConditionFlowNodeConfigurationTypeDef,  # (1)
    ConditionFlowNodeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConditionFlowNodeConfigurationTypeDef](./type_defs.md#conditionflownodeconfigurationtypedef) 
2. See [:material-code-braces: ConditionFlowNodeConfigurationOutputTypeDef](./type_defs.md#conditionflownodeconfigurationoutputtypedef) 

## MessageUnionTypeDef

```python
# MessageUnionTypeDef definition

MessageUnionTypeDef = Union[
    MessageTypeDef,  # (1)
    MessageOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 

## FunctionUnionTypeDef

```python
# FunctionUnionTypeDef definition

FunctionUnionTypeDef = Union[
    FunctionTypeDef,  # (1)
    FunctionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FunctionTypeDef](./type_defs.md#functiontypedef) 
2. See [:material-code-braces: FunctionOutputTypeDef](./type_defs.md#functionoutputtypedef) 

## HierarchicalChunkingConfigurationUnionTypeDef

```python
# HierarchicalChunkingConfigurationUnionTypeDef definition

HierarchicalChunkingConfigurationUnionTypeDef = Union[
    HierarchicalChunkingConfigurationTypeDef,  # (1)
    HierarchicalChunkingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HierarchicalChunkingConfigurationTypeDef](./type_defs.md#hierarchicalchunkingconfigurationtypedef) 
2. See [:material-code-braces: HierarchicalChunkingConfigurationOutputTypeDef](./type_defs.md#hierarchicalchunkingconfigurationoutputtypedef) 

## QueryGenerationTableUnionTypeDef

```python
# QueryGenerationTableUnionTypeDef definition

QueryGenerationTableUnionTypeDef = Union[
    QueryGenerationTableTypeDef,  # (1)
    QueryGenerationTableOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QueryGenerationTableTypeDef](./type_defs.md#querygenerationtabletypedef) 
2. See [:material-code-braces: QueryGenerationTableOutputTypeDef](./type_defs.md#querygenerationtableoutputtypedef) 

## UrlConfigurationUnionTypeDef

```python
# UrlConfigurationUnionTypeDef definition

UrlConfigurationUnionTypeDef = Union[
    UrlConfigurationTypeDef,  # (1)
    UrlConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UrlConfigurationTypeDef](./type_defs.md#urlconfigurationtypedef) 
2. See [:material-code-braces: UrlConfigurationOutputTypeDef](./type_defs.md#urlconfigurationoutputtypedef) 

## ToolChoiceUnionTypeDef

```python
# ToolChoiceUnionTypeDef definition

ToolChoiceUnionTypeDef = Union[
    ToolChoiceTypeDef,  # (1)
    ToolChoiceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolChoiceTypeDef](./type_defs.md#toolchoicetypedef) 
2. See [:material-code-braces: ToolChoiceOutputTypeDef](./type_defs.md#toolchoiceoutputtypedef) 

## WebCrawlerConfigurationUnionTypeDef

```python
# WebCrawlerConfigurationUnionTypeDef definition

WebCrawlerConfigurationUnionTypeDef = Union[
    WebCrawlerConfigurationTypeDef,  # (1)
    WebCrawlerConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WebCrawlerConfigurationTypeDef](./type_defs.md#webcrawlerconfigurationtypedef) 
2. See [:material-code-braces: WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef) 

## SupplementalDataStorageConfigurationUnionTypeDef

```python
# SupplementalDataStorageConfigurationUnionTypeDef definition

SupplementalDataStorageConfigurationUnionTypeDef = Union[
    SupplementalDataStorageConfigurationTypeDef,  # (1)
    SupplementalDataStorageConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SupplementalDataStorageConfigurationTypeDef](./type_defs.md#supplementaldatastorageconfigurationtypedef) 
2. See [:material-code-braces: SupplementalDataStorageConfigurationOutputTypeDef](./type_defs.md#supplementaldatastorageconfigurationoutputtypedef) 

## PromptConfigurationUnionTypeDef

```python
# PromptConfigurationUnionTypeDef definition

PromptConfigurationUnionTypeDef = Union[
    PromptConfigurationTypeDef,  # (1)
    PromptConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptConfigurationTypeDef](./type_defs.md#promptconfigurationtypedef) 
2. See [:material-code-braces: PromptConfigurationOutputTypeDef](./type_defs.md#promptconfigurationoutputtypedef) 

## PatternObjectFilterConfigurationUnionTypeDef

```python
# PatternObjectFilterConfigurationUnionTypeDef definition

PatternObjectFilterConfigurationUnionTypeDef = Union[
    PatternObjectFilterConfigurationTypeDef,  # (1)
    PatternObjectFilterConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PatternObjectFilterConfigurationTypeDef](./type_defs.md#patternobjectfilterconfigurationtypedef) 
2. See [:material-code-braces: PatternObjectFilterConfigurationOutputTypeDef](./type_defs.md#patternobjectfilterconfigurationoutputtypedef) 

## PromptInferenceConfigurationUnionTypeDef

```python
# PromptInferenceConfigurationUnionTypeDef definition

PromptInferenceConfigurationUnionTypeDef = Union[
    PromptInferenceConfigurationTypeDef,  # (1)
    PromptInferenceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptInferenceConfigurationTypeDef](./type_defs.md#promptinferenceconfigurationtypedef) 
2. See [:material-code-braces: PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef) 

## RedshiftQueryEngineStorageConfigurationUnionTypeDef

```python
# RedshiftQueryEngineStorageConfigurationUnionTypeDef definition

RedshiftQueryEngineStorageConfigurationUnionTypeDef = Union[
    RedshiftQueryEngineStorageConfigurationTypeDef,  # (1)
    RedshiftQueryEngineStorageConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RedshiftQueryEngineStorageConfigurationTypeDef](./type_defs.md#redshiftqueryenginestorageconfigurationtypedef) 
2. See [:material-code-braces: RedshiftQueryEngineStorageConfigurationOutputTypeDef](./type_defs.md#redshiftqueryenginestorageconfigurationoutputtypedef) 

## ToolSpecificationUnionTypeDef

```python
# ToolSpecificationUnionTypeDef definition

ToolSpecificationUnionTypeDef = Union[
    ToolSpecificationTypeDef,  # (1)
    ToolSpecificationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolSpecificationTypeDef](./type_defs.md#toolspecificationtypedef) 
2. See [:material-code-braces: ToolSpecificationOutputTypeDef](./type_defs.md#toolspecificationoutputtypedef) 

## ChunkingConfigurationUnionTypeDef

```python
# ChunkingConfigurationUnionTypeDef definition

ChunkingConfigurationUnionTypeDef = Union[
    ChunkingConfigurationTypeDef,  # (1)
    ChunkingConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ChunkingConfigurationTypeDef](./type_defs.md#chunkingconfigurationtypedef) 
2. See [:material-code-braces: ChunkingConfigurationOutputTypeDef](./type_defs.md#chunkingconfigurationoutputtypedef) 

## QueryGenerationContextUnionTypeDef

```python
# QueryGenerationContextUnionTypeDef definition

QueryGenerationContextUnionTypeDef = Union[
    QueryGenerationContextTypeDef,  # (1)
    QueryGenerationContextOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QueryGenerationContextTypeDef](./type_defs.md#querygenerationcontexttypedef) 
2. See [:material-code-braces: QueryGenerationContextOutputTypeDef](./type_defs.md#querygenerationcontextoutputtypedef) 

## WebSourceConfigurationUnionTypeDef

```python
# WebSourceConfigurationUnionTypeDef definition

WebSourceConfigurationUnionTypeDef = Union[
    WebSourceConfigurationTypeDef,  # (1)
    WebSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WebSourceConfigurationTypeDef](./type_defs.md#websourceconfigurationtypedef) 
2. See [:material-code-braces: WebSourceConfigurationOutputTypeDef](./type_defs.md#websourceconfigurationoutputtypedef) 

## CustomTransformationConfigurationUnionTypeDef

```python
# CustomTransformationConfigurationUnionTypeDef definition

CustomTransformationConfigurationUnionTypeDef = Union[
    CustomTransformationConfigurationTypeDef,  # (1)
    CustomTransformationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CustomTransformationConfigurationTypeDef](./type_defs.md#customtransformationconfigurationtypedef) 
2. See [:material-code-braces: CustomTransformationConfigurationOutputTypeDef](./type_defs.md#customtransformationconfigurationoutputtypedef) 

## VectorKnowledgeBaseConfigurationUnionTypeDef

```python
# VectorKnowledgeBaseConfigurationUnionTypeDef definition

VectorKnowledgeBaseConfigurationUnionTypeDef = Union[
    VectorKnowledgeBaseConfigurationTypeDef,  # (1)
    VectorKnowledgeBaseConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: VectorKnowledgeBaseConfigurationTypeDef](./type_defs.md#vectorknowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: VectorKnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#vectorknowledgebaseconfigurationoutputtypedef) 

## CrawlFilterConfigurationUnionTypeDef

```python
# CrawlFilterConfigurationUnionTypeDef definition

CrawlFilterConfigurationUnionTypeDef = Union[
    CrawlFilterConfigurationTypeDef,  # (1)
    CrawlFilterConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CrawlFilterConfigurationTypeDef](./type_defs.md#crawlfilterconfigurationtypedef) 
2. See [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef) 

## ToolUnionTypeDef

```python
# ToolUnionTypeDef definition

ToolUnionTypeDef = Union[
    ToolTypeDef,  # (1)
    ToolOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) 
2. See [:material-code-braces: ToolOutputTypeDef](./type_defs.md#tooloutputtypedef) 

## QueryGenerationConfigurationUnionTypeDef

```python
# QueryGenerationConfigurationUnionTypeDef definition

QueryGenerationConfigurationUnionTypeDef = Union[
    QueryGenerationConfigurationTypeDef,  # (1)
    QueryGenerationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QueryGenerationConfigurationTypeDef](./type_defs.md#querygenerationconfigurationtypedef) 
2. See [:material-code-braces: QueryGenerationConfigurationOutputTypeDef](./type_defs.md#querygenerationconfigurationoutputtypedef) 

## WebDataSourceConfigurationUnionTypeDef

```python
# WebDataSourceConfigurationUnionTypeDef definition

WebDataSourceConfigurationUnionTypeDef = Union[
    WebDataSourceConfigurationTypeDef,  # (1)
    WebDataSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WebDataSourceConfigurationTypeDef](./type_defs.md#webdatasourceconfigurationtypedef) 
2. See [:material-code-braces: WebDataSourceConfigurationOutputTypeDef](./type_defs.md#webdatasourceconfigurationoutputtypedef) 

## ConfluenceCrawlerConfigurationUnionTypeDef

```python
# ConfluenceCrawlerConfigurationUnionTypeDef definition

ConfluenceCrawlerConfigurationUnionTypeDef = Union[
    ConfluenceCrawlerConfigurationTypeDef,  # (1)
    ConfluenceCrawlerConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfluenceCrawlerConfigurationTypeDef](./type_defs.md#confluencecrawlerconfigurationtypedef) 
2. See [:material-code-braces: ConfluenceCrawlerConfigurationOutputTypeDef](./type_defs.md#confluencecrawlerconfigurationoutputtypedef) 

## SalesforceCrawlerConfigurationUnionTypeDef

```python
# SalesforceCrawlerConfigurationUnionTypeDef definition

SalesforceCrawlerConfigurationUnionTypeDef = Union[
    SalesforceCrawlerConfigurationTypeDef,  # (1)
    SalesforceCrawlerConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceCrawlerConfigurationTypeDef](./type_defs.md#salesforcecrawlerconfigurationtypedef) 
2. See [:material-code-braces: SalesforceCrawlerConfigurationOutputTypeDef](./type_defs.md#salesforcecrawlerconfigurationoutputtypedef) 

## SharePointCrawlerConfigurationUnionTypeDef

```python
# SharePointCrawlerConfigurationUnionTypeDef definition

SharePointCrawlerConfigurationUnionTypeDef = Union[
    SharePointCrawlerConfigurationTypeDef,  # (1)
    SharePointCrawlerConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SharePointCrawlerConfigurationTypeDef](./type_defs.md#sharepointcrawlerconfigurationtypedef) 
2. See [:material-code-braces: SharePointCrawlerConfigurationOutputTypeDef](./type_defs.md#sharepointcrawlerconfigurationoutputtypedef) 

## ToolConfigurationUnionTypeDef

```python
# ToolConfigurationUnionTypeDef definition

ToolConfigurationUnionTypeDef = Union[
    ToolConfigurationTypeDef,  # (1)
    ToolConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef) 
2. See [:material-code-braces: ToolConfigurationOutputTypeDef](./type_defs.md#toolconfigurationoutputtypedef) 

## RedshiftConfigurationUnionTypeDef

```python
# RedshiftConfigurationUnionTypeDef definition

RedshiftConfigurationUnionTypeDef = Union[
    RedshiftConfigurationTypeDef,  # (1)
    RedshiftConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RedshiftConfigurationTypeDef](./type_defs.md#redshiftconfigurationtypedef) 
2. See [:material-code-braces: RedshiftConfigurationOutputTypeDef](./type_defs.md#redshiftconfigurationoutputtypedef) 

## ConfluenceDataSourceConfigurationUnionTypeDef

```python
# ConfluenceDataSourceConfigurationUnionTypeDef definition

ConfluenceDataSourceConfigurationUnionTypeDef = Union[
    ConfluenceDataSourceConfigurationTypeDef,  # (1)
    ConfluenceDataSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfluenceDataSourceConfigurationTypeDef](./type_defs.md#confluencedatasourceconfigurationtypedef) 
2. See [:material-code-braces: ConfluenceDataSourceConfigurationOutputTypeDef](./type_defs.md#confluencedatasourceconfigurationoutputtypedef) 

## SalesforceDataSourceConfigurationUnionTypeDef

```python
# SalesforceDataSourceConfigurationUnionTypeDef definition

SalesforceDataSourceConfigurationUnionTypeDef = Union[
    SalesforceDataSourceConfigurationTypeDef,  # (1)
    SalesforceDataSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceDataSourceConfigurationTypeDef](./type_defs.md#salesforcedatasourceconfigurationtypedef) 
2. See [:material-code-braces: SalesforceDataSourceConfigurationOutputTypeDef](./type_defs.md#salesforcedatasourceconfigurationoutputtypedef) 

## SharePointDataSourceConfigurationUnionTypeDef

```python
# SharePointDataSourceConfigurationUnionTypeDef definition

SharePointDataSourceConfigurationUnionTypeDef = Union[
    SharePointDataSourceConfigurationTypeDef,  # (1)
    SharePointDataSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SharePointDataSourceConfigurationTypeDef](./type_defs.md#sharepointdatasourceconfigurationtypedef) 
2. See [:material-code-braces: SharePointDataSourceConfigurationOutputTypeDef](./type_defs.md#sharepointdatasourceconfigurationoutputtypedef) 

## ChatPromptTemplateConfigurationUnionTypeDef

```python
# ChatPromptTemplateConfigurationUnionTypeDef definition

ChatPromptTemplateConfigurationUnionTypeDef = Union[
    ChatPromptTemplateConfigurationTypeDef,  # (1)
    ChatPromptTemplateConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ChatPromptTemplateConfigurationTypeDef](./type_defs.md#chatprompttemplateconfigurationtypedef) 
2. See [:material-code-braces: ChatPromptTemplateConfigurationOutputTypeDef](./type_defs.md#chatprompttemplateconfigurationoutputtypedef) 

## SqlKnowledgeBaseConfigurationUnionTypeDef

```python
# SqlKnowledgeBaseConfigurationUnionTypeDef definition

SqlKnowledgeBaseConfigurationUnionTypeDef = Union[
    SqlKnowledgeBaseConfigurationTypeDef,  # (1)
    SqlKnowledgeBaseConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SqlKnowledgeBaseConfigurationTypeDef](./type_defs.md#sqlknowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: SqlKnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#sqlknowledgebaseconfigurationoutputtypedef) 

## PromptTemplateConfigurationUnionTypeDef

```python
# PromptTemplateConfigurationUnionTypeDef definition

PromptTemplateConfigurationUnionTypeDef = Union[
    PromptTemplateConfigurationTypeDef,  # (1)
    PromptTemplateConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptTemplateConfigurationTypeDef](./type_defs.md#prompttemplateconfigurationtypedef) 
2. See [:material-code-braces: PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef) 

## PromptFlowNodeInlineConfigurationUnionTypeDef

```python
# PromptFlowNodeInlineConfigurationUnionTypeDef definition

PromptFlowNodeInlineConfigurationUnionTypeDef = Union[
    PromptFlowNodeInlineConfigurationTypeDef,  # (1)
    PromptFlowNodeInlineConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptFlowNodeInlineConfigurationTypeDef](./type_defs.md#promptflownodeinlineconfigurationtypedef) 
2. See [:material-code-braces: PromptFlowNodeInlineConfigurationOutputTypeDef](./type_defs.md#promptflownodeinlineconfigurationoutputtypedef) 

## PromptVariantUnionTypeDef

```python
# PromptVariantUnionTypeDef definition

PromptVariantUnionTypeDef = Union[
    PromptVariantTypeDef,  # (1)
    PromptVariantOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptVariantTypeDef](./type_defs.md#promptvarianttypedef) 
2. See [:material-code-braces: PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef) 

## PromptFlowNodeSourceConfigurationUnionTypeDef

```python
# PromptFlowNodeSourceConfigurationUnionTypeDef definition

PromptFlowNodeSourceConfigurationUnionTypeDef = Union[
    PromptFlowNodeSourceConfigurationTypeDef,  # (1)
    PromptFlowNodeSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptFlowNodeSourceConfigurationTypeDef](./type_defs.md#promptflownodesourceconfigurationtypedef) 
2. See [:material-code-braces: PromptFlowNodeSourceConfigurationOutputTypeDef](./type_defs.md#promptflownodesourceconfigurationoutputtypedef) 

## PromptFlowNodeConfigurationUnionTypeDef

```python
# PromptFlowNodeConfigurationUnionTypeDef definition

PromptFlowNodeConfigurationUnionTypeDef = Union[
    PromptFlowNodeConfigurationTypeDef,  # (1)
    PromptFlowNodeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PromptFlowNodeConfigurationTypeDef](./type_defs.md#promptflownodeconfigurationtypedef) 
2. See [:material-code-braces: PromptFlowNodeConfigurationOutputTypeDef](./type_defs.md#promptflownodeconfigurationoutputtypedef) 

## FlowNodeConfigurationUnionTypeDef

```python
# FlowNodeConfigurationUnionTypeDef definition

FlowNodeConfigurationUnionTypeDef = Union[
    FlowNodeConfigurationTypeDef,  # (1)
    FlowNodeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FlowNodeConfigurationTypeDef](./type_defs.md#flownodeconfigurationtypedef) 
2. See [:material-code-braces: FlowNodeConfigurationOutputTypeDef](./type_defs.md#flownodeconfigurationoutputtypedef) 

## FlowNodeUnionTypeDef

```python
# FlowNodeUnionTypeDef definition

FlowNodeUnionTypeDef = Union[
    FlowNodeTypeDef,  # (1)
    FlowNodeExtraOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FlowNodeTypeDef](./type_defs.md#flownodetypedef) 
2. See [:material-code-braces: FlowNodeExtraOutputTypeDef](./type_defs.md#flownodeextraoutputtypedef) 



## S3IdentifierTypeDef

```python
# S3IdentifierTypeDef definition

class S3IdentifierTypeDef(TypedDict):
    s3BucketName: NotRequired[str],
    s3ObjectKey: NotRequired[str],
```

## ActionGroupExecutorTypeDef

```python
# ActionGroupExecutorTypeDef definition

class ActionGroupExecutorTypeDef(TypedDict):
    customControl: NotRequired[CustomControlMethodType],  # (1)
    lambda: NotRequired[str],
```

1. See [:material-code-brackets: CustomControlMethodType](./literals.md#customcontrolmethodtype) 
## ActionGroupSummaryTypeDef

```python
# ActionGroupSummaryTypeDef definition

class ActionGroupSummaryTypeDef(TypedDict):
    actionGroupId: str,
    actionGroupName: str,
    actionGroupState: ActionGroupStateType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
## AgentAliasRoutingConfigurationListItemTypeDef

```python
# AgentAliasRoutingConfigurationListItemTypeDef definition

class AgentAliasRoutingConfigurationListItemTypeDef(TypedDict):
    agentVersion: NotRequired[str],
    provisionedThroughput: NotRequired[str],
```

## AgentDescriptorTypeDef

```python
# AgentDescriptorTypeDef definition

class AgentDescriptorTypeDef(TypedDict):
    aliasArn: NotRequired[str],
```

## AgentFlowNodeConfigurationTypeDef

```python
# AgentFlowNodeConfigurationTypeDef definition

class AgentFlowNodeConfigurationTypeDef(TypedDict):
    agentAliasArn: str,
```

## AgentKnowledgeBaseSummaryTypeDef

```python
# AgentKnowledgeBaseSummaryTypeDef definition

class AgentKnowledgeBaseSummaryTypeDef(TypedDict):
    knowledgeBaseId: str,
    knowledgeBaseState: KnowledgeBaseStateType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
## AgentKnowledgeBaseTypeDef

```python
# AgentKnowledgeBaseTypeDef definition

class AgentKnowledgeBaseTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    createdAt: datetime,
    description: str,
    knowledgeBaseId: str,
    knowledgeBaseState: KnowledgeBaseStateType,  # (1)
    updatedAt: datetime,
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
## GuardrailConfigurationTypeDef

```python
# GuardrailConfigurationTypeDef definition

class GuardrailConfigurationTypeDef(TypedDict):
    guardrailIdentifier: NotRequired[str],
    guardrailVersion: NotRequired[str],
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

## AssociateAgentKnowledgeBaseRequestRequestTypeDef

```python
# AssociateAgentKnowledgeBaseRequestRequestTypeDef definition

class AssociateAgentKnowledgeBaseRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    description: str,
    knowledgeBaseId: str,
    knowledgeBaseState: NotRequired[KnowledgeBaseStateType],  # (1)
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
## BedrockDataAutomationConfigurationTypeDef

```python
# BedrockDataAutomationConfigurationTypeDef definition

class BedrockDataAutomationConfigurationTypeDef(TypedDict):
    parsingModality: NotRequired[ParsingModalityType],  # (1)
```

1. See [:material-code-brackets: ParsingModalityType](./literals.md#parsingmodalitytype) 
## BedrockEmbeddingModelConfigurationTypeDef

```python
# BedrockEmbeddingModelConfigurationTypeDef definition

class BedrockEmbeddingModelConfigurationTypeDef(TypedDict):
    dimensions: NotRequired[int],
    embeddingDataType: NotRequired[EmbeddingDataTypeType],  # (1)
```

1. See [:material-code-brackets: EmbeddingDataTypeType](./literals.md#embeddingdatatypetype) 
## ParsingPromptTypeDef

```python
# ParsingPromptTypeDef definition

class ParsingPromptTypeDef(TypedDict):
    parsingPromptText: str,
```

## PromptInputVariableTypeDef

```python
# PromptInputVariableTypeDef definition

class PromptInputVariableTypeDef(TypedDict):
    name: NotRequired[str],
```

## SystemContentBlockTypeDef

```python
# SystemContentBlockTypeDef definition

class SystemContentBlockTypeDef(TypedDict):
    text: NotRequired[str],
```

## FixedSizeChunkingConfigurationTypeDef

```python
# FixedSizeChunkingConfigurationTypeDef definition

class FixedSizeChunkingConfigurationTypeDef(TypedDict):
    maxTokens: int,
    overlapPercentage: int,
```

## SemanticChunkingConfigurationTypeDef

```python
# SemanticChunkingConfigurationTypeDef definition

class SemanticChunkingConfigurationTypeDef(TypedDict):
    breakpointPercentileThreshold: int,
    bufferSize: int,
    maxTokens: int,
```

## FlowConditionTypeDef

```python
# FlowConditionTypeDef definition

class FlowConditionTypeDef(TypedDict):
    name: str,
    expression: NotRequired[str],
```

## ConfluenceSourceConfigurationTypeDef

```python
# ConfluenceSourceConfigurationTypeDef definition

class ConfluenceSourceConfigurationTypeDef(TypedDict):
    authType: ConfluenceAuthTypeType,  # (1)
    credentialsSecretArn: str,
    hostType: ConfluenceHostTypeType,  # (2)
    hostUrl: str,
```

1. See [:material-code-brackets: ConfluenceAuthTypeType](./literals.md#confluenceauthtypetype) 
2. See [:material-code-brackets: ConfluenceHostTypeType](./literals.md#confluencehosttypetype) 
## ContentBlockTypeDef

```python
# ContentBlockTypeDef definition

class ContentBlockTypeDef(TypedDict):
    text: NotRequired[str],
```

## ServerSideEncryptionConfigurationTypeDef

```python
# ServerSideEncryptionConfigurationTypeDef definition

class ServerSideEncryptionConfigurationTypeDef(TypedDict):
    kmsKeyArn: NotRequired[str],
```

## FlowAliasRoutingConfigurationListItemTypeDef

```python
# FlowAliasRoutingConfigurationListItemTypeDef definition

class FlowAliasRoutingConfigurationListItemTypeDef(TypedDict):
    flowVersion: NotRequired[str],
```

## CreateFlowVersionRequestRequestTypeDef

```python
# CreateFlowVersionRequestRequestTypeDef definition

class CreateFlowVersionRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## CreatePromptVersionRequestRequestTypeDef

```python
# CreatePromptVersionRequestRequestTypeDef definition

class CreatePromptVersionRequestRequestTypeDef(TypedDict):
    promptIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

## CuratedQueryTypeDef

```python
# CuratedQueryTypeDef definition

class CuratedQueryTypeDef(TypedDict):
    naturalLanguage: str,
    sql: str,
```

## CustomDocumentIdentifierTypeDef

```python
# CustomDocumentIdentifierTypeDef definition

class CustomDocumentIdentifierTypeDef(TypedDict):
    id: str,
```

## CustomS3LocationTypeDef

```python
# CustomS3LocationTypeDef definition

class CustomS3LocationTypeDef(TypedDict):
    uri: str,
    bucketOwnerAccountId: NotRequired[str],
```

## OrchestrationExecutorTypeDef

```python
# OrchestrationExecutorTypeDef definition

class OrchestrationExecutorTypeDef(TypedDict):
    lambda: NotRequired[str],
```

## CyclicConnectionFlowValidationDetailsTypeDef

```python
# CyclicConnectionFlowValidationDetailsTypeDef definition

class CyclicConnectionFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## S3DataSourceConfigurationOutputTypeDef

```python
# S3DataSourceConfigurationOutputTypeDef definition

class S3DataSourceConfigurationOutputTypeDef(TypedDict):
    bucketArn: str,
    bucketOwnerAccountId: NotRequired[str],
    inclusionPrefixes: NotRequired[List[str]],
```

## DataSourceSummaryTypeDef

```python
# DataSourceSummaryTypeDef definition

class DataSourceSummaryTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    name: str,
    status: DataSourceStatusType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## DeleteAgentActionGroupRequestRequestTypeDef

```python
# DeleteAgentActionGroupRequestRequestTypeDef definition

class DeleteAgentActionGroupRequestRequestTypeDef(TypedDict):
    actionGroupId: str,
    agentId: str,
    agentVersion: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteAgentAliasRequestRequestTypeDef

```python
# DeleteAgentAliasRequestRequestTypeDef definition

class DeleteAgentAliasRequestRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
```

## DeleteAgentRequestRequestTypeDef

```python
# DeleteAgentRequestRequestTypeDef definition

class DeleteAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteAgentVersionRequestRequestTypeDef

```python
# DeleteAgentVersionRequestRequestTypeDef definition

class DeleteAgentVersionRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteDataSourceRequestRequestTypeDef

```python
# DeleteDataSourceRequestRequestTypeDef definition

class DeleteDataSourceRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
```

## DeleteFlowAliasRequestRequestTypeDef

```python
# DeleteFlowAliasRequestRequestTypeDef definition

class DeleteFlowAliasRequestRequestTypeDef(TypedDict):
    aliasIdentifier: str,
    flowIdentifier: str,
```

## DeleteFlowRequestRequestTypeDef

```python
# DeleteFlowRequestRequestTypeDef definition

class DeleteFlowRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteFlowVersionRequestRequestTypeDef

```python
# DeleteFlowVersionRequestRequestTypeDef definition

class DeleteFlowVersionRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
    flowVersion: str,
    skipResourceInUseCheck: NotRequired[bool],
```

## DeleteKnowledgeBaseRequestRequestTypeDef

```python
# DeleteKnowledgeBaseRequestRequestTypeDef definition

class DeleteKnowledgeBaseRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```

## DeletePromptRequestRequestTypeDef

```python
# DeletePromptRequestRequestTypeDef definition

class DeletePromptRequestRequestTypeDef(TypedDict):
    promptIdentifier: str,
    promptVersion: NotRequired[str],
```

## DisassociateAgentCollaboratorRequestRequestTypeDef

```python
# DisassociateAgentCollaboratorRequestRequestTypeDef definition

class DisassociateAgentCollaboratorRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    collaboratorId: str,
```

## DisassociateAgentKnowledgeBaseRequestRequestTypeDef

```python
# DisassociateAgentKnowledgeBaseRequestRequestTypeDef definition

class DisassociateAgentKnowledgeBaseRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
```

## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    uri: str,
```

## DuplicateConditionExpressionFlowValidationDetailsTypeDef

```python
# DuplicateConditionExpressionFlowValidationDetailsTypeDef definition

class DuplicateConditionExpressionFlowValidationDetailsTypeDef(TypedDict):
    expression: str,
    node: str,
```

## DuplicateConnectionsFlowValidationDetailsTypeDef

```python
# DuplicateConnectionsFlowValidationDetailsTypeDef definition

class DuplicateConnectionsFlowValidationDetailsTypeDef(TypedDict):
    source: str,
    target: str,
```

## FlowConditionalConnectionConfigurationTypeDef

```python
# FlowConditionalConnectionConfigurationTypeDef definition

class FlowConditionalConnectionConfigurationTypeDef(TypedDict):
    condition: str,
```

## FlowDataConnectionConfigurationTypeDef

```python
# FlowDataConnectionConfigurationTypeDef definition

class FlowDataConnectionConfigurationTypeDef(TypedDict):
    sourceOutput: str,
    targetInput: str,
```

## LambdaFunctionFlowNodeConfigurationTypeDef

```python
# LambdaFunctionFlowNodeConfigurationTypeDef definition

class LambdaFunctionFlowNodeConfigurationTypeDef(TypedDict):
    lambdaArn: str,
```

## LexFlowNodeConfigurationTypeDef

```python
# LexFlowNodeConfigurationTypeDef definition

class LexFlowNodeConfigurationTypeDef(TypedDict):
    botAliasArn: str,
    localeId: str,
```

## FlowNodeInputTypeDef

```python
# FlowNodeInputTypeDef definition

class FlowNodeInputTypeDef(TypedDict):
    expression: str,
    name: str,
    type: FlowNodeIODataTypeType,  # (1)
```

1. See [:material-code-brackets: FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype) 
## FlowNodeOutputTypeDef

```python
# FlowNodeOutputTypeDef definition

class FlowNodeOutputTypeDef(TypedDict):
    name: str,
    type: FlowNodeIODataTypeType,  # (1)
```

1. See [:material-code-brackets: FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype) 
## FlowSummaryTypeDef

```python
# FlowSummaryTypeDef definition

class FlowSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    id: str,
    name: str,
    status: FlowStatusType,  # (1)
    updatedAt: datetime,
    version: str,
    description: NotRequired[str],
```

1. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype) 
## IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef

```python
# IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef definition

class IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## MalformedConditionExpressionFlowValidationDetailsTypeDef

```python
# MalformedConditionExpressionFlowValidationDetailsTypeDef definition

class MalformedConditionExpressionFlowValidationDetailsTypeDef(TypedDict):
    cause: str,
    condition: str,
    node: str,
```

## MalformedNodeInputExpressionFlowValidationDetailsTypeDef

```python
# MalformedNodeInputExpressionFlowValidationDetailsTypeDef definition

class MalformedNodeInputExpressionFlowValidationDetailsTypeDef(TypedDict):
    cause: str,
    input: str,
    node: str,
```

## MismatchedNodeInputTypeFlowValidationDetailsTypeDef

```python
# MismatchedNodeInputTypeFlowValidationDetailsTypeDef definition

class MismatchedNodeInputTypeFlowValidationDetailsTypeDef(TypedDict):
    expectedType: FlowNodeIODataTypeType,  # (1)
    input: str,
    node: str,
```

1. See [:material-code-brackets: FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype) 
## MismatchedNodeOutputTypeFlowValidationDetailsTypeDef

```python
# MismatchedNodeOutputTypeFlowValidationDetailsTypeDef definition

class MismatchedNodeOutputTypeFlowValidationDetailsTypeDef(TypedDict):
    expectedType: FlowNodeIODataTypeType,  # (1)
    node: str,
    output: str,
```

1. See [:material-code-brackets: FlowNodeIODataTypeType](./literals.md#flownodeiodatatypetype) 
## MissingConnectionConfigurationFlowValidationDetailsTypeDef

```python
# MissingConnectionConfigurationFlowValidationDetailsTypeDef definition

class MissingConnectionConfigurationFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## MissingDefaultConditionFlowValidationDetailsTypeDef

```python
# MissingDefaultConditionFlowValidationDetailsTypeDef definition

class MissingDefaultConditionFlowValidationDetailsTypeDef(TypedDict):
    node: str,
```

## MissingNodeConfigurationFlowValidationDetailsTypeDef

```python
# MissingNodeConfigurationFlowValidationDetailsTypeDef definition

class MissingNodeConfigurationFlowValidationDetailsTypeDef(TypedDict):
    node: str,
```

## MissingNodeInputFlowValidationDetailsTypeDef

```python
# MissingNodeInputFlowValidationDetailsTypeDef definition

class MissingNodeInputFlowValidationDetailsTypeDef(TypedDict):
    input: str,
    node: str,
```

## MissingNodeOutputFlowValidationDetailsTypeDef

```python
# MissingNodeOutputFlowValidationDetailsTypeDef definition

class MissingNodeOutputFlowValidationDetailsTypeDef(TypedDict):
    node: str,
    output: str,
```

## MultipleNodeInputConnectionsFlowValidationDetailsTypeDef

```python
# MultipleNodeInputConnectionsFlowValidationDetailsTypeDef definition

class MultipleNodeInputConnectionsFlowValidationDetailsTypeDef(TypedDict):
    input: str,
    node: str,
```

## UnfulfilledNodeInputFlowValidationDetailsTypeDef

```python
# UnfulfilledNodeInputFlowValidationDetailsTypeDef definition

class UnfulfilledNodeInputFlowValidationDetailsTypeDef(TypedDict):
    input: str,
    node: str,
```

## UnknownConnectionConditionFlowValidationDetailsTypeDef

```python
# UnknownConnectionConditionFlowValidationDetailsTypeDef definition

class UnknownConnectionConditionFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## UnknownConnectionSourceFlowValidationDetailsTypeDef

```python
# UnknownConnectionSourceFlowValidationDetailsTypeDef definition

class UnknownConnectionSourceFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## UnknownConnectionSourceOutputFlowValidationDetailsTypeDef

```python
# UnknownConnectionSourceOutputFlowValidationDetailsTypeDef definition

class UnknownConnectionSourceOutputFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## UnknownConnectionTargetFlowValidationDetailsTypeDef

```python
# UnknownConnectionTargetFlowValidationDetailsTypeDef definition

class UnknownConnectionTargetFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## UnknownConnectionTargetInputFlowValidationDetailsTypeDef

```python
# UnknownConnectionTargetInputFlowValidationDetailsTypeDef definition

class UnknownConnectionTargetInputFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## UnreachableNodeFlowValidationDetailsTypeDef

```python
# UnreachableNodeFlowValidationDetailsTypeDef definition

class UnreachableNodeFlowValidationDetailsTypeDef(TypedDict):
    node: str,
```

## UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef

```python
# UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef definition

class UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef(TypedDict):
    connection: str,
```

## FlowVersionSummaryTypeDef

```python
# FlowVersionSummaryTypeDef definition

class FlowVersionSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    id: str,
    status: FlowStatusType,  # (1)
    version: str,
```

1. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype) 
## ParameterDetailTypeDef

```python
# ParameterDetailTypeDef definition

class ParameterDetailTypeDef(TypedDict):
    type: TypeType,  # (1)
    description: NotRequired[str],
    required: NotRequired[bool],
```

1. See [:material-code-brackets: TypeType](./literals.md#typetype) 
## GetAgentActionGroupRequestRequestTypeDef

```python
# GetAgentActionGroupRequestRequestTypeDef definition

class GetAgentActionGroupRequestRequestTypeDef(TypedDict):
    actionGroupId: str,
    agentId: str,
    agentVersion: str,
```

## GetAgentAliasRequestRequestTypeDef

```python
# GetAgentAliasRequestRequestTypeDef definition

class GetAgentAliasRequestRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentId: str,
```

## GetAgentCollaboratorRequestRequestTypeDef

```python
# GetAgentCollaboratorRequestRequestTypeDef definition

class GetAgentCollaboratorRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    collaboratorId: str,
```

## GetAgentKnowledgeBaseRequestRequestTypeDef

```python
# GetAgentKnowledgeBaseRequestRequestTypeDef definition

class GetAgentKnowledgeBaseRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
```

## GetAgentRequestRequestTypeDef

```python
# GetAgentRequestRequestTypeDef definition

class GetAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
```

## GetAgentVersionRequestRequestTypeDef

```python
# GetAgentVersionRequestRequestTypeDef definition

class GetAgentVersionRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
```

## GetDataSourceRequestRequestTypeDef

```python
# GetDataSourceRequestRequestTypeDef definition

class GetDataSourceRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
```

## GetFlowAliasRequestRequestTypeDef

```python
# GetFlowAliasRequestRequestTypeDef definition

class GetFlowAliasRequestRequestTypeDef(TypedDict):
    aliasIdentifier: str,
    flowIdentifier: str,
```

## GetFlowRequestRequestTypeDef

```python
# GetFlowRequestRequestTypeDef definition

class GetFlowRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
```

## GetFlowVersionRequestRequestTypeDef

```python
# GetFlowVersionRequestRequestTypeDef definition

class GetFlowVersionRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
    flowVersion: str,
```

## GetIngestionJobRequestRequestTypeDef

```python
# GetIngestionJobRequestRequestTypeDef definition

class GetIngestionJobRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
```

## GetKnowledgeBaseRequestRequestTypeDef

```python
# GetKnowledgeBaseRequestRequestTypeDef definition

class GetKnowledgeBaseRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
```

## GetPromptRequestRequestTypeDef

```python
# GetPromptRequestRequestTypeDef definition

class GetPromptRequestRequestTypeDef(TypedDict):
    promptIdentifier: str,
    promptVersion: NotRequired[str],
```

## HierarchicalChunkingLevelConfigurationTypeDef

```python
# HierarchicalChunkingLevelConfigurationTypeDef definition

class HierarchicalChunkingLevelConfigurationTypeDef(TypedDict):
    maxTokens: int,
```

## InferenceConfigurationOutputTypeDef

```python
# InferenceConfigurationOutputTypeDef definition

class InferenceConfigurationOutputTypeDef(TypedDict):
    maximumLength: NotRequired[int],
    stopSequences: NotRequired[List[str]],
    temperature: NotRequired[float],
    topK: NotRequired[int],
    topP: NotRequired[float],
```

## InferenceConfigurationTypeDef

```python
# InferenceConfigurationTypeDef definition

class InferenceConfigurationTypeDef(TypedDict):
    maximumLength: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
    temperature: NotRequired[float],
    topK: NotRequired[int],
    topP: NotRequired[float],
```

## IngestionJobFilterTypeDef

```python
# IngestionJobFilterTypeDef definition

class IngestionJobFilterTypeDef(TypedDict):
    attribute: IngestionJobFilterAttributeType,  # (1)
    operator: IngestionJobFilterOperatorType,  # (2)
    values: Sequence[str],
```

1. See [:material-code-brackets: IngestionJobFilterAttributeType](./literals.md#ingestionjobfilterattributetype) 
2. See [:material-code-brackets: IngestionJobFilterOperatorType](./literals.md#ingestionjobfilteroperatortype) 
## IngestionJobSortByTypeDef

```python
# IngestionJobSortByTypeDef definition

class IngestionJobSortByTypeDef(TypedDict):
    attribute: IngestionJobSortByAttributeType,  # (1)
    order: SortOrderType,  # (2)
```

1. See [:material-code-brackets: IngestionJobSortByAttributeType](./literals.md#ingestionjobsortbyattributetype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## IngestionJobStatisticsTypeDef

```python
# IngestionJobStatisticsTypeDef definition

class IngestionJobStatisticsTypeDef(TypedDict):
    numberOfDocumentsDeleted: NotRequired[int],
    numberOfDocumentsFailed: NotRequired[int],
    numberOfDocumentsScanned: NotRequired[int],
    numberOfMetadataDocumentsModified: NotRequired[int],
    numberOfMetadataDocumentsScanned: NotRequired[int],
    numberOfModifiedDocumentsIndexed: NotRequired[int],
    numberOfNewDocumentsIndexed: NotRequired[int],
```

## TextContentDocTypeDef

```python
# TextContentDocTypeDef definition

class TextContentDocTypeDef(TypedDict):
    data: str,
```

## KendraKnowledgeBaseConfigurationTypeDef

```python
# KendraKnowledgeBaseConfigurationTypeDef definition

class KendraKnowledgeBaseConfigurationTypeDef(TypedDict):
    kendraIndexArn: str,
```

## KnowledgeBaseSummaryTypeDef

```python
# KnowledgeBaseSummaryTypeDef definition

class KnowledgeBaseSummaryTypeDef(TypedDict):
    knowledgeBaseId: str,
    name: str,
    status: KnowledgeBaseStatusType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAgentActionGroupsRequestRequestTypeDef

```python
# ListAgentActionGroupsRequestRequestTypeDef definition

class ListAgentActionGroupsRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentAliasesRequestRequestTypeDef

```python
# ListAgentAliasesRequestRequestTypeDef definition

class ListAgentAliasesRequestRequestTypeDef(TypedDict):
    agentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentCollaboratorsRequestRequestTypeDef

```python
# ListAgentCollaboratorsRequestRequestTypeDef definition

class ListAgentCollaboratorsRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentKnowledgeBasesRequestRequestTypeDef

```python
# ListAgentKnowledgeBasesRequestRequestTypeDef definition

class ListAgentKnowledgeBasesRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentVersionsRequestRequestTypeDef

```python
# ListAgentVersionsRequestRequestTypeDef definition

class ListAgentVersionsRequestRequestTypeDef(TypedDict):
    agentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListAgentsRequestRequestTypeDef

```python
# ListAgentsRequestRequestTypeDef definition

class ListAgentsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataSourcesRequestRequestTypeDef

```python
# ListDataSourcesRequestRequestTypeDef definition

class ListDataSourcesRequestRequestTypeDef(TypedDict):
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListFlowAliasesRequestRequestTypeDef

```python
# ListFlowAliasesRequestRequestTypeDef definition

class ListFlowAliasesRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListFlowVersionsRequestRequestTypeDef

```python
# ListFlowVersionsRequestRequestTypeDef definition

class ListFlowVersionsRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListFlowsRequestRequestTypeDef

```python
# ListFlowsRequestRequestTypeDef definition

class ListFlowsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListKnowledgeBaseDocumentsRequestRequestTypeDef

```python
# ListKnowledgeBaseDocumentsRequestRequestTypeDef definition

class ListKnowledgeBaseDocumentsRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListKnowledgeBasesRequestRequestTypeDef

```python
# ListKnowledgeBasesRequestRequestTypeDef definition

class ListKnowledgeBasesRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListPromptsRequestRequestTypeDef

```python
# ListPromptsRequestRequestTypeDef definition

class ListPromptsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    promptIdentifier: NotRequired[str],
```

## PromptSummaryTypeDef

```python
# PromptSummaryTypeDef definition

class PromptSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    id: str,
    name: str,
    updatedAt: datetime,
    version: str,
    description: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## SessionSummaryConfigurationTypeDef

```python
# SessionSummaryConfigurationTypeDef definition

class SessionSummaryConfigurationTypeDef(TypedDict):
    maxRecentSessions: NotRequired[int],
```

## MetadataAttributeValueTypeDef

```python
# MetadataAttributeValueTypeDef definition

class MetadataAttributeValueTypeDef(TypedDict):
    type: MetadataValueTypeType,  # (1)
    booleanValue: NotRequired[bool],
    numberValue: NotRequired[float],
    stringListValue: NotRequired[Sequence[str]],
    stringValue: NotRequired[str],
```

1. See [:material-code-brackets: MetadataValueTypeType](./literals.md#metadatavaluetypetype) 
## MongoDbAtlasFieldMappingTypeDef

```python
# MongoDbAtlasFieldMappingTypeDef definition

class MongoDbAtlasFieldMappingTypeDef(TypedDict):
    metadataField: str,
    textField: str,
    vectorField: str,
```

## OpenSearchServerlessFieldMappingTypeDef

```python
# OpenSearchServerlessFieldMappingTypeDef definition

class OpenSearchServerlessFieldMappingTypeDef(TypedDict):
    metadataField: str,
    textField: str,
    vectorField: str,
```

## PatternObjectFilterOutputTypeDef

```python
# PatternObjectFilterOutputTypeDef definition

class PatternObjectFilterOutputTypeDef(TypedDict):
    objectType: str,
    exclusionFilters: NotRequired[List[str]],
    inclusionFilters: NotRequired[List[str]],
```

## PatternObjectFilterTypeDef

```python
# PatternObjectFilterTypeDef definition

class PatternObjectFilterTypeDef(TypedDict):
    objectType: str,
    exclusionFilters: NotRequired[Sequence[str]],
    inclusionFilters: NotRequired[Sequence[str]],
```

## PineconeFieldMappingTypeDef

```python
# PineconeFieldMappingTypeDef definition

class PineconeFieldMappingTypeDef(TypedDict):
    metadataField: str,
    textField: str,
```

## PrepareAgentRequestRequestTypeDef

```python
# PrepareAgentRequestRequestTypeDef definition

class PrepareAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
```

## PrepareFlowRequestRequestTypeDef

```python
# PrepareFlowRequestRequestTypeDef definition

class PrepareFlowRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
```

## PromptAgentResourceTypeDef

```python
# PromptAgentResourceTypeDef definition

class PromptAgentResourceTypeDef(TypedDict):
    agentIdentifier: str,
```

## PromptFlowNodeResourceConfigurationTypeDef

```python
# PromptFlowNodeResourceConfigurationTypeDef definition

class PromptFlowNodeResourceConfigurationTypeDef(TypedDict):
    promptArn: str,
```

## PromptModelInferenceConfigurationOutputTypeDef

```python
# PromptModelInferenceConfigurationOutputTypeDef definition

class PromptModelInferenceConfigurationOutputTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[List[str]],
    temperature: NotRequired[float],
    topP: NotRequired[float],
```

## PromptMetadataEntryTypeDef

```python
# PromptMetadataEntryTypeDef definition

class PromptMetadataEntryTypeDef(TypedDict):
    key: str,
    value: str,
```

## PromptModelInferenceConfigurationTypeDef

```python
# PromptModelInferenceConfigurationTypeDef definition

class PromptModelInferenceConfigurationTypeDef(TypedDict):
    maxTokens: NotRequired[int],
    stopSequences: NotRequired[Sequence[str]],
    temperature: NotRequired[float],
    topP: NotRequired[float],
```

## QueryGenerationColumnTypeDef

```python
# QueryGenerationColumnTypeDef definition

class QueryGenerationColumnTypeDef(TypedDict):
    description: NotRequired[str],
    inclusion: NotRequired[IncludeExcludeType],  # (1)
    name: NotRequired[str],
```

1. See [:material-code-brackets: IncludeExcludeType](./literals.md#includeexcludetype) 
## RdsFieldMappingTypeDef

```python
# RdsFieldMappingTypeDef definition

class RdsFieldMappingTypeDef(TypedDict):
    metadataField: str,
    primaryKeyField: str,
    textField: str,
    vectorField: str,
```

## RedisEnterpriseCloudFieldMappingTypeDef

```python
# RedisEnterpriseCloudFieldMappingTypeDef definition

class RedisEnterpriseCloudFieldMappingTypeDef(TypedDict):
    metadataField: str,
    textField: str,
    vectorField: str,
```

## RedshiftProvisionedAuthConfigurationTypeDef

```python
# RedshiftProvisionedAuthConfigurationTypeDef definition

class RedshiftProvisionedAuthConfigurationTypeDef(TypedDict):
    type: RedshiftProvisionedAuthTypeType,  # (1)
    databaseUser: NotRequired[str],
    usernamePasswordSecretArn: NotRequired[str],
```

1. See [:material-code-brackets: RedshiftProvisionedAuthTypeType](./literals.md#redshiftprovisionedauthtypetype) 
## RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef

```python
# RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef definition

class RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef(TypedDict):
    tableNames: List[str],
```

## RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef

```python
# RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef definition

class RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef(TypedDict):
    tableNames: Sequence[str],
```

## RedshiftQueryEngineRedshiftStorageConfigurationTypeDef

```python
# RedshiftQueryEngineRedshiftStorageConfigurationTypeDef definition

class RedshiftQueryEngineRedshiftStorageConfigurationTypeDef(TypedDict):
    databaseName: str,
```

## RedshiftServerlessAuthConfigurationTypeDef

```python
# RedshiftServerlessAuthConfigurationTypeDef definition

class RedshiftServerlessAuthConfigurationTypeDef(TypedDict):
    type: RedshiftServerlessAuthTypeType,  # (1)
    usernamePasswordSecretArn: NotRequired[str],
```

1. See [:material-code-brackets: RedshiftServerlessAuthTypeType](./literals.md#redshiftserverlessauthtypetype) 
## RetrievalFlowNodeS3ConfigurationTypeDef

```python
# RetrievalFlowNodeS3ConfigurationTypeDef definition

class RetrievalFlowNodeS3ConfigurationTypeDef(TypedDict):
    bucketName: str,
```

## S3DataSourceConfigurationTypeDef

```python
# S3DataSourceConfigurationTypeDef definition

class S3DataSourceConfigurationTypeDef(TypedDict):
    bucketArn: str,
    bucketOwnerAccountId: NotRequired[str],
    inclusionPrefixes: NotRequired[Sequence[str]],
```

## SalesforceSourceConfigurationTypeDef

```python
# SalesforceSourceConfigurationTypeDef definition

class SalesforceSourceConfigurationTypeDef(TypedDict):
    authType: SalesforceAuthTypeType,  # (1)
    credentialsSecretArn: str,
    hostUrl: str,
```

1. See [:material-code-brackets: SalesforceAuthTypeType](./literals.md#salesforceauthtypetype) 
## SeedUrlTypeDef

```python
# SeedUrlTypeDef definition

class SeedUrlTypeDef(TypedDict):
    url: NotRequired[str],
```

## SharePointSourceConfigurationOutputTypeDef

```python
# SharePointSourceConfigurationOutputTypeDef definition

class SharePointSourceConfigurationOutputTypeDef(TypedDict):
    authType: SharePointAuthTypeType,  # (1)
    credentialsSecretArn: str,
    domain: str,
    hostType: SharePointHostTypeType,  # (2)
    siteUrls: List[str],
    tenantId: NotRequired[str],
```

1. See [:material-code-brackets: SharePointAuthTypeType](./literals.md#sharepointauthtypetype) 
2. See [:material-code-brackets: SharePointHostTypeType](./literals.md#sharepointhosttypetype) 
## SharePointSourceConfigurationTypeDef

```python
# SharePointSourceConfigurationTypeDef definition

class SharePointSourceConfigurationTypeDef(TypedDict):
    authType: SharePointAuthTypeType,  # (1)
    credentialsSecretArn: str,
    domain: str,
    hostType: SharePointHostTypeType,  # (2)
    siteUrls: Sequence[str],
    tenantId: NotRequired[str],
```

1. See [:material-code-brackets: SharePointAuthTypeType](./literals.md#sharepointauthtypetype) 
2. See [:material-code-brackets: SharePointHostTypeType](./literals.md#sharepointhosttypetype) 
## SpecificToolChoiceTypeDef

```python
# SpecificToolChoiceTypeDef definition

class SpecificToolChoiceTypeDef(TypedDict):
    name: str,
```

## StartIngestionJobRequestRequestTypeDef

```python
# StartIngestionJobRequestRequestTypeDef definition

class StartIngestionJobRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## StopIngestionJobRequestRequestTypeDef

```python
# StopIngestionJobRequestRequestTypeDef definition

class StopIngestionJobRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
```

## StorageFlowNodeS3ConfigurationTypeDef

```python
# StorageFlowNodeS3ConfigurationTypeDef definition

class StorageFlowNodeS3ConfigurationTypeDef(TypedDict):
    bucketName: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## ToolInputSchemaOutputTypeDef

```python
# ToolInputSchemaOutputTypeDef definition

class ToolInputSchemaOutputTypeDef(TypedDict):
    json: NotRequired[Dict[str, Any]],
```

## ToolInputSchemaTypeDef

```python
# ToolInputSchemaTypeDef definition

class ToolInputSchemaTypeDef(TypedDict):
    json: NotRequired[Mapping[str, Any]],
```

## TransformationLambdaConfigurationTypeDef

```python
# TransformationLambdaConfigurationTypeDef definition

class TransformationLambdaConfigurationTypeDef(TypedDict):
    lambdaArn: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateAgentKnowledgeBaseRequestRequestTypeDef

```python
# UpdateAgentKnowledgeBaseRequestRequestTypeDef definition

class UpdateAgentKnowledgeBaseRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    knowledgeBaseId: str,
    description: NotRequired[str],
    knowledgeBaseState: NotRequired[KnowledgeBaseStateType],  # (1)
```

1. See [:material-code-brackets: KnowledgeBaseStateType](./literals.md#knowledgebasestatetype) 
## WebCrawlerLimitsTypeDef

```python
# WebCrawlerLimitsTypeDef definition

class WebCrawlerLimitsTypeDef(TypedDict):
    maxPages: NotRequired[int],
    rateLimit: NotRequired[int],
```

## APISchemaTypeDef

```python
# APISchemaTypeDef definition

class APISchemaTypeDef(TypedDict):
    payload: NotRequired[str],
    s3: NotRequired[S3IdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: S3IdentifierTypeDef](./type_defs.md#s3identifiertypedef) 
## AgentAliasHistoryEventTypeDef

```python
# AgentAliasHistoryEventTypeDef definition

class AgentAliasHistoryEventTypeDef(TypedDict):
    endDate: NotRequired[datetime],
    routingConfiguration: NotRequired[List[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
    startDate: NotRequired[datetime],
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
## AgentAliasSummaryTypeDef

```python
# AgentAliasSummaryTypeDef definition

class AgentAliasSummaryTypeDef(TypedDict):
    agentAliasId: str,
    agentAliasName: str,
    agentAliasStatus: AgentAliasStatusType,  # (1)
    createdAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
    routingConfiguration: NotRequired[List[AgentAliasRoutingConfigurationListItemTypeDef]],  # (2)
```

1. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype) 
2. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
## CreateAgentAliasRequestRequestTypeDef

```python
# CreateAgentAliasRequestRequestTypeDef definition

class CreateAgentAliasRequestRequestTypeDef(TypedDict):
    agentAliasName: str,
    agentId: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    routingConfiguration: NotRequired[Sequence[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
## UpdateAgentAliasRequestRequestTypeDef

```python
# UpdateAgentAliasRequestRequestTypeDef definition

class UpdateAgentAliasRequestRequestTypeDef(TypedDict):
    agentAliasId: str,
    agentAliasName: str,
    agentId: str,
    description: NotRequired[str],
    routingConfiguration: NotRequired[Sequence[AgentAliasRoutingConfigurationListItemTypeDef]],  # (1)
```

1. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
## AgentCollaboratorSummaryTypeDef

```python
# AgentCollaboratorSummaryTypeDef definition

class AgentCollaboratorSummaryTypeDef(TypedDict):
    agentDescriptor: AgentDescriptorTypeDef,  # (1)
    agentId: str,
    agentVersion: str,
    collaborationInstruction: str,
    collaboratorId: str,
    collaboratorName: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    relayConversationHistory: RelayConversationHistoryType,  # (2)
```

1. See [:material-code-braces: AgentDescriptorTypeDef](./type_defs.md#agentdescriptortypedef) 
2. See [:material-code-brackets: RelayConversationHistoryType](./literals.md#relayconversationhistorytype) 
## AgentCollaboratorTypeDef

```python
# AgentCollaboratorTypeDef definition

class AgentCollaboratorTypeDef(TypedDict):
    agentDescriptor: AgentDescriptorTypeDef,  # (1)
    agentId: str,
    agentVersion: str,
    collaborationInstruction: str,
    collaboratorId: str,
    collaboratorName: str,
    createdAt: datetime,
    lastUpdatedAt: datetime,
    clientToken: NotRequired[str],
    relayConversationHistory: NotRequired[RelayConversationHistoryType],  # (2)
```

1. See [:material-code-braces: AgentDescriptorTypeDef](./type_defs.md#agentdescriptortypedef) 
2. See [:material-code-brackets: RelayConversationHistoryType](./literals.md#relayconversationhistorytype) 
## AssociateAgentCollaboratorRequestRequestTypeDef

```python
# AssociateAgentCollaboratorRequestRequestTypeDef definition

class AssociateAgentCollaboratorRequestRequestTypeDef(TypedDict):
    agentDescriptor: AgentDescriptorTypeDef,  # (1)
    agentId: str,
    agentVersion: str,
    collaborationInstruction: str,
    collaboratorName: str,
    clientToken: NotRequired[str],
    relayConversationHistory: NotRequired[RelayConversationHistoryType],  # (2)
```

1. See [:material-code-braces: AgentDescriptorTypeDef](./type_defs.md#agentdescriptortypedef) 
2. See [:material-code-brackets: RelayConversationHistoryType](./literals.md#relayconversationhistorytype) 
## UpdateAgentCollaboratorRequestRequestTypeDef

```python
# UpdateAgentCollaboratorRequestRequestTypeDef definition

class UpdateAgentCollaboratorRequestRequestTypeDef(TypedDict):
    agentDescriptor: AgentDescriptorTypeDef,  # (1)
    agentId: str,
    agentVersion: str,
    collaborationInstruction: str,
    collaboratorId: str,
    collaboratorName: str,
    relayConversationHistory: NotRequired[RelayConversationHistoryType],  # (2)
```

1. See [:material-code-braces: AgentDescriptorTypeDef](./type_defs.md#agentdescriptortypedef) 
2. See [:material-code-brackets: RelayConversationHistoryType](./literals.md#relayconversationhistorytype) 
## AgentSummaryTypeDef

```python
# AgentSummaryTypeDef definition

class AgentSummaryTypeDef(TypedDict):
    agentId: str,
    agentName: str,
    agentStatus: AgentStatusType,  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
    latestAgentVersion: NotRequired[str],
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
## AgentVersionSummaryTypeDef

```python
# AgentVersionSummaryTypeDef definition

class AgentVersionSummaryTypeDef(TypedDict):
    agentName: str,
    agentStatus: AgentStatusType,  # (1)
    agentVersion: str,
    createdAt: datetime,
    updatedAt: datetime,
    description: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
## KnowledgeBaseFlowNodeConfigurationTypeDef

```python
# KnowledgeBaseFlowNodeConfigurationTypeDef definition

class KnowledgeBaseFlowNodeConfigurationTypeDef(TypedDict):
    knowledgeBaseId: str,
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
    modelId: NotRequired[str],
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
## AssociateAgentKnowledgeBaseResponseTypeDef

```python
# AssociateAgentKnowledgeBaseResponseTypeDef definition

class AssociateAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAgentAliasResponseTypeDef

```python
# DeleteAgentAliasResponseTypeDef definition

class DeleteAgentAliasResponseTypeDef(TypedDict):
    agentAliasId: str,
    agentAliasStatus: AgentAliasStatusType,  # (1)
    agentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAgentResponseTypeDef

```python
# DeleteAgentResponseTypeDef definition

class DeleteAgentResponseTypeDef(TypedDict):
    agentId: str,
    agentStatus: AgentStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAgentVersionResponseTypeDef

```python
# DeleteAgentVersionResponseTypeDef definition

class DeleteAgentVersionResponseTypeDef(TypedDict):
    agentId: str,
    agentStatus: AgentStatusType,  # (1)
    agentVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataSourceResponseTypeDef

```python
# DeleteDataSourceResponseTypeDef definition

class DeleteDataSourceResponseTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    status: DataSourceStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFlowAliasResponseTypeDef

```python
# DeleteFlowAliasResponseTypeDef definition

class DeleteFlowAliasResponseTypeDef(TypedDict):
    flowId: str,
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFlowResponseTypeDef

```python
# DeleteFlowResponseTypeDef definition

class DeleteFlowResponseTypeDef(TypedDict):
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteFlowVersionResponseTypeDef

```python
# DeleteFlowVersionResponseTypeDef definition

class DeleteFlowVersionResponseTypeDef(TypedDict):
    id: str,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteKnowledgeBaseResponseTypeDef

```python
# DeleteKnowledgeBaseResponseTypeDef definition

class DeleteKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBaseId: str,
    status: KnowledgeBaseStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePromptResponseTypeDef

```python
# DeletePromptResponseTypeDef definition

class DeletePromptResponseTypeDef(TypedDict):
    id: str,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentKnowledgeBaseResponseTypeDef

```python
# GetAgentKnowledgeBaseResponseTypeDef definition

class GetAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentActionGroupsResponseTypeDef

```python
# ListAgentActionGroupsResponseTypeDef definition

class ListAgentActionGroupsResponseTypeDef(TypedDict):
    actionGroupSummaries: List[ActionGroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ActionGroupSummaryTypeDef](./type_defs.md#actiongroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentKnowledgeBasesResponseTypeDef

```python
# ListAgentKnowledgeBasesResponseTypeDef definition

class ListAgentKnowledgeBasesResponseTypeDef(TypedDict):
    agentKnowledgeBaseSummaries: List[AgentKnowledgeBaseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentKnowledgeBaseSummaryTypeDef](./type_defs.md#agentknowledgebasesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PrepareAgentResponseTypeDef

```python
# PrepareAgentResponseTypeDef definition

class PrepareAgentResponseTypeDef(TypedDict):
    agentId: str,
    agentStatus: AgentStatusType,  # (1)
    agentVersion: str,
    preparedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PrepareFlowResponseTypeDef

```python
# PrepareFlowResponseTypeDef definition

class PrepareFlowResponseTypeDef(TypedDict):
    id: str,
    status: FlowStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentKnowledgeBaseResponseTypeDef

```python
# UpdateAgentKnowledgeBaseResponseTypeDef definition

class UpdateAgentKnowledgeBaseResponseTypeDef(TypedDict):
    agentKnowledgeBase: AgentKnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentKnowledgeBaseTypeDef](./type_defs.md#agentknowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmbeddingModelConfigurationTypeDef

```python
# EmbeddingModelConfigurationTypeDef definition

class EmbeddingModelConfigurationTypeDef(TypedDict):
    bedrockEmbeddingModelConfiguration: NotRequired[BedrockEmbeddingModelConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: BedrockEmbeddingModelConfigurationTypeDef](./type_defs.md#bedrockembeddingmodelconfigurationtypedef) 
## BedrockFoundationModelConfigurationTypeDef

```python
# BedrockFoundationModelConfigurationTypeDef definition

class BedrockFoundationModelConfigurationTypeDef(TypedDict):
    modelArn: str,
    parsingModality: NotRequired[ParsingModalityType],  # (1)
    parsingPrompt: NotRequired[ParsingPromptTypeDef],  # (2)
```

1. See [:material-code-brackets: ParsingModalityType](./literals.md#parsingmodalitytype) 
2. See [:material-code-braces: ParsingPromptTypeDef](./type_defs.md#parsingprompttypedef) 
## ByteContentDocTypeDef

```python
# ByteContentDocTypeDef definition

class ByteContentDocTypeDef(TypedDict):
    data: BlobTypeDef,
    mimeType: str,
```

## TextPromptTemplateConfigurationOutputTypeDef

```python
# TextPromptTemplateConfigurationOutputTypeDef definition

class TextPromptTemplateConfigurationOutputTypeDef(TypedDict):
    text: str,
    inputVariables: NotRequired[List[PromptInputVariableTypeDef]],  # (1)
```

1. See [:material-code-braces: PromptInputVariableTypeDef](./type_defs.md#promptinputvariabletypedef) 
## TextPromptTemplateConfigurationTypeDef

```python
# TextPromptTemplateConfigurationTypeDef definition

class TextPromptTemplateConfigurationTypeDef(TypedDict):
    text: str,
    inputVariables: NotRequired[Sequence[PromptInputVariableTypeDef]],  # (1)
```

1. See [:material-code-braces: PromptInputVariableTypeDef](./type_defs.md#promptinputvariabletypedef) 
## ConditionFlowNodeConfigurationOutputTypeDef

```python
# ConditionFlowNodeConfigurationOutputTypeDef definition

class ConditionFlowNodeConfigurationOutputTypeDef(TypedDict):
    conditions: List[FlowConditionTypeDef],  # (1)
```

1. See [:material-code-braces: FlowConditionTypeDef](./type_defs.md#flowconditiontypedef) 
## ConditionFlowNodeConfigurationTypeDef

```python
# ConditionFlowNodeConfigurationTypeDef definition

class ConditionFlowNodeConfigurationTypeDef(TypedDict):
    conditions: Sequence[FlowConditionTypeDef],  # (1)
```

1. See [:material-code-braces: FlowConditionTypeDef](./type_defs.md#flowconditiontypedef) 
## MessageOutputTypeDef

```python
# MessageOutputTypeDef definition

class MessageOutputTypeDef(TypedDict):
    content: List[ContentBlockTypeDef],  # (1)
    role: ConversationRoleType,  # (2)
```

1. See [:material-code-braces: ContentBlockTypeDef](./type_defs.md#contentblocktypedef) 
2. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype) 
## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    content: Sequence[ContentBlockTypeDef],  # (1)
    role: ConversationRoleType,  # (2)
```

1. See [:material-code-braces: ContentBlockTypeDef](./type_defs.md#contentblocktypedef) 
2. See [:material-code-brackets: ConversationRoleType](./literals.md#conversationroletype) 
## CreateFlowAliasRequestRequestTypeDef

```python
# CreateFlowAliasRequestRequestTypeDef definition

class CreateFlowAliasRequestRequestTypeDef(TypedDict):
    flowIdentifier: str,
    name: str,
    routingConfiguration: Sequence[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef) 
## CreateFlowAliasResponseTypeDef

```python
# CreateFlowAliasResponseTypeDef definition

class CreateFlowAliasResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    description: str,
    flowId: str,
    id: str,
    name: str,
    routingConfiguration: List[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FlowAliasSummaryTypeDef

```python
# FlowAliasSummaryTypeDef definition

class FlowAliasSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    flowId: str,
    id: str,
    name: str,
    routingConfiguration: List[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    updatedAt: datetime,
    description: NotRequired[str],
```

1. See [:material-code-braces: FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef) 
## GetFlowAliasResponseTypeDef

```python
# GetFlowAliasResponseTypeDef definition

class GetFlowAliasResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    description: str,
    flowId: str,
    id: str,
    name: str,
    routingConfiguration: List[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFlowAliasRequestRequestTypeDef

```python
# UpdateFlowAliasRequestRequestTypeDef definition

class UpdateFlowAliasRequestRequestTypeDef(TypedDict):
    aliasIdentifier: str,
    flowIdentifier: str,
    name: str,
    routingConfiguration: Sequence[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef) 
## UpdateFlowAliasResponseTypeDef

```python
# UpdateFlowAliasResponseTypeDef definition

class UpdateFlowAliasResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    description: str,
    flowId: str,
    id: str,
    name: str,
    routingConfiguration: List[FlowAliasRoutingConfigurationListItemTypeDef],  # (1)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowAliasRoutingConfigurationListItemTypeDef](./type_defs.md#flowaliasroutingconfigurationlistitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomOrchestrationTypeDef

```python
# CustomOrchestrationTypeDef definition

class CustomOrchestrationTypeDef(TypedDict):
    executor: NotRequired[OrchestrationExecutorTypeDef],  # (1)
```

1. See [:material-code-braces: OrchestrationExecutorTypeDef](./type_defs.md#orchestrationexecutortypedef) 
## ListDataSourcesResponseTypeDef

```python
# ListDataSourcesResponseTypeDef definition

class ListDataSourcesResponseTypeDef(TypedDict):
    dataSourceSummaries: List[DataSourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceSummaryTypeDef](./type_defs.md#datasourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentIdentifierTypeDef

```python
# DocumentIdentifierTypeDef definition

class DocumentIdentifierTypeDef(TypedDict):
    dataSourceType: ContentDataSourceTypeType,  # (2)
    custom: NotRequired[CustomDocumentIdentifierTypeDef],  # (1)
    s3: NotRequired[S3LocationTypeDef],  # (3)
```

1. See [:material-code-braces: CustomDocumentIdentifierTypeDef](./type_defs.md#customdocumentidentifiertypedef) 
2. See [:material-code-brackets: ContentDataSourceTypeType](./literals.md#contentdatasourcetypetype) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## IntermediateStorageTypeDef

```python
# IntermediateStorageTypeDef definition

class IntermediateStorageTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## S3ContentTypeDef

```python
# S3ContentTypeDef definition

class S3ContentTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## SupplementalDataStorageLocationTypeDef

```python
# SupplementalDataStorageLocationTypeDef definition

class SupplementalDataStorageLocationTypeDef(TypedDict):
    type: SupplementalDataStorageLocationTypeType,  # (2)
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-brackets: SupplementalDataStorageLocationTypeType](./literals.md#supplementaldatastoragelocationtypetype) 
## FlowConnectionConfigurationTypeDef

```python
# FlowConnectionConfigurationTypeDef definition

class FlowConnectionConfigurationTypeDef(TypedDict):
    conditional: NotRequired[FlowConditionalConnectionConfigurationTypeDef],  # (1)
    data: NotRequired[FlowDataConnectionConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: FlowConditionalConnectionConfigurationTypeDef](./type_defs.md#flowconditionalconnectionconfigurationtypedef) 
2. See [:material-code-braces: FlowDataConnectionConfigurationTypeDef](./type_defs.md#flowdataconnectionconfigurationtypedef) 
## ListFlowsResponseTypeDef

```python
# ListFlowsResponseTypeDef definition

class ListFlowsResponseTypeDef(TypedDict):
    flowSummaries: List[FlowSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FlowSummaryTypeDef](./type_defs.md#flowsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FlowValidationDetailsTypeDef

```python
# FlowValidationDetailsTypeDef definition

class FlowValidationDetailsTypeDef(TypedDict):
    cyclicConnection: NotRequired[CyclicConnectionFlowValidationDetailsTypeDef],  # (1)
    duplicateConditionExpression: NotRequired[DuplicateConditionExpressionFlowValidationDetailsTypeDef],  # (2)
    duplicateConnections: NotRequired[DuplicateConnectionsFlowValidationDetailsTypeDef],  # (3)
    incompatibleConnectionDataType: NotRequired[IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef],  # (4)
    malformedConditionExpression: NotRequired[MalformedConditionExpressionFlowValidationDetailsTypeDef],  # (5)
    malformedNodeInputExpression: NotRequired[MalformedNodeInputExpressionFlowValidationDetailsTypeDef],  # (6)
    mismatchedNodeInputType: NotRequired[MismatchedNodeInputTypeFlowValidationDetailsTypeDef],  # (7)
    mismatchedNodeOutputType: NotRequired[MismatchedNodeOutputTypeFlowValidationDetailsTypeDef],  # (8)
    missingConnectionConfiguration: NotRequired[MissingConnectionConfigurationFlowValidationDetailsTypeDef],  # (9)
    missingDefaultCondition: NotRequired[MissingDefaultConditionFlowValidationDetailsTypeDef],  # (10)
    missingEndingNodes: NotRequired[Dict[str, Any]],
    missingNodeConfiguration: NotRequired[MissingNodeConfigurationFlowValidationDetailsTypeDef],  # (11)
    missingNodeInput: NotRequired[MissingNodeInputFlowValidationDetailsTypeDef],  # (12)
    missingNodeOutput: NotRequired[MissingNodeOutputFlowValidationDetailsTypeDef],  # (13)
    missingStartingNodes: NotRequired[Dict[str, Any]],
    multipleNodeInputConnections: NotRequired[MultipleNodeInputConnectionsFlowValidationDetailsTypeDef],  # (14)
    unfulfilledNodeInput: NotRequired[UnfulfilledNodeInputFlowValidationDetailsTypeDef],  # (15)
    unknownConnectionCondition: NotRequired[UnknownConnectionConditionFlowValidationDetailsTypeDef],  # (16)
    unknownConnectionSource: NotRequired[UnknownConnectionSourceFlowValidationDetailsTypeDef],  # (17)
    unknownConnectionSourceOutput: NotRequired[UnknownConnectionSourceOutputFlowValidationDetailsTypeDef],  # (18)
    unknownConnectionTarget: NotRequired[UnknownConnectionTargetFlowValidationDetailsTypeDef],  # (19)
    unknownConnectionTargetInput: NotRequired[UnknownConnectionTargetInputFlowValidationDetailsTypeDef],  # (20)
    unreachableNode: NotRequired[UnreachableNodeFlowValidationDetailsTypeDef],  # (21)
    unsatisfiedConnectionConditions: NotRequired[UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef],  # (22)
    unspecified: NotRequired[Dict[str, Any]],
```

1. See [:material-code-braces: CyclicConnectionFlowValidationDetailsTypeDef](./type_defs.md#cyclicconnectionflowvalidationdetailstypedef) 
2. See [:material-code-braces: DuplicateConditionExpressionFlowValidationDetailsTypeDef](./type_defs.md#duplicateconditionexpressionflowvalidationdetailstypedef) 
3. See [:material-code-braces: DuplicateConnectionsFlowValidationDetailsTypeDef](./type_defs.md#duplicateconnectionsflowvalidationdetailstypedef) 
4. See [:material-code-braces: IncompatibleConnectionDataTypeFlowValidationDetailsTypeDef](./type_defs.md#incompatibleconnectiondatatypeflowvalidationdetailstypedef) 
5. See [:material-code-braces: MalformedConditionExpressionFlowValidationDetailsTypeDef](./type_defs.md#malformedconditionexpressionflowvalidationdetailstypedef) 
6. See [:material-code-braces: MalformedNodeInputExpressionFlowValidationDetailsTypeDef](./type_defs.md#malformednodeinputexpressionflowvalidationdetailstypedef) 
7. See [:material-code-braces: MismatchedNodeInputTypeFlowValidationDetailsTypeDef](./type_defs.md#mismatchednodeinputtypeflowvalidationdetailstypedef) 
8. See [:material-code-braces: MismatchedNodeOutputTypeFlowValidationDetailsTypeDef](./type_defs.md#mismatchednodeoutputtypeflowvalidationdetailstypedef) 
9. See [:material-code-braces: MissingConnectionConfigurationFlowValidationDetailsTypeDef](./type_defs.md#missingconnectionconfigurationflowvalidationdetailstypedef) 
10. See [:material-code-braces: MissingDefaultConditionFlowValidationDetailsTypeDef](./type_defs.md#missingdefaultconditionflowvalidationdetailstypedef) 
11. See [:material-code-braces: MissingNodeConfigurationFlowValidationDetailsTypeDef](./type_defs.md#missingnodeconfigurationflowvalidationdetailstypedef) 
12. See [:material-code-braces: MissingNodeInputFlowValidationDetailsTypeDef](./type_defs.md#missingnodeinputflowvalidationdetailstypedef) 
13. See [:material-code-braces: MissingNodeOutputFlowValidationDetailsTypeDef](./type_defs.md#missingnodeoutputflowvalidationdetailstypedef) 
14. See [:material-code-braces: MultipleNodeInputConnectionsFlowValidationDetailsTypeDef](./type_defs.md#multiplenodeinputconnectionsflowvalidationdetailstypedef) 
15. See [:material-code-braces: UnfulfilledNodeInputFlowValidationDetailsTypeDef](./type_defs.md#unfulfillednodeinputflowvalidationdetailstypedef) 
16. See [:material-code-braces: UnknownConnectionConditionFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectionconditionflowvalidationdetailstypedef) 
17. See [:material-code-braces: UnknownConnectionSourceFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectionsourceflowvalidationdetailstypedef) 
18. See [:material-code-braces: UnknownConnectionSourceOutputFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectionsourceoutputflowvalidationdetailstypedef) 
19. See [:material-code-braces: UnknownConnectionTargetFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectiontargetflowvalidationdetailstypedef) 
20. See [:material-code-braces: UnknownConnectionTargetInputFlowValidationDetailsTypeDef](./type_defs.md#unknownconnectiontargetinputflowvalidationdetailstypedef) 
21. See [:material-code-braces: UnreachableNodeFlowValidationDetailsTypeDef](./type_defs.md#unreachablenodeflowvalidationdetailstypedef) 
22. See [:material-code-braces: UnsatisfiedConnectionConditionsFlowValidationDetailsTypeDef](./type_defs.md#unsatisfiedconnectionconditionsflowvalidationdetailstypedef) 
## ListFlowVersionsResponseTypeDef

```python
# ListFlowVersionsResponseTypeDef definition

class ListFlowVersionsResponseTypeDef(TypedDict):
    flowVersionSummaries: List[FlowVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FlowVersionSummaryTypeDef](./type_defs.md#flowversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FunctionOutputTypeDef

```python
# FunctionOutputTypeDef definition

class FunctionOutputTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    parameters: NotRequired[Dict[str, ParameterDetailTypeDef]],  # (1)
    requireConfirmation: NotRequired[RequireConfirmationType],  # (2)
```

1. See [:material-code-braces: ParameterDetailTypeDef](./type_defs.md#parameterdetailtypedef) 
2. See [:material-code-brackets: RequireConfirmationType](./literals.md#requireconfirmationtype) 
## FunctionTypeDef

```python
# FunctionTypeDef definition

class FunctionTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    parameters: NotRequired[Mapping[str, ParameterDetailTypeDef]],  # (1)
    requireConfirmation: NotRequired[RequireConfirmationType],  # (2)
```

1. See [:material-code-braces: ParameterDetailTypeDef](./type_defs.md#parameterdetailtypedef) 
2. See [:material-code-brackets: RequireConfirmationType](./literals.md#requireconfirmationtype) 
## HierarchicalChunkingConfigurationOutputTypeDef

```python
# HierarchicalChunkingConfigurationOutputTypeDef definition

class HierarchicalChunkingConfigurationOutputTypeDef(TypedDict):
    levelConfigurations: List[HierarchicalChunkingLevelConfigurationTypeDef],  # (1)
    overlapTokens: int,
```

1. See [:material-code-braces: HierarchicalChunkingLevelConfigurationTypeDef](./type_defs.md#hierarchicalchunkinglevelconfigurationtypedef) 
## HierarchicalChunkingConfigurationTypeDef

```python
# HierarchicalChunkingConfigurationTypeDef definition

class HierarchicalChunkingConfigurationTypeDef(TypedDict):
    levelConfigurations: Sequence[HierarchicalChunkingLevelConfigurationTypeDef],  # (1)
    overlapTokens: int,
```

1. See [:material-code-braces: HierarchicalChunkingLevelConfigurationTypeDef](./type_defs.md#hierarchicalchunkinglevelconfigurationtypedef) 
## PromptConfigurationOutputTypeDef

```python
# PromptConfigurationOutputTypeDef definition

class PromptConfigurationOutputTypeDef(TypedDict):
    basePromptTemplate: NotRequired[str],
    foundationModel: NotRequired[str],
    inferenceConfiguration: NotRequired[InferenceConfigurationOutputTypeDef],  # (1)
    parserMode: NotRequired[CreationModeType],  # (2)
    promptCreationMode: NotRequired[CreationModeType],  # (2)
    promptState: NotRequired[PromptStateType],  # (4)
    promptType: NotRequired[PromptTypeType],  # (5)
```

1. See [:material-code-braces: InferenceConfigurationOutputTypeDef](./type_defs.md#inferenceconfigurationoutputtypedef) 
2. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
3. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
4. See [:material-code-brackets: PromptStateType](./literals.md#promptstatetype) 
5. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype) 
## ListIngestionJobsRequestRequestTypeDef

```python
# ListIngestionJobsRequestRequestTypeDef definition

class ListIngestionJobsRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    filters: NotRequired[Sequence[IngestionJobFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[IngestionJobSortByTypeDef],  # (2)
```

1. See [:material-code-braces: IngestionJobFilterTypeDef](./type_defs.md#ingestionjobfiltertypedef) 
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef) 
## IngestionJobSummaryTypeDef

```python
# IngestionJobSummaryTypeDef definition

class IngestionJobSummaryTypeDef(TypedDict):
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
    startedAt: datetime,
    status: IngestionJobStatusType,  # (2)
    updatedAt: datetime,
    description: NotRequired[str],
    statistics: NotRequired[IngestionJobStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: IngestionJobStatisticsTypeDef](./type_defs.md#ingestionjobstatisticstypedef) 
2. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
## IngestionJobTypeDef

```python
# IngestionJobTypeDef definition

class IngestionJobTypeDef(TypedDict):
    dataSourceId: str,
    ingestionJobId: str,
    knowledgeBaseId: str,
    startedAt: datetime,
    status: IngestionJobStatusType,  # (2)
    updatedAt: datetime,
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    statistics: NotRequired[IngestionJobStatisticsTypeDef],  # (1)
```

1. See [:material-code-braces: IngestionJobStatisticsTypeDef](./type_defs.md#ingestionjobstatisticstypedef) 
2. See [:material-code-brackets: IngestionJobStatusType](./literals.md#ingestionjobstatustype) 
## ListKnowledgeBasesResponseTypeDef

```python
# ListKnowledgeBasesResponseTypeDef definition

class ListKnowledgeBasesResponseTypeDef(TypedDict):
    knowledgeBaseSummaries: List[KnowledgeBaseSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KnowledgeBaseSummaryTypeDef](./type_defs.md#knowledgebasesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentActionGroupsRequestPaginateTypeDef

```python
# ListAgentActionGroupsRequestPaginateTypeDef definition

class ListAgentActionGroupsRequestPaginateTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentAliasesRequestPaginateTypeDef

```python
# ListAgentAliasesRequestPaginateTypeDef definition

class ListAgentAliasesRequestPaginateTypeDef(TypedDict):
    agentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentCollaboratorsRequestPaginateTypeDef

```python
# ListAgentCollaboratorsRequestPaginateTypeDef definition

class ListAgentCollaboratorsRequestPaginateTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentKnowledgeBasesRequestPaginateTypeDef

```python
# ListAgentKnowledgeBasesRequestPaginateTypeDef definition

class ListAgentKnowledgeBasesRequestPaginateTypeDef(TypedDict):
    agentId: str,
    agentVersion: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentVersionsRequestPaginateTypeDef

```python
# ListAgentVersionsRequestPaginateTypeDef definition

class ListAgentVersionsRequestPaginateTypeDef(TypedDict):
    agentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAgentsRequestPaginateTypeDef

```python
# ListAgentsRequestPaginateTypeDef definition

class ListAgentsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourcesRequestPaginateTypeDef

```python
# ListDataSourcesRequestPaginateTypeDef definition

class ListDataSourcesRequestPaginateTypeDef(TypedDict):
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowAliasesRequestPaginateTypeDef

```python
# ListFlowAliasesRequestPaginateTypeDef definition

class ListFlowAliasesRequestPaginateTypeDef(TypedDict):
    flowIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowVersionsRequestPaginateTypeDef

```python
# ListFlowVersionsRequestPaginateTypeDef definition

class ListFlowVersionsRequestPaginateTypeDef(TypedDict):
    flowIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListFlowsRequestPaginateTypeDef

```python
# ListFlowsRequestPaginateTypeDef definition

class ListFlowsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListIngestionJobsRequestPaginateTypeDef

```python
# ListIngestionJobsRequestPaginateTypeDef definition

class ListIngestionJobsRequestPaginateTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    filters: NotRequired[Sequence[IngestionJobFilterTypeDef]],  # (1)
    sortBy: NotRequired[IngestionJobSortByTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: IngestionJobFilterTypeDef](./type_defs.md#ingestionjobfiltertypedef) 
2. See [:material-code-braces: IngestionJobSortByTypeDef](./type_defs.md#ingestionjobsortbytypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKnowledgeBaseDocumentsRequestPaginateTypeDef

```python
# ListKnowledgeBaseDocumentsRequestPaginateTypeDef definition

class ListKnowledgeBaseDocumentsRequestPaginateTypeDef(TypedDict):
    dataSourceId: str,
    knowledgeBaseId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListKnowledgeBasesRequestPaginateTypeDef

```python
# ListKnowledgeBasesRequestPaginateTypeDef definition

class ListKnowledgeBasesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPromptsRequestPaginateTypeDef

```python
# ListPromptsRequestPaginateTypeDef definition

class ListPromptsRequestPaginateTypeDef(TypedDict):
    promptIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPromptsResponseTypeDef

```python
# ListPromptsResponseTypeDef definition

class ListPromptsResponseTypeDef(TypedDict):
    promptSummaries: List[PromptSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PromptSummaryTypeDef](./type_defs.md#promptsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MemoryConfigurationOutputTypeDef

```python
# MemoryConfigurationOutputTypeDef definition

class MemoryConfigurationOutputTypeDef(TypedDict):
    enabledMemoryTypes: List[MemoryTypeType],  # (1)
    sessionSummaryConfiguration: NotRequired[SessionSummaryConfigurationTypeDef],  # (2)
    storageDays: NotRequired[int],
```

1. See [:material-code-brackets: MemoryTypeType](./literals.md#memorytypetype) 
2. See [:material-code-braces: SessionSummaryConfigurationTypeDef](./type_defs.md#sessionsummaryconfigurationtypedef) 
## MemoryConfigurationTypeDef

```python
# MemoryConfigurationTypeDef definition

class MemoryConfigurationTypeDef(TypedDict):
    enabledMemoryTypes: Sequence[MemoryTypeType],  # (1)
    sessionSummaryConfiguration: NotRequired[SessionSummaryConfigurationTypeDef],  # (2)
    storageDays: NotRequired[int],
```

1. See [:material-code-brackets: MemoryTypeType](./literals.md#memorytypetype) 
2. See [:material-code-braces: SessionSummaryConfigurationTypeDef](./type_defs.md#sessionsummaryconfigurationtypedef) 
## MetadataAttributeTypeDef

```python
# MetadataAttributeTypeDef definition

class MetadataAttributeTypeDef(TypedDict):
    key: str,
    value: MetadataAttributeValueTypeDef,  # (1)
```

1. See [:material-code-braces: MetadataAttributeValueTypeDef](./type_defs.md#metadataattributevaluetypedef) 
## MongoDbAtlasConfigurationTypeDef

```python
# MongoDbAtlasConfigurationTypeDef definition

class MongoDbAtlasConfigurationTypeDef(TypedDict):
    collectionName: str,
    credentialsSecretArn: str,
    databaseName: str,
    endpoint: str,
    fieldMapping: MongoDbAtlasFieldMappingTypeDef,  # (1)
    vectorIndexName: str,
    endpointServiceName: NotRequired[str],
```

1. See [:material-code-braces: MongoDbAtlasFieldMappingTypeDef](./type_defs.md#mongodbatlasfieldmappingtypedef) 
## OpenSearchServerlessConfigurationTypeDef

```python
# OpenSearchServerlessConfigurationTypeDef definition

class OpenSearchServerlessConfigurationTypeDef(TypedDict):
    collectionArn: str,
    fieldMapping: OpenSearchServerlessFieldMappingTypeDef,  # (1)
    vectorIndexName: str,
```

1. See [:material-code-braces: OpenSearchServerlessFieldMappingTypeDef](./type_defs.md#opensearchserverlessfieldmappingtypedef) 
## PatternObjectFilterConfigurationOutputTypeDef

```python
# PatternObjectFilterConfigurationOutputTypeDef definition

class PatternObjectFilterConfigurationOutputTypeDef(TypedDict):
    filters: List[PatternObjectFilterOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PatternObjectFilterOutputTypeDef](./type_defs.md#patternobjectfilteroutputtypedef) 
## PineconeConfigurationTypeDef

```python
# PineconeConfigurationTypeDef definition

class PineconeConfigurationTypeDef(TypedDict):
    connectionString: str,
    credentialsSecretArn: str,
    fieldMapping: PineconeFieldMappingTypeDef,  # (1)
    namespace: NotRequired[str],
```

1. See [:material-code-braces: PineconeFieldMappingTypeDef](./type_defs.md#pineconefieldmappingtypedef) 
## PromptGenAiResourceTypeDef

```python
# PromptGenAiResourceTypeDef definition

class PromptGenAiResourceTypeDef(TypedDict):
    agent: NotRequired[PromptAgentResourceTypeDef],  # (1)
```

1. See [:material-code-braces: PromptAgentResourceTypeDef](./type_defs.md#promptagentresourcetypedef) 
## PromptInferenceConfigurationOutputTypeDef

```python
# PromptInferenceConfigurationOutputTypeDef definition

class PromptInferenceConfigurationOutputTypeDef(TypedDict):
    text: NotRequired[PromptModelInferenceConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PromptModelInferenceConfigurationOutputTypeDef](./type_defs.md#promptmodelinferenceconfigurationoutputtypedef) 
## QueryGenerationTableOutputTypeDef

```python
# QueryGenerationTableOutputTypeDef definition

class QueryGenerationTableOutputTypeDef(TypedDict):
    name: str,
    columns: NotRequired[List[QueryGenerationColumnTypeDef]],  # (1)
    description: NotRequired[str],
    inclusion: NotRequired[IncludeExcludeType],  # (2)
```

1. See [:material-code-braces: QueryGenerationColumnTypeDef](./type_defs.md#querygenerationcolumntypedef) 
2. See [:material-code-brackets: IncludeExcludeType](./literals.md#includeexcludetype) 
## QueryGenerationTableTypeDef

```python
# QueryGenerationTableTypeDef definition

class QueryGenerationTableTypeDef(TypedDict):
    name: str,
    columns: NotRequired[Sequence[QueryGenerationColumnTypeDef]],  # (1)
    description: NotRequired[str],
    inclusion: NotRequired[IncludeExcludeType],  # (2)
```

1. See [:material-code-braces: QueryGenerationColumnTypeDef](./type_defs.md#querygenerationcolumntypedef) 
2. See [:material-code-brackets: IncludeExcludeType](./literals.md#includeexcludetype) 
## RdsConfigurationTypeDef

```python
# RdsConfigurationTypeDef definition

class RdsConfigurationTypeDef(TypedDict):
    credentialsSecretArn: str,
    databaseName: str,
    fieldMapping: RdsFieldMappingTypeDef,  # (1)
    resourceArn: str,
    tableName: str,
```

1. See [:material-code-braces: RdsFieldMappingTypeDef](./type_defs.md#rdsfieldmappingtypedef) 
## RedisEnterpriseCloudConfigurationTypeDef

```python
# RedisEnterpriseCloudConfigurationTypeDef definition

class RedisEnterpriseCloudConfigurationTypeDef(TypedDict):
    credentialsSecretArn: str,
    endpoint: str,
    fieldMapping: RedisEnterpriseCloudFieldMappingTypeDef,  # (1)
    vectorIndexName: str,
```

1. See [:material-code-braces: RedisEnterpriseCloudFieldMappingTypeDef](./type_defs.md#redisenterprisecloudfieldmappingtypedef) 
## RedshiftProvisionedConfigurationTypeDef

```python
# RedshiftProvisionedConfigurationTypeDef definition

class RedshiftProvisionedConfigurationTypeDef(TypedDict):
    authConfiguration: RedshiftProvisionedAuthConfigurationTypeDef,  # (1)
    clusterIdentifier: str,
```

1. See [:material-code-braces: RedshiftProvisionedAuthConfigurationTypeDef](./type_defs.md#redshiftprovisionedauthconfigurationtypedef) 
## RedshiftQueryEngineStorageConfigurationOutputTypeDef

```python
# RedshiftQueryEngineStorageConfigurationOutputTypeDef definition

class RedshiftQueryEngineStorageConfigurationOutputTypeDef(TypedDict):
    type: RedshiftQueryEngineStorageTypeType,  # (3)
    awsDataCatalogConfiguration: NotRequired[RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef],  # (1)
    redshiftConfiguration: NotRequired[RedshiftQueryEngineRedshiftStorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef](./type_defs.md#redshiftqueryengineawsdatacatalogstorageconfigurationoutputtypedef) 
2. See [:material-code-braces: RedshiftQueryEngineRedshiftStorageConfigurationTypeDef](./type_defs.md#redshiftqueryengineredshiftstorageconfigurationtypedef) 
3. See [:material-code-brackets: RedshiftQueryEngineStorageTypeType](./literals.md#redshiftqueryenginestoragetypetype) 
## RedshiftServerlessConfigurationTypeDef

```python
# RedshiftServerlessConfigurationTypeDef definition

class RedshiftServerlessConfigurationTypeDef(TypedDict):
    authConfiguration: RedshiftServerlessAuthConfigurationTypeDef,  # (1)
    workgroupArn: str,
```

1. See [:material-code-braces: RedshiftServerlessAuthConfigurationTypeDef](./type_defs.md#redshiftserverlessauthconfigurationtypedef) 
## RetrievalFlowNodeServiceConfigurationTypeDef

```python
# RetrievalFlowNodeServiceConfigurationTypeDef definition

class RetrievalFlowNodeServiceConfigurationTypeDef(TypedDict):
    s3: NotRequired[RetrievalFlowNodeS3ConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: RetrievalFlowNodeS3ConfigurationTypeDef](./type_defs.md#retrievalflownodes3configurationtypedef) 
## UrlConfigurationOutputTypeDef

```python
# UrlConfigurationOutputTypeDef definition

class UrlConfigurationOutputTypeDef(TypedDict):
    seedUrls: NotRequired[List[SeedUrlTypeDef]],  # (1)
```

1. See [:material-code-braces: SeedUrlTypeDef](./type_defs.md#seedurltypedef) 
## UrlConfigurationTypeDef

```python
# UrlConfigurationTypeDef definition

class UrlConfigurationTypeDef(TypedDict):
    seedUrls: NotRequired[Sequence[SeedUrlTypeDef]],  # (1)
```

1. See [:material-code-braces: SeedUrlTypeDef](./type_defs.md#seedurltypedef) 
## ToolChoiceOutputTypeDef

```python
# ToolChoiceOutputTypeDef definition

class ToolChoiceOutputTypeDef(TypedDict):
    any: NotRequired[Dict[str, Any]],
    auto: NotRequired[Dict[str, Any]],
    tool: NotRequired[SpecificToolChoiceTypeDef],  # (1)
```

1. See [:material-code-braces: SpecificToolChoiceTypeDef](./type_defs.md#specifictoolchoicetypedef) 
## ToolChoiceTypeDef

```python
# ToolChoiceTypeDef definition

class ToolChoiceTypeDef(TypedDict):
    any: NotRequired[Mapping[str, Any]],
    auto: NotRequired[Mapping[str, Any]],
    tool: NotRequired[SpecificToolChoiceTypeDef],  # (1)
```

1. See [:material-code-braces: SpecificToolChoiceTypeDef](./type_defs.md#specifictoolchoicetypedef) 
## StorageFlowNodeServiceConfigurationTypeDef

```python
# StorageFlowNodeServiceConfigurationTypeDef definition

class StorageFlowNodeServiceConfigurationTypeDef(TypedDict):
    s3: NotRequired[StorageFlowNodeS3ConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: StorageFlowNodeS3ConfigurationTypeDef](./type_defs.md#storageflownodes3configurationtypedef) 
## ToolSpecificationOutputTypeDef

```python
# ToolSpecificationOutputTypeDef definition

class ToolSpecificationOutputTypeDef(TypedDict):
    inputSchema: ToolInputSchemaOutputTypeDef,  # (1)
    name: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: ToolInputSchemaOutputTypeDef](./type_defs.md#toolinputschemaoutputtypedef) 
## TransformationFunctionTypeDef

```python
# TransformationFunctionTypeDef definition

class TransformationFunctionTypeDef(TypedDict):
    transformationLambdaConfiguration: TransformationLambdaConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: TransformationLambdaConfigurationTypeDef](./type_defs.md#transformationlambdaconfigurationtypedef) 
## WebCrawlerConfigurationOutputTypeDef

```python
# WebCrawlerConfigurationOutputTypeDef definition

class WebCrawlerConfigurationOutputTypeDef(TypedDict):
    crawlerLimits: NotRequired[WebCrawlerLimitsTypeDef],  # (1)
    exclusionFilters: NotRequired[List[str]],
    inclusionFilters: NotRequired[List[str]],
    scope: NotRequired[WebScopeTypeType],  # (2)
    userAgent: NotRequired[str],
```

1. See [:material-code-braces: WebCrawlerLimitsTypeDef](./type_defs.md#webcrawlerlimitstypedef) 
2. See [:material-code-brackets: WebScopeTypeType](./literals.md#webscopetypetype) 
## WebCrawlerConfigurationTypeDef

```python
# WebCrawlerConfigurationTypeDef definition

class WebCrawlerConfigurationTypeDef(TypedDict):
    crawlerLimits: NotRequired[WebCrawlerLimitsTypeDef],  # (1)
    exclusionFilters: NotRequired[Sequence[str]],
    inclusionFilters: NotRequired[Sequence[str]],
    scope: NotRequired[WebScopeTypeType],  # (2)
    userAgent: NotRequired[str],
```

1. See [:material-code-braces: WebCrawlerLimitsTypeDef](./type_defs.md#webcrawlerlimitstypedef) 
2. See [:material-code-brackets: WebScopeTypeType](./literals.md#webscopetypetype) 
## AgentAliasTypeDef

```python
# AgentAliasTypeDef definition

class AgentAliasTypeDef(TypedDict):
    agentAliasArn: str,
    agentAliasId: str,
    agentAliasName: str,
    agentAliasStatus: AgentAliasStatusType,  # (2)
    agentId: str,
    createdAt: datetime,
    routingConfiguration: List[AgentAliasRoutingConfigurationListItemTypeDef],  # (3)
    updatedAt: datetime,
    agentAliasHistoryEvents: NotRequired[List[AgentAliasHistoryEventTypeDef]],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
```

1. See [:material-code-braces: AgentAliasHistoryEventTypeDef](./type_defs.md#agentaliashistoryeventtypedef) 
2. See [:material-code-brackets: AgentAliasStatusType](./literals.md#agentaliasstatustype) 
3. See [:material-code-braces: AgentAliasRoutingConfigurationListItemTypeDef](./type_defs.md#agentaliasroutingconfigurationlistitemtypedef) 
## ListAgentAliasesResponseTypeDef

```python
# ListAgentAliasesResponseTypeDef definition

class ListAgentAliasesResponseTypeDef(TypedDict):
    agentAliasSummaries: List[AgentAliasSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentAliasSummaryTypeDef](./type_defs.md#agentaliassummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentCollaboratorsResponseTypeDef

```python
# ListAgentCollaboratorsResponseTypeDef definition

class ListAgentCollaboratorsResponseTypeDef(TypedDict):
    agentCollaboratorSummaries: List[AgentCollaboratorSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentCollaboratorSummaryTypeDef](./type_defs.md#agentcollaboratorsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateAgentCollaboratorResponseTypeDef

```python
# AssociateAgentCollaboratorResponseTypeDef definition

class AssociateAgentCollaboratorResponseTypeDef(TypedDict):
    agentCollaborator: AgentCollaboratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentCollaboratorTypeDef](./type_defs.md#agentcollaboratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentCollaboratorResponseTypeDef

```python
# GetAgentCollaboratorResponseTypeDef definition

class GetAgentCollaboratorResponseTypeDef(TypedDict):
    agentCollaborator: AgentCollaboratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentCollaboratorTypeDef](./type_defs.md#agentcollaboratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentCollaboratorResponseTypeDef

```python
# UpdateAgentCollaboratorResponseTypeDef definition

class UpdateAgentCollaboratorResponseTypeDef(TypedDict):
    agentCollaborator: AgentCollaboratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentCollaboratorTypeDef](./type_defs.md#agentcollaboratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentsResponseTypeDef

```python
# ListAgentsResponseTypeDef definition

class ListAgentsResponseTypeDef(TypedDict):
    agentSummaries: List[AgentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentSummaryTypeDef](./type_defs.md#agentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAgentVersionsResponseTypeDef

```python
# ListAgentVersionsResponseTypeDef definition

class ListAgentVersionsResponseTypeDef(TypedDict):
    agentVersionSummaries: List[AgentVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AgentVersionSummaryTypeDef](./type_defs.md#agentversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ParsingConfigurationTypeDef

```python
# ParsingConfigurationTypeDef definition

class ParsingConfigurationTypeDef(TypedDict):
    parsingStrategy: ParsingStrategyType,  # (3)
    bedrockDataAutomationConfiguration: NotRequired[BedrockDataAutomationConfigurationTypeDef],  # (1)
    bedrockFoundationModelConfiguration: NotRequired[BedrockFoundationModelConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: BedrockDataAutomationConfigurationTypeDef](./type_defs.md#bedrockdataautomationconfigurationtypedef) 
2. See [:material-code-braces: BedrockFoundationModelConfigurationTypeDef](./type_defs.md#bedrockfoundationmodelconfigurationtypedef) 
3. See [:material-code-brackets: ParsingStrategyType](./literals.md#parsingstrategytype) 
## InlineContentTypeDef

```python
# InlineContentTypeDef definition

class InlineContentTypeDef(TypedDict):
    type: InlineContentTypeType,  # (3)
    byteContent: NotRequired[ByteContentDocTypeDef],  # (1)
    textContent: NotRequired[TextContentDocTypeDef],  # (2)
```

1. See [:material-code-braces: ByteContentDocTypeDef](./type_defs.md#bytecontentdoctypedef) 
2. See [:material-code-braces: TextContentDocTypeDef](./type_defs.md#textcontentdoctypedef) 
3. See [:material-code-brackets: InlineContentTypeType](./literals.md#inlinecontenttypetype) 
## ListFlowAliasesResponseTypeDef

```python
# ListFlowAliasesResponseTypeDef definition

class ListFlowAliasesResponseTypeDef(TypedDict):
    flowAliasSummaries: List[FlowAliasSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: FlowAliasSummaryTypeDef](./type_defs.md#flowaliassummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteKnowledgeBaseDocumentsRequestRequestTypeDef

```python
# DeleteKnowledgeBaseDocumentsRequestRequestTypeDef definition

class DeleteKnowledgeBaseDocumentsRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    documentIdentifiers: Sequence[DocumentIdentifierTypeDef],  # (1)
    knowledgeBaseId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: DocumentIdentifierTypeDef](./type_defs.md#documentidentifiertypedef) 
## GetKnowledgeBaseDocumentsRequestRequestTypeDef

```python
# GetKnowledgeBaseDocumentsRequestRequestTypeDef definition

class GetKnowledgeBaseDocumentsRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    documentIdentifiers: Sequence[DocumentIdentifierTypeDef],  # (1)
    knowledgeBaseId: str,
```

1. See [:material-code-braces: DocumentIdentifierTypeDef](./type_defs.md#documentidentifiertypedef) 
## KnowledgeBaseDocumentDetailTypeDef

```python
# KnowledgeBaseDocumentDetailTypeDef definition

class KnowledgeBaseDocumentDetailTypeDef(TypedDict):
    dataSourceId: str,
    identifier: DocumentIdentifierTypeDef,  # (1)
    knowledgeBaseId: str,
    status: DocumentStatusType,  # (2)
    statusReason: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: DocumentIdentifierTypeDef](./type_defs.md#documentidentifiertypedef) 
2. See [:material-code-brackets: DocumentStatusType](./literals.md#documentstatustype) 
## SupplementalDataStorageConfigurationOutputTypeDef

```python
# SupplementalDataStorageConfigurationOutputTypeDef definition

class SupplementalDataStorageConfigurationOutputTypeDef(TypedDict):
    storageLocations: List[SupplementalDataStorageLocationTypeDef],  # (1)
```

1. See [:material-code-braces: SupplementalDataStorageLocationTypeDef](./type_defs.md#supplementaldatastoragelocationtypedef) 
## SupplementalDataStorageConfigurationTypeDef

```python
# SupplementalDataStorageConfigurationTypeDef definition

class SupplementalDataStorageConfigurationTypeDef(TypedDict):
    storageLocations: Sequence[SupplementalDataStorageLocationTypeDef],  # (1)
```

1. See [:material-code-braces: SupplementalDataStorageLocationTypeDef](./type_defs.md#supplementaldatastoragelocationtypedef) 
## FlowConnectionTypeDef

```python
# FlowConnectionTypeDef definition

class FlowConnectionTypeDef(TypedDict):
    name: str,
    source: str,
    target: str,
    type: FlowConnectionTypeType,  # (2)
    configuration: NotRequired[FlowConnectionConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: FlowConnectionConfigurationTypeDef](./type_defs.md#flowconnectionconfigurationtypedef) 
2. See [:material-code-brackets: FlowConnectionTypeType](./literals.md#flowconnectiontypetype) 
## FlowValidationTypeDef

```python
# FlowValidationTypeDef definition

class FlowValidationTypeDef(TypedDict):
    message: str,
    severity: FlowValidationSeverityType,  # (2)
    details: NotRequired[FlowValidationDetailsTypeDef],  # (1)
    type: NotRequired[FlowValidationTypeType],  # (3)
```

1. See [:material-code-braces: FlowValidationDetailsTypeDef](./type_defs.md#flowvalidationdetailstypedef) 
2. See [:material-code-brackets: FlowValidationSeverityType](./literals.md#flowvalidationseveritytype) 
3. See [:material-code-brackets: FlowValidationTypeType](./literals.md#flowvalidationtypetype) 
## FunctionSchemaOutputTypeDef

```python
# FunctionSchemaOutputTypeDef definition

class FunctionSchemaOutputTypeDef(TypedDict):
    functions: NotRequired[List[FunctionOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: FunctionOutputTypeDef](./type_defs.md#functionoutputtypedef) 
## ChunkingConfigurationOutputTypeDef

```python
# ChunkingConfigurationOutputTypeDef definition

class ChunkingConfigurationOutputTypeDef(TypedDict):
    chunkingStrategy: ChunkingStrategyType,  # (1)
    fixedSizeChunkingConfiguration: NotRequired[FixedSizeChunkingConfigurationTypeDef],  # (2)
    hierarchicalChunkingConfiguration: NotRequired[HierarchicalChunkingConfigurationOutputTypeDef],  # (3)
    semanticChunkingConfiguration: NotRequired[SemanticChunkingConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: ChunkingStrategyType](./literals.md#chunkingstrategytype) 
2. See [:material-code-braces: FixedSizeChunkingConfigurationTypeDef](./type_defs.md#fixedsizechunkingconfigurationtypedef) 
3. See [:material-code-braces: HierarchicalChunkingConfigurationOutputTypeDef](./type_defs.md#hierarchicalchunkingconfigurationoutputtypedef) 
4. See [:material-code-braces: SemanticChunkingConfigurationTypeDef](./type_defs.md#semanticchunkingconfigurationtypedef) 
## PromptOverrideConfigurationOutputTypeDef

```python
# PromptOverrideConfigurationOutputTypeDef definition

class PromptOverrideConfigurationOutputTypeDef(TypedDict):
    promptConfigurations: List[PromptConfigurationOutputTypeDef],  # (1)
    overrideLambda: NotRequired[str],
```

1. See [:material-code-braces: PromptConfigurationOutputTypeDef](./type_defs.md#promptconfigurationoutputtypedef) 
## PromptConfigurationTypeDef

```python
# PromptConfigurationTypeDef definition

class PromptConfigurationTypeDef(TypedDict):
    basePromptTemplate: NotRequired[str],
    foundationModel: NotRequired[str],
    inferenceConfiguration: NotRequired[InferenceConfigurationUnionTypeDef],  # (1)
    parserMode: NotRequired[CreationModeType],  # (2)
    promptCreationMode: NotRequired[CreationModeType],  # (2)
    promptState: NotRequired[PromptStateType],  # (4)
    promptType: NotRequired[PromptTypeType],  # (5)
```

1. See [:material-code-braces: InferenceConfigurationTypeDef](./type_defs.md#inferenceconfigurationtypedef) [:material-code-braces: InferenceConfigurationOutputTypeDef](./type_defs.md#inferenceconfigurationoutputtypedef) 
2. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
3. See [:material-code-brackets: CreationModeType](./literals.md#creationmodetype) 
4. See [:material-code-brackets: PromptStateType](./literals.md#promptstatetype) 
5. See [:material-code-brackets: PromptTypeType](./literals.md#prompttypetype) 
## ListIngestionJobsResponseTypeDef

```python
# ListIngestionJobsResponseTypeDef definition

class ListIngestionJobsResponseTypeDef(TypedDict):
    ingestionJobSummaries: List[IngestionJobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: IngestionJobSummaryTypeDef](./type_defs.md#ingestionjobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIngestionJobResponseTypeDef

```python
# GetIngestionJobResponseTypeDef definition

class GetIngestionJobResponseTypeDef(TypedDict):
    ingestionJob: IngestionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartIngestionJobResponseTypeDef

```python
# StartIngestionJobResponseTypeDef definition

class StartIngestionJobResponseTypeDef(TypedDict):
    ingestionJob: IngestionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopIngestionJobResponseTypeDef

```python
# StopIngestionJobResponseTypeDef definition

class StopIngestionJobResponseTypeDef(TypedDict):
    ingestionJob: IngestionJobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: IngestionJobTypeDef](./type_defs.md#ingestionjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentMetadataTypeDef

```python
# DocumentMetadataTypeDef definition

class DocumentMetadataTypeDef(TypedDict):
    type: MetadataSourceTypeType,  # (3)
    inlineAttributes: NotRequired[Sequence[MetadataAttributeTypeDef]],  # (1)
    s3Location: NotRequired[CustomS3LocationTypeDef],  # (2)
```

1. See [:material-code-braces: MetadataAttributeTypeDef](./type_defs.md#metadataattributetypedef) 
2. See [:material-code-braces: CustomS3LocationTypeDef](./type_defs.md#customs3locationtypedef) 
3. See [:material-code-brackets: MetadataSourceTypeType](./literals.md#metadatasourcetypetype) 
## CrawlFilterConfigurationOutputTypeDef

```python
# CrawlFilterConfigurationOutputTypeDef definition

class CrawlFilterConfigurationOutputTypeDef(TypedDict):
    type: CrawlFilterConfigurationTypeType,  # (2)
    patternObjectFilter: NotRequired[PatternObjectFilterConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PatternObjectFilterConfigurationOutputTypeDef](./type_defs.md#patternobjectfilterconfigurationoutputtypedef) 
2. See [:material-code-brackets: CrawlFilterConfigurationTypeType](./literals.md#crawlfilterconfigurationtypetype) 
## PatternObjectFilterConfigurationTypeDef

```python
# PatternObjectFilterConfigurationTypeDef definition

class PatternObjectFilterConfigurationTypeDef(TypedDict):
    filters: Sequence[PatternObjectFilterUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PatternObjectFilterTypeDef](./type_defs.md#patternobjectfiltertypedef) [:material-code-braces: PatternObjectFilterOutputTypeDef](./type_defs.md#patternobjectfilteroutputtypedef) 
## PromptInferenceConfigurationTypeDef

```python
# PromptInferenceConfigurationTypeDef definition

class PromptInferenceConfigurationTypeDef(TypedDict):
    text: NotRequired[PromptModelInferenceConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PromptModelInferenceConfigurationTypeDef](./type_defs.md#promptmodelinferenceconfigurationtypedef) [:material-code-braces: PromptModelInferenceConfigurationOutputTypeDef](./type_defs.md#promptmodelinferenceconfigurationoutputtypedef) 
## QueryGenerationContextOutputTypeDef

```python
# QueryGenerationContextOutputTypeDef definition

class QueryGenerationContextOutputTypeDef(TypedDict):
    curatedQueries: NotRequired[List[CuratedQueryTypeDef]],  # (1)
    tables: NotRequired[List[QueryGenerationTableOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: CuratedQueryTypeDef](./type_defs.md#curatedquerytypedef) 
2. See [:material-code-braces: QueryGenerationTableOutputTypeDef](./type_defs.md#querygenerationtableoutputtypedef) 
## StorageConfigurationTypeDef

```python
# StorageConfigurationTypeDef definition

class StorageConfigurationTypeDef(TypedDict):
    type: KnowledgeBaseStorageTypeType,  # (6)
    mongoDbAtlasConfiguration: NotRequired[MongoDbAtlasConfigurationTypeDef],  # (1)
    opensearchServerlessConfiguration: NotRequired[OpenSearchServerlessConfigurationTypeDef],  # (2)
    pineconeConfiguration: NotRequired[PineconeConfigurationTypeDef],  # (3)
    rdsConfiguration: NotRequired[RdsConfigurationTypeDef],  # (4)
    redisEnterpriseCloudConfiguration: NotRequired[RedisEnterpriseCloudConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: MongoDbAtlasConfigurationTypeDef](./type_defs.md#mongodbatlasconfigurationtypedef) 
2. See [:material-code-braces: OpenSearchServerlessConfigurationTypeDef](./type_defs.md#opensearchserverlessconfigurationtypedef) 
3. See [:material-code-braces: PineconeConfigurationTypeDef](./type_defs.md#pineconeconfigurationtypedef) 
4. See [:material-code-braces: RdsConfigurationTypeDef](./type_defs.md#rdsconfigurationtypedef) 
5. See [:material-code-braces: RedisEnterpriseCloudConfigurationTypeDef](./type_defs.md#redisenterprisecloudconfigurationtypedef) 
6. See [:material-code-brackets: KnowledgeBaseStorageTypeType](./literals.md#knowledgebasestoragetypetype) 
## RedshiftQueryEngineStorageConfigurationTypeDef

```python
# RedshiftQueryEngineStorageConfigurationTypeDef definition

class RedshiftQueryEngineStorageConfigurationTypeDef(TypedDict):
    type: RedshiftQueryEngineStorageTypeType,  # (3)
    awsDataCatalogConfiguration: NotRequired[RedshiftQueryEngineAwsDataCatalogStorageConfigurationUnionTypeDef],  # (1)
    redshiftConfiguration: NotRequired[RedshiftQueryEngineRedshiftStorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftQueryEngineAwsDataCatalogStorageConfigurationTypeDef](./type_defs.md#redshiftqueryengineawsdatacatalogstorageconfigurationtypedef) [:material-code-braces: RedshiftQueryEngineAwsDataCatalogStorageConfigurationOutputTypeDef](./type_defs.md#redshiftqueryengineawsdatacatalogstorageconfigurationoutputtypedef) 
2. See [:material-code-braces: RedshiftQueryEngineRedshiftStorageConfigurationTypeDef](./type_defs.md#redshiftqueryengineredshiftstorageconfigurationtypedef) 
3. See [:material-code-brackets: RedshiftQueryEngineStorageTypeType](./literals.md#redshiftqueryenginestoragetypetype) 
## RedshiftQueryEngineConfigurationTypeDef

```python
# RedshiftQueryEngineConfigurationTypeDef definition

class RedshiftQueryEngineConfigurationTypeDef(TypedDict):
    type: RedshiftQueryEngineTypeType,  # (3)
    provisionedConfiguration: NotRequired[RedshiftProvisionedConfigurationTypeDef],  # (1)
    serverlessConfiguration: NotRequired[RedshiftServerlessConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftProvisionedConfigurationTypeDef](./type_defs.md#redshiftprovisionedconfigurationtypedef) 
2. See [:material-code-braces: RedshiftServerlessConfigurationTypeDef](./type_defs.md#redshiftserverlessconfigurationtypedef) 
3. See [:material-code-brackets: RedshiftQueryEngineTypeType](./literals.md#redshiftqueryenginetypetype) 
## RetrievalFlowNodeConfigurationTypeDef

```python
# RetrievalFlowNodeConfigurationTypeDef definition

class RetrievalFlowNodeConfigurationTypeDef(TypedDict):
    serviceConfiguration: RetrievalFlowNodeServiceConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: RetrievalFlowNodeServiceConfigurationTypeDef](./type_defs.md#retrievalflownodeserviceconfigurationtypedef) 
## WebSourceConfigurationOutputTypeDef

```python
# WebSourceConfigurationOutputTypeDef definition

class WebSourceConfigurationOutputTypeDef(TypedDict):
    urlConfiguration: UrlConfigurationOutputTypeDef,  # (1)
```

1. See [:material-code-braces: UrlConfigurationOutputTypeDef](./type_defs.md#urlconfigurationoutputtypedef) 
## StorageFlowNodeConfigurationTypeDef

```python
# StorageFlowNodeConfigurationTypeDef definition

class StorageFlowNodeConfigurationTypeDef(TypedDict):
    serviceConfiguration: StorageFlowNodeServiceConfigurationTypeDef,  # (1)
```

1. See [:material-code-braces: StorageFlowNodeServiceConfigurationTypeDef](./type_defs.md#storageflownodeserviceconfigurationtypedef) 
## ToolOutputTypeDef

```python
# ToolOutputTypeDef definition

class ToolOutputTypeDef(TypedDict):
    toolSpec: NotRequired[ToolSpecificationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ToolSpecificationOutputTypeDef](./type_defs.md#toolspecificationoutputtypedef) 
## ToolSpecificationTypeDef

```python
# ToolSpecificationTypeDef definition

class ToolSpecificationTypeDef(TypedDict):
    inputSchema: ToolInputSchemaUnionTypeDef,  # (1)
    name: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: ToolInputSchemaTypeDef](./type_defs.md#toolinputschematypedef) [:material-code-braces: ToolInputSchemaOutputTypeDef](./type_defs.md#toolinputschemaoutputtypedef) 
## TransformationTypeDef

```python
# TransformationTypeDef definition

class TransformationTypeDef(TypedDict):
    stepToApply: StepTypeType,  # (1)
    transformationFunction: TransformationFunctionTypeDef,  # (2)
```

1. See [:material-code-brackets: StepTypeType](./literals.md#steptypetype) 
2. See [:material-code-braces: TransformationFunctionTypeDef](./type_defs.md#transformationfunctiontypedef) 
## CreateAgentAliasResponseTypeDef

```python
# CreateAgentAliasResponseTypeDef definition

class CreateAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentAliasResponseTypeDef

```python
# GetAgentAliasResponseTypeDef definition

class GetAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentAliasResponseTypeDef

```python
# UpdateAgentAliasResponseTypeDef definition

class UpdateAgentAliasResponseTypeDef(TypedDict):
    agentAlias: AgentAliasTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentAliasTypeDef](./type_defs.md#agentaliastypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomContentTypeDef

```python
# CustomContentTypeDef definition

class CustomContentTypeDef(TypedDict):
    customDocumentIdentifier: CustomDocumentIdentifierTypeDef,  # (1)
    sourceType: CustomSourceTypeType,  # (4)
    inlineContent: NotRequired[InlineContentTypeDef],  # (2)
    s3Location: NotRequired[CustomS3LocationTypeDef],  # (3)
```

1. See [:material-code-braces: CustomDocumentIdentifierTypeDef](./type_defs.md#customdocumentidentifiertypedef) 
2. See [:material-code-braces: InlineContentTypeDef](./type_defs.md#inlinecontenttypedef) 
3. See [:material-code-braces: CustomS3LocationTypeDef](./type_defs.md#customs3locationtypedef) 
4. See [:material-code-brackets: CustomSourceTypeType](./literals.md#customsourcetypetype) 
## DeleteKnowledgeBaseDocumentsResponseTypeDef

```python
# DeleteKnowledgeBaseDocumentsResponseTypeDef definition

class DeleteKnowledgeBaseDocumentsResponseTypeDef(TypedDict):
    documentDetails: List[KnowledgeBaseDocumentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseDocumentDetailTypeDef](./type_defs.md#knowledgebasedocumentdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKnowledgeBaseDocumentsResponseTypeDef

```python
# GetKnowledgeBaseDocumentsResponseTypeDef definition

class GetKnowledgeBaseDocumentsResponseTypeDef(TypedDict):
    documentDetails: List[KnowledgeBaseDocumentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseDocumentDetailTypeDef](./type_defs.md#knowledgebasedocumentdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IngestKnowledgeBaseDocumentsResponseTypeDef

```python
# IngestKnowledgeBaseDocumentsResponseTypeDef definition

class IngestKnowledgeBaseDocumentsResponseTypeDef(TypedDict):
    documentDetails: List[KnowledgeBaseDocumentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseDocumentDetailTypeDef](./type_defs.md#knowledgebasedocumentdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListKnowledgeBaseDocumentsResponseTypeDef

```python
# ListKnowledgeBaseDocumentsResponseTypeDef definition

class ListKnowledgeBaseDocumentsResponseTypeDef(TypedDict):
    documentDetails: List[KnowledgeBaseDocumentDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: KnowledgeBaseDocumentDetailTypeDef](./type_defs.md#knowledgebasedocumentdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## VectorKnowledgeBaseConfigurationOutputTypeDef

```python
# VectorKnowledgeBaseConfigurationOutputTypeDef definition

class VectorKnowledgeBaseConfigurationOutputTypeDef(TypedDict):
    embeddingModelArn: str,
    embeddingModelConfiguration: NotRequired[EmbeddingModelConfigurationTypeDef],  # (1)
    supplementalDataStorageConfiguration: NotRequired[SupplementalDataStorageConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: EmbeddingModelConfigurationTypeDef](./type_defs.md#embeddingmodelconfigurationtypedef) 
2. See [:material-code-braces: SupplementalDataStorageConfigurationOutputTypeDef](./type_defs.md#supplementaldatastorageconfigurationoutputtypedef) 
## ValidateFlowDefinitionResponseTypeDef

```python
# ValidateFlowDefinitionResponseTypeDef definition

class ValidateFlowDefinitionResponseTypeDef(TypedDict):
    validations: List[FlowValidationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FlowValidationTypeDef](./type_defs.md#flowvalidationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AgentActionGroupTypeDef

```python
# AgentActionGroupTypeDef definition

class AgentActionGroupTypeDef(TypedDict):
    actionGroupId: str,
    actionGroupName: str,
    actionGroupState: ActionGroupStateType,  # (2)
    agentId: str,
    agentVersion: str,
    createdAt: datetime,
    updatedAt: datetime,
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (1)
    apiSchema: NotRequired[APISchemaTypeDef],  # (3)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    functionSchema: NotRequired[FunctionSchemaOutputTypeDef],  # (4)
    parentActionSignature: NotRequired[ActionGroupSignatureType],  # (5)
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
2. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
4. See [:material-code-braces: FunctionSchemaOutputTypeDef](./type_defs.md#functionschemaoutputtypedef) 
5. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
## FunctionSchemaTypeDef

```python
# FunctionSchemaTypeDef definition

class FunctionSchemaTypeDef(TypedDict):
    functions: NotRequired[Sequence[FunctionUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: FunctionTypeDef](./type_defs.md#functiontypedef) [:material-code-braces: FunctionOutputTypeDef](./type_defs.md#functionoutputtypedef) 
## ChunkingConfigurationTypeDef

```python
# ChunkingConfigurationTypeDef definition

class ChunkingConfigurationTypeDef(TypedDict):
    chunkingStrategy: ChunkingStrategyType,  # (1)
    fixedSizeChunkingConfiguration: NotRequired[FixedSizeChunkingConfigurationTypeDef],  # (2)
    hierarchicalChunkingConfiguration: NotRequired[HierarchicalChunkingConfigurationUnionTypeDef],  # (3)
    semanticChunkingConfiguration: NotRequired[SemanticChunkingConfigurationTypeDef],  # (4)
```

1. See [:material-code-brackets: ChunkingStrategyType](./literals.md#chunkingstrategytype) 
2. See [:material-code-braces: FixedSizeChunkingConfigurationTypeDef](./type_defs.md#fixedsizechunkingconfigurationtypedef) 
3. See [:material-code-braces: HierarchicalChunkingConfigurationTypeDef](./type_defs.md#hierarchicalchunkingconfigurationtypedef) [:material-code-braces: HierarchicalChunkingConfigurationOutputTypeDef](./type_defs.md#hierarchicalchunkingconfigurationoutputtypedef) 
4. See [:material-code-braces: SemanticChunkingConfigurationTypeDef](./type_defs.md#semanticchunkingconfigurationtypedef) 
## AgentTypeDef

```python
# AgentTypeDef definition

class AgentTypeDef(TypedDict):
    agentArn: str,
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    agentStatus: AgentStatusType,  # (2)
    agentVersion: str,
    createdAt: datetime,
    idleSessionTTLInSeconds: int,
    updatedAt: datetime,
    agentCollaboration: NotRequired[AgentCollaborationType],  # (1)
    clientToken: NotRequired[str],
    customOrchestration: NotRequired[CustomOrchestrationTypeDef],  # (3)
    customerEncryptionKeyArn: NotRequired[str],
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    foundationModel: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (4)
    instruction: NotRequired[str],
    memoryConfiguration: NotRequired[MemoryConfigurationOutputTypeDef],  # (5)
    orchestrationType: NotRequired[OrchestrationTypeType],  # (6)
    preparedAt: NotRequired[datetime],
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationOutputTypeDef],  # (7)
    recommendedActions: NotRequired[List[str]],
```

1. See [:material-code-brackets: AgentCollaborationType](./literals.md#agentcollaborationtype) 
2. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
3. See [:material-code-braces: CustomOrchestrationTypeDef](./type_defs.md#customorchestrationtypedef) 
4. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
5. See [:material-code-braces: MemoryConfigurationOutputTypeDef](./type_defs.md#memoryconfigurationoutputtypedef) 
6. See [:material-code-brackets: OrchestrationTypeType](./literals.md#orchestrationtypetype) 
7. See [:material-code-braces: PromptOverrideConfigurationOutputTypeDef](./type_defs.md#promptoverrideconfigurationoutputtypedef) 
## AgentVersionTypeDef

```python
# AgentVersionTypeDef definition

class AgentVersionTypeDef(TypedDict):
    agentArn: str,
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    agentStatus: AgentStatusType,  # (2)
    createdAt: datetime,
    idleSessionTTLInSeconds: int,
    updatedAt: datetime,
    version: str,
    agentCollaboration: NotRequired[AgentCollaborationType],  # (1)
    customerEncryptionKeyArn: NotRequired[str],
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    foundationModel: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (3)
    instruction: NotRequired[str],
    memoryConfiguration: NotRequired[MemoryConfigurationOutputTypeDef],  # (4)
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationOutputTypeDef],  # (5)
    recommendedActions: NotRequired[List[str]],
```

1. See [:material-code-brackets: AgentCollaborationType](./literals.md#agentcollaborationtype) 
2. See [:material-code-brackets: AgentStatusType](./literals.md#agentstatustype) 
3. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
4. See [:material-code-braces: MemoryConfigurationOutputTypeDef](./type_defs.md#memoryconfigurationoutputtypedef) 
5. See [:material-code-braces: PromptOverrideConfigurationOutputTypeDef](./type_defs.md#promptoverrideconfigurationoutputtypedef) 
## ConfluenceCrawlerConfigurationOutputTypeDef

```python
# ConfluenceCrawlerConfigurationOutputTypeDef definition

class ConfluenceCrawlerConfigurationOutputTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef) 
## SalesforceCrawlerConfigurationOutputTypeDef

```python
# SalesforceCrawlerConfigurationOutputTypeDef definition

class SalesforceCrawlerConfigurationOutputTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef) 
## SharePointCrawlerConfigurationOutputTypeDef

```python
# SharePointCrawlerConfigurationOutputTypeDef definition

class SharePointCrawlerConfigurationOutputTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef) 
## QueryGenerationConfigurationOutputTypeDef

```python
# QueryGenerationConfigurationOutputTypeDef definition

class QueryGenerationConfigurationOutputTypeDef(TypedDict):
    executionTimeoutSeconds: NotRequired[int],
    generationContext: NotRequired[QueryGenerationContextOutputTypeDef],  # (1)
```

1. See [:material-code-braces: QueryGenerationContextOutputTypeDef](./type_defs.md#querygenerationcontextoutputtypedef) 
## QueryGenerationContextTypeDef

```python
# QueryGenerationContextTypeDef definition

class QueryGenerationContextTypeDef(TypedDict):
    curatedQueries: NotRequired[Sequence[CuratedQueryTypeDef]],  # (1)
    tables: NotRequired[Sequence[QueryGenerationTableUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: CuratedQueryTypeDef](./type_defs.md#curatedquerytypedef) 
2. See [:material-code-braces: QueryGenerationTableTypeDef](./type_defs.md#querygenerationtabletypedef) [:material-code-braces: QueryGenerationTableOutputTypeDef](./type_defs.md#querygenerationtableoutputtypedef) 
## WebDataSourceConfigurationOutputTypeDef

```python
# WebDataSourceConfigurationOutputTypeDef definition

class WebDataSourceConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: WebSourceConfigurationOutputTypeDef,  # (2)
    crawlerConfiguration: NotRequired[WebCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef) 
2. See [:material-code-braces: WebSourceConfigurationOutputTypeDef](./type_defs.md#websourceconfigurationoutputtypedef) 
## WebSourceConfigurationTypeDef

```python
# WebSourceConfigurationTypeDef definition

class WebSourceConfigurationTypeDef(TypedDict):
    urlConfiguration: UrlConfigurationUnionTypeDef,  # (1)
```

1. See [:material-code-braces: UrlConfigurationTypeDef](./type_defs.md#urlconfigurationtypedef) [:material-code-braces: UrlConfigurationOutputTypeDef](./type_defs.md#urlconfigurationoutputtypedef) 
## ToolConfigurationOutputTypeDef

```python
# ToolConfigurationOutputTypeDef definition

class ToolConfigurationOutputTypeDef(TypedDict):
    tools: List[ToolOutputTypeDef],  # (2)
    toolChoice: NotRequired[ToolChoiceOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ToolChoiceOutputTypeDef](./type_defs.md#toolchoiceoutputtypedef) 
2. See [:material-code-braces: ToolOutputTypeDef](./type_defs.md#tooloutputtypedef) 
## CustomTransformationConfigurationOutputTypeDef

```python
# CustomTransformationConfigurationOutputTypeDef definition

class CustomTransformationConfigurationOutputTypeDef(TypedDict):
    intermediateStorage: IntermediateStorageTypeDef,  # (1)
    transformations: List[TransformationTypeDef],  # (2)
```

1. See [:material-code-braces: IntermediateStorageTypeDef](./type_defs.md#intermediatestoragetypedef) 
2. See [:material-code-braces: TransformationTypeDef](./type_defs.md#transformationtypedef) 
## CustomTransformationConfigurationTypeDef

```python
# CustomTransformationConfigurationTypeDef definition

class CustomTransformationConfigurationTypeDef(TypedDict):
    intermediateStorage: IntermediateStorageTypeDef,  # (1)
    transformations: Sequence[TransformationTypeDef],  # (2)
```

1. See [:material-code-braces: IntermediateStorageTypeDef](./type_defs.md#intermediatestoragetypedef) 
2. See [:material-code-braces: TransformationTypeDef](./type_defs.md#transformationtypedef) 
## DocumentContentTypeDef

```python
# DocumentContentTypeDef definition

class DocumentContentTypeDef(TypedDict):
    dataSourceType: ContentDataSourceTypeType,  # (2)
    custom: NotRequired[CustomContentTypeDef],  # (1)
    s3: NotRequired[S3ContentTypeDef],  # (3)
```

1. See [:material-code-braces: CustomContentTypeDef](./type_defs.md#customcontenttypedef) 
2. See [:material-code-brackets: ContentDataSourceTypeType](./literals.md#contentdatasourcetypetype) 
3. See [:material-code-braces: S3ContentTypeDef](./type_defs.md#s3contenttypedef) 
## VectorKnowledgeBaseConfigurationTypeDef

```python
# VectorKnowledgeBaseConfigurationTypeDef definition

class VectorKnowledgeBaseConfigurationTypeDef(TypedDict):
    embeddingModelArn: str,
    embeddingModelConfiguration: NotRequired[EmbeddingModelConfigurationTypeDef],  # (1)
    supplementalDataStorageConfiguration: NotRequired[SupplementalDataStorageConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: EmbeddingModelConfigurationTypeDef](./type_defs.md#embeddingmodelconfigurationtypedef) 
2. See [:material-code-braces: SupplementalDataStorageConfigurationTypeDef](./type_defs.md#supplementaldatastorageconfigurationtypedef) [:material-code-braces: SupplementalDataStorageConfigurationOutputTypeDef](./type_defs.md#supplementaldatastorageconfigurationoutputtypedef) 
## CreateAgentActionGroupResponseTypeDef

```python
# CreateAgentActionGroupResponseTypeDef definition

class CreateAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentActionGroupResponseTypeDef

```python
# GetAgentActionGroupResponseTypeDef definition

class GetAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentActionGroupResponseTypeDef

```python
# UpdateAgentActionGroupResponseTypeDef definition

class UpdateAgentActionGroupResponseTypeDef(TypedDict):
    agentActionGroup: AgentActionGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentActionGroupTypeDef](./type_defs.md#agentactiongrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAgentActionGroupRequestRequestTypeDef

```python
# CreateAgentActionGroupRequestRequestTypeDef definition

class CreateAgentActionGroupRequestRequestTypeDef(TypedDict):
    actionGroupName: str,
    agentId: str,
    agentVersion: str,
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (1)
    actionGroupState: NotRequired[ActionGroupStateType],  # (2)
    apiSchema: NotRequired[APISchemaTypeDef],  # (3)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    functionSchema: NotRequired[FunctionSchemaTypeDef],  # (4)
    parentActionGroupSignature: NotRequired[ActionGroupSignatureType],  # (5)
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
2. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
4. See [:material-code-braces: FunctionSchemaTypeDef](./type_defs.md#functionschematypedef) 
5. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
## UpdateAgentActionGroupRequestRequestTypeDef

```python
# UpdateAgentActionGroupRequestRequestTypeDef definition

class UpdateAgentActionGroupRequestRequestTypeDef(TypedDict):
    actionGroupId: str,
    actionGroupName: str,
    agentId: str,
    agentVersion: str,
    actionGroupExecutor: NotRequired[ActionGroupExecutorTypeDef],  # (1)
    actionGroupState: NotRequired[ActionGroupStateType],  # (2)
    apiSchema: NotRequired[APISchemaTypeDef],  # (3)
    description: NotRequired[str],
    functionSchema: NotRequired[FunctionSchemaTypeDef],  # (4)
    parentActionGroupSignature: NotRequired[ActionGroupSignatureType],  # (5)
```

1. See [:material-code-braces: ActionGroupExecutorTypeDef](./type_defs.md#actiongroupexecutortypedef) 
2. See [:material-code-brackets: ActionGroupStateType](./literals.md#actiongroupstatetype) 
3. See [:material-code-braces: APISchemaTypeDef](./type_defs.md#apischematypedef) 
4. See [:material-code-braces: FunctionSchemaTypeDef](./type_defs.md#functionschematypedef) 
5. See [:material-code-brackets: ActionGroupSignatureType](./literals.md#actiongroupsignaturetype) 
## CreateAgentResponseTypeDef

```python
# CreateAgentResponseTypeDef definition

class CreateAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentResponseTypeDef

```python
# GetAgentResponseTypeDef definition

class GetAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAgentResponseTypeDef

```python
# UpdateAgentResponseTypeDef definition

class UpdateAgentResponseTypeDef(TypedDict):
    agent: AgentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentTypeDef](./type_defs.md#agenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAgentVersionResponseTypeDef

```python
# GetAgentVersionResponseTypeDef definition

class GetAgentVersionResponseTypeDef(TypedDict):
    agentVersion: AgentVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AgentVersionTypeDef](./type_defs.md#agentversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromptOverrideConfigurationTypeDef

```python
# PromptOverrideConfigurationTypeDef definition

class PromptOverrideConfigurationTypeDef(TypedDict):
    promptConfigurations: Sequence[PromptConfigurationUnionTypeDef],  # (1)
    overrideLambda: NotRequired[str],
```

1. See [:material-code-braces: PromptConfigurationTypeDef](./type_defs.md#promptconfigurationtypedef) [:material-code-braces: PromptConfigurationOutputTypeDef](./type_defs.md#promptconfigurationoutputtypedef) 
## ConfluenceDataSourceConfigurationOutputTypeDef

```python
# ConfluenceDataSourceConfigurationOutputTypeDef definition

class ConfluenceDataSourceConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: ConfluenceSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[ConfluenceCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ConfluenceCrawlerConfigurationOutputTypeDef](./type_defs.md#confluencecrawlerconfigurationoutputtypedef) 
2. See [:material-code-braces: ConfluenceSourceConfigurationTypeDef](./type_defs.md#confluencesourceconfigurationtypedef) 
## SalesforceDataSourceConfigurationOutputTypeDef

```python
# SalesforceDataSourceConfigurationOutputTypeDef definition

class SalesforceDataSourceConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: SalesforceSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[SalesforceCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SalesforceCrawlerConfigurationOutputTypeDef](./type_defs.md#salesforcecrawlerconfigurationoutputtypedef) 
2. See [:material-code-braces: SalesforceSourceConfigurationTypeDef](./type_defs.md#salesforcesourceconfigurationtypedef) 
## SharePointDataSourceConfigurationOutputTypeDef

```python
# SharePointDataSourceConfigurationOutputTypeDef definition

class SharePointDataSourceConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: SharePointSourceConfigurationOutputTypeDef,  # (2)
    crawlerConfiguration: NotRequired[SharePointCrawlerConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SharePointCrawlerConfigurationOutputTypeDef](./type_defs.md#sharepointcrawlerconfigurationoutputtypedef) 
2. See [:material-code-braces: SharePointSourceConfigurationOutputTypeDef](./type_defs.md#sharepointsourceconfigurationoutputtypedef) 
## CrawlFilterConfigurationTypeDef

```python
# CrawlFilterConfigurationTypeDef definition

class CrawlFilterConfigurationTypeDef(TypedDict):
    type: CrawlFilterConfigurationTypeType,  # (2)
    patternObjectFilter: NotRequired[PatternObjectFilterConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PatternObjectFilterConfigurationTypeDef](./type_defs.md#patternobjectfilterconfigurationtypedef) [:material-code-braces: PatternObjectFilterConfigurationOutputTypeDef](./type_defs.md#patternobjectfilterconfigurationoutputtypedef) 
2. See [:material-code-brackets: CrawlFilterConfigurationTypeType](./literals.md#crawlfilterconfigurationtypetype) 
## RedshiftConfigurationOutputTypeDef

```python
# RedshiftConfigurationOutputTypeDef definition

class RedshiftConfigurationOutputTypeDef(TypedDict):
    queryEngineConfiguration: RedshiftQueryEngineConfigurationTypeDef,  # (1)
    storageConfigurations: List[RedshiftQueryEngineStorageConfigurationOutputTypeDef],  # (3)
    queryGenerationConfiguration: NotRequired[QueryGenerationConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftQueryEngineConfigurationTypeDef](./type_defs.md#redshiftqueryengineconfigurationtypedef) 
2. See [:material-code-braces: QueryGenerationConfigurationOutputTypeDef](./type_defs.md#querygenerationconfigurationoutputtypedef) 
3. See [:material-code-braces: RedshiftQueryEngineStorageConfigurationOutputTypeDef](./type_defs.md#redshiftqueryenginestorageconfigurationoutputtypedef) 
## ChatPromptTemplateConfigurationOutputTypeDef

```python
# ChatPromptTemplateConfigurationOutputTypeDef definition

class ChatPromptTemplateConfigurationOutputTypeDef(TypedDict):
    messages: List[MessageOutputTypeDef],  # (2)
    inputVariables: NotRequired[List[PromptInputVariableTypeDef]],  # (1)
    system: NotRequired[List[SystemContentBlockTypeDef]],  # (3)
    toolConfiguration: NotRequired[ToolConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-braces: PromptInputVariableTypeDef](./type_defs.md#promptinputvariabletypedef) 
2. See [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
3. See [:material-code-braces: SystemContentBlockTypeDef](./type_defs.md#systemcontentblocktypedef) 
4. See [:material-code-braces: ToolConfigurationOutputTypeDef](./type_defs.md#toolconfigurationoutputtypedef) 
## ToolTypeDef

```python
# ToolTypeDef definition

class ToolTypeDef(TypedDict):
    toolSpec: NotRequired[ToolSpecificationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ToolSpecificationTypeDef](./type_defs.md#toolspecificationtypedef) [:material-code-braces: ToolSpecificationOutputTypeDef](./type_defs.md#toolspecificationoutputtypedef) 
## VectorIngestionConfigurationOutputTypeDef

```python
# VectorIngestionConfigurationOutputTypeDef definition

class VectorIngestionConfigurationOutputTypeDef(TypedDict):
    chunkingConfiguration: NotRequired[ChunkingConfigurationOutputTypeDef],  # (1)
    customTransformationConfiguration: NotRequired[CustomTransformationConfigurationOutputTypeDef],  # (2)
    parsingConfiguration: NotRequired[ParsingConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ChunkingConfigurationOutputTypeDef](./type_defs.md#chunkingconfigurationoutputtypedef) 
2. See [:material-code-braces: CustomTransformationConfigurationOutputTypeDef](./type_defs.md#customtransformationconfigurationoutputtypedef) 
3. See [:material-code-braces: ParsingConfigurationTypeDef](./type_defs.md#parsingconfigurationtypedef) 
## KnowledgeBaseDocumentTypeDef

```python
# KnowledgeBaseDocumentTypeDef definition

class KnowledgeBaseDocumentTypeDef(TypedDict):
    content: DocumentContentTypeDef,  # (1)
    metadata: NotRequired[DocumentMetadataTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentContentTypeDef](./type_defs.md#documentcontenttypedef) 
2. See [:material-code-braces: DocumentMetadataTypeDef](./type_defs.md#documentmetadatatypedef) 
## CreateAgentRequestRequestTypeDef

```python
# CreateAgentRequestRequestTypeDef definition

class CreateAgentRequestRequestTypeDef(TypedDict):
    agentName: str,
    agentCollaboration: NotRequired[AgentCollaborationType],  # (1)
    agentResourceRoleArn: NotRequired[str],
    clientToken: NotRequired[str],
    customOrchestration: NotRequired[CustomOrchestrationTypeDef],  # (2)
    customerEncryptionKeyArn: NotRequired[str],
    description: NotRequired[str],
    foundationModel: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (3)
    idleSessionTTLInSeconds: NotRequired[int],
    instruction: NotRequired[str],
    memoryConfiguration: NotRequired[MemoryConfigurationTypeDef],  # (4)
    orchestrationType: NotRequired[OrchestrationTypeType],  # (5)
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationTypeDef],  # (6)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: AgentCollaborationType](./literals.md#agentcollaborationtype) 
2. See [:material-code-braces: CustomOrchestrationTypeDef](./type_defs.md#customorchestrationtypedef) 
3. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
4. See [:material-code-braces: MemoryConfigurationTypeDef](./type_defs.md#memoryconfigurationtypedef) 
5. See [:material-code-brackets: OrchestrationTypeType](./literals.md#orchestrationtypetype) 
6. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
## UpdateAgentRequestRequestTypeDef

```python
# UpdateAgentRequestRequestTypeDef definition

class UpdateAgentRequestRequestTypeDef(TypedDict):
    agentId: str,
    agentName: str,
    agentResourceRoleArn: str,
    foundationModel: str,
    agentCollaboration: NotRequired[AgentCollaborationType],  # (1)
    customOrchestration: NotRequired[CustomOrchestrationTypeDef],  # (2)
    customerEncryptionKeyArn: NotRequired[str],
    description: NotRequired[str],
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (3)
    idleSessionTTLInSeconds: NotRequired[int],
    instruction: NotRequired[str],
    memoryConfiguration: NotRequired[MemoryConfigurationTypeDef],  # (4)
    orchestrationType: NotRequired[OrchestrationTypeType],  # (5)
    promptOverrideConfiguration: NotRequired[PromptOverrideConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: AgentCollaborationType](./literals.md#agentcollaborationtype) 
2. See [:material-code-braces: CustomOrchestrationTypeDef](./type_defs.md#customorchestrationtypedef) 
3. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
4. See [:material-code-braces: MemoryConfigurationTypeDef](./type_defs.md#memoryconfigurationtypedef) 
5. See [:material-code-brackets: OrchestrationTypeType](./literals.md#orchestrationtypetype) 
6. See [:material-code-braces: PromptOverrideConfigurationTypeDef](./type_defs.md#promptoverrideconfigurationtypedef) 
## DataSourceConfigurationOutputTypeDef

```python
# DataSourceConfigurationOutputTypeDef definition

class DataSourceConfigurationOutputTypeDef(TypedDict):
    type: DataSourceTypeType,  # (5)
    confluenceConfiguration: NotRequired[ConfluenceDataSourceConfigurationOutputTypeDef],  # (1)
    s3Configuration: NotRequired[S3DataSourceConfigurationOutputTypeDef],  # (2)
    salesforceConfiguration: NotRequired[SalesforceDataSourceConfigurationOutputTypeDef],  # (3)
    sharePointConfiguration: NotRequired[SharePointDataSourceConfigurationOutputTypeDef],  # (4)
    webConfiguration: NotRequired[WebDataSourceConfigurationOutputTypeDef],  # (6)
```

1. See [:material-code-braces: ConfluenceDataSourceConfigurationOutputTypeDef](./type_defs.md#confluencedatasourceconfigurationoutputtypedef) 
2. See [:material-code-braces: S3DataSourceConfigurationOutputTypeDef](./type_defs.md#s3datasourceconfigurationoutputtypedef) 
3. See [:material-code-braces: SalesforceDataSourceConfigurationOutputTypeDef](./type_defs.md#salesforcedatasourceconfigurationoutputtypedef) 
4. See [:material-code-braces: SharePointDataSourceConfigurationOutputTypeDef](./type_defs.md#sharepointdatasourceconfigurationoutputtypedef) 
5. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
6. See [:material-code-braces: WebDataSourceConfigurationOutputTypeDef](./type_defs.md#webdatasourceconfigurationoutputtypedef) 
## SqlKnowledgeBaseConfigurationOutputTypeDef

```python
# SqlKnowledgeBaseConfigurationOutputTypeDef definition

class SqlKnowledgeBaseConfigurationOutputTypeDef(TypedDict):
    type: QueryEngineTypeType,  # (2)
    redshiftConfiguration: NotRequired[RedshiftConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: RedshiftConfigurationOutputTypeDef](./type_defs.md#redshiftconfigurationoutputtypedef) 
2. See [:material-code-brackets: QueryEngineTypeType](./literals.md#queryenginetypetype) 
## QueryGenerationConfigurationTypeDef

```python
# QueryGenerationConfigurationTypeDef definition

class QueryGenerationConfigurationTypeDef(TypedDict):
    executionTimeoutSeconds: NotRequired[int],
    generationContext: NotRequired[QueryGenerationContextUnionTypeDef],  # (1)
```

1. See [:material-code-braces: QueryGenerationContextTypeDef](./type_defs.md#querygenerationcontexttypedef) [:material-code-braces: QueryGenerationContextOutputTypeDef](./type_defs.md#querygenerationcontextoutputtypedef) 
## WebDataSourceConfigurationTypeDef

```python
# WebDataSourceConfigurationTypeDef definition

class WebDataSourceConfigurationTypeDef(TypedDict):
    sourceConfiguration: WebSourceConfigurationUnionTypeDef,  # (2)
    crawlerConfiguration: NotRequired[WebCrawlerConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: WebCrawlerConfigurationTypeDef](./type_defs.md#webcrawlerconfigurationtypedef) [:material-code-braces: WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef) 
2. See [:material-code-braces: WebSourceConfigurationTypeDef](./type_defs.md#websourceconfigurationtypedef) [:material-code-braces: WebSourceConfigurationOutputTypeDef](./type_defs.md#websourceconfigurationoutputtypedef) 
## PromptTemplateConfigurationOutputTypeDef

```python
# PromptTemplateConfigurationOutputTypeDef definition

class PromptTemplateConfigurationOutputTypeDef(TypedDict):
    chat: NotRequired[ChatPromptTemplateConfigurationOutputTypeDef],  # (1)
    text: NotRequired[TextPromptTemplateConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ChatPromptTemplateConfigurationOutputTypeDef](./type_defs.md#chatprompttemplateconfigurationoutputtypedef) 
2. See [:material-code-braces: TextPromptTemplateConfigurationOutputTypeDef](./type_defs.md#textprompttemplateconfigurationoutputtypedef) 
## VectorIngestionConfigurationTypeDef

```python
# VectorIngestionConfigurationTypeDef definition

class VectorIngestionConfigurationTypeDef(TypedDict):
    chunkingConfiguration: NotRequired[ChunkingConfigurationUnionTypeDef],  # (1)
    customTransformationConfiguration: NotRequired[CustomTransformationConfigurationUnionTypeDef],  # (2)
    parsingConfiguration: NotRequired[ParsingConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: ChunkingConfigurationTypeDef](./type_defs.md#chunkingconfigurationtypedef) [:material-code-braces: ChunkingConfigurationOutputTypeDef](./type_defs.md#chunkingconfigurationoutputtypedef) 
2. See [:material-code-braces: CustomTransformationConfigurationTypeDef](./type_defs.md#customtransformationconfigurationtypedef) [:material-code-braces: CustomTransformationConfigurationOutputTypeDef](./type_defs.md#customtransformationconfigurationoutputtypedef) 
3. See [:material-code-braces: ParsingConfigurationTypeDef](./type_defs.md#parsingconfigurationtypedef) 
## IngestKnowledgeBaseDocumentsRequestRequestTypeDef

```python
# IngestKnowledgeBaseDocumentsRequestRequestTypeDef definition

class IngestKnowledgeBaseDocumentsRequestRequestTypeDef(TypedDict):
    dataSourceId: str,
    documents: Sequence[KnowledgeBaseDocumentTypeDef],  # (1)
    knowledgeBaseId: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: KnowledgeBaseDocumentTypeDef](./type_defs.md#knowledgebasedocumenttypedef) 
## DataSourceTypeDef

```python
# DataSourceTypeDef definition

class DataSourceTypeDef(TypedDict):
    createdAt: datetime,
    dataSourceConfiguration: DataSourceConfigurationOutputTypeDef,  # (2)
    dataSourceId: str,
    knowledgeBaseId: str,
    name: str,
    status: DataSourceStatusType,  # (4)
    updatedAt: datetime,
    dataDeletionPolicy: NotRequired[DataDeletionPolicyType],  # (1)
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationOutputTypeDef],  # (5)
```

1. See [:material-code-brackets: DataDeletionPolicyType](./literals.md#datadeletionpolicytype) 
2. See [:material-code-braces: DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
5. See [:material-code-braces: VectorIngestionConfigurationOutputTypeDef](./type_defs.md#vectoringestionconfigurationoutputtypedef) 
## ConfluenceCrawlerConfigurationTypeDef

```python
# ConfluenceCrawlerConfigurationTypeDef definition

class ConfluenceCrawlerConfigurationTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationTypeDef](./type_defs.md#crawlfilterconfigurationtypedef) [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef) 
## SalesforceCrawlerConfigurationTypeDef

```python
# SalesforceCrawlerConfigurationTypeDef definition

class SalesforceCrawlerConfigurationTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationTypeDef](./type_defs.md#crawlfilterconfigurationtypedef) [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef) 
## SharePointCrawlerConfigurationTypeDef

```python
# SharePointCrawlerConfigurationTypeDef definition

class SharePointCrawlerConfigurationTypeDef(TypedDict):
    filterConfiguration: NotRequired[CrawlFilterConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: CrawlFilterConfigurationTypeDef](./type_defs.md#crawlfilterconfigurationtypedef) [:material-code-braces: CrawlFilterConfigurationOutputTypeDef](./type_defs.md#crawlfilterconfigurationoutputtypedef) 
## KnowledgeBaseConfigurationOutputTypeDef

```python
# KnowledgeBaseConfigurationOutputTypeDef definition

class KnowledgeBaseConfigurationOutputTypeDef(TypedDict):
    type: KnowledgeBaseTypeType,  # (3)
    kendraKnowledgeBaseConfiguration: NotRequired[KendraKnowledgeBaseConfigurationTypeDef],  # (1)
    sqlKnowledgeBaseConfiguration: NotRequired[SqlKnowledgeBaseConfigurationOutputTypeDef],  # (2)
    vectorKnowledgeBaseConfiguration: NotRequired[VectorKnowledgeBaseConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-braces: KendraKnowledgeBaseConfigurationTypeDef](./type_defs.md#kendraknowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: SqlKnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#sqlknowledgebaseconfigurationoutputtypedef) 
3. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype) 
4. See [:material-code-braces: VectorKnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#vectorknowledgebaseconfigurationoutputtypedef) 
## PromptFlowNodeInlineConfigurationOutputTypeDef

```python
# PromptFlowNodeInlineConfigurationOutputTypeDef definition

class PromptFlowNodeInlineConfigurationOutputTypeDef(TypedDict):
    modelId: str,
    templateConfiguration: PromptTemplateConfigurationOutputTypeDef,  # (2)
    templateType: PromptTemplateTypeType,  # (3)
    additionalModelRequestFields: NotRequired[Dict[str, Any]],
    inferenceConfiguration: NotRequired[PromptInferenceConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef) 
2. See [:material-code-braces: PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef) 
3. See [:material-code-brackets: PromptTemplateTypeType](./literals.md#prompttemplatetypetype) 
## PromptVariantOutputTypeDef

```python
# PromptVariantOutputTypeDef definition

class PromptVariantOutputTypeDef(TypedDict):
    name: str,
    templateConfiguration: PromptTemplateConfigurationOutputTypeDef,  # (4)
    templateType: PromptTemplateTypeType,  # (5)
    additionalModelRequestFields: NotRequired[Dict[str, Any]],
    genAiResource: NotRequired[PromptGenAiResourceTypeDef],  # (1)
    inferenceConfiguration: NotRequired[PromptInferenceConfigurationOutputTypeDef],  # (2)
    metadata: NotRequired[List[PromptMetadataEntryTypeDef]],  # (3)
    modelId: NotRequired[str],
```

1. See [:material-code-braces: PromptGenAiResourceTypeDef](./type_defs.md#promptgenairesourcetypedef) 
2. See [:material-code-braces: PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef) 
3. See [:material-code-braces: PromptMetadataEntryTypeDef](./type_defs.md#promptmetadataentrytypedef) 
4. See [:material-code-braces: PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef) 
5. See [:material-code-brackets: PromptTemplateTypeType](./literals.md#prompttemplatetypetype) 
## ToolConfigurationTypeDef

```python
# ToolConfigurationTypeDef definition

class ToolConfigurationTypeDef(TypedDict):
    tools: Sequence[ToolUnionTypeDef],  # (2)
    toolChoice: NotRequired[ToolChoiceUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ToolChoiceTypeDef](./type_defs.md#toolchoicetypedef) [:material-code-braces: ToolChoiceOutputTypeDef](./type_defs.md#toolchoiceoutputtypedef) 
2. See [:material-code-braces: ToolTypeDef](./type_defs.md#tooltypedef) [:material-code-braces: ToolOutputTypeDef](./type_defs.md#tooloutputtypedef) 
## CreateDataSourceResponseTypeDef

```python
# CreateDataSourceResponseTypeDef definition

class CreateDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataSourceResponseTypeDef

```python
# GetDataSourceResponseTypeDef definition

class GetDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSourceResponseTypeDef

```python
# UpdateDataSourceResponseTypeDef definition

class UpdateDataSourceResponseTypeDef(TypedDict):
    dataSource: DataSourceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataSourceTypeDef](./type_defs.md#datasourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## KnowledgeBaseTypeDef

```python
# KnowledgeBaseTypeDef definition

class KnowledgeBaseTypeDef(TypedDict):
    createdAt: datetime,
    knowledgeBaseArn: str,
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationOutputTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    roleArn: str,
    status: KnowledgeBaseStatusType,  # (2)
    updatedAt: datetime,
    description: NotRequired[str],
    failureReasons: NotRequired[List[str]],
    storageConfiguration: NotRequired[StorageConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: KnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#knowledgebaseconfigurationoutputtypedef) 
2. See [:material-code-brackets: KnowledgeBaseStatusType](./literals.md#knowledgebasestatustype) 
3. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
## RedshiftConfigurationTypeDef

```python
# RedshiftConfigurationTypeDef definition

class RedshiftConfigurationTypeDef(TypedDict):
    queryEngineConfiguration: RedshiftQueryEngineConfigurationTypeDef,  # (1)
    storageConfigurations: Sequence[RedshiftQueryEngineStorageConfigurationUnionTypeDef],  # (3)
    queryGenerationConfiguration: NotRequired[QueryGenerationConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftQueryEngineConfigurationTypeDef](./type_defs.md#redshiftqueryengineconfigurationtypedef) 
2. See [:material-code-braces: QueryGenerationConfigurationTypeDef](./type_defs.md#querygenerationconfigurationtypedef) [:material-code-braces: QueryGenerationConfigurationOutputTypeDef](./type_defs.md#querygenerationconfigurationoutputtypedef) 
3. See [:material-code-braces: RedshiftQueryEngineStorageConfigurationTypeDef](./type_defs.md#redshiftqueryenginestorageconfigurationtypedef) [:material-code-braces: RedshiftQueryEngineStorageConfigurationOutputTypeDef](./type_defs.md#redshiftqueryenginestorageconfigurationoutputtypedef) 
## PromptFlowNodeSourceConfigurationOutputTypeDef

```python
# PromptFlowNodeSourceConfigurationOutputTypeDef definition

class PromptFlowNodeSourceConfigurationOutputTypeDef(TypedDict):
    inline: NotRequired[PromptFlowNodeInlineConfigurationOutputTypeDef],  # (1)
    resource: NotRequired[PromptFlowNodeResourceConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: PromptFlowNodeInlineConfigurationOutputTypeDef](./type_defs.md#promptflownodeinlineconfigurationoutputtypedef) 
2. See [:material-code-braces: PromptFlowNodeResourceConfigurationTypeDef](./type_defs.md#promptflownoderesourceconfigurationtypedef) 
## CreatePromptResponseTypeDef

```python
# CreatePromptResponseTypeDef definition

class CreatePromptResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    defaultVariant: str,
    description: str,
    id: str,
    name: str,
    updatedAt: datetime,
    variants: List[PromptVariantOutputTypeDef],  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePromptVersionResponseTypeDef

```python
# CreatePromptVersionResponseTypeDef definition

class CreatePromptVersionResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    defaultVariant: str,
    description: str,
    id: str,
    name: str,
    updatedAt: datetime,
    variants: List[PromptVariantOutputTypeDef],  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPromptResponseTypeDef

```python
# GetPromptResponseTypeDef definition

class GetPromptResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    defaultVariant: str,
    description: str,
    id: str,
    name: str,
    updatedAt: datetime,
    variants: List[PromptVariantOutputTypeDef],  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePromptResponseTypeDef

```python
# UpdatePromptResponseTypeDef definition

class UpdatePromptResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    defaultVariant: str,
    description: str,
    id: str,
    name: str,
    updatedAt: datetime,
    variants: List[PromptVariantOutputTypeDef],  # (1)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfluenceDataSourceConfigurationTypeDef

```python
# ConfluenceDataSourceConfigurationTypeDef definition

class ConfluenceDataSourceConfigurationTypeDef(TypedDict):
    sourceConfiguration: ConfluenceSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[ConfluenceCrawlerConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ConfluenceCrawlerConfigurationTypeDef](./type_defs.md#confluencecrawlerconfigurationtypedef) [:material-code-braces: ConfluenceCrawlerConfigurationOutputTypeDef](./type_defs.md#confluencecrawlerconfigurationoutputtypedef) 
2. See [:material-code-braces: ConfluenceSourceConfigurationTypeDef](./type_defs.md#confluencesourceconfigurationtypedef) 
## SalesforceDataSourceConfigurationTypeDef

```python
# SalesforceDataSourceConfigurationTypeDef definition

class SalesforceDataSourceConfigurationTypeDef(TypedDict):
    sourceConfiguration: SalesforceSourceConfigurationTypeDef,  # (2)
    crawlerConfiguration: NotRequired[SalesforceCrawlerConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: SalesforceCrawlerConfigurationTypeDef](./type_defs.md#salesforcecrawlerconfigurationtypedef) [:material-code-braces: SalesforceCrawlerConfigurationOutputTypeDef](./type_defs.md#salesforcecrawlerconfigurationoutputtypedef) 
2. See [:material-code-braces: SalesforceSourceConfigurationTypeDef](./type_defs.md#salesforcesourceconfigurationtypedef) 
## SharePointDataSourceConfigurationTypeDef

```python
# SharePointDataSourceConfigurationTypeDef definition

class SharePointDataSourceConfigurationTypeDef(TypedDict):
    sourceConfiguration: SharePointSourceConfigurationUnionTypeDef,  # (2)
    crawlerConfiguration: NotRequired[SharePointCrawlerConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: SharePointCrawlerConfigurationTypeDef](./type_defs.md#sharepointcrawlerconfigurationtypedef) [:material-code-braces: SharePointCrawlerConfigurationOutputTypeDef](./type_defs.md#sharepointcrawlerconfigurationoutputtypedef) 
2. See [:material-code-braces: SharePointSourceConfigurationTypeDef](./type_defs.md#sharepointsourceconfigurationtypedef) [:material-code-braces: SharePointSourceConfigurationOutputTypeDef](./type_defs.md#sharepointsourceconfigurationoutputtypedef) 
## CreateKnowledgeBaseResponseTypeDef

```python
# CreateKnowledgeBaseResponseTypeDef definition

class CreateKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetKnowledgeBaseResponseTypeDef

```python
# GetKnowledgeBaseResponseTypeDef definition

class GetKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateKnowledgeBaseResponseTypeDef

```python
# UpdateKnowledgeBaseResponseTypeDef definition

class UpdateKnowledgeBaseResponseTypeDef(TypedDict):
    knowledgeBase: KnowledgeBaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KnowledgeBaseTypeDef](./type_defs.md#knowledgebasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromptFlowNodeConfigurationOutputTypeDef

```python
# PromptFlowNodeConfigurationOutputTypeDef definition

class PromptFlowNodeConfigurationOutputTypeDef(TypedDict):
    sourceConfiguration: PromptFlowNodeSourceConfigurationOutputTypeDef,  # (2)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
2. See [:material-code-braces: PromptFlowNodeSourceConfigurationOutputTypeDef](./type_defs.md#promptflownodesourceconfigurationoutputtypedef) 
## ChatPromptTemplateConfigurationTypeDef

```python
# ChatPromptTemplateConfigurationTypeDef definition

class ChatPromptTemplateConfigurationTypeDef(TypedDict):
    messages: Sequence[MessageUnionTypeDef],  # (2)
    inputVariables: NotRequired[Sequence[PromptInputVariableTypeDef]],  # (1)
    system: NotRequired[Sequence[SystemContentBlockTypeDef]],  # (3)
    toolConfiguration: NotRequired[ToolConfigurationUnionTypeDef],  # (4)
```

1. See [:material-code-braces: PromptInputVariableTypeDef](./type_defs.md#promptinputvariabletypedef) 
2. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) [:material-code-braces: MessageOutputTypeDef](./type_defs.md#messageoutputtypedef) 
3. See [:material-code-braces: SystemContentBlockTypeDef](./type_defs.md#systemcontentblocktypedef) 
4. See [:material-code-braces: ToolConfigurationTypeDef](./type_defs.md#toolconfigurationtypedef) [:material-code-braces: ToolConfigurationOutputTypeDef](./type_defs.md#toolconfigurationoutputtypedef) 
## SqlKnowledgeBaseConfigurationTypeDef

```python
# SqlKnowledgeBaseConfigurationTypeDef definition

class SqlKnowledgeBaseConfigurationTypeDef(TypedDict):
    type: QueryEngineTypeType,  # (2)
    redshiftConfiguration: NotRequired[RedshiftConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: RedshiftConfigurationTypeDef](./type_defs.md#redshiftconfigurationtypedef) [:material-code-braces: RedshiftConfigurationOutputTypeDef](./type_defs.md#redshiftconfigurationoutputtypedef) 
2. See [:material-code-brackets: QueryEngineTypeType](./literals.md#queryenginetypetype) 
## FlowNodeConfigurationOutputTypeDef

```python
# FlowNodeConfigurationOutputTypeDef definition

class FlowNodeConfigurationOutputTypeDef(TypedDict):
    agent: NotRequired[AgentFlowNodeConfigurationTypeDef],  # (1)
    collector: NotRequired[Dict[str, Any]],
    condition: NotRequired[ConditionFlowNodeConfigurationOutputTypeDef],  # (2)
    input: NotRequired[Dict[str, Any]],
    iterator: NotRequired[Dict[str, Any]],
    knowledgeBase: NotRequired[KnowledgeBaseFlowNodeConfigurationTypeDef],  # (3)
    lambdaFunction: NotRequired[LambdaFunctionFlowNodeConfigurationTypeDef],  # (4)
    lex: NotRequired[LexFlowNodeConfigurationTypeDef],  # (5)
    output: NotRequired[Dict[str, Any]],
    prompt: NotRequired[PromptFlowNodeConfigurationOutputTypeDef],  # (6)
    retrieval: NotRequired[RetrievalFlowNodeConfigurationTypeDef],  # (7)
    storage: NotRequired[StorageFlowNodeConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: AgentFlowNodeConfigurationTypeDef](./type_defs.md#agentflownodeconfigurationtypedef) 
2. See [:material-code-braces: ConditionFlowNodeConfigurationOutputTypeDef](./type_defs.md#conditionflownodeconfigurationoutputtypedef) 
3. See [:material-code-braces: KnowledgeBaseFlowNodeConfigurationTypeDef](./type_defs.md#knowledgebaseflownodeconfigurationtypedef) 
4. See [:material-code-braces: LambdaFunctionFlowNodeConfigurationTypeDef](./type_defs.md#lambdafunctionflownodeconfigurationtypedef) 
5. See [:material-code-braces: LexFlowNodeConfigurationTypeDef](./type_defs.md#lexflownodeconfigurationtypedef) 
6. See [:material-code-braces: PromptFlowNodeConfigurationOutputTypeDef](./type_defs.md#promptflownodeconfigurationoutputtypedef) 
7. See [:material-code-braces: RetrievalFlowNodeConfigurationTypeDef](./type_defs.md#retrievalflownodeconfigurationtypedef) 
8. See [:material-code-braces: StorageFlowNodeConfigurationTypeDef](./type_defs.md#storageflownodeconfigurationtypedef) 
## DataSourceConfigurationTypeDef

```python
# DataSourceConfigurationTypeDef definition

class DataSourceConfigurationTypeDef(TypedDict):
    type: DataSourceTypeType,  # (5)
    confluenceConfiguration: NotRequired[ConfluenceDataSourceConfigurationUnionTypeDef],  # (1)
    s3Configuration: NotRequired[S3DataSourceConfigurationUnionTypeDef],  # (2)
    salesforceConfiguration: NotRequired[SalesforceDataSourceConfigurationUnionTypeDef],  # (3)
    sharePointConfiguration: NotRequired[SharePointDataSourceConfigurationUnionTypeDef],  # (4)
    webConfiguration: NotRequired[WebDataSourceConfigurationUnionTypeDef],  # (6)
```

1. See [:material-code-braces: ConfluenceDataSourceConfigurationTypeDef](./type_defs.md#confluencedatasourceconfigurationtypedef) [:material-code-braces: ConfluenceDataSourceConfigurationOutputTypeDef](./type_defs.md#confluencedatasourceconfigurationoutputtypedef) 
2. See [:material-code-braces: S3DataSourceConfigurationTypeDef](./type_defs.md#s3datasourceconfigurationtypedef) [:material-code-braces: S3DataSourceConfigurationOutputTypeDef](./type_defs.md#s3datasourceconfigurationoutputtypedef) 
3. See [:material-code-braces: SalesforceDataSourceConfigurationTypeDef](./type_defs.md#salesforcedatasourceconfigurationtypedef) [:material-code-braces: SalesforceDataSourceConfigurationOutputTypeDef](./type_defs.md#salesforcedatasourceconfigurationoutputtypedef) 
4. See [:material-code-braces: SharePointDataSourceConfigurationTypeDef](./type_defs.md#sharepointdatasourceconfigurationtypedef) [:material-code-braces: SharePointDataSourceConfigurationOutputTypeDef](./type_defs.md#sharepointdatasourceconfigurationoutputtypedef) 
5. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
6. See [:material-code-braces: WebDataSourceConfigurationTypeDef](./type_defs.md#webdatasourceconfigurationtypedef) [:material-code-braces: WebDataSourceConfigurationOutputTypeDef](./type_defs.md#webdatasourceconfigurationoutputtypedef) 
## FlowNodeExtraOutputTypeDef

```python
# FlowNodeExtraOutputTypeDef definition

class FlowNodeExtraOutputTypeDef(TypedDict):
    name: str,
    type: FlowNodeTypeType,  # (4)
    configuration: NotRequired[FlowNodeConfigurationOutputTypeDef],  # (1)
    inputs: NotRequired[List[FlowNodeInputTypeDef]],  # (2)
    outputs: NotRequired[List[FlowNodeOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: FlowNodeConfigurationOutputTypeDef](./type_defs.md#flownodeconfigurationoutputtypedef) 
2. See [:material-code-braces: FlowNodeInputTypeDef](./type_defs.md#flownodeinputtypedef) 
3. See [:material-code-braces: FlowNodeOutputTypeDef](./type_defs.md#flownodeoutputtypedef) 
4. See [:material-code-brackets: FlowNodeTypeType](./literals.md#flownodetypetype) 
## PromptTemplateConfigurationTypeDef

```python
# PromptTemplateConfigurationTypeDef definition

class PromptTemplateConfigurationTypeDef(TypedDict):
    chat: NotRequired[ChatPromptTemplateConfigurationUnionTypeDef],  # (1)
    text: NotRequired[TextPromptTemplateConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ChatPromptTemplateConfigurationTypeDef](./type_defs.md#chatprompttemplateconfigurationtypedef) [:material-code-braces: ChatPromptTemplateConfigurationOutputTypeDef](./type_defs.md#chatprompttemplateconfigurationoutputtypedef) 
2. See [:material-code-braces: TextPromptTemplateConfigurationTypeDef](./type_defs.md#textprompttemplateconfigurationtypedef) [:material-code-braces: TextPromptTemplateConfigurationOutputTypeDef](./type_defs.md#textprompttemplateconfigurationoutputtypedef) 
## CreateDataSourceRequestRequestTypeDef

```python
# CreateDataSourceRequestRequestTypeDef definition

class CreateDataSourceRequestRequestTypeDef(TypedDict):
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    clientToken: NotRequired[str],
    dataDeletionPolicy: NotRequired[DataDeletionPolicyType],  # (2)
    description: NotRequired[str],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-brackets: DataDeletionPolicyType](./literals.md#datadeletionpolicytype) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
## UpdateDataSourceRequestRequestTypeDef

```python
# UpdateDataSourceRequestRequestTypeDef definition

class UpdateDataSourceRequestRequestTypeDef(TypedDict):
    dataSourceConfiguration: DataSourceConfigurationTypeDef,  # (1)
    dataSourceId: str,
    knowledgeBaseId: str,
    name: str,
    dataDeletionPolicy: NotRequired[DataDeletionPolicyType],  # (2)
    description: NotRequired[str],
    serverSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (3)
    vectorIngestionConfiguration: NotRequired[VectorIngestionConfigurationTypeDef],  # (4)
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-brackets: DataDeletionPolicyType](./literals.md#datadeletionpolicytype) 
3. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
4. See [:material-code-braces: VectorIngestionConfigurationTypeDef](./type_defs.md#vectoringestionconfigurationtypedef) 
## KnowledgeBaseConfigurationTypeDef

```python
# KnowledgeBaseConfigurationTypeDef definition

class KnowledgeBaseConfigurationTypeDef(TypedDict):
    type: KnowledgeBaseTypeType,  # (3)
    kendraKnowledgeBaseConfiguration: NotRequired[KendraKnowledgeBaseConfigurationTypeDef],  # (1)
    sqlKnowledgeBaseConfiguration: NotRequired[SqlKnowledgeBaseConfigurationUnionTypeDef],  # (2)
    vectorKnowledgeBaseConfiguration: NotRequired[VectorKnowledgeBaseConfigurationUnionTypeDef],  # (4)
```

1. See [:material-code-braces: KendraKnowledgeBaseConfigurationTypeDef](./type_defs.md#kendraknowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: SqlKnowledgeBaseConfigurationTypeDef](./type_defs.md#sqlknowledgebaseconfigurationtypedef) [:material-code-braces: SqlKnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#sqlknowledgebaseconfigurationoutputtypedef) 
3. See [:material-code-brackets: KnowledgeBaseTypeType](./literals.md#knowledgebasetypetype) 
4. See [:material-code-braces: VectorKnowledgeBaseConfigurationTypeDef](./type_defs.md#vectorknowledgebaseconfigurationtypedef) [:material-code-braces: VectorKnowledgeBaseConfigurationOutputTypeDef](./type_defs.md#vectorknowledgebaseconfigurationoutputtypedef) 
## FlowDefinitionOutputTypeDef

```python
# FlowDefinitionOutputTypeDef definition

class FlowDefinitionOutputTypeDef(TypedDict):
    connections: NotRequired[List[FlowConnectionTypeDef]],  # (1)
    nodes: NotRequired[List[FlowNodeExtraOutputTypeDef]],  # (2)
```

1. See [:material-code-braces: FlowConnectionTypeDef](./type_defs.md#flowconnectiontypedef) 
2. See [:material-code-braces: FlowNodeExtraOutputTypeDef](./type_defs.md#flownodeextraoutputtypedef) 
## CreateKnowledgeBaseRequestRequestTypeDef

```python
# CreateKnowledgeBaseRequestRequestTypeDef definition

class CreateKnowledgeBaseRequestRequestTypeDef(TypedDict):
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    name: str,
    roleArn: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    storageConfiguration: NotRequired[StorageConfigurationTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
## UpdateKnowledgeBaseRequestRequestTypeDef

```python
# UpdateKnowledgeBaseRequestRequestTypeDef definition

class UpdateKnowledgeBaseRequestRequestTypeDef(TypedDict):
    knowledgeBaseConfiguration: KnowledgeBaseConfigurationTypeDef,  # (1)
    knowledgeBaseId: str,
    name: str,
    roleArn: str,
    description: NotRequired[str],
    storageConfiguration: NotRequired[StorageConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: KnowledgeBaseConfigurationTypeDef](./type_defs.md#knowledgebaseconfigurationtypedef) 
2. See [:material-code-braces: StorageConfigurationTypeDef](./type_defs.md#storageconfigurationtypedef) 
## CreateFlowResponseTypeDef

```python
# CreateFlowResponseTypeDef definition

class CreateFlowResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    updatedAt: datetime,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef) 
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFlowVersionResponseTypeDef

```python
# CreateFlowVersionResponseTypeDef definition

class CreateFlowVersionResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef) 
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFlowResponseTypeDef

```python
# GetFlowResponseTypeDef definition

class GetFlowResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    updatedAt: datetime,
    validations: List[FlowValidationTypeDef],  # (3)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef) 
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype) 
3. See [:material-code-braces: FlowValidationTypeDef](./type_defs.md#flowvalidationtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetFlowVersionResponseTypeDef

```python
# GetFlowVersionResponseTypeDef definition

class GetFlowVersionResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef) 
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFlowResponseTypeDef

```python
# UpdateFlowResponseTypeDef definition

class UpdateFlowResponseTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    customerEncryptionKeyArn: str,
    definition: FlowDefinitionOutputTypeDef,  # (1)
    description: str,
    executionRoleArn: str,
    id: str,
    name: str,
    status: FlowStatusType,  # (2)
    updatedAt: datetime,
    version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: FlowDefinitionOutputTypeDef](./type_defs.md#flowdefinitionoutputtypedef) 
2. See [:material-code-brackets: FlowStatusType](./literals.md#flowstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromptFlowNodeInlineConfigurationTypeDef

```python
# PromptFlowNodeInlineConfigurationTypeDef definition

class PromptFlowNodeInlineConfigurationTypeDef(TypedDict):
    modelId: str,
    templateConfiguration: PromptTemplateConfigurationUnionTypeDef,  # (2)
    templateType: PromptTemplateTypeType,  # (3)
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    inferenceConfiguration: NotRequired[PromptInferenceConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: PromptInferenceConfigurationTypeDef](./type_defs.md#promptinferenceconfigurationtypedef) [:material-code-braces: PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef) 
2. See [:material-code-braces: PromptTemplateConfigurationTypeDef](./type_defs.md#prompttemplateconfigurationtypedef) [:material-code-braces: PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef) 
3. See [:material-code-brackets: PromptTemplateTypeType](./literals.md#prompttemplatetypetype) 
## PromptVariantTypeDef

```python
# PromptVariantTypeDef definition

class PromptVariantTypeDef(TypedDict):
    name: str,
    templateConfiguration: PromptTemplateConfigurationUnionTypeDef,  # (4)
    templateType: PromptTemplateTypeType,  # (5)
    additionalModelRequestFields: NotRequired[Mapping[str, Any]],
    genAiResource: NotRequired[PromptGenAiResourceTypeDef],  # (1)
    inferenceConfiguration: NotRequired[PromptInferenceConfigurationUnionTypeDef],  # (2)
    metadata: NotRequired[Sequence[PromptMetadataEntryTypeDef]],  # (3)
    modelId: NotRequired[str],
```

1. See [:material-code-braces: PromptGenAiResourceTypeDef](./type_defs.md#promptgenairesourcetypedef) 
2. See [:material-code-braces: PromptInferenceConfigurationTypeDef](./type_defs.md#promptinferenceconfigurationtypedef) [:material-code-braces: PromptInferenceConfigurationOutputTypeDef](./type_defs.md#promptinferenceconfigurationoutputtypedef) 
3. See [:material-code-braces: PromptMetadataEntryTypeDef](./type_defs.md#promptmetadataentrytypedef) 
4. See [:material-code-braces: PromptTemplateConfigurationTypeDef](./type_defs.md#prompttemplateconfigurationtypedef) [:material-code-braces: PromptTemplateConfigurationOutputTypeDef](./type_defs.md#prompttemplateconfigurationoutputtypedef) 
5. See [:material-code-brackets: PromptTemplateTypeType](./literals.md#prompttemplatetypetype) 
## UpdatePromptRequestRequestTypeDef

```python
# UpdatePromptRequestRequestTypeDef definition

class UpdatePromptRequestRequestTypeDef(TypedDict):
    name: str,
    promptIdentifier: str,
    customerEncryptionKeyArn: NotRequired[str],
    defaultVariant: NotRequired[str],
    description: NotRequired[str],
    variants: NotRequired[Sequence[PromptVariantTypeDef]],  # (1)
```

1. See [:material-code-braces: PromptVariantTypeDef](./type_defs.md#promptvarianttypedef) 
## PromptFlowNodeSourceConfigurationTypeDef

```python
# PromptFlowNodeSourceConfigurationTypeDef definition

class PromptFlowNodeSourceConfigurationTypeDef(TypedDict):
    inline: NotRequired[PromptFlowNodeInlineConfigurationUnionTypeDef],  # (1)
    resource: NotRequired[PromptFlowNodeResourceConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: PromptFlowNodeInlineConfigurationTypeDef](./type_defs.md#promptflownodeinlineconfigurationtypedef) [:material-code-braces: PromptFlowNodeInlineConfigurationOutputTypeDef](./type_defs.md#promptflownodeinlineconfigurationoutputtypedef) 
2. See [:material-code-braces: PromptFlowNodeResourceConfigurationTypeDef](./type_defs.md#promptflownoderesourceconfigurationtypedef) 
## CreatePromptRequestRequestTypeDef

```python
# CreatePromptRequestRequestTypeDef definition

class CreatePromptRequestRequestTypeDef(TypedDict):
    name: str,
    clientToken: NotRequired[str],
    customerEncryptionKeyArn: NotRequired[str],
    defaultVariant: NotRequired[str],
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    variants: NotRequired[Sequence[PromptVariantUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: PromptVariantTypeDef](./type_defs.md#promptvarianttypedef) [:material-code-braces: PromptVariantOutputTypeDef](./type_defs.md#promptvariantoutputtypedef) 
## PromptFlowNodeConfigurationTypeDef

```python
# PromptFlowNodeConfigurationTypeDef definition

class PromptFlowNodeConfigurationTypeDef(TypedDict):
    sourceConfiguration: PromptFlowNodeSourceConfigurationUnionTypeDef,  # (2)
    guardrailConfiguration: NotRequired[GuardrailConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: GuardrailConfigurationTypeDef](./type_defs.md#guardrailconfigurationtypedef) 
2. See [:material-code-braces: PromptFlowNodeSourceConfigurationTypeDef](./type_defs.md#promptflownodesourceconfigurationtypedef) [:material-code-braces: PromptFlowNodeSourceConfigurationOutputTypeDef](./type_defs.md#promptflownodesourceconfigurationoutputtypedef) 
## FlowNodeConfigurationTypeDef

```python
# FlowNodeConfigurationTypeDef definition

class FlowNodeConfigurationTypeDef(TypedDict):
    agent: NotRequired[AgentFlowNodeConfigurationTypeDef],  # (1)
    collector: NotRequired[Mapping[str, Any]],
    condition: NotRequired[ConditionFlowNodeConfigurationUnionTypeDef],  # (2)
    input: NotRequired[Mapping[str, Any]],
    iterator: NotRequired[Mapping[str, Any]],
    knowledgeBase: NotRequired[KnowledgeBaseFlowNodeConfigurationTypeDef],  # (3)
    lambdaFunction: NotRequired[LambdaFunctionFlowNodeConfigurationTypeDef],  # (4)
    lex: NotRequired[LexFlowNodeConfigurationTypeDef],  # (5)
    output: NotRequired[Mapping[str, Any]],
    prompt: NotRequired[PromptFlowNodeConfigurationUnionTypeDef],  # (6)
    retrieval: NotRequired[RetrievalFlowNodeConfigurationTypeDef],  # (7)
    storage: NotRequired[StorageFlowNodeConfigurationTypeDef],  # (8)
```

1. See [:material-code-braces: AgentFlowNodeConfigurationTypeDef](./type_defs.md#agentflownodeconfigurationtypedef) 
2. See [:material-code-braces: ConditionFlowNodeConfigurationTypeDef](./type_defs.md#conditionflownodeconfigurationtypedef) [:material-code-braces: ConditionFlowNodeConfigurationOutputTypeDef](./type_defs.md#conditionflownodeconfigurationoutputtypedef) 
3. See [:material-code-braces: KnowledgeBaseFlowNodeConfigurationTypeDef](./type_defs.md#knowledgebaseflownodeconfigurationtypedef) 
4. See [:material-code-braces: LambdaFunctionFlowNodeConfigurationTypeDef](./type_defs.md#lambdafunctionflownodeconfigurationtypedef) 
5. See [:material-code-braces: LexFlowNodeConfigurationTypeDef](./type_defs.md#lexflownodeconfigurationtypedef) 
6. See [:material-code-braces: PromptFlowNodeConfigurationTypeDef](./type_defs.md#promptflownodeconfigurationtypedef) [:material-code-braces: PromptFlowNodeConfigurationOutputTypeDef](./type_defs.md#promptflownodeconfigurationoutputtypedef) 
7. See [:material-code-braces: RetrievalFlowNodeConfigurationTypeDef](./type_defs.md#retrievalflownodeconfigurationtypedef) 
8. See [:material-code-braces: StorageFlowNodeConfigurationTypeDef](./type_defs.md#storageflownodeconfigurationtypedef) 
## FlowNodeTypeDef

```python
# FlowNodeTypeDef definition

class FlowNodeTypeDef(TypedDict):
    name: str,
    type: FlowNodeTypeType,  # (4)
    configuration: NotRequired[FlowNodeConfigurationUnionTypeDef],  # (1)
    inputs: NotRequired[Sequence[FlowNodeInputTypeDef]],  # (2)
    outputs: NotRequired[Sequence[FlowNodeOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: FlowNodeConfigurationTypeDef](./type_defs.md#flownodeconfigurationtypedef) [:material-code-braces: FlowNodeConfigurationOutputTypeDef](./type_defs.md#flownodeconfigurationoutputtypedef) 
2. See [:material-code-braces: FlowNodeInputTypeDef](./type_defs.md#flownodeinputtypedef) 
3. See [:material-code-braces: FlowNodeOutputTypeDef](./type_defs.md#flownodeoutputtypedef) 
4. See [:material-code-brackets: FlowNodeTypeType](./literals.md#flownodetypetype) 
## FlowDefinitionTypeDef

```python
# FlowDefinitionTypeDef definition

class FlowDefinitionTypeDef(TypedDict):
    connections: NotRequired[Sequence[FlowConnectionTypeDef]],  # (1)
    nodes: NotRequired[Sequence[FlowNodeUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: FlowConnectionTypeDef](./type_defs.md#flowconnectiontypedef) 
2. See [:material-code-braces: FlowNodeTypeDef](./type_defs.md#flownodetypedef) [:material-code-braces: FlowNodeExtraOutputTypeDef](./type_defs.md#flownodeextraoutputtypedef) 
## CreateFlowRequestRequestTypeDef

```python
# CreateFlowRequestRequestTypeDef definition

class CreateFlowRequestRequestTypeDef(TypedDict):
    executionRoleArn: str,
    name: str,
    clientToken: NotRequired[str],
    customerEncryptionKeyArn: NotRequired[str],
    definition: NotRequired[FlowDefinitionTypeDef],  # (1)
    description: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef) 
## UpdateFlowRequestRequestTypeDef

```python
# UpdateFlowRequestRequestTypeDef definition

class UpdateFlowRequestRequestTypeDef(TypedDict):
    executionRoleArn: str,
    flowIdentifier: str,
    name: str,
    customerEncryptionKeyArn: NotRequired[str],
    definition: NotRequired[FlowDefinitionTypeDef],  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef) 
## ValidateFlowDefinitionRequestRequestTypeDef

```python
# ValidateFlowDefinitionRequestRequestTypeDef definition

class ValidateFlowDefinitionRequestRequestTypeDef(TypedDict):
    definition: FlowDefinitionTypeDef,  # (1)
```

1. See [:material-code-braces: FlowDefinitionTypeDef](./type_defs.md#flowdefinitiontypedef) 

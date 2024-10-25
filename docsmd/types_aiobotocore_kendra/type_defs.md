# Type definitions

> [Index](../README.md) > [Kendra](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Kendra](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#Kendra)
    type annotations stubs module [types-aiobotocore-kendra](https://pypi.org/project/types-aiobotocore-kendra/).

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


## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ContentSourceConfigurationUnionTypeDef

```python
# ContentSourceConfigurationUnionTypeDef definition

ContentSourceConfigurationUnionTypeDef = Union[
    ContentSourceConfigurationTypeDef,  # (1)
    ContentSourceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ContentSourceConfigurationTypeDef](./type_defs.md#contentsourceconfigurationtypedef) 
2. See [:material-code-braces: ContentSourceConfigurationOutputTypeDef](./type_defs.md#contentsourceconfigurationoutputtypedef) 

## DataSourceVpcConfigurationUnionTypeDef

```python
# DataSourceVpcConfigurationUnionTypeDef definition

DataSourceVpcConfigurationUnionTypeDef = Union[
    DataSourceVpcConfigurationTypeDef,  # (1)
    DataSourceVpcConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
2. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 

## RelevanceUnionTypeDef

```python
# RelevanceUnionTypeDef definition

RelevanceUnionTypeDef = Union[
    RelevanceTypeDef,  # (1)
    RelevanceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RelevanceTypeDef](./type_defs.md#relevancetypedef) 
2. See [:material-code-braces: RelevanceOutputTypeDef](./type_defs.md#relevanceoutputtypedef) 

## SeedUrlConfigurationUnionTypeDef

```python
# SeedUrlConfigurationUnionTypeDef definition

SeedUrlConfigurationUnionTypeDef = Union[
    SeedUrlConfigurationTypeDef,  # (1)
    SeedUrlConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SeedUrlConfigurationTypeDef](./type_defs.md#seedurlconfigurationtypedef) 
2. See [:material-code-braces: SeedUrlConfigurationOutputTypeDef](./type_defs.md#seedurlconfigurationoutputtypedef) 

## SiteMapsConfigurationUnionTypeDef

```python
# SiteMapsConfigurationUnionTypeDef definition

SiteMapsConfigurationUnionTypeDef = Union[
    SiteMapsConfigurationTypeDef,  # (1)
    SiteMapsConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SiteMapsConfigurationTypeDef](./type_defs.md#sitemapsconfigurationtypedef) 
2. See [:material-code-braces: SiteMapsConfigurationOutputTypeDef](./type_defs.md#sitemapsconfigurationoutputtypedef) 

## TemplateConfigurationUnionTypeDef

```python
# TemplateConfigurationUnionTypeDef definition

TemplateConfigurationUnionTypeDef = Union[
    TemplateConfigurationTypeDef,  # (1)
    TemplateConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef) 
2. See [:material-code-braces: TemplateConfigurationOutputTypeDef](./type_defs.md#templateconfigurationoutputtypedef) 

## ColumnConfigurationUnionTypeDef

```python
# ColumnConfigurationUnionTypeDef definition

ColumnConfigurationUnionTypeDef = Union[
    ColumnConfigurationTypeDef,  # (1)
    ColumnConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnConfigurationTypeDef](./type_defs.md#columnconfigurationtypedef) 
2. See [:material-code-braces: ColumnConfigurationOutputTypeDef](./type_defs.md#columnconfigurationoutputtypedef) 

## GoogleDriveConfigurationUnionTypeDef

```python
# GoogleDriveConfigurationUnionTypeDef definition

GoogleDriveConfigurationUnionTypeDef = Union[
    GoogleDriveConfigurationTypeDef,  # (1)
    GoogleDriveConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GoogleDriveConfigurationTypeDef](./type_defs.md#googledriveconfigurationtypedef) 
2. See [:material-code-braces: GoogleDriveConfigurationOutputTypeDef](./type_defs.md#googledriveconfigurationoutputtypedef) 

## SalesforceChatterFeedConfigurationUnionTypeDef

```python
# SalesforceChatterFeedConfigurationUnionTypeDef definition

SalesforceChatterFeedConfigurationUnionTypeDef = Union[
    SalesforceChatterFeedConfigurationTypeDef,  # (1)
    SalesforceChatterFeedConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceChatterFeedConfigurationTypeDef](./type_defs.md#salesforcechatterfeedconfigurationtypedef) 
2. See [:material-code-braces: SalesforceChatterFeedConfigurationOutputTypeDef](./type_defs.md#salesforcechatterfeedconfigurationoutputtypedef) 

## SalesforceCustomKnowledgeArticleTypeConfigurationUnionTypeDef

```python
# SalesforceCustomKnowledgeArticleTypeConfigurationUnionTypeDef definition

SalesforceCustomKnowledgeArticleTypeConfigurationUnionTypeDef = Union[
    SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef,  # (1)
    SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef](./type_defs.md#salesforcecustomknowledgearticletypeconfigurationtypedef) 
2. See [:material-code-braces: SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef](./type_defs.md#salesforcecustomknowledgearticletypeconfigurationoutputtypedef) 

## SalesforceStandardKnowledgeArticleTypeConfigurationUnionTypeDef

```python
# SalesforceStandardKnowledgeArticleTypeConfigurationUnionTypeDef definition

SalesforceStandardKnowledgeArticleTypeConfigurationUnionTypeDef = Union[
    SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef,  # (1)
    SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef](./type_defs.md#salesforcestandardknowledgearticletypeconfigurationtypedef) 
2. See [:material-code-braces: SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef](./type_defs.md#salesforcestandardknowledgearticletypeconfigurationoutputtypedef) 

## SalesforceStandardObjectAttachmentConfigurationUnionTypeDef

```python
# SalesforceStandardObjectAttachmentConfigurationUnionTypeDef definition

SalesforceStandardObjectAttachmentConfigurationUnionTypeDef = Union[
    SalesforceStandardObjectAttachmentConfigurationTypeDef,  # (1)
    SalesforceStandardObjectAttachmentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceStandardObjectAttachmentConfigurationTypeDef](./type_defs.md#salesforcestandardobjectattachmentconfigurationtypedef) 
2. See [:material-code-braces: SalesforceStandardObjectAttachmentConfigurationOutputTypeDef](./type_defs.md#salesforcestandardobjectattachmentconfigurationoutputtypedef) 

## SalesforceStandardObjectConfigurationUnionTypeDef

```python
# SalesforceStandardObjectConfigurationUnionTypeDef definition

SalesforceStandardObjectConfigurationUnionTypeDef = Union[
    SalesforceStandardObjectConfigurationTypeDef,  # (1)
    SalesforceStandardObjectConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceStandardObjectConfigurationTypeDef](./type_defs.md#salesforcestandardobjectconfigurationtypedef) 
2. See [:material-code-braces: SalesforceStandardObjectConfigurationOutputTypeDef](./type_defs.md#salesforcestandardobjectconfigurationoutputtypedef) 

## ServiceNowKnowledgeArticleConfigurationUnionTypeDef

```python
# ServiceNowKnowledgeArticleConfigurationUnionTypeDef definition

ServiceNowKnowledgeArticleConfigurationUnionTypeDef = Union[
    ServiceNowKnowledgeArticleConfigurationTypeDef,  # (1)
    ServiceNowKnowledgeArticleConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceNowKnowledgeArticleConfigurationTypeDef](./type_defs.md#servicenowknowledgearticleconfigurationtypedef) 
2. See [:material-code-braces: ServiceNowKnowledgeArticleConfigurationOutputTypeDef](./type_defs.md#servicenowknowledgearticleconfigurationoutputtypedef) 

## ServiceNowServiceCatalogConfigurationUnionTypeDef

```python
# ServiceNowServiceCatalogConfigurationUnionTypeDef definition

ServiceNowServiceCatalogConfigurationUnionTypeDef = Union[
    ServiceNowServiceCatalogConfigurationTypeDef,  # (1)
    ServiceNowServiceCatalogConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceNowServiceCatalogConfigurationTypeDef](./type_defs.md#servicenowservicecatalogconfigurationtypedef) 
2. See [:material-code-braces: ServiceNowServiceCatalogConfigurationOutputTypeDef](./type_defs.md#servicenowservicecatalogconfigurationoutputtypedef) 

## WorkDocsConfigurationUnionTypeDef

```python
# WorkDocsConfigurationUnionTypeDef definition

WorkDocsConfigurationUnionTypeDef = Union[
    WorkDocsConfigurationTypeDef,  # (1)
    WorkDocsConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: WorkDocsConfigurationTypeDef](./type_defs.md#workdocsconfigurationtypedef) 
2. See [:material-code-braces: WorkDocsConfigurationOutputTypeDef](./type_defs.md#workdocsconfigurationoutputtypedef) 

## OneDriveUsersUnionTypeDef

```python
# OneDriveUsersUnionTypeDef definition

OneDriveUsersUnionTypeDef = Union[
    OneDriveUsersTypeDef,  # (1)
    OneDriveUsersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OneDriveUsersTypeDef](./type_defs.md#onedriveuserstypedef) 
2. See [:material-code-braces: OneDriveUsersOutputTypeDef](./type_defs.md#onedriveusersoutputtypedef) 

## AuthenticationConfigurationUnionTypeDef

```python
# AuthenticationConfigurationUnionTypeDef definition

AuthenticationConfigurationUnionTypeDef = Union[
    AuthenticationConfigurationTypeDef,  # (1)
    AuthenticationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef) 
2. See [:material-code-braces: AuthenticationConfigurationOutputTypeDef](./type_defs.md#authenticationconfigurationoutputtypedef) 

## DocumentAttributeValueUnionTypeDef

```python
# DocumentAttributeValueUnionTypeDef definition

DocumentAttributeValueUnionTypeDef = Union[
    DocumentAttributeValueTypeDef,  # (1)
    DocumentAttributeValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) 
2. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 

## ConfluenceAttachmentConfigurationUnionTypeDef

```python
# ConfluenceAttachmentConfigurationUnionTypeDef definition

ConfluenceAttachmentConfigurationUnionTypeDef = Union[
    ConfluenceAttachmentConfigurationTypeDef,  # (1)
    ConfluenceAttachmentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfluenceAttachmentConfigurationTypeDef](./type_defs.md#confluenceattachmentconfigurationtypedef) 
2. See [:material-code-braces: ConfluenceAttachmentConfigurationOutputTypeDef](./type_defs.md#confluenceattachmentconfigurationoutputtypedef) 

## ConfluenceBlogConfigurationUnionTypeDef

```python
# ConfluenceBlogConfigurationUnionTypeDef definition

ConfluenceBlogConfigurationUnionTypeDef = Union[
    ConfluenceBlogConfigurationTypeDef,  # (1)
    ConfluenceBlogConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfluenceBlogConfigurationTypeDef](./type_defs.md#confluenceblogconfigurationtypedef) 
2. See [:material-code-braces: ConfluenceBlogConfigurationOutputTypeDef](./type_defs.md#confluenceblogconfigurationoutputtypedef) 

## ConfluencePageConfigurationUnionTypeDef

```python
# ConfluencePageConfigurationUnionTypeDef definition

ConfluencePageConfigurationUnionTypeDef = Union[
    ConfluencePageConfigurationTypeDef,  # (1)
    ConfluencePageConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfluencePageConfigurationTypeDef](./type_defs.md#confluencepageconfigurationtypedef) 
2. See [:material-code-braces: ConfluencePageConfigurationOutputTypeDef](./type_defs.md#confluencepageconfigurationoutputtypedef) 

## ConfluenceSpaceConfigurationUnionTypeDef

```python
# ConfluenceSpaceConfigurationUnionTypeDef definition

ConfluenceSpaceConfigurationUnionTypeDef = Union[
    ConfluenceSpaceConfigurationTypeDef,  # (1)
    ConfluenceSpaceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfluenceSpaceConfigurationTypeDef](./type_defs.md#confluencespaceconfigurationtypedef) 
2. See [:material-code-braces: ConfluenceSpaceConfigurationOutputTypeDef](./type_defs.md#confluencespaceconfigurationoutputtypedef) 

## HierarchicalPrincipalUnionTypeDef

```python
# HierarchicalPrincipalUnionTypeDef definition

HierarchicalPrincipalUnionTypeDef = Union[
    HierarchicalPrincipalTypeDef,  # (1)
    HierarchicalPrincipalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HierarchicalPrincipalTypeDef](./type_defs.md#hierarchicalprincipaltypedef) 
2. See [:material-code-braces: HierarchicalPrincipalOutputTypeDef](./type_defs.md#hierarchicalprincipaloutputtypedef) 

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

## AlfrescoConfigurationUnionTypeDef

```python
# AlfrescoConfigurationUnionTypeDef definition

AlfrescoConfigurationUnionTypeDef = Union[
    AlfrescoConfigurationTypeDef,  # (1)
    AlfrescoConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AlfrescoConfigurationTypeDef](./type_defs.md#alfrescoconfigurationtypedef) 
2. See [:material-code-braces: AlfrescoConfigurationOutputTypeDef](./type_defs.md#alfrescoconfigurationoutputtypedef) 

## BoxConfigurationUnionTypeDef

```python
# BoxConfigurationUnionTypeDef definition

BoxConfigurationUnionTypeDef = Union[
    BoxConfigurationTypeDef,  # (1)
    BoxConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BoxConfigurationTypeDef](./type_defs.md#boxconfigurationtypedef) 
2. See [:material-code-braces: BoxConfigurationOutputTypeDef](./type_defs.md#boxconfigurationoutputtypedef) 

## FsxConfigurationUnionTypeDef

```python
# FsxConfigurationUnionTypeDef definition

FsxConfigurationUnionTypeDef = Union[
    FsxConfigurationTypeDef,  # (1)
    FsxConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: FsxConfigurationTypeDef](./type_defs.md#fsxconfigurationtypedef) 
2. See [:material-code-braces: FsxConfigurationOutputTypeDef](./type_defs.md#fsxconfigurationoutputtypedef) 

## GitHubConfigurationUnionTypeDef

```python
# GitHubConfigurationUnionTypeDef definition

GitHubConfigurationUnionTypeDef = Union[
    GitHubConfigurationTypeDef,  # (1)
    GitHubConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: GitHubConfigurationTypeDef](./type_defs.md#githubconfigurationtypedef) 
2. See [:material-code-braces: GitHubConfigurationOutputTypeDef](./type_defs.md#githubconfigurationoutputtypedef) 

## JiraConfigurationUnionTypeDef

```python
# JiraConfigurationUnionTypeDef definition

JiraConfigurationUnionTypeDef = Union[
    JiraConfigurationTypeDef,  # (1)
    JiraConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: JiraConfigurationTypeDef](./type_defs.md#jiraconfigurationtypedef) 
2. See [:material-code-braces: JiraConfigurationOutputTypeDef](./type_defs.md#jiraconfigurationoutputtypedef) 

## QuipConfigurationUnionTypeDef

```python
# QuipConfigurationUnionTypeDef definition

QuipConfigurationUnionTypeDef = Union[
    QuipConfigurationTypeDef,  # (1)
    QuipConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: QuipConfigurationTypeDef](./type_defs.md#quipconfigurationtypedef) 
2. See [:material-code-braces: QuipConfigurationOutputTypeDef](./type_defs.md#quipconfigurationoutputtypedef) 

## SharePointConfigurationUnionTypeDef

```python
# SharePointConfigurationUnionTypeDef definition

SharePointConfigurationUnionTypeDef = Union[
    SharePointConfigurationTypeDef,  # (1)
    SharePointConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SharePointConfigurationTypeDef](./type_defs.md#sharepointconfigurationtypedef) 
2. See [:material-code-braces: SharePointConfigurationOutputTypeDef](./type_defs.md#sharepointconfigurationoutputtypedef) 

## SlackConfigurationUnionTypeDef

```python
# SlackConfigurationUnionTypeDef definition

SlackConfigurationUnionTypeDef = Union[
    SlackConfigurationTypeDef,  # (1)
    SlackConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SlackConfigurationTypeDef](./type_defs.md#slackconfigurationtypedef) 
2. See [:material-code-braces: SlackConfigurationOutputTypeDef](./type_defs.md#slackconfigurationoutputtypedef) 

## DocumentMetadataConfigurationUnionTypeDef

```python
# DocumentMetadataConfigurationUnionTypeDef definition

DocumentMetadataConfigurationUnionTypeDef = Union[
    DocumentMetadataConfigurationTypeDef,  # (1)
    DocumentMetadataConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentMetadataConfigurationTypeDef](./type_defs.md#documentmetadataconfigurationtypedef) 
2. See [:material-code-braces: DocumentMetadataConfigurationOutputTypeDef](./type_defs.md#documentmetadataconfigurationoutputtypedef) 

## UrlsUnionTypeDef

```python
# UrlsUnionTypeDef definition

UrlsUnionTypeDef = Union[
    UrlsTypeDef,  # (1)
    UrlsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UrlsTypeDef](./type_defs.md#urlstypedef) 
2. See [:material-code-braces: UrlsOutputTypeDef](./type_defs.md#urlsoutputtypedef) 

## DatabaseConfigurationUnionTypeDef

```python
# DatabaseConfigurationUnionTypeDef definition

DatabaseConfigurationUnionTypeDef = Union[
    DatabaseConfigurationTypeDef,  # (1)
    DatabaseConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DatabaseConfigurationTypeDef](./type_defs.md#databaseconfigurationtypedef) 
2. See [:material-code-braces: DatabaseConfigurationOutputTypeDef](./type_defs.md#databaseconfigurationoutputtypedef) 

## SalesforceKnowledgeArticleConfigurationUnionTypeDef

```python
# SalesforceKnowledgeArticleConfigurationUnionTypeDef definition

SalesforceKnowledgeArticleConfigurationUnionTypeDef = Union[
    SalesforceKnowledgeArticleConfigurationTypeDef,  # (1)
    SalesforceKnowledgeArticleConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceKnowledgeArticleConfigurationTypeDef](./type_defs.md#salesforceknowledgearticleconfigurationtypedef) 
2. See [:material-code-braces: SalesforceKnowledgeArticleConfigurationOutputTypeDef](./type_defs.md#salesforceknowledgearticleconfigurationoutputtypedef) 

## ServiceNowConfigurationUnionTypeDef

```python
# ServiceNowConfigurationUnionTypeDef definition

ServiceNowConfigurationUnionTypeDef = Union[
    ServiceNowConfigurationTypeDef,  # (1)
    ServiceNowConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServiceNowConfigurationTypeDef](./type_defs.md#servicenowconfigurationtypedef) 
2. See [:material-code-braces: ServiceNowConfigurationOutputTypeDef](./type_defs.md#servicenowconfigurationoutputtypedef) 

## OneDriveConfigurationUnionTypeDef

```python
# OneDriveConfigurationUnionTypeDef definition

OneDriveConfigurationUnionTypeDef = Union[
    OneDriveConfigurationTypeDef,  # (1)
    OneDriveConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OneDriveConfigurationTypeDef](./type_defs.md#onedriveconfigurationtypedef) 
2. See [:material-code-braces: OneDriveConfigurationOutputTypeDef](./type_defs.md#onedriveconfigurationoutputtypedef) 

## DocumentAttributeConditionUnionTypeDef

```python
# DocumentAttributeConditionUnionTypeDef definition

DocumentAttributeConditionUnionTypeDef = Union[
    DocumentAttributeConditionTypeDef,  # (1)
    DocumentAttributeConditionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef) 
2. See [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 

## DocumentAttributeTargetUnionTypeDef

```python
# DocumentAttributeTargetUnionTypeDef definition

DocumentAttributeTargetUnionTypeDef = Union[
    DocumentAttributeTargetTypeDef,  # (1)
    DocumentAttributeTargetOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeTargetTypeDef](./type_defs.md#documentattributetargettypedef) 
2. See [:material-code-braces: DocumentAttributeTargetOutputTypeDef](./type_defs.md#documentattributetargetoutputtypedef) 

## DocumentAttributeUnionTypeDef

```python
# DocumentAttributeUnionTypeDef definition

DocumentAttributeUnionTypeDef = Union[
    DocumentAttributeTypeDef,  # (1)
    DocumentAttributeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) 
2. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 

## ConfluenceConfigurationUnionTypeDef

```python
# ConfluenceConfigurationUnionTypeDef definition

ConfluenceConfigurationUnionTypeDef = Union[
    ConfluenceConfigurationTypeDef,  # (1)
    ConfluenceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfluenceConfigurationTypeDef](./type_defs.md#confluenceconfigurationtypedef) 
2. See [:material-code-braces: ConfluenceConfigurationOutputTypeDef](./type_defs.md#confluenceconfigurationoutputtypedef) 

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

## SalesforceConfigurationUnionTypeDef

```python
# SalesforceConfigurationUnionTypeDef definition

SalesforceConfigurationUnionTypeDef = Union[
    SalesforceConfigurationTypeDef,  # (1)
    SalesforceConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: SalesforceConfigurationTypeDef](./type_defs.md#salesforceconfigurationtypedef) 
2. See [:material-code-braces: SalesforceConfigurationOutputTypeDef](./type_defs.md#salesforceconfigurationoutputtypedef) 

## HookConfigurationUnionTypeDef

```python
# HookConfigurationUnionTypeDef definition

HookConfigurationUnionTypeDef = Union[
    HookConfigurationTypeDef,  # (1)
    HookConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef) 
2. See [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 

## InlineCustomDocumentEnrichmentConfigurationUnionTypeDef

```python
# InlineCustomDocumentEnrichmentConfigurationUnionTypeDef definition

InlineCustomDocumentEnrichmentConfigurationUnionTypeDef = Union[
    InlineCustomDocumentEnrichmentConfigurationTypeDef,  # (1)
    InlineCustomDocumentEnrichmentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InlineCustomDocumentEnrichmentConfigurationTypeDef](./type_defs.md#inlinecustomdocumentenrichmentconfigurationtypedef) 
2. See [:material-code-braces: InlineCustomDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#inlinecustomdocumentenrichmentconfigurationoutputtypedef) 



## AccessControlConfigurationSummaryTypeDef

```python
# AccessControlConfigurationSummaryTypeDef definition

class AccessControlConfigurationSummaryTypeDef(TypedDict):
    Id: str,
```

## AccessControlListConfigurationTypeDef

```python
# AccessControlListConfigurationTypeDef definition

class AccessControlListConfigurationTypeDef(TypedDict):
    KeyPath: NotRequired[str],
```

## AclConfigurationTypeDef

```python
# AclConfigurationTypeDef definition

class AclConfigurationTypeDef(TypedDict):
    AllowedGroupsColumnName: str,
```

## DataSourceToIndexFieldMappingTypeDef

```python
# DataSourceToIndexFieldMappingTypeDef definition

class DataSourceToIndexFieldMappingTypeDef(TypedDict):
    DataSourceFieldName: str,
    IndexFieldName: str,
    DateFieldFormat: NotRequired[str],
```

## DataSourceVpcConfigurationOutputTypeDef

```python
# DataSourceVpcConfigurationOutputTypeDef definition

class DataSourceVpcConfigurationOutputTypeDef(TypedDict):
    SubnetIds: List[str],
    SecurityGroupIds: List[str],
```

## S3PathTypeDef

```python
# S3PathTypeDef definition

class S3PathTypeDef(TypedDict):
    Bucket: str,
    Key: str,
```

## EntityConfigurationTypeDef

```python
# EntityConfigurationTypeDef definition

class EntityConfigurationTypeDef(TypedDict):
    EntityId: str,
    EntityType: EntityTypeType,  # (1)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
## FailedEntityTypeDef

```python
# FailedEntityTypeDef definition

class FailedEntityTypeDef(TypedDict):
    EntityId: NotRequired[str],
    ErrorMessage: NotRequired[str],
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

## EntityPersonaConfigurationTypeDef

```python
# EntityPersonaConfigurationTypeDef definition

class EntityPersonaConfigurationTypeDef(TypedDict):
    EntityId: str,
    Persona: PersonaType,  # (1)
```

1. See [:material-code-brackets: PersonaType](./literals.md#personatype) 
## SuggestableConfigTypeDef

```python
# SuggestableConfigTypeDef definition

class SuggestableConfigTypeDef(TypedDict):
    AttributeName: NotRequired[str],
    Suggestable: NotRequired[bool],
```

## BasicAuthenticationConfigurationTypeDef

```python
# BasicAuthenticationConfigurationTypeDef definition

class BasicAuthenticationConfigurationTypeDef(TypedDict):
    Host: str,
    Port: int,
    Credentials: str,
```

## DataSourceSyncJobMetricTargetTypeDef

```python
# DataSourceSyncJobMetricTargetTypeDef definition

class DataSourceSyncJobMetricTargetTypeDef(TypedDict):
    DataSourceId: str,
    DataSourceSyncJobId: NotRequired[str],
```

## BatchDeleteDocumentResponseFailedDocumentTypeDef

```python
# BatchDeleteDocumentResponseFailedDocumentTypeDef definition

class BatchDeleteDocumentResponseFailedDocumentTypeDef(TypedDict):
    Id: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## BatchDeleteFeaturedResultsSetErrorTypeDef

```python
# BatchDeleteFeaturedResultsSetErrorTypeDef definition

class BatchDeleteFeaturedResultsSetErrorTypeDef(TypedDict):
    Id: str,
    ErrorCode: ErrorCodeType,  # (1)
    ErrorMessage: str,
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## BatchDeleteFeaturedResultsSetRequestRequestTypeDef

```python
# BatchDeleteFeaturedResultsSetRequestRequestTypeDef definition

class BatchDeleteFeaturedResultsSetRequestRequestTypeDef(TypedDict):
    IndexId: str,
    FeaturedResultsSetIds: Sequence[str],
```

## BatchGetDocumentStatusResponseErrorTypeDef

```python
# BatchGetDocumentStatusResponseErrorTypeDef definition

class BatchGetDocumentStatusResponseErrorTypeDef(TypedDict):
    DocumentId: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## StatusTypeDef

```python
# StatusTypeDef definition

class StatusTypeDef(TypedDict):
    DocumentId: NotRequired[str],
    DocumentStatus: NotRequired[DocumentStatusType],  # (1)
    FailureCode: NotRequired[str],
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: DocumentStatusType](./literals.md#documentstatustype) 
## BatchPutDocumentResponseFailedDocumentTypeDef

```python
# BatchPutDocumentResponseFailedDocumentTypeDef definition

class BatchPutDocumentResponseFailedDocumentTypeDef(TypedDict):
    Id: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
## CapacityUnitsConfigurationTypeDef

```python
# CapacityUnitsConfigurationTypeDef definition

class CapacityUnitsConfigurationTypeDef(TypedDict):
    StorageCapacityUnits: int,
    QueryCapacityUnits: int,
```

## ClearQuerySuggestionsRequestRequestTypeDef

```python
# ClearQuerySuggestionsRequestRequestTypeDef definition

class ClearQuerySuggestionsRequestRequestTypeDef(TypedDict):
    IndexId: str,
```

## ExpandConfigurationTypeDef

```python
# ExpandConfigurationTypeDef definition

class ExpandConfigurationTypeDef(TypedDict):
    MaxResultItemsToExpand: NotRequired[int],
    MaxExpandedResultsPerItem: NotRequired[int],
```

## SortingConfigurationTypeDef

```python
# SortingConfigurationTypeDef definition

class SortingConfigurationTypeDef(TypedDict):
    DocumentAttributeKey: str,
    SortOrder: SortOrderType,  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ConfluenceAttachmentToIndexFieldMappingTypeDef

```python
# ConfluenceAttachmentToIndexFieldMappingTypeDef definition

class ConfluenceAttachmentToIndexFieldMappingTypeDef(TypedDict):
    DataSourceFieldName: NotRequired[ConfluenceAttachmentFieldNameType],  # (1)
    DateFieldFormat: NotRequired[str],
    IndexFieldName: NotRequired[str],
```

1. See [:material-code-brackets: ConfluenceAttachmentFieldNameType](./literals.md#confluenceattachmentfieldnametype) 
## ConfluenceBlogToIndexFieldMappingTypeDef

```python
# ConfluenceBlogToIndexFieldMappingTypeDef definition

class ConfluenceBlogToIndexFieldMappingTypeDef(TypedDict):
    DataSourceFieldName: NotRequired[ConfluenceBlogFieldNameType],  # (1)
    DateFieldFormat: NotRequired[str],
    IndexFieldName: NotRequired[str],
```

1. See [:material-code-brackets: ConfluenceBlogFieldNameType](./literals.md#confluenceblogfieldnametype) 
## ProxyConfigurationTypeDef

```python
# ProxyConfigurationTypeDef definition

class ProxyConfigurationTypeDef(TypedDict):
    Host: str,
    Port: int,
    Credentials: NotRequired[str],
```

## ConfluencePageToIndexFieldMappingTypeDef

```python
# ConfluencePageToIndexFieldMappingTypeDef definition

class ConfluencePageToIndexFieldMappingTypeDef(TypedDict):
    DataSourceFieldName: NotRequired[ConfluencePageFieldNameType],  # (1)
    DateFieldFormat: NotRequired[str],
    IndexFieldName: NotRequired[str],
```

1. See [:material-code-brackets: ConfluencePageFieldNameType](./literals.md#confluencepagefieldnametype) 
## ConfluenceSpaceToIndexFieldMappingTypeDef

```python
# ConfluenceSpaceToIndexFieldMappingTypeDef definition

class ConfluenceSpaceToIndexFieldMappingTypeDef(TypedDict):
    DataSourceFieldName: NotRequired[ConfluenceSpaceFieldNameType],  # (1)
    DateFieldFormat: NotRequired[str],
    IndexFieldName: NotRequired[str],
```

1. See [:material-code-brackets: ConfluenceSpaceFieldNameType](./literals.md#confluencespacefieldnametype) 
## ConnectionConfigurationTypeDef

```python
# ConnectionConfigurationTypeDef definition

class ConnectionConfigurationTypeDef(TypedDict):
    DatabaseHost: str,
    DatabasePort: int,
    DatabaseName: str,
    TableName: str,
    SecretArn: str,
```

## ContentSourceConfigurationOutputTypeDef

```python
# ContentSourceConfigurationOutputTypeDef definition

class ContentSourceConfigurationOutputTypeDef(TypedDict):
    DataSourceIds: NotRequired[List[str]],
    FaqIds: NotRequired[List[str]],
    DirectPutContent: NotRequired[bool],
```

## ContentSourceConfigurationTypeDef

```python
# ContentSourceConfigurationTypeDef definition

class ContentSourceConfigurationTypeDef(TypedDict):
    DataSourceIds: NotRequired[Sequence[str]],
    FaqIds: NotRequired[Sequence[str]],
    DirectPutContent: NotRequired[bool],
```

## CorrectionTypeDef

```python
# CorrectionTypeDef definition

class CorrectionTypeDef(TypedDict):
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
    Term: NotRequired[str],
    CorrectedTerm: NotRequired[str],
```

## PrincipalTypeDef

```python
# PrincipalTypeDef definition

class PrincipalTypeDef(TypedDict):
    Name: str,
    Type: PrincipalTypeType,  # (1)
    Access: ReadAccessTypeType,  # (2)
    DataSourceId: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
2. See [:material-code-brackets: ReadAccessTypeType](./literals.md#readaccesstypetype) 
## DataSourceVpcConfigurationTypeDef

```python
# DataSourceVpcConfigurationTypeDef definition

class DataSourceVpcConfigurationTypeDef(TypedDict):
    SubnetIds: Sequence[str],
    SecurityGroupIds: Sequence[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## FeaturedDocumentTypeDef

```python
# FeaturedDocumentTypeDef definition

class FeaturedDocumentTypeDef(TypedDict):
    Id: NotRequired[str],
```

## ServerSideEncryptionConfigurationTypeDef

```python
# ServerSideEncryptionConfigurationTypeDef definition

class ServerSideEncryptionConfigurationTypeDef(TypedDict):
    KmsKeyId: NotRequired[str],
```

## UserGroupResolutionConfigurationTypeDef

```python
# UserGroupResolutionConfigurationTypeDef definition

class UserGroupResolutionConfigurationTypeDef(TypedDict):
    UserGroupResolutionMode: UserGroupResolutionModeType,  # (1)
```

1. See [:material-code-brackets: UserGroupResolutionModeType](./literals.md#usergroupresolutionmodetype) 
## TemplateConfigurationOutputTypeDef

```python
# TemplateConfigurationOutputTypeDef definition

class TemplateConfigurationOutputTypeDef(TypedDict):
    Template: NotRequired[Dict[str, Any]],
```

## DataSourceGroupTypeDef

```python
# DataSourceGroupTypeDef definition

class DataSourceGroupTypeDef(TypedDict):
    GroupId: str,
    DataSourceId: str,
```

## DataSourceSummaryTypeDef

```python
# DataSourceSummaryTypeDef definition

class DataSourceSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    Type: NotRequired[DataSourceTypeType],  # (1)
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
    Status: NotRequired[DataSourceStatusType],  # (2)
    LanguageCode: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## DataSourceSyncJobMetricsTypeDef

```python
# DataSourceSyncJobMetricsTypeDef definition

class DataSourceSyncJobMetricsTypeDef(TypedDict):
    DocumentsAdded: NotRequired[str],
    DocumentsModified: NotRequired[str],
    DocumentsDeleted: NotRequired[str],
    DocumentsFailed: NotRequired[str],
    DocumentsScanned: NotRequired[str],
```

## SqlConfigurationTypeDef

```python
# SqlConfigurationTypeDef definition

class SqlConfigurationTypeDef(TypedDict):
    QueryIdentifiersEnclosingOption: NotRequired[QueryIdentifiersEnclosingOptionType],  # (1)
```

1. See [:material-code-brackets: QueryIdentifiersEnclosingOptionType](./literals.md#queryidentifiersenclosingoptiontype) 
## DeleteAccessControlConfigurationRequestRequestTypeDef

```python
# DeleteAccessControlConfigurationRequestRequestTypeDef definition

class DeleteAccessControlConfigurationRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Id: str,
```

## DeleteDataSourceRequestRequestTypeDef

```python
# DeleteDataSourceRequestRequestTypeDef definition

class DeleteDataSourceRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## DeleteExperienceRequestRequestTypeDef

```python
# DeleteExperienceRequestRequestTypeDef definition

class DeleteExperienceRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## DeleteFaqRequestRequestTypeDef

```python
# DeleteFaqRequestRequestTypeDef definition

class DeleteFaqRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## DeleteIndexRequestRequestTypeDef

```python
# DeleteIndexRequestRequestTypeDef definition

class DeleteIndexRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DeletePrincipalMappingRequestRequestTypeDef

```python
# DeletePrincipalMappingRequestRequestTypeDef definition

class DeletePrincipalMappingRequestRequestTypeDef(TypedDict):
    IndexId: str,
    GroupId: str,
    DataSourceId: NotRequired[str],
    OrderingId: NotRequired[int],
```

## DeleteQuerySuggestionsBlockListRequestRequestTypeDef

```python
# DeleteQuerySuggestionsBlockListRequestRequestTypeDef definition

class DeleteQuerySuggestionsBlockListRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Id: str,
```

## DeleteThesaurusRequestRequestTypeDef

```python
# DeleteThesaurusRequestRequestTypeDef definition

class DeleteThesaurusRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## DescribeAccessControlConfigurationRequestRequestTypeDef

```python
# DescribeAccessControlConfigurationRequestRequestTypeDef definition

class DescribeAccessControlConfigurationRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Id: str,
```

## DescribeDataSourceRequestRequestTypeDef

```python
# DescribeDataSourceRequestRequestTypeDef definition

class DescribeDataSourceRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## DescribeExperienceRequestRequestTypeDef

```python
# DescribeExperienceRequestRequestTypeDef definition

class DescribeExperienceRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## ExperienceEndpointTypeDef

```python
# ExperienceEndpointTypeDef definition

class ExperienceEndpointTypeDef(TypedDict):
    EndpointType: NotRequired[EndpointTypeType],  # (1)
    Endpoint: NotRequired[str],
```

1. See [:material-code-brackets: EndpointTypeType](./literals.md#endpointtypetype) 
## DescribeFaqRequestRequestTypeDef

```python
# DescribeFaqRequestRequestTypeDef definition

class DescribeFaqRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## DescribeFeaturedResultsSetRequestRequestTypeDef

```python
# DescribeFeaturedResultsSetRequestRequestTypeDef definition

class DescribeFeaturedResultsSetRequestRequestTypeDef(TypedDict):
    IndexId: str,
    FeaturedResultsSetId: str,
```

## FeaturedDocumentMissingTypeDef

```python
# FeaturedDocumentMissingTypeDef definition

class FeaturedDocumentMissingTypeDef(TypedDict):
    Id: NotRequired[str],
```

## FeaturedDocumentWithMetadataTypeDef

```python
# FeaturedDocumentWithMetadataTypeDef definition

class FeaturedDocumentWithMetadataTypeDef(TypedDict):
    Id: NotRequired[str],
    Title: NotRequired[str],
    URI: NotRequired[str],
```

## DescribeIndexRequestRequestTypeDef

```python
# DescribeIndexRequestRequestTypeDef definition

class DescribeIndexRequestRequestTypeDef(TypedDict):
    Id: str,
```

## DescribePrincipalMappingRequestRequestTypeDef

```python
# DescribePrincipalMappingRequestRequestTypeDef definition

class DescribePrincipalMappingRequestRequestTypeDef(TypedDict):
    IndexId: str,
    GroupId: str,
    DataSourceId: NotRequired[str],
```

## GroupOrderingIdSummaryTypeDef

```python
# GroupOrderingIdSummaryTypeDef definition

class GroupOrderingIdSummaryTypeDef(TypedDict):
    Status: NotRequired[PrincipalMappingStatusType],  # (1)
    LastUpdatedAt: NotRequired[datetime],
    ReceivedAt: NotRequired[datetime],
    OrderingId: NotRequired[int],
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalMappingStatusType](./literals.md#principalmappingstatustype) 
## DescribeQuerySuggestionsBlockListRequestRequestTypeDef

```python
# DescribeQuerySuggestionsBlockListRequestRequestTypeDef definition

class DescribeQuerySuggestionsBlockListRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Id: str,
```

## DescribeQuerySuggestionsConfigRequestRequestTypeDef

```python
# DescribeQuerySuggestionsConfigRequestRequestTypeDef definition

class DescribeQuerySuggestionsConfigRequestRequestTypeDef(TypedDict):
    IndexId: str,
```

## DescribeThesaurusRequestRequestTypeDef

```python
# DescribeThesaurusRequestRequestTypeDef definition

class DescribeThesaurusRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## DisassociatePersonasFromEntitiesRequestRequestTypeDef

```python
# DisassociatePersonasFromEntitiesRequestRequestTypeDef definition

class DisassociatePersonasFromEntitiesRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    EntityIds: Sequence[str],
```

## DocumentAttributeValueOutputTypeDef

```python
# DocumentAttributeValueOutputTypeDef definition

class DocumentAttributeValueOutputTypeDef(TypedDict):
    StringValue: NotRequired[str],
    StringListValue: NotRequired[List[str]],
    LongValue: NotRequired[int],
    DateValue: NotRequired[datetime],
```

## RelevanceOutputTypeDef

```python
# RelevanceOutputTypeDef definition

class RelevanceOutputTypeDef(TypedDict):
    Freshness: NotRequired[bool],
    Importance: NotRequired[int],
    Duration: NotRequired[str],
    RankOrder: NotRequired[OrderType],  # (1)
    ValueImportanceMap: NotRequired[Dict[str, int]],
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## SearchTypeDef

```python
# SearchTypeDef definition

class SearchTypeDef(TypedDict):
    Facetable: NotRequired[bool],
    Searchable: NotRequired[bool],
    Displayable: NotRequired[bool],
    Sortable: NotRequired[bool],
```

## DocumentsMetadataConfigurationTypeDef

```python
# DocumentsMetadataConfigurationTypeDef definition

class DocumentsMetadataConfigurationTypeDef(TypedDict):
    S3Prefix: NotRequired[str],
```

## EntityDisplayDataTypeDef

```python
# EntityDisplayDataTypeDef definition

class EntityDisplayDataTypeDef(TypedDict):
    UserName: NotRequired[str],
    GroupName: NotRequired[str],
    IdentifiedUserName: NotRequired[str],
    FirstName: NotRequired[str],
    LastName: NotRequired[str],
```

## UserIdentityConfigurationTypeDef

```python
# UserIdentityConfigurationTypeDef definition

class UserIdentityConfigurationTypeDef(TypedDict):
    IdentityAttributeName: NotRequired[str],
```

## FacetTypeDef

```python
# FacetTypeDef definition

class FacetTypeDef(TypedDict):
    DocumentAttributeKey: NotRequired[str],
    Facets: NotRequired[Sequence[Mapping[str, Any]]],
    MaxResults: NotRequired[int],
```

## FaqStatisticsTypeDef

```python
# FaqStatisticsTypeDef definition

class FaqStatisticsTypeDef(TypedDict):
    IndexedQuestionAnswersCount: int,
```

## FaqSummaryTypeDef

```python
# FaqSummaryTypeDef definition

class FaqSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[FaqStatusType],  # (1)
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
    FileFormat: NotRequired[FaqFileFormatType],  # (2)
    LanguageCode: NotRequired[str],
```

1. See [:material-code-brackets: FaqStatusType](./literals.md#faqstatustype) 
2. See [:material-code-brackets: FaqFileFormatType](./literals.md#faqfileformattype) 
## FeaturedResultsSetSummaryTypeDef

```python
# FeaturedResultsSetSummaryTypeDef definition

class FeaturedResultsSetSummaryTypeDef(TypedDict):
    FeaturedResultsSetId: NotRequired[str],
    FeaturedResultsSetName: NotRequired[str],
    Status: NotRequired[FeaturedResultsSetStatusType],  # (1)
    LastUpdatedTimestamp: NotRequired[int],
    CreationTimestamp: NotRequired[int],
```

1. See [:material-code-brackets: FeaturedResultsSetStatusType](./literals.md#featuredresultssetstatustype) 
## GetSnapshotsRequestRequestTypeDef

```python
# GetSnapshotsRequestRequestTypeDef definition

class GetSnapshotsRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Interval: IntervalType,  # (1)
    MetricType: MetricTypeType,  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: IntervalType](./literals.md#intervaltype) 
2. See [:material-code-brackets: MetricTypeType](./literals.md#metrictypetype) 
## TimeRangeOutputTypeDef

```python
# TimeRangeOutputTypeDef definition

class TimeRangeOutputTypeDef(TypedDict):
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

## GitHubDocumentCrawlPropertiesTypeDef

```python
# GitHubDocumentCrawlPropertiesTypeDef definition

class GitHubDocumentCrawlPropertiesTypeDef(TypedDict):
    CrawlRepositoryDocuments: NotRequired[bool],
    CrawlIssue: NotRequired[bool],
    CrawlIssueComment: NotRequired[bool],
    CrawlIssueCommentAttachment: NotRequired[bool],
    CrawlPullRequest: NotRequired[bool],
    CrawlPullRequestComment: NotRequired[bool],
    CrawlPullRequestCommentAttachment: NotRequired[bool],
```

## SaaSConfigurationTypeDef

```python
# SaaSConfigurationTypeDef definition

class SaaSConfigurationTypeDef(TypedDict):
    OrganizationName: str,
    HostUrl: str,
```

## MemberGroupTypeDef

```python
# MemberGroupTypeDef definition

class MemberGroupTypeDef(TypedDict):
    GroupId: str,
    DataSourceId: NotRequired[str],
```

## MemberUserTypeDef

```python
# MemberUserTypeDef definition

class MemberUserTypeDef(TypedDict):
    UserId: str,
```

## GroupSummaryTypeDef

```python
# GroupSummaryTypeDef definition

class GroupSummaryTypeDef(TypedDict):
    GroupId: NotRequired[str],
    OrderingId: NotRequired[int],
```

## HighlightTypeDef

```python
# HighlightTypeDef definition

class HighlightTypeDef(TypedDict):
    BeginOffset: int,
    EndOffset: int,
    TopAnswer: NotRequired[bool],
    Type: NotRequired[HighlightTypeType],  # (1)
```

1. See [:material-code-brackets: HighlightTypeType](./literals.md#highlighttypetype) 
## IndexConfigurationSummaryTypeDef

```python
# IndexConfigurationSummaryTypeDef definition

class IndexConfigurationSummaryTypeDef(TypedDict):
    CreatedAt: datetime,
    UpdatedAt: datetime,
    Status: IndexStatusType,  # (2)
    Name: NotRequired[str],
    Id: NotRequired[str],
    Edition: NotRequired[IndexEditionType],  # (1)
```

1. See [:material-code-brackets: IndexEditionType](./literals.md#indexeditiontype) 
2. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
## TextDocumentStatisticsTypeDef

```python
# TextDocumentStatisticsTypeDef definition

class TextDocumentStatisticsTypeDef(TypedDict):
    IndexedTextDocumentsCount: int,
    IndexedTextBytes: int,
```

## JsonTokenTypeConfigurationTypeDef

```python
# JsonTokenTypeConfigurationTypeDef definition

class JsonTokenTypeConfigurationTypeDef(TypedDict):
    UserNameAttributeField: str,
    GroupAttributeField: str,
```

## JwtTokenTypeConfigurationTypeDef

```python
# JwtTokenTypeConfigurationTypeDef definition

class JwtTokenTypeConfigurationTypeDef(TypedDict):
    KeyLocation: KeyLocationType,  # (1)
    URL: NotRequired[str],
    SecretManagerArn: NotRequired[str],
    UserNameAttributeField: NotRequired[str],
    GroupAttributeField: NotRequired[str],
    Issuer: NotRequired[str],
    ClaimRegex: NotRequired[str],
```

1. See [:material-code-brackets: KeyLocationType](./literals.md#keylocationtype) 
## ListAccessControlConfigurationsRequestRequestTypeDef

```python
# ListAccessControlConfigurationsRequestRequestTypeDef definition

class ListAccessControlConfigurationsRequestRequestTypeDef(TypedDict):
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDataSourcesRequestRequestTypeDef

```python
# ListDataSourcesRequestRequestTypeDef definition

class ListDataSourcesRequestRequestTypeDef(TypedDict):
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListEntityPersonasRequestRequestTypeDef

```python
# ListEntityPersonasRequestRequestTypeDef definition

class ListEntityPersonasRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PersonasSummaryTypeDef

```python
# PersonasSummaryTypeDef definition

class PersonasSummaryTypeDef(TypedDict):
    EntityId: NotRequired[str],
    Persona: NotRequired[PersonaType],  # (1)
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: PersonaType](./literals.md#personatype) 
## ListExperienceEntitiesRequestRequestTypeDef

```python
# ListExperienceEntitiesRequestRequestTypeDef definition

class ListExperienceEntitiesRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    NextToken: NotRequired[str],
```

## ListExperiencesRequestRequestTypeDef

```python
# ListExperiencesRequestRequestTypeDef definition

class ListExperiencesRequestRequestTypeDef(TypedDict):
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListFaqsRequestRequestTypeDef

```python
# ListFaqsRequestRequestTypeDef definition

class ListFaqsRequestRequestTypeDef(TypedDict):
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListFeaturedResultsSetsRequestRequestTypeDef

```python
# ListFeaturedResultsSetsRequestRequestTypeDef definition

class ListFeaturedResultsSetsRequestRequestTypeDef(TypedDict):
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListGroupsOlderThanOrderingIdRequestRequestTypeDef

```python
# ListGroupsOlderThanOrderingIdRequestRequestTypeDef definition

class ListGroupsOlderThanOrderingIdRequestRequestTypeDef(TypedDict):
    IndexId: str,
    OrderingId: int,
    DataSourceId: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListIndicesRequestRequestTypeDef

```python
# ListIndicesRequestRequestTypeDef definition

class ListIndicesRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListQuerySuggestionsBlockListsRequestRequestTypeDef

```python
# ListQuerySuggestionsBlockListsRequestRequestTypeDef definition

class ListQuerySuggestionsBlockListsRequestRequestTypeDef(TypedDict):
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## QuerySuggestionsBlockListSummaryTypeDef

```python
# QuerySuggestionsBlockListSummaryTypeDef definition

class QuerySuggestionsBlockListSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[QuerySuggestionsBlockListStatusType],  # (1)
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
    ItemCount: NotRequired[int],
```

1. See [:material-code-brackets: QuerySuggestionsBlockListStatusType](./literals.md#querysuggestionsblockliststatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## ListThesauriRequestRequestTypeDef

```python
# ListThesauriRequestRequestTypeDef definition

class ListThesauriRequestRequestTypeDef(TypedDict):
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ThesaurusSummaryTypeDef

```python
# ThesaurusSummaryTypeDef definition

class ThesaurusSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[ThesaurusStatusType],  # (1)
    CreatedAt: NotRequired[datetime],
    UpdatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: ThesaurusStatusType](./literals.md#thesaurusstatustype) 
## SpellCorrectionConfigurationTypeDef

```python
# SpellCorrectionConfigurationTypeDef definition

class SpellCorrectionConfigurationTypeDef(TypedDict):
    IncludeQuerySpellCheckSuggestions: bool,
```

## ScoreAttributesTypeDef

```python
# ScoreAttributesTypeDef definition

class ScoreAttributesTypeDef(TypedDict):
    ScoreConfidence: NotRequired[ScoreConfidenceType],  # (1)
```

1. See [:material-code-brackets: ScoreConfidenceType](./literals.md#scoreconfidencetype) 
## WarningTypeDef

```python
# WarningTypeDef definition

class WarningTypeDef(TypedDict):
    Message: NotRequired[str],
    Code: NotRequired[WarningCodeType],  # (1)
```

1. See [:material-code-brackets: WarningCodeType](./literals.md#warningcodetype) 
## RelevanceFeedbackTypeDef

```python
# RelevanceFeedbackTypeDef definition

class RelevanceFeedbackTypeDef(TypedDict):
    ResultId: str,
    RelevanceValue: RelevanceTypeType,  # (1)
```

1. See [:material-code-brackets: RelevanceTypeType](./literals.md#relevancetypetype) 
## RelevanceTypeDef

```python
# RelevanceTypeDef definition

class RelevanceTypeDef(TypedDict):
    Freshness: NotRequired[bool],
    Importance: NotRequired[int],
    Duration: NotRequired[str],
    RankOrder: NotRequired[OrderType],  # (1)
    ValueImportanceMap: NotRequired[Mapping[str, int]],
```

1. See [:material-code-brackets: OrderType](./literals.md#ordertype) 
## SeedUrlConfigurationOutputTypeDef

```python
# SeedUrlConfigurationOutputTypeDef definition

class SeedUrlConfigurationOutputTypeDef(TypedDict):
    SeedUrls: List[str],
    WebCrawlerMode: NotRequired[WebCrawlerModeType],  # (1)
```

1. See [:material-code-brackets: WebCrawlerModeType](./literals.md#webcrawlermodetype) 
## SeedUrlConfigurationTypeDef

```python
# SeedUrlConfigurationTypeDef definition

class SeedUrlConfigurationTypeDef(TypedDict):
    SeedUrls: Sequence[str],
    WebCrawlerMode: NotRequired[WebCrawlerModeType],  # (1)
```

1. See [:material-code-brackets: WebCrawlerModeType](./literals.md#webcrawlermodetype) 
## SiteMapsConfigurationOutputTypeDef

```python
# SiteMapsConfigurationOutputTypeDef definition

class SiteMapsConfigurationOutputTypeDef(TypedDict):
    SiteMaps: List[str],
```

## SiteMapsConfigurationTypeDef

```python
# SiteMapsConfigurationTypeDef definition

class SiteMapsConfigurationTypeDef(TypedDict):
    SiteMaps: Sequence[str],
```

## StartDataSourceSyncJobRequestRequestTypeDef

```python
# StartDataSourceSyncJobRequestRequestTypeDef definition

class StartDataSourceSyncJobRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## StopDataSourceSyncJobRequestRequestTypeDef

```python
# StopDataSourceSyncJobRequestRequestTypeDef definition

class StopDataSourceSyncJobRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
```

## SuggestionHighlightTypeDef

```python
# SuggestionHighlightTypeDef definition

class SuggestionHighlightTypeDef(TypedDict):
    BeginOffset: NotRequired[int],
    EndOffset: NotRequired[int],
```

## TableCellTypeDef

```python
# TableCellTypeDef definition

class TableCellTypeDef(TypedDict):
    Value: NotRequired[str],
    TopAnswer: NotRequired[bool],
    Highlighted: NotRequired[bool],
    Header: NotRequired[bool],
```

## TemplateConfigurationTypeDef

```python
# TemplateConfigurationTypeDef definition

class TemplateConfigurationTypeDef(TypedDict):
    Template: NotRequired[Mapping[str, Any]],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## ColumnConfigurationOutputTypeDef

```python
# ColumnConfigurationOutputTypeDef definition

class ColumnConfigurationOutputTypeDef(TypedDict):
    DocumentIdColumnName: str,
    DocumentDataColumnName: str,
    ChangeDetectingColumns: List[str],
    DocumentTitleColumnName: NotRequired[str],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## ColumnConfigurationTypeDef

```python
# ColumnConfigurationTypeDef definition

class ColumnConfigurationTypeDef(TypedDict):
    DocumentIdColumnName: str,
    DocumentDataColumnName: str,
    ChangeDetectingColumns: Sequence[str],
    DocumentTitleColumnName: NotRequired[str],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## GoogleDriveConfigurationOutputTypeDef

```python
# GoogleDriveConfigurationOutputTypeDef definition

class GoogleDriveConfigurationOutputTypeDef(TypedDict):
    SecretArn: str,
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    ExcludeMimeTypes: NotRequired[List[str]],
    ExcludeUserAccounts: NotRequired[List[str]],
    ExcludeSharedDrives: NotRequired[List[str]],
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## GoogleDriveConfigurationTypeDef

```python
# GoogleDriveConfigurationTypeDef definition

class GoogleDriveConfigurationTypeDef(TypedDict):
    SecretArn: str,
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    ExcludeMimeTypes: NotRequired[Sequence[str]],
    ExcludeUserAccounts: NotRequired[Sequence[str]],
    ExcludeSharedDrives: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## SalesforceChatterFeedConfigurationOutputTypeDef

```python
# SalesforceChatterFeedConfigurationOutputTypeDef definition

class SalesforceChatterFeedConfigurationOutputTypeDef(TypedDict):
    DocumentDataFieldName: str,
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    IncludeFilterTypes: NotRequired[List[SalesforceChatterFeedIncludeFilterTypeType]],  # (2)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
2. See [:material-code-brackets: SalesforceChatterFeedIncludeFilterTypeType](./literals.md#salesforcechatterfeedincludefiltertypetype) 
## SalesforceChatterFeedConfigurationTypeDef

```python
# SalesforceChatterFeedConfigurationTypeDef definition

class SalesforceChatterFeedConfigurationTypeDef(TypedDict):
    DocumentDataFieldName: str,
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    IncludeFilterTypes: NotRequired[Sequence[SalesforceChatterFeedIncludeFilterTypeType]],  # (2)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
2. See [:material-code-brackets: SalesforceChatterFeedIncludeFilterTypeType](./literals.md#salesforcechatterfeedincludefiltertypetype) 
## SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef

```python
# SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef definition

class SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef(TypedDict):
    Name: str,
    DocumentDataFieldName: str,
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef

```python
# SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef definition

class SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef(TypedDict):
    Name: str,
    DocumentDataFieldName: str,
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef

```python
# SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef definition

class SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef(TypedDict):
    DocumentDataFieldName: str,
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef

```python
# SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef definition

class SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef(TypedDict):
    DocumentDataFieldName: str,
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## SalesforceStandardObjectAttachmentConfigurationOutputTypeDef

```python
# SalesforceStandardObjectAttachmentConfigurationOutputTypeDef definition

class SalesforceStandardObjectAttachmentConfigurationOutputTypeDef(TypedDict):
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## SalesforceStandardObjectAttachmentConfigurationTypeDef

```python
# SalesforceStandardObjectAttachmentConfigurationTypeDef definition

class SalesforceStandardObjectAttachmentConfigurationTypeDef(TypedDict):
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## SalesforceStandardObjectConfigurationOutputTypeDef

```python
# SalesforceStandardObjectConfigurationOutputTypeDef definition

class SalesforceStandardObjectConfigurationOutputTypeDef(TypedDict):
    Name: SalesforceStandardObjectNameType,  # (1)
    DocumentDataFieldName: str,
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (2)
```

1. See [:material-code-brackets: SalesforceStandardObjectNameType](./literals.md#salesforcestandardobjectnametype) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## SalesforceStandardObjectConfigurationTypeDef

```python
# SalesforceStandardObjectConfigurationTypeDef definition

class SalesforceStandardObjectConfigurationTypeDef(TypedDict):
    Name: SalesforceStandardObjectNameType,  # (1)
    DocumentDataFieldName: str,
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (2)
```

1. See [:material-code-brackets: SalesforceStandardObjectNameType](./literals.md#salesforcestandardobjectnametype) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## ServiceNowKnowledgeArticleConfigurationOutputTypeDef

```python
# ServiceNowKnowledgeArticleConfigurationOutputTypeDef definition

class ServiceNowKnowledgeArticleConfigurationOutputTypeDef(TypedDict):
    DocumentDataFieldName: str,
    CrawlAttachments: NotRequired[bool],
    IncludeAttachmentFilePatterns: NotRequired[List[str]],
    ExcludeAttachmentFilePatterns: NotRequired[List[str]],
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    FilterQuery: NotRequired[str],
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## ServiceNowKnowledgeArticleConfigurationTypeDef

```python
# ServiceNowKnowledgeArticleConfigurationTypeDef definition

class ServiceNowKnowledgeArticleConfigurationTypeDef(TypedDict):
    DocumentDataFieldName: str,
    CrawlAttachments: NotRequired[bool],
    IncludeAttachmentFilePatterns: NotRequired[Sequence[str]],
    ExcludeAttachmentFilePatterns: NotRequired[Sequence[str]],
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    FilterQuery: NotRequired[str],
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## ServiceNowServiceCatalogConfigurationOutputTypeDef

```python
# ServiceNowServiceCatalogConfigurationOutputTypeDef definition

class ServiceNowServiceCatalogConfigurationOutputTypeDef(TypedDict):
    DocumentDataFieldName: str,
    CrawlAttachments: NotRequired[bool],
    IncludeAttachmentFilePatterns: NotRequired[List[str]],
    ExcludeAttachmentFilePatterns: NotRequired[List[str]],
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## ServiceNowServiceCatalogConfigurationTypeDef

```python
# ServiceNowServiceCatalogConfigurationTypeDef definition

class ServiceNowServiceCatalogConfigurationTypeDef(TypedDict):
    DocumentDataFieldName: str,
    CrawlAttachments: NotRequired[bool],
    IncludeAttachmentFilePatterns: NotRequired[Sequence[str]],
    ExcludeAttachmentFilePatterns: NotRequired[Sequence[str]],
    DocumentTitleFieldName: NotRequired[str],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## WorkDocsConfigurationOutputTypeDef

```python
# WorkDocsConfigurationOutputTypeDef definition

class WorkDocsConfigurationOutputTypeDef(TypedDict):
    OrganizationId: str,
    CrawlComments: NotRequired[bool],
    UseChangeLog: NotRequired[bool],
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## WorkDocsConfigurationTypeDef

```python
# WorkDocsConfigurationTypeDef definition

class WorkDocsConfigurationTypeDef(TypedDict):
    OrganizationId: str,
    CrawlComments: NotRequired[bool],
    UseChangeLog: NotRequired[bool],
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## BoxConfigurationOutputTypeDef

```python
# BoxConfigurationOutputTypeDef definition

class BoxConfigurationOutputTypeDef(TypedDict):
    EnterpriseId: str,
    SecretArn: str,
    UseChangeLog: NotRequired[bool],
    CrawlComments: NotRequired[bool],
    CrawlTasks: NotRequired[bool],
    CrawlWebLinks: NotRequired[bool],
    FileFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    TaskFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    CommentFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    WebLinkFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (5)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
5. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
## FsxConfigurationOutputTypeDef

```python
# FsxConfigurationOutputTypeDef definition

class FsxConfigurationOutputTypeDef(TypedDict):
    FileSystemId: str,
    FileSystemType: FsxFileSystemTypeType,  # (1)
    VpcConfiguration: DataSourceVpcConfigurationOutputTypeDef,  # (2)
    SecretArn: NotRequired[str],
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (3)
```

1. See [:material-code-brackets: FsxFileSystemTypeType](./literals.md#fsxfilesystemtypetype) 
2. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## JiraConfigurationOutputTypeDef

```python
# JiraConfigurationOutputTypeDef definition

class JiraConfigurationOutputTypeDef(TypedDict):
    JiraAccountUrl: str,
    SecretArn: str,
    UseChangeLog: NotRequired[bool],
    Project: NotRequired[List[str]],
    IssueType: NotRequired[List[str]],
    Status: NotRequired[List[str]],
    IssueSubEntityFilter: NotRequired[List[IssueSubEntityType]],  # (1)
    AttachmentFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    CommentFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    IssueFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    ProjectFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    WorkLogFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (7)
```

1. See [:material-code-brackets: IssueSubEntityType](./literals.md#issuesubentitytype) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
5. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
6. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
7. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
## QuipConfigurationOutputTypeDef

```python
# QuipConfigurationOutputTypeDef definition

class QuipConfigurationOutputTypeDef(TypedDict):
    Domain: str,
    SecretArn: str,
    CrawlFileComments: NotRequired[bool],
    CrawlChatRooms: NotRequired[bool],
    CrawlAttachments: NotRequired[bool],
    FolderIds: NotRequired[List[str]],
    ThreadFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    MessageFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    AttachmentFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (4)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
## SlackConfigurationOutputTypeDef

```python
# SlackConfigurationOutputTypeDef definition

class SlackConfigurationOutputTypeDef(TypedDict):
    TeamId: str,
    SecretArn: str,
    SlackEntityList: List[SlackEntityType],  # (2)
    SinceCrawlDate: str,
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (1)
    UseChangeLog: NotRequired[bool],
    CrawlBotMessage: NotRequired[bool],
    ExcludeArchived: NotRequired[bool],
    LookBackPeriod: NotRequired[int],
    PrivateChannelFilter: NotRequired[List[str]],
    PublicChannelFilter: NotRequired[List[str]],
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (3)
```

1. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
2. See [:material-code-brackets: SlackEntityType](./literals.md#slackentitytype) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## AlfrescoConfigurationOutputTypeDef

```python
# AlfrescoConfigurationOutputTypeDef definition

class AlfrescoConfigurationOutputTypeDef(TypedDict):
    SiteUrl: str,
    SiteId: str,
    SecretArn: str,
    SslCertificateS3Path: S3PathTypeDef,  # (1)
    CrawlSystemFolders: NotRequired[bool],
    CrawlComments: NotRequired[bool],
    EntityFilter: NotRequired[List[AlfrescoEntityType]],  # (2)
    DocumentLibraryFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (3)
    BlogFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (3)
    WikiFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (3)
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (6)
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
2. See [:material-code-brackets: AlfrescoEntityType](./literals.md#alfrescoentitytype) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
5. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
6. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
## OnPremiseConfigurationTypeDef

```python
# OnPremiseConfigurationTypeDef definition

class OnPremiseConfigurationTypeDef(TypedDict):
    HostUrl: str,
    OrganizationName: str,
    SslCertificateS3Path: S3PathTypeDef,  # (1)
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
## OneDriveUsersOutputTypeDef

```python
# OneDriveUsersOutputTypeDef definition

class OneDriveUsersOutputTypeDef(TypedDict):
    OneDriveUserList: NotRequired[List[str]],
    OneDriveUserS3Path: NotRequired[S3PathTypeDef],  # (1)
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
## OneDriveUsersTypeDef

```python
# OneDriveUsersTypeDef definition

class OneDriveUsersTypeDef(TypedDict):
    OneDriveUserList: NotRequired[Sequence[str]],
    OneDriveUserS3Path: NotRequired[S3PathTypeDef],  # (1)
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
## UpdateQuerySuggestionsBlockListRequestRequestTypeDef

```python
# UpdateQuerySuggestionsBlockListRequestRequestTypeDef definition

class UpdateQuerySuggestionsBlockListRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Id: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    SourceS3Path: NotRequired[S3PathTypeDef],  # (1)
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
## UpdateThesaurusRequestRequestTypeDef

```python
# UpdateThesaurusRequestRequestTypeDef definition

class UpdateThesaurusRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    RoleArn: NotRequired[str],
    SourceS3Path: NotRequired[S3PathTypeDef],  # (1)
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
## AssociateEntitiesToExperienceRequestRequestTypeDef

```python
# AssociateEntitiesToExperienceRequestRequestTypeDef definition

class AssociateEntitiesToExperienceRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    EntityList: Sequence[EntityConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EntityConfigurationTypeDef](./type_defs.md#entityconfigurationtypedef) 
## DisassociateEntitiesFromExperienceRequestRequestTypeDef

```python
# DisassociateEntitiesFromExperienceRequestRequestTypeDef definition

class DisassociateEntitiesFromExperienceRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    EntityList: Sequence[EntityConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EntityConfigurationTypeDef](./type_defs.md#entityconfigurationtypedef) 
## AssociateEntitiesToExperienceResponseTypeDef

```python
# AssociateEntitiesToExperienceResponseTypeDef definition

class AssociateEntitiesToExperienceResponseTypeDef(TypedDict):
    FailedEntityList: List[FailedEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedEntityTypeDef](./type_defs.md#failedentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociatePersonasToEntitiesResponseTypeDef

```python
# AssociatePersonasToEntitiesResponseTypeDef definition

class AssociatePersonasToEntitiesResponseTypeDef(TypedDict):
    FailedEntityList: List[FailedEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedEntityTypeDef](./type_defs.md#failedentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAccessControlConfigurationResponseTypeDef

```python
# CreateAccessControlConfigurationResponseTypeDef definition

class CreateAccessControlConfigurationResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataSourceResponseTypeDef

```python
# CreateDataSourceResponseTypeDef definition

class CreateDataSourceResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateExperienceResponseTypeDef

```python
# CreateExperienceResponseTypeDef definition

class CreateExperienceResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFaqResponseTypeDef

```python
# CreateFaqResponseTypeDef definition

class CreateFaqResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateIndexResponseTypeDef

```python
# CreateIndexResponseTypeDef definition

class CreateIndexResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateQuerySuggestionsBlockListResponseTypeDef

```python
# CreateQuerySuggestionsBlockListResponseTypeDef definition

class CreateQuerySuggestionsBlockListResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateThesaurusResponseTypeDef

```python
# CreateThesaurusResponseTypeDef definition

class CreateThesaurusResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeFaqResponseTypeDef

```python
# DescribeFaqResponseTypeDef definition

class DescribeFaqResponseTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    Name: str,
    Description: str,
    CreatedAt: datetime,
    UpdatedAt: datetime,
    S3Path: S3PathTypeDef,  # (1)
    Status: FaqStatusType,  # (2)
    RoleArn: str,
    ErrorMessage: str,
    FileFormat: FaqFileFormatType,  # (3)
    LanguageCode: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
2. See [:material-code-brackets: FaqStatusType](./literals.md#faqstatustype) 
3. See [:material-code-brackets: FaqFileFormatType](./literals.md#faqfileformattype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeQuerySuggestionsBlockListResponseTypeDef

```python
# DescribeQuerySuggestionsBlockListResponseTypeDef definition

class DescribeQuerySuggestionsBlockListResponseTypeDef(TypedDict):
    IndexId: str,
    Id: str,
    Name: str,
    Description: str,
    Status: QuerySuggestionsBlockListStatusType,  # (1)
    ErrorMessage: str,
    CreatedAt: datetime,
    UpdatedAt: datetime,
    SourceS3Path: S3PathTypeDef,  # (2)
    ItemCount: int,
    FileSizeBytes: int,
    RoleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: QuerySuggestionsBlockListStatusType](./literals.md#querysuggestionsblockliststatustype) 
2. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeThesaurusResponseTypeDef

```python
# DescribeThesaurusResponseTypeDef definition

class DescribeThesaurusResponseTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    Name: str,
    Description: str,
    Status: ThesaurusStatusType,  # (1)
    ErrorMessage: str,
    CreatedAt: datetime,
    UpdatedAt: datetime,
    RoleArn: str,
    SourceS3Path: S3PathTypeDef,  # (2)
    FileSizeBytes: int,
    TermCount: int,
    SynonymRuleCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ThesaurusStatusType](./literals.md#thesaurusstatustype) 
2. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateEntitiesFromExperienceResponseTypeDef

```python
# DisassociateEntitiesFromExperienceResponseTypeDef definition

class DisassociateEntitiesFromExperienceResponseTypeDef(TypedDict):
    FailedEntityList: List[FailedEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedEntityTypeDef](./type_defs.md#failedentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociatePersonasFromEntitiesResponseTypeDef

```python
# DisassociatePersonasFromEntitiesResponseTypeDef definition

class DisassociatePersonasFromEntitiesResponseTypeDef(TypedDict):
    FailedEntityList: List[FailedEntityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedEntityTypeDef](./type_defs.md#failedentitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAccessControlConfigurationsResponseTypeDef

```python
# ListAccessControlConfigurationsResponseTypeDef definition

class ListAccessControlConfigurationsResponseTypeDef(TypedDict):
    AccessControlConfigurations: List[AccessControlConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AccessControlConfigurationSummaryTypeDef](./type_defs.md#accesscontrolconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataSourceSyncJobResponseTypeDef

```python
# StartDataSourceSyncJobResponseTypeDef definition

class StartDataSourceSyncJobResponseTypeDef(TypedDict):
    ExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociatePersonasToEntitiesRequestRequestTypeDef

```python
# AssociatePersonasToEntitiesRequestRequestTypeDef definition

class AssociatePersonasToEntitiesRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    Personas: Sequence[EntityPersonaConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: EntityPersonaConfigurationTypeDef](./type_defs.md#entitypersonaconfigurationtypedef) 
## AttributeSuggestionsDescribeConfigTypeDef

```python
# AttributeSuggestionsDescribeConfigTypeDef definition

class AttributeSuggestionsDescribeConfigTypeDef(TypedDict):
    SuggestableConfigList: NotRequired[List[SuggestableConfigTypeDef]],  # (1)
    AttributeSuggestionsMode: NotRequired[AttributeSuggestionsModeType],  # (2)
```

1. See [:material-code-braces: SuggestableConfigTypeDef](./type_defs.md#suggestableconfigtypedef) 
2. See [:material-code-brackets: AttributeSuggestionsModeType](./literals.md#attributesuggestionsmodetype) 
## AttributeSuggestionsUpdateConfigTypeDef

```python
# AttributeSuggestionsUpdateConfigTypeDef definition

class AttributeSuggestionsUpdateConfigTypeDef(TypedDict):
    SuggestableConfigList: NotRequired[Sequence[SuggestableConfigTypeDef]],  # (1)
    AttributeSuggestionsMode: NotRequired[AttributeSuggestionsModeType],  # (2)
```

1. See [:material-code-braces: SuggestableConfigTypeDef](./type_defs.md#suggestableconfigtypedef) 
2. See [:material-code-brackets: AttributeSuggestionsModeType](./literals.md#attributesuggestionsmodetype) 
## AuthenticationConfigurationOutputTypeDef

```python
# AuthenticationConfigurationOutputTypeDef definition

class AuthenticationConfigurationOutputTypeDef(TypedDict):
    BasicAuthentication: NotRequired[List[BasicAuthenticationConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: BasicAuthenticationConfigurationTypeDef](./type_defs.md#basicauthenticationconfigurationtypedef) 
## AuthenticationConfigurationTypeDef

```python
# AuthenticationConfigurationTypeDef definition

class AuthenticationConfigurationTypeDef(TypedDict):
    BasicAuthentication: NotRequired[Sequence[BasicAuthenticationConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: BasicAuthenticationConfigurationTypeDef](./type_defs.md#basicauthenticationconfigurationtypedef) 
## BatchDeleteDocumentRequestRequestTypeDef

```python
# BatchDeleteDocumentRequestRequestTypeDef definition

class BatchDeleteDocumentRequestRequestTypeDef(TypedDict):
    IndexId: str,
    DocumentIdList: Sequence[str],
    DataSourceSyncJobMetricTarget: NotRequired[DataSourceSyncJobMetricTargetTypeDef],  # (1)
```

1. See [:material-code-braces: DataSourceSyncJobMetricTargetTypeDef](./type_defs.md#datasourcesyncjobmetrictargettypedef) 
## BatchDeleteDocumentResponseTypeDef

```python
# BatchDeleteDocumentResponseTypeDef definition

class BatchDeleteDocumentResponseTypeDef(TypedDict):
    FailedDocuments: List[BatchDeleteDocumentResponseFailedDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteDocumentResponseFailedDocumentTypeDef](./type_defs.md#batchdeletedocumentresponsefaileddocumenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDeleteFeaturedResultsSetResponseTypeDef

```python
# BatchDeleteFeaturedResultsSetResponseTypeDef definition

class BatchDeleteFeaturedResultsSetResponseTypeDef(TypedDict):
    Errors: List[BatchDeleteFeaturedResultsSetErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchDeleteFeaturedResultsSetErrorTypeDef](./type_defs.md#batchdeletefeaturedresultsseterrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetDocumentStatusResponseTypeDef

```python
# BatchGetDocumentStatusResponseTypeDef definition

class BatchGetDocumentStatusResponseTypeDef(TypedDict):
    Errors: List[BatchGetDocumentStatusResponseErrorTypeDef],  # (1)
    DocumentStatusList: List[StatusTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchGetDocumentStatusResponseErrorTypeDef](./type_defs.md#batchgetdocumentstatusresponseerrortypedef) 
2. See [:material-code-braces: StatusTypeDef](./type_defs.md#statustypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutDocumentResponseTypeDef

```python
# BatchPutDocumentResponseTypeDef definition

class BatchPutDocumentResponseTypeDef(TypedDict):
    FailedDocuments: List[BatchPutDocumentResponseFailedDocumentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchPutDocumentResponseFailedDocumentTypeDef](./type_defs.md#batchputdocumentresponsefaileddocumenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ClickFeedbackTypeDef

```python
# ClickFeedbackTypeDef definition

class ClickFeedbackTypeDef(TypedDict):
    ResultId: str,
    ClickTime: TimestampTypeDef,
```

## DocumentAttributeValueTypeDef

```python
# DocumentAttributeValueTypeDef definition

class DocumentAttributeValueTypeDef(TypedDict):
    StringValue: NotRequired[str],
    StringListValue: NotRequired[Sequence[str]],
    LongValue: NotRequired[int],
    DateValue: NotRequired[TimestampTypeDef],
```

## TimeRangeTypeDef

```python
# TimeRangeTypeDef definition

class TimeRangeTypeDef(TypedDict):
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
```

## CollapseConfigurationTypeDef

```python
# CollapseConfigurationTypeDef definition

class CollapseConfigurationTypeDef(TypedDict):
    DocumentAttributeKey: str,
    SortingConfigurations: NotRequired[Sequence[SortingConfigurationTypeDef]],  # (1)
    MissingAttributeKeyStrategy: NotRequired[MissingAttributeKeyStrategyType],  # (2)
    Expand: NotRequired[bool],
    ExpandConfiguration: NotRequired[ExpandConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: SortingConfigurationTypeDef](./type_defs.md#sortingconfigurationtypedef) 
2. See [:material-code-brackets: MissingAttributeKeyStrategyType](./literals.md#missingattributekeystrategytype) 
3. See [:material-code-braces: ExpandConfigurationTypeDef](./type_defs.md#expandconfigurationtypedef) 
## ConfluenceAttachmentConfigurationOutputTypeDef

```python
# ConfluenceAttachmentConfigurationOutputTypeDef definition

class ConfluenceAttachmentConfigurationOutputTypeDef(TypedDict):
    CrawlAttachments: NotRequired[bool],
    AttachmentFieldMappings: NotRequired[List[ConfluenceAttachmentToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfluenceAttachmentToIndexFieldMappingTypeDef](./type_defs.md#confluenceattachmenttoindexfieldmappingtypedef) 
## ConfluenceAttachmentConfigurationTypeDef

```python
# ConfluenceAttachmentConfigurationTypeDef definition

class ConfluenceAttachmentConfigurationTypeDef(TypedDict):
    CrawlAttachments: NotRequired[bool],
    AttachmentFieldMappings: NotRequired[Sequence[ConfluenceAttachmentToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfluenceAttachmentToIndexFieldMappingTypeDef](./type_defs.md#confluenceattachmenttoindexfieldmappingtypedef) 
## ConfluenceBlogConfigurationOutputTypeDef

```python
# ConfluenceBlogConfigurationOutputTypeDef definition

class ConfluenceBlogConfigurationOutputTypeDef(TypedDict):
    BlogFieldMappings: NotRequired[List[ConfluenceBlogToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfluenceBlogToIndexFieldMappingTypeDef](./type_defs.md#confluenceblogtoindexfieldmappingtypedef) 
## ConfluenceBlogConfigurationTypeDef

```python
# ConfluenceBlogConfigurationTypeDef definition

class ConfluenceBlogConfigurationTypeDef(TypedDict):
    BlogFieldMappings: NotRequired[Sequence[ConfluenceBlogToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfluenceBlogToIndexFieldMappingTypeDef](./type_defs.md#confluenceblogtoindexfieldmappingtypedef) 
## SharePointConfigurationOutputTypeDef

```python
# SharePointConfigurationOutputTypeDef definition

class SharePointConfigurationOutputTypeDef(TypedDict):
    SharePointVersion: SharePointVersionType,  # (1)
    Urls: List[str],
    SecretArn: str,
    CrawlAttachments: NotRequired[bool],
    UseChangeLog: NotRequired[bool],
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (2)
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (3)
    DocumentTitleFieldName: NotRequired[str],
    DisableLocalGroups: NotRequired[bool],
    SslCertificateS3Path: NotRequired[S3PathTypeDef],  # (4)
    AuthenticationType: NotRequired[SharePointOnlineAuthenticationTypeType],  # (5)
    ProxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: SharePointVersionType](./literals.md#sharepointversiontype) 
2. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
5. See [:material-code-brackets: SharePointOnlineAuthenticationTypeType](./literals.md#sharepointonlineauthenticationtypetype) 
6. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
## ConfluencePageConfigurationOutputTypeDef

```python
# ConfluencePageConfigurationOutputTypeDef definition

class ConfluencePageConfigurationOutputTypeDef(TypedDict):
    PageFieldMappings: NotRequired[List[ConfluencePageToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfluencePageToIndexFieldMappingTypeDef](./type_defs.md#confluencepagetoindexfieldmappingtypedef) 
## ConfluencePageConfigurationTypeDef

```python
# ConfluencePageConfigurationTypeDef definition

class ConfluencePageConfigurationTypeDef(TypedDict):
    PageFieldMappings: NotRequired[Sequence[ConfluencePageToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfluencePageToIndexFieldMappingTypeDef](./type_defs.md#confluencepagetoindexfieldmappingtypedef) 
## ConfluenceSpaceConfigurationOutputTypeDef

```python
# ConfluenceSpaceConfigurationOutputTypeDef definition

class ConfluenceSpaceConfigurationOutputTypeDef(TypedDict):
    CrawlPersonalSpaces: NotRequired[bool],
    CrawlArchivedSpaces: NotRequired[bool],
    IncludeSpaces: NotRequired[List[str]],
    ExcludeSpaces: NotRequired[List[str]],
    SpaceFieldMappings: NotRequired[List[ConfluenceSpaceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfluenceSpaceToIndexFieldMappingTypeDef](./type_defs.md#confluencespacetoindexfieldmappingtypedef) 
## ConfluenceSpaceConfigurationTypeDef

```python
# ConfluenceSpaceConfigurationTypeDef definition

class ConfluenceSpaceConfigurationTypeDef(TypedDict):
    CrawlPersonalSpaces: NotRequired[bool],
    CrawlArchivedSpaces: NotRequired[bool],
    IncludeSpaces: NotRequired[Sequence[str]],
    ExcludeSpaces: NotRequired[Sequence[str]],
    SpaceFieldMappings: NotRequired[Sequence[ConfluenceSpaceToIndexFieldMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: ConfluenceSpaceToIndexFieldMappingTypeDef](./type_defs.md#confluencespacetoindexfieldmappingtypedef) 
## SpellCorrectedQueryTypeDef

```python
# SpellCorrectedQueryTypeDef definition

class SpellCorrectedQueryTypeDef(TypedDict):
    SuggestedQueryText: NotRequired[str],
    Corrections: NotRequired[List[CorrectionTypeDef]],  # (1)
```

1. See [:material-code-braces: CorrectionTypeDef](./type_defs.md#correctiontypedef) 
## HierarchicalPrincipalOutputTypeDef

```python
# HierarchicalPrincipalOutputTypeDef definition

class HierarchicalPrincipalOutputTypeDef(TypedDict):
    PrincipalList: List[PrincipalTypeDef],  # (1)
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
## HierarchicalPrincipalTypeDef

```python
# HierarchicalPrincipalTypeDef definition

class HierarchicalPrincipalTypeDef(TypedDict):
    PrincipalList: Sequence[PrincipalTypeDef],  # (1)
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
## CreateFaqRequestRequestTypeDef

```python
# CreateFaqRequestRequestTypeDef definition

class CreateFaqRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Name: str,
    S3Path: S3PathTypeDef,  # (1)
    RoleArn: str,
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    FileFormat: NotRequired[FaqFileFormatType],  # (3)
    ClientToken: NotRequired[str],
    LanguageCode: NotRequired[str],
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: FaqFileFormatType](./literals.md#faqfileformattype) 
## CreateQuerySuggestionsBlockListRequestRequestTypeDef

```python
# CreateQuerySuggestionsBlockListRequestRequestTypeDef definition

class CreateQuerySuggestionsBlockListRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Name: str,
    SourceS3Path: S3PathTypeDef,  # (1)
    RoleArn: str,
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateThesaurusRequestRequestTypeDef

```python
# CreateThesaurusRequestRequestTypeDef definition

class CreateThesaurusRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Name: str,
    RoleArn: str,
    SourceS3Path: S3PathTypeDef,  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateFeaturedResultsSetRequestRequestTypeDef

```python
# CreateFeaturedResultsSetRequestRequestTypeDef definition

class CreateFeaturedResultsSetRequestRequestTypeDef(TypedDict):
    IndexId: str,
    FeaturedResultsSetName: str,
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    Status: NotRequired[FeaturedResultsSetStatusType],  # (1)
    QueryTexts: NotRequired[Sequence[str]],
    FeaturedDocuments: NotRequired[Sequence[FeaturedDocumentTypeDef]],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: FeaturedResultsSetStatusType](./literals.md#featuredresultssetstatustype) 
2. See [:material-code-braces: FeaturedDocumentTypeDef](./type_defs.md#featureddocumenttypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## FeaturedResultsSetTypeDef

```python
# FeaturedResultsSetTypeDef definition

class FeaturedResultsSetTypeDef(TypedDict):
    FeaturedResultsSetId: NotRequired[str],
    FeaturedResultsSetName: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[FeaturedResultsSetStatusType],  # (1)
    QueryTexts: NotRequired[List[str]],
    FeaturedDocuments: NotRequired[List[FeaturedDocumentTypeDef]],  # (2)
    LastUpdatedTimestamp: NotRequired[int],
    CreationTimestamp: NotRequired[int],
```

1. See [:material-code-brackets: FeaturedResultsSetStatusType](./literals.md#featuredresultssetstatustype) 
2. See [:material-code-braces: FeaturedDocumentTypeDef](./type_defs.md#featureddocumenttypedef) 
## UpdateFeaturedResultsSetRequestRequestTypeDef

```python
# UpdateFeaturedResultsSetRequestRequestTypeDef definition

class UpdateFeaturedResultsSetRequestRequestTypeDef(TypedDict):
    IndexId: str,
    FeaturedResultsSetId: str,
    FeaturedResultsSetName: NotRequired[str],
    Description: NotRequired[str],
    Status: NotRequired[FeaturedResultsSetStatusType],  # (1)
    QueryTexts: NotRequired[Sequence[str]],
    FeaturedDocuments: NotRequired[Sequence[FeaturedDocumentTypeDef]],  # (2)
```

1. See [:material-code-brackets: FeaturedResultsSetStatusType](./literals.md#featuredresultssetstatustype) 
2. See [:material-code-braces: FeaturedDocumentTypeDef](./type_defs.md#featureddocumenttypedef) 
## UserContextTypeDef

```python
# UserContextTypeDef definition

class UserContextTypeDef(TypedDict):
    Token: NotRequired[str],
    UserId: NotRequired[str],
    Groups: NotRequired[Sequence[str]],
    DataSourceGroups: NotRequired[Sequence[DataSourceGroupTypeDef]],  # (1)
```

1. See [:material-code-braces: DataSourceGroupTypeDef](./type_defs.md#datasourcegrouptypedef) 
## ListDataSourcesResponseTypeDef

```python
# ListDataSourcesResponseTypeDef definition

class ListDataSourcesResponseTypeDef(TypedDict):
    SummaryItems: List[DataSourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceSummaryTypeDef](./type_defs.md#datasourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceSyncJobTypeDef

```python
# DataSourceSyncJobTypeDef definition

class DataSourceSyncJobTypeDef(TypedDict):
    ExecutionId: NotRequired[str],
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    Status: NotRequired[DataSourceSyncJobStatusType],  # (1)
    ErrorMessage: NotRequired[str],
    ErrorCode: NotRequired[ErrorCodeType],  # (2)
    DataSourceErrorCode: NotRequired[str],
    Metrics: NotRequired[DataSourceSyncJobMetricsTypeDef],  # (3)
```

1. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
2. See [:material-code-brackets: ErrorCodeType](./literals.md#errorcodetype) 
3. See [:material-code-braces: DataSourceSyncJobMetricsTypeDef](./type_defs.md#datasourcesyncjobmetricstypedef) 
## ExperiencesSummaryTypeDef

```python
# ExperiencesSummaryTypeDef definition

class ExperiencesSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    CreatedAt: NotRequired[datetime],
    Status: NotRequired[ExperienceStatusType],  # (1)
    Endpoints: NotRequired[List[ExperienceEndpointTypeDef]],  # (2)
```

1. See [:material-code-brackets: ExperienceStatusType](./literals.md#experiencestatustype) 
2. See [:material-code-braces: ExperienceEndpointTypeDef](./type_defs.md#experienceendpointtypedef) 
## DescribeFeaturedResultsSetResponseTypeDef

```python
# DescribeFeaturedResultsSetResponseTypeDef definition

class DescribeFeaturedResultsSetResponseTypeDef(TypedDict):
    FeaturedResultsSetId: str,
    FeaturedResultsSetName: str,
    Description: str,
    Status: FeaturedResultsSetStatusType,  # (1)
    QueryTexts: List[str],
    FeaturedDocumentsWithMetadata: List[FeaturedDocumentWithMetadataTypeDef],  # (2)
    FeaturedDocumentsMissing: List[FeaturedDocumentMissingTypeDef],  # (3)
    LastUpdatedTimestamp: int,
    CreationTimestamp: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: FeaturedResultsSetStatusType](./literals.md#featuredresultssetstatustype) 
2. See [:material-code-braces: FeaturedDocumentWithMetadataTypeDef](./type_defs.md#featureddocumentwithmetadatatypedef) 
3. See [:material-code-braces: FeaturedDocumentMissingTypeDef](./type_defs.md#featureddocumentmissingtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePrincipalMappingResponseTypeDef

```python
# DescribePrincipalMappingResponseTypeDef definition

class DescribePrincipalMappingResponseTypeDef(TypedDict):
    IndexId: str,
    DataSourceId: str,
    GroupId: str,
    GroupOrderingIdSummaries: List[GroupOrderingIdSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupOrderingIdSummaryTypeDef](./type_defs.md#grouporderingidsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentAttributeConditionOutputTypeDef

```python
# DocumentAttributeConditionOutputTypeDef definition

class DocumentAttributeConditionOutputTypeDef(TypedDict):
    ConditionDocumentAttributeKey: str,
    Operator: ConditionOperatorType,  # (1)
    ConditionOnValue: NotRequired[DocumentAttributeValueOutputTypeDef],  # (2)
```

1. See [:material-code-brackets: ConditionOperatorType](./literals.md#conditionoperatortype) 
2. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentAttributeOutputTypeDef

```python
# DocumentAttributeOutputTypeDef definition

class DocumentAttributeOutputTypeDef(TypedDict):
    Key: str,
    Value: DocumentAttributeValueOutputTypeDef,  # (1)
```

1. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentAttributeTargetOutputTypeDef

```python
# DocumentAttributeTargetOutputTypeDef definition

class DocumentAttributeTargetOutputTypeDef(TypedDict):
    TargetDocumentAttributeKey: NotRequired[str],
    TargetDocumentAttributeValueDeletion: NotRequired[bool],
    TargetDocumentAttributeValue: NotRequired[DocumentAttributeValueOutputTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentAttributeValueCountPairTypeDef

```python
# DocumentAttributeValueCountPairTypeDef definition

class DocumentAttributeValueCountPairTypeDef(TypedDict):
    DocumentAttributeValue: NotRequired[DocumentAttributeValueOutputTypeDef],  # (1)
    Count: NotRequired[int],
    FacetResults: NotRequired[List[Dict[str, Any]]],
```

1. See [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentMetadataConfigurationOutputTypeDef

```python
# DocumentMetadataConfigurationOutputTypeDef definition

class DocumentMetadataConfigurationOutputTypeDef(TypedDict):
    Name: str,
    Type: DocumentAttributeValueTypeType,  # (1)
    Relevance: NotRequired[RelevanceOutputTypeDef],  # (2)
    Search: NotRequired[SearchTypeDef],  # (3)
```

1. See [:material-code-brackets: DocumentAttributeValueTypeType](./literals.md#documentattributevaluetypetype) 
2. See [:material-code-braces: RelevanceOutputTypeDef](./type_defs.md#relevanceoutputtypedef) 
3. See [:material-code-braces: SearchTypeDef](./type_defs.md#searchtypedef) 
## S3DataSourceConfigurationOutputTypeDef

```python
# S3DataSourceConfigurationOutputTypeDef definition

class S3DataSourceConfigurationOutputTypeDef(TypedDict):
    BucketName: str,
    InclusionPrefixes: NotRequired[List[str]],
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    DocumentsMetadataConfiguration: NotRequired[DocumentsMetadataConfigurationTypeDef],  # (1)
    AccessControlListConfiguration: NotRequired[AccessControlListConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentsMetadataConfigurationTypeDef](./type_defs.md#documentsmetadataconfigurationtypedef) 
2. See [:material-code-braces: AccessControlListConfigurationTypeDef](./type_defs.md#accesscontrollistconfigurationtypedef) 
## S3DataSourceConfigurationTypeDef

```python
# S3DataSourceConfigurationTypeDef definition

class S3DataSourceConfigurationTypeDef(TypedDict):
    BucketName: str,
    InclusionPrefixes: NotRequired[Sequence[str]],
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    DocumentsMetadataConfiguration: NotRequired[DocumentsMetadataConfigurationTypeDef],  # (1)
    AccessControlListConfiguration: NotRequired[AccessControlListConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentsMetadataConfigurationTypeDef](./type_defs.md#documentsmetadataconfigurationtypedef) 
2. See [:material-code-braces: AccessControlListConfigurationTypeDef](./type_defs.md#accesscontrollistconfigurationtypedef) 
## ExperienceEntitiesSummaryTypeDef

```python
# ExperienceEntitiesSummaryTypeDef definition

class ExperienceEntitiesSummaryTypeDef(TypedDict):
    EntityId: NotRequired[str],
    EntityType: NotRequired[EntityTypeType],  # (1)
    DisplayData: NotRequired[EntityDisplayDataTypeDef],  # (2)
```

1. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
2. See [:material-code-braces: EntityDisplayDataTypeDef](./type_defs.md#entitydisplaydatatypedef) 
## ExperienceConfigurationOutputTypeDef

```python
# ExperienceConfigurationOutputTypeDef definition

class ExperienceConfigurationOutputTypeDef(TypedDict):
    ContentSourceConfiguration: NotRequired[ContentSourceConfigurationOutputTypeDef],  # (1)
    UserIdentityConfiguration: NotRequired[UserIdentityConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ContentSourceConfigurationOutputTypeDef](./type_defs.md#contentsourceconfigurationoutputtypedef) 
2. See [:material-code-braces: UserIdentityConfigurationTypeDef](./type_defs.md#useridentityconfigurationtypedef) 
## ListFaqsResponseTypeDef

```python
# ListFaqsResponseTypeDef definition

class ListFaqsResponseTypeDef(TypedDict):
    FaqSummaryItems: List[FaqSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FaqSummaryTypeDef](./type_defs.md#faqsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListFeaturedResultsSetsResponseTypeDef

```python
# ListFeaturedResultsSetsResponseTypeDef definition

class ListFeaturedResultsSetsResponseTypeDef(TypedDict):
    FeaturedResultsSetSummaryItems: List[FeaturedResultsSetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: FeaturedResultsSetSummaryTypeDef](./type_defs.md#featuredresultssetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSnapshotsResponseTypeDef

```python
# GetSnapshotsResponseTypeDef definition

class GetSnapshotsResponseTypeDef(TypedDict):
    SnapShotTimeFilter: TimeRangeOutputTypeDef,  # (1)
    SnapshotsDataHeader: List[str],
    SnapshotsData: List[List[str]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TimeRangeOutputTypeDef](./type_defs.md#timerangeoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GroupMembersTypeDef

```python
# GroupMembersTypeDef definition

class GroupMembersTypeDef(TypedDict):
    MemberGroups: NotRequired[Sequence[MemberGroupTypeDef]],  # (1)
    MemberUsers: NotRequired[Sequence[MemberUserTypeDef]],  # (2)
    S3PathforGroupMembers: NotRequired[S3PathTypeDef],  # (3)
```

1. See [:material-code-braces: MemberGroupTypeDef](./type_defs.md#membergrouptypedef) 
2. See [:material-code-braces: MemberUserTypeDef](./type_defs.md#memberusertypedef) 
3. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
## ListGroupsOlderThanOrderingIdResponseTypeDef

```python
# ListGroupsOlderThanOrderingIdResponseTypeDef definition

class ListGroupsOlderThanOrderingIdResponseTypeDef(TypedDict):
    GroupsSummaries: List[GroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TextWithHighlightsTypeDef

```python
# TextWithHighlightsTypeDef definition

class TextWithHighlightsTypeDef(TypedDict):
    Text: NotRequired[str],
    Highlights: NotRequired[List[HighlightTypeDef]],  # (1)
```

1. See [:material-code-braces: HighlightTypeDef](./type_defs.md#highlighttypedef) 
## ListIndicesResponseTypeDef

```python
# ListIndicesResponseTypeDef definition

class ListIndicesResponseTypeDef(TypedDict):
    IndexConfigurationSummaryItems: List[IndexConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: IndexConfigurationSummaryTypeDef](./type_defs.md#indexconfigurationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## IndexStatisticsTypeDef

```python
# IndexStatisticsTypeDef definition

class IndexStatisticsTypeDef(TypedDict):
    FaqStatistics: FaqStatisticsTypeDef,  # (1)
    TextDocumentStatistics: TextDocumentStatisticsTypeDef,  # (2)
```

1. See [:material-code-braces: FaqStatisticsTypeDef](./type_defs.md#faqstatisticstypedef) 
2. See [:material-code-braces: TextDocumentStatisticsTypeDef](./type_defs.md#textdocumentstatisticstypedef) 
## UserTokenConfigurationTypeDef

```python
# UserTokenConfigurationTypeDef definition

class UserTokenConfigurationTypeDef(TypedDict):
    JwtTokenTypeConfiguration: NotRequired[JwtTokenTypeConfigurationTypeDef],  # (1)
    JsonTokenTypeConfiguration: NotRequired[JsonTokenTypeConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: JwtTokenTypeConfigurationTypeDef](./type_defs.md#jwttokentypeconfigurationtypedef) 
2. See [:material-code-braces: JsonTokenTypeConfigurationTypeDef](./type_defs.md#jsontokentypeconfigurationtypedef) 
## ListEntityPersonasResponseTypeDef

```python
# ListEntityPersonasResponseTypeDef definition

class ListEntityPersonasResponseTypeDef(TypedDict):
    SummaryItems: List[PersonasSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PersonasSummaryTypeDef](./type_defs.md#personassummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQuerySuggestionsBlockListsResponseTypeDef

```python
# ListQuerySuggestionsBlockListsResponseTypeDef definition

class ListQuerySuggestionsBlockListsResponseTypeDef(TypedDict):
    BlockListSummaryItems: List[QuerySuggestionsBlockListSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QuerySuggestionsBlockListSummaryTypeDef](./type_defs.md#querysuggestionsblocklistsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListThesauriResponseTypeDef

```python
# ListThesauriResponseTypeDef definition

class ListThesauriResponseTypeDef(TypedDict):
    ThesaurusSummaryItems: List[ThesaurusSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ThesaurusSummaryTypeDef](./type_defs.md#thesaurussummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UrlsOutputTypeDef

```python
# UrlsOutputTypeDef definition

class UrlsOutputTypeDef(TypedDict):
    SeedUrlConfiguration: NotRequired[SeedUrlConfigurationOutputTypeDef],  # (1)
    SiteMapsConfiguration: NotRequired[SiteMapsConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: SeedUrlConfigurationOutputTypeDef](./type_defs.md#seedurlconfigurationoutputtypedef) 
2. See [:material-code-braces: SiteMapsConfigurationOutputTypeDef](./type_defs.md#sitemapsconfigurationoutputtypedef) 
## SuggestionTextWithHighlightsTypeDef

```python
# SuggestionTextWithHighlightsTypeDef definition

class SuggestionTextWithHighlightsTypeDef(TypedDict):
    Text: NotRequired[str],
    Highlights: NotRequired[List[SuggestionHighlightTypeDef]],  # (1)
```

1. See [:material-code-braces: SuggestionHighlightTypeDef](./type_defs.md#suggestionhighlighttypedef) 
## TableRowTypeDef

```python
# TableRowTypeDef definition

class TableRowTypeDef(TypedDict):
    Cells: NotRequired[List[TableCellTypeDef]],  # (1)
```

1. See [:material-code-braces: TableCellTypeDef](./type_defs.md#tablecelltypedef) 
## DatabaseConfigurationOutputTypeDef

```python
# DatabaseConfigurationOutputTypeDef definition

class DatabaseConfigurationOutputTypeDef(TypedDict):
    DatabaseEngineType: DatabaseEngineTypeType,  # (1)
    ConnectionConfiguration: ConnectionConfigurationTypeDef,  # (2)
    ColumnConfiguration: ColumnConfigurationOutputTypeDef,  # (4)
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (3)
    AclConfiguration: NotRequired[AclConfigurationTypeDef],  # (5)
    SqlConfiguration: NotRequired[SqlConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: DatabaseEngineTypeType](./literals.md#databaseenginetypetype) 
2. See [:material-code-braces: ConnectionConfigurationTypeDef](./type_defs.md#connectionconfigurationtypedef) 
3. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
4. See [:material-code-braces: ColumnConfigurationOutputTypeDef](./type_defs.md#columnconfigurationoutputtypedef) 
5. See [:material-code-braces: AclConfigurationTypeDef](./type_defs.md#aclconfigurationtypedef) 
6. See [:material-code-braces: SqlConfigurationTypeDef](./type_defs.md#sqlconfigurationtypedef) 
## SalesforceKnowledgeArticleConfigurationOutputTypeDef

```python
# SalesforceKnowledgeArticleConfigurationOutputTypeDef definition

class SalesforceKnowledgeArticleConfigurationOutputTypeDef(TypedDict):
    IncludedStates: List[SalesforceKnowledgeArticleStateType],  # (1)
    StandardKnowledgeArticleTypeConfiguration: NotRequired[SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef],  # (2)
    CustomKnowledgeArticleTypeConfigurations: NotRequired[List[SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: SalesforceKnowledgeArticleStateType](./literals.md#salesforceknowledgearticlestatetype) 
2. See [:material-code-braces: SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef](./type_defs.md#salesforcestandardknowledgearticletypeconfigurationoutputtypedef) 
3. See [:material-code-braces: SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef](./type_defs.md#salesforcecustomknowledgearticletypeconfigurationoutputtypedef) 
## ServiceNowConfigurationOutputTypeDef

```python
# ServiceNowConfigurationOutputTypeDef definition

class ServiceNowConfigurationOutputTypeDef(TypedDict):
    HostUrl: str,
    SecretArn: str,
    ServiceNowBuildVersion: ServiceNowBuildVersionTypeType,  # (1)
    KnowledgeArticleConfiguration: NotRequired[ServiceNowKnowledgeArticleConfigurationOutputTypeDef],  # (2)
    ServiceCatalogConfiguration: NotRequired[ServiceNowServiceCatalogConfigurationOutputTypeDef],  # (3)
    AuthenticationType: NotRequired[ServiceNowAuthenticationTypeType],  # (4)
```

1. See [:material-code-brackets: ServiceNowBuildVersionTypeType](./literals.md#servicenowbuildversiontypetype) 
2. See [:material-code-braces: ServiceNowKnowledgeArticleConfigurationOutputTypeDef](./type_defs.md#servicenowknowledgearticleconfigurationoutputtypedef) 
3. See [:material-code-braces: ServiceNowServiceCatalogConfigurationOutputTypeDef](./type_defs.md#servicenowservicecatalogconfigurationoutputtypedef) 
4. See [:material-code-brackets: ServiceNowAuthenticationTypeType](./literals.md#servicenowauthenticationtypetype) 
## GitHubConfigurationOutputTypeDef

```python
# GitHubConfigurationOutputTypeDef definition

class GitHubConfigurationOutputTypeDef(TypedDict):
    SecretArn: str,
    SaaSConfiguration: NotRequired[SaaSConfigurationTypeDef],  # (1)
    OnPremiseConfiguration: NotRequired[OnPremiseConfigurationTypeDef],  # (2)
    Type: NotRequired[TypeType],  # (3)
    UseChangeLog: NotRequired[bool],
    GitHubDocumentCrawlProperties: NotRequired[GitHubDocumentCrawlPropertiesTypeDef],  # (4)
    RepositoryFilter: NotRequired[List[str]],
    InclusionFolderNamePatterns: NotRequired[List[str]],
    InclusionFileTypePatterns: NotRequired[List[str]],
    InclusionFileNamePatterns: NotRequired[List[str]],
    ExclusionFolderNamePatterns: NotRequired[List[str]],
    ExclusionFileTypePatterns: NotRequired[List[str]],
    ExclusionFileNamePatterns: NotRequired[List[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (5)
    GitHubRepositoryConfigurationFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubCommitConfigurationFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubIssueDocumentConfigurationFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubIssueCommentConfigurationFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubIssueAttachmentConfigurationFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubPullRequestCommentConfigurationFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubPullRequestDocumentConfigurationFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubPullRequestDocumentAttachmentConfigurationFieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (6)
```

1. See [:material-code-braces: SaaSConfigurationTypeDef](./type_defs.md#saasconfigurationtypedef) 
2. See [:material-code-braces: OnPremiseConfigurationTypeDef](./type_defs.md#onpremiseconfigurationtypedef) 
3. See [:material-code-brackets: TypeType](./literals.md#typetype) 
4. See [:material-code-braces: GitHubDocumentCrawlPropertiesTypeDef](./type_defs.md#githubdocumentcrawlpropertiestypedef) 
5. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
6. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
7. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
8. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
9. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
10. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
11. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
12. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
13. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## OneDriveConfigurationOutputTypeDef

```python
# OneDriveConfigurationOutputTypeDef definition

class OneDriveConfigurationOutputTypeDef(TypedDict):
    TenantDomain: str,
    SecretArn: str,
    OneDriveUsers: OneDriveUsersOutputTypeDef,  # (1)
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    FieldMappings: NotRequired[List[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    DisableLocalGroups: NotRequired[bool],
```

1. See [:material-code-braces: OneDriveUsersOutputTypeDef](./type_defs.md#onedriveusersoutputtypedef) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## DescribeQuerySuggestionsConfigResponseTypeDef

```python
# DescribeQuerySuggestionsConfigResponseTypeDef definition

class DescribeQuerySuggestionsConfigResponseTypeDef(TypedDict):
    Mode: ModeType,  # (1)
    Status: QuerySuggestionsStatusType,  # (2)
    QueryLogLookBackWindowInDays: int,
    IncludeQueriesWithoutUserInformation: bool,
    MinimumNumberOfQueryingUsers: int,
    MinimumQueryCount: int,
    LastSuggestionsBuildTime: datetime,
    LastClearTime: datetime,
    TotalSuggestionsCount: int,
    AttributeSuggestionsConfig: AttributeSuggestionsDescribeConfigTypeDef,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ModeType](./literals.md#modetype) 
2. See [:material-code-brackets: QuerySuggestionsStatusType](./literals.md#querysuggestionsstatustype) 
3. See [:material-code-braces: AttributeSuggestionsDescribeConfigTypeDef](./type_defs.md#attributesuggestionsdescribeconfigtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateQuerySuggestionsConfigRequestRequestTypeDef

```python
# UpdateQuerySuggestionsConfigRequestRequestTypeDef definition

class UpdateQuerySuggestionsConfigRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Mode: NotRequired[ModeType],  # (1)
    QueryLogLookBackWindowInDays: NotRequired[int],
    IncludeQueriesWithoutUserInformation: NotRequired[bool],
    MinimumNumberOfQueryingUsers: NotRequired[int],
    MinimumQueryCount: NotRequired[int],
    AttributeSuggestionsConfig: NotRequired[AttributeSuggestionsUpdateConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ModeType](./literals.md#modetype) 
2. See [:material-code-braces: AttributeSuggestionsUpdateConfigTypeDef](./type_defs.md#attributesuggestionsupdateconfigtypedef) 
## SubmitFeedbackRequestRequestTypeDef

```python
# SubmitFeedbackRequestRequestTypeDef definition

class SubmitFeedbackRequestRequestTypeDef(TypedDict):
    IndexId: str,
    QueryId: str,
    ClickFeedbackItems: NotRequired[Sequence[ClickFeedbackTypeDef]],  # (1)
    RelevanceFeedbackItems: NotRequired[Sequence[RelevanceFeedbackTypeDef]],  # (2)
```

1. See [:material-code-braces: ClickFeedbackTypeDef](./type_defs.md#clickfeedbacktypedef) 
2. See [:material-code-braces: RelevanceFeedbackTypeDef](./type_defs.md#relevancefeedbacktypedef) 
## ListDataSourceSyncJobsRequestRequestTypeDef

```python
# ListDataSourceSyncJobsRequestRequestTypeDef definition

class ListDataSourceSyncJobsRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    StartTimeFilter: NotRequired[TimeRangeTypeDef],  # (1)
    StatusFilter: NotRequired[DataSourceSyncJobStatusType],  # (2)
```

1. See [:material-code-braces: TimeRangeTypeDef](./type_defs.md#timerangetypedef) 
2. See [:material-code-brackets: DataSourceSyncJobStatusType](./literals.md#datasourcesyncjobstatustype) 
## ConfluenceConfigurationOutputTypeDef

```python
# ConfluenceConfigurationOutputTypeDef definition

class ConfluenceConfigurationOutputTypeDef(TypedDict):
    ServerUrl: str,
    SecretArn: str,
    Version: ConfluenceVersionType,  # (1)
    SpaceConfiguration: NotRequired[ConfluenceSpaceConfigurationOutputTypeDef],  # (2)
    PageConfiguration: NotRequired[ConfluencePageConfigurationOutputTypeDef],  # (3)
    BlogConfiguration: NotRequired[ConfluenceBlogConfigurationOutputTypeDef],  # (4)
    AttachmentConfiguration: NotRequired[ConfluenceAttachmentConfigurationOutputTypeDef],  # (5)
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationOutputTypeDef],  # (6)
    InclusionPatterns: NotRequired[List[str]],
    ExclusionPatterns: NotRequired[List[str]],
    ProxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (7)
    AuthenticationType: NotRequired[ConfluenceAuthenticationTypeType],  # (8)
```

1. See [:material-code-brackets: ConfluenceVersionType](./literals.md#confluenceversiontype) 
2. See [:material-code-braces: ConfluenceSpaceConfigurationOutputTypeDef](./type_defs.md#confluencespaceconfigurationoutputtypedef) 
3. See [:material-code-braces: ConfluencePageConfigurationOutputTypeDef](./type_defs.md#confluencepageconfigurationoutputtypedef) 
4. See [:material-code-braces: ConfluenceBlogConfigurationOutputTypeDef](./type_defs.md#confluenceblogconfigurationoutputtypedef) 
5. See [:material-code-braces: ConfluenceAttachmentConfigurationOutputTypeDef](./type_defs.md#confluenceattachmentconfigurationoutputtypedef) 
6. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
7. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
8. See [:material-code-brackets: ConfluenceAuthenticationTypeType](./literals.md#confluenceauthenticationtypetype) 
## ExperienceConfigurationTypeDef

```python
# ExperienceConfigurationTypeDef definition

class ExperienceConfigurationTypeDef(TypedDict):
    ContentSourceConfiguration: NotRequired[ContentSourceConfigurationUnionTypeDef],  # (1)
    UserIdentityConfiguration: NotRequired[UserIdentityConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ContentSourceConfigurationTypeDef](./type_defs.md#contentsourceconfigurationtypedef) [:material-code-braces: ContentSourceConfigurationOutputTypeDef](./type_defs.md#contentsourceconfigurationoutputtypedef) 
2. See [:material-code-braces: UserIdentityConfigurationTypeDef](./type_defs.md#useridentityconfigurationtypedef) 
## DescribeAccessControlConfigurationResponseTypeDef

```python
# DescribeAccessControlConfigurationResponseTypeDef definition

class DescribeAccessControlConfigurationResponseTypeDef(TypedDict):
    Name: str,
    Description: str,
    ErrorMessage: str,
    AccessControlList: List[PrincipalTypeDef],  # (1)
    HierarchicalAccessControlList: List[HierarchicalPrincipalOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
2. See [:material-code-braces: HierarchicalPrincipalOutputTypeDef](./type_defs.md#hierarchicalprincipaloutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccessControlConfigurationRequestRequestTypeDef

```python
# UpdateAccessControlConfigurationRequestRequestTypeDef definition

class UpdateAccessControlConfigurationRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Id: str,
    Name: NotRequired[str],
    Description: NotRequired[str],
    AccessControlList: NotRequired[Sequence[PrincipalTypeDef]],  # (1)
    HierarchicalAccessControlList: NotRequired[Sequence[HierarchicalPrincipalTypeDef]],  # (2)
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
2. See [:material-code-braces: HierarchicalPrincipalTypeDef](./type_defs.md#hierarchicalprincipaltypedef) 
## AlfrescoConfigurationTypeDef

```python
# AlfrescoConfigurationTypeDef definition

class AlfrescoConfigurationTypeDef(TypedDict):
    SiteUrl: str,
    SiteId: str,
    SecretArn: str,
    SslCertificateS3Path: S3PathTypeDef,  # (1)
    CrawlSystemFolders: NotRequired[bool],
    CrawlComments: NotRequired[bool],
    EntityFilter: NotRequired[Sequence[AlfrescoEntityType]],  # (2)
    DocumentLibraryFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (3)
    BlogFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (3)
    WikiFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (3)
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (6)
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
2. See [:material-code-brackets: AlfrescoEntityType](./literals.md#alfrescoentitytype) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
5. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
6. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
## BoxConfigurationTypeDef

```python
# BoxConfigurationTypeDef definition

class BoxConfigurationTypeDef(TypedDict):
    EnterpriseId: str,
    SecretArn: str,
    UseChangeLog: NotRequired[bool],
    CrawlComments: NotRequired[bool],
    CrawlTasks: NotRequired[bool],
    CrawlWebLinks: NotRequired[bool],
    FileFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    TaskFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    CommentFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    WebLinkFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (5)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
5. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
## FsxConfigurationTypeDef

```python
# FsxConfigurationTypeDef definition

class FsxConfigurationTypeDef(TypedDict):
    FileSystemId: str,
    FileSystemType: FsxFileSystemTypeType,  # (1)
    VpcConfiguration: DataSourceVpcConfigurationUnionTypeDef,  # (2)
    SecretArn: NotRequired[str],
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (3)
```

1. See [:material-code-brackets: FsxFileSystemTypeType](./literals.md#fsxfilesystemtypetype) 
2. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## GitHubConfigurationTypeDef

```python
# GitHubConfigurationTypeDef definition

class GitHubConfigurationTypeDef(TypedDict):
    SecretArn: str,
    SaaSConfiguration: NotRequired[SaaSConfigurationTypeDef],  # (1)
    OnPremiseConfiguration: NotRequired[OnPremiseConfigurationTypeDef],  # (2)
    Type: NotRequired[TypeType],  # (3)
    UseChangeLog: NotRequired[bool],
    GitHubDocumentCrawlProperties: NotRequired[GitHubDocumentCrawlPropertiesTypeDef],  # (4)
    RepositoryFilter: NotRequired[Sequence[str]],
    InclusionFolderNamePatterns: NotRequired[Sequence[str]],
    InclusionFileTypePatterns: NotRequired[Sequence[str]],
    InclusionFileNamePatterns: NotRequired[Sequence[str]],
    ExclusionFolderNamePatterns: NotRequired[Sequence[str]],
    ExclusionFileTypePatterns: NotRequired[Sequence[str]],
    ExclusionFileNamePatterns: NotRequired[Sequence[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (5)
    GitHubRepositoryConfigurationFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubCommitConfigurationFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubIssueDocumentConfigurationFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubIssueCommentConfigurationFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubIssueAttachmentConfigurationFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubPullRequestCommentConfigurationFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubPullRequestDocumentConfigurationFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (6)
    GitHubPullRequestDocumentAttachmentConfigurationFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (6)
```

1. See [:material-code-braces: SaaSConfigurationTypeDef](./type_defs.md#saasconfigurationtypedef) 
2. See [:material-code-braces: OnPremiseConfigurationTypeDef](./type_defs.md#onpremiseconfigurationtypedef) 
3. See [:material-code-brackets: TypeType](./literals.md#typetype) 
4. See [:material-code-braces: GitHubDocumentCrawlPropertiesTypeDef](./type_defs.md#githubdocumentcrawlpropertiestypedef) 
5. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
6. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
7. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
8. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
9. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
10. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
11. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
12. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
13. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## JiraConfigurationTypeDef

```python
# JiraConfigurationTypeDef definition

class JiraConfigurationTypeDef(TypedDict):
    JiraAccountUrl: str,
    SecretArn: str,
    UseChangeLog: NotRequired[bool],
    Project: NotRequired[Sequence[str]],
    IssueType: NotRequired[Sequence[str]],
    Status: NotRequired[Sequence[str]],
    IssueSubEntityFilter: NotRequired[Sequence[IssueSubEntityType]],  # (1)
    AttachmentFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    CommentFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    IssueFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    ProjectFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    WorkLogFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (7)
```

1. See [:material-code-brackets: IssueSubEntityType](./literals.md#issuesubentitytype) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
5. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
6. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
7. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
## QuipConfigurationTypeDef

```python
# QuipConfigurationTypeDef definition

class QuipConfigurationTypeDef(TypedDict):
    Domain: str,
    SecretArn: str,
    CrawlFileComments: NotRequired[bool],
    CrawlChatRooms: NotRequired[bool],
    CrawlAttachments: NotRequired[bool],
    FolderIds: NotRequired[Sequence[str]],
    ThreadFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    MessageFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    AttachmentFieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (1)
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (4)
```

1. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
## SharePointConfigurationTypeDef

```python
# SharePointConfigurationTypeDef definition

class SharePointConfigurationTypeDef(TypedDict):
    SharePointVersion: SharePointVersionType,  # (1)
    Urls: Sequence[str],
    SecretArn: str,
    CrawlAttachments: NotRequired[bool],
    UseChangeLog: NotRequired[bool],
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (2)
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (3)
    DocumentTitleFieldName: NotRequired[str],
    DisableLocalGroups: NotRequired[bool],
    SslCertificateS3Path: NotRequired[S3PathTypeDef],  # (4)
    AuthenticationType: NotRequired[SharePointOnlineAuthenticationTypeType],  # (5)
    ProxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: SharePointVersionType](./literals.md#sharepointversiontype) 
2. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
4. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
5. See [:material-code-brackets: SharePointOnlineAuthenticationTypeType](./literals.md#sharepointonlineauthenticationtypetype) 
6. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
## SlackConfigurationTypeDef

```python
# SlackConfigurationTypeDef definition

class SlackConfigurationTypeDef(TypedDict):
    TeamId: str,
    SecretArn: str,
    SlackEntityList: Sequence[SlackEntityType],  # (2)
    SinceCrawlDate: str,
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (1)
    UseChangeLog: NotRequired[bool],
    CrawlBotMessage: NotRequired[bool],
    ExcludeArchived: NotRequired[bool],
    LookBackPeriod: NotRequired[int],
    PrivateChannelFilter: NotRequired[Sequence[str]],
    PublicChannelFilter: NotRequired[Sequence[str]],
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (3)
```

1. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
2. See [:material-code-brackets: SlackEntityType](./literals.md#slackentitytype) 
3. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## CreateFeaturedResultsSetResponseTypeDef

```python
# CreateFeaturedResultsSetResponseTypeDef definition

class CreateFeaturedResultsSetResponseTypeDef(TypedDict):
    FeaturedResultsSet: FeaturedResultsSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeaturedResultsSetTypeDef](./type_defs.md#featuredresultssettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateFeaturedResultsSetResponseTypeDef

```python
# UpdateFeaturedResultsSetResponseTypeDef definition

class UpdateFeaturedResultsSetResponseTypeDef(TypedDict):
    FeaturedResultsSet: FeaturedResultsSetTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FeaturedResultsSetTypeDef](./type_defs.md#featuredresultssettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSourceSyncJobsResponseTypeDef

```python
# ListDataSourceSyncJobsResponseTypeDef definition

class ListDataSourceSyncJobsResponseTypeDef(TypedDict):
    History: List[DataSourceSyncJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceSyncJobTypeDef](./type_defs.md#datasourcesyncjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExperiencesResponseTypeDef

```python
# ListExperiencesResponseTypeDef definition

class ListExperiencesResponseTypeDef(TypedDict):
    SummaryItems: List[ExperiencesSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExperiencesSummaryTypeDef](./type_defs.md#experiencessummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## HookConfigurationOutputTypeDef

```python
# HookConfigurationOutputTypeDef definition

class HookConfigurationOutputTypeDef(TypedDict):
    LambdaArn: str,
    S3Bucket: str,
    InvocationCondition: NotRequired[DocumentAttributeConditionOutputTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 
## RetrieveResultItemTypeDef

```python
# RetrieveResultItemTypeDef definition

class RetrieveResultItemTypeDef(TypedDict):
    Id: NotRequired[str],
    DocumentId: NotRequired[str],
    DocumentTitle: NotRequired[str],
    Content: NotRequired[str],
    DocumentURI: NotRequired[str],
    DocumentAttributes: NotRequired[List[DocumentAttributeOutputTypeDef]],  # (1)
    ScoreAttributes: NotRequired[ScoreAttributesTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
2. See [:material-code-braces: ScoreAttributesTypeDef](./type_defs.md#scoreattributestypedef) 
## SourceDocumentTypeDef

```python
# SourceDocumentTypeDef definition

class SourceDocumentTypeDef(TypedDict):
    DocumentId: NotRequired[str],
    SuggestionAttributes: NotRequired[List[str]],
    AdditionalAttributes: NotRequired[List[DocumentAttributeOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
## InlineCustomDocumentEnrichmentConfigurationOutputTypeDef

```python
# InlineCustomDocumentEnrichmentConfigurationOutputTypeDef definition

class InlineCustomDocumentEnrichmentConfigurationOutputTypeDef(TypedDict):
    Condition: NotRequired[DocumentAttributeConditionOutputTypeDef],  # (1)
    Target: NotRequired[DocumentAttributeTargetOutputTypeDef],  # (2)
    DocumentContentDeletion: NotRequired[bool],
```

1. See [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 
2. See [:material-code-braces: DocumentAttributeTargetOutputTypeDef](./type_defs.md#documentattributetargetoutputtypedef) 
## FacetResultTypeDef

```python
# FacetResultTypeDef definition

class FacetResultTypeDef(TypedDict):
    DocumentAttributeKey: NotRequired[str],
    DocumentAttributeValueType: NotRequired[DocumentAttributeValueTypeType],  # (1)
    DocumentAttributeValueCountPairs: NotRequired[List[DocumentAttributeValueCountPairTypeDef]],  # (2)
```

1. See [:material-code-brackets: DocumentAttributeValueTypeType](./literals.md#documentattributevaluetypetype) 
2. See [:material-code-braces: DocumentAttributeValueCountPairTypeDef](./type_defs.md#documentattributevaluecountpairtypedef) 
## ListExperienceEntitiesResponseTypeDef

```python
# ListExperienceEntitiesResponseTypeDef definition

class ListExperienceEntitiesResponseTypeDef(TypedDict):
    SummaryItems: List[ExperienceEntitiesSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ExperienceEntitiesSummaryTypeDef](./type_defs.md#experienceentitiessummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExperienceResponseTypeDef

```python
# DescribeExperienceResponseTypeDef definition

class DescribeExperienceResponseTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    Name: str,
    Endpoints: List[ExperienceEndpointTypeDef],  # (1)
    Configuration: ExperienceConfigurationOutputTypeDef,  # (2)
    CreatedAt: datetime,
    UpdatedAt: datetime,
    Description: str,
    Status: ExperienceStatusType,  # (3)
    RoleArn: str,
    ErrorMessage: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ExperienceEndpointTypeDef](./type_defs.md#experienceendpointtypedef) 
2. See [:material-code-braces: ExperienceConfigurationOutputTypeDef](./type_defs.md#experienceconfigurationoutputtypedef) 
3. See [:material-code-brackets: ExperienceStatusType](./literals.md#experiencestatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutPrincipalMappingRequestRequestTypeDef

```python
# PutPrincipalMappingRequestRequestTypeDef definition

class PutPrincipalMappingRequestRequestTypeDef(TypedDict):
    IndexId: str,
    GroupId: str,
    GroupMembers: GroupMembersTypeDef,  # (1)
    DataSourceId: NotRequired[str],
    OrderingId: NotRequired[int],
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: GroupMembersTypeDef](./type_defs.md#groupmemberstypedef) 
## AdditionalResultAttributeValueTypeDef

```python
# AdditionalResultAttributeValueTypeDef definition

class AdditionalResultAttributeValueTypeDef(TypedDict):
    TextWithHighlightsValue: NotRequired[TextWithHighlightsTypeDef],  # (1)
```

1. See [:material-code-braces: TextWithHighlightsTypeDef](./type_defs.md#textwithhighlightstypedef) 
## ExpandedResultItemTypeDef

```python
# ExpandedResultItemTypeDef definition

class ExpandedResultItemTypeDef(TypedDict):
    Id: NotRequired[str],
    DocumentId: NotRequired[str],
    DocumentTitle: NotRequired[TextWithHighlightsTypeDef],  # (1)
    DocumentExcerpt: NotRequired[TextWithHighlightsTypeDef],  # (1)
    DocumentURI: NotRequired[str],
    DocumentAttributes: NotRequired[List[DocumentAttributeOutputTypeDef]],  # (3)
```

1. See [:material-code-braces: TextWithHighlightsTypeDef](./type_defs.md#textwithhighlightstypedef) 
2. See [:material-code-braces: TextWithHighlightsTypeDef](./type_defs.md#textwithhighlightstypedef) 
3. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
## CreateIndexRequestRequestTypeDef

```python
# CreateIndexRequestRequestTypeDef definition

class CreateIndexRequestRequestTypeDef(TypedDict):
    Name: str,
    RoleArn: str,
    Edition: NotRequired[IndexEditionType],  # (1)
    ServerSideEncryptionConfiguration: NotRequired[ServerSideEncryptionConfigurationTypeDef],  # (2)
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    UserTokenConfigurations: NotRequired[Sequence[UserTokenConfigurationTypeDef]],  # (4)
    UserContextPolicy: NotRequired[UserContextPolicyType],  # (5)
    UserGroupResolutionConfiguration: NotRequired[UserGroupResolutionConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: IndexEditionType](./literals.md#indexeditiontype) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: UserTokenConfigurationTypeDef](./type_defs.md#usertokenconfigurationtypedef) 
5. See [:material-code-brackets: UserContextPolicyType](./literals.md#usercontextpolicytype) 
6. See [:material-code-braces: UserGroupResolutionConfigurationTypeDef](./type_defs.md#usergroupresolutionconfigurationtypedef) 
## DescribeIndexResponseTypeDef

```python
# DescribeIndexResponseTypeDef definition

class DescribeIndexResponseTypeDef(TypedDict):
    Name: str,
    Id: str,
    Edition: IndexEditionType,  # (1)
    RoleArn: str,
    ServerSideEncryptionConfiguration: ServerSideEncryptionConfigurationTypeDef,  # (2)
    Status: IndexStatusType,  # (3)
    Description: str,
    CreatedAt: datetime,
    UpdatedAt: datetime,
    DocumentMetadataConfigurations: List[DocumentMetadataConfigurationOutputTypeDef],  # (4)
    IndexStatistics: IndexStatisticsTypeDef,  # (5)
    ErrorMessage: str,
    CapacityUnits: CapacityUnitsConfigurationTypeDef,  # (6)
    UserTokenConfigurations: List[UserTokenConfigurationTypeDef],  # (7)
    UserContextPolicy: UserContextPolicyType,  # (8)
    UserGroupResolutionConfiguration: UserGroupResolutionConfigurationTypeDef,  # (9)
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-brackets: IndexEditionType](./literals.md#indexeditiontype) 
2. See [:material-code-braces: ServerSideEncryptionConfigurationTypeDef](./type_defs.md#serversideencryptionconfigurationtypedef) 
3. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
4. See [:material-code-braces: DocumentMetadataConfigurationOutputTypeDef](./type_defs.md#documentmetadataconfigurationoutputtypedef) 
5. See [:material-code-braces: IndexStatisticsTypeDef](./type_defs.md#indexstatisticstypedef) 
6. See [:material-code-braces: CapacityUnitsConfigurationTypeDef](./type_defs.md#capacityunitsconfigurationtypedef) 
7. See [:material-code-braces: UserTokenConfigurationTypeDef](./type_defs.md#usertokenconfigurationtypedef) 
8. See [:material-code-brackets: UserContextPolicyType](./literals.md#usercontextpolicytype) 
9. See [:material-code-braces: UserGroupResolutionConfigurationTypeDef](./type_defs.md#usergroupresolutionconfigurationtypedef) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DocumentMetadataConfigurationTypeDef

```python
# DocumentMetadataConfigurationTypeDef definition

class DocumentMetadataConfigurationTypeDef(TypedDict):
    Name: str,
    Type: DocumentAttributeValueTypeType,  # (1)
    Relevance: NotRequired[RelevanceUnionTypeDef],  # (2)
    Search: NotRequired[SearchTypeDef],  # (3)
```

1. See [:material-code-brackets: DocumentAttributeValueTypeType](./literals.md#documentattributevaluetypetype) 
2. See [:material-code-braces: RelevanceTypeDef](./type_defs.md#relevancetypedef) [:material-code-braces: RelevanceOutputTypeDef](./type_defs.md#relevanceoutputtypedef) 
3. See [:material-code-braces: SearchTypeDef](./type_defs.md#searchtypedef) 
## DocumentRelevanceConfigurationTypeDef

```python
# DocumentRelevanceConfigurationTypeDef definition

class DocumentRelevanceConfigurationTypeDef(TypedDict):
    Name: str,
    Relevance: RelevanceUnionTypeDef,  # (1)
```

1. See [:material-code-braces: RelevanceTypeDef](./type_defs.md#relevancetypedef) [:material-code-braces: RelevanceOutputTypeDef](./type_defs.md#relevanceoutputtypedef) 
## WebCrawlerConfigurationOutputTypeDef

```python
# WebCrawlerConfigurationOutputTypeDef definition

class WebCrawlerConfigurationOutputTypeDef(TypedDict):
    Urls: UrlsOutputTypeDef,  # (1)
    CrawlDepth: NotRequired[int],
    MaxLinksPerPage: NotRequired[int],
    MaxContentSizePerPageInMegaBytes: NotRequired[float],
    MaxUrlsPerMinuteCrawlRate: NotRequired[int],
    UrlInclusionPatterns: NotRequired[List[str]],
    UrlExclusionPatterns: NotRequired[List[str]],
    ProxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (2)
    AuthenticationConfiguration: NotRequired[AuthenticationConfigurationOutputTypeDef],  # (3)
```

1. See [:material-code-braces: UrlsOutputTypeDef](./type_defs.md#urlsoutputtypedef) 
2. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
3. See [:material-code-braces: AuthenticationConfigurationOutputTypeDef](./type_defs.md#authenticationconfigurationoutputtypedef) 
## UrlsTypeDef

```python
# UrlsTypeDef definition

class UrlsTypeDef(TypedDict):
    SeedUrlConfiguration: NotRequired[SeedUrlConfigurationUnionTypeDef],  # (1)
    SiteMapsConfiguration: NotRequired[SiteMapsConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: SeedUrlConfigurationTypeDef](./type_defs.md#seedurlconfigurationtypedef) [:material-code-braces: SeedUrlConfigurationOutputTypeDef](./type_defs.md#seedurlconfigurationoutputtypedef) 
2. See [:material-code-braces: SiteMapsConfigurationTypeDef](./type_defs.md#sitemapsconfigurationtypedef) [:material-code-braces: SiteMapsConfigurationOutputTypeDef](./type_defs.md#sitemapsconfigurationoutputtypedef) 
## SuggestionValueTypeDef

```python
# SuggestionValueTypeDef definition

class SuggestionValueTypeDef(TypedDict):
    Text: NotRequired[SuggestionTextWithHighlightsTypeDef],  # (1)
```

1. See [:material-code-braces: SuggestionTextWithHighlightsTypeDef](./type_defs.md#suggestiontextwithhighlightstypedef) 
## TableExcerptTypeDef

```python
# TableExcerptTypeDef definition

class TableExcerptTypeDef(TypedDict):
    Rows: NotRequired[List[TableRowTypeDef]],  # (1)
    TotalNumberOfRows: NotRequired[int],
```

1. See [:material-code-braces: TableRowTypeDef](./type_defs.md#tablerowtypedef) 
## DatabaseConfigurationTypeDef

```python
# DatabaseConfigurationTypeDef definition

class DatabaseConfigurationTypeDef(TypedDict):
    DatabaseEngineType: DatabaseEngineTypeType,  # (1)
    ConnectionConfiguration: ConnectionConfigurationTypeDef,  # (2)
    ColumnConfiguration: ColumnConfigurationUnionTypeDef,  # (4)
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (3)
    AclConfiguration: NotRequired[AclConfigurationTypeDef],  # (5)
    SqlConfiguration: NotRequired[SqlConfigurationTypeDef],  # (6)
```

1. See [:material-code-brackets: DatabaseEngineTypeType](./literals.md#databaseenginetypetype) 
2. See [:material-code-braces: ConnectionConfigurationTypeDef](./type_defs.md#connectionconfigurationtypedef) 
3. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
4. See [:material-code-braces: ColumnConfigurationTypeDef](./type_defs.md#columnconfigurationtypedef) [:material-code-braces: ColumnConfigurationOutputTypeDef](./type_defs.md#columnconfigurationoutputtypedef) 
5. See [:material-code-braces: AclConfigurationTypeDef](./type_defs.md#aclconfigurationtypedef) 
6. See [:material-code-braces: SqlConfigurationTypeDef](./type_defs.md#sqlconfigurationtypedef) 
## SalesforceConfigurationOutputTypeDef

```python
# SalesforceConfigurationOutputTypeDef definition

class SalesforceConfigurationOutputTypeDef(TypedDict):
    ServerUrl: str,
    SecretArn: str,
    StandardObjectConfigurations: NotRequired[List[SalesforceStandardObjectConfigurationOutputTypeDef]],  # (1)
    KnowledgeArticleConfiguration: NotRequired[SalesforceKnowledgeArticleConfigurationOutputTypeDef],  # (2)
    ChatterFeedConfiguration: NotRequired[SalesforceChatterFeedConfigurationOutputTypeDef],  # (3)
    CrawlAttachments: NotRequired[bool],
    StandardObjectAttachmentConfiguration: NotRequired[SalesforceStandardObjectAttachmentConfigurationOutputTypeDef],  # (4)
    IncludeAttachmentFilePatterns: NotRequired[List[str]],
    ExcludeAttachmentFilePatterns: NotRequired[List[str]],
```

1. See [:material-code-braces: SalesforceStandardObjectConfigurationOutputTypeDef](./type_defs.md#salesforcestandardobjectconfigurationoutputtypedef) 
2. See [:material-code-braces: SalesforceKnowledgeArticleConfigurationOutputTypeDef](./type_defs.md#salesforceknowledgearticleconfigurationoutputtypedef) 
3. See [:material-code-braces: SalesforceChatterFeedConfigurationOutputTypeDef](./type_defs.md#salesforcechatterfeedconfigurationoutputtypedef) 
4. See [:material-code-braces: SalesforceStandardObjectAttachmentConfigurationOutputTypeDef](./type_defs.md#salesforcestandardobjectattachmentconfigurationoutputtypedef) 
## SalesforceKnowledgeArticleConfigurationTypeDef

```python
# SalesforceKnowledgeArticleConfigurationTypeDef definition

class SalesforceKnowledgeArticleConfigurationTypeDef(TypedDict):
    IncludedStates: Sequence[SalesforceKnowledgeArticleStateType],  # (1)
    StandardKnowledgeArticleTypeConfiguration: NotRequired[SalesforceStandardKnowledgeArticleTypeConfigurationUnionTypeDef],  # (2)
    CustomKnowledgeArticleTypeConfigurations: NotRequired[Sequence[SalesforceCustomKnowledgeArticleTypeConfigurationUnionTypeDef]],  # (3)
```

1. See [:material-code-brackets: SalesforceKnowledgeArticleStateType](./literals.md#salesforceknowledgearticlestatetype) 
2. See [:material-code-braces: SalesforceStandardKnowledgeArticleTypeConfigurationTypeDef](./type_defs.md#salesforcestandardknowledgearticletypeconfigurationtypedef) [:material-code-braces: SalesforceStandardKnowledgeArticleTypeConfigurationOutputTypeDef](./type_defs.md#salesforcestandardknowledgearticletypeconfigurationoutputtypedef) 
3. See [:material-code-braces: SalesforceCustomKnowledgeArticleTypeConfigurationTypeDef](./type_defs.md#salesforcecustomknowledgearticletypeconfigurationtypedef) [:material-code-braces: SalesforceCustomKnowledgeArticleTypeConfigurationOutputTypeDef](./type_defs.md#salesforcecustomknowledgearticletypeconfigurationoutputtypedef) 
## ServiceNowConfigurationTypeDef

```python
# ServiceNowConfigurationTypeDef definition

class ServiceNowConfigurationTypeDef(TypedDict):
    HostUrl: str,
    SecretArn: str,
    ServiceNowBuildVersion: ServiceNowBuildVersionTypeType,  # (1)
    KnowledgeArticleConfiguration: NotRequired[ServiceNowKnowledgeArticleConfigurationUnionTypeDef],  # (2)
    ServiceCatalogConfiguration: NotRequired[ServiceNowServiceCatalogConfigurationUnionTypeDef],  # (3)
    AuthenticationType: NotRequired[ServiceNowAuthenticationTypeType],  # (4)
```

1. See [:material-code-brackets: ServiceNowBuildVersionTypeType](./literals.md#servicenowbuildversiontypetype) 
2. See [:material-code-braces: ServiceNowKnowledgeArticleConfigurationTypeDef](./type_defs.md#servicenowknowledgearticleconfigurationtypedef) [:material-code-braces: ServiceNowKnowledgeArticleConfigurationOutputTypeDef](./type_defs.md#servicenowknowledgearticleconfigurationoutputtypedef) 
3. See [:material-code-braces: ServiceNowServiceCatalogConfigurationTypeDef](./type_defs.md#servicenowservicecatalogconfigurationtypedef) [:material-code-braces: ServiceNowServiceCatalogConfigurationOutputTypeDef](./type_defs.md#servicenowservicecatalogconfigurationoutputtypedef) 
4. See [:material-code-brackets: ServiceNowAuthenticationTypeType](./literals.md#servicenowauthenticationtypetype) 
## OneDriveConfigurationTypeDef

```python
# OneDriveConfigurationTypeDef definition

class OneDriveConfigurationTypeDef(TypedDict):
    TenantDomain: str,
    SecretArn: str,
    OneDriveUsers: OneDriveUsersUnionTypeDef,  # (1)
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    FieldMappings: NotRequired[Sequence[DataSourceToIndexFieldMappingTypeDef]],  # (2)
    DisableLocalGroups: NotRequired[bool],
```

1. See [:material-code-braces: OneDriveUsersTypeDef](./type_defs.md#onedriveuserstypedef) [:material-code-braces: OneDriveUsersOutputTypeDef](./type_defs.md#onedriveusersoutputtypedef) 
2. See [:material-code-braces: DataSourceToIndexFieldMappingTypeDef](./type_defs.md#datasourcetoindexfieldmappingtypedef) 
## DocumentAttributeConditionTypeDef

```python
# DocumentAttributeConditionTypeDef definition

class DocumentAttributeConditionTypeDef(TypedDict):
    ConditionDocumentAttributeKey: str,
    Operator: ConditionOperatorType,  # (1)
    ConditionOnValue: NotRequired[DocumentAttributeValueUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: ConditionOperatorType](./literals.md#conditionoperatortype) 
2. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentAttributeTargetTypeDef

```python
# DocumentAttributeTargetTypeDef definition

class DocumentAttributeTargetTypeDef(TypedDict):
    TargetDocumentAttributeKey: NotRequired[str],
    TargetDocumentAttributeValueDeletion: NotRequired[bool],
    TargetDocumentAttributeValue: NotRequired[DocumentAttributeValueUnionTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## DocumentAttributeTypeDef

```python
# DocumentAttributeTypeDef definition

class DocumentAttributeTypeDef(TypedDict):
    Key: str,
    Value: DocumentAttributeValueUnionTypeDef,  # (1)
```

1. See [:material-code-braces: DocumentAttributeValueTypeDef](./type_defs.md#documentattributevaluetypedef) [:material-code-braces: DocumentAttributeValueOutputTypeDef](./type_defs.md#documentattributevalueoutputtypedef) 
## ConfluenceConfigurationTypeDef

```python
# ConfluenceConfigurationTypeDef definition

class ConfluenceConfigurationTypeDef(TypedDict):
    ServerUrl: str,
    SecretArn: str,
    Version: ConfluenceVersionType,  # (1)
    SpaceConfiguration: NotRequired[ConfluenceSpaceConfigurationUnionTypeDef],  # (2)
    PageConfiguration: NotRequired[ConfluencePageConfigurationUnionTypeDef],  # (3)
    BlogConfiguration: NotRequired[ConfluenceBlogConfigurationUnionTypeDef],  # (4)
    AttachmentConfiguration: NotRequired[ConfluenceAttachmentConfigurationUnionTypeDef],  # (5)
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationUnionTypeDef],  # (6)
    InclusionPatterns: NotRequired[Sequence[str]],
    ExclusionPatterns: NotRequired[Sequence[str]],
    ProxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (7)
    AuthenticationType: NotRequired[ConfluenceAuthenticationTypeType],  # (8)
```

1. See [:material-code-brackets: ConfluenceVersionType](./literals.md#confluenceversiontype) 
2. See [:material-code-braces: ConfluenceSpaceConfigurationTypeDef](./type_defs.md#confluencespaceconfigurationtypedef) [:material-code-braces: ConfluenceSpaceConfigurationOutputTypeDef](./type_defs.md#confluencespaceconfigurationoutputtypedef) 
3. See [:material-code-braces: ConfluencePageConfigurationTypeDef](./type_defs.md#confluencepageconfigurationtypedef) [:material-code-braces: ConfluencePageConfigurationOutputTypeDef](./type_defs.md#confluencepageconfigurationoutputtypedef) 
4. See [:material-code-braces: ConfluenceBlogConfigurationTypeDef](./type_defs.md#confluenceblogconfigurationtypedef) [:material-code-braces: ConfluenceBlogConfigurationOutputTypeDef](./type_defs.md#confluenceblogconfigurationoutputtypedef) 
5. See [:material-code-braces: ConfluenceAttachmentConfigurationTypeDef](./type_defs.md#confluenceattachmentconfigurationtypedef) [:material-code-braces: ConfluenceAttachmentConfigurationOutputTypeDef](./type_defs.md#confluenceattachmentconfigurationoutputtypedef) 
6. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
7. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
8. See [:material-code-brackets: ConfluenceAuthenticationTypeType](./literals.md#confluenceauthenticationtypetype) 
## CreateExperienceRequestRequestTypeDef

```python
# CreateExperienceRequestRequestTypeDef definition

class CreateExperienceRequestRequestTypeDef(TypedDict):
    Name: str,
    IndexId: str,
    RoleArn: NotRequired[str],
    Configuration: NotRequired[ExperienceConfigurationTypeDef],  # (1)
    Description: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ExperienceConfigurationTypeDef](./type_defs.md#experienceconfigurationtypedef) 
## UpdateExperienceRequestRequestTypeDef

```python
# UpdateExperienceRequestRequestTypeDef definition

class UpdateExperienceRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    Name: NotRequired[str],
    RoleArn: NotRequired[str],
    Configuration: NotRequired[ExperienceConfigurationTypeDef],  # (1)
    Description: NotRequired[str],
```

1. See [:material-code-braces: ExperienceConfigurationTypeDef](./type_defs.md#experienceconfigurationtypedef) 
## CreateAccessControlConfigurationRequestRequestTypeDef

```python
# CreateAccessControlConfigurationRequestRequestTypeDef definition

class CreateAccessControlConfigurationRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Name: str,
    Description: NotRequired[str],
    AccessControlList: NotRequired[Sequence[PrincipalTypeDef]],  # (1)
    HierarchicalAccessControlList: NotRequired[Sequence[HierarchicalPrincipalUnionTypeDef]],  # (2)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
2. See [:material-code-braces: HierarchicalPrincipalTypeDef](./type_defs.md#hierarchicalprincipaltypedef) [:material-code-braces: HierarchicalPrincipalOutputTypeDef](./type_defs.md#hierarchicalprincipaloutputtypedef) 
## RetrieveResultTypeDef

```python
# RetrieveResultTypeDef definition

class RetrieveResultTypeDef(TypedDict):
    QueryId: str,
    ResultItems: List[RetrieveResultItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetrieveResultItemTypeDef](./type_defs.md#retrieveresultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CustomDocumentEnrichmentConfigurationOutputTypeDef

```python
# CustomDocumentEnrichmentConfigurationOutputTypeDef definition

class CustomDocumentEnrichmentConfigurationOutputTypeDef(TypedDict):
    InlineConfigurations: NotRequired[List[InlineCustomDocumentEnrichmentConfigurationOutputTypeDef]],  # (1)
    PreExtractionHookConfiguration: NotRequired[HookConfigurationOutputTypeDef],  # (2)
    PostExtractionHookConfiguration: NotRequired[HookConfigurationOutputTypeDef],  # (2)
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: InlineCustomDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#inlinecustomdocumentenrichmentconfigurationoutputtypedef) 
2. See [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 
3. See [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 
## AdditionalResultAttributeTypeDef

```python
# AdditionalResultAttributeTypeDef definition

class AdditionalResultAttributeTypeDef(TypedDict):
    Key: str,
    ValueType: AdditionalResultAttributeValueTypeType,  # (1)
    Value: AdditionalResultAttributeValueTypeDef,  # (2)
```

1. See [:material-code-brackets: AdditionalResultAttributeValueTypeType](./literals.md#additionalresultattributevaluetypetype) 
2. See [:material-code-braces: AdditionalResultAttributeValueTypeDef](./type_defs.md#additionalresultattributevaluetypedef) 
## CollapsedResultDetailTypeDef

```python
# CollapsedResultDetailTypeDef definition

class CollapsedResultDetailTypeDef(TypedDict):
    DocumentAttribute: DocumentAttributeOutputTypeDef,  # (1)
    ExpandedResults: NotRequired[List[ExpandedResultItemTypeDef]],  # (2)
```

1. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
2. See [:material-code-braces: ExpandedResultItemTypeDef](./type_defs.md#expandedresultitemtypedef) 
## SuggestionTypeDef

```python
# SuggestionTypeDef definition

class SuggestionTypeDef(TypedDict):
    Id: NotRequired[str],
    Value: NotRequired[SuggestionValueTypeDef],  # (1)
    SourceDocuments: NotRequired[List[SourceDocumentTypeDef]],  # (2)
```

1. See [:material-code-braces: SuggestionValueTypeDef](./type_defs.md#suggestionvaluetypedef) 
2. See [:material-code-braces: SourceDocumentTypeDef](./type_defs.md#sourcedocumenttypedef) 
## DataSourceConfigurationOutputTypeDef

```python
# DataSourceConfigurationOutputTypeDef definition

class DataSourceConfigurationOutputTypeDef(TypedDict):
    S3Configuration: NotRequired[S3DataSourceConfigurationOutputTypeDef],  # (1)
    SharePointConfiguration: NotRequired[SharePointConfigurationOutputTypeDef],  # (2)
    DatabaseConfiguration: NotRequired[DatabaseConfigurationOutputTypeDef],  # (3)
    SalesforceConfiguration: NotRequired[SalesforceConfigurationOutputTypeDef],  # (4)
    OneDriveConfiguration: NotRequired[OneDriveConfigurationOutputTypeDef],  # (5)
    ServiceNowConfiguration: NotRequired[ServiceNowConfigurationOutputTypeDef],  # (6)
    ConfluenceConfiguration: NotRequired[ConfluenceConfigurationOutputTypeDef],  # (7)
    GoogleDriveConfiguration: NotRequired[GoogleDriveConfigurationOutputTypeDef],  # (8)
    WebCrawlerConfiguration: NotRequired[WebCrawlerConfigurationOutputTypeDef],  # (9)
    WorkDocsConfiguration: NotRequired[WorkDocsConfigurationOutputTypeDef],  # (10)
    FsxConfiguration: NotRequired[FsxConfigurationOutputTypeDef],  # (11)
    SlackConfiguration: NotRequired[SlackConfigurationOutputTypeDef],  # (12)
    BoxConfiguration: NotRequired[BoxConfigurationOutputTypeDef],  # (13)
    QuipConfiguration: NotRequired[QuipConfigurationOutputTypeDef],  # (14)
    JiraConfiguration: NotRequired[JiraConfigurationOutputTypeDef],  # (15)
    GitHubConfiguration: NotRequired[GitHubConfigurationOutputTypeDef],  # (16)
    AlfrescoConfiguration: NotRequired[AlfrescoConfigurationOutputTypeDef],  # (17)
    TemplateConfiguration: NotRequired[TemplateConfigurationOutputTypeDef],  # (18)
```

1. See [:material-code-braces: S3DataSourceConfigurationOutputTypeDef](./type_defs.md#s3datasourceconfigurationoutputtypedef) 
2. See [:material-code-braces: SharePointConfigurationOutputTypeDef](./type_defs.md#sharepointconfigurationoutputtypedef) 
3. See [:material-code-braces: DatabaseConfigurationOutputTypeDef](./type_defs.md#databaseconfigurationoutputtypedef) 
4. See [:material-code-braces: SalesforceConfigurationOutputTypeDef](./type_defs.md#salesforceconfigurationoutputtypedef) 
5. See [:material-code-braces: OneDriveConfigurationOutputTypeDef](./type_defs.md#onedriveconfigurationoutputtypedef) 
6. See [:material-code-braces: ServiceNowConfigurationOutputTypeDef](./type_defs.md#servicenowconfigurationoutputtypedef) 
7. See [:material-code-braces: ConfluenceConfigurationOutputTypeDef](./type_defs.md#confluenceconfigurationoutputtypedef) 
8. See [:material-code-braces: GoogleDriveConfigurationOutputTypeDef](./type_defs.md#googledriveconfigurationoutputtypedef) 
9. See [:material-code-braces: WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef) 
10. See [:material-code-braces: WorkDocsConfigurationOutputTypeDef](./type_defs.md#workdocsconfigurationoutputtypedef) 
11. See [:material-code-braces: FsxConfigurationOutputTypeDef](./type_defs.md#fsxconfigurationoutputtypedef) 
12. See [:material-code-braces: SlackConfigurationOutputTypeDef](./type_defs.md#slackconfigurationoutputtypedef) 
13. See [:material-code-braces: BoxConfigurationOutputTypeDef](./type_defs.md#boxconfigurationoutputtypedef) 
14. See [:material-code-braces: QuipConfigurationOutputTypeDef](./type_defs.md#quipconfigurationoutputtypedef) 
15. See [:material-code-braces: JiraConfigurationOutputTypeDef](./type_defs.md#jiraconfigurationoutputtypedef) 
16. See [:material-code-braces: GitHubConfigurationOutputTypeDef](./type_defs.md#githubconfigurationoutputtypedef) 
17. See [:material-code-braces: AlfrescoConfigurationOutputTypeDef](./type_defs.md#alfrescoconfigurationoutputtypedef) 
18. See [:material-code-braces: TemplateConfigurationOutputTypeDef](./type_defs.md#templateconfigurationoutputtypedef) 
## FeaturedResultsItemTypeDef

```python
# FeaturedResultsItemTypeDef definition

class FeaturedResultsItemTypeDef(TypedDict):
    Id: NotRequired[str],
    Type: NotRequired[QueryResultTypeType],  # (1)
    AdditionalAttributes: NotRequired[List[AdditionalResultAttributeTypeDef]],  # (2)
    DocumentId: NotRequired[str],
    DocumentTitle: NotRequired[TextWithHighlightsTypeDef],  # (3)
    DocumentExcerpt: NotRequired[TextWithHighlightsTypeDef],  # (3)
    DocumentURI: NotRequired[str],
    DocumentAttributes: NotRequired[List[DocumentAttributeOutputTypeDef]],  # (5)
    FeedbackToken: NotRequired[str],
```

1. See [:material-code-brackets: QueryResultTypeType](./literals.md#queryresulttypetype) 
2. See [:material-code-braces: AdditionalResultAttributeTypeDef](./type_defs.md#additionalresultattributetypedef) 
3. See [:material-code-braces: TextWithHighlightsTypeDef](./type_defs.md#textwithhighlightstypedef) 
4. See [:material-code-braces: TextWithHighlightsTypeDef](./type_defs.md#textwithhighlightstypedef) 
5. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
## QueryResultItemTypeDef

```python
# QueryResultItemTypeDef definition

class QueryResultItemTypeDef(TypedDict):
    Id: NotRequired[str],
    Type: NotRequired[QueryResultTypeType],  # (1)
    Format: NotRequired[QueryResultFormatType],  # (2)
    AdditionalAttributes: NotRequired[List[AdditionalResultAttributeTypeDef]],  # (3)
    DocumentId: NotRequired[str],
    DocumentTitle: NotRequired[TextWithHighlightsTypeDef],  # (4)
    DocumentExcerpt: NotRequired[TextWithHighlightsTypeDef],  # (4)
    DocumentURI: NotRequired[str],
    DocumentAttributes: NotRequired[List[DocumentAttributeOutputTypeDef]],  # (6)
    ScoreAttributes: NotRequired[ScoreAttributesTypeDef],  # (7)
    FeedbackToken: NotRequired[str],
    TableExcerpt: NotRequired[TableExcerptTypeDef],  # (8)
    CollapsedResultDetail: NotRequired[CollapsedResultDetailTypeDef],  # (9)
```

1. See [:material-code-brackets: QueryResultTypeType](./literals.md#queryresulttypetype) 
2. See [:material-code-brackets: QueryResultFormatType](./literals.md#queryresultformattype) 
3. See [:material-code-braces: AdditionalResultAttributeTypeDef](./type_defs.md#additionalresultattributetypedef) 
4. See [:material-code-braces: TextWithHighlightsTypeDef](./type_defs.md#textwithhighlightstypedef) 
5. See [:material-code-braces: TextWithHighlightsTypeDef](./type_defs.md#textwithhighlightstypedef) 
6. See [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
7. See [:material-code-braces: ScoreAttributesTypeDef](./type_defs.md#scoreattributestypedef) 
8. See [:material-code-braces: TableExcerptTypeDef](./type_defs.md#tableexcerpttypedef) 
9. See [:material-code-braces: CollapsedResultDetailTypeDef](./type_defs.md#collapsedresultdetailtypedef) 
## UpdateIndexRequestRequestTypeDef

```python
# UpdateIndexRequestRequestTypeDef definition

class UpdateIndexRequestRequestTypeDef(TypedDict):
    Id: str,
    Name: NotRequired[str],
    RoleArn: NotRequired[str],
    Description: NotRequired[str],
    DocumentMetadataConfigurationUpdates: NotRequired[Sequence[DocumentMetadataConfigurationUnionTypeDef]],  # (1)
    CapacityUnits: NotRequired[CapacityUnitsConfigurationTypeDef],  # (2)
    UserTokenConfigurations: NotRequired[Sequence[UserTokenConfigurationTypeDef]],  # (3)
    UserContextPolicy: NotRequired[UserContextPolicyType],  # (4)
    UserGroupResolutionConfiguration: NotRequired[UserGroupResolutionConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: DocumentMetadataConfigurationTypeDef](./type_defs.md#documentmetadataconfigurationtypedef) [:material-code-braces: DocumentMetadataConfigurationOutputTypeDef](./type_defs.md#documentmetadataconfigurationoutputtypedef) 
2. See [:material-code-braces: CapacityUnitsConfigurationTypeDef](./type_defs.md#capacityunitsconfigurationtypedef) 
3. See [:material-code-braces: UserTokenConfigurationTypeDef](./type_defs.md#usertokenconfigurationtypedef) 
4. See [:material-code-brackets: UserContextPolicyType](./literals.md#usercontextpolicytype) 
5. See [:material-code-braces: UserGroupResolutionConfigurationTypeDef](./type_defs.md#usergroupresolutionconfigurationtypedef) 
## WebCrawlerConfigurationTypeDef

```python
# WebCrawlerConfigurationTypeDef definition

class WebCrawlerConfigurationTypeDef(TypedDict):
    Urls: UrlsUnionTypeDef,  # (1)
    CrawlDepth: NotRequired[int],
    MaxLinksPerPage: NotRequired[int],
    MaxContentSizePerPageInMegaBytes: NotRequired[float],
    MaxUrlsPerMinuteCrawlRate: NotRequired[int],
    UrlInclusionPatterns: NotRequired[Sequence[str]],
    UrlExclusionPatterns: NotRequired[Sequence[str]],
    ProxyConfiguration: NotRequired[ProxyConfigurationTypeDef],  # (2)
    AuthenticationConfiguration: NotRequired[AuthenticationConfigurationUnionTypeDef],  # (3)
```

1. See [:material-code-braces: UrlsTypeDef](./type_defs.md#urlstypedef) [:material-code-braces: UrlsOutputTypeDef](./type_defs.md#urlsoutputtypedef) 
2. See [:material-code-braces: ProxyConfigurationTypeDef](./type_defs.md#proxyconfigurationtypedef) 
3. See [:material-code-braces: AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef) [:material-code-braces: AuthenticationConfigurationOutputTypeDef](./type_defs.md#authenticationconfigurationoutputtypedef) 
## GetQuerySuggestionsResponseTypeDef

```python
# GetQuerySuggestionsResponseTypeDef definition

class GetQuerySuggestionsResponseTypeDef(TypedDict):
    QuerySuggestionsId: str,
    Suggestions: List[SuggestionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SuggestionTypeDef](./type_defs.md#suggestiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeDataSourceResponseTypeDef

```python
# DescribeDataSourceResponseTypeDef definition

class DescribeDataSourceResponseTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    Name: str,
    Type: DataSourceTypeType,  # (1)
    Configuration: DataSourceConfigurationOutputTypeDef,  # (2)
    VpcConfiguration: DataSourceVpcConfigurationOutputTypeDef,  # (3)
    CreatedAt: datetime,
    UpdatedAt: datetime,
    Description: str,
    Status: DataSourceStatusType,  # (4)
    Schedule: str,
    RoleArn: str,
    ErrorMessage: str,
    LanguageCode: str,
    CustomDocumentEnrichmentConfiguration: CustomDocumentEnrichmentConfigurationOutputTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef) 
3. See [:material-code-braces: DataSourceVpcConfigurationOutputTypeDef](./type_defs.md#datasourcevpcconfigurationoutputtypedef) 
4. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
5. See [:material-code-braces: CustomDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#customdocumentenrichmentconfigurationoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SalesforceConfigurationTypeDef

```python
# SalesforceConfigurationTypeDef definition

class SalesforceConfigurationTypeDef(TypedDict):
    ServerUrl: str,
    SecretArn: str,
    StandardObjectConfigurations: NotRequired[Sequence[SalesforceStandardObjectConfigurationUnionTypeDef]],  # (1)
    KnowledgeArticleConfiguration: NotRequired[SalesforceKnowledgeArticleConfigurationUnionTypeDef],  # (2)
    ChatterFeedConfiguration: NotRequired[SalesforceChatterFeedConfigurationUnionTypeDef],  # (3)
    CrawlAttachments: NotRequired[bool],
    StandardObjectAttachmentConfiguration: NotRequired[SalesforceStandardObjectAttachmentConfigurationUnionTypeDef],  # (4)
    IncludeAttachmentFilePatterns: NotRequired[Sequence[str]],
    ExcludeAttachmentFilePatterns: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: SalesforceStandardObjectConfigurationTypeDef](./type_defs.md#salesforcestandardobjectconfigurationtypedef) [:material-code-braces: SalesforceStandardObjectConfigurationOutputTypeDef](./type_defs.md#salesforcestandardobjectconfigurationoutputtypedef) 
2. See [:material-code-braces: SalesforceKnowledgeArticleConfigurationTypeDef](./type_defs.md#salesforceknowledgearticleconfigurationtypedef) [:material-code-braces: SalesforceKnowledgeArticleConfigurationOutputTypeDef](./type_defs.md#salesforceknowledgearticleconfigurationoutputtypedef) 
3. See [:material-code-braces: SalesforceChatterFeedConfigurationTypeDef](./type_defs.md#salesforcechatterfeedconfigurationtypedef) [:material-code-braces: SalesforceChatterFeedConfigurationOutputTypeDef](./type_defs.md#salesforcechatterfeedconfigurationoutputtypedef) 
4. See [:material-code-braces: SalesforceStandardObjectAttachmentConfigurationTypeDef](./type_defs.md#salesforcestandardobjectattachmentconfigurationtypedef) [:material-code-braces: SalesforceStandardObjectAttachmentConfigurationOutputTypeDef](./type_defs.md#salesforcestandardobjectattachmentconfigurationoutputtypedef) 
## HookConfigurationTypeDef

```python
# HookConfigurationTypeDef definition

class HookConfigurationTypeDef(TypedDict):
    LambdaArn: str,
    S3Bucket: str,
    InvocationCondition: NotRequired[DocumentAttributeConditionUnionTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef) [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 
## InlineCustomDocumentEnrichmentConfigurationTypeDef

```python
# InlineCustomDocumentEnrichmentConfigurationTypeDef definition

class InlineCustomDocumentEnrichmentConfigurationTypeDef(TypedDict):
    Condition: NotRequired[DocumentAttributeConditionUnionTypeDef],  # (1)
    Target: NotRequired[DocumentAttributeTargetUnionTypeDef],  # (2)
    DocumentContentDeletion: NotRequired[bool],
```

1. See [:material-code-braces: DocumentAttributeConditionTypeDef](./type_defs.md#documentattributeconditiontypedef) [:material-code-braces: DocumentAttributeConditionOutputTypeDef](./type_defs.md#documentattributeconditionoutputtypedef) 
2. See [:material-code-braces: DocumentAttributeTargetTypeDef](./type_defs.md#documentattributetargettypedef) [:material-code-braces: DocumentAttributeTargetOutputTypeDef](./type_defs.md#documentattributetargetoutputtypedef) 
## AttributeFilterTypeDef

```python
# AttributeFilterTypeDef definition

class AttributeFilterTypeDef(TypedDict):
    AndAllFilters: NotRequired[Sequence[Mapping[str, Any]]],
    OrAllFilters: NotRequired[Sequence[Mapping[str, Any]]],
    NotFilter: NotRequired[Mapping[str, Any]],
    EqualsTo: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    ContainsAll: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    ContainsAny: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    GreaterThan: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    GreaterThanOrEquals: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    LessThan: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
    LessThanOrEquals: NotRequired[DocumentAttributeUnionTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
2. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
3. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
4. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
5. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
6. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
7. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
## DocumentInfoTypeDef

```python
# DocumentInfoTypeDef definition

class DocumentInfoTypeDef(TypedDict):
    DocumentId: str,
    Attributes: NotRequired[Sequence[DocumentAttributeUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
## DocumentTypeDef

```python
# DocumentTypeDef definition

class DocumentTypeDef(TypedDict):
    Id: str,
    Title: NotRequired[str],
    Blob: NotRequired[BlobTypeDef],
    S3Path: NotRequired[S3PathTypeDef],  # (1)
    Attributes: NotRequired[Sequence[DocumentAttributeUnionTypeDef]],  # (2)
    AccessControlList: NotRequired[Sequence[PrincipalTypeDef]],  # (3)
    HierarchicalAccessControlList: NotRequired[Sequence[HierarchicalPrincipalUnionTypeDef]],  # (4)
    ContentType: NotRequired[ContentTypeType],  # (5)
    AccessControlConfigurationId: NotRequired[str],
```

1. See [:material-code-braces: S3PathTypeDef](./type_defs.md#s3pathtypedef) 
2. See [:material-code-braces: DocumentAttributeTypeDef](./type_defs.md#documentattributetypedef) [:material-code-braces: DocumentAttributeOutputTypeDef](./type_defs.md#documentattributeoutputtypedef) 
3. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
4. See [:material-code-braces: HierarchicalPrincipalTypeDef](./type_defs.md#hierarchicalprincipaltypedef) [:material-code-braces: HierarchicalPrincipalOutputTypeDef](./type_defs.md#hierarchicalprincipaloutputtypedef) 
5. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
## QueryResultTypeDef

```python
# QueryResultTypeDef definition

class QueryResultTypeDef(TypedDict):
    QueryId: str,
    ResultItems: List[QueryResultItemTypeDef],  # (1)
    FacetResults: List[FacetResultTypeDef],  # (2)
    TotalNumberOfResults: int,
    Warnings: List[WarningTypeDef],  # (3)
    SpellCorrectedQueries: List[SpellCorrectedQueryTypeDef],  # (4)
    FeaturedResultsItems: List[FeaturedResultsItemTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: QueryResultItemTypeDef](./type_defs.md#queryresultitemtypedef) 
2. See [:material-code-braces: FacetResultTypeDef](./type_defs.md#facetresulttypedef) 
3. See [:material-code-braces: WarningTypeDef](./type_defs.md#warningtypedef) 
4. See [:material-code-braces: SpellCorrectedQueryTypeDef](./type_defs.md#spellcorrectedquerytypedef) 
5. See [:material-code-braces: FeaturedResultsItemTypeDef](./type_defs.md#featuredresultsitemtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AttributeSuggestionsGetConfigTypeDef

```python
# AttributeSuggestionsGetConfigTypeDef definition

class AttributeSuggestionsGetConfigTypeDef(TypedDict):
    SuggestionAttributes: NotRequired[Sequence[str]],
    AdditionalResponseAttributes: NotRequired[Sequence[str]],
    AttributeFilter: NotRequired[AttributeFilterTypeDef],  # (1)
    UserContext: NotRequired[UserContextTypeDef],  # (2)
```

1. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) 
2. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
## QueryRequestRequestTypeDef

```python
# QueryRequestRequestTypeDef definition

class QueryRequestRequestTypeDef(TypedDict):
    IndexId: str,
    QueryText: NotRequired[str],
    AttributeFilter: NotRequired[AttributeFilterTypeDef],  # (1)
    Facets: NotRequired[Sequence[FacetTypeDef]],  # (2)
    RequestedDocumentAttributes: NotRequired[Sequence[str]],
    QueryResultTypeFilter: NotRequired[QueryResultTypeType],  # (3)
    DocumentRelevanceOverrideConfigurations: NotRequired[Sequence[DocumentRelevanceConfigurationTypeDef]],  # (4)
    PageNumber: NotRequired[int],
    PageSize: NotRequired[int],
    SortingConfiguration: NotRequired[SortingConfigurationTypeDef],  # (5)
    SortingConfigurations: NotRequired[Sequence[SortingConfigurationTypeDef]],  # (6)
    UserContext: NotRequired[UserContextTypeDef],  # (7)
    VisitorId: NotRequired[str],
    SpellCorrectionConfiguration: NotRequired[SpellCorrectionConfigurationTypeDef],  # (8)
    CollapseConfiguration: NotRequired[CollapseConfigurationTypeDef],  # (9)
```

1. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) 
2. See [:material-code-braces: FacetTypeDef](./type_defs.md#facettypedef) 
3. See [:material-code-brackets: QueryResultTypeType](./literals.md#queryresulttypetype) 
4. See [:material-code-braces: DocumentRelevanceConfigurationTypeDef](./type_defs.md#documentrelevanceconfigurationtypedef) 
5. See [:material-code-braces: SortingConfigurationTypeDef](./type_defs.md#sortingconfigurationtypedef) 
6. See [:material-code-braces: SortingConfigurationTypeDef](./type_defs.md#sortingconfigurationtypedef) 
7. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
8. See [:material-code-braces: SpellCorrectionConfigurationTypeDef](./type_defs.md#spellcorrectionconfigurationtypedef) 
9. See [:material-code-braces: CollapseConfigurationTypeDef](./type_defs.md#collapseconfigurationtypedef) 
## RetrieveRequestRequestTypeDef

```python
# RetrieveRequestRequestTypeDef definition

class RetrieveRequestRequestTypeDef(TypedDict):
    IndexId: str,
    QueryText: str,
    AttributeFilter: NotRequired[AttributeFilterTypeDef],  # (1)
    RequestedDocumentAttributes: NotRequired[Sequence[str]],
    DocumentRelevanceOverrideConfigurations: NotRequired[Sequence[DocumentRelevanceConfigurationTypeDef]],  # (2)
    PageNumber: NotRequired[int],
    PageSize: NotRequired[int],
    UserContext: NotRequired[UserContextTypeDef],  # (3)
```

1. See [:material-code-braces: AttributeFilterTypeDef](./type_defs.md#attributefiltertypedef) 
2. See [:material-code-braces: DocumentRelevanceConfigurationTypeDef](./type_defs.md#documentrelevanceconfigurationtypedef) 
3. See [:material-code-braces: UserContextTypeDef](./type_defs.md#usercontexttypedef) 
## BatchGetDocumentStatusRequestRequestTypeDef

```python
# BatchGetDocumentStatusRequestRequestTypeDef definition

class BatchGetDocumentStatusRequestRequestTypeDef(TypedDict):
    IndexId: str,
    DocumentInfoList: Sequence[DocumentInfoTypeDef],  # (1)
```

1. See [:material-code-braces: DocumentInfoTypeDef](./type_defs.md#documentinfotypedef) 
## DataSourceConfigurationTypeDef

```python
# DataSourceConfigurationTypeDef definition

class DataSourceConfigurationTypeDef(TypedDict):
    S3Configuration: NotRequired[S3DataSourceConfigurationUnionTypeDef],  # (1)
    SharePointConfiguration: NotRequired[SharePointConfigurationUnionTypeDef],  # (2)
    DatabaseConfiguration: NotRequired[DatabaseConfigurationUnionTypeDef],  # (3)
    SalesforceConfiguration: NotRequired[SalesforceConfigurationUnionTypeDef],  # (4)
    OneDriveConfiguration: NotRequired[OneDriveConfigurationUnionTypeDef],  # (5)
    ServiceNowConfiguration: NotRequired[ServiceNowConfigurationUnionTypeDef],  # (6)
    ConfluenceConfiguration: NotRequired[ConfluenceConfigurationUnionTypeDef],  # (7)
    GoogleDriveConfiguration: NotRequired[GoogleDriveConfigurationUnionTypeDef],  # (8)
    WebCrawlerConfiguration: NotRequired[WebCrawlerConfigurationUnionTypeDef],  # (9)
    WorkDocsConfiguration: NotRequired[WorkDocsConfigurationUnionTypeDef],  # (10)
    FsxConfiguration: NotRequired[FsxConfigurationUnionTypeDef],  # (11)
    SlackConfiguration: NotRequired[SlackConfigurationUnionTypeDef],  # (12)
    BoxConfiguration: NotRequired[BoxConfigurationUnionTypeDef],  # (13)
    QuipConfiguration: NotRequired[QuipConfigurationUnionTypeDef],  # (14)
    JiraConfiguration: NotRequired[JiraConfigurationUnionTypeDef],  # (15)
    GitHubConfiguration: NotRequired[GitHubConfigurationUnionTypeDef],  # (16)
    AlfrescoConfiguration: NotRequired[AlfrescoConfigurationUnionTypeDef],  # (17)
    TemplateConfiguration: NotRequired[TemplateConfigurationUnionTypeDef],  # (18)
```

1. See [:material-code-braces: S3DataSourceConfigurationTypeDef](./type_defs.md#s3datasourceconfigurationtypedef) [:material-code-braces: S3DataSourceConfigurationOutputTypeDef](./type_defs.md#s3datasourceconfigurationoutputtypedef) 
2. See [:material-code-braces: SharePointConfigurationTypeDef](./type_defs.md#sharepointconfigurationtypedef) [:material-code-braces: SharePointConfigurationOutputTypeDef](./type_defs.md#sharepointconfigurationoutputtypedef) 
3. See [:material-code-braces: DatabaseConfigurationTypeDef](./type_defs.md#databaseconfigurationtypedef) [:material-code-braces: DatabaseConfigurationOutputTypeDef](./type_defs.md#databaseconfigurationoutputtypedef) 
4. See [:material-code-braces: SalesforceConfigurationTypeDef](./type_defs.md#salesforceconfigurationtypedef) [:material-code-braces: SalesforceConfigurationOutputTypeDef](./type_defs.md#salesforceconfigurationoutputtypedef) 
5. See [:material-code-braces: OneDriveConfigurationTypeDef](./type_defs.md#onedriveconfigurationtypedef) [:material-code-braces: OneDriveConfigurationOutputTypeDef](./type_defs.md#onedriveconfigurationoutputtypedef) 
6. See [:material-code-braces: ServiceNowConfigurationTypeDef](./type_defs.md#servicenowconfigurationtypedef) [:material-code-braces: ServiceNowConfigurationOutputTypeDef](./type_defs.md#servicenowconfigurationoutputtypedef) 
7. See [:material-code-braces: ConfluenceConfigurationTypeDef](./type_defs.md#confluenceconfigurationtypedef) [:material-code-braces: ConfluenceConfigurationOutputTypeDef](./type_defs.md#confluenceconfigurationoutputtypedef) 
8. See [:material-code-braces: GoogleDriveConfigurationTypeDef](./type_defs.md#googledriveconfigurationtypedef) [:material-code-braces: GoogleDriveConfigurationOutputTypeDef](./type_defs.md#googledriveconfigurationoutputtypedef) 
9. See [:material-code-braces: WebCrawlerConfigurationTypeDef](./type_defs.md#webcrawlerconfigurationtypedef) [:material-code-braces: WebCrawlerConfigurationOutputTypeDef](./type_defs.md#webcrawlerconfigurationoutputtypedef) 
10. See [:material-code-braces: WorkDocsConfigurationTypeDef](./type_defs.md#workdocsconfigurationtypedef) [:material-code-braces: WorkDocsConfigurationOutputTypeDef](./type_defs.md#workdocsconfigurationoutputtypedef) 
11. See [:material-code-braces: FsxConfigurationTypeDef](./type_defs.md#fsxconfigurationtypedef) [:material-code-braces: FsxConfigurationOutputTypeDef](./type_defs.md#fsxconfigurationoutputtypedef) 
12. See [:material-code-braces: SlackConfigurationTypeDef](./type_defs.md#slackconfigurationtypedef) [:material-code-braces: SlackConfigurationOutputTypeDef](./type_defs.md#slackconfigurationoutputtypedef) 
13. See [:material-code-braces: BoxConfigurationTypeDef](./type_defs.md#boxconfigurationtypedef) [:material-code-braces: BoxConfigurationOutputTypeDef](./type_defs.md#boxconfigurationoutputtypedef) 
14. See [:material-code-braces: QuipConfigurationTypeDef](./type_defs.md#quipconfigurationtypedef) [:material-code-braces: QuipConfigurationOutputTypeDef](./type_defs.md#quipconfigurationoutputtypedef) 
15. See [:material-code-braces: JiraConfigurationTypeDef](./type_defs.md#jiraconfigurationtypedef) [:material-code-braces: JiraConfigurationOutputTypeDef](./type_defs.md#jiraconfigurationoutputtypedef) 
16. See [:material-code-braces: GitHubConfigurationTypeDef](./type_defs.md#githubconfigurationtypedef) [:material-code-braces: GitHubConfigurationOutputTypeDef](./type_defs.md#githubconfigurationoutputtypedef) 
17. See [:material-code-braces: AlfrescoConfigurationTypeDef](./type_defs.md#alfrescoconfigurationtypedef) [:material-code-braces: AlfrescoConfigurationOutputTypeDef](./type_defs.md#alfrescoconfigurationoutputtypedef) 
18. See [:material-code-braces: TemplateConfigurationTypeDef](./type_defs.md#templateconfigurationtypedef) [:material-code-braces: TemplateConfigurationOutputTypeDef](./type_defs.md#templateconfigurationoutputtypedef) 
## CustomDocumentEnrichmentConfigurationTypeDef

```python
# CustomDocumentEnrichmentConfigurationTypeDef definition

class CustomDocumentEnrichmentConfigurationTypeDef(TypedDict):
    InlineConfigurations: NotRequired[Sequence[InlineCustomDocumentEnrichmentConfigurationUnionTypeDef]],  # (1)
    PreExtractionHookConfiguration: NotRequired[HookConfigurationUnionTypeDef],  # (2)
    PostExtractionHookConfiguration: NotRequired[HookConfigurationUnionTypeDef],  # (2)
    RoleArn: NotRequired[str],
```

1. See [:material-code-braces: InlineCustomDocumentEnrichmentConfigurationTypeDef](./type_defs.md#inlinecustomdocumentenrichmentconfigurationtypedef) [:material-code-braces: InlineCustomDocumentEnrichmentConfigurationOutputTypeDef](./type_defs.md#inlinecustomdocumentenrichmentconfigurationoutputtypedef) 
2. See [:material-code-braces: HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef) [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 
3. See [:material-code-braces: HookConfigurationTypeDef](./type_defs.md#hookconfigurationtypedef) [:material-code-braces: HookConfigurationOutputTypeDef](./type_defs.md#hookconfigurationoutputtypedef) 
## GetQuerySuggestionsRequestRequestTypeDef

```python
# GetQuerySuggestionsRequestRequestTypeDef definition

class GetQuerySuggestionsRequestRequestTypeDef(TypedDict):
    IndexId: str,
    QueryText: str,
    MaxSuggestionsCount: NotRequired[int],
    SuggestionTypes: NotRequired[Sequence[SuggestionTypeType]],  # (1)
    AttributeSuggestionsConfig: NotRequired[AttributeSuggestionsGetConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: SuggestionTypeType](./literals.md#suggestiontypetype) 
2. See [:material-code-braces: AttributeSuggestionsGetConfigTypeDef](./type_defs.md#attributesuggestionsgetconfigtypedef) 
## BatchPutDocumentRequestRequestTypeDef

```python
# BatchPutDocumentRequestRequestTypeDef definition

class BatchPutDocumentRequestRequestTypeDef(TypedDict):
    IndexId: str,
    Documents: Sequence[DocumentTypeDef],  # (1)
    RoleArn: NotRequired[str],
    CustomDocumentEnrichmentConfiguration: NotRequired[CustomDocumentEnrichmentConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: DocumentTypeDef](./type_defs.md#documenttypedef) 
2. See [:material-code-braces: CustomDocumentEnrichmentConfigurationTypeDef](./type_defs.md#customdocumentenrichmentconfigurationtypedef) 
## CreateDataSourceRequestRequestTypeDef

```python
# CreateDataSourceRequestRequestTypeDef definition

class CreateDataSourceRequestRequestTypeDef(TypedDict):
    Name: str,
    IndexId: str,
    Type: DataSourceTypeType,  # (1)
    Configuration: NotRequired[DataSourceConfigurationTypeDef],  # (2)
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationTypeDef],  # (3)
    Description: NotRequired[str],
    Schedule: NotRequired[str],
    RoleArn: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
    ClientToken: NotRequired[str],
    LanguageCode: NotRequired[str],
    CustomDocumentEnrichmentConfiguration: NotRequired[CustomDocumentEnrichmentConfigurationTypeDef],  # (5)
```

1. See [:material-code-brackets: DataSourceTypeType](./literals.md#datasourcetypetype) 
2. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
3. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CustomDocumentEnrichmentConfigurationTypeDef](./type_defs.md#customdocumentenrichmentconfigurationtypedef) 
## UpdateDataSourceRequestRequestTypeDef

```python
# UpdateDataSourceRequestRequestTypeDef definition

class UpdateDataSourceRequestRequestTypeDef(TypedDict):
    Id: str,
    IndexId: str,
    Name: NotRequired[str],
    Configuration: NotRequired[DataSourceConfigurationTypeDef],  # (1)
    VpcConfiguration: NotRequired[DataSourceVpcConfigurationTypeDef],  # (2)
    Description: NotRequired[str],
    Schedule: NotRequired[str],
    RoleArn: NotRequired[str],
    LanguageCode: NotRequired[str],
    CustomDocumentEnrichmentConfiguration: NotRequired[CustomDocumentEnrichmentConfigurationTypeDef],  # (3)
```

1. See [:material-code-braces: DataSourceConfigurationTypeDef](./type_defs.md#datasourceconfigurationtypedef) 
2. See [:material-code-braces: DataSourceVpcConfigurationTypeDef](./type_defs.md#datasourcevpcconfigurationtypedef) 
3. See [:material-code-braces: CustomDocumentEnrichmentConfigurationTypeDef](./type_defs.md#customdocumentenrichmentconfigurationtypedef) 

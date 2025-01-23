# Type definitions

> [Index](../README.md) > [Amplify](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Amplify](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#amplify)
    type annotations stubs module [types-aiobotocore-amplify](https://pypi.org/project/types-aiobotocore-amplify/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AutoBranchCreationConfigOutputTypeDef

```python
# AutoBranchCreationConfigOutputTypeDef definition

class AutoBranchCreationConfigOutputTypeDef(TypedDict):
    stage: NotRequired[StageType],  # (1)
    framework: NotRequired[str],
    enableAutoBuild: NotRequired[bool],
    environmentVariables: NotRequired[Dict[str, str]],
    basicAuthCredentials: NotRequired[str],
    enableBasicAuth: NotRequired[bool],
    enablePerformanceMode: NotRequired[bool],
    buildSpec: NotRequired[str],
    enablePullRequestPreview: NotRequired[bool],
    pullRequestEnvironmentName: NotRequired[str],
```

1. See [:material-code-brackets: StageType](./literals.md#stagetype) 
## CacheConfigTypeDef

```python
# CacheConfigTypeDef definition

class CacheConfigTypeDef(TypedDict):
    type: CacheConfigTypeType,  # (1)
```

1. See [:material-code-brackets: CacheConfigTypeType](./literals.md#cacheconfigtypetype) 
## CustomRuleTypeDef

```python
# CustomRuleTypeDef definition

class CustomRuleTypeDef(TypedDict):
    source: str,
    target: str,
    status: NotRequired[str],
    condition: NotRequired[str],
```

## ProductionBranchTypeDef

```python
# ProductionBranchTypeDef definition

class ProductionBranchTypeDef(TypedDict):
    lastDeployTime: NotRequired[datetime],
    status: NotRequired[str],
    thumbnailUrl: NotRequired[str],
    branchName: NotRequired[str],
```

## WafConfigurationTypeDef

```python
# WafConfigurationTypeDef definition

class WafConfigurationTypeDef(TypedDict):
    webAclArn: NotRequired[str],
    wafStatus: NotRequired[WafStatusType],  # (1)
    statusReason: NotRequired[str],
```

1. See [:material-code-brackets: WafStatusType](./literals.md#wafstatustype) 
## ArtifactTypeDef

```python
# ArtifactTypeDef definition

class ArtifactTypeDef(TypedDict):
    artifactFileName: str,
    artifactId: str,
```

## AutoBranchCreationConfigTypeDef

```python
# AutoBranchCreationConfigTypeDef definition

class AutoBranchCreationConfigTypeDef(TypedDict):
    stage: NotRequired[StageType],  # (1)
    framework: NotRequired[str],
    enableAutoBuild: NotRequired[bool],
    environmentVariables: NotRequired[Mapping[str, str]],
    basicAuthCredentials: NotRequired[str],
    enableBasicAuth: NotRequired[bool],
    enablePerformanceMode: NotRequired[bool],
    buildSpec: NotRequired[str],
    enablePullRequestPreview: NotRequired[bool],
    pullRequestEnvironmentName: NotRequired[str],
```

1. See [:material-code-brackets: StageType](./literals.md#stagetype) 
## BackendEnvironmentTypeDef

```python
# BackendEnvironmentTypeDef definition

class BackendEnvironmentTypeDef(TypedDict):
    backendEnvironmentArn: str,
    environmentName: str,
    createTime: datetime,
    updateTime: datetime,
    stackName: NotRequired[str],
    deploymentArtifacts: NotRequired[str],
```

## BackendTypeDef

```python
# BackendTypeDef definition

class BackendTypeDef(TypedDict):
    stackArn: NotRequired[str],
```

## CertificateSettingsTypeDef

```python
# CertificateSettingsTypeDef definition

class CertificateSettingsTypeDef(TypedDict):
    type: CertificateTypeType,  # (1)
    customCertificateArn: NotRequired[str],
```

1. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype) 
## CertificateTypeDef

```python
# CertificateTypeDef definition

class CertificateTypeDef(TypedDict):
    type: CertificateTypeType,  # (1)
    customCertificateArn: NotRequired[str],
    certificateVerificationDNSRecord: NotRequired[str],
```

1. See [:material-code-brackets: CertificateTypeType](./literals.md#certificatetypetype) 
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

## CreateBackendEnvironmentRequestRequestTypeDef

```python
# CreateBackendEnvironmentRequestRequestTypeDef definition

class CreateBackendEnvironmentRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
    stackName: NotRequired[str],
    deploymentArtifacts: NotRequired[str],
```

## CreateDeploymentRequestRequestTypeDef

```python
# CreateDeploymentRequestRequestTypeDef definition

class CreateDeploymentRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    fileMap: NotRequired[Mapping[str, str]],
```

## SubDomainSettingTypeDef

```python
# SubDomainSettingTypeDef definition

class SubDomainSettingTypeDef(TypedDict):
    prefix: str,
    branchName: str,
```

## CreateWebhookRequestRequestTypeDef

```python
# CreateWebhookRequestRequestTypeDef definition

class CreateWebhookRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    description: NotRequired[str],
```

## WebhookTypeDef

```python
# WebhookTypeDef definition

class WebhookTypeDef(TypedDict):
    webhookArn: str,
    webhookId: str,
    webhookUrl: str,
    branchName: str,
    description: str,
    createTime: datetime,
    updateTime: datetime,
```

## DeleteAppRequestRequestTypeDef

```python
# DeleteAppRequestRequestTypeDef definition

class DeleteAppRequestRequestTypeDef(TypedDict):
    appId: str,
```

## DeleteBackendEnvironmentRequestRequestTypeDef

```python
# DeleteBackendEnvironmentRequestRequestTypeDef definition

class DeleteBackendEnvironmentRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
```

## DeleteBranchRequestRequestTypeDef

```python
# DeleteBranchRequestRequestTypeDef definition

class DeleteBranchRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
```

## DeleteDomainAssociationRequestRequestTypeDef

```python
# DeleteDomainAssociationRequestRequestTypeDef definition

class DeleteDomainAssociationRequestRequestTypeDef(TypedDict):
    appId: str,
    domainName: str,
```

## DeleteJobRequestRequestTypeDef

```python
# DeleteJobRequestRequestTypeDef definition

class DeleteJobRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    jobId: str,
```

## JobSummaryTypeDef

```python
# JobSummaryTypeDef definition

class JobSummaryTypeDef(TypedDict):
    jobArn: str,
    jobId: str,
    commitId: str,
    commitMessage: str,
    commitTime: datetime,
    startTime: datetime,
    status: JobStatusType,  # (1)
    jobType: JobTypeType,  # (2)
    endTime: NotRequired[datetime],
    sourceUrl: NotRequired[str],
    sourceUrlType: NotRequired[SourceUrlTypeType],  # (3)
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: SourceUrlTypeType](./literals.md#sourceurltypetype) 
## DeleteWebhookRequestRequestTypeDef

```python
# DeleteWebhookRequestRequestTypeDef definition

class DeleteWebhookRequestRequestTypeDef(TypedDict):
    webhookId: str,
```

## GetAppRequestRequestTypeDef

```python
# GetAppRequestRequestTypeDef definition

class GetAppRequestRequestTypeDef(TypedDict):
    appId: str,
```

## GetArtifactUrlRequestRequestTypeDef

```python
# GetArtifactUrlRequestRequestTypeDef definition

class GetArtifactUrlRequestRequestTypeDef(TypedDict):
    artifactId: str,
```

## GetBackendEnvironmentRequestRequestTypeDef

```python
# GetBackendEnvironmentRequestRequestTypeDef definition

class GetBackendEnvironmentRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: str,
```

## GetBranchRequestRequestTypeDef

```python
# GetBranchRequestRequestTypeDef definition

class GetBranchRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
```

## GetDomainAssociationRequestRequestTypeDef

```python
# GetDomainAssociationRequestRequestTypeDef definition

class GetDomainAssociationRequestRequestTypeDef(TypedDict):
    appId: str,
    domainName: str,
```

## GetJobRequestRequestTypeDef

```python
# GetJobRequestRequestTypeDef definition

class GetJobRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    jobId: str,
```

## GetWebhookRequestRequestTypeDef

```python
# GetWebhookRequestRequestTypeDef definition

class GetWebhookRequestRequestTypeDef(TypedDict):
    webhookId: str,
```

## StepTypeDef

```python
# StepTypeDef definition

class StepTypeDef(TypedDict):
    stepName: str,
    startTime: datetime,
    status: JobStatusType,  # (1)
    endTime: datetime,
    logUrl: NotRequired[str],
    artifactsUrl: NotRequired[str],
    testArtifactsUrl: NotRequired[str],
    testConfigUrl: NotRequired[str],
    screenshots: NotRequired[Dict[str, str]],
    statusReason: NotRequired[str],
    context: NotRequired[str],
```

1. See [:material-code-brackets: JobStatusType](./literals.md#jobstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAppsRequestRequestTypeDef

```python
# ListAppsRequestRequestTypeDef definition

class ListAppsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListArtifactsRequestRequestTypeDef

```python
# ListArtifactsRequestRequestTypeDef definition

class ListArtifactsRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    jobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListBackendEnvironmentsRequestRequestTypeDef

```python
# ListBackendEnvironmentsRequestRequestTypeDef definition

class ListBackendEnvironmentsRequestRequestTypeDef(TypedDict):
    appId: str,
    environmentName: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListBranchesRequestRequestTypeDef

```python
# ListBranchesRequestRequestTypeDef definition

class ListBranchesRequestRequestTypeDef(TypedDict):
    appId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListDomainAssociationsRequestRequestTypeDef

```python
# ListDomainAssociationsRequestRequestTypeDef definition

class ListDomainAssociationsRequestRequestTypeDef(TypedDict):
    appId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListJobsRequestRequestTypeDef

```python
# ListJobsRequestRequestTypeDef definition

class ListJobsRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListWebhooksRequestRequestTypeDef

```python
# ListWebhooksRequestRequestTypeDef definition

class ListWebhooksRequestRequestTypeDef(TypedDict):
    appId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## StartDeploymentRequestRequestTypeDef

```python
# StartDeploymentRequestRequestTypeDef definition

class StartDeploymentRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    jobId: NotRequired[str],
    sourceUrl: NotRequired[str],
    sourceUrlType: NotRequired[SourceUrlTypeType],  # (1)
```

1. See [:material-code-brackets: SourceUrlTypeType](./literals.md#sourceurltypetype) 
## StopJobRequestRequestTypeDef

```python
# StopJobRequestRequestTypeDef definition

class StopJobRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    jobId: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateWebhookRequestRequestTypeDef

```python
# UpdateWebhookRequestRequestTypeDef definition

class UpdateWebhookRequestRequestTypeDef(TypedDict):
    webhookId: str,
    branchName: NotRequired[str],
    description: NotRequired[str],
```

## AppTypeDef

```python
# AppTypeDef definition

class AppTypeDef(TypedDict):
    appId: str,
    appArn: str,
    name: str,
    description: str,
    repository: str,
    platform: PlatformType,  # (1)
    createTime: datetime,
    updateTime: datetime,
    environmentVariables: Dict[str, str],
    defaultDomain: str,
    enableBranchAutoBuild: bool,
    enableBasicAuth: bool,
    tags: NotRequired[Dict[str, str]],
    iamServiceRoleArn: NotRequired[str],
    enableBranchAutoDeletion: NotRequired[bool],
    basicAuthCredentials: NotRequired[str],
    customRules: NotRequired[List[CustomRuleTypeDef]],  # (2)
    productionBranch: NotRequired[ProductionBranchTypeDef],  # (3)
    buildSpec: NotRequired[str],
    customHeaders: NotRequired[str],
    enableAutoBranchCreation: NotRequired[bool],
    autoBranchCreationPatterns: NotRequired[List[str]],
    autoBranchCreationConfig: NotRequired[AutoBranchCreationConfigOutputTypeDef],  # (4)
    repositoryCloneMethod: NotRequired[RepositoryCloneMethodType],  # (5)
    cacheConfig: NotRequired[CacheConfigTypeDef],  # (6)
    webhookCreateTime: NotRequired[datetime],
    wafConfiguration: NotRequired[WafConfigurationTypeDef],  # (7)
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: CustomRuleTypeDef](./type_defs.md#customruletypedef) 
3. See [:material-code-braces: ProductionBranchTypeDef](./type_defs.md#productionbranchtypedef) 
4. See [:material-code-braces: AutoBranchCreationConfigOutputTypeDef](./type_defs.md#autobranchcreationconfigoutputtypedef) 
5. See [:material-code-brackets: RepositoryCloneMethodType](./literals.md#repositoryclonemethodtype) 
6. See [:material-code-braces: CacheConfigTypeDef](./type_defs.md#cacheconfigtypedef) 
7. See [:material-code-braces: WafConfigurationTypeDef](./type_defs.md#wafconfigurationtypedef) 
## CreateAppRequestRequestTypeDef

```python
# CreateAppRequestRequestTypeDef definition

class CreateAppRequestRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    repository: NotRequired[str],
    platform: NotRequired[PlatformType],  # (1)
    iamServiceRoleArn: NotRequired[str],
    oauthToken: NotRequired[str],
    accessToken: NotRequired[str],
    environmentVariables: NotRequired[Mapping[str, str]],
    enableBranchAutoBuild: NotRequired[bool],
    enableBranchAutoDeletion: NotRequired[bool],
    enableBasicAuth: NotRequired[bool],
    basicAuthCredentials: NotRequired[str],
    customRules: NotRequired[Sequence[CustomRuleTypeDef]],  # (2)
    tags: NotRequired[Mapping[str, str]],
    buildSpec: NotRequired[str],
    customHeaders: NotRequired[str],
    enableAutoBranchCreation: NotRequired[bool],
    autoBranchCreationPatterns: NotRequired[Sequence[str]],
    autoBranchCreationConfig: NotRequired[AutoBranchCreationConfigTypeDef],  # (3)
    cacheConfig: NotRequired[CacheConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: CustomRuleTypeDef](./type_defs.md#customruletypedef) 
3. See [:material-code-braces: AutoBranchCreationConfigTypeDef](./type_defs.md#autobranchcreationconfigtypedef) 
4. See [:material-code-braces: CacheConfigTypeDef](./type_defs.md#cacheconfigtypedef) 
## UpdateAppRequestRequestTypeDef

```python
# UpdateAppRequestRequestTypeDef definition

class UpdateAppRequestRequestTypeDef(TypedDict):
    appId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    platform: NotRequired[PlatformType],  # (1)
    iamServiceRoleArn: NotRequired[str],
    environmentVariables: NotRequired[Mapping[str, str]],
    enableBranchAutoBuild: NotRequired[bool],
    enableBranchAutoDeletion: NotRequired[bool],
    enableBasicAuth: NotRequired[bool],
    basicAuthCredentials: NotRequired[str],
    customRules: NotRequired[Sequence[CustomRuleTypeDef]],  # (2)
    buildSpec: NotRequired[str],
    customHeaders: NotRequired[str],
    enableAutoBranchCreation: NotRequired[bool],
    autoBranchCreationPatterns: NotRequired[Sequence[str]],
    autoBranchCreationConfig: NotRequired[AutoBranchCreationConfigTypeDef],  # (3)
    repository: NotRequired[str],
    oauthToken: NotRequired[str],
    accessToken: NotRequired[str],
    cacheConfig: NotRequired[CacheConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: PlatformType](./literals.md#platformtype) 
2. See [:material-code-braces: CustomRuleTypeDef](./type_defs.md#customruletypedef) 
3. See [:material-code-braces: AutoBranchCreationConfigTypeDef](./type_defs.md#autobranchcreationconfigtypedef) 
4. See [:material-code-braces: CacheConfigTypeDef](./type_defs.md#cacheconfigtypedef) 
## BranchTypeDef

```python
# BranchTypeDef definition

class BranchTypeDef(TypedDict):
    branchArn: str,
    branchName: str,
    description: str,
    stage: StageType,  # (1)
    displayName: str,
    enableNotification: bool,
    createTime: datetime,
    updateTime: datetime,
    environmentVariables: Dict[str, str],
    enableAutoBuild: bool,
    customDomains: List[str],
    framework: str,
    activeJobId: str,
    totalNumberOfJobs: str,
    enableBasicAuth: bool,
    ttl: str,
    enablePullRequestPreview: bool,
    tags: NotRequired[Dict[str, str]],
    enablePerformanceMode: NotRequired[bool],
    thumbnailUrl: NotRequired[str],
    basicAuthCredentials: NotRequired[str],
    buildSpec: NotRequired[str],
    associatedResources: NotRequired[List[str]],
    pullRequestEnvironmentName: NotRequired[str],
    destinationBranch: NotRequired[str],
    sourceBranch: NotRequired[str],
    backendEnvironmentArn: NotRequired[str],
    backend: NotRequired[BackendTypeDef],  # (2)
```

1. See [:material-code-brackets: StageType](./literals.md#stagetype) 
2. See [:material-code-braces: BackendTypeDef](./type_defs.md#backendtypedef) 
## CreateBranchRequestRequestTypeDef

```python
# CreateBranchRequestRequestTypeDef definition

class CreateBranchRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    description: NotRequired[str],
    stage: NotRequired[StageType],  # (1)
    framework: NotRequired[str],
    enableNotification: NotRequired[bool],
    enableAutoBuild: NotRequired[bool],
    environmentVariables: NotRequired[Mapping[str, str]],
    basicAuthCredentials: NotRequired[str],
    enableBasicAuth: NotRequired[bool],
    enablePerformanceMode: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
    buildSpec: NotRequired[str],
    ttl: NotRequired[str],
    displayName: NotRequired[str],
    enablePullRequestPreview: NotRequired[bool],
    pullRequestEnvironmentName: NotRequired[str],
    backendEnvironmentArn: NotRequired[str],
    backend: NotRequired[BackendTypeDef],  # (2)
```

1. See [:material-code-brackets: StageType](./literals.md#stagetype) 
2. See [:material-code-braces: BackendTypeDef](./type_defs.md#backendtypedef) 
## UpdateBranchRequestRequestTypeDef

```python
# UpdateBranchRequestRequestTypeDef definition

class UpdateBranchRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    description: NotRequired[str],
    framework: NotRequired[str],
    stage: NotRequired[StageType],  # (1)
    enableNotification: NotRequired[bool],
    enableAutoBuild: NotRequired[bool],
    environmentVariables: NotRequired[Mapping[str, str]],
    basicAuthCredentials: NotRequired[str],
    enableBasicAuth: NotRequired[bool],
    enablePerformanceMode: NotRequired[bool],
    buildSpec: NotRequired[str],
    ttl: NotRequired[str],
    displayName: NotRequired[str],
    enablePullRequestPreview: NotRequired[bool],
    pullRequestEnvironmentName: NotRequired[str],
    backendEnvironmentArn: NotRequired[str],
    backend: NotRequired[BackendTypeDef],  # (2)
```

1. See [:material-code-brackets: StageType](./literals.md#stagetype) 
2. See [:material-code-braces: BackendTypeDef](./type_defs.md#backendtypedef) 
## CreateBackendEnvironmentResultTypeDef

```python
# CreateBackendEnvironmentResultTypeDef definition

class CreateBackendEnvironmentResultTypeDef(TypedDict):
    backendEnvironment: BackendEnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackendEnvironmentTypeDef](./type_defs.md#backendenvironmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDeploymentResultTypeDef

```python
# CreateDeploymentResultTypeDef definition

class CreateDeploymentResultTypeDef(TypedDict):
    jobId: str,
    fileUploadUrls: Dict[str, str],
    zipUploadUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackendEnvironmentResultTypeDef

```python
# DeleteBackendEnvironmentResultTypeDef definition

class DeleteBackendEnvironmentResultTypeDef(TypedDict):
    backendEnvironment: BackendEnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackendEnvironmentTypeDef](./type_defs.md#backendenvironmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateAccessLogsResultTypeDef

```python
# GenerateAccessLogsResultTypeDef definition

class GenerateAccessLogsResultTypeDef(TypedDict):
    logUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetArtifactUrlResultTypeDef

```python
# GetArtifactUrlResultTypeDef definition

class GetArtifactUrlResultTypeDef(TypedDict):
    artifactId: str,
    artifactUrl: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBackendEnvironmentResultTypeDef

```python
# GetBackendEnvironmentResultTypeDef definition

class GetBackendEnvironmentResultTypeDef(TypedDict):
    backendEnvironment: BackendEnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackendEnvironmentTypeDef](./type_defs.md#backendenvironmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListArtifactsResultTypeDef

```python
# ListArtifactsResultTypeDef definition

class ListArtifactsResultTypeDef(TypedDict):
    artifacts: List[ArtifactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ArtifactTypeDef](./type_defs.md#artifacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackendEnvironmentsResultTypeDef

```python
# ListBackendEnvironmentsResultTypeDef definition

class ListBackendEnvironmentsResultTypeDef(TypedDict):
    backendEnvironments: List[BackendEnvironmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BackendEnvironmentTypeDef](./type_defs.md#backendenvironmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainAssociationRequestRequestTypeDef

```python
# CreateDomainAssociationRequestRequestTypeDef definition

class CreateDomainAssociationRequestRequestTypeDef(TypedDict):
    appId: str,
    domainName: str,
    subDomainSettings: Sequence[SubDomainSettingTypeDef],  # (1)
    enableAutoSubDomain: NotRequired[bool],
    autoSubDomainCreationPatterns: NotRequired[Sequence[str]],
    autoSubDomainIAMRole: NotRequired[str],
    certificateSettings: NotRequired[CertificateSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: SubDomainSettingTypeDef](./type_defs.md#subdomainsettingtypedef) 
2. See [:material-code-braces: CertificateSettingsTypeDef](./type_defs.md#certificatesettingstypedef) 
## SubDomainTypeDef

```python
# SubDomainTypeDef definition

class SubDomainTypeDef(TypedDict):
    subDomainSetting: SubDomainSettingTypeDef,  # (1)
    verified: bool,
    dnsRecord: str,
```

1. See [:material-code-braces: SubDomainSettingTypeDef](./type_defs.md#subdomainsettingtypedef) 
## UpdateDomainAssociationRequestRequestTypeDef

```python
# UpdateDomainAssociationRequestRequestTypeDef definition

class UpdateDomainAssociationRequestRequestTypeDef(TypedDict):
    appId: str,
    domainName: str,
    enableAutoSubDomain: NotRequired[bool],
    subDomainSettings: NotRequired[Sequence[SubDomainSettingTypeDef]],  # (1)
    autoSubDomainCreationPatterns: NotRequired[Sequence[str]],
    autoSubDomainIAMRole: NotRequired[str],
    certificateSettings: NotRequired[CertificateSettingsTypeDef],  # (2)
```

1. See [:material-code-braces: SubDomainSettingTypeDef](./type_defs.md#subdomainsettingtypedef) 
2. See [:material-code-braces: CertificateSettingsTypeDef](./type_defs.md#certificatesettingstypedef) 
## CreateWebhookResultTypeDef

```python
# CreateWebhookResultTypeDef definition

class CreateWebhookResultTypeDef(TypedDict):
    webhook: WebhookTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebhookTypeDef](./type_defs.md#webhooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteWebhookResultTypeDef

```python
# DeleteWebhookResultTypeDef definition

class DeleteWebhookResultTypeDef(TypedDict):
    webhook: WebhookTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebhookTypeDef](./type_defs.md#webhooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWebhookResultTypeDef

```python
# GetWebhookResultTypeDef definition

class GetWebhookResultTypeDef(TypedDict):
    webhook: WebhookTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebhookTypeDef](./type_defs.md#webhooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWebhooksResultTypeDef

```python
# ListWebhooksResultTypeDef definition

class ListWebhooksResultTypeDef(TypedDict):
    webhooks: List[WebhookTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WebhookTypeDef](./type_defs.md#webhooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateWebhookResultTypeDef

```python
# UpdateWebhookResultTypeDef definition

class UpdateWebhookResultTypeDef(TypedDict):
    webhook: WebhookTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WebhookTypeDef](./type_defs.md#webhooktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteJobResultTypeDef

```python
# DeleteJobResultTypeDef definition

class DeleteJobResultTypeDef(TypedDict):
    jobSummary: JobSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListJobsResultTypeDef

```python
# ListJobsResultTypeDef definition

class ListJobsResultTypeDef(TypedDict):
    jobSummaries: List[JobSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDeploymentResultTypeDef

```python
# StartDeploymentResultTypeDef definition

class StartDeploymentResultTypeDef(TypedDict):
    jobSummary: JobSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartJobResultTypeDef

```python
# StartJobResultTypeDef definition

class StartJobResultTypeDef(TypedDict):
    jobSummary: JobSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopJobResultTypeDef

```python
# StopJobResultTypeDef definition

class StopJobResultTypeDef(TypedDict):
    jobSummary: JobSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateAccessLogsRequestRequestTypeDef

```python
# GenerateAccessLogsRequestRequestTypeDef definition

class GenerateAccessLogsRequestRequestTypeDef(TypedDict):
    domainName: str,
    appId: str,
    startTime: NotRequired[TimestampTypeDef],
    endTime: NotRequired[TimestampTypeDef],
```

## StartJobRequestRequestTypeDef

```python
# StartJobRequestRequestTypeDef definition

class StartJobRequestRequestTypeDef(TypedDict):
    appId: str,
    branchName: str,
    jobType: JobTypeType,  # (1)
    jobId: NotRequired[str],
    jobReason: NotRequired[str],
    commitId: NotRequired[str],
    commitMessage: NotRequired[str],
    commitTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
## JobTypeDef

```python
# JobTypeDef definition

class JobTypeDef(TypedDict):
    summary: JobSummaryTypeDef,  # (1)
    steps: List[StepTypeDef],  # (2)
```

1. See [:material-code-braces: JobSummaryTypeDef](./type_defs.md#jobsummarytypedef) 
2. See [:material-code-braces: StepTypeDef](./type_defs.md#steptypedef) 
## ListAppsRequestPaginateTypeDef

```python
# ListAppsRequestPaginateTypeDef definition

class ListAppsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBranchesRequestPaginateTypeDef

```python
# ListBranchesRequestPaginateTypeDef definition

class ListBranchesRequestPaginateTypeDef(TypedDict):
    appId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainAssociationsRequestPaginateTypeDef

```python
# ListDomainAssociationsRequestPaginateTypeDef definition

class ListDomainAssociationsRequestPaginateTypeDef(TypedDict):
    appId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobsRequestPaginateTypeDef

```python
# ListJobsRequestPaginateTypeDef definition

class ListJobsRequestPaginateTypeDef(TypedDict):
    appId: str,
    branchName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## CreateAppResultTypeDef

```python
# CreateAppResultTypeDef definition

class CreateAppResultTypeDef(TypedDict):
    app: AppTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteAppResultTypeDef

```python
# DeleteAppResultTypeDef definition

class DeleteAppResultTypeDef(TypedDict):
    app: AppTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppResultTypeDef

```python
# GetAppResultTypeDef definition

class GetAppResultTypeDef(TypedDict):
    app: AppTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAppsResultTypeDef

```python
# ListAppsResultTypeDef definition

class ListAppsResultTypeDef(TypedDict):
    apps: List[AppTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppResultTypeDef

```python
# UpdateAppResultTypeDef definition

class UpdateAppResultTypeDef(TypedDict):
    app: AppTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AppTypeDef](./type_defs.md#apptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateBranchResultTypeDef

```python
# CreateBranchResultTypeDef definition

class CreateBranchResultTypeDef(TypedDict):
    branch: BranchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBranchResultTypeDef

```python
# DeleteBranchResultTypeDef definition

class DeleteBranchResultTypeDef(TypedDict):
    branch: BranchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetBranchResultTypeDef

```python
# GetBranchResultTypeDef definition

class GetBranchResultTypeDef(TypedDict):
    branch: BranchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBranchesResultTypeDef

```python
# ListBranchesResultTypeDef definition

class ListBranchesResultTypeDef(TypedDict):
    branches: List[BranchTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateBranchResultTypeDef

```python
# UpdateBranchResultTypeDef definition

class UpdateBranchResultTypeDef(TypedDict):
    branch: BranchTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BranchTypeDef](./type_defs.md#branchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DomainAssociationTypeDef

```python
# DomainAssociationTypeDef definition

class DomainAssociationTypeDef(TypedDict):
    domainAssociationArn: str,
    domainName: str,
    enableAutoSubDomain: bool,
    domainStatus: DomainStatusType,  # (1)
    statusReason: str,
    subDomains: List[SubDomainTypeDef],  # (3)
    autoSubDomainCreationPatterns: NotRequired[List[str]],
    autoSubDomainIAMRole: NotRequired[str],
    updateStatus: NotRequired[UpdateStatusType],  # (2)
    certificateVerificationDNSRecord: NotRequired[str],
    certificate: NotRequired[CertificateTypeDef],  # (4)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-brackets: UpdateStatusType](./literals.md#updatestatustype) 
3. See [:material-code-braces: SubDomainTypeDef](./type_defs.md#subdomaintypedef) 
4. See [:material-code-braces: CertificateTypeDef](./type_defs.md#certificatetypedef) 
## GetJobResultTypeDef

```python
# GetJobResultTypeDef definition

class GetJobResultTypeDef(TypedDict):
    job: JobTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobTypeDef](./type_defs.md#jobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDomainAssociationResultTypeDef

```python
# CreateDomainAssociationResultTypeDef definition

class CreateDomainAssociationResultTypeDef(TypedDict):
    domainAssociation: DomainAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainAssociationTypeDef](./type_defs.md#domainassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainAssociationResultTypeDef

```python
# DeleteDomainAssociationResultTypeDef definition

class DeleteDomainAssociationResultTypeDef(TypedDict):
    domainAssociation: DomainAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainAssociationTypeDef](./type_defs.md#domainassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainAssociationResultTypeDef

```python
# GetDomainAssociationResultTypeDef definition

class GetDomainAssociationResultTypeDef(TypedDict):
    domainAssociation: DomainAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainAssociationTypeDef](./type_defs.md#domainassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainAssociationsResultTypeDef

```python
# ListDomainAssociationsResultTypeDef definition

class ListDomainAssociationsResultTypeDef(TypedDict):
    domainAssociations: List[DomainAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainAssociationTypeDef](./type_defs.md#domainassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainAssociationResultTypeDef

```python
# UpdateDomainAssociationResultTypeDef definition

class UpdateDomainAssociationResultTypeDef(TypedDict):
    domainAssociation: DomainAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainAssociationTypeDef](./type_defs.md#domainassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

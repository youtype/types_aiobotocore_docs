# Type definitions

> [Index](../README.md) > [Proton](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Proton](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/proton.html#Proton)
    type annotations stubs module [types-aiobotocore-proton](https://pypi.org/project/types-aiobotocore-proton/).



## AcceptEnvironmentAccountConnectionInputRequestTypeDef

```python
# AcceptEnvironmentAccountConnectionInputRequestTypeDef definition

class AcceptEnvironmentAccountConnectionInputRequestTypeDef(TypedDict):
    id: str,
```

## EnvironmentAccountConnectionTypeDef

```python
# EnvironmentAccountConnectionTypeDef definition

class EnvironmentAccountConnectionTypeDef(TypedDict):
    arn: str,
    environmentAccountId: str,
    environmentName: str,
    id: str,
    lastModifiedAt: datetime,
    managementAccountId: str,
    requestedAt: datetime,
    roleArn: str,
    status: EnvironmentAccountConnectionStatusType,  # (1)
    codebuildRoleArn: NotRequired[str],
    componentRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentAccountConnectionStatusType](./literals.md#environmentaccountconnectionstatustype) 
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

## RepositoryBranchTypeDef

```python
# RepositoryBranchTypeDef definition

class RepositoryBranchTypeDef(TypedDict):
    arn: str,
    branch: str,
    name: str,
    provider: RepositoryProviderType,  # (1)
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## CancelComponentDeploymentInputRequestTypeDef

```python
# CancelComponentDeploymentInputRequestTypeDef definition

class CancelComponentDeploymentInputRequestTypeDef(TypedDict):
    componentName: str,
```

## ComponentTypeDef

```python
# ComponentTypeDef definition

class ComponentTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    environmentName: str,
    lastModifiedAt: datetime,
    name: str,
    deploymentStatusMessage: NotRequired[str],
    description: NotRequired[str],
    lastAttemptedDeploymentId: NotRequired[str],
    lastClientRequestToken: NotRequired[str],
    lastDeploymentAttemptedAt: NotRequired[datetime],
    lastDeploymentSucceededAt: NotRequired[datetime],
    lastSucceededDeploymentId: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
    serviceSpec: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## CancelEnvironmentDeploymentInputRequestTypeDef

```python
# CancelEnvironmentDeploymentInputRequestTypeDef definition

class CancelEnvironmentDeploymentInputRequestTypeDef(TypedDict):
    environmentName: str,
```

## CancelServiceInstanceDeploymentInputRequestTypeDef

```python
# CancelServiceInstanceDeploymentInputRequestTypeDef definition

class CancelServiceInstanceDeploymentInputRequestTypeDef(TypedDict):
    serviceInstanceName: str,
    serviceName: str,
```

## ServiceInstanceTypeDef

```python
# ServiceInstanceTypeDef definition

class ServiceInstanceTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    environmentName: str,
    lastDeploymentAttemptedAt: datetime,
    lastDeploymentSucceededAt: datetime,
    name: str,
    serviceName: str,
    templateMajorVersion: str,
    templateMinorVersion: str,
    templateName: str,
    deploymentStatusMessage: NotRequired[str],
    lastAttemptedDeploymentId: NotRequired[str],
    lastClientRequestToken: NotRequired[str],
    lastSucceededDeploymentId: NotRequired[str],
    spec: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## CancelServicePipelineDeploymentInputRequestTypeDef

```python
# CancelServicePipelineDeploymentInputRequestTypeDef definition

class CancelServicePipelineDeploymentInputRequestTypeDef(TypedDict):
    serviceName: str,
```

## ServicePipelineTypeDef

```python
# ServicePipelineTypeDef definition

class ServicePipelineTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    lastDeploymentAttemptedAt: datetime,
    lastDeploymentSucceededAt: datetime,
    templateMajorVersion: str,
    templateMinorVersion: str,
    templateName: str,
    deploymentStatusMessage: NotRequired[str],
    lastAttemptedDeploymentId: NotRequired[str],
    lastSucceededDeploymentId: NotRequired[str],
    spec: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## CompatibleEnvironmentTemplateInputTypeDef

```python
# CompatibleEnvironmentTemplateInputTypeDef definition

class CompatibleEnvironmentTemplateInputTypeDef(TypedDict):
    majorVersion: str,
    templateName: str,
```

## CompatibleEnvironmentTemplateTypeDef

```python
# CompatibleEnvironmentTemplateTypeDef definition

class CompatibleEnvironmentTemplateTypeDef(TypedDict):
    majorVersion: str,
    templateName: str,
```

## ComponentStateTypeDef

```python
# ComponentStateTypeDef definition

class ComponentStateTypeDef(TypedDict):
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
    serviceSpec: NotRequired[str],
    templateFile: NotRequired[str],
```

## ComponentSummaryTypeDef

```python
# ComponentSummaryTypeDef definition

class ComponentSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    environmentName: str,
    lastModifiedAt: datetime,
    name: str,
    deploymentStatusMessage: NotRequired[str],
    lastAttemptedDeploymentId: NotRequired[str],
    lastDeploymentAttemptedAt: NotRequired[datetime],
    lastDeploymentSucceededAt: NotRequired[datetime],
    lastSucceededDeploymentId: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## ResourceCountsSummaryTypeDef

```python
# ResourceCountsSummaryTypeDef definition

class ResourceCountsSummaryTypeDef(TypedDict):
    total: int,
    behindMajor: NotRequired[int],
    behindMinor: NotRequired[int],
    failed: NotRequired[int],
    upToDate: NotRequired[int],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: str,
    value: str,
```

## RepositoryBranchInputTypeDef

```python
# RepositoryBranchInputTypeDef definition

class RepositoryBranchInputTypeDef(TypedDict):
    branch: str,
    name: str,
    provider: RepositoryProviderType,  # (1)
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## EnvironmentTemplateTypeDef

```python
# EnvironmentTemplateTypeDef definition

class EnvironmentTemplateTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    name: str,
    description: NotRequired[str],
    displayName: NotRequired[str],
    encryptionKey: NotRequired[str],
    provisioning: NotRequired[ProvisioningType],  # (1)
    recommendedVersion: NotRequired[str],
```

1. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
## EnvironmentTemplateVersionTypeDef

```python
# EnvironmentTemplateVersionTypeDef definition

class EnvironmentTemplateVersionTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    majorVersion: str,
    minorVersion: str,
    status: TemplateVersionStatusType,  # (1)
    templateName: str,
    description: NotRequired[str],
    recommendedMinorVersion: NotRequired[str],
    schema: NotRequired[str],
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: TemplateVersionStatusType](./literals.md#templateversionstatustype) 
## RepositoryTypeDef

```python
# RepositoryTypeDef definition

class RepositoryTypeDef(TypedDict):
    arn: str,
    connectionArn: str,
    name: str,
    provider: RepositoryProviderType,  # (1)
    encryptionKey: NotRequired[str],
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## CreateServiceSyncConfigInputRequestTypeDef

```python
# CreateServiceSyncConfigInputRequestTypeDef definition

class CreateServiceSyncConfigInputRequestTypeDef(TypedDict):
    branch: str,
    filePath: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    serviceName: str,
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## ServiceSyncConfigTypeDef

```python
# ServiceSyncConfigTypeDef definition

class ServiceSyncConfigTypeDef(TypedDict):
    branch: str,
    filePath: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    serviceName: str,
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## ServiceTemplateTypeDef

```python
# ServiceTemplateTypeDef definition

class ServiceTemplateTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    name: str,
    description: NotRequired[str],
    displayName: NotRequired[str],
    encryptionKey: NotRequired[str],
    pipelineProvisioning: NotRequired[ProvisioningType],  # (1)
    recommendedVersion: NotRequired[str],
```

1. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
## CreateTemplateSyncConfigInputRequestTypeDef

```python
# CreateTemplateSyncConfigInputRequestTypeDef definition

class CreateTemplateSyncConfigInputRequestTypeDef(TypedDict):
    branch: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    templateName: str,
    templateType: TemplateTypeType,  # (2)
    subdirectory: NotRequired[str],
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## TemplateSyncConfigTypeDef

```python
# TemplateSyncConfigTypeDef definition

class TemplateSyncConfigTypeDef(TypedDict):
    branch: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    templateName: str,
    templateType: TemplateTypeType,  # (2)
    subdirectory: NotRequired[str],
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## DeleteComponentInputRequestTypeDef

```python
# DeleteComponentInputRequestTypeDef definition

class DeleteComponentInputRequestTypeDef(TypedDict):
    name: str,
```

## DeleteDeploymentInputRequestTypeDef

```python
# DeleteDeploymentInputRequestTypeDef definition

class DeleteDeploymentInputRequestTypeDef(TypedDict):
    id: str,
```

## DeleteEnvironmentAccountConnectionInputRequestTypeDef

```python
# DeleteEnvironmentAccountConnectionInputRequestTypeDef definition

class DeleteEnvironmentAccountConnectionInputRequestTypeDef(TypedDict):
    id: str,
```

## DeleteEnvironmentInputRequestTypeDef

```python
# DeleteEnvironmentInputRequestTypeDef definition

class DeleteEnvironmentInputRequestTypeDef(TypedDict):
    name: str,
```

## DeleteEnvironmentTemplateInputRequestTypeDef

```python
# DeleteEnvironmentTemplateInputRequestTypeDef definition

class DeleteEnvironmentTemplateInputRequestTypeDef(TypedDict):
    name: str,
```

## DeleteEnvironmentTemplateVersionInputRequestTypeDef

```python
# DeleteEnvironmentTemplateVersionInputRequestTypeDef definition

class DeleteEnvironmentTemplateVersionInputRequestTypeDef(TypedDict):
    majorVersion: str,
    minorVersion: str,
    templateName: str,
```

## DeleteRepositoryInputRequestTypeDef

```python
# DeleteRepositoryInputRequestTypeDef definition

class DeleteRepositoryInputRequestTypeDef(TypedDict):
    name: str,
    provider: RepositoryProviderType,  # (1)
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## DeleteServiceInputRequestTypeDef

```python
# DeleteServiceInputRequestTypeDef definition

class DeleteServiceInputRequestTypeDef(TypedDict):
    name: str,
```

## DeleteServiceSyncConfigInputRequestTypeDef

```python
# DeleteServiceSyncConfigInputRequestTypeDef definition

class DeleteServiceSyncConfigInputRequestTypeDef(TypedDict):
    serviceName: str,
```

## DeleteServiceTemplateInputRequestTypeDef

```python
# DeleteServiceTemplateInputRequestTypeDef definition

class DeleteServiceTemplateInputRequestTypeDef(TypedDict):
    name: str,
```

## DeleteServiceTemplateVersionInputRequestTypeDef

```python
# DeleteServiceTemplateVersionInputRequestTypeDef definition

class DeleteServiceTemplateVersionInputRequestTypeDef(TypedDict):
    majorVersion: str,
    minorVersion: str,
    templateName: str,
```

## DeleteTemplateSyncConfigInputRequestTypeDef

```python
# DeleteTemplateSyncConfigInputRequestTypeDef definition

class DeleteTemplateSyncConfigInputRequestTypeDef(TypedDict):
    templateName: str,
    templateType: TemplateTypeType,  # (1)
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## EnvironmentStateTypeDef

```python
# EnvironmentStateTypeDef definition

class EnvironmentStateTypeDef(TypedDict):
    templateMajorVersion: str,
    templateMinorVersion: str,
    templateName: str,
    spec: NotRequired[str],
```

## ServiceInstanceStateTypeDef

```python
# ServiceInstanceStateTypeDef definition

class ServiceInstanceStateTypeDef(TypedDict):
    spec: str,
    templateMajorVersion: str,
    templateMinorVersion: str,
    templateName: str,
    lastSuccessfulComponentDeploymentIds: NotRequired[List[str]],
    lastSuccessfulEnvironmentDeploymentId: NotRequired[str],
    lastSuccessfulServicePipelineDeploymentId: NotRequired[str],
```

## ServicePipelineStateTypeDef

```python
# ServicePipelineStateTypeDef definition

class ServicePipelineStateTypeDef(TypedDict):
    templateMajorVersion: str,
    templateMinorVersion: str,
    templateName: str,
    spec: NotRequired[str],
```

## DeploymentSummaryTypeDef

```python
# DeploymentSummaryTypeDef definition

class DeploymentSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    environmentName: str,
    id: str,
    lastModifiedAt: datetime,
    targetArn: str,
    targetResourceCreatedAt: datetime,
    targetResourceType: DeploymentTargetResourceTypeType,  # (2)
    completedAt: NotRequired[datetime],
    componentName: NotRequired[str],
    lastAttemptedDeploymentId: NotRequired[str],
    lastSucceededDeploymentId: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-brackets: DeploymentTargetResourceTypeType](./literals.md#deploymenttargetresourcetypetype) 
## EnvironmentAccountConnectionSummaryTypeDef

```python
# EnvironmentAccountConnectionSummaryTypeDef definition

class EnvironmentAccountConnectionSummaryTypeDef(TypedDict):
    arn: str,
    environmentAccountId: str,
    environmentName: str,
    id: str,
    lastModifiedAt: datetime,
    managementAccountId: str,
    requestedAt: datetime,
    roleArn: str,
    status: EnvironmentAccountConnectionStatusType,  # (1)
    componentRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentAccountConnectionStatusType](./literals.md#environmentaccountconnectionstatustype) 
## EnvironmentSummaryTypeDef

```python
# EnvironmentSummaryTypeDef definition

class EnvironmentSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    lastDeploymentAttemptedAt: datetime,
    lastDeploymentSucceededAt: datetime,
    name: str,
    templateMajorVersion: str,
    templateMinorVersion: str,
    templateName: str,
    componentRoleArn: NotRequired[str],
    deploymentStatusMessage: NotRequired[str],
    description: NotRequired[str],
    environmentAccountConnectionId: NotRequired[str],
    environmentAccountId: NotRequired[str],
    lastAttemptedDeploymentId: NotRequired[str],
    lastSucceededDeploymentId: NotRequired[str],
    protonServiceRoleArn: NotRequired[str],
    provisioning: NotRequired[ProvisioningType],  # (2)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
## EnvironmentTemplateFilterTypeDef

```python
# EnvironmentTemplateFilterTypeDef definition

class EnvironmentTemplateFilterTypeDef(TypedDict):
    majorVersion: str,
    templateName: str,
```

## EnvironmentTemplateSummaryTypeDef

```python
# EnvironmentTemplateSummaryTypeDef definition

class EnvironmentTemplateSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    name: str,
    description: NotRequired[str],
    displayName: NotRequired[str],
    provisioning: NotRequired[ProvisioningType],  # (1)
    recommendedVersion: NotRequired[str],
```

1. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
## EnvironmentTemplateVersionSummaryTypeDef

```python
# EnvironmentTemplateVersionSummaryTypeDef definition

class EnvironmentTemplateVersionSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    majorVersion: str,
    minorVersion: str,
    status: TemplateVersionStatusType,  # (1)
    templateName: str,
    description: NotRequired[str],
    recommendedMinorVersion: NotRequired[str],
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: TemplateVersionStatusType](./literals.md#templateversionstatustype) 
## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## GetComponentInputRequestTypeDef

```python
# GetComponentInputRequestTypeDef definition

class GetComponentInputRequestTypeDef(TypedDict):
    name: str,
```

## GetDeploymentInputRequestTypeDef

```python
# GetDeploymentInputRequestTypeDef definition

class GetDeploymentInputRequestTypeDef(TypedDict):
    id: str,
    componentName: NotRequired[str],
    environmentName: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
```

## GetEnvironmentAccountConnectionInputRequestTypeDef

```python
# GetEnvironmentAccountConnectionInputRequestTypeDef definition

class GetEnvironmentAccountConnectionInputRequestTypeDef(TypedDict):
    id: str,
```

## GetEnvironmentInputRequestTypeDef

```python
# GetEnvironmentInputRequestTypeDef definition

class GetEnvironmentInputRequestTypeDef(TypedDict):
    name: str,
```

## GetEnvironmentTemplateInputRequestTypeDef

```python
# GetEnvironmentTemplateInputRequestTypeDef definition

class GetEnvironmentTemplateInputRequestTypeDef(TypedDict):
    name: str,
```

## GetEnvironmentTemplateVersionInputRequestTypeDef

```python
# GetEnvironmentTemplateVersionInputRequestTypeDef definition

class GetEnvironmentTemplateVersionInputRequestTypeDef(TypedDict):
    majorVersion: str,
    minorVersion: str,
    templateName: str,
```

## GetRepositoryInputRequestTypeDef

```python
# GetRepositoryInputRequestTypeDef definition

class GetRepositoryInputRequestTypeDef(TypedDict):
    name: str,
    provider: RepositoryProviderType,  # (1)
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## GetRepositorySyncStatusInputRequestTypeDef

```python
# GetRepositorySyncStatusInputRequestTypeDef definition

class GetRepositorySyncStatusInputRequestTypeDef(TypedDict):
    branch: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    syncType: SyncTypeType,  # (2)
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: SyncTypeType](./literals.md#synctypetype) 
## GetServiceInputRequestTypeDef

```python
# GetServiceInputRequestTypeDef definition

class GetServiceInputRequestTypeDef(TypedDict):
    name: str,
```

## GetServiceInstanceInputRequestTypeDef

```python
# GetServiceInstanceInputRequestTypeDef definition

class GetServiceInstanceInputRequestTypeDef(TypedDict):
    name: str,
    serviceName: str,
```

## GetServiceInstanceSyncStatusInputRequestTypeDef

```python
# GetServiceInstanceSyncStatusInputRequestTypeDef definition

class GetServiceInstanceSyncStatusInputRequestTypeDef(TypedDict):
    serviceInstanceName: str,
    serviceName: str,
```

## RevisionTypeDef

```python
# RevisionTypeDef definition

class RevisionTypeDef(TypedDict):
    branch: str,
    directory: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    sha: str,
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## GetServiceSyncBlockerSummaryInputRequestTypeDef

```python
# GetServiceSyncBlockerSummaryInputRequestTypeDef definition

class GetServiceSyncBlockerSummaryInputRequestTypeDef(TypedDict):
    serviceName: str,
    serviceInstanceName: NotRequired[str],
```

## GetServiceSyncConfigInputRequestTypeDef

```python
# GetServiceSyncConfigInputRequestTypeDef definition

class GetServiceSyncConfigInputRequestTypeDef(TypedDict):
    serviceName: str,
```

## GetServiceTemplateInputRequestTypeDef

```python
# GetServiceTemplateInputRequestTypeDef definition

class GetServiceTemplateInputRequestTypeDef(TypedDict):
    name: str,
```

## GetServiceTemplateVersionInputRequestTypeDef

```python
# GetServiceTemplateVersionInputRequestTypeDef definition

class GetServiceTemplateVersionInputRequestTypeDef(TypedDict):
    majorVersion: str,
    minorVersion: str,
    templateName: str,
```

## GetTemplateSyncConfigInputRequestTypeDef

```python
# GetTemplateSyncConfigInputRequestTypeDef definition

class GetTemplateSyncConfigInputRequestTypeDef(TypedDict):
    templateName: str,
    templateType: TemplateTypeType,  # (1)
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## GetTemplateSyncStatusInputRequestTypeDef

```python
# GetTemplateSyncStatusInputRequestTypeDef definition

class GetTemplateSyncStatusInputRequestTypeDef(TypedDict):
    templateName: str,
    templateType: TemplateTypeType,  # (1)
    templateVersion: str,
```

1. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListComponentOutputsInputRequestTypeDef

```python
# ListComponentOutputsInputRequestTypeDef definition

class ListComponentOutputsInputRequestTypeDef(TypedDict):
    componentName: str,
    deploymentId: NotRequired[str],
    nextToken: NotRequired[str],
```

## OutputTypeDef

```python
# OutputTypeDef definition

class OutputTypeDef(TypedDict):
    key: NotRequired[str],
    valueString: NotRequired[str],
```

## ListComponentProvisionedResourcesInputRequestTypeDef

```python
# ListComponentProvisionedResourcesInputRequestTypeDef definition

class ListComponentProvisionedResourcesInputRequestTypeDef(TypedDict):
    componentName: str,
    nextToken: NotRequired[str],
```

## ProvisionedResourceTypeDef

```python
# ProvisionedResourceTypeDef definition

class ProvisionedResourceTypeDef(TypedDict):
    identifier: NotRequired[str],
    name: NotRequired[str],
    provisioningEngine: NotRequired[ProvisionedResourceEngineType],  # (1)
```

1. See [:material-code-brackets: ProvisionedResourceEngineType](./literals.md#provisionedresourceenginetype) 
## ListComponentsInputRequestTypeDef

```python
# ListComponentsInputRequestTypeDef definition

class ListComponentsInputRequestTypeDef(TypedDict):
    environmentName: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
```

## ListDeploymentsInputRequestTypeDef

```python
# ListDeploymentsInputRequestTypeDef definition

class ListDeploymentsInputRequestTypeDef(TypedDict):
    componentName: NotRequired[str],
    environmentName: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
```

## ListEnvironmentAccountConnectionsInputRequestTypeDef

```python
# ListEnvironmentAccountConnectionsInputRequestTypeDef definition

class ListEnvironmentAccountConnectionsInputRequestTypeDef(TypedDict):
    requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,  # (1)
    environmentName: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    statuses: NotRequired[Sequence[EnvironmentAccountConnectionStatusType]],  # (2)
```

1. See [:material-code-brackets: EnvironmentAccountConnectionRequesterAccountTypeType](./literals.md#environmentaccountconnectionrequesteraccounttypetype) 
2. See [:material-code-brackets: EnvironmentAccountConnectionStatusType](./literals.md#environmentaccountconnectionstatustype) 
## ListEnvironmentOutputsInputRequestTypeDef

```python
# ListEnvironmentOutputsInputRequestTypeDef definition

class ListEnvironmentOutputsInputRequestTypeDef(TypedDict):
    environmentName: str,
    deploymentId: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListEnvironmentProvisionedResourcesInputRequestTypeDef

```python
# ListEnvironmentProvisionedResourcesInputRequestTypeDef definition

class ListEnvironmentProvisionedResourcesInputRequestTypeDef(TypedDict):
    environmentName: str,
    nextToken: NotRequired[str],
```

## ListEnvironmentTemplateVersionsInputRequestTypeDef

```python
# ListEnvironmentTemplateVersionsInputRequestTypeDef definition

class ListEnvironmentTemplateVersionsInputRequestTypeDef(TypedDict):
    templateName: str,
    majorVersion: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEnvironmentTemplatesInputRequestTypeDef

```python
# ListEnvironmentTemplatesInputRequestTypeDef definition

class ListEnvironmentTemplatesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListRepositoriesInputRequestTypeDef

```python
# ListRepositoriesInputRequestTypeDef definition

class ListRepositoriesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## RepositorySummaryTypeDef

```python
# RepositorySummaryTypeDef definition

class RepositorySummaryTypeDef(TypedDict):
    arn: str,
    connectionArn: str,
    name: str,
    provider: RepositoryProviderType,  # (1)
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## ListRepositorySyncDefinitionsInputRequestTypeDef

```python
# ListRepositorySyncDefinitionsInputRequestTypeDef definition

class ListRepositorySyncDefinitionsInputRequestTypeDef(TypedDict):
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    syncType: SyncTypeType,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: SyncTypeType](./literals.md#synctypetype) 
## RepositorySyncDefinitionTypeDef

```python
# RepositorySyncDefinitionTypeDef definition

class RepositorySyncDefinitionTypeDef(TypedDict):
    branch: str,
    directory: str,
    parent: str,
    target: str,
```

## ListServiceInstanceOutputsInputRequestTypeDef

```python
# ListServiceInstanceOutputsInputRequestTypeDef definition

class ListServiceInstanceOutputsInputRequestTypeDef(TypedDict):
    serviceInstanceName: str,
    serviceName: str,
    deploymentId: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListServiceInstanceProvisionedResourcesInputRequestTypeDef

```python
# ListServiceInstanceProvisionedResourcesInputRequestTypeDef definition

class ListServiceInstanceProvisionedResourcesInputRequestTypeDef(TypedDict):
    serviceInstanceName: str,
    serviceName: str,
    nextToken: NotRequired[str],
```

## ListServiceInstancesFilterTypeDef

```python
# ListServiceInstancesFilterTypeDef definition

class ListServiceInstancesFilterTypeDef(TypedDict):
    key: NotRequired[ListServiceInstancesFilterByType],  # (1)
    value: NotRequired[str],
```

1. See [:material-code-brackets: ListServiceInstancesFilterByType](./literals.md#listserviceinstancesfilterbytype) 
## ServiceInstanceSummaryTypeDef

```python
# ServiceInstanceSummaryTypeDef definition

class ServiceInstanceSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    environmentName: str,
    lastDeploymentAttemptedAt: datetime,
    lastDeploymentSucceededAt: datetime,
    name: str,
    serviceName: str,
    templateMajorVersion: str,
    templateMinorVersion: str,
    templateName: str,
    deploymentStatusMessage: NotRequired[str],
    lastAttemptedDeploymentId: NotRequired[str],
    lastSucceededDeploymentId: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## ListServicePipelineOutputsInputRequestTypeDef

```python
# ListServicePipelineOutputsInputRequestTypeDef definition

class ListServicePipelineOutputsInputRequestTypeDef(TypedDict):
    serviceName: str,
    deploymentId: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListServicePipelineProvisionedResourcesInputRequestTypeDef

```python
# ListServicePipelineProvisionedResourcesInputRequestTypeDef definition

class ListServicePipelineProvisionedResourcesInputRequestTypeDef(TypedDict):
    serviceName: str,
    nextToken: NotRequired[str],
```

## ListServiceTemplateVersionsInputRequestTypeDef

```python
# ListServiceTemplateVersionsInputRequestTypeDef definition

class ListServiceTemplateVersionsInputRequestTypeDef(TypedDict):
    templateName: str,
    majorVersion: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceTemplateVersionSummaryTypeDef

```python
# ServiceTemplateVersionSummaryTypeDef definition

class ServiceTemplateVersionSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    majorVersion: str,
    minorVersion: str,
    status: TemplateVersionStatusType,  # (1)
    templateName: str,
    description: NotRequired[str],
    recommendedMinorVersion: NotRequired[str],
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: TemplateVersionStatusType](./literals.md#templateversionstatustype) 
## ListServiceTemplatesInputRequestTypeDef

```python
# ListServiceTemplatesInputRequestTypeDef definition

class ListServiceTemplatesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceTemplateSummaryTypeDef

```python
# ServiceTemplateSummaryTypeDef definition

class ServiceTemplateSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    name: str,
    description: NotRequired[str],
    displayName: NotRequired[str],
    pipelineProvisioning: NotRequired[ProvisioningType],  # (1)
    recommendedVersion: NotRequired[str],
```

1. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
## ListServicesInputRequestTypeDef

```python
# ListServicesInputRequestTypeDef definition

class ListServicesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ServiceSummaryTypeDef

```python
# ServiceSummaryTypeDef definition

class ServiceSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    name: str,
    status: ServiceStatusType,  # (1)
    templateName: str,
    description: NotRequired[str],
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ServiceStatusType](./literals.md#servicestatustype) 
## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## RejectEnvironmentAccountConnectionInputRequestTypeDef

```python
# RejectEnvironmentAccountConnectionInputRequestTypeDef definition

class RejectEnvironmentAccountConnectionInputRequestTypeDef(TypedDict):
    id: str,
```

## RepositorySyncEventTypeDef

```python
# RepositorySyncEventTypeDef definition

class RepositorySyncEventTypeDef(TypedDict):
    event: str,
    time: datetime,
    type: str,
    externalId: NotRequired[str],
```

## ResourceSyncEventTypeDef

```python
# ResourceSyncEventTypeDef definition

class ResourceSyncEventTypeDef(TypedDict):
    event: str,
    time: datetime,
    type: str,
    externalId: NotRequired[str],
```

## S3ObjectSourceTypeDef

```python
# S3ObjectSourceTypeDef definition

class S3ObjectSourceTypeDef(TypedDict):
    bucket: str,
    key: str,
```

## SyncBlockerContextTypeDef

```python
# SyncBlockerContextTypeDef definition

class SyncBlockerContextTypeDef(TypedDict):
    key: str,
    value: str,
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateComponentInputRequestTypeDef

```python
# UpdateComponentInputRequestTypeDef definition

class UpdateComponentInputRequestTypeDef(TypedDict):
    deploymentType: ComponentDeploymentUpdateTypeType,  # (1)
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
    serviceSpec: NotRequired[str],
    templateFile: NotRequired[str],
```

1. See [:material-code-brackets: ComponentDeploymentUpdateTypeType](./literals.md#componentdeploymentupdatetypetype) 
## UpdateEnvironmentAccountConnectionInputRequestTypeDef

```python
# UpdateEnvironmentAccountConnectionInputRequestTypeDef definition

class UpdateEnvironmentAccountConnectionInputRequestTypeDef(TypedDict):
    id: str,
    codebuildRoleArn: NotRequired[str],
    componentRoleArn: NotRequired[str],
    roleArn: NotRequired[str],
```

## UpdateEnvironmentTemplateInputRequestTypeDef

```python
# UpdateEnvironmentTemplateInputRequestTypeDef definition

class UpdateEnvironmentTemplateInputRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    displayName: NotRequired[str],
```

## UpdateEnvironmentTemplateVersionInputRequestTypeDef

```python
# UpdateEnvironmentTemplateVersionInputRequestTypeDef definition

class UpdateEnvironmentTemplateVersionInputRequestTypeDef(TypedDict):
    majorVersion: str,
    minorVersion: str,
    templateName: str,
    description: NotRequired[str],
    status: NotRequired[TemplateVersionStatusType],  # (1)
```

1. See [:material-code-brackets: TemplateVersionStatusType](./literals.md#templateversionstatustype) 
## UpdateServiceInputRequestTypeDef

```python
# UpdateServiceInputRequestTypeDef definition

class UpdateServiceInputRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    spec: NotRequired[str],
```

## UpdateServiceInstanceInputRequestTypeDef

```python
# UpdateServiceInstanceInputRequestTypeDef definition

class UpdateServiceInstanceInputRequestTypeDef(TypedDict):
    deploymentType: DeploymentUpdateTypeType,  # (1)
    name: str,
    serviceName: str,
    clientToken: NotRequired[str],
    spec: NotRequired[str],
    templateMajorVersion: NotRequired[str],
    templateMinorVersion: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype) 
## UpdateServicePipelineInputRequestTypeDef

```python
# UpdateServicePipelineInputRequestTypeDef definition

class UpdateServicePipelineInputRequestTypeDef(TypedDict):
    deploymentType: DeploymentUpdateTypeType,  # (1)
    serviceName: str,
    spec: str,
    templateMajorVersion: NotRequired[str],
    templateMinorVersion: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype) 
## UpdateServiceSyncBlockerInputRequestTypeDef

```python
# UpdateServiceSyncBlockerInputRequestTypeDef definition

class UpdateServiceSyncBlockerInputRequestTypeDef(TypedDict):
    id: str,
    resolvedReason: str,
```

## UpdateServiceSyncConfigInputRequestTypeDef

```python
# UpdateServiceSyncConfigInputRequestTypeDef definition

class UpdateServiceSyncConfigInputRequestTypeDef(TypedDict):
    branch: str,
    filePath: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    serviceName: str,
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
## UpdateServiceTemplateInputRequestTypeDef

```python
# UpdateServiceTemplateInputRequestTypeDef definition

class UpdateServiceTemplateInputRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    displayName: NotRequired[str],
```

## UpdateTemplateSyncConfigInputRequestTypeDef

```python
# UpdateTemplateSyncConfigInputRequestTypeDef definition

class UpdateTemplateSyncConfigInputRequestTypeDef(TypedDict):
    branch: str,
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    templateName: str,
    templateType: TemplateTypeType,  # (2)
    subdirectory: NotRequired[str],
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: TemplateTypeType](./literals.md#templatetypetype) 
## AcceptEnvironmentAccountConnectionOutputTypeDef

```python
# AcceptEnvironmentAccountConnectionOutputTypeDef definition

class AcceptEnvironmentAccountConnectionOutputTypeDef(TypedDict):
    environmentAccountConnection: EnvironmentAccountConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentAccountConnectionTypeDef](./type_defs.md#environmentaccountconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentAccountConnectionOutputTypeDef

```python
# CreateEnvironmentAccountConnectionOutputTypeDef definition

class CreateEnvironmentAccountConnectionOutputTypeDef(TypedDict):
    environmentAccountConnection: EnvironmentAccountConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentAccountConnectionTypeDef](./type_defs.md#environmentaccountconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEnvironmentAccountConnectionOutputTypeDef

```python
# DeleteEnvironmentAccountConnectionOutputTypeDef definition

class DeleteEnvironmentAccountConnectionOutputTypeDef(TypedDict):
    environmentAccountConnection: EnvironmentAccountConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentAccountConnectionTypeDef](./type_defs.md#environmentaccountconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentAccountConnectionOutputTypeDef

```python
# GetEnvironmentAccountConnectionOutputTypeDef definition

class GetEnvironmentAccountConnectionOutputTypeDef(TypedDict):
    environmentAccountConnection: EnvironmentAccountConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentAccountConnectionTypeDef](./type_defs.md#environmentaccountconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectEnvironmentAccountConnectionOutputTypeDef

```python
# RejectEnvironmentAccountConnectionOutputTypeDef definition

class RejectEnvironmentAccountConnectionOutputTypeDef(TypedDict):
    environmentAccountConnection: EnvironmentAccountConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentAccountConnectionTypeDef](./type_defs.md#environmentaccountconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentAccountConnectionOutputTypeDef

```python
# UpdateEnvironmentAccountConnectionOutputTypeDef definition

class UpdateEnvironmentAccountConnectionOutputTypeDef(TypedDict):
    environmentAccountConnection: EnvironmentAccountConnectionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentAccountConnectionTypeDef](./type_defs.md#environmentaccountconnectiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AccountSettingsTypeDef

```python
# AccountSettingsTypeDef definition

class AccountSettingsTypeDef(TypedDict):
    pipelineCodebuildRoleArn: NotRequired[str],
    pipelineProvisioningRepository: NotRequired[RepositoryBranchTypeDef],  # (1)
    pipelineServiceRoleArn: NotRequired[str],
```

1. See [:material-code-braces: RepositoryBranchTypeDef](./type_defs.md#repositorybranchtypedef) 
## EnvironmentTypeDef

```python
# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    lastDeploymentAttemptedAt: datetime,
    lastDeploymentSucceededAt: datetime,
    name: str,
    templateMajorVersion: str,
    templateMinorVersion: str,
    templateName: str,
    codebuildRoleArn: NotRequired[str],
    componentRoleArn: NotRequired[str],
    deploymentStatusMessage: NotRequired[str],
    description: NotRequired[str],
    environmentAccountConnectionId: NotRequired[str],
    environmentAccountId: NotRequired[str],
    lastAttemptedDeploymentId: NotRequired[str],
    lastSucceededDeploymentId: NotRequired[str],
    protonServiceRoleArn: NotRequired[str],
    provisioning: NotRequired[ProvisioningType],  # (2)
    provisioningRepository: NotRequired[RepositoryBranchTypeDef],  # (3)
    spec: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
3. See [:material-code-braces: RepositoryBranchTypeDef](./type_defs.md#repositorybranchtypedef) 
## CancelComponentDeploymentOutputTypeDef

```python
# CancelComponentDeploymentOutputTypeDef definition

class CancelComponentDeploymentOutputTypeDef(TypedDict):
    component: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateComponentOutputTypeDef

```python
# CreateComponentOutputTypeDef definition

class CreateComponentOutputTypeDef(TypedDict):
    component: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteComponentOutputTypeDef

```python
# DeleteComponentOutputTypeDef definition

class DeleteComponentOutputTypeDef(TypedDict):
    component: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComponentOutputTypeDef

```python
# GetComponentOutputTypeDef definition

class GetComponentOutputTypeDef(TypedDict):
    component: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateComponentOutputTypeDef

```python
# UpdateComponentOutputTypeDef definition

class UpdateComponentOutputTypeDef(TypedDict):
    component: ComponentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentTypeDef](./type_defs.md#componenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelServiceInstanceDeploymentOutputTypeDef

```python
# CancelServiceInstanceDeploymentOutputTypeDef definition

class CancelServiceInstanceDeploymentOutputTypeDef(TypedDict):
    serviceInstance: ServiceInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceInstanceTypeDef](./type_defs.md#serviceinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceInstanceOutputTypeDef

```python
# CreateServiceInstanceOutputTypeDef definition

class CreateServiceInstanceOutputTypeDef(TypedDict):
    serviceInstance: ServiceInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceInstanceTypeDef](./type_defs.md#serviceinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceInstanceOutputTypeDef

```python
# GetServiceInstanceOutputTypeDef definition

class GetServiceInstanceOutputTypeDef(TypedDict):
    serviceInstance: ServiceInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceInstanceTypeDef](./type_defs.md#serviceinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceInstanceOutputTypeDef

```python
# UpdateServiceInstanceOutputTypeDef definition

class UpdateServiceInstanceOutputTypeDef(TypedDict):
    serviceInstance: ServiceInstanceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceInstanceTypeDef](./type_defs.md#serviceinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelServicePipelineDeploymentOutputTypeDef

```python
# CancelServicePipelineDeploymentOutputTypeDef definition

class CancelServicePipelineDeploymentOutputTypeDef(TypedDict):
    pipeline: ServicePipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServicePipelineTypeDef](./type_defs.md#servicepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceTypeDef

```python
# ServiceTypeDef definition

class ServiceTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    lastModifiedAt: datetime,
    name: str,
    spec: str,
    status: ServiceStatusType,  # (2)
    templateName: str,
    branchName: NotRequired[str],
    description: NotRequired[str],
    pipeline: NotRequired[ServicePipelineTypeDef],  # (1)
    repositoryConnectionArn: NotRequired[str],
    repositoryId: NotRequired[str],
    statusMessage: NotRequired[str],
```

1. See [:material-code-braces: ServicePipelineTypeDef](./type_defs.md#servicepipelinetypedef) 
2. See [:material-code-brackets: ServiceStatusType](./literals.md#servicestatustype) 
## UpdateServicePipelineOutputTypeDef

```python
# UpdateServicePipelineOutputTypeDef definition

class UpdateServicePipelineOutputTypeDef(TypedDict):
    pipeline: ServicePipelineTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServicePipelineTypeDef](./type_defs.md#servicepipelinetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceTemplateVersionInputRequestTypeDef

```python
# UpdateServiceTemplateVersionInputRequestTypeDef definition

class UpdateServiceTemplateVersionInputRequestTypeDef(TypedDict):
    majorVersion: str,
    minorVersion: str,
    templateName: str,
    compatibleEnvironmentTemplates: NotRequired[Sequence[CompatibleEnvironmentTemplateInputTypeDef]],  # (1)
    description: NotRequired[str],
    status: NotRequired[TemplateVersionStatusType],  # (2)
    supportedComponentSources: NotRequired[Sequence[ServiceTemplateSupportedComponentSourceTypeType]],  # (3)
```

1. See [:material-code-braces: CompatibleEnvironmentTemplateInputTypeDef](./type_defs.md#compatibleenvironmenttemplateinputtypedef) 
2. See [:material-code-brackets: TemplateVersionStatusType](./literals.md#templateversionstatustype) 
3. See [:material-code-brackets: ServiceTemplateSupportedComponentSourceTypeType](./literals.md#servicetemplatesupportedcomponentsourcetypetype) 
## ServiceTemplateVersionTypeDef

```python
# ServiceTemplateVersionTypeDef definition

class ServiceTemplateVersionTypeDef(TypedDict):
    arn: str,
    compatibleEnvironmentTemplates: List[CompatibleEnvironmentTemplateTypeDef],  # (1)
    createdAt: datetime,
    lastModifiedAt: datetime,
    majorVersion: str,
    minorVersion: str,
    status: TemplateVersionStatusType,  # (2)
    templateName: str,
    description: NotRequired[str],
    recommendedMinorVersion: NotRequired[str],
    schema: NotRequired[str],
    statusMessage: NotRequired[str],
    supportedComponentSources: NotRequired[List[ServiceTemplateSupportedComponentSourceTypeType]],  # (3)
```

1. See [:material-code-braces: CompatibleEnvironmentTemplateTypeDef](./type_defs.md#compatibleenvironmenttemplatetypedef) 
2. See [:material-code-brackets: TemplateVersionStatusType](./literals.md#templateversionstatustype) 
3. See [:material-code-brackets: ServiceTemplateSupportedComponentSourceTypeType](./literals.md#servicetemplatesupportedcomponentsourcetypetype) 
## ListComponentsOutputTypeDef

```python
# ListComponentsOutputTypeDef definition

class ListComponentsOutputTypeDef(TypedDict):
    components: List[ComponentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComponentSummaryTypeDef](./type_defs.md#componentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CountsSummaryTypeDef

```python
# CountsSummaryTypeDef definition

class CountsSummaryTypeDef(TypedDict):
    components: NotRequired[ResourceCountsSummaryTypeDef],  # (1)
    environmentTemplates: NotRequired[ResourceCountsSummaryTypeDef],  # (1)
    environments: NotRequired[ResourceCountsSummaryTypeDef],  # (1)
    pipelines: NotRequired[ResourceCountsSummaryTypeDef],  # (1)
    serviceInstances: NotRequired[ResourceCountsSummaryTypeDef],  # (1)
    serviceTemplates: NotRequired[ResourceCountsSummaryTypeDef],  # (1)
    services: NotRequired[ResourceCountsSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceCountsSummaryTypeDef](./type_defs.md#resourcecountssummarytypedef) 
2. See [:material-code-braces: ResourceCountsSummaryTypeDef](./type_defs.md#resourcecountssummarytypedef) 
3. See [:material-code-braces: ResourceCountsSummaryTypeDef](./type_defs.md#resourcecountssummarytypedef) 
4. See [:material-code-braces: ResourceCountsSummaryTypeDef](./type_defs.md#resourcecountssummarytypedef) 
5. See [:material-code-braces: ResourceCountsSummaryTypeDef](./type_defs.md#resourcecountssummarytypedef) 
6. See [:material-code-braces: ResourceCountsSummaryTypeDef](./type_defs.md#resourcecountssummarytypedef) 
7. See [:material-code-braces: ResourceCountsSummaryTypeDef](./type_defs.md#resourcecountssummarytypedef) 
## CreateComponentInputRequestTypeDef

```python
# CreateComponentInputRequestTypeDef definition

class CreateComponentInputRequestTypeDef(TypedDict):
    manifest: str,
    name: str,
    templateFile: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    environmentName: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
    serviceSpec: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEnvironmentAccountConnectionInputRequestTypeDef

```python
# CreateEnvironmentAccountConnectionInputRequestTypeDef definition

class CreateEnvironmentAccountConnectionInputRequestTypeDef(TypedDict):
    environmentName: str,
    managementAccountId: str,
    clientToken: NotRequired[str],
    codebuildRoleArn: NotRequired[str],
    componentRoleArn: NotRequired[str],
    roleArn: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEnvironmentTemplateInputRequestTypeDef

```python
# CreateEnvironmentTemplateInputRequestTypeDef definition

class CreateEnvironmentTemplateInputRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    displayName: NotRequired[str],
    encryptionKey: NotRequired[str],
    provisioning: NotRequired[ProvisioningType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateRepositoryInputRequestTypeDef

```python
# CreateRepositoryInputRequestTypeDef definition

class CreateRepositoryInputRequestTypeDef(TypedDict):
    connectionArn: str,
    name: str,
    provider: RepositoryProviderType,  # (1)
    encryptionKey: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateServiceInputRequestTypeDef

```python
# CreateServiceInputRequestTypeDef definition

class CreateServiceInputRequestTypeDef(TypedDict):
    name: str,
    spec: str,
    templateMajorVersion: str,
    templateName: str,
    branchName: NotRequired[str],
    description: NotRequired[str],
    repositoryConnectionArn: NotRequired[str],
    repositoryId: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    templateMinorVersion: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateServiceInstanceInputRequestTypeDef

```python
# CreateServiceInstanceInputRequestTypeDef definition

class CreateServiceInstanceInputRequestTypeDef(TypedDict):
    name: str,
    serviceName: str,
    spec: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    templateMajorVersion: NotRequired[str],
    templateMinorVersion: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateServiceTemplateInputRequestTypeDef

```python
# CreateServiceTemplateInputRequestTypeDef definition

class CreateServiceTemplateInputRequestTypeDef(TypedDict):
    name: str,
    description: NotRequired[str],
    displayName: NotRequired[str],
    encryptionKey: NotRequired[str],
    pipelineProvisioning: NotRequired[ProvisioningType],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: ProvisioningType](./literals.md#provisioningtype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    nextToken: str,
    tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEnvironmentInputRequestTypeDef

```python
# CreateEnvironmentInputRequestTypeDef definition

class CreateEnvironmentInputRequestTypeDef(TypedDict):
    name: str,
    spec: str,
    templateMajorVersion: str,
    templateName: str,
    codebuildRoleArn: NotRequired[str],
    componentRoleArn: NotRequired[str],
    description: NotRequired[str],
    environmentAccountConnectionId: NotRequired[str],
    protonServiceRoleArn: NotRequired[str],
    provisioningRepository: NotRequired[RepositoryBranchInputTypeDef],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    templateMinorVersion: NotRequired[str],
```

1. See [:material-code-braces: RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateAccountSettingsInputRequestTypeDef

```python
# UpdateAccountSettingsInputRequestTypeDef definition

class UpdateAccountSettingsInputRequestTypeDef(TypedDict):
    deletePipelineProvisioningRepository: NotRequired[bool],
    pipelineCodebuildRoleArn: NotRequired[str],
    pipelineProvisioningRepository: NotRequired[RepositoryBranchInputTypeDef],  # (1)
    pipelineServiceRoleArn: NotRequired[str],
```

1. See [:material-code-braces: RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef) 
## UpdateEnvironmentInputRequestTypeDef

```python
# UpdateEnvironmentInputRequestTypeDef definition

class UpdateEnvironmentInputRequestTypeDef(TypedDict):
    deploymentType: DeploymentUpdateTypeType,  # (1)
    name: str,
    codebuildRoleArn: NotRequired[str],
    componentRoleArn: NotRequired[str],
    description: NotRequired[str],
    environmentAccountConnectionId: NotRequired[str],
    protonServiceRoleArn: NotRequired[str],
    provisioningRepository: NotRequired[RepositoryBranchInputTypeDef],  # (2)
    spec: NotRequired[str],
    templateMajorVersion: NotRequired[str],
    templateMinorVersion: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentUpdateTypeType](./literals.md#deploymentupdatetypetype) 
2. See [:material-code-braces: RepositoryBranchInputTypeDef](./type_defs.md#repositorybranchinputtypedef) 
## CreateEnvironmentTemplateOutputTypeDef

```python
# CreateEnvironmentTemplateOutputTypeDef definition

class CreateEnvironmentTemplateOutputTypeDef(TypedDict):
    environmentTemplate: EnvironmentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateTypeDef](./type_defs.md#environmenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEnvironmentTemplateOutputTypeDef

```python
# DeleteEnvironmentTemplateOutputTypeDef definition

class DeleteEnvironmentTemplateOutputTypeDef(TypedDict):
    environmentTemplate: EnvironmentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateTypeDef](./type_defs.md#environmenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentTemplateOutputTypeDef

```python
# GetEnvironmentTemplateOutputTypeDef definition

class GetEnvironmentTemplateOutputTypeDef(TypedDict):
    environmentTemplate: EnvironmentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateTypeDef](./type_defs.md#environmenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentTemplateOutputTypeDef

```python
# UpdateEnvironmentTemplateOutputTypeDef definition

class UpdateEnvironmentTemplateOutputTypeDef(TypedDict):
    environmentTemplate: EnvironmentTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateTypeDef](./type_defs.md#environmenttemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentTemplateVersionOutputTypeDef

```python
# CreateEnvironmentTemplateVersionOutputTypeDef definition

class CreateEnvironmentTemplateVersionOutputTypeDef(TypedDict):
    environmentTemplateVersion: EnvironmentTemplateVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateVersionTypeDef](./type_defs.md#environmenttemplateversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEnvironmentTemplateVersionOutputTypeDef

```python
# DeleteEnvironmentTemplateVersionOutputTypeDef definition

class DeleteEnvironmentTemplateVersionOutputTypeDef(TypedDict):
    environmentTemplateVersion: EnvironmentTemplateVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateVersionTypeDef](./type_defs.md#environmenttemplateversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentTemplateVersionOutputTypeDef

```python
# GetEnvironmentTemplateVersionOutputTypeDef definition

class GetEnvironmentTemplateVersionOutputTypeDef(TypedDict):
    environmentTemplateVersion: EnvironmentTemplateVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateVersionTypeDef](./type_defs.md#environmenttemplateversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentTemplateVersionOutputTypeDef

```python
# UpdateEnvironmentTemplateVersionOutputTypeDef definition

class UpdateEnvironmentTemplateVersionOutputTypeDef(TypedDict):
    environmentTemplateVersion: EnvironmentTemplateVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateVersionTypeDef](./type_defs.md#environmenttemplateversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRepositoryOutputTypeDef

```python
# CreateRepositoryOutputTypeDef definition

class CreateRepositoryOutputTypeDef(TypedDict):
    repository: RepositoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRepositoryOutputTypeDef

```python
# DeleteRepositoryOutputTypeDef definition

class DeleteRepositoryOutputTypeDef(TypedDict):
    repository: RepositoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRepositoryOutputTypeDef

```python
# GetRepositoryOutputTypeDef definition

class GetRepositoryOutputTypeDef(TypedDict):
    repository: RepositoryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositoryTypeDef](./type_defs.md#repositorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceSyncConfigOutputTypeDef

```python
# CreateServiceSyncConfigOutputTypeDef definition

class CreateServiceSyncConfigOutputTypeDef(TypedDict):
    serviceSyncConfig: ServiceSyncConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSyncConfigTypeDef](./type_defs.md#servicesyncconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceSyncConfigOutputTypeDef

```python
# DeleteServiceSyncConfigOutputTypeDef definition

class DeleteServiceSyncConfigOutputTypeDef(TypedDict):
    serviceSyncConfig: ServiceSyncConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSyncConfigTypeDef](./type_defs.md#servicesyncconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceSyncConfigOutputTypeDef

```python
# GetServiceSyncConfigOutputTypeDef definition

class GetServiceSyncConfigOutputTypeDef(TypedDict):
    serviceSyncConfig: ServiceSyncConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSyncConfigTypeDef](./type_defs.md#servicesyncconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceSyncConfigOutputTypeDef

```python
# UpdateServiceSyncConfigOutputTypeDef definition

class UpdateServiceSyncConfigOutputTypeDef(TypedDict):
    serviceSyncConfig: ServiceSyncConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSyncConfigTypeDef](./type_defs.md#servicesyncconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceTemplateOutputTypeDef

```python
# CreateServiceTemplateOutputTypeDef definition

class CreateServiceTemplateOutputTypeDef(TypedDict):
    serviceTemplate: ServiceTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateTypeDef](./type_defs.md#servicetemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceTemplateOutputTypeDef

```python
# DeleteServiceTemplateOutputTypeDef definition

class DeleteServiceTemplateOutputTypeDef(TypedDict):
    serviceTemplate: ServiceTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateTypeDef](./type_defs.md#servicetemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceTemplateOutputTypeDef

```python
# GetServiceTemplateOutputTypeDef definition

class GetServiceTemplateOutputTypeDef(TypedDict):
    serviceTemplate: ServiceTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateTypeDef](./type_defs.md#servicetemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceTemplateOutputTypeDef

```python
# UpdateServiceTemplateOutputTypeDef definition

class UpdateServiceTemplateOutputTypeDef(TypedDict):
    serviceTemplate: ServiceTemplateTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateTypeDef](./type_defs.md#servicetemplatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTemplateSyncConfigOutputTypeDef

```python
# CreateTemplateSyncConfigOutputTypeDef definition

class CreateTemplateSyncConfigOutputTypeDef(TypedDict):
    templateSyncConfig: TemplateSyncConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateSyncConfigTypeDef](./type_defs.md#templatesyncconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTemplateSyncConfigOutputTypeDef

```python
# DeleteTemplateSyncConfigOutputTypeDef definition

class DeleteTemplateSyncConfigOutputTypeDef(TypedDict):
    templateSyncConfig: TemplateSyncConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateSyncConfigTypeDef](./type_defs.md#templatesyncconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTemplateSyncConfigOutputTypeDef

```python
# GetTemplateSyncConfigOutputTypeDef definition

class GetTemplateSyncConfigOutputTypeDef(TypedDict):
    templateSyncConfig: TemplateSyncConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateSyncConfigTypeDef](./type_defs.md#templatesyncconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTemplateSyncConfigOutputTypeDef

```python
# UpdateTemplateSyncConfigOutputTypeDef definition

class UpdateTemplateSyncConfigOutputTypeDef(TypedDict):
    templateSyncConfig: TemplateSyncConfigTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TemplateSyncConfigTypeDef](./type_defs.md#templatesyncconfigtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentStateTypeDef

```python
# DeploymentStateTypeDef definition

class DeploymentStateTypeDef(TypedDict):
    component: NotRequired[ComponentStateTypeDef],  # (1)
    environment: NotRequired[EnvironmentStateTypeDef],  # (2)
    serviceInstance: NotRequired[ServiceInstanceStateTypeDef],  # (3)
    servicePipeline: NotRequired[ServicePipelineStateTypeDef],  # (4)
```

1. See [:material-code-braces: ComponentStateTypeDef](./type_defs.md#componentstatetypedef) 
2. See [:material-code-braces: EnvironmentStateTypeDef](./type_defs.md#environmentstatetypedef) 
3. See [:material-code-braces: ServiceInstanceStateTypeDef](./type_defs.md#serviceinstancestatetypedef) 
4. See [:material-code-braces: ServicePipelineStateTypeDef](./type_defs.md#servicepipelinestatetypedef) 
## ListDeploymentsOutputTypeDef

```python
# ListDeploymentsOutputTypeDef definition

class ListDeploymentsOutputTypeDef(TypedDict):
    deployments: List[DeploymentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentSummaryTypeDef](./type_defs.md#deploymentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentAccountConnectionsOutputTypeDef

```python
# ListEnvironmentAccountConnectionsOutputTypeDef definition

class ListEnvironmentAccountConnectionsOutputTypeDef(TypedDict):
    environmentAccountConnections: List[EnvironmentAccountConnectionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentAccountConnectionSummaryTypeDef](./type_defs.md#environmentaccountconnectionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsOutputTypeDef

```python
# ListEnvironmentsOutputTypeDef definition

class ListEnvironmentsOutputTypeDef(TypedDict):
    environments: List[EnvironmentSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsInputRequestTypeDef

```python
# ListEnvironmentsInputRequestTypeDef definition

class ListEnvironmentsInputRequestTypeDef(TypedDict):
    environmentTemplates: NotRequired[Sequence[EnvironmentTemplateFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentTemplateFilterTypeDef](./type_defs.md#environmenttemplatefiltertypedef) 
## ListEnvironmentTemplatesOutputTypeDef

```python
# ListEnvironmentTemplatesOutputTypeDef definition

class ListEnvironmentTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    templates: List[EnvironmentTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateSummaryTypeDef](./type_defs.md#environmenttemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentTemplateVersionsOutputTypeDef

```python
# ListEnvironmentTemplateVersionsOutputTypeDef definition

class ListEnvironmentTemplateVersionsOutputTypeDef(TypedDict):
    nextToken: str,
    templateVersions: List[EnvironmentTemplateVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateVersionSummaryTypeDef](./type_defs.md#environmenttemplateversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComponentInputComponentDeletedWaitTypeDef

```python
# GetComponentInputComponentDeletedWaitTypeDef definition

class GetComponentInputComponentDeletedWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetComponentInputComponentDeployedWaitTypeDef

```python
# GetComponentInputComponentDeployedWaitTypeDef definition

class GetComponentInputComponentDeployedWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetEnvironmentInputEnvironmentDeployedWaitTypeDef

```python
# GetEnvironmentInputEnvironmentDeployedWaitTypeDef definition

class GetEnvironmentInputEnvironmentDeployedWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef

```python
# GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef definition

class GetEnvironmentTemplateVersionInputEnvironmentTemplateVersionRegisteredWaitTypeDef(TypedDict):
    majorVersion: str,
    minorVersion: str,
    templateName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetServiceInputServiceCreatedWaitTypeDef

```python
# GetServiceInputServiceCreatedWaitTypeDef definition

class GetServiceInputServiceCreatedWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetServiceInputServiceDeletedWaitTypeDef

```python
# GetServiceInputServiceDeletedWaitTypeDef definition

class GetServiceInputServiceDeletedWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetServiceInputServicePipelineDeployedWaitTypeDef

```python
# GetServiceInputServicePipelineDeployedWaitTypeDef definition

class GetServiceInputServicePipelineDeployedWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetServiceInputServiceUpdatedWaitTypeDef

```python
# GetServiceInputServiceUpdatedWaitTypeDef definition

class GetServiceInputServiceUpdatedWaitTypeDef(TypedDict):
    name: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef

```python
# GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef definition

class GetServiceInstanceInputServiceInstanceDeployedWaitTypeDef(TypedDict):
    name: str,
    serviceName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef

```python
# GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef definition

class GetServiceTemplateVersionInputServiceTemplateVersionRegisteredWaitTypeDef(TypedDict):
    majorVersion: str,
    minorVersion: str,
    templateName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## ListComponentOutputsInputListComponentOutputsPaginateTypeDef

```python
# ListComponentOutputsInputListComponentOutputsPaginateTypeDef definition

class ListComponentOutputsInputListComponentOutputsPaginateTypeDef(TypedDict):
    componentName: str,
    deploymentId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef

```python
# ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef definition

class ListComponentProvisionedResourcesInputListComponentProvisionedResourcesPaginateTypeDef(TypedDict):
    componentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComponentsInputListComponentsPaginateTypeDef

```python
# ListComponentsInputListComponentsPaginateTypeDef definition

class ListComponentsInputListComponentsPaginateTypeDef(TypedDict):
    environmentName: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentsInputListDeploymentsPaginateTypeDef

```python
# ListDeploymentsInputListDeploymentsPaginateTypeDef definition

class ListDeploymentsInputListDeploymentsPaginateTypeDef(TypedDict):
    componentName: NotRequired[str],
    environmentName: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef

```python
# ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef definition

class ListEnvironmentAccountConnectionsInputListEnvironmentAccountConnectionsPaginateTypeDef(TypedDict):
    requestedBy: EnvironmentAccountConnectionRequesterAccountTypeType,  # (1)
    environmentName: NotRequired[str],
    statuses: NotRequired[Sequence[EnvironmentAccountConnectionStatusType]],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EnvironmentAccountConnectionRequesterAccountTypeType](./literals.md#environmentaccountconnectionrequesteraccounttypetype) 
2. See [:material-code-brackets: EnvironmentAccountConnectionStatusType](./literals.md#environmentaccountconnectionstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef

```python
# ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef definition

class ListEnvironmentOutputsInputListEnvironmentOutputsPaginateTypeDef(TypedDict):
    environmentName: str,
    deploymentId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef

```python
# ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef definition

class ListEnvironmentProvisionedResourcesInputListEnvironmentProvisionedResourcesPaginateTypeDef(TypedDict):
    environmentName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef

```python
# ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef definition

class ListEnvironmentTemplateVersionsInputListEnvironmentTemplateVersionsPaginateTypeDef(TypedDict):
    templateName: str,
    majorVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef

```python
# ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef definition

class ListEnvironmentTemplatesInputListEnvironmentTemplatesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsInputListEnvironmentsPaginateTypeDef

```python
# ListEnvironmentsInputListEnvironmentsPaginateTypeDef definition

class ListEnvironmentsInputListEnvironmentsPaginateTypeDef(TypedDict):
    environmentTemplates: NotRequired[Sequence[EnvironmentTemplateFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: EnvironmentTemplateFilterTypeDef](./type_defs.md#environmenttemplatefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRepositoriesInputListRepositoriesPaginateTypeDef

```python
# ListRepositoriesInputListRepositoriesPaginateTypeDef definition

class ListRepositoriesInputListRepositoriesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef

```python
# ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef definition

class ListRepositorySyncDefinitionsInputListRepositorySyncDefinitionsPaginateTypeDef(TypedDict):
    repositoryName: str,
    repositoryProvider: RepositoryProviderType,  # (1)
    syncType: SyncTypeType,  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RepositoryProviderType](./literals.md#repositoryprovidertype) 
2. See [:material-code-brackets: SyncTypeType](./literals.md#synctypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef

```python
# ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef definition

class ListServiceInstanceOutputsInputListServiceInstanceOutputsPaginateTypeDef(TypedDict):
    serviceInstanceName: str,
    serviceName: str,
    deploymentId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef

```python
# ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef definition

class ListServiceInstanceProvisionedResourcesInputListServiceInstanceProvisionedResourcesPaginateTypeDef(TypedDict):
    serviceInstanceName: str,
    serviceName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef

```python
# ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef definition

class ListServicePipelineOutputsInputListServicePipelineOutputsPaginateTypeDef(TypedDict):
    serviceName: str,
    deploymentId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef

```python
# ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef definition

class ListServicePipelineProvisionedResourcesInputListServicePipelineProvisionedResourcesPaginateTypeDef(TypedDict):
    serviceName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef

```python
# ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef definition

class ListServiceTemplateVersionsInputListServiceTemplateVersionsPaginateTypeDef(TypedDict):
    templateName: str,
    majorVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef

```python
# ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef definition

class ListServiceTemplatesInputListServiceTemplatesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServicesInputListServicesPaginateTypeDef

```python
# ListServicesInputListServicesPaginateTypeDef definition

class ListServicesInputListServicesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceInputListTagsForResourcePaginateTypeDef

```python
# ListTagsForResourceInputListTagsForResourcePaginateTypeDef definition

class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(TypedDict):
    resourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListComponentOutputsOutputTypeDef

```python
# ListComponentOutputsOutputTypeDef definition

class ListComponentOutputsOutputTypeDef(TypedDict):
    nextToken: str,
    outputs: List[OutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentOutputsOutputTypeDef

```python
# ListEnvironmentOutputsOutputTypeDef definition

class ListEnvironmentOutputsOutputTypeDef(TypedDict):
    nextToken: str,
    outputs: List[OutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceInstanceOutputsOutputTypeDef

```python
# ListServiceInstanceOutputsOutputTypeDef definition

class ListServiceInstanceOutputsOutputTypeDef(TypedDict):
    nextToken: str,
    outputs: List[OutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicePipelineOutputsOutputTypeDef

```python
# ListServicePipelineOutputsOutputTypeDef definition

class ListServicePipelineOutputsOutputTypeDef(TypedDict):
    nextToken: str,
    outputs: List[OutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotifyResourceDeploymentStatusChangeInputRequestTypeDef

```python
# NotifyResourceDeploymentStatusChangeInputRequestTypeDef definition

class NotifyResourceDeploymentStatusChangeInputRequestTypeDef(TypedDict):
    resourceArn: str,
    deploymentId: NotRequired[str],
    outputs: NotRequired[Sequence[OutputTypeDef]],  # (1)
    status: NotRequired[ResourceDeploymentStatusType],  # (2)
    statusMessage: NotRequired[str],
```

1. See [:material-code-braces: OutputTypeDef](./type_defs.md#outputtypedef) 
2. See [:material-code-brackets: ResourceDeploymentStatusType](./literals.md#resourcedeploymentstatustype) 
## ListComponentProvisionedResourcesOutputTypeDef

```python
# ListComponentProvisionedResourcesOutputTypeDef definition

class ListComponentProvisionedResourcesOutputTypeDef(TypedDict):
    nextToken: str,
    provisionedResources: List[ProvisionedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedResourceTypeDef](./type_defs.md#provisionedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentProvisionedResourcesOutputTypeDef

```python
# ListEnvironmentProvisionedResourcesOutputTypeDef definition

class ListEnvironmentProvisionedResourcesOutputTypeDef(TypedDict):
    nextToken: str,
    provisionedResources: List[ProvisionedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedResourceTypeDef](./type_defs.md#provisionedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceInstanceProvisionedResourcesOutputTypeDef

```python
# ListServiceInstanceProvisionedResourcesOutputTypeDef definition

class ListServiceInstanceProvisionedResourcesOutputTypeDef(TypedDict):
    nextToken: str,
    provisionedResources: List[ProvisionedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedResourceTypeDef](./type_defs.md#provisionedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicePipelineProvisionedResourcesOutputTypeDef

```python
# ListServicePipelineProvisionedResourcesOutputTypeDef definition

class ListServicePipelineProvisionedResourcesOutputTypeDef(TypedDict):
    nextToken: str,
    provisionedResources: List[ProvisionedResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedResourceTypeDef](./type_defs.md#provisionedresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRepositoriesOutputTypeDef

```python
# ListRepositoriesOutputTypeDef definition

class ListRepositoriesOutputTypeDef(TypedDict):
    nextToken: str,
    repositories: List[RepositorySummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositorySummaryTypeDef](./type_defs.md#repositorysummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRepositorySyncDefinitionsOutputTypeDef

```python
# ListRepositorySyncDefinitionsOutputTypeDef definition

class ListRepositorySyncDefinitionsOutputTypeDef(TypedDict):
    nextToken: str,
    syncDefinitions: List[RepositorySyncDefinitionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositorySyncDefinitionTypeDef](./type_defs.md#repositorysyncdefinitiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceInstancesInputListServiceInstancesPaginateTypeDef

```python
# ListServiceInstancesInputListServiceInstancesPaginateTypeDef definition

class ListServiceInstancesInputListServiceInstancesPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[ListServiceInstancesFilterTypeDef]],  # (1)
    serviceName: NotRequired[str],
    sortBy: NotRequired[ListServiceInstancesSortByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-braces: ListServiceInstancesFilterTypeDef](./type_defs.md#listserviceinstancesfiltertypedef) 
2. See [:material-code-brackets: ListServiceInstancesSortByType](./literals.md#listserviceinstancessortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceInstancesInputRequestTypeDef

```python
# ListServiceInstancesInputRequestTypeDef definition

class ListServiceInstancesInputRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[ListServiceInstancesFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    serviceName: NotRequired[str],
    sortBy: NotRequired[ListServiceInstancesSortByType],  # (2)
    sortOrder: NotRequired[SortOrderType],  # (3)
```

1. See [:material-code-braces: ListServiceInstancesFilterTypeDef](./type_defs.md#listserviceinstancesfiltertypedef) 
2. See [:material-code-brackets: ListServiceInstancesSortByType](./literals.md#listserviceinstancessortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListServiceInstancesOutputTypeDef

```python
# ListServiceInstancesOutputTypeDef definition

class ListServiceInstancesOutputTypeDef(TypedDict):
    nextToken: str,
    serviceInstances: List[ServiceInstanceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceInstanceSummaryTypeDef](./type_defs.md#serviceinstancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceTemplateVersionsOutputTypeDef

```python
# ListServiceTemplateVersionsOutputTypeDef definition

class ListServiceTemplateVersionsOutputTypeDef(TypedDict):
    nextToken: str,
    templateVersions: List[ServiceTemplateVersionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateVersionSummaryTypeDef](./type_defs.md#servicetemplateversionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceTemplatesOutputTypeDef

```python
# ListServiceTemplatesOutputTypeDef definition

class ListServiceTemplatesOutputTypeDef(TypedDict):
    nextToken: str,
    templates: List[ServiceTemplateSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateSummaryTypeDef](./type_defs.md#servicetemplatesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServicesOutputTypeDef

```python
# ListServicesOutputTypeDef definition

class ListServicesOutputTypeDef(TypedDict):
    nextToken: str,
    services: List[ServiceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSummaryTypeDef](./type_defs.md#servicesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RepositorySyncAttemptTypeDef

```python
# RepositorySyncAttemptTypeDef definition

class RepositorySyncAttemptTypeDef(TypedDict):
    events: List[RepositorySyncEventTypeDef],  # (1)
    startedAt: datetime,
    status: RepositorySyncStatusType,  # (2)
```

1. See [:material-code-braces: RepositorySyncEventTypeDef](./type_defs.md#repositorysynceventtypedef) 
2. See [:material-code-brackets: RepositorySyncStatusType](./literals.md#repositorysyncstatustype) 
## ResourceSyncAttemptTypeDef

```python
# ResourceSyncAttemptTypeDef definition

class ResourceSyncAttemptTypeDef(TypedDict):
    events: List[ResourceSyncEventTypeDef],  # (1)
    initialRevision: RevisionTypeDef,  # (2)
    startedAt: datetime,
    status: ResourceSyncStatusType,  # (3)
    target: str,
    targetRevision: RevisionTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSyncEventTypeDef](./type_defs.md#resourcesynceventtypedef) 
2. See [:material-code-braces: RevisionTypeDef](./type_defs.md#revisiontypedef) 
3. See [:material-code-brackets: ResourceSyncStatusType](./literals.md#resourcesyncstatustype) 
4. See [:material-code-braces: RevisionTypeDef](./type_defs.md#revisiontypedef) 
## TemplateVersionSourceInputTypeDef

```python
# TemplateVersionSourceInputTypeDef definition

class TemplateVersionSourceInputTypeDef(TypedDict):
    s3: NotRequired[S3ObjectSourceTypeDef],  # (1)
```

1. See [:material-code-braces: S3ObjectSourceTypeDef](./type_defs.md#s3objectsourcetypedef) 
## SyncBlockerTypeDef

```python
# SyncBlockerTypeDef definition

class SyncBlockerTypeDef(TypedDict):
    createdAt: datetime,
    createdReason: str,
    id: str,
    status: BlockerStatusType,  # (2)
    type: BlockerTypeType,  # (3)
    contexts: NotRequired[List[SyncBlockerContextTypeDef]],  # (1)
    resolvedAt: NotRequired[datetime],
    resolvedReason: NotRequired[str],
```

1. See [:material-code-braces: SyncBlockerContextTypeDef](./type_defs.md#syncblockercontexttypedef) 
2. See [:material-code-brackets: BlockerStatusType](./literals.md#blockerstatustype) 
3. See [:material-code-brackets: BlockerTypeType](./literals.md#blockertypetype) 
## GetAccountSettingsOutputTypeDef

```python
# GetAccountSettingsOutputTypeDef definition

class GetAccountSettingsOutputTypeDef(TypedDict):
    accountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAccountSettingsOutputTypeDef

```python
# UpdateAccountSettingsOutputTypeDef definition

class UpdateAccountSettingsOutputTypeDef(TypedDict):
    accountSettings: AccountSettingsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AccountSettingsTypeDef](./type_defs.md#accountsettingstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelEnvironmentDeploymentOutputTypeDef

```python
# CancelEnvironmentDeploymentOutputTypeDef definition

class CancelEnvironmentDeploymentOutputTypeDef(TypedDict):
    environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentOutputTypeDef

```python
# CreateEnvironmentOutputTypeDef definition

class CreateEnvironmentOutputTypeDef(TypedDict):
    environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteEnvironmentOutputTypeDef

```python
# DeleteEnvironmentOutputTypeDef definition

class DeleteEnvironmentOutputTypeDef(TypedDict):
    environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentOutputTypeDef

```python
# GetEnvironmentOutputTypeDef definition

class GetEnvironmentOutputTypeDef(TypedDict):
    environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentOutputTypeDef

```python
# UpdateEnvironmentOutputTypeDef definition

class UpdateEnvironmentOutputTypeDef(TypedDict):
    environment: EnvironmentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceOutputTypeDef

```python
# CreateServiceOutputTypeDef definition

class CreateServiceOutputTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceOutputTypeDef

```python
# DeleteServiceOutputTypeDef definition

class DeleteServiceOutputTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceOutputTypeDef

```python
# GetServiceOutputTypeDef definition

class GetServiceOutputTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceOutputTypeDef

```python
# UpdateServiceOutputTypeDef definition

class UpdateServiceOutputTypeDef(TypedDict):
    service: ServiceTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTypeDef](./type_defs.md#servicetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateServiceTemplateVersionOutputTypeDef

```python
# CreateServiceTemplateVersionOutputTypeDef definition

class CreateServiceTemplateVersionOutputTypeDef(TypedDict):
    serviceTemplateVersion: ServiceTemplateVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateVersionTypeDef](./type_defs.md#servicetemplateversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteServiceTemplateVersionOutputTypeDef

```python
# DeleteServiceTemplateVersionOutputTypeDef definition

class DeleteServiceTemplateVersionOutputTypeDef(TypedDict):
    serviceTemplateVersion: ServiceTemplateVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateVersionTypeDef](./type_defs.md#servicetemplateversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceTemplateVersionOutputTypeDef

```python
# GetServiceTemplateVersionOutputTypeDef definition

class GetServiceTemplateVersionOutputTypeDef(TypedDict):
    serviceTemplateVersion: ServiceTemplateVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateVersionTypeDef](./type_defs.md#servicetemplateversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceTemplateVersionOutputTypeDef

```python
# UpdateServiceTemplateVersionOutputTypeDef definition

class UpdateServiceTemplateVersionOutputTypeDef(TypedDict):
    serviceTemplateVersion: ServiceTemplateVersionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceTemplateVersionTypeDef](./type_defs.md#servicetemplateversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcesSummaryOutputTypeDef

```python
# GetResourcesSummaryOutputTypeDef definition

class GetResourcesSummaryOutputTypeDef(TypedDict):
    counts: CountsSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CountsSummaryTypeDef](./type_defs.md#countssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentTypeDef

```python
# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    deploymentStatus: DeploymentStatusType,  # (1)
    environmentName: str,
    id: str,
    lastModifiedAt: datetime,
    targetArn: str,
    targetResourceCreatedAt: datetime,
    targetResourceType: DeploymentTargetResourceTypeType,  # (3)
    completedAt: NotRequired[datetime],
    componentName: NotRequired[str],
    deploymentStatusMessage: NotRequired[str],
    initialState: NotRequired[DeploymentStateTypeDef],  # (2)
    lastAttemptedDeploymentId: NotRequired[str],
    lastSucceededDeploymentId: NotRequired[str],
    serviceInstanceName: NotRequired[str],
    serviceName: NotRequired[str],
    targetState: NotRequired[DeploymentStateTypeDef],  # (2)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: DeploymentStateTypeDef](./type_defs.md#deploymentstatetypedef) 
3. See [:material-code-brackets: DeploymentTargetResourceTypeType](./literals.md#deploymenttargetresourcetypetype) 
4. See [:material-code-braces: DeploymentStateTypeDef](./type_defs.md#deploymentstatetypedef) 
## GetRepositorySyncStatusOutputTypeDef

```python
# GetRepositorySyncStatusOutputTypeDef definition

class GetRepositorySyncStatusOutputTypeDef(TypedDict):
    latestSync: RepositorySyncAttemptTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RepositorySyncAttemptTypeDef](./type_defs.md#repositorysyncattempttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceInstanceSyncStatusOutputTypeDef

```python
# GetServiceInstanceSyncStatusOutputTypeDef definition

class GetServiceInstanceSyncStatusOutputTypeDef(TypedDict):
    desiredState: RevisionTypeDef,  # (1)
    latestSuccessfulSync: ResourceSyncAttemptTypeDef,  # (2)
    latestSync: ResourceSyncAttemptTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: RevisionTypeDef](./type_defs.md#revisiontypedef) 
2. See [:material-code-braces: ResourceSyncAttemptTypeDef](./type_defs.md#resourcesyncattempttypedef) 
3. See [:material-code-braces: ResourceSyncAttemptTypeDef](./type_defs.md#resourcesyncattempttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTemplateSyncStatusOutputTypeDef

```python
# GetTemplateSyncStatusOutputTypeDef definition

class GetTemplateSyncStatusOutputTypeDef(TypedDict):
    desiredState: RevisionTypeDef,  # (1)
    latestSuccessfulSync: ResourceSyncAttemptTypeDef,  # (2)
    latestSync: ResourceSyncAttemptTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: RevisionTypeDef](./type_defs.md#revisiontypedef) 
2. See [:material-code-braces: ResourceSyncAttemptTypeDef](./type_defs.md#resourcesyncattempttypedef) 
3. See [:material-code-braces: ResourceSyncAttemptTypeDef](./type_defs.md#resourcesyncattempttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentTemplateVersionInputRequestTypeDef

```python
# CreateEnvironmentTemplateVersionInputRequestTypeDef definition

class CreateEnvironmentTemplateVersionInputRequestTypeDef(TypedDict):
    source: TemplateVersionSourceInputTypeDef,  # (1)
    templateName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    majorVersion: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: TemplateVersionSourceInputTypeDef](./type_defs.md#templateversionsourceinputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateServiceTemplateVersionInputRequestTypeDef

```python
# CreateServiceTemplateVersionInputRequestTypeDef definition

class CreateServiceTemplateVersionInputRequestTypeDef(TypedDict):
    compatibleEnvironmentTemplates: Sequence[CompatibleEnvironmentTemplateInputTypeDef],  # (1)
    source: TemplateVersionSourceInputTypeDef,  # (2)
    templateName: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    majorVersion: NotRequired[str],
    supportedComponentSources: NotRequired[Sequence[ServiceTemplateSupportedComponentSourceTypeType]],  # (3)
    tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-braces: CompatibleEnvironmentTemplateInputTypeDef](./type_defs.md#compatibleenvironmenttemplateinputtypedef) 
2. See [:material-code-braces: TemplateVersionSourceInputTypeDef](./type_defs.md#templateversionsourceinputtypedef) 
3. See [:material-code-brackets: ServiceTemplateSupportedComponentSourceTypeType](./literals.md#servicetemplatesupportedcomponentsourcetypetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ServiceSyncBlockerSummaryTypeDef

```python
# ServiceSyncBlockerSummaryTypeDef definition

class ServiceSyncBlockerSummaryTypeDef(TypedDict):
    serviceName: str,
    latestBlockers: NotRequired[List[SyncBlockerTypeDef]],  # (1)
    serviceInstanceName: NotRequired[str],
```

1. See [:material-code-braces: SyncBlockerTypeDef](./type_defs.md#syncblockertypedef) 
## UpdateServiceSyncBlockerOutputTypeDef

```python
# UpdateServiceSyncBlockerOutputTypeDef definition

class UpdateServiceSyncBlockerOutputTypeDef(TypedDict):
    serviceInstanceName: str,
    serviceName: str,
    serviceSyncBlocker: SyncBlockerTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SyncBlockerTypeDef](./type_defs.md#syncblockertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDeploymentOutputTypeDef

```python
# DeleteDeploymentOutputTypeDef definition

class DeleteDeploymentOutputTypeDef(TypedDict):
    deployment: DeploymentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentOutputTypeDef

```python
# GetDeploymentOutputTypeDef definition

class GetDeploymentOutputTypeDef(TypedDict):
    deployment: DeploymentTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetServiceSyncBlockerSummaryOutputTypeDef

```python
# GetServiceSyncBlockerSummaryOutputTypeDef definition

class GetServiceSyncBlockerSummaryOutputTypeDef(TypedDict):
    serviceSyncBlockerSummary: ServiceSyncBlockerSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceSyncBlockerSummaryTypeDef](./type_defs.md#servicesyncblockersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

# Type definitions

> [Index](../README.md) > [SMS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#SMS)
    type annotations stubs module [types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ServerReplicationParametersUnionTypeDef

```python
# ServerReplicationParametersUnionTypeDef definition

ServerReplicationParametersUnionTypeDef = Union[
    ServerReplicationParametersTypeDef,  # (1)
    ServerReplicationParametersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServerReplicationParametersTypeDef](./type_defs.md#serverreplicationparameterstypedef) 
2. See [:material-code-braces: ServerReplicationParametersOutputTypeDef](./type_defs.md#serverreplicationparametersoutputtypedef) 

## ServerGroupUnionTypeDef

```python
# ServerGroupUnionTypeDef definition

ServerGroupUnionTypeDef = Union[
    ServerGroupTypeDef,  # (1)
    ServerGroupOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServerGroupTypeDef](./type_defs.md#servergrouptypedef) 
2. See [:material-code-braces: ServerGroupOutputTypeDef](./type_defs.md#servergroupoutputtypedef) 

## ServerReplicationConfigurationUnionTypeDef

```python
# ServerReplicationConfigurationUnionTypeDef definition

ServerReplicationConfigurationUnionTypeDef = Union[
    ServerReplicationConfigurationTypeDef,  # (1)
    ServerReplicationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServerReplicationConfigurationTypeDef](./type_defs.md#serverreplicationconfigurationtypedef) 
2. See [:material-code-braces: ServerReplicationConfigurationOutputTypeDef](./type_defs.md#serverreplicationconfigurationoutputtypedef) 

## ServerGroupLaunchConfigurationUnionTypeDef

```python
# ServerGroupLaunchConfigurationUnionTypeDef definition

ServerGroupLaunchConfigurationUnionTypeDef = Union[
    ServerGroupLaunchConfigurationTypeDef,  # (1)
    ServerGroupLaunchConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServerGroupLaunchConfigurationTypeDef](./type_defs.md#servergrouplaunchconfigurationtypedef) 
2. See [:material-code-braces: ServerGroupLaunchConfigurationOutputTypeDef](./type_defs.md#servergrouplaunchconfigurationoutputtypedef) 

## ServerGroupValidationConfigurationUnionTypeDef

```python
# ServerGroupValidationConfigurationUnionTypeDef definition

ServerGroupValidationConfigurationUnionTypeDef = Union[
    ServerGroupValidationConfigurationTypeDef,  # (1)
    ServerGroupValidationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServerGroupValidationConfigurationTypeDef](./type_defs.md#servergroupvalidationconfigurationtypedef) 
2. See [:material-code-braces: ServerGroupValidationConfigurationOutputTypeDef](./type_defs.md#servergroupvalidationconfigurationoutputtypedef) 

## ServerGroupReplicationConfigurationUnionTypeDef

```python
# ServerGroupReplicationConfigurationUnionTypeDef definition

ServerGroupReplicationConfigurationUnionTypeDef = Union[
    ServerGroupReplicationConfigurationTypeDef,  # (1)
    ServerGroupReplicationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ServerGroupReplicationConfigurationTypeDef](./type_defs.md#servergroupreplicationconfigurationtypedef) 
2. See [:material-code-braces: ServerGroupReplicationConfigurationOutputTypeDef](./type_defs.md#servergroupreplicationconfigurationoutputtypedef) 



## LaunchDetailsTypeDef

```python
# LaunchDetailsTypeDef definition

class LaunchDetailsTypeDef(TypedDict):
    latestLaunchTime: NotRequired[datetime],
    stackName: NotRequired[str],
    stackId: NotRequired[str],
```

## ConnectorTypeDef

```python
# ConnectorTypeDef definition

class ConnectorTypeDef(TypedDict):
    connectorId: NotRequired[str],
    version: NotRequired[str],
    status: NotRequired[ConnectorStatusType],  # (1)
    capabilityList: NotRequired[List[ConnectorCapabilityType]],  # (2)
    vmManagerName: NotRequired[str],
    vmManagerType: NotRequired[VmManagerTypeType],  # (3)
    vmManagerId: NotRequired[str],
    ipAddress: NotRequired[str],
    macAddress: NotRequired[str],
    associatedOn: NotRequired[datetime],
```

1. See [:material-code-brackets: ConnectorStatusType](./literals.md#connectorstatustype) 
2. See [:material-code-brackets: ConnectorCapabilityType](./literals.md#connectorcapabilitytype) 
3. See [:material-code-brackets: VmManagerTypeType](./literals.md#vmmanagertypetype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
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

## DeleteAppLaunchConfigurationRequestRequestTypeDef

```python
# DeleteAppLaunchConfigurationRequestRequestTypeDef definition

class DeleteAppLaunchConfigurationRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## DeleteAppReplicationConfigurationRequestRequestTypeDef

```python
# DeleteAppReplicationConfigurationRequestRequestTypeDef definition

class DeleteAppReplicationConfigurationRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## DeleteAppRequestRequestTypeDef

```python
# DeleteAppRequestRequestTypeDef definition

class DeleteAppRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    forceStopAppReplication: NotRequired[bool],
    forceTerminateApp: NotRequired[bool],
```

## DeleteAppValidationConfigurationRequestRequestTypeDef

```python
# DeleteAppValidationConfigurationRequestRequestTypeDef definition

class DeleteAppValidationConfigurationRequestRequestTypeDef(TypedDict):
    appId: str,
```

## DeleteReplicationJobRequestRequestTypeDef

```python
# DeleteReplicationJobRequestRequestTypeDef definition

class DeleteReplicationJobRequestRequestTypeDef(TypedDict):
    replicationJobId: str,
```

## DisassociateConnectorRequestRequestTypeDef

```python
# DisassociateConnectorRequestRequestTypeDef definition

class DisassociateConnectorRequestRequestTypeDef(TypedDict):
    connectorId: str,
```

## GenerateChangeSetRequestRequestTypeDef

```python
# GenerateChangeSetRequestRequestTypeDef definition

class GenerateChangeSetRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    changesetFormat: NotRequired[OutputFormatType],  # (1)
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## S3LocationTypeDef

```python
# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
```

## GenerateTemplateRequestRequestTypeDef

```python
# GenerateTemplateRequestRequestTypeDef definition

class GenerateTemplateRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    templateFormat: NotRequired[OutputFormatType],  # (1)
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## GetAppLaunchConfigurationRequestRequestTypeDef

```python
# GetAppLaunchConfigurationRequestRequestTypeDef definition

class GetAppLaunchConfigurationRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## GetAppReplicationConfigurationRequestRequestTypeDef

```python
# GetAppReplicationConfigurationRequestRequestTypeDef definition

class GetAppReplicationConfigurationRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## GetAppRequestRequestTypeDef

```python
# GetAppRequestRequestTypeDef definition

class GetAppRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## GetAppValidationConfigurationRequestRequestTypeDef

```python
# GetAppValidationConfigurationRequestRequestTypeDef definition

class GetAppValidationConfigurationRequestRequestTypeDef(TypedDict):
    appId: str,
```

## GetAppValidationOutputRequestRequestTypeDef

```python
# GetAppValidationOutputRequestRequestTypeDef definition

class GetAppValidationOutputRequestRequestTypeDef(TypedDict):
    appId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetConnectorsRequestRequestTypeDef

```python
# GetConnectorsRequestRequestTypeDef definition

class GetConnectorsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetReplicationJobsRequestRequestTypeDef

```python
# GetReplicationJobsRequestRequestTypeDef definition

class GetReplicationJobsRequestRequestTypeDef(TypedDict):
    replicationJobId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetReplicationRunsRequestRequestTypeDef

```python
# GetReplicationRunsRequestRequestTypeDef definition

class GetReplicationRunsRequestRequestTypeDef(TypedDict):
    replicationJobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## VmServerAddressTypeDef

```python
# VmServerAddressTypeDef definition

class VmServerAddressTypeDef(TypedDict):
    vmManagerId: NotRequired[str],
    vmId: NotRequired[str],
```

## ImportAppCatalogRequestRequestTypeDef

```python
# ImportAppCatalogRequestRequestTypeDef definition

class ImportAppCatalogRequestRequestTypeDef(TypedDict):
    roleName: NotRequired[str],
```

## LaunchAppRequestRequestTypeDef

```python
# LaunchAppRequestRequestTypeDef definition

class LaunchAppRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## ListAppsRequestRequestTypeDef

```python
# ListAppsRequestRequestTypeDef definition

class ListAppsRequestRequestTypeDef(TypedDict):
    appIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## NotificationContextTypeDef

```python
# NotificationContextTypeDef definition

class NotificationContextTypeDef(TypedDict):
    validationId: NotRequired[str],
    status: NotRequired[ValidationStatusType],  # (1)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ValidationStatusType](./literals.md#validationstatustype) 
## ReplicationRunStageDetailsTypeDef

```python
# ReplicationRunStageDetailsTypeDef definition

class ReplicationRunStageDetailsTypeDef(TypedDict):
    stage: NotRequired[str],
    stageProgress: NotRequired[str],
```

## ServerReplicationParametersOutputTypeDef

```python
# ServerReplicationParametersOutputTypeDef definition

class ServerReplicationParametersOutputTypeDef(TypedDict):
    seedTime: NotRequired[datetime],
    frequency: NotRequired[int],
    runOnce: NotRequired[bool],
    licenseType: NotRequired[LicenseTypeType],  # (1)
    numberOfRecentAmisToKeep: NotRequired[int],
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
## StartAppReplicationRequestRequestTypeDef

```python
# StartAppReplicationRequestRequestTypeDef definition

class StartAppReplicationRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## StartOnDemandAppReplicationRequestRequestTypeDef

```python
# StartOnDemandAppReplicationRequestRequestTypeDef definition

class StartOnDemandAppReplicationRequestRequestTypeDef(TypedDict):
    appId: str,
    description: NotRequired[str],
```

## StartOnDemandReplicationRunRequestRequestTypeDef

```python
# StartOnDemandReplicationRunRequestRequestTypeDef definition

class StartOnDemandReplicationRunRequestRequestTypeDef(TypedDict):
    replicationJobId: str,
    description: NotRequired[str],
```

## StopAppReplicationRequestRequestTypeDef

```python
# StopAppReplicationRequestRequestTypeDef definition

class StopAppReplicationRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## TerminateAppRequestRequestTypeDef

```python
# TerminateAppRequestRequestTypeDef definition

class TerminateAppRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## AppSummaryTypeDef

```python
# AppSummaryTypeDef definition

class AppSummaryTypeDef(TypedDict):
    appId: NotRequired[str],
    importedAppId: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[AppStatusType],  # (1)
    statusMessage: NotRequired[str],
    replicationConfigurationStatus: NotRequired[AppReplicationConfigurationStatusType],  # (2)
    replicationStatus: NotRequired[AppReplicationStatusType],  # (3)
    replicationStatusMessage: NotRequired[str],
    latestReplicationTime: NotRequired[datetime],
    launchConfigurationStatus: NotRequired[AppLaunchConfigurationStatusType],  # (4)
    launchStatus: NotRequired[AppLaunchStatusType],  # (5)
    launchStatusMessage: NotRequired[str],
    launchDetails: NotRequired[LaunchDetailsTypeDef],  # (6)
    creationTime: NotRequired[datetime],
    lastModified: NotRequired[datetime],
    roleName: NotRequired[str],
    totalServerGroups: NotRequired[int],
    totalServers: NotRequired[int],
```

1. See [:material-code-brackets: AppStatusType](./literals.md#appstatustype) 
2. See [:material-code-brackets: AppReplicationConfigurationStatusType](./literals.md#appreplicationconfigurationstatustype) 
3. See [:material-code-brackets: AppReplicationStatusType](./literals.md#appreplicationstatustype) 
4. See [:material-code-brackets: AppLaunchConfigurationStatusType](./literals.md#applaunchconfigurationstatustype) 
5. See [:material-code-brackets: AppLaunchStatusType](./literals.md#applaunchstatustype) 
6. See [:material-code-braces: LaunchDetailsTypeDef](./type_defs.md#launchdetailstypedef) 
## CreateReplicationJobResponseTypeDef

```python
# CreateReplicationJobResponseTypeDef definition

class CreateReplicationJobResponseTypeDef(TypedDict):
    replicationJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectorsResponseTypeDef

```python
# GetConnectorsResponseTypeDef definition

class GetConnectorsResponseTypeDef(TypedDict):
    connectorList: List[ConnectorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectorTypeDef](./type_defs.md#connectortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartOnDemandReplicationRunResponseTypeDef

```python
# StartOnDemandReplicationRunResponseTypeDef definition

class StartOnDemandReplicationRunResponseTypeDef(TypedDict):
    replicationRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicationJobRequestRequestTypeDef

```python
# CreateReplicationJobRequestRequestTypeDef definition

class CreateReplicationJobRequestRequestTypeDef(TypedDict):
    serverId: str,
    seedReplicationTime: TimestampTypeDef,
    frequency: NotRequired[int],
    runOnce: NotRequired[bool],
    licenseType: NotRequired[LicenseTypeType],  # (1)
    roleName: NotRequired[str],
    description: NotRequired[str],
    numberOfRecentAmisToKeep: NotRequired[int],
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
## ServerReplicationParametersTypeDef

```python
# ServerReplicationParametersTypeDef definition

class ServerReplicationParametersTypeDef(TypedDict):
    seedTime: NotRequired[TimestampTypeDef],
    frequency: NotRequired[int],
    runOnce: NotRequired[bool],
    licenseType: NotRequired[LicenseTypeType],  # (1)
    numberOfRecentAmisToKeep: NotRequired[int],
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
## UpdateReplicationJobRequestRequestTypeDef

```python
# UpdateReplicationJobRequestRequestTypeDef definition

class UpdateReplicationJobRequestRequestTypeDef(TypedDict):
    replicationJobId: str,
    frequency: NotRequired[int],
    nextReplicationRunStartTime: NotRequired[TimestampTypeDef],
    licenseType: NotRequired[LicenseTypeType],  # (1)
    roleName: NotRequired[str],
    description: NotRequired[str],
    numberOfRecentAmisToKeep: NotRequired[int],
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
## GenerateChangeSetResponseTypeDef

```python
# GenerateChangeSetResponseTypeDef definition

class GenerateChangeSetResponseTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateTemplateResponseTypeDef

```python
# GenerateTemplateResponseTypeDef definition

class GenerateTemplateResponseTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SSMOutputTypeDef

```python
# SSMOutputTypeDef definition

class SSMOutputTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## SourceTypeDef

```python
# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## UserDataTypeDef

```python
# UserDataTypeDef definition

class UserDataTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## GetConnectorsRequestGetConnectorsPaginateTypeDef

```python
# GetConnectorsRequestGetConnectorsPaginateTypeDef definition

class GetConnectorsRequestGetConnectorsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef

```python
# GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef definition

class GetReplicationJobsRequestGetReplicationJobsPaginateTypeDef(TypedDict):
    replicationJobId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef

```python
# GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef definition

class GetReplicationRunsRequestGetReplicationRunsPaginateTypeDef(TypedDict):
    replicationJobId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAppsRequestListAppsPaginateTypeDef

```python
# ListAppsRequestListAppsPaginateTypeDef definition

class ListAppsRequestListAppsPaginateTypeDef(TypedDict):
    appIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetServersRequestGetServersPaginateTypeDef

```python
# GetServersRequestGetServersPaginateTypeDef definition

class GetServersRequestGetServersPaginateTypeDef(TypedDict):
    vmServerAddressList: NotRequired[Sequence[VmServerAddressTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetServersRequestRequestTypeDef

```python
# GetServersRequestRequestTypeDef definition

class GetServersRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    vmServerAddressList: NotRequired[Sequence[VmServerAddressTypeDef]],  # (1)
```

1. See [:material-code-braces: VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef) 
## VmServerTypeDef

```python
# VmServerTypeDef definition

class VmServerTypeDef(TypedDict):
    vmServerAddress: NotRequired[VmServerAddressTypeDef],  # (1)
    vmName: NotRequired[str],
    vmManagerName: NotRequired[str],
    vmManagerType: NotRequired[VmManagerTypeType],  # (2)
    vmPath: NotRequired[str],
```

1. See [:material-code-braces: VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef) 
2. See [:material-code-brackets: VmManagerTypeType](./literals.md#vmmanagertypetype) 
## NotifyAppValidationOutputRequestRequestTypeDef

```python
# NotifyAppValidationOutputRequestRequestTypeDef definition

class NotifyAppValidationOutputRequestRequestTypeDef(TypedDict):
    appId: str,
    notificationContext: NotRequired[NotificationContextTypeDef],  # (1)
```

1. See [:material-code-braces: NotificationContextTypeDef](./type_defs.md#notificationcontexttypedef) 
## ReplicationRunTypeDef

```python
# ReplicationRunTypeDef definition

class ReplicationRunTypeDef(TypedDict):
    replicationRunId: NotRequired[str],
    state: NotRequired[ReplicationRunStateType],  # (1)
    type: NotRequired[ReplicationRunTypeType],  # (2)
    stageDetails: NotRequired[ReplicationRunStageDetailsTypeDef],  # (3)
    statusMessage: NotRequired[str],
    amiId: NotRequired[str],
    scheduledStartTime: NotRequired[datetime],
    completedTime: NotRequired[datetime],
    description: NotRequired[str],
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
```

1. See [:material-code-brackets: ReplicationRunStateType](./literals.md#replicationrunstatetype) 
2. See [:material-code-brackets: ReplicationRunTypeType](./literals.md#replicationruntypetype) 
3. See [:material-code-braces: ReplicationRunStageDetailsTypeDef](./type_defs.md#replicationrunstagedetailstypedef) 
## ListAppsResponseTypeDef

```python
# ListAppsResponseTypeDef definition

class ListAppsResponseTypeDef(TypedDict):
    apps: List[AppSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AppSummaryTypeDef](./type_defs.md#appsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AppValidationOutputTypeDef

```python
# AppValidationOutputTypeDef definition

class AppValidationOutputTypeDef(TypedDict):
    ssmOutput: NotRequired[SSMOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SSMOutputTypeDef](./type_defs.md#ssmoutputtypedef) 
## SSMValidationParametersTypeDef

```python
# SSMValidationParametersTypeDef definition

class SSMValidationParametersTypeDef(TypedDict):
    source: NotRequired[SourceTypeDef],  # (1)
    instanceId: NotRequired[str],
    scriptType: NotRequired[ScriptTypeType],  # (2)
    command: NotRequired[str],
    executionTimeoutSeconds: NotRequired[int],
    outputS3BucketName: NotRequired[str],
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-brackets: ScriptTypeType](./literals.md#scripttypetype) 
## UserDataValidationParametersTypeDef

```python
# UserDataValidationParametersTypeDef definition

class UserDataValidationParametersTypeDef(TypedDict):
    source: NotRequired[SourceTypeDef],  # (1)
    scriptType: NotRequired[ScriptTypeType],  # (2)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-brackets: ScriptTypeType](./literals.md#scripttypetype) 
## ServerTypeDef

```python
# ServerTypeDef definition

class ServerTypeDef(TypedDict):
    serverId: NotRequired[str],
    serverType: NotRequired[ServerTypeType],  # (1)
    vmServer: NotRequired[VmServerTypeDef],  # (2)
    replicationJobId: NotRequired[str],
    replicationJobTerminated: NotRequired[bool],
```

1. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
2. See [:material-code-braces: VmServerTypeDef](./type_defs.md#vmservertypedef) 
## ReplicationJobTypeDef

```python
# ReplicationJobTypeDef definition

class ReplicationJobTypeDef(TypedDict):
    replicationJobId: NotRequired[str],
    serverId: NotRequired[str],
    serverType: NotRequired[ServerTypeType],  # (1)
    vmServer: NotRequired[VmServerTypeDef],  # (2)
    seedReplicationTime: NotRequired[datetime],
    frequency: NotRequired[int],
    runOnce: NotRequired[bool],
    nextReplicationRunStartTime: NotRequired[datetime],
    licenseType: NotRequired[LicenseTypeType],  # (3)
    roleName: NotRequired[str],
    latestAmiId: NotRequired[str],
    state: NotRequired[ReplicationJobStateType],  # (4)
    statusMessage: NotRequired[str],
    description: NotRequired[str],
    numberOfRecentAmisToKeep: NotRequired[int],
    encrypted: NotRequired[bool],
    kmsKeyId: NotRequired[str],
    replicationRunList: NotRequired[List[ReplicationRunTypeDef]],  # (5)
```

1. See [:material-code-brackets: ServerTypeType](./literals.md#servertypetype) 
2. See [:material-code-braces: VmServerTypeDef](./type_defs.md#vmservertypedef) 
3. See [:material-code-brackets: LicenseTypeType](./literals.md#licensetypetype) 
4. See [:material-code-brackets: ReplicationJobStateType](./literals.md#replicationjobstatetype) 
5. See [:material-code-braces: ReplicationRunTypeDef](./type_defs.md#replicationruntypedef) 
## AppValidationConfigurationTypeDef

```python
# AppValidationConfigurationTypeDef definition

class AppValidationConfigurationTypeDef(TypedDict):
    validationId: NotRequired[str],
    name: NotRequired[str],
    appValidationStrategy: NotRequired[AppValidationStrategyType],  # (1)
    ssmValidationParameters: NotRequired[SSMValidationParametersTypeDef],  # (2)
```

1. See [:material-code-brackets: AppValidationStrategyType](./literals.md#appvalidationstrategytype) 
2. See [:material-code-braces: SSMValidationParametersTypeDef](./type_defs.md#ssmvalidationparameterstypedef) 
## GetServersResponseTypeDef

```python
# GetServersResponseTypeDef definition

class GetServersResponseTypeDef(TypedDict):
    lastModifiedOn: datetime,
    serverCatalogStatus: ServerCatalogStatusType,  # (1)
    serverList: List[ServerTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ServerCatalogStatusType](./literals.md#servercatalogstatustype) 
2. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServerGroupOutputTypeDef

```python
# ServerGroupOutputTypeDef definition

class ServerGroupOutputTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    name: NotRequired[str],
    serverList: NotRequired[List[ServerTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
## ServerGroupTypeDef

```python
# ServerGroupTypeDef definition

class ServerGroupTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    name: NotRequired[str],
    serverList: NotRequired[Sequence[ServerTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
## ServerLaunchConfigurationTypeDef

```python
# ServerLaunchConfigurationTypeDef definition

class ServerLaunchConfigurationTypeDef(TypedDict):
    server: NotRequired[ServerTypeDef],  # (1)
    logicalId: NotRequired[str],
    vpc: NotRequired[str],
    subnet: NotRequired[str],
    securityGroup: NotRequired[str],
    ec2KeyName: NotRequired[str],
    userData: NotRequired[UserDataTypeDef],  # (2)
    instanceType: NotRequired[str],
    associatePublicIpAddress: NotRequired[bool],
    iamInstanceProfileName: NotRequired[str],
    configureScript: NotRequired[S3LocationTypeDef],  # (3)
    configureScriptType: NotRequired[ScriptTypeType],  # (4)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: UserDataTypeDef](./type_defs.md#userdatatypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-brackets: ScriptTypeType](./literals.md#scripttypetype) 
## ServerReplicationConfigurationOutputTypeDef

```python
# ServerReplicationConfigurationOutputTypeDef definition

class ServerReplicationConfigurationOutputTypeDef(TypedDict):
    server: NotRequired[ServerTypeDef],  # (1)
    serverReplicationParameters: NotRequired[ServerReplicationParametersOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ServerReplicationParametersOutputTypeDef](./type_defs.md#serverreplicationparametersoutputtypedef) 
## ServerReplicationConfigurationTypeDef

```python
# ServerReplicationConfigurationTypeDef definition

class ServerReplicationConfigurationTypeDef(TypedDict):
    server: NotRequired[ServerTypeDef],  # (1)
    serverReplicationParameters: NotRequired[ServerReplicationParametersUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ServerReplicationParametersTypeDef](./type_defs.md#serverreplicationparameterstypedef) [:material-code-braces: ServerReplicationParametersOutputTypeDef](./type_defs.md#serverreplicationparametersoutputtypedef) 
## ServerValidationConfigurationTypeDef

```python
# ServerValidationConfigurationTypeDef definition

class ServerValidationConfigurationTypeDef(TypedDict):
    server: NotRequired[ServerTypeDef],  # (1)
    validationId: NotRequired[str],
    name: NotRequired[str],
    serverValidationStrategy: NotRequired[ServerValidationStrategyType],  # (2)
    userDataValidationParameters: NotRequired[UserDataValidationParametersTypeDef],  # (3)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-brackets: ServerValidationStrategyType](./literals.md#servervalidationstrategytype) 
3. See [:material-code-braces: UserDataValidationParametersTypeDef](./type_defs.md#userdatavalidationparameterstypedef) 
## ServerValidationOutputTypeDef

```python
# ServerValidationOutputTypeDef definition

class ServerValidationOutputTypeDef(TypedDict):
    server: NotRequired[ServerTypeDef],  # (1)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
## GetReplicationJobsResponseTypeDef

```python
# GetReplicationJobsResponseTypeDef definition

class GetReplicationJobsResponseTypeDef(TypedDict):
    replicationJobList: List[ReplicationJobTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReplicationJobTypeDef](./type_defs.md#replicationjobtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReplicationRunsResponseTypeDef

```python
# GetReplicationRunsResponseTypeDef definition

class GetReplicationRunsResponseTypeDef(TypedDict):
    replicationJob: ReplicationJobTypeDef,  # (1)
    replicationRunList: List[ReplicationRunTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ReplicationJobTypeDef](./type_defs.md#replicationjobtypedef) 
2. See [:material-code-braces: ReplicationRunTypeDef](./type_defs.md#replicationruntypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAppResponseTypeDef

```python
# CreateAppResponseTypeDef definition

class CreateAppResponseTypeDef(TypedDict):
    appSummary: AppSummaryTypeDef,  # (1)
    serverGroups: List[ServerGroupOutputTypeDef],  # (2)
    tags: List[TagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AppSummaryTypeDef](./type_defs.md#appsummarytypedef) 
2. See [:material-code-braces: ServerGroupOutputTypeDef](./type_defs.md#servergroupoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppResponseTypeDef

```python
# GetAppResponseTypeDef definition

class GetAppResponseTypeDef(TypedDict):
    appSummary: AppSummaryTypeDef,  # (1)
    serverGroups: List[ServerGroupOutputTypeDef],  # (2)
    tags: List[TagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AppSummaryTypeDef](./type_defs.md#appsummarytypedef) 
2. See [:material-code-braces: ServerGroupOutputTypeDef](./type_defs.md#servergroupoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppResponseTypeDef

```python
# UpdateAppResponseTypeDef definition

class UpdateAppResponseTypeDef(TypedDict):
    appSummary: AppSummaryTypeDef,  # (1)
    serverGroups: List[ServerGroupOutputTypeDef],  # (2)
    tags: List[TagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: AppSummaryTypeDef](./type_defs.md#appsummarytypedef) 
2. See [:material-code-braces: ServerGroupOutputTypeDef](./type_defs.md#servergroupoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAppRequestRequestTypeDef

```python
# UpdateAppRequestRequestTypeDef definition

class UpdateAppRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    roleName: NotRequired[str],
    serverGroups: NotRequired[Sequence[ServerGroupTypeDef]],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ServerGroupTypeDef](./type_defs.md#servergrouptypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ServerGroupLaunchConfigurationOutputTypeDef

```python
# ServerGroupLaunchConfigurationOutputTypeDef definition

class ServerGroupLaunchConfigurationOutputTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    launchOrder: NotRequired[int],
    serverLaunchConfigurations: NotRequired[List[ServerLaunchConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerLaunchConfigurationTypeDef](./type_defs.md#serverlaunchconfigurationtypedef) 
## ServerGroupLaunchConfigurationTypeDef

```python
# ServerGroupLaunchConfigurationTypeDef definition

class ServerGroupLaunchConfigurationTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    launchOrder: NotRequired[int],
    serverLaunchConfigurations: NotRequired[Sequence[ServerLaunchConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerLaunchConfigurationTypeDef](./type_defs.md#serverlaunchconfigurationtypedef) 
## ServerGroupReplicationConfigurationOutputTypeDef

```python
# ServerGroupReplicationConfigurationOutputTypeDef definition

class ServerGroupReplicationConfigurationOutputTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    serverReplicationConfigurations: NotRequired[List[ServerReplicationConfigurationOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerReplicationConfigurationOutputTypeDef](./type_defs.md#serverreplicationconfigurationoutputtypedef) 
## ServerGroupValidationConfigurationOutputTypeDef

```python
# ServerGroupValidationConfigurationOutputTypeDef definition

class ServerGroupValidationConfigurationOutputTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    serverValidationConfigurations: NotRequired[List[ServerValidationConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerValidationConfigurationTypeDef](./type_defs.md#servervalidationconfigurationtypedef) 
## ServerGroupValidationConfigurationTypeDef

```python
# ServerGroupValidationConfigurationTypeDef definition

class ServerGroupValidationConfigurationTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    serverValidationConfigurations: NotRequired[Sequence[ServerValidationConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerValidationConfigurationTypeDef](./type_defs.md#servervalidationconfigurationtypedef) 
## ValidationOutputTypeDef

```python
# ValidationOutputTypeDef definition

class ValidationOutputTypeDef(TypedDict):
    validationId: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[ValidationStatusType],  # (1)
    statusMessage: NotRequired[str],
    latestValidationTime: NotRequired[datetime],
    appValidationOutput: NotRequired[AppValidationOutputTypeDef],  # (2)
    serverValidationOutput: NotRequired[ServerValidationOutputTypeDef],  # (3)
```

1. See [:material-code-brackets: ValidationStatusType](./literals.md#validationstatustype) 
2. See [:material-code-braces: AppValidationOutputTypeDef](./type_defs.md#appvalidationoutputtypedef) 
3. See [:material-code-braces: ServerValidationOutputTypeDef](./type_defs.md#servervalidationoutputtypedef) 
## CreateAppRequestRequestTypeDef

```python
# CreateAppRequestRequestTypeDef definition

class CreateAppRequestRequestTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    roleName: NotRequired[str],
    clientToken: NotRequired[str],
    serverGroups: NotRequired[Sequence[ServerGroupUnionTypeDef]],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ServerGroupTypeDef](./type_defs.md#servergrouptypedef) [:material-code-braces: ServerGroupOutputTypeDef](./type_defs.md#servergroupoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetAppLaunchConfigurationResponseTypeDef

```python
# GetAppLaunchConfigurationResponseTypeDef definition

class GetAppLaunchConfigurationResponseTypeDef(TypedDict):
    appId: str,
    roleName: str,
    autoLaunch: bool,
    serverGroupLaunchConfigurations: List[ServerGroupLaunchConfigurationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerGroupLaunchConfigurationOutputTypeDef](./type_defs.md#servergrouplaunchconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppReplicationConfigurationResponseTypeDef

```python
# GetAppReplicationConfigurationResponseTypeDef definition

class GetAppReplicationConfigurationResponseTypeDef(TypedDict):
    serverGroupReplicationConfigurations: List[ServerGroupReplicationConfigurationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerGroupReplicationConfigurationOutputTypeDef](./type_defs.md#servergroupreplicationconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServerGroupReplicationConfigurationTypeDef

```python
# ServerGroupReplicationConfigurationTypeDef definition

class ServerGroupReplicationConfigurationTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    serverReplicationConfigurations: NotRequired[Sequence[ServerReplicationConfigurationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerReplicationConfigurationTypeDef](./type_defs.md#serverreplicationconfigurationtypedef) [:material-code-braces: ServerReplicationConfigurationOutputTypeDef](./type_defs.md#serverreplicationconfigurationoutputtypedef) 
## GetAppValidationConfigurationResponseTypeDef

```python
# GetAppValidationConfigurationResponseTypeDef definition

class GetAppValidationConfigurationResponseTypeDef(TypedDict):
    appValidationConfigurations: List[AppValidationConfigurationTypeDef],  # (1)
    serverGroupValidationConfigurations: List[ServerGroupValidationConfigurationOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AppValidationConfigurationTypeDef](./type_defs.md#appvalidationconfigurationtypedef) 
2. See [:material-code-braces: ServerGroupValidationConfigurationOutputTypeDef](./type_defs.md#servergroupvalidationconfigurationoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAppValidationOutputResponseTypeDef

```python
# GetAppValidationOutputResponseTypeDef definition

class GetAppValidationOutputResponseTypeDef(TypedDict):
    validationOutputList: List[ValidationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidationOutputTypeDef](./type_defs.md#validationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAppLaunchConfigurationRequestRequestTypeDef

```python
# PutAppLaunchConfigurationRequestRequestTypeDef definition

class PutAppLaunchConfigurationRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    roleName: NotRequired[str],
    autoLaunch: NotRequired[bool],
    serverGroupLaunchConfigurations: NotRequired[Sequence[ServerGroupLaunchConfigurationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerGroupLaunchConfigurationTypeDef](./type_defs.md#servergrouplaunchconfigurationtypedef) [:material-code-braces: ServerGroupLaunchConfigurationOutputTypeDef](./type_defs.md#servergrouplaunchconfigurationoutputtypedef) 
## PutAppValidationConfigurationRequestRequestTypeDef

```python
# PutAppValidationConfigurationRequestRequestTypeDef definition

class PutAppValidationConfigurationRequestRequestTypeDef(TypedDict):
    appId: str,
    appValidationConfigurations: NotRequired[Sequence[AppValidationConfigurationTypeDef]],  # (1)
    serverGroupValidationConfigurations: NotRequired[Sequence[ServerGroupValidationConfigurationUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: AppValidationConfigurationTypeDef](./type_defs.md#appvalidationconfigurationtypedef) 
2. See [:material-code-braces: ServerGroupValidationConfigurationTypeDef](./type_defs.md#servergroupvalidationconfigurationtypedef) [:material-code-braces: ServerGroupValidationConfigurationOutputTypeDef](./type_defs.md#servergroupvalidationconfigurationoutputtypedef) 
## PutAppReplicationConfigurationRequestRequestTypeDef

```python
# PutAppReplicationConfigurationRequestRequestTypeDef definition

class PutAppReplicationConfigurationRequestRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    serverGroupReplicationConfigurations: NotRequired[Sequence[ServerGroupReplicationConfigurationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerGroupReplicationConfigurationTypeDef](./type_defs.md#servergroupreplicationconfigurationtypedef) [:material-code-braces: ServerGroupReplicationConfigurationOutputTypeDef](./type_defs.md#servergroupreplicationconfigurationoutputtypedef) 

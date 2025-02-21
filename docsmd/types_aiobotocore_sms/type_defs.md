# Type definitions

> [Index](../README.md) > [SMS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SMS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms.html#sms)
    type annotations stubs module [types-aiobotocore-sms](https://pypi.org/project/types-aiobotocore-sms/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_sms.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ServerReplicationParametersUnionTypeDef

```python
# ServerReplicationParametersUnionTypeDef Union usage example

from types_aiobotocore_sms.type_defs import ServerReplicationParametersUnionTypeDef


def get_value() -> ServerReplicationParametersUnionTypeDef:
    return ...


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
# ServerGroupUnionTypeDef Union usage example

from types_aiobotocore_sms.type_defs import ServerGroupUnionTypeDef


def get_value() -> ServerGroupUnionTypeDef:
    return ...


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
# ServerReplicationConfigurationUnionTypeDef Union usage example

from types_aiobotocore_sms.type_defs import ServerReplicationConfigurationUnionTypeDef


def get_value() -> ServerReplicationConfigurationUnionTypeDef:
    return ...


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
# ServerGroupLaunchConfigurationUnionTypeDef Union usage example

from types_aiobotocore_sms.type_defs import ServerGroupLaunchConfigurationUnionTypeDef


def get_value() -> ServerGroupLaunchConfigurationUnionTypeDef:
    return ...


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
# ServerGroupValidationConfigurationUnionTypeDef Union usage example

from types_aiobotocore_sms.type_defs import ServerGroupValidationConfigurationUnionTypeDef


def get_value() -> ServerGroupValidationConfigurationUnionTypeDef:
    return ...


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
# ServerGroupReplicationConfigurationUnionTypeDef Union usage example

from types_aiobotocore_sms.type_defs import ServerGroupReplicationConfigurationUnionTypeDef


def get_value() -> ServerGroupReplicationConfigurationUnionTypeDef:
    return ...


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
# LaunchDetailsTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import LaunchDetailsTypeDef


def get_value() -> LaunchDetailsTypeDef:
    return {
        "latestLaunchTime": ...,
    }


# LaunchDetailsTypeDef definition

class LaunchDetailsTypeDef(TypedDict):
    latestLaunchTime: NotRequired[datetime],
    stackName: NotRequired[str],
    stackId: NotRequired[str],
```

## ConnectorTypeDef

```python
# ConnectorTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ConnectorTypeDef


def get_value() -> ConnectorTypeDef:
    return {
        "connectorId": ...,
    }


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
# TagTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## DeleteAppLaunchConfigurationRequestTypeDef

```python
# DeleteAppLaunchConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import DeleteAppLaunchConfigurationRequestTypeDef


def get_value() -> DeleteAppLaunchConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# DeleteAppLaunchConfigurationRequestTypeDef definition

class DeleteAppLaunchConfigurationRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## DeleteAppReplicationConfigurationRequestTypeDef

```python
# DeleteAppReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import DeleteAppReplicationConfigurationRequestTypeDef


def get_value() -> DeleteAppReplicationConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# DeleteAppReplicationConfigurationRequestTypeDef definition

class DeleteAppReplicationConfigurationRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## DeleteAppRequestTypeDef

```python
# DeleteAppRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import DeleteAppRequestTypeDef


def get_value() -> DeleteAppRequestTypeDef:
    return {
        "appId": ...,
    }


# DeleteAppRequestTypeDef definition

class DeleteAppRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    forceStopAppReplication: NotRequired[bool],
    forceTerminateApp: NotRequired[bool],
```

## DeleteAppValidationConfigurationRequestTypeDef

```python
# DeleteAppValidationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import DeleteAppValidationConfigurationRequestTypeDef


def get_value() -> DeleteAppValidationConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# DeleteAppValidationConfigurationRequestTypeDef definition

class DeleteAppValidationConfigurationRequestTypeDef(TypedDict):
    appId: str,
```

## DeleteReplicationJobRequestTypeDef

```python
# DeleteReplicationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import DeleteReplicationJobRequestTypeDef


def get_value() -> DeleteReplicationJobRequestTypeDef:
    return {
        "replicationJobId": ...,
    }


# DeleteReplicationJobRequestTypeDef definition

class DeleteReplicationJobRequestTypeDef(TypedDict):
    replicationJobId: str,
```

## DisassociateConnectorRequestTypeDef

```python
# DisassociateConnectorRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import DisassociateConnectorRequestTypeDef


def get_value() -> DisassociateConnectorRequestTypeDef:
    return {
        "connectorId": ...,
    }


# DisassociateConnectorRequestTypeDef definition

class DisassociateConnectorRequestTypeDef(TypedDict):
    connectorId: str,
```

## GenerateChangeSetRequestTypeDef

```python
# GenerateChangeSetRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GenerateChangeSetRequestTypeDef


def get_value() -> GenerateChangeSetRequestTypeDef:
    return {
        "appId": ...,
    }


# GenerateChangeSetRequestTypeDef definition

class GenerateChangeSetRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    changesetFormat: NotRequired[OutputFormatType],  # (1)
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## S3LocationTypeDef

```python
# S3LocationTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import S3LocationTypeDef


def get_value() -> S3LocationTypeDef:
    return {
        "bucket": ...,
    }


# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: NotRequired[str],
    key: NotRequired[str],
```

## GenerateTemplateRequestTypeDef

```python
# GenerateTemplateRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GenerateTemplateRequestTypeDef


def get_value() -> GenerateTemplateRequestTypeDef:
    return {
        "appId": ...,
    }


# GenerateTemplateRequestTypeDef definition

class GenerateTemplateRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    templateFormat: NotRequired[OutputFormatType],  # (1)
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
## GetAppLaunchConfigurationRequestTypeDef

```python
# GetAppLaunchConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppLaunchConfigurationRequestTypeDef


def get_value() -> GetAppLaunchConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# GetAppLaunchConfigurationRequestTypeDef definition

class GetAppLaunchConfigurationRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## GetAppReplicationConfigurationRequestTypeDef

```python
# GetAppReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppReplicationConfigurationRequestTypeDef


def get_value() -> GetAppReplicationConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# GetAppReplicationConfigurationRequestTypeDef definition

class GetAppReplicationConfigurationRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## GetAppRequestTypeDef

```python
# GetAppRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppRequestTypeDef


def get_value() -> GetAppRequestTypeDef:
    return {
        "appId": ...,
    }


# GetAppRequestTypeDef definition

class GetAppRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## GetAppValidationConfigurationRequestTypeDef

```python
# GetAppValidationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppValidationConfigurationRequestTypeDef


def get_value() -> GetAppValidationConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# GetAppValidationConfigurationRequestTypeDef definition

class GetAppValidationConfigurationRequestTypeDef(TypedDict):
    appId: str,
```

## GetAppValidationOutputRequestTypeDef

```python
# GetAppValidationOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppValidationOutputRequestTypeDef


def get_value() -> GetAppValidationOutputRequestTypeDef:
    return {
        "appId": ...,
    }


# GetAppValidationOutputRequestTypeDef definition

class GetAppValidationOutputRequestTypeDef(TypedDict):
    appId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import PaginatorConfigTypeDef


def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }


# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetConnectorsRequestTypeDef

```python
# GetConnectorsRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetConnectorsRequestTypeDef


def get_value() -> GetConnectorsRequestTypeDef:
    return {
        "nextToken": ...,
    }


# GetConnectorsRequestTypeDef definition

class GetConnectorsRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetReplicationJobsRequestTypeDef

```python
# GetReplicationJobsRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetReplicationJobsRequestTypeDef


def get_value() -> GetReplicationJobsRequestTypeDef:
    return {
        "replicationJobId": ...,
    }


# GetReplicationJobsRequestTypeDef definition

class GetReplicationJobsRequestTypeDef(TypedDict):
    replicationJobId: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetReplicationRunsRequestTypeDef

```python
# GetReplicationRunsRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetReplicationRunsRequestTypeDef


def get_value() -> GetReplicationRunsRequestTypeDef:
    return {
        "replicationJobId": ...,
    }


# GetReplicationRunsRequestTypeDef definition

class GetReplicationRunsRequestTypeDef(TypedDict):
    replicationJobId: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## VmServerAddressTypeDef

```python
# VmServerAddressTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import VmServerAddressTypeDef


def get_value() -> VmServerAddressTypeDef:
    return {
        "vmManagerId": ...,
    }


# VmServerAddressTypeDef definition

class VmServerAddressTypeDef(TypedDict):
    vmManagerId: NotRequired[str],
    vmId: NotRequired[str],
```

## ImportAppCatalogRequestTypeDef

```python
# ImportAppCatalogRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ImportAppCatalogRequestTypeDef


def get_value() -> ImportAppCatalogRequestTypeDef:
    return {
        "roleName": ...,
    }


# ImportAppCatalogRequestTypeDef definition

class ImportAppCatalogRequestTypeDef(TypedDict):
    roleName: NotRequired[str],
```

## LaunchAppRequestTypeDef

```python
# LaunchAppRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import LaunchAppRequestTypeDef


def get_value() -> LaunchAppRequestTypeDef:
    return {
        "appId": ...,
    }


# LaunchAppRequestTypeDef definition

class LaunchAppRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## ListAppsRequestTypeDef

```python
# ListAppsRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ListAppsRequestTypeDef


def get_value() -> ListAppsRequestTypeDef:
    return {
        "appIds": ...,
    }


# ListAppsRequestTypeDef definition

class ListAppsRequestTypeDef(TypedDict):
    appIds: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## NotificationContextTypeDef

```python
# NotificationContextTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import NotificationContextTypeDef


def get_value() -> NotificationContextTypeDef:
    return {
        "validationId": ...,
    }


# NotificationContextTypeDef definition

class NotificationContextTypeDef(TypedDict):
    validationId: NotRequired[str],
    status: NotRequired[ValidationStatusType],  # (1)
    statusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ValidationStatusType](./literals.md#validationstatustype) 
## ReplicationRunStageDetailsTypeDef

```python
# ReplicationRunStageDetailsTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ReplicationRunStageDetailsTypeDef


def get_value() -> ReplicationRunStageDetailsTypeDef:
    return {
        "stage": ...,
    }


# ReplicationRunStageDetailsTypeDef definition

class ReplicationRunStageDetailsTypeDef(TypedDict):
    stage: NotRequired[str],
    stageProgress: NotRequired[str],
```

## ServerReplicationParametersOutputTypeDef

```python
# ServerReplicationParametersOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerReplicationParametersOutputTypeDef


def get_value() -> ServerReplicationParametersOutputTypeDef:
    return {
        "seedTime": ...,
    }


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
## StartAppReplicationRequestTypeDef

```python
# StartAppReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import StartAppReplicationRequestTypeDef


def get_value() -> StartAppReplicationRequestTypeDef:
    return {
        "appId": ...,
    }


# StartAppReplicationRequestTypeDef definition

class StartAppReplicationRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## StartOnDemandAppReplicationRequestTypeDef

```python
# StartOnDemandAppReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import StartOnDemandAppReplicationRequestTypeDef


def get_value() -> StartOnDemandAppReplicationRequestTypeDef:
    return {
        "appId": ...,
    }


# StartOnDemandAppReplicationRequestTypeDef definition

class StartOnDemandAppReplicationRequestTypeDef(TypedDict):
    appId: str,
    description: NotRequired[str],
```

## StartOnDemandReplicationRunRequestTypeDef

```python
# StartOnDemandReplicationRunRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import StartOnDemandReplicationRunRequestTypeDef


def get_value() -> StartOnDemandReplicationRunRequestTypeDef:
    return {
        "replicationJobId": ...,
    }


# StartOnDemandReplicationRunRequestTypeDef definition

class StartOnDemandReplicationRunRequestTypeDef(TypedDict):
    replicationJobId: str,
    description: NotRequired[str],
```

## StopAppReplicationRequestTypeDef

```python
# StopAppReplicationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import StopAppReplicationRequestTypeDef


def get_value() -> StopAppReplicationRequestTypeDef:
    return {
        "appId": ...,
    }


# StopAppReplicationRequestTypeDef definition

class StopAppReplicationRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## TerminateAppRequestTypeDef

```python
# TerminateAppRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import TerminateAppRequestTypeDef


def get_value() -> TerminateAppRequestTypeDef:
    return {
        "appId": ...,
    }


# TerminateAppRequestTypeDef definition

class TerminateAppRequestTypeDef(TypedDict):
    appId: NotRequired[str],
```

## AppSummaryTypeDef

```python
# AppSummaryTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import AppSummaryTypeDef


def get_value() -> AppSummaryTypeDef:
    return {
        "appId": ...,
    }


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
# CreateReplicationJobResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import CreateReplicationJobResponseTypeDef


def get_value() -> CreateReplicationJobResponseTypeDef:
    return {
        "replicationJobId": ...,
    }


# CreateReplicationJobResponseTypeDef definition

class CreateReplicationJobResponseTypeDef(TypedDict):
    replicationJobId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectorsResponseTypeDef

```python
# GetConnectorsResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetConnectorsResponseTypeDef


def get_value() -> GetConnectorsResponseTypeDef:
    return {
        "connectorList": ...,
    }


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
# StartOnDemandReplicationRunResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import StartOnDemandReplicationRunResponseTypeDef


def get_value() -> StartOnDemandReplicationRunResponseTypeDef:
    return {
        "replicationRunId": ...,
    }


# StartOnDemandReplicationRunResponseTypeDef definition

class StartOnDemandReplicationRunResponseTypeDef(TypedDict):
    replicationRunId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicationJobRequestTypeDef

```python
# CreateReplicationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import CreateReplicationJobRequestTypeDef


def get_value() -> CreateReplicationJobRequestTypeDef:
    return {
        "serverId": ...,
    }


# CreateReplicationJobRequestTypeDef definition

class CreateReplicationJobRequestTypeDef(TypedDict):
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
# ServerReplicationParametersTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerReplicationParametersTypeDef


def get_value() -> ServerReplicationParametersTypeDef:
    return {
        "seedTime": ...,
    }


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
## UpdateReplicationJobRequestTypeDef

```python
# UpdateReplicationJobRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import UpdateReplicationJobRequestTypeDef


def get_value() -> UpdateReplicationJobRequestTypeDef:
    return {
        "replicationJobId": ...,
    }


# UpdateReplicationJobRequestTypeDef definition

class UpdateReplicationJobRequestTypeDef(TypedDict):
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
# GenerateChangeSetResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GenerateChangeSetResponseTypeDef


def get_value() -> GenerateChangeSetResponseTypeDef:
    return {
        "s3Location": ...,
    }


# GenerateChangeSetResponseTypeDef definition

class GenerateChangeSetResponseTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GenerateTemplateResponseTypeDef

```python
# GenerateTemplateResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GenerateTemplateResponseTypeDef


def get_value() -> GenerateTemplateResponseTypeDef:
    return {
        "s3Location": ...,
    }


# GenerateTemplateResponseTypeDef definition

class GenerateTemplateResponseTypeDef(TypedDict):
    s3Location: S3LocationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SSMOutputTypeDef

```python
# SSMOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import SSMOutputTypeDef


def get_value() -> SSMOutputTypeDef:
    return {
        "s3Location": ...,
    }


# SSMOutputTypeDef definition

class SSMOutputTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## SourceTypeDef

```python
# SourceTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import SourceTypeDef


def get_value() -> SourceTypeDef:
    return {
        "s3Location": ...,
    }


# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## UserDataTypeDef

```python
# UserDataTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import UserDataTypeDef


def get_value() -> UserDataTypeDef:
    return {
        "s3Location": ...,
    }


# UserDataTypeDef definition

class UserDataTypeDef(TypedDict):
    s3Location: NotRequired[S3LocationTypeDef],  # (1)
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## GetConnectorsRequestPaginateTypeDef

```python
# GetConnectorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetConnectorsRequestPaginateTypeDef


def get_value() -> GetConnectorsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# GetConnectorsRequestPaginateTypeDef definition

class GetConnectorsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetReplicationJobsRequestPaginateTypeDef

```python
# GetReplicationJobsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetReplicationJobsRequestPaginateTypeDef


def get_value() -> GetReplicationJobsRequestPaginateTypeDef:
    return {
        "replicationJobId": ...,
    }


# GetReplicationJobsRequestPaginateTypeDef definition

class GetReplicationJobsRequestPaginateTypeDef(TypedDict):
    replicationJobId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetReplicationRunsRequestPaginateTypeDef

```python
# GetReplicationRunsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetReplicationRunsRequestPaginateTypeDef


def get_value() -> GetReplicationRunsRequestPaginateTypeDef:
    return {
        "replicationJobId": ...,
    }


# GetReplicationRunsRequestPaginateTypeDef definition

class GetReplicationRunsRequestPaginateTypeDef(TypedDict):
    replicationJobId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAppsRequestPaginateTypeDef

```python
# ListAppsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ListAppsRequestPaginateTypeDef


def get_value() -> ListAppsRequestPaginateTypeDef:
    return {
        "appIds": ...,
    }


# ListAppsRequestPaginateTypeDef definition

class ListAppsRequestPaginateTypeDef(TypedDict):
    appIds: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetServersRequestPaginateTypeDef

```python
# GetServersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetServersRequestPaginateTypeDef


def get_value() -> GetServersRequestPaginateTypeDef:
    return {
        "vmServerAddressList": ...,
    }


# GetServersRequestPaginateTypeDef definition

class GetServersRequestPaginateTypeDef(TypedDict):
    vmServerAddressList: NotRequired[Sequence[VmServerAddressTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetServersRequestTypeDef

```python
# GetServersRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetServersRequestTypeDef


def get_value() -> GetServersRequestTypeDef:
    return {
        "nextToken": ...,
    }


# GetServersRequestTypeDef definition

class GetServersRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    vmServerAddressList: NotRequired[Sequence[VmServerAddressTypeDef]],  # (1)
```

1. See [:material-code-braces: VmServerAddressTypeDef](./type_defs.md#vmserveraddresstypedef) 
## VmServerTypeDef

```python
# VmServerTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import VmServerTypeDef


def get_value() -> VmServerTypeDef:
    return {
        "vmServerAddress": ...,
    }


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
## NotifyAppValidationOutputRequestTypeDef

```python
# NotifyAppValidationOutputRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import NotifyAppValidationOutputRequestTypeDef


def get_value() -> NotifyAppValidationOutputRequestTypeDef:
    return {
        "appId": ...,
    }


# NotifyAppValidationOutputRequestTypeDef definition

class NotifyAppValidationOutputRequestTypeDef(TypedDict):
    appId: str,
    notificationContext: NotRequired[NotificationContextTypeDef],  # (1)
```

1. See [:material-code-braces: NotificationContextTypeDef](./type_defs.md#notificationcontexttypedef) 
## ReplicationRunTypeDef

```python
# ReplicationRunTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ReplicationRunTypeDef


def get_value() -> ReplicationRunTypeDef:
    return {
        "replicationRunId": ...,
    }


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
# ListAppsResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ListAppsResponseTypeDef


def get_value() -> ListAppsResponseTypeDef:
    return {
        "apps": ...,
    }


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
# AppValidationOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import AppValidationOutputTypeDef


def get_value() -> AppValidationOutputTypeDef:
    return {
        "ssmOutput": ...,
    }


# AppValidationOutputTypeDef definition

class AppValidationOutputTypeDef(TypedDict):
    ssmOutput: NotRequired[SSMOutputTypeDef],  # (1)
```

1. See [:material-code-braces: SSMOutputTypeDef](./type_defs.md#ssmoutputtypedef) 
## SSMValidationParametersTypeDef

```python
# SSMValidationParametersTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import SSMValidationParametersTypeDef


def get_value() -> SSMValidationParametersTypeDef:
    return {
        "source": ...,
    }


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
# UserDataValidationParametersTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import UserDataValidationParametersTypeDef


def get_value() -> UserDataValidationParametersTypeDef:
    return {
        "source": ...,
    }


# UserDataValidationParametersTypeDef definition

class UserDataValidationParametersTypeDef(TypedDict):
    source: NotRequired[SourceTypeDef],  # (1)
    scriptType: NotRequired[ScriptTypeType],  # (2)
```

1. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
2. See [:material-code-brackets: ScriptTypeType](./literals.md#scripttypetype) 
## ServerTypeDef

```python
# ServerTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerTypeDef


def get_value() -> ServerTypeDef:
    return {
        "serverId": ...,
    }


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
# ReplicationJobTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ReplicationJobTypeDef


def get_value() -> ReplicationJobTypeDef:
    return {
        "replicationJobId": ...,
    }


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
# AppValidationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import AppValidationConfigurationTypeDef


def get_value() -> AppValidationConfigurationTypeDef:
    return {
        "validationId": ...,
    }


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
# GetServersResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetServersResponseTypeDef


def get_value() -> GetServersResponseTypeDef:
    return {
        "lastModifiedOn": ...,
    }


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
# ServerGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerGroupOutputTypeDef


def get_value() -> ServerGroupOutputTypeDef:
    return {
        "serverGroupId": ...,
    }


# ServerGroupOutputTypeDef definition

class ServerGroupOutputTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    name: NotRequired[str],
    serverList: NotRequired[List[ServerTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
## ServerGroupTypeDef

```python
# ServerGroupTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerGroupTypeDef


def get_value() -> ServerGroupTypeDef:
    return {
        "serverGroupId": ...,
    }


# ServerGroupTypeDef definition

class ServerGroupTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    name: NotRequired[str],
    serverList: NotRequired[Sequence[ServerTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
## ServerLaunchConfigurationTypeDef

```python
# ServerLaunchConfigurationTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerLaunchConfigurationTypeDef


def get_value() -> ServerLaunchConfigurationTypeDef:
    return {
        "server": ...,
    }


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
# ServerReplicationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerReplicationConfigurationOutputTypeDef


def get_value() -> ServerReplicationConfigurationOutputTypeDef:
    return {
        "server": ...,
    }


# ServerReplicationConfigurationOutputTypeDef definition

class ServerReplicationConfigurationOutputTypeDef(TypedDict):
    server: NotRequired[ServerTypeDef],  # (1)
    serverReplicationParameters: NotRequired[ServerReplicationParametersOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ServerReplicationParametersOutputTypeDef](./type_defs.md#serverreplicationparametersoutputtypedef) 
## ServerReplicationConfigurationTypeDef

```python
# ServerReplicationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerReplicationConfigurationTypeDef


def get_value() -> ServerReplicationConfigurationTypeDef:
    return {
        "server": ...,
    }


# ServerReplicationConfigurationTypeDef definition

class ServerReplicationConfigurationTypeDef(TypedDict):
    server: NotRequired[ServerTypeDef],  # (1)
    serverReplicationParameters: NotRequired[ServerReplicationParametersUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
2. See [:material-code-braces: ServerReplicationParametersTypeDef](./type_defs.md#serverreplicationparameterstypedef) [:material-code-braces: ServerReplicationParametersOutputTypeDef](./type_defs.md#serverreplicationparametersoutputtypedef) 
## ServerValidationConfigurationTypeDef

```python
# ServerValidationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerValidationConfigurationTypeDef


def get_value() -> ServerValidationConfigurationTypeDef:
    return {
        "server": ...,
    }


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
# ServerValidationOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerValidationOutputTypeDef


def get_value() -> ServerValidationOutputTypeDef:
    return {
        "server": ...,
    }


# ServerValidationOutputTypeDef definition

class ServerValidationOutputTypeDef(TypedDict):
    server: NotRequired[ServerTypeDef],  # (1)
```

1. See [:material-code-braces: ServerTypeDef](./type_defs.md#servertypedef) 
## GetReplicationJobsResponseTypeDef

```python
# GetReplicationJobsResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetReplicationJobsResponseTypeDef


def get_value() -> GetReplicationJobsResponseTypeDef:
    return {
        "replicationJobList": ...,
    }


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
# GetReplicationRunsResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetReplicationRunsResponseTypeDef


def get_value() -> GetReplicationRunsResponseTypeDef:
    return {
        "replicationJob": ...,
    }


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
# CreateAppResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import CreateAppResponseTypeDef


def get_value() -> CreateAppResponseTypeDef:
    return {
        "appSummary": ...,
    }


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
# GetAppResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppResponseTypeDef


def get_value() -> GetAppResponseTypeDef:
    return {
        "appSummary": ...,
    }


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
# UpdateAppResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import UpdateAppResponseTypeDef


def get_value() -> UpdateAppResponseTypeDef:
    return {
        "appSummary": ...,
    }


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
## ServerGroupLaunchConfigurationOutputTypeDef

```python
# ServerGroupLaunchConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerGroupLaunchConfigurationOutputTypeDef


def get_value() -> ServerGroupLaunchConfigurationOutputTypeDef:
    return {
        "serverGroupId": ...,
    }


# ServerGroupLaunchConfigurationOutputTypeDef definition

class ServerGroupLaunchConfigurationOutputTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    launchOrder: NotRequired[int],
    serverLaunchConfigurations: NotRequired[List[ServerLaunchConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerLaunchConfigurationTypeDef](./type_defs.md#serverlaunchconfigurationtypedef) 
## ServerGroupLaunchConfigurationTypeDef

```python
# ServerGroupLaunchConfigurationTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerGroupLaunchConfigurationTypeDef


def get_value() -> ServerGroupLaunchConfigurationTypeDef:
    return {
        "serverGroupId": ...,
    }


# ServerGroupLaunchConfigurationTypeDef definition

class ServerGroupLaunchConfigurationTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    launchOrder: NotRequired[int],
    serverLaunchConfigurations: NotRequired[Sequence[ServerLaunchConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerLaunchConfigurationTypeDef](./type_defs.md#serverlaunchconfigurationtypedef) 
## ServerGroupReplicationConfigurationOutputTypeDef

```python
# ServerGroupReplicationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerGroupReplicationConfigurationOutputTypeDef


def get_value() -> ServerGroupReplicationConfigurationOutputTypeDef:
    return {
        "serverGroupId": ...,
    }


# ServerGroupReplicationConfigurationOutputTypeDef definition

class ServerGroupReplicationConfigurationOutputTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    serverReplicationConfigurations: NotRequired[List[ServerReplicationConfigurationOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerReplicationConfigurationOutputTypeDef](./type_defs.md#serverreplicationconfigurationoutputtypedef) 
## ServerGroupValidationConfigurationOutputTypeDef

```python
# ServerGroupValidationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerGroupValidationConfigurationOutputTypeDef


def get_value() -> ServerGroupValidationConfigurationOutputTypeDef:
    return {
        "serverGroupId": ...,
    }


# ServerGroupValidationConfigurationOutputTypeDef definition

class ServerGroupValidationConfigurationOutputTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    serverValidationConfigurations: NotRequired[List[ServerValidationConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerValidationConfigurationTypeDef](./type_defs.md#servervalidationconfigurationtypedef) 
## ServerGroupValidationConfigurationTypeDef

```python
# ServerGroupValidationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerGroupValidationConfigurationTypeDef


def get_value() -> ServerGroupValidationConfigurationTypeDef:
    return {
        "serverGroupId": ...,
    }


# ServerGroupValidationConfigurationTypeDef definition

class ServerGroupValidationConfigurationTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    serverValidationConfigurations: NotRequired[Sequence[ServerValidationConfigurationTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerValidationConfigurationTypeDef](./type_defs.md#servervalidationconfigurationtypedef) 
## ValidationOutputTypeDef

```python
# ValidationOutputTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ValidationOutputTypeDef


def get_value() -> ValidationOutputTypeDef:
    return {
        "validationId": ...,
    }


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
## CreateAppRequestTypeDef

```python
# CreateAppRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import CreateAppRequestTypeDef


def get_value() -> CreateAppRequestTypeDef:
    return {
        "name": ...,
    }


# CreateAppRequestTypeDef definition

class CreateAppRequestTypeDef(TypedDict):
    name: NotRequired[str],
    description: NotRequired[str],
    roleName: NotRequired[str],
    clientToken: NotRequired[str],
    serverGroups: NotRequired[Sequence[ServerGroupUnionTypeDef]],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ServerGroupTypeDef](./type_defs.md#servergrouptypedef) [:material-code-braces: ServerGroupOutputTypeDef](./type_defs.md#servergroupoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateAppRequestTypeDef

```python
# UpdateAppRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import UpdateAppRequestTypeDef


def get_value() -> UpdateAppRequestTypeDef:
    return {
        "appId": ...,
    }


# UpdateAppRequestTypeDef definition

class UpdateAppRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    roleName: NotRequired[str],
    serverGroups: NotRequired[Sequence[ServerGroupUnionTypeDef]],  # (1)
    tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ServerGroupTypeDef](./type_defs.md#servergrouptypedef) [:material-code-braces: ServerGroupOutputTypeDef](./type_defs.md#servergroupoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetAppLaunchConfigurationResponseTypeDef

```python
# GetAppLaunchConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppLaunchConfigurationResponseTypeDef


def get_value() -> GetAppLaunchConfigurationResponseTypeDef:
    return {
        "appId": ...,
    }


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
# GetAppReplicationConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppReplicationConfigurationResponseTypeDef


def get_value() -> GetAppReplicationConfigurationResponseTypeDef:
    return {
        "serverGroupReplicationConfigurations": ...,
    }


# GetAppReplicationConfigurationResponseTypeDef definition

class GetAppReplicationConfigurationResponseTypeDef(TypedDict):
    serverGroupReplicationConfigurations: List[ServerGroupReplicationConfigurationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServerGroupReplicationConfigurationOutputTypeDef](./type_defs.md#servergroupreplicationconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServerGroupReplicationConfigurationTypeDef

```python
# ServerGroupReplicationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import ServerGroupReplicationConfigurationTypeDef


def get_value() -> ServerGroupReplicationConfigurationTypeDef:
    return {
        "serverGroupId": ...,
    }


# ServerGroupReplicationConfigurationTypeDef definition

class ServerGroupReplicationConfigurationTypeDef(TypedDict):
    serverGroupId: NotRequired[str],
    serverReplicationConfigurations: NotRequired[Sequence[ServerReplicationConfigurationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerReplicationConfigurationTypeDef](./type_defs.md#serverreplicationconfigurationtypedef) [:material-code-braces: ServerReplicationConfigurationOutputTypeDef](./type_defs.md#serverreplicationconfigurationoutputtypedef) 
## GetAppValidationConfigurationResponseTypeDef

```python
# GetAppValidationConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppValidationConfigurationResponseTypeDef


def get_value() -> GetAppValidationConfigurationResponseTypeDef:
    return {
        "appValidationConfigurations": ...,
    }


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
# GetAppValidationOutputResponseTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import GetAppValidationOutputResponseTypeDef


def get_value() -> GetAppValidationOutputResponseTypeDef:
    return {
        "validationOutputList": ...,
    }


# GetAppValidationOutputResponseTypeDef definition

class GetAppValidationOutputResponseTypeDef(TypedDict):
    validationOutputList: List[ValidationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ValidationOutputTypeDef](./type_defs.md#validationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAppLaunchConfigurationRequestTypeDef

```python
# PutAppLaunchConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import PutAppLaunchConfigurationRequestTypeDef


def get_value() -> PutAppLaunchConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# PutAppLaunchConfigurationRequestTypeDef definition

class PutAppLaunchConfigurationRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    roleName: NotRequired[str],
    autoLaunch: NotRequired[bool],
    serverGroupLaunchConfigurations: NotRequired[Sequence[ServerGroupLaunchConfigurationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerGroupLaunchConfigurationTypeDef](./type_defs.md#servergrouplaunchconfigurationtypedef) [:material-code-braces: ServerGroupLaunchConfigurationOutputTypeDef](./type_defs.md#servergrouplaunchconfigurationoutputtypedef) 
## PutAppValidationConfigurationRequestTypeDef

```python
# PutAppValidationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import PutAppValidationConfigurationRequestTypeDef


def get_value() -> PutAppValidationConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# PutAppValidationConfigurationRequestTypeDef definition

class PutAppValidationConfigurationRequestTypeDef(TypedDict):
    appId: str,
    appValidationConfigurations: NotRequired[Sequence[AppValidationConfigurationTypeDef]],  # (1)
    serverGroupValidationConfigurations: NotRequired[Sequence[ServerGroupValidationConfigurationUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: AppValidationConfigurationTypeDef](./type_defs.md#appvalidationconfigurationtypedef) 
2. See [:material-code-braces: ServerGroupValidationConfigurationTypeDef](./type_defs.md#servergroupvalidationconfigurationtypedef) [:material-code-braces: ServerGroupValidationConfigurationOutputTypeDef](./type_defs.md#servergroupvalidationconfigurationoutputtypedef) 
## PutAppReplicationConfigurationRequestTypeDef

```python
# PutAppReplicationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_sms.type_defs import PutAppReplicationConfigurationRequestTypeDef


def get_value() -> PutAppReplicationConfigurationRequestTypeDef:
    return {
        "appId": ...,
    }


# PutAppReplicationConfigurationRequestTypeDef definition

class PutAppReplicationConfigurationRequestTypeDef(TypedDict):
    appId: NotRequired[str],
    serverGroupReplicationConfigurations: NotRequired[Sequence[ServerGroupReplicationConfigurationUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: ServerGroupReplicationConfigurationTypeDef](./type_defs.md#servergroupreplicationconfigurationtypedef) [:material-code-braces: ServerGroupReplicationConfigurationOutputTypeDef](./type_defs.md#servergroupreplicationconfigurationoutputtypedef) 

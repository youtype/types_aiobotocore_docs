# Type definitions

> [Index](../README.md) > [ManagedintegrationsforIoTDeviceManagement](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ManagedintegrationsforIoTDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-managed-integrations.html#managedintegrationsforiotdevicemanagement)
    type annotations stubs module [types-aiobotocore-iot-managed-integrations](https://pypi.org/project/types-aiobotocore-iot-managed-integrations/).

## OtaTaskExecutionRetryConfigUnionTypeDef

```python
# OtaTaskExecutionRetryConfigUnionTypeDef Union usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskExecutionRetryConfigUnionTypeDef


def get_value() -> OtaTaskExecutionRetryConfigUnionTypeDef:
    return ...


# OtaTaskExecutionRetryConfigUnionTypeDef definition

OtaTaskExecutionRetryConfigUnionTypeDef = Union[
    OtaTaskExecutionRetryConfigTypeDef,  # (1)
    OtaTaskExecutionRetryConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OtaTaskExecutionRetryConfigTypeDef](./type_defs.md#otataskexecutionretryconfigtypedef)
2. See [:material-code-braces: OtaTaskExecutionRetryConfigOutputTypeDef](./type_defs.md#otataskexecutionretryconfigoutputtypedef)

## OtaTaskSchedulingConfigUnionTypeDef

```python
# OtaTaskSchedulingConfigUnionTypeDef Union usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskSchedulingConfigUnionTypeDef


def get_value() -> OtaTaskSchedulingConfigUnionTypeDef:
    return ...


# OtaTaskSchedulingConfigUnionTypeDef definition

OtaTaskSchedulingConfigUnionTypeDef = Union[
    OtaTaskSchedulingConfigTypeDef,  # (1)
    OtaTaskSchedulingConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OtaTaskSchedulingConfigTypeDef](./type_defs.md#otataskschedulingconfigtypedef)
2. See [:material-code-braces: OtaTaskSchedulingConfigOutputTypeDef](./type_defs.md#otataskschedulingconfigoutputtypedef)

## CapabilityReportUnionTypeDef

```python
# CapabilityReportUnionTypeDef Union usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CapabilityReportUnionTypeDef


def get_value() -> CapabilityReportUnionTypeDef:
    return ...


# CapabilityReportUnionTypeDef definition

CapabilityReportUnionTypeDef = Union[
    CapabilityReportTypeDef,  # (1)
    CapabilityReportOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: CapabilityReportTypeDef](./type_defs.md#capabilityreporttypedef)
2. See [:material-code-braces: CapabilityReportOutputTypeDef](./type_defs.md#capabilityreportoutputtypedef)

## PushConfigUnionTypeDef

```python
# PushConfigUnionTypeDef Union usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PushConfigUnionTypeDef


def get_value() -> PushConfigUnionTypeDef:
    return ...


# PushConfigUnionTypeDef definition

PushConfigUnionTypeDef = Union[
    PushConfigTypeDef,  # (1)
    PushConfigOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PushConfigTypeDef](./type_defs.md#pushconfigtypedef)
2. See [:material-code-braces: PushConfigOutputTypeDef](./type_defs.md#pushconfigoutputtypedef)



## AbortConfigCriteriaTypeDef

```python
# AbortConfigCriteriaTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import AbortConfigCriteriaTypeDef


def get_value() -> AbortConfigCriteriaTypeDef:
    return {
        "Action": ...,
    }


# AbortConfigCriteriaTypeDef definition

class AbortConfigCriteriaTypeDef(TypedDict):
    Action: NotRequired[AbortCriteriaActionType],  # (1)
    FailureType: NotRequired[AbortCriteriaFailureTypeType],  # (2)
    MinNumberOfExecutedThings: NotRequired[int],
    ThresholdPercentage: NotRequired[float],
```

1. See [:material-code-brackets: AbortCriteriaActionType](./literals.md#abortcriteriaactiontype)
2. See [:material-code-brackets: AbortCriteriaFailureTypeType](./literals.md#abortcriteriafailuretypetype)

## CapabilityActionTypeDef

```python
# CapabilityActionTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CapabilityActionTypeDef


def get_value() -> CapabilityActionTypeDef:
    return {
        "name": ...,
    }


# CapabilityActionTypeDef definition

class CapabilityActionTypeDef(TypedDict):
    name: str,
    ref: NotRequired[str],
    actionTraceId: NotRequired[str],
    parameters: NotRequired[Mapping[str, Any]],
```


## CapabilityReportCapabilityOutputTypeDef

```python
# CapabilityReportCapabilityOutputTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CapabilityReportCapabilityOutputTypeDef


def get_value() -> CapabilityReportCapabilityOutputTypeDef:
    return {
        "id": ...,
    }


# CapabilityReportCapabilityOutputTypeDef definition

class CapabilityReportCapabilityOutputTypeDef(TypedDict):
    id: str,
    name: str,
    version: str,
    properties: List[str],
    actions: List[str],
    events: List[str],
```


## CapabilityReportCapabilityTypeDef

```python
# CapabilityReportCapabilityTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CapabilityReportCapabilityTypeDef


def get_value() -> CapabilityReportCapabilityTypeDef:
    return {
        "id": ...,
    }


# CapabilityReportCapabilityTypeDef definition

class CapabilityReportCapabilityTypeDef(TypedDict):
    id: str,
    name: str,
    version: str,
    properties: Sequence[str],
    actions: Sequence[str],
    events: Sequence[str],
```


## ConfigurationErrorTypeDef

```python
# ConfigurationErrorTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ConfigurationErrorTypeDef


def get_value() -> ConfigurationErrorTypeDef:
    return {
        "code": ...,
    }


# ConfigurationErrorTypeDef definition

class ConfigurationErrorTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```


## CreateCredentialLockerRequestTypeDef

```python
# CreateCredentialLockerRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateCredentialLockerRequestTypeDef


def get_value() -> CreateCredentialLockerRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateCredentialLockerRequestTypeDef definition

class CreateCredentialLockerRequestTypeDef(TypedDict):
    Name: NotRequired[str],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```


## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ResponseMetadataTypeDef


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


## CreateDestinationRequestTypeDef

```python
# CreateDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateDestinationRequestTypeDef


def get_value() -> CreateDestinationRequestTypeDef:
    return {
        "DeliveryDestinationArn": ...,
    }


# CreateDestinationRequestTypeDef definition

class CreateDestinationRequestTypeDef(TypedDict):
    DeliveryDestinationArn: str,
    DeliveryDestinationType: DeliveryDestinationTypeType,  # (1)
    Name: str,
    RoleArn: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype)

## CreateEventLogConfigurationRequestTypeDef

```python
# CreateEventLogConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateEventLogConfigurationRequestTypeDef


def get_value() -> CreateEventLogConfigurationRequestTypeDef:
    return {
        "ResourceType": ...,
    }


# CreateEventLogConfigurationRequestTypeDef definition

class CreateEventLogConfigurationRequestTypeDef(TypedDict):
    ResourceType: str,
    EventLogLevel: LogLevelType,  # (1)
    ResourceId: NotRequired[str],
    ClientToken: NotRequired[str],
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype)

## CreateNotificationConfigurationRequestTypeDef

```python
# CreateNotificationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateNotificationConfigurationRequestTypeDef


def get_value() -> CreateNotificationConfigurationRequestTypeDef:
    return {
        "EventType": ...,
    }


# CreateNotificationConfigurationRequestTypeDef definition

class CreateNotificationConfigurationRequestTypeDef(TypedDict):
    EventType: EventTypeType,  # (1)
    DestinationName: str,
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype)

## CreateProvisioningProfileRequestTypeDef

```python
# CreateProvisioningProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateProvisioningProfileRequestTypeDef


def get_value() -> CreateProvisioningProfileRequestTypeDef:
    return {
        "ProvisioningType": ...,
    }


# CreateProvisioningProfileRequestTypeDef definition

class CreateProvisioningProfileRequestTypeDef(TypedDict):
    ProvisioningType: ProvisioningTypeType,  # (1)
    CaCertificate: NotRequired[str],
    Name: NotRequired[str],
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ProvisioningTypeType](./literals.md#provisioningtypetype)

## CredentialLockerSummaryTypeDef

```python
# CredentialLockerSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CredentialLockerSummaryTypeDef


def get_value() -> CredentialLockerSummaryTypeDef:
    return {
        "Id": ...,
    }


# CredentialLockerSummaryTypeDef definition

class CredentialLockerSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    Name: NotRequired[str],
    CreatedAt: NotRequired[datetime.datetime],
```


## DeleteCredentialLockerRequestTypeDef

```python
# DeleteCredentialLockerRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DeleteCredentialLockerRequestTypeDef


def get_value() -> DeleteCredentialLockerRequestTypeDef:
    return {
        "Identifier": ...,
    }


# DeleteCredentialLockerRequestTypeDef definition

class DeleteCredentialLockerRequestTypeDef(TypedDict):
    Identifier: str,
```


## DeleteDestinationRequestTypeDef

```python
# DeleteDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DeleteDestinationRequestTypeDef


def get_value() -> DeleteDestinationRequestTypeDef:
    return {
        "Name": ...,
    }


# DeleteDestinationRequestTypeDef definition

class DeleteDestinationRequestTypeDef(TypedDict):
    Name: str,
```


## DeleteEventLogConfigurationRequestTypeDef

```python
# DeleteEventLogConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DeleteEventLogConfigurationRequestTypeDef


def get_value() -> DeleteEventLogConfigurationRequestTypeDef:
    return {
        "Id": ...,
    }


# DeleteEventLogConfigurationRequestTypeDef definition

class DeleteEventLogConfigurationRequestTypeDef(TypedDict):
    Id: str,
```


## DeleteManagedThingRequestTypeDef

```python
# DeleteManagedThingRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DeleteManagedThingRequestTypeDef


def get_value() -> DeleteManagedThingRequestTypeDef:
    return {
        "Identifier": ...,
    }


# DeleteManagedThingRequestTypeDef definition

class DeleteManagedThingRequestTypeDef(TypedDict):
    Identifier: str,
    Force: NotRequired[bool],
```


## DeleteNotificationConfigurationRequestTypeDef

```python
# DeleteNotificationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DeleteNotificationConfigurationRequestTypeDef


def get_value() -> DeleteNotificationConfigurationRequestTypeDef:
    return {
        "EventType": ...,
    }


# DeleteNotificationConfigurationRequestTypeDef definition

class DeleteNotificationConfigurationRequestTypeDef(TypedDict):
    EventType: EventTypeType,  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype)

## DeleteOtaTaskConfigurationRequestTypeDef

```python
# DeleteOtaTaskConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DeleteOtaTaskConfigurationRequestTypeDef


def get_value() -> DeleteOtaTaskConfigurationRequestTypeDef:
    return {
        "Identifier": ...,
    }


# DeleteOtaTaskConfigurationRequestTypeDef definition

class DeleteOtaTaskConfigurationRequestTypeDef(TypedDict):
    Identifier: str,
```


## DeleteOtaTaskRequestTypeDef

```python
# DeleteOtaTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DeleteOtaTaskRequestTypeDef


def get_value() -> DeleteOtaTaskRequestTypeDef:
    return {
        "Identifier": ...,
    }


# DeleteOtaTaskRequestTypeDef definition

class DeleteOtaTaskRequestTypeDef(TypedDict):
    Identifier: str,
```


## DeleteProvisioningProfileRequestTypeDef

```python
# DeleteProvisioningProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DeleteProvisioningProfileRequestTypeDef


def get_value() -> DeleteProvisioningProfileRequestTypeDef:
    return {
        "Identifier": ...,
    }


# DeleteProvisioningProfileRequestTypeDef definition

class DeleteProvisioningProfileRequestTypeDef(TypedDict):
    Identifier: str,
```


## DestinationSummaryTypeDef

```python
# DestinationSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import DestinationSummaryTypeDef


def get_value() -> DestinationSummaryTypeDef:
    return {
        "Description": ...,
    }


# DestinationSummaryTypeDef definition

class DestinationSummaryTypeDef(TypedDict):
    Description: NotRequired[str],
    DeliveryDestinationArn: NotRequired[str],
    DeliveryDestinationType: NotRequired[DeliveryDestinationTypeType],  # (1)
    Name: NotRequired[str],
    RoleArn: NotRequired[str],
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype)

## EventLogConfigurationSummaryTypeDef

```python
# EventLogConfigurationSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import EventLogConfigurationSummaryTypeDef


def get_value() -> EventLogConfigurationSummaryTypeDef:
    return {
        "Id": ...,
    }


# EventLogConfigurationSummaryTypeDef definition

class EventLogConfigurationSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    EventLogLevel: NotRequired[LogLevelType],  # (1)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype)

## RolloutRateIncreaseCriteriaTypeDef

```python
# RolloutRateIncreaseCriteriaTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import RolloutRateIncreaseCriteriaTypeDef


def get_value() -> RolloutRateIncreaseCriteriaTypeDef:
    return {
        "numberOfNotifiedThings": ...,
    }


# RolloutRateIncreaseCriteriaTypeDef definition

class RolloutRateIncreaseCriteriaTypeDef(TypedDict):
    numberOfNotifiedThings: NotRequired[int],
    numberOfSucceededThings: NotRequired[int],
```


## GetCredentialLockerRequestTypeDef

```python
# GetCredentialLockerRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetCredentialLockerRequestTypeDef


def get_value() -> GetCredentialLockerRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetCredentialLockerRequestTypeDef definition

class GetCredentialLockerRequestTypeDef(TypedDict):
    Identifier: str,
```


## GetDestinationRequestTypeDef

```python
# GetDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetDestinationRequestTypeDef


def get_value() -> GetDestinationRequestTypeDef:
    return {
        "Name": ...,
    }


# GetDestinationRequestTypeDef definition

class GetDestinationRequestTypeDef(TypedDict):
    Name: str,
```


## GetDeviceDiscoveryRequestTypeDef

```python
# GetDeviceDiscoveryRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetDeviceDiscoveryRequestTypeDef


def get_value() -> GetDeviceDiscoveryRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetDeviceDiscoveryRequestTypeDef definition

class GetDeviceDiscoveryRequestTypeDef(TypedDict):
    Identifier: str,
```


## GetEventLogConfigurationRequestTypeDef

```python
# GetEventLogConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetEventLogConfigurationRequestTypeDef


def get_value() -> GetEventLogConfigurationRequestTypeDef:
    return {
        "Id": ...,
    }


# GetEventLogConfigurationRequestTypeDef definition

class GetEventLogConfigurationRequestTypeDef(TypedDict):
    Id: str,
```


## GetManagedThingCapabilitiesRequestTypeDef

```python
# GetManagedThingCapabilitiesRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingCapabilitiesRequestTypeDef


def get_value() -> GetManagedThingCapabilitiesRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetManagedThingCapabilitiesRequestTypeDef definition

class GetManagedThingCapabilitiesRequestTypeDef(TypedDict):
    Identifier: str,
```


## GetManagedThingConnectivityDataRequestTypeDef

```python
# GetManagedThingConnectivityDataRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingConnectivityDataRequestTypeDef


def get_value() -> GetManagedThingConnectivityDataRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetManagedThingConnectivityDataRequestTypeDef definition

class GetManagedThingConnectivityDataRequestTypeDef(TypedDict):
    Identifier: str,
```


## GetManagedThingMetaDataRequestTypeDef

```python
# GetManagedThingMetaDataRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingMetaDataRequestTypeDef


def get_value() -> GetManagedThingMetaDataRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetManagedThingMetaDataRequestTypeDef definition

class GetManagedThingMetaDataRequestTypeDef(TypedDict):
    Identifier: str,
```


## GetManagedThingRequestTypeDef

```python
# GetManagedThingRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingRequestTypeDef


def get_value() -> GetManagedThingRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetManagedThingRequestTypeDef definition

class GetManagedThingRequestTypeDef(TypedDict):
    Identifier: str,
```


## GetManagedThingStateRequestTypeDef

```python
# GetManagedThingStateRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingStateRequestTypeDef


def get_value() -> GetManagedThingStateRequestTypeDef:
    return {
        "ManagedThingId": ...,
    }


# GetManagedThingStateRequestTypeDef definition

class GetManagedThingStateRequestTypeDef(TypedDict):
    ManagedThingId: str,
```


## GetNotificationConfigurationRequestTypeDef

```python
# GetNotificationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetNotificationConfigurationRequestTypeDef


def get_value() -> GetNotificationConfigurationRequestTypeDef:
    return {
        "EventType": ...,
    }


# GetNotificationConfigurationRequestTypeDef definition

class GetNotificationConfigurationRequestTypeDef(TypedDict):
    EventType: EventTypeType,  # (1)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype)

## GetOtaTaskConfigurationRequestTypeDef

```python
# GetOtaTaskConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetOtaTaskConfigurationRequestTypeDef


def get_value() -> GetOtaTaskConfigurationRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetOtaTaskConfigurationRequestTypeDef definition

class GetOtaTaskConfigurationRequestTypeDef(TypedDict):
    Identifier: str,
```


## GetOtaTaskRequestTypeDef

```python
# GetOtaTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetOtaTaskRequestTypeDef


def get_value() -> GetOtaTaskRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetOtaTaskRequestTypeDef definition

class GetOtaTaskRequestTypeDef(TypedDict):
    Identifier: str,
```


## TaskProcessingDetailsTypeDef

```python
# TaskProcessingDetailsTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import TaskProcessingDetailsTypeDef


def get_value() -> TaskProcessingDetailsTypeDef:
    return {
        "NumberOfCanceledThings": ...,
    }


# TaskProcessingDetailsTypeDef definition

class TaskProcessingDetailsTypeDef(TypedDict):
    NumberOfCanceledThings: NotRequired[int],
    NumberOfFailedThings: NotRequired[int],
    NumberOfInProgressThings: NotRequired[int],
    numberOfQueuedThings: NotRequired[int],
    numberOfRejectedThings: NotRequired[int],
    numberOfRemovedThings: NotRequired[int],
    numberOfSucceededThings: NotRequired[int],
    numberOfTimedOutThings: NotRequired[int],
    processingTargets: NotRequired[List[str]],
```


## GetProvisioningProfileRequestTypeDef

```python
# GetProvisioningProfileRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetProvisioningProfileRequestTypeDef


def get_value() -> GetProvisioningProfileRequestTypeDef:
    return {
        "Identifier": ...,
    }


# GetProvisioningProfileRequestTypeDef definition

class GetProvisioningProfileRequestTypeDef(TypedDict):
    Identifier: str,
```


## GetRuntimeLogConfigurationRequestTypeDef

```python
# GetRuntimeLogConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetRuntimeLogConfigurationRequestTypeDef


def get_value() -> GetRuntimeLogConfigurationRequestTypeDef:
    return {
        "ManagedThingId": ...,
    }


# GetRuntimeLogConfigurationRequestTypeDef definition

class GetRuntimeLogConfigurationRequestTypeDef(TypedDict):
    ManagedThingId: str,
```


## RuntimeLogConfigurationsTypeDef

```python
# RuntimeLogConfigurationsTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import RuntimeLogConfigurationsTypeDef


def get_value() -> RuntimeLogConfigurationsTypeDef:
    return {
        "LogLevel": ...,
    }


# RuntimeLogConfigurationsTypeDef definition

class RuntimeLogConfigurationsTypeDef(TypedDict):
    LogLevel: NotRequired[LogLevelType],  # (1)
    LogFlushLevel: NotRequired[LogLevelType],  # (1)
    LocalStoreLocation: NotRequired[str],
    LocalStoreFileRotationMaxFiles: NotRequired[int],
    LocalStoreFileRotationMaxBytes: NotRequired[int],
    UploadLog: NotRequired[bool],
    UploadPeriodMinutes: NotRequired[int],
    DeleteLocalStoreAfterUpload: NotRequired[bool],
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype)
2. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype)

## GetSchemaVersionRequestTypeDef

```python
# GetSchemaVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetSchemaVersionRequestTypeDef


def get_value() -> GetSchemaVersionRequestTypeDef:
    return {
        "Type": ...,
    }


# GetSchemaVersionRequestTypeDef definition

class GetSchemaVersionRequestTypeDef(TypedDict):
    Type: SchemaVersionTypeType,  # (1)
    SchemaVersionedId: str,
    Format: NotRequired[SchemaVersionFormatType],  # (2)
```

1. See [:material-code-brackets: SchemaVersionTypeType](./literals.md#schemaversiontypetype)
2. See [:material-code-brackets: SchemaVersionFormatType](./literals.md#schemaversionformattype)

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PaginatorConfigTypeDef


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


## ListCredentialLockersRequestTypeDef

```python
# ListCredentialLockersRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListCredentialLockersRequestTypeDef


def get_value() -> ListCredentialLockersRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListCredentialLockersRequestTypeDef definition

class ListCredentialLockersRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```


## ListDestinationsRequestTypeDef

```python
# ListDestinationsRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListDestinationsRequestTypeDef


def get_value() -> ListDestinationsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListDestinationsRequestTypeDef definition

class ListDestinationsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```


## ListEventLogConfigurationsRequestTypeDef

```python
# ListEventLogConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListEventLogConfigurationsRequestTypeDef


def get_value() -> ListEventLogConfigurationsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListEventLogConfigurationsRequestTypeDef definition

class ListEventLogConfigurationsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```


## ListManagedThingSchemasRequestTypeDef

```python
# ListManagedThingSchemasRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListManagedThingSchemasRequestTypeDef


def get_value() -> ListManagedThingSchemasRequestTypeDef:
    return {
        "Identifier": ...,
    }


# ListManagedThingSchemasRequestTypeDef definition

class ListManagedThingSchemasRequestTypeDef(TypedDict):
    Identifier: str,
    EndpointIdFilter: NotRequired[str],
    CapabilityIdFilter: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```


## ManagedThingSchemaListItemTypeDef

```python
# ManagedThingSchemaListItemTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ManagedThingSchemaListItemTypeDef


def get_value() -> ManagedThingSchemaListItemTypeDef:
    return {
        "EndpointId": ...,
    }


# ManagedThingSchemaListItemTypeDef definition

class ManagedThingSchemaListItemTypeDef(TypedDict):
    EndpointId: NotRequired[str],
    CapabilityId: NotRequired[str],
    Schema: NotRequired[Dict[str, Any]],
```


## ListManagedThingsRequestTypeDef

```python
# ListManagedThingsRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListManagedThingsRequestTypeDef


def get_value() -> ListManagedThingsRequestTypeDef:
    return {
        "OwnerFilter": ...,
    }


# ListManagedThingsRequestTypeDef definition

class ListManagedThingsRequestTypeDef(TypedDict):
    OwnerFilter: NotRequired[str],
    CredentialLockerFilter: NotRequired[str],
    RoleFilter: NotRequired[RoleType],  # (1)
    ParentControllerIdentifierFilter: NotRequired[str],
    ConnectorPolicyIdFilter: NotRequired[str],
    SerialNumberFilter: NotRequired[str],
    ProvisioningStatusFilter: NotRequired[ProvisioningStatusType],  # (2)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype)
2. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype)

## ManagedThingSummaryTypeDef

```python
# ManagedThingSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ManagedThingSummaryTypeDef


def get_value() -> ManagedThingSummaryTypeDef:
    return {
        "Id": ...,
    }


# ManagedThingSummaryTypeDef definition

class ManagedThingSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Arn: NotRequired[str],
    AdvertisedProductId: NotRequired[str],
    Brand: NotRequired[str],
    Classification: NotRequired[str],
    ConnectorDeviceId: NotRequired[str],
    ConnectorPolicyId: NotRequired[str],
    Model: NotRequired[str],
    Name: NotRequired[str],
    Owner: NotRequired[str],
    CredentialLockerId: NotRequired[str],
    ParentControllerId: NotRequired[str],
    ProvisioningStatus: NotRequired[ProvisioningStatusType],  # (1)
    Role: NotRequired[RoleType],  # (2)
    SerialNumber: NotRequired[str],
    CreatedAt: NotRequired[datetime.datetime],
    UpdatedAt: NotRequired[datetime.datetime],
    ActivatedAt: NotRequired[datetime.datetime],
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype)
2. See [:material-code-brackets: RoleType](./literals.md#roletype)

## ListNotificationConfigurationsRequestTypeDef

```python
# ListNotificationConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListNotificationConfigurationsRequestTypeDef


def get_value() -> ListNotificationConfigurationsRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListNotificationConfigurationsRequestTypeDef definition

class ListNotificationConfigurationsRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```


## NotificationConfigurationSummaryTypeDef

```python
# NotificationConfigurationSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import NotificationConfigurationSummaryTypeDef


def get_value() -> NotificationConfigurationSummaryTypeDef:
    return {
        "EventType": ...,
    }


# NotificationConfigurationSummaryTypeDef definition

class NotificationConfigurationSummaryTypeDef(TypedDict):
    EventType: NotRequired[EventTypeType],  # (1)
    DestinationName: NotRequired[str],
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype)

## ListOtaTaskConfigurationsRequestTypeDef

```python
# ListOtaTaskConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTaskConfigurationsRequestTypeDef


def get_value() -> ListOtaTaskConfigurationsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListOtaTaskConfigurationsRequestTypeDef definition

class ListOtaTaskConfigurationsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```


## OtaTaskConfigurationSummaryTypeDef

```python
# OtaTaskConfigurationSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskConfigurationSummaryTypeDef


def get_value() -> OtaTaskConfigurationSummaryTypeDef:
    return {
        "TaskConfigurationId": ...,
    }


# OtaTaskConfigurationSummaryTypeDef definition

class OtaTaskConfigurationSummaryTypeDef(TypedDict):
    TaskConfigurationId: NotRequired[str],
    Name: NotRequired[str],
    CreatedAt: NotRequired[datetime.datetime],
```


## ListOtaTaskExecutionsRequestTypeDef

```python
# ListOtaTaskExecutionsRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTaskExecutionsRequestTypeDef


def get_value() -> ListOtaTaskExecutionsRequestTypeDef:
    return {
        "Identifier": ...,
    }


# ListOtaTaskExecutionsRequestTypeDef definition

class ListOtaTaskExecutionsRequestTypeDef(TypedDict):
    Identifier: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```


## ListOtaTasksRequestTypeDef

```python
# ListOtaTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTasksRequestTypeDef


def get_value() -> ListOtaTasksRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListOtaTasksRequestTypeDef definition

class ListOtaTasksRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```


## OtaTaskSummaryTypeDef

```python
# OtaTaskSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskSummaryTypeDef


def get_value() -> OtaTaskSummaryTypeDef:
    return {
        "TaskId": ...,
    }


# OtaTaskSummaryTypeDef definition

class OtaTaskSummaryTypeDef(TypedDict):
    TaskId: NotRequired[str],
    TaskArn: NotRequired[str],
    CreatedAt: NotRequired[datetime.datetime],
    LastUpdatedAt: NotRequired[datetime.datetime],
    TaskConfigurationId: NotRequired[str],
    Status: NotRequired[OtaStatusType],  # (1)
```

1. See [:material-code-brackets: OtaStatusType](./literals.md#otastatustype)

## ListProvisioningProfilesRequestTypeDef

```python
# ListProvisioningProfilesRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListProvisioningProfilesRequestTypeDef


def get_value() -> ListProvisioningProfilesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListProvisioningProfilesRequestTypeDef definition

class ListProvisioningProfilesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```


## ProvisioningProfileSummaryTypeDef

```python
# ProvisioningProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ProvisioningProfileSummaryTypeDef


def get_value() -> ProvisioningProfileSummaryTypeDef:
    return {
        "Name": ...,
    }


# ProvisioningProfileSummaryTypeDef definition

class ProvisioningProfileSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    Id: NotRequired[str],
    Arn: NotRequired[str],
    ProvisioningType: NotRequired[ProvisioningTypeType],  # (1)
```

1. See [:material-code-brackets: ProvisioningTypeType](./literals.md#provisioningtypetype)

## ListSchemaVersionsRequestTypeDef

```python
# ListSchemaVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListSchemaVersionsRequestTypeDef


def get_value() -> ListSchemaVersionsRequestTypeDef:
    return {
        "Type": ...,
    }


# ListSchemaVersionsRequestTypeDef definition

class ListSchemaVersionsRequestTypeDef(TypedDict):
    Type: SchemaVersionTypeType,  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    SchemaId: NotRequired[str],
    Namespace: NotRequired[str],
    Visibility: NotRequired[SchemaVersionVisibilityType],  # (2)
    SemanticVersion: NotRequired[str],
```

1. See [:material-code-brackets: SchemaVersionTypeType](./literals.md#schemaversiontypetype)
2. See [:material-code-brackets: SchemaVersionVisibilityType](./literals.md#schemaversionvisibilitytype)

## SchemaVersionListItemTypeDef

```python
# SchemaVersionListItemTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import SchemaVersionListItemTypeDef


def get_value() -> SchemaVersionListItemTypeDef:
    return {
        "SchemaId": ...,
    }


# SchemaVersionListItemTypeDef definition

class SchemaVersionListItemTypeDef(TypedDict):
    SchemaId: NotRequired[str],
    Type: NotRequired[SchemaVersionTypeType],  # (1)
    Description: NotRequired[str],
    Namespace: NotRequired[str],
    SemanticVersion: NotRequired[str],
    Visibility: NotRequired[SchemaVersionVisibilityType],  # (2)
```

1. See [:material-code-brackets: SchemaVersionTypeType](./literals.md#schemaversiontypetype)
2. See [:material-code-brackets: SchemaVersionVisibilityType](./literals.md#schemaversionvisibilitytype)

## RetryConfigCriteriaTypeDef

```python
# RetryConfigCriteriaTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import RetryConfigCriteriaTypeDef


def get_value() -> RetryConfigCriteriaTypeDef:
    return {
        "FailureType": ...,
    }


# RetryConfigCriteriaTypeDef definition

class RetryConfigCriteriaTypeDef(TypedDict):
    FailureType: NotRequired[RetryCriteriaFailureTypeType],  # (1)
    MinNumberOfRetries: NotRequired[int],
```

1. See [:material-code-brackets: RetryCriteriaFailureTypeType](./literals.md#retrycriteriafailuretypetype)

## OtaTaskExecutionSummaryTypeDef

```python
# OtaTaskExecutionSummaryTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskExecutionSummaryTypeDef


def get_value() -> OtaTaskExecutionSummaryTypeDef:
    return {
        "ExecutionNumber": ...,
    }


# OtaTaskExecutionSummaryTypeDef definition

class OtaTaskExecutionSummaryTypeDef(TypedDict):
    ExecutionNumber: NotRequired[int],
    LastUpdatedAt: NotRequired[datetime.datetime],
    QueuedAt: NotRequired[datetime.datetime],
    RetryAttempt: NotRequired[int],
    StartedAt: NotRequired[datetime.datetime],
    Status: NotRequired[OtaTaskExecutionStatusType],  # (1)
```

1. See [:material-code-brackets: OtaTaskExecutionStatusType](./literals.md#otataskexecutionstatustype)

## ScheduleMaintenanceWindowTypeDef

```python
# ScheduleMaintenanceWindowTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ScheduleMaintenanceWindowTypeDef


def get_value() -> ScheduleMaintenanceWindowTypeDef:
    return {
        "DurationInMinutes": ...,
    }


# ScheduleMaintenanceWindowTypeDef definition

class ScheduleMaintenanceWindowTypeDef(TypedDict):
    DurationInMinutes: NotRequired[int],
    StartTime: NotRequired[str],
```


## OtaTaskTimeoutConfigTypeDef

```python
# OtaTaskTimeoutConfigTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskTimeoutConfigTypeDef


def get_value() -> OtaTaskTimeoutConfigTypeDef:
    return {
        "InProgressTimeoutInMinutes": ...,
    }


# OtaTaskTimeoutConfigTypeDef definition

class OtaTaskTimeoutConfigTypeDef(TypedDict):
    InProgressTimeoutInMinutes: NotRequired[int],
```


## PutDefaultEncryptionConfigurationRequestTypeDef

```python
# PutDefaultEncryptionConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PutDefaultEncryptionConfigurationRequestTypeDef


def get_value() -> PutDefaultEncryptionConfigurationRequestTypeDef:
    return {
        "encryptionType": ...,
    }


# PutDefaultEncryptionConfigurationRequestTypeDef definition

class PutDefaultEncryptionConfigurationRequestTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype)

## PutHubConfigurationRequestTypeDef

```python
# PutHubConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PutHubConfigurationRequestTypeDef


def get_value() -> PutHubConfigurationRequestTypeDef:
    return {
        "HubTokenTimerExpirySettingInSeconds": ...,
    }


# PutHubConfigurationRequestTypeDef definition

class PutHubConfigurationRequestTypeDef(TypedDict):
    HubTokenTimerExpirySettingInSeconds: int,
```


## ResetRuntimeLogConfigurationRequestTypeDef

```python
# ResetRuntimeLogConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ResetRuntimeLogConfigurationRequestTypeDef


def get_value() -> ResetRuntimeLogConfigurationRequestTypeDef:
    return {
        "ManagedThingId": ...,
    }


# ResetRuntimeLogConfigurationRequestTypeDef definition

class ResetRuntimeLogConfigurationRequestTypeDef(TypedDict):
    ManagedThingId: str,
```


## StartDeviceDiscoveryRequestTypeDef

```python
# StartDeviceDiscoveryRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import StartDeviceDiscoveryRequestTypeDef


def get_value() -> StartDeviceDiscoveryRequestTypeDef:
    return {
        "DiscoveryType": ...,
    }


# StartDeviceDiscoveryRequestTypeDef definition

class StartDeviceDiscoveryRequestTypeDef(TypedDict):
    DiscoveryType: DiscoveryTypeType,  # (1)
    ControllerIdentifier: NotRequired[str],
    ConnectorAssociationIdentifier: NotRequired[str],
    AuthenticationMaterial: NotRequired[str],
    AuthenticationMaterialType: NotRequired[DiscoveryAuthMaterialTypeType],  # (2)
    ClientToken: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DiscoveryTypeType](./literals.md#discoverytypetype)
2. See [:material-code-brackets: DiscoveryAuthMaterialTypeType](./literals.md#discoveryauthmaterialtypetype)

## StateCapabilityTypeDef

```python
# StateCapabilityTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import StateCapabilityTypeDef


def get_value() -> StateCapabilityTypeDef:
    return {
        "id": ...,
    }


# StateCapabilityTypeDef definition

class StateCapabilityTypeDef(TypedDict):
    id: str,
    name: str,
    version: str,
    properties: NotRequired[Dict[str, Any]],
```


## UpdateDestinationRequestTypeDef

```python
# UpdateDestinationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import UpdateDestinationRequestTypeDef


def get_value() -> UpdateDestinationRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateDestinationRequestTypeDef definition

class UpdateDestinationRequestTypeDef(TypedDict):
    Name: str,
    DeliveryDestinationArn: NotRequired[str],
    DeliveryDestinationType: NotRequired[DeliveryDestinationTypeType],  # (1)
    RoleArn: NotRequired[str],
    Description: NotRequired[str],
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype)

## UpdateEventLogConfigurationRequestTypeDef

```python
# UpdateEventLogConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import UpdateEventLogConfigurationRequestTypeDef


def get_value() -> UpdateEventLogConfigurationRequestTypeDef:
    return {
        "Id": ...,
    }


# UpdateEventLogConfigurationRequestTypeDef definition

class UpdateEventLogConfigurationRequestTypeDef(TypedDict):
    Id: str,
    EventLogLevel: LogLevelType,  # (1)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype)

## UpdateNotificationConfigurationRequestTypeDef

```python
# UpdateNotificationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import UpdateNotificationConfigurationRequestTypeDef


def get_value() -> UpdateNotificationConfigurationRequestTypeDef:
    return {
        "EventType": ...,
    }


# UpdateNotificationConfigurationRequestTypeDef definition

class UpdateNotificationConfigurationRequestTypeDef(TypedDict):
    EventType: EventTypeType,  # (1)
    DestinationName: str,
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype)

## UpdateOtaTaskRequestTypeDef

```python
# UpdateOtaTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import UpdateOtaTaskRequestTypeDef


def get_value() -> UpdateOtaTaskRequestTypeDef:
    return {
        "Identifier": ...,
    }


# UpdateOtaTaskRequestTypeDef definition

class UpdateOtaTaskRequestTypeDef(TypedDict):
    Identifier: str,
    Description: NotRequired[str],
    TaskConfigurationId: NotRequired[str],
```


## OtaTaskAbortConfigOutputTypeDef

```python
# OtaTaskAbortConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskAbortConfigOutputTypeDef


def get_value() -> OtaTaskAbortConfigOutputTypeDef:
    return {
        "AbortConfigCriteriaList": ...,
    }


# OtaTaskAbortConfigOutputTypeDef definition

class OtaTaskAbortConfigOutputTypeDef(TypedDict):
    AbortConfigCriteriaList: NotRequired[List[AbortConfigCriteriaTypeDef]],  # (1)
```

1. See `List[AbortConfigCriteriaTypeDef]`

## OtaTaskAbortConfigTypeDef

```python
# OtaTaskAbortConfigTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskAbortConfigTypeDef


def get_value() -> OtaTaskAbortConfigTypeDef:
    return {
        "AbortConfigCriteriaList": ...,
    }


# OtaTaskAbortConfigTypeDef definition

class OtaTaskAbortConfigTypeDef(TypedDict):
    AbortConfigCriteriaList: NotRequired[Sequence[AbortConfigCriteriaTypeDef]],  # (1)
```

1. See `Sequence[AbortConfigCriteriaTypeDef]`

## CommandCapabilityTypeDef

```python
# CommandCapabilityTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CommandCapabilityTypeDef


def get_value() -> CommandCapabilityTypeDef:
    return {
        "id": ...,
    }


# CommandCapabilityTypeDef definition

class CommandCapabilityTypeDef(TypedDict):
    id: str,
    name: str,
    version: str,
    actions: Sequence[CapabilityActionTypeDef],  # (1)
```

1. See `Sequence[CapabilityActionTypeDef]`

## CapabilityReportEndpointOutputTypeDef

```python
# CapabilityReportEndpointOutputTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CapabilityReportEndpointOutputTypeDef


def get_value() -> CapabilityReportEndpointOutputTypeDef:
    return {
        "id": ...,
    }


# CapabilityReportEndpointOutputTypeDef definition

class CapabilityReportEndpointOutputTypeDef(TypedDict):
    id: str,
    deviceTypes: List[str],
    capabilities: List[CapabilityReportCapabilityOutputTypeDef],  # (1)
```

1. See `List[CapabilityReportCapabilityOutputTypeDef]`

## CapabilityReportEndpointTypeDef

```python
# CapabilityReportEndpointTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CapabilityReportEndpointTypeDef


def get_value() -> CapabilityReportEndpointTypeDef:
    return {
        "id": ...,
    }


# CapabilityReportEndpointTypeDef definition

class CapabilityReportEndpointTypeDef(TypedDict):
    id: str,
    deviceTypes: Sequence[str],
    capabilities: Sequence[CapabilityReportCapabilityTypeDef],  # (1)
```

1. See `Sequence[CapabilityReportCapabilityTypeDef]`

## ConfigurationStatusTypeDef

```python
# ConfigurationStatusTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ConfigurationStatusTypeDef


def get_value() -> ConfigurationStatusTypeDef:
    return {
        "error": ...,
    }


# ConfigurationStatusTypeDef definition

class ConfigurationStatusTypeDef(TypedDict):
    state: ConfigurationStateType,  # (2)
    error: NotRequired[ConfigurationErrorTypeDef],  # (1)
```

1. See [:material-code-braces: ConfigurationErrorTypeDef](./type_defs.md#configurationerrortypedef)
2. See [:material-code-brackets: ConfigurationStateType](./literals.md#configurationstatetype)

## CreateCredentialLockerResponseTypeDef

```python
# CreateCredentialLockerResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateCredentialLockerResponseTypeDef


def get_value() -> CreateCredentialLockerResponseTypeDef:
    return {
        "Id": ...,
    }


# CreateCredentialLockerResponseTypeDef definition

class CreateCredentialLockerResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    CreatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateDestinationResponseTypeDef

```python
# CreateDestinationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateDestinationResponseTypeDef


def get_value() -> CreateDestinationResponseTypeDef:
    return {
        "Name": ...,
    }


# CreateDestinationResponseTypeDef definition

class CreateDestinationResponseTypeDef(TypedDict):
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateEventLogConfigurationResponseTypeDef

```python
# CreateEventLogConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateEventLogConfigurationResponseTypeDef


def get_value() -> CreateEventLogConfigurationResponseTypeDef:
    return {
        "Id": ...,
    }


# CreateEventLogConfigurationResponseTypeDef definition

class CreateEventLogConfigurationResponseTypeDef(TypedDict):
    Id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateManagedThingResponseTypeDef

```python
# CreateManagedThingResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateManagedThingResponseTypeDef


def get_value() -> CreateManagedThingResponseTypeDef:
    return {
        "Id": ...,
    }


# CreateManagedThingResponseTypeDef definition

class CreateManagedThingResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    CreatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateNotificationConfigurationResponseTypeDef

```python
# CreateNotificationConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateNotificationConfigurationResponseTypeDef


def get_value() -> CreateNotificationConfigurationResponseTypeDef:
    return {
        "EventType": ...,
    }


# CreateNotificationConfigurationResponseTypeDef definition

class CreateNotificationConfigurationResponseTypeDef(TypedDict):
    EventType: EventTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateOtaTaskConfigurationResponseTypeDef

```python
# CreateOtaTaskConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateOtaTaskConfigurationResponseTypeDef


def get_value() -> CreateOtaTaskConfigurationResponseTypeDef:
    return {
        "TaskConfigurationId": ...,
    }


# CreateOtaTaskConfigurationResponseTypeDef definition

class CreateOtaTaskConfigurationResponseTypeDef(TypedDict):
    TaskConfigurationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateOtaTaskResponseTypeDef

```python
# CreateOtaTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateOtaTaskResponseTypeDef


def get_value() -> CreateOtaTaskResponseTypeDef:
    return {
        "TaskId": ...,
    }


# CreateOtaTaskResponseTypeDef definition

class CreateOtaTaskResponseTypeDef(TypedDict):
    TaskId: str,
    TaskArn: str,
    Description: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateProvisioningProfileResponseTypeDef

```python
# CreateProvisioningProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateProvisioningProfileResponseTypeDef


def get_value() -> CreateProvisioningProfileResponseTypeDef:
    return {
        "Arn": ...,
    }


# CreateProvisioningProfileResponseTypeDef definition

class CreateProvisioningProfileResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    ProvisioningType: ProvisioningTypeType,  # (1)
    Id: str,
    ClaimCertificate: str,
    ClaimCertificatePrivateKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProvisioningTypeType](./literals.md#provisioningtypetype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetCredentialLockerResponseTypeDef

```python
# GetCredentialLockerResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetCredentialLockerResponseTypeDef


def get_value() -> GetCredentialLockerResponseTypeDef:
    return {
        "Id": ...,
    }


# GetCredentialLockerResponseTypeDef definition

class GetCredentialLockerResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    Name: str,
    CreatedAt: datetime.datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetCustomEndpointResponseTypeDef

```python
# GetCustomEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetCustomEndpointResponseTypeDef


def get_value() -> GetCustomEndpointResponseTypeDef:
    return {
        "EndpointAddress": ...,
    }


# GetCustomEndpointResponseTypeDef definition

class GetCustomEndpointResponseTypeDef(TypedDict):
    EndpointAddress: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetDestinationResponseTypeDef

```python
# GetDestinationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetDestinationResponseTypeDef


def get_value() -> GetDestinationResponseTypeDef:
    return {
        "Description": ...,
    }


# GetDestinationResponseTypeDef definition

class GetDestinationResponseTypeDef(TypedDict):
    Description: str,
    DeliveryDestinationArn: str,
    DeliveryDestinationType: DeliveryDestinationTypeType,  # (1)
    Name: str,
    RoleArn: str,
    CreatedAt: datetime.datetime,
    UpdatedAt: datetime.datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeliveryDestinationTypeType](./literals.md#deliverydestinationtypetype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetDeviceDiscoveryResponseTypeDef

```python
# GetDeviceDiscoveryResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetDeviceDiscoveryResponseTypeDef


def get_value() -> GetDeviceDiscoveryResponseTypeDef:
    return {
        "Id": ...,
    }


# GetDeviceDiscoveryResponseTypeDef definition

class GetDeviceDiscoveryResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    DiscoveryType: DiscoveryTypeType,  # (1)
    Status: DeviceDiscoveryStatusType,  # (2)
    StartedAt: datetime.datetime,
    ControllerId: str,
    ConnectorAssociationId: str,
    FinishedAt: datetime.datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: DiscoveryTypeType](./literals.md#discoverytypetype)
2. See [:material-code-brackets: DeviceDiscoveryStatusType](./literals.md#devicediscoverystatustype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetEventLogConfigurationResponseTypeDef

```python
# GetEventLogConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetEventLogConfigurationResponseTypeDef


def get_value() -> GetEventLogConfigurationResponseTypeDef:
    return {
        "Id": ...,
    }


# GetEventLogConfigurationResponseTypeDef definition

class GetEventLogConfigurationResponseTypeDef(TypedDict):
    Id: str,
    ResourceType: str,
    ResourceId: str,
    EventLogLevel: LogLevelType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LogLevelType](./literals.md#logleveltype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetHubConfigurationResponseTypeDef

```python
# GetHubConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetHubConfigurationResponseTypeDef


def get_value() -> GetHubConfigurationResponseTypeDef:
    return {
        "HubTokenTimerExpirySettingInSeconds": ...,
    }


# GetHubConfigurationResponseTypeDef definition

class GetHubConfigurationResponseTypeDef(TypedDict):
    HubTokenTimerExpirySettingInSeconds: int,
    UpdatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetManagedThingConnectivityDataResponseTypeDef

```python
# GetManagedThingConnectivityDataResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingConnectivityDataResponseTypeDef


def get_value() -> GetManagedThingConnectivityDataResponseTypeDef:
    return {
        "ManagedThingId": ...,
    }


# GetManagedThingConnectivityDataResponseTypeDef definition

class GetManagedThingConnectivityDataResponseTypeDef(TypedDict):
    ManagedThingId: str,
    Connected: bool,
    Timestamp: datetime.datetime,
    DisconnectReason: DisconnectReasonValueType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DisconnectReasonValueType](./literals.md#disconnectreasonvaluetype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetManagedThingMetaDataResponseTypeDef

```python
# GetManagedThingMetaDataResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingMetaDataResponseTypeDef


def get_value() -> GetManagedThingMetaDataResponseTypeDef:
    return {
        "ManagedThingId": ...,
    }


# GetManagedThingMetaDataResponseTypeDef definition

class GetManagedThingMetaDataResponseTypeDef(TypedDict):
    ManagedThingId: str,
    MetaData: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetManagedThingResponseTypeDef

```python
# GetManagedThingResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingResponseTypeDef


def get_value() -> GetManagedThingResponseTypeDef:
    return {
        "Id": ...,
    }


# GetManagedThingResponseTypeDef definition

class GetManagedThingResponseTypeDef(TypedDict):
    Id: str,
    Arn: str,
    Owner: str,
    CredentialLockerId: str,
    AdvertisedProductId: str,
    Role: RoleType,  # (1)
    ProvisioningStatus: ProvisioningStatusType,  # (2)
    Name: str,
    Model: str,
    Brand: str,
    SerialNumber: str,
    UniversalProductCode: str,
    InternationalArticleNumber: str,
    ConnectorPolicyId: str,
    ConnectorDeviceId: str,
    DeviceSpecificKey: str,
    MacAddress: str,
    ParentControllerId: str,
    Classification: str,
    CreatedAt: datetime.datetime,
    UpdatedAt: datetime.datetime,
    ActivatedAt: datetime.datetime,
    HubNetworkMode: HubNetworkModeType,  # (3)
    MetaData: Dict[str, str],
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype)
2. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype)
3. See [:material-code-brackets: HubNetworkModeType](./literals.md#hubnetworkmodetype)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetNotificationConfigurationResponseTypeDef

```python
# GetNotificationConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetNotificationConfigurationResponseTypeDef


def get_value() -> GetNotificationConfigurationResponseTypeDef:
    return {
        "EventType": ...,
    }


# GetNotificationConfigurationResponseTypeDef definition

class GetNotificationConfigurationResponseTypeDef(TypedDict):
    EventType: EventTypeType,  # (1)
    DestinationName: str,
    CreatedAt: datetime.datetime,
    UpdatedAt: datetime.datetime,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EventTypeType](./literals.md#eventtypetype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetProvisioningProfileResponseTypeDef

```python
# GetProvisioningProfileResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetProvisioningProfileResponseTypeDef


def get_value() -> GetProvisioningProfileResponseTypeDef:
    return {
        "Arn": ...,
    }


# GetProvisioningProfileResponseTypeDef definition

class GetProvisioningProfileResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    ProvisioningType: ProvisioningTypeType,  # (1)
    Id: str,
    ClaimCertificate: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ProvisioningTypeType](./literals.md#provisioningtypetype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetSchemaVersionResponseTypeDef

```python
# GetSchemaVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetSchemaVersionResponseTypeDef


def get_value() -> GetSchemaVersionResponseTypeDef:
    return {
        "SchemaId": ...,
    }


# GetSchemaVersionResponseTypeDef definition

class GetSchemaVersionResponseTypeDef(TypedDict):
    SchemaId: str,
    Type: SchemaVersionTypeType,  # (1)
    Description: str,
    Namespace: str,
    SemanticVersion: str,
    Visibility: SchemaVersionVisibilityType,  # (2)
    Schema: Dict[str, Any],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SchemaVersionTypeType](./literals.md#schemaversiontypetype)
2. See [:material-code-brackets: SchemaVersionVisibilityType](./literals.md#schemaversionvisibilitytype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PutHubConfigurationResponseTypeDef

```python
# PutHubConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PutHubConfigurationResponseTypeDef


def get_value() -> PutHubConfigurationResponseTypeDef:
    return {
        "HubTokenTimerExpirySettingInSeconds": ...,
    }


# PutHubConfigurationResponseTypeDef definition

class PutHubConfigurationResponseTypeDef(TypedDict):
    HubTokenTimerExpirySettingInSeconds: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## RegisterCustomEndpointResponseTypeDef

```python
# RegisterCustomEndpointResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import RegisterCustomEndpointResponseTypeDef


def get_value() -> RegisterCustomEndpointResponseTypeDef:
    return {
        "EndpointAddress": ...,
    }


# RegisterCustomEndpointResponseTypeDef definition

class RegisterCustomEndpointResponseTypeDef(TypedDict):
    EndpointAddress: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## SendManagedThingCommandResponseTypeDef

```python
# SendManagedThingCommandResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import SendManagedThingCommandResponseTypeDef


def get_value() -> SendManagedThingCommandResponseTypeDef:
    return {
        "TraceId": ...,
    }


# SendManagedThingCommandResponseTypeDef definition

class SendManagedThingCommandResponseTypeDef(TypedDict):
    TraceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## StartDeviceDiscoveryResponseTypeDef

```python
# StartDeviceDiscoveryResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import StartDeviceDiscoveryResponseTypeDef


def get_value() -> StartDeviceDiscoveryResponseTypeDef:
    return {
        "Id": ...,
    }


# StartDeviceDiscoveryResponseTypeDef definition

class StartDeviceDiscoveryResponseTypeDef(TypedDict):
    Id: str,
    StartedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListCredentialLockersResponseTypeDef

```python
# ListCredentialLockersResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListCredentialLockersResponseTypeDef


def get_value() -> ListCredentialLockersResponseTypeDef:
    return {
        "Items": ...,
    }


# ListCredentialLockersResponseTypeDef definition

class ListCredentialLockersResponseTypeDef(TypedDict):
    Items: List[CredentialLockerSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[CredentialLockerSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListDestinationsResponseTypeDef

```python
# ListDestinationsResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListDestinationsResponseTypeDef


def get_value() -> ListDestinationsResponseTypeDef:
    return {
        "DestinationList": ...,
    }


# ListDestinationsResponseTypeDef definition

class ListDestinationsResponseTypeDef(TypedDict):
    DestinationList: List[DestinationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[DestinationSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListEventLogConfigurationsResponseTypeDef

```python
# ListEventLogConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListEventLogConfigurationsResponseTypeDef


def get_value() -> ListEventLogConfigurationsResponseTypeDef:
    return {
        "EventLogConfigurationList": ...,
    }


# ListEventLogConfigurationsResponseTypeDef definition

class ListEventLogConfigurationsResponseTypeDef(TypedDict):
    EventLogConfigurationList: List[EventLogConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[EventLogConfigurationSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ExponentialRolloutRateTypeDef

```python
# ExponentialRolloutRateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ExponentialRolloutRateTypeDef


def get_value() -> ExponentialRolloutRateTypeDef:
    return {
        "BaseRatePerMinute": ...,
    }


# ExponentialRolloutRateTypeDef definition

class ExponentialRolloutRateTypeDef(TypedDict):
    BaseRatePerMinute: NotRequired[int],
    IncrementFactor: NotRequired[float],
    RateIncreaseCriteria: NotRequired[RolloutRateIncreaseCriteriaTypeDef],  # (1)
```

1. See [:material-code-braces: RolloutRateIncreaseCriteriaTypeDef](./type_defs.md#rolloutrateincreasecriteriatypedef)

## GetRuntimeLogConfigurationResponseTypeDef

```python
# GetRuntimeLogConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetRuntimeLogConfigurationResponseTypeDef


def get_value() -> GetRuntimeLogConfigurationResponseTypeDef:
    return {
        "ManagedThingId": ...,
    }


# GetRuntimeLogConfigurationResponseTypeDef definition

class GetRuntimeLogConfigurationResponseTypeDef(TypedDict):
    ManagedThingId: str,
    RuntimeLogConfigurations: RuntimeLogConfigurationsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RuntimeLogConfigurationsTypeDef](./type_defs.md#runtimelogconfigurationstypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PutRuntimeLogConfigurationRequestTypeDef

```python
# PutRuntimeLogConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PutRuntimeLogConfigurationRequestTypeDef


def get_value() -> PutRuntimeLogConfigurationRequestTypeDef:
    return {
        "ManagedThingId": ...,
    }


# PutRuntimeLogConfigurationRequestTypeDef definition

class PutRuntimeLogConfigurationRequestTypeDef(TypedDict):
    ManagedThingId: str,
    RuntimeLogConfigurations: RuntimeLogConfigurationsTypeDef,  # (1)
```

1. See [:material-code-braces: RuntimeLogConfigurationsTypeDef](./type_defs.md#runtimelogconfigurationstypedef)

## ListCredentialLockersRequestPaginateTypeDef

```python
# ListCredentialLockersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListCredentialLockersRequestPaginateTypeDef


def get_value() -> ListCredentialLockersRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListCredentialLockersRequestPaginateTypeDef definition

class ListCredentialLockersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListDestinationsRequestPaginateTypeDef

```python
# ListDestinationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListDestinationsRequestPaginateTypeDef


def get_value() -> ListDestinationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListDestinationsRequestPaginateTypeDef definition

class ListDestinationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListEventLogConfigurationsRequestPaginateTypeDef

```python
# ListEventLogConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListEventLogConfigurationsRequestPaginateTypeDef


def get_value() -> ListEventLogConfigurationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListEventLogConfigurationsRequestPaginateTypeDef definition

class ListEventLogConfigurationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListManagedThingSchemasRequestPaginateTypeDef

```python
# ListManagedThingSchemasRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListManagedThingSchemasRequestPaginateTypeDef


def get_value() -> ListManagedThingSchemasRequestPaginateTypeDef:
    return {
        "Identifier": ...,
    }


# ListManagedThingSchemasRequestPaginateTypeDef definition

class ListManagedThingSchemasRequestPaginateTypeDef(TypedDict):
    Identifier: str,
    EndpointIdFilter: NotRequired[str],
    CapabilityIdFilter: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListManagedThingsRequestPaginateTypeDef

```python
# ListManagedThingsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListManagedThingsRequestPaginateTypeDef


def get_value() -> ListManagedThingsRequestPaginateTypeDef:
    return {
        "OwnerFilter": ...,
    }


# ListManagedThingsRequestPaginateTypeDef definition

class ListManagedThingsRequestPaginateTypeDef(TypedDict):
    OwnerFilter: NotRequired[str],
    CredentialLockerFilter: NotRequired[str],
    RoleFilter: NotRequired[RoleType],  # (1)
    ParentControllerIdentifierFilter: NotRequired[str],
    ConnectorPolicyIdFilter: NotRequired[str],
    SerialNumberFilter: NotRequired[str],
    ProvisioningStatusFilter: NotRequired[ProvisioningStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype)
2. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListNotificationConfigurationsRequestPaginateTypeDef

```python
# ListNotificationConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListNotificationConfigurationsRequestPaginateTypeDef


def get_value() -> ListNotificationConfigurationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListNotificationConfigurationsRequestPaginateTypeDef definition

class ListNotificationConfigurationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListOtaTaskConfigurationsRequestPaginateTypeDef

```python
# ListOtaTaskConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTaskConfigurationsRequestPaginateTypeDef


def get_value() -> ListOtaTaskConfigurationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListOtaTaskConfigurationsRequestPaginateTypeDef definition

class ListOtaTaskConfigurationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListOtaTaskExecutionsRequestPaginateTypeDef

```python
# ListOtaTaskExecutionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTaskExecutionsRequestPaginateTypeDef


def get_value() -> ListOtaTaskExecutionsRequestPaginateTypeDef:
    return {
        "Identifier": ...,
    }


# ListOtaTaskExecutionsRequestPaginateTypeDef definition

class ListOtaTaskExecutionsRequestPaginateTypeDef(TypedDict):
    Identifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListOtaTasksRequestPaginateTypeDef

```python
# ListOtaTasksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTasksRequestPaginateTypeDef


def get_value() -> ListOtaTasksRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListOtaTasksRequestPaginateTypeDef definition

class ListOtaTasksRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListProvisioningProfilesRequestPaginateTypeDef

```python
# ListProvisioningProfilesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListProvisioningProfilesRequestPaginateTypeDef


def get_value() -> ListProvisioningProfilesRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListProvisioningProfilesRequestPaginateTypeDef definition

class ListProvisioningProfilesRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListSchemaVersionsRequestPaginateTypeDef

```python
# ListSchemaVersionsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListSchemaVersionsRequestPaginateTypeDef


def get_value() -> ListSchemaVersionsRequestPaginateTypeDef:
    return {
        "Type": ...,
    }


# ListSchemaVersionsRequestPaginateTypeDef definition

class ListSchemaVersionsRequestPaginateTypeDef(TypedDict):
    Type: SchemaVersionTypeType,  # (1)
    SchemaId: NotRequired[str],
    Namespace: NotRequired[str],
    Visibility: NotRequired[SchemaVersionVisibilityType],  # (2)
    SemanticVersion: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SchemaVersionTypeType](./literals.md#schemaversiontypetype)
2. See [:material-code-brackets: SchemaVersionVisibilityType](./literals.md#schemaversionvisibilitytype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## ListManagedThingSchemasResponseTypeDef

```python
# ListManagedThingSchemasResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListManagedThingSchemasResponseTypeDef


def get_value() -> ListManagedThingSchemasResponseTypeDef:
    return {
        "Items": ...,
    }


# ListManagedThingSchemasResponseTypeDef definition

class ListManagedThingSchemasResponseTypeDef(TypedDict):
    Items: List[ManagedThingSchemaListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[ManagedThingSchemaListItemTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListManagedThingsResponseTypeDef

```python
# ListManagedThingsResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListManagedThingsResponseTypeDef


def get_value() -> ListManagedThingsResponseTypeDef:
    return {
        "Items": ...,
    }


# ListManagedThingsResponseTypeDef definition

class ListManagedThingsResponseTypeDef(TypedDict):
    Items: List[ManagedThingSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[ManagedThingSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListNotificationConfigurationsResponseTypeDef

```python
# ListNotificationConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListNotificationConfigurationsResponseTypeDef


def get_value() -> ListNotificationConfigurationsResponseTypeDef:
    return {
        "NotificationConfigurationList": ...,
    }


# ListNotificationConfigurationsResponseTypeDef definition

class ListNotificationConfigurationsResponseTypeDef(TypedDict):
    NotificationConfigurationList: List[NotificationConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[NotificationConfigurationSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListOtaTaskConfigurationsResponseTypeDef

```python
# ListOtaTaskConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTaskConfigurationsResponseTypeDef


def get_value() -> ListOtaTaskConfigurationsResponseTypeDef:
    return {
        "Items": ...,
    }


# ListOtaTaskConfigurationsResponseTypeDef definition

class ListOtaTaskConfigurationsResponseTypeDef(TypedDict):
    Items: List[OtaTaskConfigurationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[OtaTaskConfigurationSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListOtaTasksResponseTypeDef

```python
# ListOtaTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTasksResponseTypeDef


def get_value() -> ListOtaTasksResponseTypeDef:
    return {
        "Tasks": ...,
    }


# ListOtaTasksResponseTypeDef definition

class ListOtaTasksResponseTypeDef(TypedDict):
    Tasks: List[OtaTaskSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[OtaTaskSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListProvisioningProfilesResponseTypeDef

```python
# ListProvisioningProfilesResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListProvisioningProfilesResponseTypeDef


def get_value() -> ListProvisioningProfilesResponseTypeDef:
    return {
        "Items": ...,
    }


# ListProvisioningProfilesResponseTypeDef definition

class ListProvisioningProfilesResponseTypeDef(TypedDict):
    Items: List[ProvisioningProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[ProvisioningProfileSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListSchemaVersionsResponseTypeDef

```python
# ListSchemaVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListSchemaVersionsResponseTypeDef


def get_value() -> ListSchemaVersionsResponseTypeDef:
    return {
        "Items": ...,
    }


# ListSchemaVersionsResponseTypeDef definition

class ListSchemaVersionsResponseTypeDef(TypedDict):
    Items: List[SchemaVersionListItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[SchemaVersionListItemTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## OtaTaskExecutionRetryConfigOutputTypeDef

```python
# OtaTaskExecutionRetryConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskExecutionRetryConfigOutputTypeDef


def get_value() -> OtaTaskExecutionRetryConfigOutputTypeDef:
    return {
        "RetryConfigCriteria": ...,
    }


# OtaTaskExecutionRetryConfigOutputTypeDef definition

class OtaTaskExecutionRetryConfigOutputTypeDef(TypedDict):
    RetryConfigCriteria: NotRequired[List[RetryConfigCriteriaTypeDef]],  # (1)
```

1. See `List[RetryConfigCriteriaTypeDef]`

## OtaTaskExecutionRetryConfigTypeDef

```python
# OtaTaskExecutionRetryConfigTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskExecutionRetryConfigTypeDef


def get_value() -> OtaTaskExecutionRetryConfigTypeDef:
    return {
        "RetryConfigCriteria": ...,
    }


# OtaTaskExecutionRetryConfigTypeDef definition

class OtaTaskExecutionRetryConfigTypeDef(TypedDict):
    RetryConfigCriteria: NotRequired[Sequence[RetryConfigCriteriaTypeDef]],  # (1)
```

1. See `Sequence[RetryConfigCriteriaTypeDef]`

## OtaTaskExecutionSummariesTypeDef

```python
# OtaTaskExecutionSummariesTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskExecutionSummariesTypeDef


def get_value() -> OtaTaskExecutionSummariesTypeDef:
    return {
        "TaskExecutionSummary": ...,
    }


# OtaTaskExecutionSummariesTypeDef definition

class OtaTaskExecutionSummariesTypeDef(TypedDict):
    TaskExecutionSummary: NotRequired[OtaTaskExecutionSummaryTypeDef],  # (1)
    ManagedThingId: NotRequired[str],
```

1. See [:material-code-braces: OtaTaskExecutionSummaryTypeDef](./type_defs.md#otataskexecutionsummarytypedef)

## OtaTaskSchedulingConfigOutputTypeDef

```python
# OtaTaskSchedulingConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskSchedulingConfigOutputTypeDef


def get_value() -> OtaTaskSchedulingConfigOutputTypeDef:
    return {
        "EndBehavior": ...,
    }


# OtaTaskSchedulingConfigOutputTypeDef definition

class OtaTaskSchedulingConfigOutputTypeDef(TypedDict):
    EndBehavior: NotRequired[SchedulingConfigEndBehaviorType],  # (1)
    EndTime: NotRequired[str],
    MaintenanceWindows: NotRequired[List[ScheduleMaintenanceWindowTypeDef]],  # (2)
    StartTime: NotRequired[str],
```

1. See [:material-code-brackets: SchedulingConfigEndBehaviorType](./literals.md#schedulingconfigendbehaviortype)
2. See `List[ScheduleMaintenanceWindowTypeDef]`

## OtaTaskSchedulingConfigTypeDef

```python
# OtaTaskSchedulingConfigTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskSchedulingConfigTypeDef


def get_value() -> OtaTaskSchedulingConfigTypeDef:
    return {
        "EndBehavior": ...,
    }


# OtaTaskSchedulingConfigTypeDef definition

class OtaTaskSchedulingConfigTypeDef(TypedDict):
    EndBehavior: NotRequired[SchedulingConfigEndBehaviorType],  # (1)
    EndTime: NotRequired[str],
    MaintenanceWindows: NotRequired[Sequence[ScheduleMaintenanceWindowTypeDef]],  # (2)
    StartTime: NotRequired[str],
```

1. See [:material-code-brackets: SchedulingConfigEndBehaviorType](./literals.md#schedulingconfigendbehaviortype)
2. See `Sequence[ScheduleMaintenanceWindowTypeDef]`

## StateEndpointTypeDef

```python
# StateEndpointTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import StateEndpointTypeDef


def get_value() -> StateEndpointTypeDef:
    return {
        "endpointId": ...,
    }


# StateEndpointTypeDef definition

class StateEndpointTypeDef(TypedDict):
    endpointId: str,
    capabilities: List[StateCapabilityTypeDef],  # (1)
```

1. See `List[StateCapabilityTypeDef]`

## CommandEndpointTypeDef

```python
# CommandEndpointTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CommandEndpointTypeDef


def get_value() -> CommandEndpointTypeDef:
    return {
        "endpointId": ...,
    }


# CommandEndpointTypeDef definition

class CommandEndpointTypeDef(TypedDict):
    endpointId: str,
    capabilities: Sequence[CommandCapabilityTypeDef],  # (1)
```

1. See `Sequence[CommandCapabilityTypeDef]`

## CapabilityReportOutputTypeDef

```python
# CapabilityReportOutputTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CapabilityReportOutputTypeDef


def get_value() -> CapabilityReportOutputTypeDef:
    return {
        "version": ...,
    }


# CapabilityReportOutputTypeDef definition

class CapabilityReportOutputTypeDef(TypedDict):
    version: str,
    endpoints: List[CapabilityReportEndpointOutputTypeDef],  # (1)
    nodeId: NotRequired[str],
```

1. See `List[CapabilityReportEndpointOutputTypeDef]`

## CapabilityReportTypeDef

```python
# CapabilityReportTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CapabilityReportTypeDef


def get_value() -> CapabilityReportTypeDef:
    return {
        "version": ...,
    }


# CapabilityReportTypeDef definition

class CapabilityReportTypeDef(TypedDict):
    version: str,
    endpoints: Sequence[CapabilityReportEndpointTypeDef],  # (1)
    nodeId: NotRequired[str],
```

1. See `Sequence[CapabilityReportEndpointTypeDef]`

## GetDefaultEncryptionConfigurationResponseTypeDef

```python
# GetDefaultEncryptionConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetDefaultEncryptionConfigurationResponseTypeDef


def get_value() -> GetDefaultEncryptionConfigurationResponseTypeDef:
    return {
        "configurationStatus": ...,
    }


# GetDefaultEncryptionConfigurationResponseTypeDef definition

class GetDefaultEncryptionConfigurationResponseTypeDef(TypedDict):
    configurationStatus: ConfigurationStatusTypeDef,  # (1)
    encryptionType: EncryptionTypeType,  # (2)
    kmsKeyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConfigurationStatusTypeDef](./type_defs.md#configurationstatustypedef)
2. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PutDefaultEncryptionConfigurationResponseTypeDef

```python
# PutDefaultEncryptionConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PutDefaultEncryptionConfigurationResponseTypeDef


def get_value() -> PutDefaultEncryptionConfigurationResponseTypeDef:
    return {
        "configurationStatus": ...,
    }


# PutDefaultEncryptionConfigurationResponseTypeDef definition

class PutDefaultEncryptionConfigurationResponseTypeDef(TypedDict):
    configurationStatus: ConfigurationStatusTypeDef,  # (1)
    encryptionType: EncryptionTypeType,  # (2)
    kmsKeyArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConfigurationStatusTypeDef](./type_defs.md#configurationstatustypedef)
2. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype)
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## OtaTaskExecutionRolloutConfigTypeDef

```python
# OtaTaskExecutionRolloutConfigTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import OtaTaskExecutionRolloutConfigTypeDef


def get_value() -> OtaTaskExecutionRolloutConfigTypeDef:
    return {
        "ExponentialRolloutRate": ...,
    }


# OtaTaskExecutionRolloutConfigTypeDef definition

class OtaTaskExecutionRolloutConfigTypeDef(TypedDict):
    ExponentialRolloutRate: NotRequired[ExponentialRolloutRateTypeDef],  # (1)
    MaximumPerMinute: NotRequired[int],
```

1. See [:material-code-braces: ExponentialRolloutRateTypeDef](./type_defs.md#exponentialrolloutratetypedef)

## ListOtaTaskExecutionsResponseTypeDef

```python
# ListOtaTaskExecutionsResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import ListOtaTaskExecutionsResponseTypeDef


def get_value() -> ListOtaTaskExecutionsResponseTypeDef:
    return {
        "ExecutionSummaries": ...,
    }


# ListOtaTaskExecutionsResponseTypeDef definition

class ListOtaTaskExecutionsResponseTypeDef(TypedDict):
    ExecutionSummaries: List[OtaTaskExecutionSummariesTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See `List[OtaTaskExecutionSummariesTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetOtaTaskResponseTypeDef

```python
# GetOtaTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetOtaTaskResponseTypeDef


def get_value() -> GetOtaTaskResponseTypeDef:
    return {
        "TaskId": ...,
    }


# GetOtaTaskResponseTypeDef definition

class GetOtaTaskResponseTypeDef(TypedDict):
    TaskId: str,
    TaskArn: str,
    Description: str,
    S3Url: str,
    Protocol: OtaProtocolType,  # (1)
    OtaType: OtaTypeType,  # (2)
    OtaTargetQueryString: str,
    OtaMechanism: OtaMechanismType,  # (3)
    Target: List[str],
    CreatedAt: datetime.datetime,
    LastUpdatedAt: datetime.datetime,
    TaskConfigurationId: str,
    TaskProcessingDetails: TaskProcessingDetailsTypeDef,  # (4)
    OtaSchedulingConfig: OtaTaskSchedulingConfigOutputTypeDef,  # (5)
    OtaTaskExecutionRetryConfig: OtaTaskExecutionRetryConfigOutputTypeDef,  # (6)
    Status: OtaStatusType,  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-brackets: OtaProtocolType](./literals.md#otaprotocoltype)
2. See [:material-code-brackets: OtaTypeType](./literals.md#otatypetype)
3. See [:material-code-brackets: OtaMechanismType](./literals.md#otamechanismtype)
4. See [:material-code-braces: TaskProcessingDetailsTypeDef](./type_defs.md#taskprocessingdetailstypedef)
5. See [:material-code-braces: OtaTaskSchedulingConfigOutputTypeDef](./type_defs.md#otataskschedulingconfigoutputtypedef)
6. See [:material-code-braces: OtaTaskExecutionRetryConfigOutputTypeDef](./type_defs.md#otataskexecutionretryconfigoutputtypedef)
7. See [:material-code-brackets: OtaStatusType](./literals.md#otastatustype)
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetManagedThingStateResponseTypeDef

```python
# GetManagedThingStateResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingStateResponseTypeDef


def get_value() -> GetManagedThingStateResponseTypeDef:
    return {
        "Endpoints": ...,
    }


# GetManagedThingStateResponseTypeDef definition

class GetManagedThingStateResponseTypeDef(TypedDict):
    Endpoints: List[StateEndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See `List[StateEndpointTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## SendManagedThingCommandRequestTypeDef

```python
# SendManagedThingCommandRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import SendManagedThingCommandRequestTypeDef


def get_value() -> SendManagedThingCommandRequestTypeDef:
    return {
        "ManagedThingId": ...,
    }


# SendManagedThingCommandRequestTypeDef definition

class SendManagedThingCommandRequestTypeDef(TypedDict):
    ManagedThingId: str,
    Endpoints: Sequence[CommandEndpointTypeDef],  # (1)
    ConnectorAssociationId: NotRequired[str],
```

1. See `Sequence[CommandEndpointTypeDef]`

## GetManagedThingCapabilitiesResponseTypeDef

```python
# GetManagedThingCapabilitiesResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetManagedThingCapabilitiesResponseTypeDef


def get_value() -> GetManagedThingCapabilitiesResponseTypeDef:
    return {
        "ManagedThingId": ...,
    }


# GetManagedThingCapabilitiesResponseTypeDef definition

class GetManagedThingCapabilitiesResponseTypeDef(TypedDict):
    ManagedThingId: str,
    Capabilities: str,
    CapabilityReport: CapabilityReportOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CapabilityReportOutputTypeDef](./type_defs.md#capabilityreportoutputtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PushConfigOutputTypeDef

```python
# PushConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PushConfigOutputTypeDef


def get_value() -> PushConfigOutputTypeDef:
    return {
        "AbortConfig": ...,
    }


# PushConfigOutputTypeDef definition

class PushConfigOutputTypeDef(TypedDict):
    AbortConfig: NotRequired[OtaTaskAbortConfigOutputTypeDef],  # (1)
    RolloutConfig: NotRequired[OtaTaskExecutionRolloutConfigTypeDef],  # (2)
    TimeoutConfig: NotRequired[OtaTaskTimeoutConfigTypeDef],  # (3)
```

1. See [:material-code-braces: OtaTaskAbortConfigOutputTypeDef](./type_defs.md#otataskabortconfigoutputtypedef)
2. See [:material-code-braces: OtaTaskExecutionRolloutConfigTypeDef](./type_defs.md#otataskexecutionrolloutconfigtypedef)
3. See [:material-code-braces: OtaTaskTimeoutConfigTypeDef](./type_defs.md#otatasktimeoutconfigtypedef)

## PushConfigTypeDef

```python
# PushConfigTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import PushConfigTypeDef


def get_value() -> PushConfigTypeDef:
    return {
        "AbortConfig": ...,
    }


# PushConfigTypeDef definition

class PushConfigTypeDef(TypedDict):
    AbortConfig: NotRequired[OtaTaskAbortConfigTypeDef],  # (1)
    RolloutConfig: NotRequired[OtaTaskExecutionRolloutConfigTypeDef],  # (2)
    TimeoutConfig: NotRequired[OtaTaskTimeoutConfigTypeDef],  # (3)
```

1. See [:material-code-braces: OtaTaskAbortConfigTypeDef](./type_defs.md#otataskabortconfigtypedef)
2. See [:material-code-braces: OtaTaskExecutionRolloutConfigTypeDef](./type_defs.md#otataskexecutionrolloutconfigtypedef)
3. See [:material-code-braces: OtaTaskTimeoutConfigTypeDef](./type_defs.md#otatasktimeoutconfigtypedef)

## CreateOtaTaskRequestTypeDef

```python
# CreateOtaTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateOtaTaskRequestTypeDef


def get_value() -> CreateOtaTaskRequestTypeDef:
    return {
        "S3Url": ...,
    }


# CreateOtaTaskRequestTypeDef definition

class CreateOtaTaskRequestTypeDef(TypedDict):
    S3Url: str,
    OtaType: OtaTypeType,  # (1)
    Description: NotRequired[str],
    Protocol: NotRequired[OtaProtocolType],  # (2)
    Target: NotRequired[Sequence[str]],
    TaskConfigurationId: NotRequired[str],
    OtaMechanism: NotRequired[OtaMechanismType],  # (3)
    OtaTargetQueryString: NotRequired[str],
    ClientToken: NotRequired[str],
    OtaSchedulingConfig: NotRequired[OtaTaskSchedulingConfigUnionTypeDef],  # (4)
    OtaTaskExecutionRetryConfig: NotRequired[OtaTaskExecutionRetryConfigUnionTypeDef],  # (5)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: OtaTypeType](./literals.md#otatypetype)
2. See [:material-code-brackets: OtaProtocolType](./literals.md#otaprotocoltype)
3. See [:material-code-brackets: OtaMechanismType](./literals.md#otamechanismtype)
4. See [:material-code-braces: OtaTaskSchedulingConfigUnionTypeDef](#otataskschedulingconfiguniontypedef)
5. See [:material-code-braces: OtaTaskExecutionRetryConfigUnionTypeDef](#otataskexecutionretryconfiguniontypedef)

## CreateManagedThingRequestTypeDef

```python
# CreateManagedThingRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateManagedThingRequestTypeDef


def get_value() -> CreateManagedThingRequestTypeDef:
    return {
        "Role": ...,
    }


# CreateManagedThingRequestTypeDef definition

class CreateManagedThingRequestTypeDef(TypedDict):
    Role: RoleType,  # (1)
    AuthenticationMaterial: str,
    AuthenticationMaterialType: AuthMaterialTypeType,  # (2)
    Owner: NotRequired[str],
    CredentialLockerId: NotRequired[str],
    SerialNumber: NotRequired[str],
    Brand: NotRequired[str],
    Model: NotRequired[str],
    Name: NotRequired[str],
    CapabilityReport: NotRequired[CapabilityReportUnionTypeDef],  # (3)
    Capabilities: NotRequired[str],
    ClientToken: NotRequired[str],
    Classification: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
    MetaData: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype)
2. See [:material-code-brackets: AuthMaterialTypeType](./literals.md#authmaterialtypetype)
3. See [:material-code-braces: CapabilityReportUnionTypeDef](#capabilityreportuniontypedef)

## UpdateManagedThingRequestTypeDef

```python
# UpdateManagedThingRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import UpdateManagedThingRequestTypeDef


def get_value() -> UpdateManagedThingRequestTypeDef:
    return {
        "Identifier": ...,
    }


# UpdateManagedThingRequestTypeDef definition

class UpdateManagedThingRequestTypeDef(TypedDict):
    Identifier: str,
    Owner: NotRequired[str],
    CredentialLockerId: NotRequired[str],
    SerialNumber: NotRequired[str],
    Brand: NotRequired[str],
    Model: NotRequired[str],
    Name: NotRequired[str],
    CapabilityReport: NotRequired[CapabilityReportUnionTypeDef],  # (1)
    Capabilities: NotRequired[str],
    Classification: NotRequired[str],
    HubNetworkMode: NotRequired[HubNetworkModeType],  # (2)
    MetaData: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: CapabilityReportUnionTypeDef](#capabilityreportuniontypedef)
2. See [:material-code-brackets: HubNetworkModeType](./literals.md#hubnetworkmodetype)

## GetOtaTaskConfigurationResponseTypeDef

```python
# GetOtaTaskConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import GetOtaTaskConfigurationResponseTypeDef


def get_value() -> GetOtaTaskConfigurationResponseTypeDef:
    return {
        "TaskConfigurationId": ...,
    }


# GetOtaTaskConfigurationResponseTypeDef definition

class GetOtaTaskConfigurationResponseTypeDef(TypedDict):
    TaskConfigurationId: str,
    Name: str,
    PushConfig: PushConfigOutputTypeDef,  # (1)
    Description: str,
    CreatedAt: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PushConfigOutputTypeDef](./type_defs.md#pushconfigoutputtypedef)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## CreateOtaTaskConfigurationRequestTypeDef

```python
# CreateOtaTaskConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_iot_managed_integrations.type_defs import CreateOtaTaskConfigurationRequestTypeDef


def get_value() -> CreateOtaTaskConfigurationRequestTypeDef:
    return {
        "Description": ...,
    }


# CreateOtaTaskConfigurationRequestTypeDef definition

class CreateOtaTaskConfigurationRequestTypeDef(TypedDict):
    Description: NotRequired[str],
    Name: NotRequired[str],
    PushConfig: NotRequired[PushConfigUnionTypeDef],  # (1)
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: PushConfigUnionTypeDef](#pushconfiguniontypedef)


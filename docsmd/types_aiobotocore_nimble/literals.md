# Literals

> [Index](../README.md) > [NimbleStudio](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [NimbleStudio](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/nimble.html#NimbleStudio)
    type annotations stubs module [types-aiobotocore-nimble](https://pypi.org/project/types-aiobotocore-nimble/).

## AutomaticTerminationModeType

```python
# AutomaticTerminationModeType usage example

from types_aiobotocore_nimble.literals import AutomaticTerminationModeType

def get_value() -> AutomaticTerminationModeType:
    return "ACTIVATED"
```

```python
# AutomaticTerminationModeType definition

AutomaticTerminationModeType = Literal[
    "ACTIVATED",
    "DEACTIVATED",
]
```
## LaunchProfileDeletedWaiterName

```python
# LaunchProfileDeletedWaiterName usage example

from types_aiobotocore_nimble.literals import LaunchProfileDeletedWaiterName

def get_value() -> LaunchProfileDeletedWaiterName:
    return "launch_profile_deleted"
```

```python
# LaunchProfileDeletedWaiterName definition

LaunchProfileDeletedWaiterName = Literal[
    "launch_profile_deleted",
]
```
## LaunchProfilePersonaType

```python
# LaunchProfilePersonaType usage example

from types_aiobotocore_nimble.literals import LaunchProfilePersonaType

def get_value() -> LaunchProfilePersonaType:
    return "USER"
```

```python
# LaunchProfilePersonaType definition

LaunchProfilePersonaType = Literal[
    "USER",
]
```
## LaunchProfilePlatformType

```python
# LaunchProfilePlatformType usage example

from types_aiobotocore_nimble.literals import LaunchProfilePlatformType

def get_value() -> LaunchProfilePlatformType:
    return "LINUX"
```

```python
# LaunchProfilePlatformType definition

LaunchProfilePlatformType = Literal[
    "LINUX",
    "WINDOWS",
]
```
## LaunchProfileReadyWaiterName

```python
# LaunchProfileReadyWaiterName usage example

from types_aiobotocore_nimble.literals import LaunchProfileReadyWaiterName

def get_value() -> LaunchProfileReadyWaiterName:
    return "launch_profile_ready"
```

```python
# LaunchProfileReadyWaiterName definition

LaunchProfileReadyWaiterName = Literal[
    "launch_profile_ready",
]
```
## LaunchProfileStateType

```python
# LaunchProfileStateType usage example

from types_aiobotocore_nimble.literals import LaunchProfileStateType

def get_value() -> LaunchProfileStateType:
    return "CREATE_FAILED"
```

```python
# LaunchProfileStateType definition

LaunchProfileStateType = Literal[
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "READY",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
]
```
## LaunchProfileStatusCodeType

```python
# LaunchProfileStatusCodeType usage example

from types_aiobotocore_nimble.literals import LaunchProfileStatusCodeType

def get_value() -> LaunchProfileStatusCodeType:
    return "ENCRYPTION_KEY_ACCESS_DENIED"
```

```python
# LaunchProfileStatusCodeType definition

LaunchProfileStatusCodeType = Literal[
    "ENCRYPTION_KEY_ACCESS_DENIED",
    "ENCRYPTION_KEY_NOT_FOUND",
    "INTERNAL_ERROR",
    "INVALID_INSTANCE_TYPES_PROVIDED",
    "INVALID_SUBNETS_COMBINATION",
    "INVALID_SUBNETS_PROVIDED",
    "LAUNCH_PROFILE_CREATE_IN_PROGRESS",
    "LAUNCH_PROFILE_CREATED",
    "LAUNCH_PROFILE_DELETE_IN_PROGRESS",
    "LAUNCH_PROFILE_DELETED",
    "LAUNCH_PROFILE_UPDATE_IN_PROGRESS",
    "LAUNCH_PROFILE_UPDATED",
    "LAUNCH_PROFILE_WITH_STREAM_SESSIONS_NOT_DELETED",
    "STREAMING_IMAGE_NOT_FOUND",
    "STREAMING_IMAGE_NOT_READY",
]
```
## LaunchProfileValidationStateType

```python
# LaunchProfileValidationStateType usage example

from types_aiobotocore_nimble.literals import LaunchProfileValidationStateType

def get_value() -> LaunchProfileValidationStateType:
    return "VALIDATION_FAILED"
```

```python
# LaunchProfileValidationStateType definition

LaunchProfileValidationStateType = Literal[
    "VALIDATION_FAILED",
    "VALIDATION_FAILED_INTERNAL_SERVER_ERROR",
    "VALIDATION_IN_PROGRESS",
    "VALIDATION_NOT_STARTED",
    "VALIDATION_SUCCESS",
]
```
## LaunchProfileValidationStatusCodeType

```python
# LaunchProfileValidationStatusCodeType usage example

from types_aiobotocore_nimble.literals import LaunchProfileValidationStatusCodeType

def get_value() -> LaunchProfileValidationStatusCodeType:
    return "VALIDATION_FAILED_INTERNAL_SERVER_ERROR"
```

```python
# LaunchProfileValidationStatusCodeType definition

LaunchProfileValidationStatusCodeType = Literal[
    "VALIDATION_FAILED_INTERNAL_SERVER_ERROR",
    "VALIDATION_FAILED_INVALID_ACTIVE_DIRECTORY",
    "VALIDATION_FAILED_INVALID_SECURITY_GROUP_ASSOCIATION",
    "VALIDATION_FAILED_INVALID_SUBNET_ROUTE_TABLE_ASSOCIATION",
    "VALIDATION_FAILED_SUBNET_NOT_FOUND",
    "VALIDATION_FAILED_UNAUTHORIZED",
    "VALIDATION_IN_PROGRESS",
    "VALIDATION_NOT_STARTED",
    "VALIDATION_SUCCESS",
]
```
## LaunchProfileValidationTypeType

```python
# LaunchProfileValidationTypeType usage example

from types_aiobotocore_nimble.literals import LaunchProfileValidationTypeType

def get_value() -> LaunchProfileValidationTypeType:
    return "VALIDATE_ACTIVE_DIRECTORY_STUDIO_COMPONENT"
```

```python
# LaunchProfileValidationTypeType definition

LaunchProfileValidationTypeType = Literal[
    "VALIDATE_ACTIVE_DIRECTORY_STUDIO_COMPONENT",
    "VALIDATE_NETWORK_ACL_ASSOCIATION",
    "VALIDATE_SECURITY_GROUP_ASSOCIATION",
    "VALIDATE_SUBNET_ASSOCIATION",
]
```
## ListEulaAcceptancesPaginatorName

```python
# ListEulaAcceptancesPaginatorName usage example

from types_aiobotocore_nimble.literals import ListEulaAcceptancesPaginatorName

def get_value() -> ListEulaAcceptancesPaginatorName:
    return "list_eula_acceptances"
```

```python
# ListEulaAcceptancesPaginatorName definition

ListEulaAcceptancesPaginatorName = Literal[
    "list_eula_acceptances",
]
```
## ListEulasPaginatorName

```python
# ListEulasPaginatorName usage example

from types_aiobotocore_nimble.literals import ListEulasPaginatorName

def get_value() -> ListEulasPaginatorName:
    return "list_eulas"
```

```python
# ListEulasPaginatorName definition

ListEulasPaginatorName = Literal[
    "list_eulas",
]
```
## ListLaunchProfileMembersPaginatorName

```python
# ListLaunchProfileMembersPaginatorName usage example

from types_aiobotocore_nimble.literals import ListLaunchProfileMembersPaginatorName

def get_value() -> ListLaunchProfileMembersPaginatorName:
    return "list_launch_profile_members"
```

```python
# ListLaunchProfileMembersPaginatorName definition

ListLaunchProfileMembersPaginatorName = Literal[
    "list_launch_profile_members",
]
```
## ListLaunchProfilesPaginatorName

```python
# ListLaunchProfilesPaginatorName usage example

from types_aiobotocore_nimble.literals import ListLaunchProfilesPaginatorName

def get_value() -> ListLaunchProfilesPaginatorName:
    return "list_launch_profiles"
```

```python
# ListLaunchProfilesPaginatorName definition

ListLaunchProfilesPaginatorName = Literal[
    "list_launch_profiles",
]
```
## ListStreamingImagesPaginatorName

```python
# ListStreamingImagesPaginatorName usage example

from types_aiobotocore_nimble.literals import ListStreamingImagesPaginatorName

def get_value() -> ListStreamingImagesPaginatorName:
    return "list_streaming_images"
```

```python
# ListStreamingImagesPaginatorName definition

ListStreamingImagesPaginatorName = Literal[
    "list_streaming_images",
]
```
## ListStreamingSessionBackupsPaginatorName

```python
# ListStreamingSessionBackupsPaginatorName usage example

from types_aiobotocore_nimble.literals import ListStreamingSessionBackupsPaginatorName

def get_value() -> ListStreamingSessionBackupsPaginatorName:
    return "list_streaming_session_backups"
```

```python
# ListStreamingSessionBackupsPaginatorName definition

ListStreamingSessionBackupsPaginatorName = Literal[
    "list_streaming_session_backups",
]
```
## ListStreamingSessionsPaginatorName

```python
# ListStreamingSessionsPaginatorName usage example

from types_aiobotocore_nimble.literals import ListStreamingSessionsPaginatorName

def get_value() -> ListStreamingSessionsPaginatorName:
    return "list_streaming_sessions"
```

```python
# ListStreamingSessionsPaginatorName definition

ListStreamingSessionsPaginatorName = Literal[
    "list_streaming_sessions",
]
```
## ListStudioComponentsPaginatorName

```python
# ListStudioComponentsPaginatorName usage example

from types_aiobotocore_nimble.literals import ListStudioComponentsPaginatorName

def get_value() -> ListStudioComponentsPaginatorName:
    return "list_studio_components"
```

```python
# ListStudioComponentsPaginatorName definition

ListStudioComponentsPaginatorName = Literal[
    "list_studio_components",
]
```
## ListStudioMembersPaginatorName

```python
# ListStudioMembersPaginatorName usage example

from types_aiobotocore_nimble.literals import ListStudioMembersPaginatorName

def get_value() -> ListStudioMembersPaginatorName:
    return "list_studio_members"
```

```python
# ListStudioMembersPaginatorName definition

ListStudioMembersPaginatorName = Literal[
    "list_studio_members",
]
```
## ListStudiosPaginatorName

```python
# ListStudiosPaginatorName usage example

from types_aiobotocore_nimble.literals import ListStudiosPaginatorName

def get_value() -> ListStudiosPaginatorName:
    return "list_studios"
```

```python
# ListStudiosPaginatorName definition

ListStudiosPaginatorName = Literal[
    "list_studios",
]
```
## SessionBackupModeType

```python
# SessionBackupModeType usage example

from types_aiobotocore_nimble.literals import SessionBackupModeType

def get_value() -> SessionBackupModeType:
    return "AUTOMATIC"
```

```python
# SessionBackupModeType definition

SessionBackupModeType = Literal[
    "AUTOMATIC",
    "DEACTIVATED",
]
```
## SessionPersistenceModeType

```python
# SessionPersistenceModeType usage example

from types_aiobotocore_nimble.literals import SessionPersistenceModeType

def get_value() -> SessionPersistenceModeType:
    return "ACTIVATED"
```

```python
# SessionPersistenceModeType definition

SessionPersistenceModeType = Literal[
    "ACTIVATED",
    "DEACTIVATED",
]
```
## StreamingClipboardModeType

```python
# StreamingClipboardModeType usage example

from types_aiobotocore_nimble.literals import StreamingClipboardModeType

def get_value() -> StreamingClipboardModeType:
    return "DISABLED"
```

```python
# StreamingClipboardModeType definition

StreamingClipboardModeType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## StreamingImageDeletedWaiterName

```python
# StreamingImageDeletedWaiterName usage example

from types_aiobotocore_nimble.literals import StreamingImageDeletedWaiterName

def get_value() -> StreamingImageDeletedWaiterName:
    return "streaming_image_deleted"
```

```python
# StreamingImageDeletedWaiterName definition

StreamingImageDeletedWaiterName = Literal[
    "streaming_image_deleted",
]
```
## StreamingImageEncryptionConfigurationKeyTypeType

```python
# StreamingImageEncryptionConfigurationKeyTypeType usage example

from types_aiobotocore_nimble.literals import StreamingImageEncryptionConfigurationKeyTypeType

def get_value() -> StreamingImageEncryptionConfigurationKeyTypeType:
    return "CUSTOMER_MANAGED_KEY"
```

```python
# StreamingImageEncryptionConfigurationKeyTypeType definition

StreamingImageEncryptionConfigurationKeyTypeType = Literal[
    "CUSTOMER_MANAGED_KEY",
]
```
## StreamingImageReadyWaiterName

```python
# StreamingImageReadyWaiterName usage example

from types_aiobotocore_nimble.literals import StreamingImageReadyWaiterName

def get_value() -> StreamingImageReadyWaiterName:
    return "streaming_image_ready"
```

```python
# StreamingImageReadyWaiterName definition

StreamingImageReadyWaiterName = Literal[
    "streaming_image_ready",
]
```
## StreamingImageStateType

```python
# StreamingImageStateType usage example

from types_aiobotocore_nimble.literals import StreamingImageStateType

def get_value() -> StreamingImageStateType:
    return "CREATE_FAILED"
```

```python
# StreamingImageStateType definition

StreamingImageStateType = Literal[
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "READY",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
]
```
## StreamingImageStatusCodeType

```python
# StreamingImageStatusCodeType usage example

from types_aiobotocore_nimble.literals import StreamingImageStatusCodeType

def get_value() -> StreamingImageStatusCodeType:
    return "ACCESS_DENIED"
```

```python
# StreamingImageStatusCodeType definition

StreamingImageStatusCodeType = Literal[
    "ACCESS_DENIED",
    "INTERNAL_ERROR",
    "STREAMING_IMAGE_CREATE_IN_PROGRESS",
    "STREAMING_IMAGE_DELETE_IN_PROGRESS",
    "STREAMING_IMAGE_DELETED",
    "STREAMING_IMAGE_READY",
    "STREAMING_IMAGE_UPDATE_IN_PROGRESS",
]
```
## StreamingInstanceTypeType

```python
# StreamingInstanceTypeType usage example

from types_aiobotocore_nimble.literals import StreamingInstanceTypeType

def get_value() -> StreamingInstanceTypeType:
    return "g3.4xlarge"
```

```python
# StreamingInstanceTypeType definition

StreamingInstanceTypeType = Literal[
    "g3.4xlarge",
    "g3s.xlarge",
    "g4dn.12xlarge",
    "g4dn.16xlarge",
    "g4dn.2xlarge",
    "g4dn.4xlarge",
    "g4dn.8xlarge",
    "g4dn.xlarge",
    "g5.16xlarge",
    "g5.2xlarge",
    "g5.4xlarge",
    "g5.8xlarge",
    "g5.xlarge",
]
```
## StreamingSessionDeletedWaiterName

```python
# StreamingSessionDeletedWaiterName usage example

from types_aiobotocore_nimble.literals import StreamingSessionDeletedWaiterName

def get_value() -> StreamingSessionDeletedWaiterName:
    return "streaming_session_deleted"
```

```python
# StreamingSessionDeletedWaiterName definition

StreamingSessionDeletedWaiterName = Literal[
    "streaming_session_deleted",
]
```
## StreamingSessionReadyWaiterName

```python
# StreamingSessionReadyWaiterName usage example

from types_aiobotocore_nimble.literals import StreamingSessionReadyWaiterName

def get_value() -> StreamingSessionReadyWaiterName:
    return "streaming_session_ready"
```

```python
# StreamingSessionReadyWaiterName definition

StreamingSessionReadyWaiterName = Literal[
    "streaming_session_ready",
]
```
## StreamingSessionStateType

```python
# StreamingSessionStateType usage example

from types_aiobotocore_nimble.literals import StreamingSessionStateType

def get_value() -> StreamingSessionStateType:
    return "CREATE_FAILED"
```

```python
# StreamingSessionStateType definition

StreamingSessionStateType = Literal[
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "READY",
    "START_FAILED",
    "START_IN_PROGRESS",
    "STOP_FAILED",
    "STOP_IN_PROGRESS",
    "STOPPED",
]
```
## StreamingSessionStatusCodeType

```python
# StreamingSessionStatusCodeType usage example

from types_aiobotocore_nimble.literals import StreamingSessionStatusCodeType

def get_value() -> StreamingSessionStatusCodeType:
    return "ACTIVE_DIRECTORY_DOMAIN_JOIN_ERROR"
```

```python
# StreamingSessionStatusCodeType definition

StreamingSessionStatusCodeType = Literal[
    "ACTIVE_DIRECTORY_DOMAIN_JOIN_ERROR",
    "AMI_VALIDATION_ERROR",
    "DECRYPT_STREAMING_IMAGE_ERROR",
    "INITIALIZATION_SCRIPT_ERROR",
    "INSUFFICIENT_CAPACITY",
    "INTERNAL_ERROR",
    "NETWORK_CONNECTION_ERROR",
    "NETWORK_INTERFACE_ERROR",
    "STREAMING_SESSION_CREATE_IN_PROGRESS",
    "STREAMING_SESSION_DELETE_IN_PROGRESS",
    "STREAMING_SESSION_DELETED",
    "STREAMING_SESSION_READY",
    "STREAMING_SESSION_START_IN_PROGRESS",
    "STREAMING_SESSION_STARTED",
    "STREAMING_SESSION_STOP_IN_PROGRESS",
    "STREAMING_SESSION_STOPPED",
]
```
## StreamingSessionStoppedWaiterName

```python
# StreamingSessionStoppedWaiterName usage example

from types_aiobotocore_nimble.literals import StreamingSessionStoppedWaiterName

def get_value() -> StreamingSessionStoppedWaiterName:
    return "streaming_session_stopped"
```

```python
# StreamingSessionStoppedWaiterName definition

StreamingSessionStoppedWaiterName = Literal[
    "streaming_session_stopped",
]
```
## StreamingSessionStorageModeType

```python
# StreamingSessionStorageModeType usage example

from types_aiobotocore_nimble.literals import StreamingSessionStorageModeType

def get_value() -> StreamingSessionStorageModeType:
    return "UPLOAD"
```

```python
# StreamingSessionStorageModeType definition

StreamingSessionStorageModeType = Literal[
    "UPLOAD",
]
```
## StreamingSessionStreamReadyWaiterName

```python
# StreamingSessionStreamReadyWaiterName usage example

from types_aiobotocore_nimble.literals import StreamingSessionStreamReadyWaiterName

def get_value() -> StreamingSessionStreamReadyWaiterName:
    return "streaming_session_stream_ready"
```

```python
# StreamingSessionStreamReadyWaiterName definition

StreamingSessionStreamReadyWaiterName = Literal[
    "streaming_session_stream_ready",
]
```
## StreamingSessionStreamStateType

```python
# StreamingSessionStreamStateType usage example

from types_aiobotocore_nimble.literals import StreamingSessionStreamStateType

def get_value() -> StreamingSessionStreamStateType:
    return "CREATE_FAILED"
```

```python
# StreamingSessionStreamStateType definition

StreamingSessionStreamStateType = Literal[
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "READY",
]
```
## StreamingSessionStreamStatusCodeType

```python
# StreamingSessionStreamStatusCodeType usage example

from types_aiobotocore_nimble.literals import StreamingSessionStreamStatusCodeType

def get_value() -> StreamingSessionStreamStatusCodeType:
    return "INTERNAL_ERROR"
```

```python
# StreamingSessionStreamStatusCodeType definition

StreamingSessionStreamStatusCodeType = Literal[
    "INTERNAL_ERROR",
    "NETWORK_CONNECTION_ERROR",
    "STREAM_CREATE_IN_PROGRESS",
    "STREAM_DELETE_IN_PROGRESS",
    "STREAM_DELETED",
    "STREAM_READY",
]
```
## StudioComponentDeletedWaiterName

```python
# StudioComponentDeletedWaiterName usage example

from types_aiobotocore_nimble.literals import StudioComponentDeletedWaiterName

def get_value() -> StudioComponentDeletedWaiterName:
    return "studio_component_deleted"
```

```python
# StudioComponentDeletedWaiterName definition

StudioComponentDeletedWaiterName = Literal[
    "studio_component_deleted",
]
```
## StudioComponentInitializationScriptRunContextType

```python
# StudioComponentInitializationScriptRunContextType usage example

from types_aiobotocore_nimble.literals import StudioComponentInitializationScriptRunContextType

def get_value() -> StudioComponentInitializationScriptRunContextType:
    return "SYSTEM_INITIALIZATION"
```

```python
# StudioComponentInitializationScriptRunContextType definition

StudioComponentInitializationScriptRunContextType = Literal[
    "SYSTEM_INITIALIZATION",
    "USER_INITIALIZATION",
]
```
## StudioComponentReadyWaiterName

```python
# StudioComponentReadyWaiterName usage example

from types_aiobotocore_nimble.literals import StudioComponentReadyWaiterName

def get_value() -> StudioComponentReadyWaiterName:
    return "studio_component_ready"
```

```python
# StudioComponentReadyWaiterName definition

StudioComponentReadyWaiterName = Literal[
    "studio_component_ready",
]
```
## StudioComponentStateType

```python
# StudioComponentStateType usage example

from types_aiobotocore_nimble.literals import StudioComponentStateType

def get_value() -> StudioComponentStateType:
    return "CREATE_FAILED"
```

```python
# StudioComponentStateType definition

StudioComponentStateType = Literal[
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "READY",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
]
```
## StudioComponentStatusCodeType

```python
# StudioComponentStatusCodeType usage example

from types_aiobotocore_nimble.literals import StudioComponentStatusCodeType

def get_value() -> StudioComponentStatusCodeType:
    return "ACTIVE_DIRECTORY_ALREADY_EXISTS"
```

```python
# StudioComponentStatusCodeType definition

StudioComponentStatusCodeType = Literal[
    "ACTIVE_DIRECTORY_ALREADY_EXISTS",
    "ENCRYPTION_KEY_ACCESS_DENIED",
    "ENCRYPTION_KEY_NOT_FOUND",
    "INTERNAL_ERROR",
    "STUDIO_COMPONENT_CREATE_IN_PROGRESS",
    "STUDIO_COMPONENT_CREATED",
    "STUDIO_COMPONENT_DELETE_IN_PROGRESS",
    "STUDIO_COMPONENT_DELETED",
    "STUDIO_COMPONENT_UPDATE_IN_PROGRESS",
    "STUDIO_COMPONENT_UPDATED",
]
```
## StudioComponentSubtypeType

```python
# StudioComponentSubtypeType usage example

from types_aiobotocore_nimble.literals import StudioComponentSubtypeType

def get_value() -> StudioComponentSubtypeType:
    return "AMAZON_FSX_FOR_LUSTRE"
```

```python
# StudioComponentSubtypeType definition

StudioComponentSubtypeType = Literal[
    "AMAZON_FSX_FOR_LUSTRE",
    "AMAZON_FSX_FOR_WINDOWS",
    "AWS_MANAGED_MICROSOFT_AD",
    "CUSTOM",
]
```
## StudioComponentTypeType

```python
# StudioComponentTypeType usage example

from types_aiobotocore_nimble.literals import StudioComponentTypeType

def get_value() -> StudioComponentTypeType:
    return "ACTIVE_DIRECTORY"
```

```python
# StudioComponentTypeType definition

StudioComponentTypeType = Literal[
    "ACTIVE_DIRECTORY",
    "COMPUTE_FARM",
    "CUSTOM",
    "LICENSE_SERVICE",
    "SHARED_FILE_SYSTEM",
]
```
## StudioDeletedWaiterName

```python
# StudioDeletedWaiterName usage example

from types_aiobotocore_nimble.literals import StudioDeletedWaiterName

def get_value() -> StudioDeletedWaiterName:
    return "studio_deleted"
```

```python
# StudioDeletedWaiterName definition

StudioDeletedWaiterName = Literal[
    "studio_deleted",
]
```
## StudioEncryptionConfigurationKeyTypeType

```python
# StudioEncryptionConfigurationKeyTypeType usage example

from types_aiobotocore_nimble.literals import StudioEncryptionConfigurationKeyTypeType

def get_value() -> StudioEncryptionConfigurationKeyTypeType:
    return "AWS_OWNED_KEY"
```

```python
# StudioEncryptionConfigurationKeyTypeType definition

StudioEncryptionConfigurationKeyTypeType = Literal[
    "AWS_OWNED_KEY",
    "CUSTOMER_MANAGED_KEY",
]
```
## StudioPersonaType

```python
# StudioPersonaType usage example

from types_aiobotocore_nimble.literals import StudioPersonaType

def get_value() -> StudioPersonaType:
    return "ADMINISTRATOR"
```

```python
# StudioPersonaType definition

StudioPersonaType = Literal[
    "ADMINISTRATOR",
]
```
## StudioReadyWaiterName

```python
# StudioReadyWaiterName usage example

from types_aiobotocore_nimble.literals import StudioReadyWaiterName

def get_value() -> StudioReadyWaiterName:
    return "studio_ready"
```

```python
# StudioReadyWaiterName definition

StudioReadyWaiterName = Literal[
    "studio_ready",
]
```
## StudioStateType

```python
# StudioStateType usage example

from types_aiobotocore_nimble.literals import StudioStateType

def get_value() -> StudioStateType:
    return "CREATE_FAILED"
```

```python
# StudioStateType definition

StudioStateType = Literal[
    "CREATE_FAILED",
    "CREATE_IN_PROGRESS",
    "DELETE_FAILED",
    "DELETE_IN_PROGRESS",
    "DELETED",
    "READY",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
]
```
## StudioStatusCodeType

```python
# StudioStatusCodeType usage example

from types_aiobotocore_nimble.literals import StudioStatusCodeType

def get_value() -> StudioStatusCodeType:
    return "AWS_SSO_ACCESS_DENIED"
```

```python
# StudioStatusCodeType definition

StudioStatusCodeType = Literal[
    "AWS_SSO_ACCESS_DENIED",
    "AWS_SSO_CONFIGURATION_REPAIR_IN_PROGRESS",
    "AWS_SSO_CONFIGURATION_REPAIRED",
    "AWS_SSO_NOT_ENABLED",
    "AWS_STS_REGION_DISABLED",
    "ENCRYPTION_KEY_ACCESS_DENIED",
    "ENCRYPTION_KEY_NOT_FOUND",
    "INTERNAL_ERROR",
    "ROLE_COULD_NOT_BE_ASSUMED",
    "ROLE_NOT_OWNED_BY_STUDIO_OWNER",
    "STUDIO_CREATE_IN_PROGRESS",
    "STUDIO_CREATED",
    "STUDIO_DELETE_IN_PROGRESS",
    "STUDIO_DELETED",
    "STUDIO_UPDATE_IN_PROGRESS",
    "STUDIO_UPDATED",
    "STUDIO_WITH_LAUNCH_PROFILES_NOT_DELETED",
    "STUDIO_WITH_STREAMING_IMAGES_NOT_DELETED",
    "STUDIO_WITH_STUDIO_COMPONENTS_NOT_DELETED",
]
```
## VolumeRetentionModeType

```python
# VolumeRetentionModeType usage example

from types_aiobotocore_nimble.literals import VolumeRetentionModeType

def get_value() -> VolumeRetentionModeType:
    return "DELETE"
```

```python
# VolumeRetentionModeType definition

VolumeRetentionModeType = Literal[
    "DELETE",
    "RETAIN",
]
```
## NimbleStudioServiceName

```python
# NimbleStudioServiceName usage example

from types_aiobotocore_nimble.literals import NimbleStudioServiceName

def get_value() -> NimbleStudioServiceName:
    return "nimble"
```

```python
# NimbleStudioServiceName definition

NimbleStudioServiceName = Literal[
    "nimble",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_nimble.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python
# ServiceName definition

ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appfabric",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-zonal-shift",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "backupstorage",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudtrail-data",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecatalyst",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcases",
    "connectparticipant",
    "controltower",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "docdb-elastic",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "internetmonitor",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-roborunner",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotfleetwise",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "ivs-realtime",
    "ivschat",
    "kafka",
    "kafkaconnect",
    "kendra",
    "kendra-ranking",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesis-video-webrtc-storage",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "license-manager-linux-subscriptions",
    "license-manager-user-subscriptions",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "m2",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediapackagev2",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "medical-imaging",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhuborchestrator",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "oam",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "payment-cryptography",
    "payment-cryptography-data",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "pipes",
    "polly",
    "pricing",
    "privatenetworks",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-geospatial",
    "sagemaker-metrics",
    "sagemaker-runtime",
    "savingsplans",
    "scheduler",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "securitylake",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "simspaceweaver",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_nimble.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python
# ResourceServiceName definition

ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example

from types_aiobotocore_nimble.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_eula_acceptances"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_eula_acceptances",
    "list_eulas",
    "list_launch_profile_members",
    "list_launch_profiles",
    "list_streaming_images",
    "list_streaming_session_backups",
    "list_streaming_sessions",
    "list_studio_components",
    "list_studio_members",
    "list_studios",
]
```
## WaiterName

```python
# WaiterName usage example

from types_aiobotocore_nimble.literals import WaiterName

def get_value() -> WaiterName:
    return "launch_profile_deleted"
```

```python
# WaiterName definition

WaiterName = Literal[
    "launch_profile_deleted",
    "launch_profile_ready",
    "streaming_image_deleted",
    "streaming_image_ready",
    "streaming_session_deleted",
    "streaming_session_ready",
    "streaming_session_stopped",
    "streaming_session_stream_ready",
    "studio_component_deleted",
    "studio_component_ready",
    "studio_deleted",
    "studio_ready",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_nimble.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-north-1",
    "eu-west-1",
    "eu-west-2",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```

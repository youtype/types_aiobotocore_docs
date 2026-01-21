# Literals

> [Index](../README.md) > [IoTSiteWise](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [IoTSiteWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsitewise.html#iotsitewise)
    type annotations stubs module [types-aiobotocore-iotsitewise](https://pypi.org/project/types-aiobotocore-iotsitewise/).

## AggregateTypeType

```python
# AggregateTypeType usage example
from types_aiobotocore_iotsitewise.literals import AggregateTypeType

def get_value() -> AggregateTypeType:
    return "AVERAGE"
```

```python
# AggregateTypeType definition
AggregateTypeType = Literal[
    "AVERAGE",
    "COUNT",
    "MAXIMUM",
    "MINIMUM",
    "STANDARD_DEVIATION",
    "SUM",
]
```
## AssetActiveWaiterName

```python
# AssetActiveWaiterName usage example
from types_aiobotocore_iotsitewise.literals import AssetActiveWaiterName

def get_value() -> AssetActiveWaiterName:
    return "asset_active"
```

```python
# AssetActiveWaiterName definition
AssetActiveWaiterName = Literal[
    "asset_active",
]
```
## AssetErrorCodeType

```python
# AssetErrorCodeType usage example
from types_aiobotocore_iotsitewise.literals import AssetErrorCodeType

def get_value() -> AssetErrorCodeType:
    return "INTERNAL_FAILURE"
```

```python
# AssetErrorCodeType definition
AssetErrorCodeType = Literal[
    "INTERNAL_FAILURE",
]
```
## AssetModelActiveWaiterName

```python
# AssetModelActiveWaiterName usage example
from types_aiobotocore_iotsitewise.literals import AssetModelActiveWaiterName

def get_value() -> AssetModelActiveWaiterName:
    return "asset_model_active"
```

```python
# AssetModelActiveWaiterName definition
AssetModelActiveWaiterName = Literal[
    "asset_model_active",
]
```
## AssetModelNotExistsWaiterName

```python
# AssetModelNotExistsWaiterName usage example
from types_aiobotocore_iotsitewise.literals import AssetModelNotExistsWaiterName

def get_value() -> AssetModelNotExistsWaiterName:
    return "asset_model_not_exists"
```

```python
# AssetModelNotExistsWaiterName definition
AssetModelNotExistsWaiterName = Literal[
    "asset_model_not_exists",
]
```
## AssetModelStateType

```python
# AssetModelStateType usage example
from types_aiobotocore_iotsitewise.literals import AssetModelStateType

def get_value() -> AssetModelStateType:
    return "ACTIVE"
```

```python
# AssetModelStateType definition
AssetModelStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "PROPAGATING",
    "UPDATING",
]
```
## AssetModelTypeType

```python
# AssetModelTypeType usage example
from types_aiobotocore_iotsitewise.literals import AssetModelTypeType

def get_value() -> AssetModelTypeType:
    return "ASSET_MODEL"
```

```python
# AssetModelTypeType definition
AssetModelTypeType = Literal[
    "ASSET_MODEL",
    "COMPONENT_MODEL",
    "INTERFACE",
]
```
## AssetModelVersionTypeType

```python
# AssetModelVersionTypeType usage example
from types_aiobotocore_iotsitewise.literals import AssetModelVersionTypeType

def get_value() -> AssetModelVersionTypeType:
    return "ACTIVE"
```

```python
# AssetModelVersionTypeType definition
AssetModelVersionTypeType = Literal[
    "ACTIVE",
    "LATEST",
]
```
## AssetNotExistsWaiterName

```python
# AssetNotExistsWaiterName usage example
from types_aiobotocore_iotsitewise.literals import AssetNotExistsWaiterName

def get_value() -> AssetNotExistsWaiterName:
    return "asset_not_exists"
```

```python
# AssetNotExistsWaiterName definition
AssetNotExistsWaiterName = Literal[
    "asset_not_exists",
]
```
## AssetRelationshipTypeType

```python
# AssetRelationshipTypeType usage example
from types_aiobotocore_iotsitewise.literals import AssetRelationshipTypeType

def get_value() -> AssetRelationshipTypeType:
    return "HIERARCHY"
```

```python
# AssetRelationshipTypeType definition
AssetRelationshipTypeType = Literal[
    "HIERARCHY",
]
```
## AssetStateType

```python
# AssetStateType usage example
from types_aiobotocore_iotsitewise.literals import AssetStateType

def get_value() -> AssetStateType:
    return "ACTIVE"
```

```python
# AssetStateType definition
AssetStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "UPDATING",
]
```
## AuthModeType

```python
# AuthModeType usage example
from types_aiobotocore_iotsitewise.literals import AuthModeType

def get_value() -> AuthModeType:
    return "IAM"
```

```python
# AuthModeType definition
AuthModeType = Literal[
    "IAM",
    "SSO",
]
```
## BatchEntryCompletionStatusType

```python
# BatchEntryCompletionStatusType usage example
from types_aiobotocore_iotsitewise.literals import BatchEntryCompletionStatusType

def get_value() -> BatchEntryCompletionStatusType:
    return "ERROR"
```

```python
# BatchEntryCompletionStatusType definition
BatchEntryCompletionStatusType = Literal[
    "ERROR",
    "SUCCESS",
]
```
## BatchGetAssetPropertyAggregatesErrorCodeType

```python
# BatchGetAssetPropertyAggregatesErrorCodeType usage example
from types_aiobotocore_iotsitewise.literals import BatchGetAssetPropertyAggregatesErrorCodeType

def get_value() -> BatchGetAssetPropertyAggregatesErrorCodeType:
    return "AccessDeniedException"
```

```python
# BatchGetAssetPropertyAggregatesErrorCodeType definition
BatchGetAssetPropertyAggregatesErrorCodeType = Literal[
    "AccessDeniedException",
    "InvalidRequestException",
    "ResourceNotFoundException",
]
```
## BatchGetAssetPropertyValueErrorCodeType

```python
# BatchGetAssetPropertyValueErrorCodeType usage example
from types_aiobotocore_iotsitewise.literals import BatchGetAssetPropertyValueErrorCodeType

def get_value() -> BatchGetAssetPropertyValueErrorCodeType:
    return "AccessDeniedException"
```

```python
# BatchGetAssetPropertyValueErrorCodeType definition
BatchGetAssetPropertyValueErrorCodeType = Literal[
    "AccessDeniedException",
    "InvalidRequestException",
    "ResourceNotFoundException",
]
```
## BatchGetAssetPropertyValueHistoryErrorCodeType

```python
# BatchGetAssetPropertyValueHistoryErrorCodeType usage example
from types_aiobotocore_iotsitewise.literals import BatchGetAssetPropertyValueHistoryErrorCodeType

def get_value() -> BatchGetAssetPropertyValueHistoryErrorCodeType:
    return "AccessDeniedException"
```

```python
# BatchGetAssetPropertyValueHistoryErrorCodeType definition
BatchGetAssetPropertyValueHistoryErrorCodeType = Literal[
    "AccessDeniedException",
    "InvalidRequestException",
    "ResourceNotFoundException",
]
```
## BatchPutAssetPropertyValueErrorCodeType

```python
# BatchPutAssetPropertyValueErrorCodeType usage example
from types_aiobotocore_iotsitewise.literals import BatchPutAssetPropertyValueErrorCodeType

def get_value() -> BatchPutAssetPropertyValueErrorCodeType:
    return "AccessDeniedException"
```

```python
# BatchPutAssetPropertyValueErrorCodeType definition
BatchPutAssetPropertyValueErrorCodeType = Literal[
    "AccessDeniedException",
    "ConflictingOperationException",
    "InternalFailureException",
    "InvalidRequestException",
    "LimitExceededException",
    "ResourceNotFoundException",
    "ServiceUnavailableException",
    "ThrottlingException",
    "TimestampOutOfRangeException",
]
```
## CapabilitySyncStatusType

```python
# CapabilitySyncStatusType usage example
from types_aiobotocore_iotsitewise.literals import CapabilitySyncStatusType

def get_value() -> CapabilitySyncStatusType:
    return "IN_SYNC"
```

```python
# CapabilitySyncStatusType definition
CapabilitySyncStatusType = Literal[
    "IN_SYNC",
    "NOT_APPLICABLE",
    "OUT_OF_SYNC",
    "SYNC_FAILED",
    "UNKNOWN",
]
```
## ColumnNameType

```python
# ColumnNameType usage example
from types_aiobotocore_iotsitewise.literals import ColumnNameType

def get_value() -> ColumnNameType:
    return "ALIAS"
```

```python
# ColumnNameType definition
ColumnNameType = Literal[
    "ALIAS",
    "ASSET_ID",
    "DATA_TYPE",
    "PROPERTY_ID",
    "QUALITY",
    "TIMESTAMP_NANO_OFFSET",
    "TIMESTAMP_SECONDS",
    "VALUE",
]
```
## ComputationModelStateType

```python
# ComputationModelStateType usage example
from types_aiobotocore_iotsitewise.literals import ComputationModelStateType

def get_value() -> ComputationModelStateType:
    return "ACTIVE"
```

```python
# ComputationModelStateType definition
ComputationModelStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "UPDATING",
]
```
## ComputationModelTypeType

```python
# ComputationModelTypeType usage example
from types_aiobotocore_iotsitewise.literals import ComputationModelTypeType

def get_value() -> ComputationModelTypeType:
    return "ANOMALY_DETECTION"
```

```python
# ComputationModelTypeType definition
ComputationModelTypeType = Literal[
    "ANOMALY_DETECTION",
]
```
## ComputeLocationType

```python
# ComputeLocationType usage example
from types_aiobotocore_iotsitewise.literals import ComputeLocationType

def get_value() -> ComputeLocationType:
    return "CLOUD"
```

```python
# ComputeLocationType definition
ComputeLocationType = Literal[
    "CLOUD",
    "EDGE",
]
```
## ConfigurationStateType

```python
# ConfigurationStateType usage example
from types_aiobotocore_iotsitewise.literals import ConfigurationStateType

def get_value() -> ConfigurationStateType:
    return "ACTIVE"
```

```python
# ConfigurationStateType definition
ConfigurationStateType = Literal[
    "ACTIVE",
    "UPDATE_FAILED",
    "UPDATE_IN_PROGRESS",
]
```
## CoreDeviceOperatingSystemType

```python
# CoreDeviceOperatingSystemType usage example
from types_aiobotocore_iotsitewise.literals import CoreDeviceOperatingSystemType

def get_value() -> CoreDeviceOperatingSystemType:
    return "LINUX_AARCH64"
```

```python
# CoreDeviceOperatingSystemType definition
CoreDeviceOperatingSystemType = Literal[
    "LINUX_AARCH64",
    "LINUX_AMD64",
    "WINDOWS_AMD64",
]
```
## DatasetSourceFormatType

```python
# DatasetSourceFormatType usage example
from types_aiobotocore_iotsitewise.literals import DatasetSourceFormatType

def get_value() -> DatasetSourceFormatType:
    return "KNOWLEDGE_BASE"
```

```python
# DatasetSourceFormatType definition
DatasetSourceFormatType = Literal[
    "KNOWLEDGE_BASE",
]
```
## DatasetSourceTypeType

```python
# DatasetSourceTypeType usage example
from types_aiobotocore_iotsitewise.literals import DatasetSourceTypeType

def get_value() -> DatasetSourceTypeType:
    return "KENDRA"
```

```python
# DatasetSourceTypeType definition
DatasetSourceTypeType = Literal[
    "KENDRA",
]
```
## DatasetStateType

```python
# DatasetStateType usage example
from types_aiobotocore_iotsitewise.literals import DatasetStateType

def get_value() -> DatasetStateType:
    return "ACTIVE"
```

```python
# DatasetStateType definition
DatasetStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "UPDATING",
]
```
## DetailedErrorCodeType

```python
# DetailedErrorCodeType usage example
from types_aiobotocore_iotsitewise.literals import DetailedErrorCodeType

def get_value() -> DetailedErrorCodeType:
    return "INCOMPATIBLE_COMPUTE_LOCATION"
```

```python
# DetailedErrorCodeType definition
DetailedErrorCodeType = Literal[
    "INCOMPATIBLE_COMPUTE_LOCATION",
    "INCOMPATIBLE_FORWARDING_CONFIGURATION",
]
```
## DisassociatedDataStorageStateType

```python
# DisassociatedDataStorageStateType usage example
from types_aiobotocore_iotsitewise.literals import DisassociatedDataStorageStateType

def get_value() -> DisassociatedDataStorageStateType:
    return "DISABLED"
```

```python
# DisassociatedDataStorageStateType definition
DisassociatedDataStorageStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## EncryptionTypeType

```python
# EncryptionTypeType usage example
from types_aiobotocore_iotsitewise.literals import EncryptionTypeType

def get_value() -> EncryptionTypeType:
    return "KMS_BASED_ENCRYPTION"
```

```python
# EncryptionTypeType definition
EncryptionTypeType = Literal[
    "KMS_BASED_ENCRYPTION",
    "SITEWISE_DEFAULT_ENCRYPTION",
]
```
## ErrorCodeType

```python
# ErrorCodeType usage example
from types_aiobotocore_iotsitewise.literals import ErrorCodeType

def get_value() -> ErrorCodeType:
    return "INTERNAL_FAILURE"
```

```python
# ErrorCodeType definition
ErrorCodeType = Literal[
    "INTERNAL_FAILURE",
    "VALIDATION_ERROR",
]
```
## ExecuteQueryPaginatorName

```python
# ExecuteQueryPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ExecuteQueryPaginatorName

def get_value() -> ExecuteQueryPaginatorName:
    return "execute_query"
```

```python
# ExecuteQueryPaginatorName definition
ExecuteQueryPaginatorName = Literal[
    "execute_query",
]
```
## ExecutionStateType

```python
# ExecutionStateType usage example
from types_aiobotocore_iotsitewise.literals import ExecutionStateType

def get_value() -> ExecutionStateType:
    return "COMPLETED"
```

```python
# ExecutionStateType definition
ExecutionStateType = Literal[
    "COMPLETED",
    "FAILED",
    "RUNNING",
]
```
## ForwardingConfigStateType

```python
# ForwardingConfigStateType usage example
from types_aiobotocore_iotsitewise.literals import ForwardingConfigStateType

def get_value() -> ForwardingConfigStateType:
    return "DISABLED"
```

```python
# ForwardingConfigStateType definition
ForwardingConfigStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## GetAssetPropertyAggregatesPaginatorName

```python
# GetAssetPropertyAggregatesPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import GetAssetPropertyAggregatesPaginatorName

def get_value() -> GetAssetPropertyAggregatesPaginatorName:
    return "get_asset_property_aggregates"
```

```python
# GetAssetPropertyAggregatesPaginatorName definition
GetAssetPropertyAggregatesPaginatorName = Literal[
    "get_asset_property_aggregates",
]
```
## GetAssetPropertyValueHistoryPaginatorName

```python
# GetAssetPropertyValueHistoryPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import GetAssetPropertyValueHistoryPaginatorName

def get_value() -> GetAssetPropertyValueHistoryPaginatorName:
    return "get_asset_property_value_history"
```

```python
# GetAssetPropertyValueHistoryPaginatorName definition
GetAssetPropertyValueHistoryPaginatorName = Literal[
    "get_asset_property_value_history",
]
```
## GetInterpolatedAssetPropertyValuesPaginatorName

```python
# GetInterpolatedAssetPropertyValuesPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import GetInterpolatedAssetPropertyValuesPaginatorName

def get_value() -> GetInterpolatedAssetPropertyValuesPaginatorName:
    return "get_interpolated_asset_property_values"
```

```python
# GetInterpolatedAssetPropertyValuesPaginatorName definition
GetInterpolatedAssetPropertyValuesPaginatorName = Literal[
    "get_interpolated_asset_property_values",
]
```
## IdentityTypeType

```python
# IdentityTypeType usage example
from types_aiobotocore_iotsitewise.literals import IdentityTypeType

def get_value() -> IdentityTypeType:
    return "GROUP"
```

```python
# IdentityTypeType definition
IdentityTypeType = Literal[
    "GROUP",
    "IAM",
    "USER",
]
```
## ImageFileTypeType

```python
# ImageFileTypeType usage example
from types_aiobotocore_iotsitewise.literals import ImageFileTypeType

def get_value() -> ImageFileTypeType:
    return "PNG"
```

```python
# ImageFileTypeType definition
ImageFileTypeType = Literal[
    "PNG",
]
```
## JobStatusType

```python
# JobStatusType usage example
from types_aiobotocore_iotsitewise.literals import JobStatusType

def get_value() -> JobStatusType:
    return "CANCELLED"
```

```python
# JobStatusType definition
JobStatusType = Literal[
    "CANCELLED",
    "COMPLETED",
    "COMPLETED_WITH_FAILURES",
    "FAILED",
    "PENDING",
    "RUNNING",
]
```
## ListAccessPoliciesPaginatorName

```python
# ListAccessPoliciesPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListAccessPoliciesPaginatorName

def get_value() -> ListAccessPoliciesPaginatorName:
    return "list_access_policies"
```

```python
# ListAccessPoliciesPaginatorName definition
ListAccessPoliciesPaginatorName = Literal[
    "list_access_policies",
]
```
## ListActionsPaginatorName

```python
# ListActionsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListActionsPaginatorName

def get_value() -> ListActionsPaginatorName:
    return "list_actions"
```

```python
# ListActionsPaginatorName definition
ListActionsPaginatorName = Literal[
    "list_actions",
]
```
## ListAssetModelCompositeModelsPaginatorName

```python
# ListAssetModelCompositeModelsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListAssetModelCompositeModelsPaginatorName

def get_value() -> ListAssetModelCompositeModelsPaginatorName:
    return "list_asset_model_composite_models"
```

```python
# ListAssetModelCompositeModelsPaginatorName definition
ListAssetModelCompositeModelsPaginatorName = Literal[
    "list_asset_model_composite_models",
]
```
## ListAssetModelPropertiesFilterType

```python
# ListAssetModelPropertiesFilterType usage example
from types_aiobotocore_iotsitewise.literals import ListAssetModelPropertiesFilterType

def get_value() -> ListAssetModelPropertiesFilterType:
    return "ALL"
```

```python
# ListAssetModelPropertiesFilterType definition
ListAssetModelPropertiesFilterType = Literal[
    "ALL",
    "BASE",
]
```
## ListAssetModelPropertiesPaginatorName

```python
# ListAssetModelPropertiesPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListAssetModelPropertiesPaginatorName

def get_value() -> ListAssetModelPropertiesPaginatorName:
    return "list_asset_model_properties"
```

```python
# ListAssetModelPropertiesPaginatorName definition
ListAssetModelPropertiesPaginatorName = Literal[
    "list_asset_model_properties",
]
```
## ListAssetModelsPaginatorName

```python
# ListAssetModelsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListAssetModelsPaginatorName

def get_value() -> ListAssetModelsPaginatorName:
    return "list_asset_models"
```

```python
# ListAssetModelsPaginatorName definition
ListAssetModelsPaginatorName = Literal[
    "list_asset_models",
]
```
## ListAssetPropertiesFilterType

```python
# ListAssetPropertiesFilterType usage example
from types_aiobotocore_iotsitewise.literals import ListAssetPropertiesFilterType

def get_value() -> ListAssetPropertiesFilterType:
    return "ALL"
```

```python
# ListAssetPropertiesFilterType definition
ListAssetPropertiesFilterType = Literal[
    "ALL",
    "BASE",
]
```
## ListAssetPropertiesPaginatorName

```python
# ListAssetPropertiesPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListAssetPropertiesPaginatorName

def get_value() -> ListAssetPropertiesPaginatorName:
    return "list_asset_properties"
```

```python
# ListAssetPropertiesPaginatorName definition
ListAssetPropertiesPaginatorName = Literal[
    "list_asset_properties",
]
```
## ListAssetRelationshipsPaginatorName

```python
# ListAssetRelationshipsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListAssetRelationshipsPaginatorName

def get_value() -> ListAssetRelationshipsPaginatorName:
    return "list_asset_relationships"
```

```python
# ListAssetRelationshipsPaginatorName definition
ListAssetRelationshipsPaginatorName = Literal[
    "list_asset_relationships",
]
```
## ListAssetsFilterType

```python
# ListAssetsFilterType usage example
from types_aiobotocore_iotsitewise.literals import ListAssetsFilterType

def get_value() -> ListAssetsFilterType:
    return "ALL"
```

```python
# ListAssetsFilterType definition
ListAssetsFilterType = Literal[
    "ALL",
    "TOP_LEVEL",
]
```
## ListAssetsPaginatorName

```python
# ListAssetsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListAssetsPaginatorName

def get_value() -> ListAssetsPaginatorName:
    return "list_assets"
```

```python
# ListAssetsPaginatorName definition
ListAssetsPaginatorName = Literal[
    "list_assets",
]
```
## ListAssociatedAssetsPaginatorName

```python
# ListAssociatedAssetsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListAssociatedAssetsPaginatorName

def get_value() -> ListAssociatedAssetsPaginatorName:
    return "list_associated_assets"
```

```python
# ListAssociatedAssetsPaginatorName definition
ListAssociatedAssetsPaginatorName = Literal[
    "list_associated_assets",
]
```
## ListBulkImportJobsFilterType

```python
# ListBulkImportJobsFilterType usage example
from types_aiobotocore_iotsitewise.literals import ListBulkImportJobsFilterType

def get_value() -> ListBulkImportJobsFilterType:
    return "ALL"
```

```python
# ListBulkImportJobsFilterType definition
ListBulkImportJobsFilterType = Literal[
    "ALL",
    "CANCELLED",
    "COMPLETED",
    "COMPLETED_WITH_FAILURES",
    "FAILED",
    "PENDING",
    "RUNNING",
]
```
## ListBulkImportJobsPaginatorName

```python
# ListBulkImportJobsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListBulkImportJobsPaginatorName

def get_value() -> ListBulkImportJobsPaginatorName:
    return "list_bulk_import_jobs"
```

```python
# ListBulkImportJobsPaginatorName definition
ListBulkImportJobsPaginatorName = Literal[
    "list_bulk_import_jobs",
]
```
## ListCompositionRelationshipsPaginatorName

```python
# ListCompositionRelationshipsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListCompositionRelationshipsPaginatorName

def get_value() -> ListCompositionRelationshipsPaginatorName:
    return "list_composition_relationships"
```

```python
# ListCompositionRelationshipsPaginatorName definition
ListCompositionRelationshipsPaginatorName = Literal[
    "list_composition_relationships",
]
```
## ListComputationModelDataBindingUsagesPaginatorName

```python
# ListComputationModelDataBindingUsagesPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListComputationModelDataBindingUsagesPaginatorName

def get_value() -> ListComputationModelDataBindingUsagesPaginatorName:
    return "list_computation_model_data_binding_usages"
```

```python
# ListComputationModelDataBindingUsagesPaginatorName definition
ListComputationModelDataBindingUsagesPaginatorName = Literal[
    "list_computation_model_data_binding_usages",
]
```
## ListComputationModelResolveToResourcesPaginatorName

```python
# ListComputationModelResolveToResourcesPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListComputationModelResolveToResourcesPaginatorName

def get_value() -> ListComputationModelResolveToResourcesPaginatorName:
    return "list_computation_model_resolve_to_resources"
```

```python
# ListComputationModelResolveToResourcesPaginatorName definition
ListComputationModelResolveToResourcesPaginatorName = Literal[
    "list_computation_model_resolve_to_resources",
]
```
## ListComputationModelsPaginatorName

```python
# ListComputationModelsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListComputationModelsPaginatorName

def get_value() -> ListComputationModelsPaginatorName:
    return "list_computation_models"
```

```python
# ListComputationModelsPaginatorName definition
ListComputationModelsPaginatorName = Literal[
    "list_computation_models",
]
```
## ListDashboardsPaginatorName

```python
# ListDashboardsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListDashboardsPaginatorName

def get_value() -> ListDashboardsPaginatorName:
    return "list_dashboards"
```

```python
# ListDashboardsPaginatorName definition
ListDashboardsPaginatorName = Literal[
    "list_dashboards",
]
```
## ListDatasetsPaginatorName

```python
# ListDatasetsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListDatasetsPaginatorName

def get_value() -> ListDatasetsPaginatorName:
    return "list_datasets"
```

```python
# ListDatasetsPaginatorName definition
ListDatasetsPaginatorName = Literal[
    "list_datasets",
]
```
## ListExecutionsPaginatorName

```python
# ListExecutionsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListExecutionsPaginatorName

def get_value() -> ListExecutionsPaginatorName:
    return "list_executions"
```

```python
# ListExecutionsPaginatorName definition
ListExecutionsPaginatorName = Literal[
    "list_executions",
]
```
## ListGatewaysPaginatorName

```python
# ListGatewaysPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListGatewaysPaginatorName

def get_value() -> ListGatewaysPaginatorName:
    return "list_gateways"
```

```python
# ListGatewaysPaginatorName definition
ListGatewaysPaginatorName = Literal[
    "list_gateways",
]
```
## ListInterfaceRelationshipsPaginatorName

```python
# ListInterfaceRelationshipsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListInterfaceRelationshipsPaginatorName

def get_value() -> ListInterfaceRelationshipsPaginatorName:
    return "list_interface_relationships"
```

```python
# ListInterfaceRelationshipsPaginatorName definition
ListInterfaceRelationshipsPaginatorName = Literal[
    "list_interface_relationships",
]
```
## ListPortalsPaginatorName

```python
# ListPortalsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListPortalsPaginatorName

def get_value() -> ListPortalsPaginatorName:
    return "list_portals"
```

```python
# ListPortalsPaginatorName definition
ListPortalsPaginatorName = Literal[
    "list_portals",
]
```
## ListProjectAssetsPaginatorName

```python
# ListProjectAssetsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListProjectAssetsPaginatorName

def get_value() -> ListProjectAssetsPaginatorName:
    return "list_project_assets"
```

```python
# ListProjectAssetsPaginatorName definition
ListProjectAssetsPaginatorName = Literal[
    "list_project_assets",
]
```
## ListProjectsPaginatorName

```python
# ListProjectsPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListProjectsPaginatorName

def get_value() -> ListProjectsPaginatorName:
    return "list_projects"
```

```python
# ListProjectsPaginatorName definition
ListProjectsPaginatorName = Literal[
    "list_projects",
]
```
## ListTimeSeriesPaginatorName

```python
# ListTimeSeriesPaginatorName usage example
from types_aiobotocore_iotsitewise.literals import ListTimeSeriesPaginatorName

def get_value() -> ListTimeSeriesPaginatorName:
    return "list_time_series"
```

```python
# ListTimeSeriesPaginatorName definition
ListTimeSeriesPaginatorName = Literal[
    "list_time_series",
]
```
## ListTimeSeriesTypeType

```python
# ListTimeSeriesTypeType usage example
from types_aiobotocore_iotsitewise.literals import ListTimeSeriesTypeType

def get_value() -> ListTimeSeriesTypeType:
    return "ASSOCIATED"
```

```python
# ListTimeSeriesTypeType definition
ListTimeSeriesTypeType = Literal[
    "ASSOCIATED",
    "DISASSOCIATED",
]
```
## LoggingLevelType

```python
# LoggingLevelType usage example
from types_aiobotocore_iotsitewise.literals import LoggingLevelType

def get_value() -> LoggingLevelType:
    return "ERROR"
```

```python
# LoggingLevelType definition
LoggingLevelType = Literal[
    "ERROR",
    "INFO",
    "OFF",
]
```
## MonitorErrorCodeType

```python
# MonitorErrorCodeType usage example
from types_aiobotocore_iotsitewise.literals import MonitorErrorCodeType

def get_value() -> MonitorErrorCodeType:
    return "INTERNAL_FAILURE"
```

```python
# MonitorErrorCodeType definition
MonitorErrorCodeType = Literal[
    "INTERNAL_FAILURE",
    "LIMIT_EXCEEDED",
    "VALIDATION_ERROR",
]
```
## PermissionType

```python
# PermissionType usage example
from types_aiobotocore_iotsitewise.literals import PermissionType

def get_value() -> PermissionType:
    return "ADMINISTRATOR"
```

```python
# PermissionType definition
PermissionType = Literal[
    "ADMINISTRATOR",
    "VIEWER",
]
```
## PortalActiveWaiterName

```python
# PortalActiveWaiterName usage example
from types_aiobotocore_iotsitewise.literals import PortalActiveWaiterName

def get_value() -> PortalActiveWaiterName:
    return "portal_active"
```

```python
# PortalActiveWaiterName definition
PortalActiveWaiterName = Literal[
    "portal_active",
]
```
## PortalNotExistsWaiterName

```python
# PortalNotExistsWaiterName usage example
from types_aiobotocore_iotsitewise.literals import PortalNotExistsWaiterName

def get_value() -> PortalNotExistsWaiterName:
    return "portal_not_exists"
```

```python
# PortalNotExistsWaiterName definition
PortalNotExistsWaiterName = Literal[
    "portal_not_exists",
]
```
## PortalStateType

```python
# PortalStateType usage example
from types_aiobotocore_iotsitewise.literals import PortalStateType

def get_value() -> PortalStateType:
    return "ACTIVE"
```

```python
# PortalStateType definition
PortalStateType = Literal[
    "ACTIVE",
    "CREATING",
    "DELETING",
    "FAILED",
    "PENDING",
    "UPDATING",
]
```
## PortalTypeType

```python
# PortalTypeType usage example
from types_aiobotocore_iotsitewise.literals import PortalTypeType

def get_value() -> PortalTypeType:
    return "SITEWISE_PORTAL_V1"
```

```python
# PortalTypeType definition
PortalTypeType = Literal[
    "SITEWISE_PORTAL_V1",
    "SITEWISE_PORTAL_V2",
]
```
## PropertyDataTypeType

```python
# PropertyDataTypeType usage example
from types_aiobotocore_iotsitewise.literals import PropertyDataTypeType

def get_value() -> PropertyDataTypeType:
    return "BOOLEAN"
```

```python
# PropertyDataTypeType definition
PropertyDataTypeType = Literal[
    "BOOLEAN",
    "DOUBLE",
    "INTEGER",
    "STRING",
    "STRUCT",
]
```
## PropertyNotificationStateType

```python
# PropertyNotificationStateType usage example
from types_aiobotocore_iotsitewise.literals import PropertyNotificationStateType

def get_value() -> PropertyNotificationStateType:
    return "DISABLED"
```

```python
# PropertyNotificationStateType definition
PropertyNotificationStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## QualityType

```python
# QualityType usage example
from types_aiobotocore_iotsitewise.literals import QualityType

def get_value() -> QualityType:
    return "BAD"
```

```python
# QualityType definition
QualityType = Literal[
    "BAD",
    "GOOD",
    "UNCERTAIN",
]
```
## RawValueTypeType

```python
# RawValueTypeType usage example
from types_aiobotocore_iotsitewise.literals import RawValueTypeType

def get_value() -> RawValueTypeType:
    return "B"
```

```python
# RawValueTypeType definition
RawValueTypeType = Literal[
    "B",
    "D",
    "I",
    "S",
    "U",
]
```
## ResolveToResourceTypeType

```python
# ResolveToResourceTypeType usage example
from types_aiobotocore_iotsitewise.literals import ResolveToResourceTypeType

def get_value() -> ResolveToResourceTypeType:
    return "ASSET"
```

```python
# ResolveToResourceTypeType definition
ResolveToResourceTypeType = Literal[
    "ASSET",
]
```
## ResourceTypeType

```python
# ResourceTypeType usage example
from types_aiobotocore_iotsitewise.literals import ResourceTypeType

def get_value() -> ResourceTypeType:
    return "PORTAL"
```

```python
# ResourceTypeType definition
ResourceTypeType = Literal[
    "PORTAL",
    "PROJECT",
]
```
## ScalarTypeType

```python
# ScalarTypeType usage example
from types_aiobotocore_iotsitewise.literals import ScalarTypeType

def get_value() -> ScalarTypeType:
    return "BOOLEAN"
```

```python
# ScalarTypeType definition
ScalarTypeType = Literal[
    "BOOLEAN",
    "DOUBLE",
    "INT",
    "STRING",
    "TIMESTAMP",
]
```
## StorageTypeType

```python
# StorageTypeType usage example
from types_aiobotocore_iotsitewise.literals import StorageTypeType

def get_value() -> StorageTypeType:
    return "MULTI_LAYER_STORAGE"
```

```python
# StorageTypeType definition
StorageTypeType = Literal[
    "MULTI_LAYER_STORAGE",
    "SITEWISE_DEFAULT_STORAGE",
]
```
## TargetResourceTypeType

```python
# TargetResourceTypeType usage example
from types_aiobotocore_iotsitewise.literals import TargetResourceTypeType

def get_value() -> TargetResourceTypeType:
    return "ASSET"
```

```python
# TargetResourceTypeType definition
TargetResourceTypeType = Literal[
    "ASSET",
    "COMPUTATION_MODEL",
]
```
## TimeOrderingType

```python
# TimeOrderingType usage example
from types_aiobotocore_iotsitewise.literals import TimeOrderingType

def get_value() -> TimeOrderingType:
    return "ASCENDING"
```

```python
# TimeOrderingType definition
TimeOrderingType = Literal[
    "ASCENDING",
    "DESCENDING",
]
```
## TraversalDirectionType

```python
# TraversalDirectionType usage example
from types_aiobotocore_iotsitewise.literals import TraversalDirectionType

def get_value() -> TraversalDirectionType:
    return "CHILD"
```

```python
# TraversalDirectionType definition
TraversalDirectionType = Literal[
    "CHILD",
    "PARENT",
]
```
## TraversalTypeType

```python
# TraversalTypeType usage example
from types_aiobotocore_iotsitewise.literals import TraversalTypeType

def get_value() -> TraversalTypeType:
    return "PATH_TO_ROOT"
```

```python
# TraversalTypeType definition
TraversalTypeType = Literal[
    "PATH_TO_ROOT",
]
```
## WarmTierStateType

```python
# WarmTierStateType usage example
from types_aiobotocore_iotsitewise.literals import WarmTierStateType

def get_value() -> WarmTierStateType:
    return "DISABLED"
```

```python
# WarmTierStateType definition
WarmTierStateType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## IoTSiteWiseServiceName

```python
# IoTSiteWiseServiceName usage example
from types_aiobotocore_iotsitewise.literals import IoTSiteWiseServiceName

def get_value() -> IoTSiteWiseServiceName:
    return "iotsitewise"
```

```python
# IoTSiteWiseServiceName definition
IoTSiteWiseServiceName = Literal[
    "iotsitewise",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_iotsitewise.literals import ServiceName

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
    "aiops",
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
    "application-signals",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "arc-region-switch",
    "arc-zonal-shift",
    "artifact",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "b2bi",
    "backup",
    "backup-gateway",
    "backupsearch",
    "batch",
    "bcm-dashboards",
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bcm-recommended-actions",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-agentcore",
    "bedrock-agentcore-control",
    "bedrock-data-automation",
    "bedrock-data-automation-runtime",
    "bedrock-runtime",
    "billing",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chatbot",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-media-pipelines",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "chime-sdk-voice",
    "cleanrooms",
    "cleanroomsml",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudfront-keyvaluestore",
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
    "codeconnections",
    "codedeploy",
    "codeguru-reviewer",
    "codeguru-security",
    "codeguruprofiler",
    "codepipeline",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "compute-optimizer-automation",
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
    "connectcampaignsv2",
    "connectcases",
    "connectparticipant",
    "controlcatalog",
    "controltower",
    "cost-optimization-hub",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "datazone",
    "dax",
    "deadline",
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
    "ds-data",
    "dsql",
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
    "eks-auth",
    "elasticache",
    "elasticbeanstalk",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "emr-serverless",
    "entityresolution",
    "es",
    "events",
    "evidently",
    "evs",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "freetier",
    "fsx",
    "gamelift",
    "gameliftstreams",
    "geo-maps",
    "geo-places",
    "geo-routes",
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
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector-scan",
    "inspector2",
    "internetmonitor",
    "invoicing",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot-managed-integrations",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
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
    "keyspacesstreams",
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
    "launch-wizard",
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
    "m2",
    "machinelearning",
    "macie2",
    "mailmanager",
    "managedblockchain",
    "managedblockchain-query",
    "marketplace-agreement",
    "marketplace-catalog",
    "marketplace-deployment",
    "marketplace-entitlement",
    "marketplace-reporting",
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
    "mpa",
    "mq",
    "mturk",
    "mwaa",
    "mwaa-serverless",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "nova-act",
    "oam",
    "observabilityadmin",
    "odb",
    "omics",
    "opensearch",
    "opensearchserverless",
    "organizations",
    "osis",
    "outposts",
    "panorama",
    "partnercentral-account",
    "partnercentral-benefits",
    "partnercentral-channel",
    "partnercentral-selling",
    "payment-cryptography",
    "payment-cryptography-data",
    "pca-connector-ad",
    "pca-connector-scep",
    "pcs",
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
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "redshift-serverless",
    "rekognition",
    "repostspace",
    "resiliencehub",
    "resource-explorer-2",
    "resource-groups",
    "resourcegroupstaggingapi",
    "rolesanywhere",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53globalresolver",
    "route53profiles",
    "route53resolver",
    "rtbfabric",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "s3tables",
    "s3vectors",
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
    "security-ir",
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
    "signin",
    "simspaceweaver",
    "snow-device-management",
    "snowball",
    "sns",
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-guiconnect",
    "ssm-incidents",
    "ssm-quicksetup",
    "ssm-sap",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "supplychain",
    "support",
    "support-app",
    "swf",
    "synthetics",
    "taxsettings",
    "textract",
    "timestream-influxdb",
    "timestream-query",
    "timestream-write",
    "tnb",
    "transcribe",
    "transfer",
    "translate",
    "trustedadvisor",
    "verifiedpermissions",
    "voice-id",
    "vpc-lattice",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wickr",
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-instances",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example
from types_aiobotocore_iotsitewise.literals import ResourceServiceName

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
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python
# PaginatorName usage example
from types_aiobotocore_iotsitewise.literals import PaginatorName

def get_value() -> PaginatorName:
    return "execute_query"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "execute_query",
    "get_asset_property_aggregates",
    "get_asset_property_value_history",
    "get_interpolated_asset_property_values",
    "list_access_policies",
    "list_actions",
    "list_asset_model_composite_models",
    "list_asset_model_properties",
    "list_asset_models",
    "list_asset_properties",
    "list_asset_relationships",
    "list_assets",
    "list_associated_assets",
    "list_bulk_import_jobs",
    "list_composition_relationships",
    "list_computation_model_data_binding_usages",
    "list_computation_model_resolve_to_resources",
    "list_computation_models",
    "list_dashboards",
    "list_datasets",
    "list_executions",
    "list_gateways",
    "list_interface_relationships",
    "list_portals",
    "list_project_assets",
    "list_projects",
    "list_time_series",
]
```
## WaiterName

```python
# WaiterName usage example
from types_aiobotocore_iotsitewise.literals import WaiterName

def get_value() -> WaiterName:
    return "asset_active"
```

```python
# WaiterName definition
WaiterName = Literal[
    "asset_active",
    "asset_model_active",
    "asset_model_not_exists",
    "asset_not_exists",
    "portal_active",
    "portal_not_exists",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_iotsitewise.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition
RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-south-1",
    "ap-southeast-1",
    "ap-southeast-2",
    "ca-central-1",
    "eu-central-1",
    "eu-west-1",
    "us-east-1",
    "us-east-2",
    "us-west-2",
]
```

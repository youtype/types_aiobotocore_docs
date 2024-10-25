# Literals

> [Index](../README.md) > [DataZone](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [DataZone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
    type annotations stubs module [types-aiobotocore-datazone](https://pypi.org/project/types-aiobotocore-datazone/).

## AcceptRuleBehaviorType

```python
# AcceptRuleBehaviorType usage example

from types_aiobotocore_datazone.literals import AcceptRuleBehaviorType

def get_value() -> AcceptRuleBehaviorType:
    return "ALL"
```

```python
# AcceptRuleBehaviorType definition

AcceptRuleBehaviorType = Literal[
    "ALL",
    "NONE",
]
```
## AuthTypeType

```python
# AuthTypeType usage example

from types_aiobotocore_datazone.literals import AuthTypeType

def get_value() -> AuthTypeType:
    return "DISABLED"
```

```python
# AuthTypeType definition

AuthTypeType = Literal[
    "DISABLED",
    "IAM_IDC",
]
```
## ChangeActionType

```python
# ChangeActionType usage example

from types_aiobotocore_datazone.literals import ChangeActionType

def get_value() -> ChangeActionType:
    return "PUBLISH"
```

```python
# ChangeActionType definition

ChangeActionType = Literal[
    "PUBLISH",
    "UNPUBLISH",
]
```
## ConfigurableActionTypeAuthorizationType

```python
# ConfigurableActionTypeAuthorizationType usage example

from types_aiobotocore_datazone.literals import ConfigurableActionTypeAuthorizationType

def get_value() -> ConfigurableActionTypeAuthorizationType:
    return "HTTPS"
```

```python
# ConfigurableActionTypeAuthorizationType definition

ConfigurableActionTypeAuthorizationType = Literal[
    "HTTPS",
    "IAM",
]
```
## DataAssetActivityStatusType

```python
# DataAssetActivityStatusType usage example

from types_aiobotocore_datazone.literals import DataAssetActivityStatusType

def get_value() -> DataAssetActivityStatusType:
    return "FAILED"
```

```python
# DataAssetActivityStatusType definition

DataAssetActivityStatusType = Literal[
    "FAILED",
    "PUBLISHING_FAILED",
    "SKIPPED_ALREADY_IMPORTED",
    "SKIPPED_ARCHIVED",
    "SKIPPED_NO_ACCESS",
    "SUCCEEDED_CREATED",
    "SUCCEEDED_UPDATED",
    "UNCHANGED",
]
```
## DataProductItemTypeType

```python
# DataProductItemTypeType usage example

from types_aiobotocore_datazone.literals import DataProductItemTypeType

def get_value() -> DataProductItemTypeType:
    return "ASSET"
```

```python
# DataProductItemTypeType definition

DataProductItemTypeType = Literal[
    "ASSET",
]
```
## DataProductStatusType

```python
# DataProductStatusType usage example

from types_aiobotocore_datazone.literals import DataProductStatusType

def get_value() -> DataProductStatusType:
    return "CREATED"
```

```python
# DataProductStatusType definition

DataProductStatusType = Literal[
    "CREATE_FAILED",
    "CREATED",
    "CREATING",
]
```
## DataSourceErrorTypeType

```python
# DataSourceErrorTypeType usage example

from types_aiobotocore_datazone.literals import DataSourceErrorTypeType

def get_value() -> DataSourceErrorTypeType:
    return "ACCESS_DENIED_EXCEPTION"
```

```python
# DataSourceErrorTypeType definition

DataSourceErrorTypeType = Literal[
    "ACCESS_DENIED_EXCEPTION",
    "CONFLICT_EXCEPTION",
    "INTERNAL_SERVER_EXCEPTION",
    "RESOURCE_NOT_FOUND_EXCEPTION",
    "SERVICE_QUOTA_EXCEEDED_EXCEPTION",
    "THROTTLING_EXCEPTION",
    "VALIDATION_EXCEPTION",
]
```
## DataSourceRunStatusType

```python
# DataSourceRunStatusType usage example

from types_aiobotocore_datazone.literals import DataSourceRunStatusType

def get_value() -> DataSourceRunStatusType:
    return "FAILED"
```

```python
# DataSourceRunStatusType definition

DataSourceRunStatusType = Literal[
    "FAILED",
    "PARTIALLY_SUCCEEDED",
    "REQUESTED",
    "RUNNING",
    "SUCCESS",
]
```
## DataSourceRunTypeType

```python
# DataSourceRunTypeType usage example

from types_aiobotocore_datazone.literals import DataSourceRunTypeType

def get_value() -> DataSourceRunTypeType:
    return "PRIORITIZED"
```

```python
# DataSourceRunTypeType definition

DataSourceRunTypeType = Literal[
    "PRIORITIZED",
    "SCHEDULED",
]
```
## DataSourceStatusType

```python
# DataSourceStatusType usage example

from types_aiobotocore_datazone.literals import DataSourceStatusType

def get_value() -> DataSourceStatusType:
    return "CREATING"
```

```python
# DataSourceStatusType definition

DataSourceStatusType = Literal[
    "CREATING",
    "DELETING",
    "FAILED_CREATION",
    "FAILED_DELETION",
    "FAILED_UPDATE",
    "READY",
    "RUNNING",
    "UPDATING",
]
```
## DataZoneEntityTypeType

```python
# DataZoneEntityTypeType usage example

from types_aiobotocore_datazone.literals import DataZoneEntityTypeType

def get_value() -> DataZoneEntityTypeType:
    return "DOMAIN_UNIT"
```

```python
# DataZoneEntityTypeType definition

DataZoneEntityTypeType = Literal[
    "DOMAIN_UNIT",
]
```
## DeploymentStatusType

```python
# DeploymentStatusType usage example

from types_aiobotocore_datazone.literals import DeploymentStatusType

def get_value() -> DeploymentStatusType:
    return "FAILED"
```

```python
# DeploymentStatusType definition

DeploymentStatusType = Literal[
    "FAILED",
    "IN_PROGRESS",
    "PENDING_DEPLOYMENT",
    "SUCCESSFUL",
]
```
## DeploymentTypeType

```python
# DeploymentTypeType usage example

from types_aiobotocore_datazone.literals import DeploymentTypeType

def get_value() -> DeploymentTypeType:
    return "CREATE"
```

```python
# DeploymentTypeType definition

DeploymentTypeType = Literal[
    "CREATE",
    "DELETE",
    "UPDATE",
]
```
## DomainStatusType

```python
# DomainStatusType usage example

from types_aiobotocore_datazone.literals import DomainStatusType

def get_value() -> DomainStatusType:
    return "AVAILABLE"
```

```python
# DomainStatusType definition

DomainStatusType = Literal[
    "AVAILABLE",
    "CREATING",
    "CREATION_FAILED",
    "DELETED",
    "DELETING",
    "DELETION_FAILED",
]
```
## DomainUnitDesignationType

```python
# DomainUnitDesignationType usage example

from types_aiobotocore_datazone.literals import DomainUnitDesignationType

def get_value() -> DomainUnitDesignationType:
    return "OWNER"
```

```python
# DomainUnitDesignationType definition

DomainUnitDesignationType = Literal[
    "OWNER",
]
```
## EdgeDirectionType

```python
# EdgeDirectionType usage example

from types_aiobotocore_datazone.literals import EdgeDirectionType

def get_value() -> EdgeDirectionType:
    return "DOWNSTREAM"
```

```python
# EdgeDirectionType definition

EdgeDirectionType = Literal[
    "DOWNSTREAM",
    "UPSTREAM",
]
```
## EnableSettingType

```python
# EnableSettingType usage example

from types_aiobotocore_datazone.literals import EnableSettingType

def get_value() -> EnableSettingType:
    return "DISABLED"
```

```python
# EnableSettingType definition

EnableSettingType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## EntityTypeType

```python
# EntityTypeType usage example

from types_aiobotocore_datazone.literals import EntityTypeType

def get_value() -> EntityTypeType:
    return "ASSET"
```

```python
# EntityTypeType definition

EntityTypeType = Literal[
    "ASSET",
    "DATA_PRODUCT",
]
```
## EnvironmentStatusType

```python
# EnvironmentStatusType usage example

from types_aiobotocore_datazone.literals import EnvironmentStatusType

def get_value() -> EnvironmentStatusType:
    return "ACTIVE"
```

```python
# EnvironmentStatusType definition

EnvironmentStatusType = Literal[
    "ACTIVE",
    "CREATE_FAILED",
    "CREATING",
    "DELETE_FAILED",
    "DELETED",
    "DELETING",
    "DISABLED",
    "EXPIRED",
    "INACCESSIBLE",
    "SUSPENDED",
    "UPDATE_FAILED",
    "UPDATING",
    "VALIDATION_FAILED",
]
```
## FilterExpressionTypeType

```python
# FilterExpressionTypeType usage example

from types_aiobotocore_datazone.literals import FilterExpressionTypeType

def get_value() -> FilterExpressionTypeType:
    return "EXCLUDE"
```

```python
# FilterExpressionTypeType definition

FilterExpressionTypeType = Literal[
    "EXCLUDE",
    "INCLUDE",
]
```
## FilterStatusType

```python
# FilterStatusType usage example

from types_aiobotocore_datazone.literals import FilterStatusType

def get_value() -> FilterStatusType:
    return "INVALID"
```

```python
# FilterStatusType definition

FilterStatusType = Literal[
    "INVALID",
    "VALID",
]
```
## FormTypeStatusType

```python
# FormTypeStatusType usage example

from types_aiobotocore_datazone.literals import FormTypeStatusType

def get_value() -> FormTypeStatusType:
    return "DISABLED"
```

```python
# FormTypeStatusType definition

FormTypeStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## GlossaryStatusType

```python
# GlossaryStatusType usage example

from types_aiobotocore_datazone.literals import GlossaryStatusType

def get_value() -> GlossaryStatusType:
    return "DISABLED"
```

```python
# GlossaryStatusType definition

GlossaryStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## GlossaryTermStatusType

```python
# GlossaryTermStatusType usage example

from types_aiobotocore_datazone.literals import GlossaryTermStatusType

def get_value() -> GlossaryTermStatusType:
    return "DISABLED"
```

```python
# GlossaryTermStatusType definition

GlossaryTermStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## GroupProfileStatusType

```python
# GroupProfileStatusType usage example

from types_aiobotocore_datazone.literals import GroupProfileStatusType

def get_value() -> GroupProfileStatusType:
    return "ASSIGNED"
```

```python
# GroupProfileStatusType definition

GroupProfileStatusType = Literal[
    "ASSIGNED",
    "NOT_ASSIGNED",
]
```
## GroupSearchTypeType

```python
# GroupSearchTypeType usage example

from types_aiobotocore_datazone.literals import GroupSearchTypeType

def get_value() -> GroupSearchTypeType:
    return "DATAZONE_SSO_GROUP"
```

```python
# GroupSearchTypeType definition

GroupSearchTypeType = Literal[
    "DATAZONE_SSO_GROUP",
    "SSO_GROUP",
]
```
## InventorySearchScopeType

```python
# InventorySearchScopeType usage example

from types_aiobotocore_datazone.literals import InventorySearchScopeType

def get_value() -> InventorySearchScopeType:
    return "ASSET"
```

```python
# InventorySearchScopeType definition

InventorySearchScopeType = Literal[
    "ASSET",
    "DATA_PRODUCT",
    "GLOSSARY",
    "GLOSSARY_TERM",
]
```
## ListAssetFiltersPaginatorName

```python
# ListAssetFiltersPaginatorName usage example

from types_aiobotocore_datazone.literals import ListAssetFiltersPaginatorName

def get_value() -> ListAssetFiltersPaginatorName:
    return "list_asset_filters"
```

```python
# ListAssetFiltersPaginatorName definition

ListAssetFiltersPaginatorName = Literal[
    "list_asset_filters",
]
```
## ListAssetRevisionsPaginatorName

```python
# ListAssetRevisionsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListAssetRevisionsPaginatorName

def get_value() -> ListAssetRevisionsPaginatorName:
    return "list_asset_revisions"
```

```python
# ListAssetRevisionsPaginatorName definition

ListAssetRevisionsPaginatorName = Literal[
    "list_asset_revisions",
]
```
## ListDataProductRevisionsPaginatorName

```python
# ListDataProductRevisionsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListDataProductRevisionsPaginatorName

def get_value() -> ListDataProductRevisionsPaginatorName:
    return "list_data_product_revisions"
```

```python
# ListDataProductRevisionsPaginatorName definition

ListDataProductRevisionsPaginatorName = Literal[
    "list_data_product_revisions",
]
```
## ListDataSourceRunActivitiesPaginatorName

```python
# ListDataSourceRunActivitiesPaginatorName usage example

from types_aiobotocore_datazone.literals import ListDataSourceRunActivitiesPaginatorName

def get_value() -> ListDataSourceRunActivitiesPaginatorName:
    return "list_data_source_run_activities"
```

```python
# ListDataSourceRunActivitiesPaginatorName definition

ListDataSourceRunActivitiesPaginatorName = Literal[
    "list_data_source_run_activities",
]
```
## ListDataSourceRunsPaginatorName

```python
# ListDataSourceRunsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListDataSourceRunsPaginatorName

def get_value() -> ListDataSourceRunsPaginatorName:
    return "list_data_source_runs"
```

```python
# ListDataSourceRunsPaginatorName definition

ListDataSourceRunsPaginatorName = Literal[
    "list_data_source_runs",
]
```
## ListDataSourcesPaginatorName

```python
# ListDataSourcesPaginatorName usage example

from types_aiobotocore_datazone.literals import ListDataSourcesPaginatorName

def get_value() -> ListDataSourcesPaginatorName:
    return "list_data_sources"
```

```python
# ListDataSourcesPaginatorName definition

ListDataSourcesPaginatorName = Literal[
    "list_data_sources",
]
```
## ListDomainUnitsForParentPaginatorName

```python
# ListDomainUnitsForParentPaginatorName usage example

from types_aiobotocore_datazone.literals import ListDomainUnitsForParentPaginatorName

def get_value() -> ListDomainUnitsForParentPaginatorName:
    return "list_domain_units_for_parent"
```

```python
# ListDomainUnitsForParentPaginatorName definition

ListDomainUnitsForParentPaginatorName = Literal[
    "list_domain_units_for_parent",
]
```
## ListDomainsPaginatorName

```python
# ListDomainsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListDomainsPaginatorName

def get_value() -> ListDomainsPaginatorName:
    return "list_domains"
```

```python
# ListDomainsPaginatorName definition

ListDomainsPaginatorName = Literal[
    "list_domains",
]
```
## ListEntityOwnersPaginatorName

```python
# ListEntityOwnersPaginatorName usage example

from types_aiobotocore_datazone.literals import ListEntityOwnersPaginatorName

def get_value() -> ListEntityOwnersPaginatorName:
    return "list_entity_owners"
```

```python
# ListEntityOwnersPaginatorName definition

ListEntityOwnersPaginatorName = Literal[
    "list_entity_owners",
]
```
## ListEnvironmentActionsPaginatorName

```python
# ListEnvironmentActionsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListEnvironmentActionsPaginatorName

def get_value() -> ListEnvironmentActionsPaginatorName:
    return "list_environment_actions"
```

```python
# ListEnvironmentActionsPaginatorName definition

ListEnvironmentActionsPaginatorName = Literal[
    "list_environment_actions",
]
```
## ListEnvironmentBlueprintConfigurationsPaginatorName

```python
# ListEnvironmentBlueprintConfigurationsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListEnvironmentBlueprintConfigurationsPaginatorName

def get_value() -> ListEnvironmentBlueprintConfigurationsPaginatorName:
    return "list_environment_blueprint_configurations"
```

```python
# ListEnvironmentBlueprintConfigurationsPaginatorName definition

ListEnvironmentBlueprintConfigurationsPaginatorName = Literal[
    "list_environment_blueprint_configurations",
]
```
## ListEnvironmentBlueprintsPaginatorName

```python
# ListEnvironmentBlueprintsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListEnvironmentBlueprintsPaginatorName

def get_value() -> ListEnvironmentBlueprintsPaginatorName:
    return "list_environment_blueprints"
```

```python
# ListEnvironmentBlueprintsPaginatorName definition

ListEnvironmentBlueprintsPaginatorName = Literal[
    "list_environment_blueprints",
]
```
## ListEnvironmentProfilesPaginatorName

```python
# ListEnvironmentProfilesPaginatorName usage example

from types_aiobotocore_datazone.literals import ListEnvironmentProfilesPaginatorName

def get_value() -> ListEnvironmentProfilesPaginatorName:
    return "list_environment_profiles"
```

```python
# ListEnvironmentProfilesPaginatorName definition

ListEnvironmentProfilesPaginatorName = Literal[
    "list_environment_profiles",
]
```
## ListEnvironmentsPaginatorName

```python
# ListEnvironmentsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListEnvironmentsPaginatorName

def get_value() -> ListEnvironmentsPaginatorName:
    return "list_environments"
```

```python
# ListEnvironmentsPaginatorName definition

ListEnvironmentsPaginatorName = Literal[
    "list_environments",
]
```
## ListLineageNodeHistoryPaginatorName

```python
# ListLineageNodeHistoryPaginatorName usage example

from types_aiobotocore_datazone.literals import ListLineageNodeHistoryPaginatorName

def get_value() -> ListLineageNodeHistoryPaginatorName:
    return "list_lineage_node_history"
```

```python
# ListLineageNodeHistoryPaginatorName definition

ListLineageNodeHistoryPaginatorName = Literal[
    "list_lineage_node_history",
]
```
## ListMetadataGenerationRunsPaginatorName

```python
# ListMetadataGenerationRunsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListMetadataGenerationRunsPaginatorName

def get_value() -> ListMetadataGenerationRunsPaginatorName:
    return "list_metadata_generation_runs"
```

```python
# ListMetadataGenerationRunsPaginatorName definition

ListMetadataGenerationRunsPaginatorName = Literal[
    "list_metadata_generation_runs",
]
```
## ListNotificationsPaginatorName

```python
# ListNotificationsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListNotificationsPaginatorName

def get_value() -> ListNotificationsPaginatorName:
    return "list_notifications"
```

```python
# ListNotificationsPaginatorName definition

ListNotificationsPaginatorName = Literal[
    "list_notifications",
]
```
## ListPolicyGrantsPaginatorName

```python
# ListPolicyGrantsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListPolicyGrantsPaginatorName

def get_value() -> ListPolicyGrantsPaginatorName:
    return "list_policy_grants"
```

```python
# ListPolicyGrantsPaginatorName definition

ListPolicyGrantsPaginatorName = Literal[
    "list_policy_grants",
]
```
## ListProjectMembershipsPaginatorName

```python
# ListProjectMembershipsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListProjectMembershipsPaginatorName

def get_value() -> ListProjectMembershipsPaginatorName:
    return "list_project_memberships"
```

```python
# ListProjectMembershipsPaginatorName definition

ListProjectMembershipsPaginatorName = Literal[
    "list_project_memberships",
]
```
## ListProjectsPaginatorName

```python
# ListProjectsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListProjectsPaginatorName

def get_value() -> ListProjectsPaginatorName:
    return "list_projects"
```

```python
# ListProjectsPaginatorName definition

ListProjectsPaginatorName = Literal[
    "list_projects",
]
```
## ListSubscriptionGrantsPaginatorName

```python
# ListSubscriptionGrantsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListSubscriptionGrantsPaginatorName

def get_value() -> ListSubscriptionGrantsPaginatorName:
    return "list_subscription_grants"
```

```python
# ListSubscriptionGrantsPaginatorName definition

ListSubscriptionGrantsPaginatorName = Literal[
    "list_subscription_grants",
]
```
## ListSubscriptionRequestsPaginatorName

```python
# ListSubscriptionRequestsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListSubscriptionRequestsPaginatorName

def get_value() -> ListSubscriptionRequestsPaginatorName:
    return "list_subscription_requests"
```

```python
# ListSubscriptionRequestsPaginatorName definition

ListSubscriptionRequestsPaginatorName = Literal[
    "list_subscription_requests",
]
```
## ListSubscriptionTargetsPaginatorName

```python
# ListSubscriptionTargetsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListSubscriptionTargetsPaginatorName

def get_value() -> ListSubscriptionTargetsPaginatorName:
    return "list_subscription_targets"
```

```python
# ListSubscriptionTargetsPaginatorName definition

ListSubscriptionTargetsPaginatorName = Literal[
    "list_subscription_targets",
]
```
## ListSubscriptionsPaginatorName

```python
# ListSubscriptionsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListSubscriptionsPaginatorName

def get_value() -> ListSubscriptionsPaginatorName:
    return "list_subscriptions"
```

```python
# ListSubscriptionsPaginatorName definition

ListSubscriptionsPaginatorName = Literal[
    "list_subscriptions",
]
```
## ListTimeSeriesDataPointsPaginatorName

```python
# ListTimeSeriesDataPointsPaginatorName usage example

from types_aiobotocore_datazone.literals import ListTimeSeriesDataPointsPaginatorName

def get_value() -> ListTimeSeriesDataPointsPaginatorName:
    return "list_time_series_data_points"
```

```python
# ListTimeSeriesDataPointsPaginatorName definition

ListTimeSeriesDataPointsPaginatorName = Literal[
    "list_time_series_data_points",
]
```
## ListingStatusType

```python
# ListingStatusType usage example

from types_aiobotocore_datazone.literals import ListingStatusType

def get_value() -> ListingStatusType:
    return "ACTIVE"
```

```python
# ListingStatusType definition

ListingStatusType = Literal[
    "ACTIVE",
    "CREATING",
    "INACTIVE",
]
```
## ManagedPolicyTypeType

```python
# ManagedPolicyTypeType usage example

from types_aiobotocore_datazone.literals import ManagedPolicyTypeType

def get_value() -> ManagedPolicyTypeType:
    return "ADD_TO_PROJECT_MEMBER_POOL"
```

```python
# ManagedPolicyTypeType definition

ManagedPolicyTypeType = Literal[
    "ADD_TO_PROJECT_MEMBER_POOL",
    "CREATE_ASSET_TYPE",
    "CREATE_DOMAIN_UNIT",
    "CREATE_ENVIRONMENT",
    "CREATE_ENVIRONMENT_PROFILE",
    "CREATE_FORM_TYPE",
    "CREATE_GLOSSARY",
    "CREATE_PROJECT",
    "DELEGATE_CREATE_ENVIRONMENT_PROFILE",
    "OVERRIDE_DOMAIN_UNIT_OWNERS",
    "OVERRIDE_PROJECT_OWNERS",
]
```
## MetadataGenerationRunStatusType

```python
# MetadataGenerationRunStatusType usage example

from types_aiobotocore_datazone.literals import MetadataGenerationRunStatusType

def get_value() -> MetadataGenerationRunStatusType:
    return "CANCELED"
```

```python
# MetadataGenerationRunStatusType definition

MetadataGenerationRunStatusType = Literal[
    "CANCELED",
    "FAILED",
    "IN_PROGRESS",
    "SUBMITTED",
    "SUCCEEDED",
]
```
## MetadataGenerationRunTypeType

```python
# MetadataGenerationRunTypeType usage example

from types_aiobotocore_datazone.literals import MetadataGenerationRunTypeType

def get_value() -> MetadataGenerationRunTypeType:
    return "BUSINESS_DESCRIPTIONS"
```

```python
# MetadataGenerationRunTypeType definition

MetadataGenerationRunTypeType = Literal[
    "BUSINESS_DESCRIPTIONS",
]
```
## MetadataGenerationTargetTypeType

```python
# MetadataGenerationTargetTypeType usage example

from types_aiobotocore_datazone.literals import MetadataGenerationTargetTypeType

def get_value() -> MetadataGenerationTargetTypeType:
    return "ASSET"
```

```python
# MetadataGenerationTargetTypeType definition

MetadataGenerationTargetTypeType = Literal[
    "ASSET",
]
```
## NotificationResourceTypeType

```python
# NotificationResourceTypeType usage example

from types_aiobotocore_datazone.literals import NotificationResourceTypeType

def get_value() -> NotificationResourceTypeType:
    return "PROJECT"
```

```python
# NotificationResourceTypeType definition

NotificationResourceTypeType = Literal[
    "PROJECT",
]
```
## NotificationRoleType

```python
# NotificationRoleType usage example

from types_aiobotocore_datazone.literals import NotificationRoleType

def get_value() -> NotificationRoleType:
    return "DOMAIN_OWNER"
```

```python
# NotificationRoleType definition

NotificationRoleType = Literal[
    "DOMAIN_OWNER",
    "PROJECT_CONTRIBUTOR",
    "PROJECT_OWNER",
    "PROJECT_SUBSCRIBER",
    "PROJECT_VIEWER",
]
```
## NotificationTypeType

```python
# NotificationTypeType usage example

from types_aiobotocore_datazone.literals import NotificationTypeType

def get_value() -> NotificationTypeType:
    return "EVENT"
```

```python
# NotificationTypeType definition

NotificationTypeType = Literal[
    "EVENT",
    "TASK",
]
```
## ProjectDesignationType

```python
# ProjectDesignationType usage example

from types_aiobotocore_datazone.literals import ProjectDesignationType

def get_value() -> ProjectDesignationType:
    return "CONTRIBUTOR"
```

```python
# ProjectDesignationType definition

ProjectDesignationType = Literal[
    "CONTRIBUTOR",
    "OWNER",
    "PROJECT_CATALOG_STEWARD",
]
```
## ProjectStatusType

```python
# ProjectStatusType usage example

from types_aiobotocore_datazone.literals import ProjectStatusType

def get_value() -> ProjectStatusType:
    return "ACTIVE"
```

```python
# ProjectStatusType definition

ProjectStatusType = Literal[
    "ACTIVE",
    "DELETE_FAILED",
    "DELETING",
]
```
## RejectRuleBehaviorType

```python
# RejectRuleBehaviorType usage example

from types_aiobotocore_datazone.literals import RejectRuleBehaviorType

def get_value() -> RejectRuleBehaviorType:
    return "ALL"
```

```python
# RejectRuleBehaviorType definition

RejectRuleBehaviorType = Literal[
    "ALL",
    "NONE",
]
```
## SearchGroupProfilesPaginatorName

```python
# SearchGroupProfilesPaginatorName usage example

from types_aiobotocore_datazone.literals import SearchGroupProfilesPaginatorName

def get_value() -> SearchGroupProfilesPaginatorName:
    return "search_group_profiles"
```

```python
# SearchGroupProfilesPaginatorName definition

SearchGroupProfilesPaginatorName = Literal[
    "search_group_profiles",
]
```
## SearchListingsPaginatorName

```python
# SearchListingsPaginatorName usage example

from types_aiobotocore_datazone.literals import SearchListingsPaginatorName

def get_value() -> SearchListingsPaginatorName:
    return "search_listings"
```

```python
# SearchListingsPaginatorName definition

SearchListingsPaginatorName = Literal[
    "search_listings",
]
```
## SearchOutputAdditionalAttributeType

```python
# SearchOutputAdditionalAttributeType usage example

from types_aiobotocore_datazone.literals import SearchOutputAdditionalAttributeType

def get_value() -> SearchOutputAdditionalAttributeType:
    return "FORMS"
```

```python
# SearchOutputAdditionalAttributeType definition

SearchOutputAdditionalAttributeType = Literal[
    "FORMS",
    "TIME_SERIES_DATA_POINT_FORMS",
]
```
## SearchPaginatorName

```python
# SearchPaginatorName usage example

from types_aiobotocore_datazone.literals import SearchPaginatorName

def get_value() -> SearchPaginatorName:
    return "search"
```

```python
# SearchPaginatorName definition

SearchPaginatorName = Literal[
    "search",
]
```
## SearchTypesPaginatorName

```python
# SearchTypesPaginatorName usage example

from types_aiobotocore_datazone.literals import SearchTypesPaginatorName

def get_value() -> SearchTypesPaginatorName:
    return "search_types"
```

```python
# SearchTypesPaginatorName definition

SearchTypesPaginatorName = Literal[
    "search_types",
]
```
## SearchUserProfilesPaginatorName

```python
# SearchUserProfilesPaginatorName usage example

from types_aiobotocore_datazone.literals import SearchUserProfilesPaginatorName

def get_value() -> SearchUserProfilesPaginatorName:
    return "search_user_profiles"
```

```python
# SearchUserProfilesPaginatorName definition

SearchUserProfilesPaginatorName = Literal[
    "search_user_profiles",
]
```
## SelfGrantStatusType

```python
# SelfGrantStatusType usage example

from types_aiobotocore_datazone.literals import SelfGrantStatusType

def get_value() -> SelfGrantStatusType:
    return "GRANTED"
```

```python
# SelfGrantStatusType definition

SelfGrantStatusType = Literal[
    "GRANT_FAILED",
    "GRANT_IN_PROGRESS",
    "GRANT_PENDING",
    "GRANTED",
    "REVOKE_FAILED",
    "REVOKE_IN_PROGRESS",
    "REVOKE_PENDING",
]
```
## SortFieldProjectType

```python
# SortFieldProjectType usage example

from types_aiobotocore_datazone.literals import SortFieldProjectType

def get_value() -> SortFieldProjectType:
    return "NAME"
```

```python
# SortFieldProjectType definition

SortFieldProjectType = Literal[
    "NAME",
]
```
## SortKeyType

```python
# SortKeyType usage example

from types_aiobotocore_datazone.literals import SortKeyType

def get_value() -> SortKeyType:
    return "CREATED_AT"
```

```python
# SortKeyType definition

SortKeyType = Literal[
    "CREATED_AT",
    "UPDATED_AT",
]
```
## SortOrderType

```python
# SortOrderType usage example

from types_aiobotocore_datazone.literals import SortOrderType

def get_value() -> SortOrderType:
    return "ASCENDING"
```

```python
# SortOrderType definition

SortOrderType = Literal[
    "ASCENDING",
    "DESCENDING",
]
```
## SubscriptionGrantOverallStatusType

```python
# SubscriptionGrantOverallStatusType usage example

from types_aiobotocore_datazone.literals import SubscriptionGrantOverallStatusType

def get_value() -> SubscriptionGrantOverallStatusType:
    return "COMPLETED"
```

```python
# SubscriptionGrantOverallStatusType definition

SubscriptionGrantOverallStatusType = Literal[
    "COMPLETED",
    "GRANT_AND_REVOKE_FAILED",
    "GRANT_FAILED",
    "IN_PROGRESS",
    "INACCESSIBLE",
    "PENDING",
    "REVOKE_FAILED",
]
```
## SubscriptionGrantStatusType

```python
# SubscriptionGrantStatusType usage example

from types_aiobotocore_datazone.literals import SubscriptionGrantStatusType

def get_value() -> SubscriptionGrantStatusType:
    return "GRANTED"
```

```python
# SubscriptionGrantStatusType definition

SubscriptionGrantStatusType = Literal[
    "GRANT_FAILED",
    "GRANT_IN_PROGRESS",
    "GRANT_PENDING",
    "GRANTED",
    "REVOKE_FAILED",
    "REVOKE_IN_PROGRESS",
    "REVOKE_PENDING",
    "REVOKED",
]
```
## SubscriptionRequestStatusType

```python
# SubscriptionRequestStatusType usage example

from types_aiobotocore_datazone.literals import SubscriptionRequestStatusType

def get_value() -> SubscriptionRequestStatusType:
    return "ACCEPTED"
```

```python
# SubscriptionRequestStatusType definition

SubscriptionRequestStatusType = Literal[
    "ACCEPTED",
    "PENDING",
    "REJECTED",
]
```
## SubscriptionStatusType

```python
# SubscriptionStatusType usage example

from types_aiobotocore_datazone.literals import SubscriptionStatusType

def get_value() -> SubscriptionStatusType:
    return "APPROVED"
```

```python
# SubscriptionStatusType definition

SubscriptionStatusType = Literal[
    "APPROVED",
    "CANCELLED",
    "REVOKED",
]
```
## TargetEntityTypeType

```python
# TargetEntityTypeType usage example

from types_aiobotocore_datazone.literals import TargetEntityTypeType

def get_value() -> TargetEntityTypeType:
    return "DOMAIN_UNIT"
```

```python
# TargetEntityTypeType definition

TargetEntityTypeType = Literal[
    "DOMAIN_UNIT",
    "ENVIRONMENT_BLUEPRINT_CONFIGURATION",
    "ENVIRONMENT_PROFILE",
]
```
## TaskStatusType

```python
# TaskStatusType usage example

from types_aiobotocore_datazone.literals import TaskStatusType

def get_value() -> TaskStatusType:
    return "ACTIVE"
```

```python
# TaskStatusType definition

TaskStatusType = Literal[
    "ACTIVE",
    "INACTIVE",
]
```
## TimeSeriesEntityTypeType

```python
# TimeSeriesEntityTypeType usage example

from types_aiobotocore_datazone.literals import TimeSeriesEntityTypeType

def get_value() -> TimeSeriesEntityTypeType:
    return "ASSET"
```

```python
# TimeSeriesEntityTypeType definition

TimeSeriesEntityTypeType = Literal[
    "ASSET",
    "LISTING",
]
```
## TimezoneType

```python
# TimezoneType usage example

from types_aiobotocore_datazone.literals import TimezoneType

def get_value() -> TimezoneType:
    return "AFRICA_JOHANNESBURG"
```

```python
# TimezoneType definition

TimezoneType = Literal[
    "AFRICA_JOHANNESBURG",
    "AMERICA_MONTREAL",
    "AMERICA_SAO_PAULO",
    "ASIA_BAHRAIN",
    "ASIA_BANGKOK",
    "ASIA_CALCUTTA",
    "ASIA_DUBAI",
    "ASIA_HONG_KONG",
    "ASIA_JAKARTA",
    "ASIA_KUALA_LUMPUR",
    "ASIA_SEOUL",
    "ASIA_SHANGHAI",
    "ASIA_SINGAPORE",
    "ASIA_TAIPEI",
    "ASIA_TOKYO",
    "AUSTRALIA_MELBOURNE",
    "AUSTRALIA_SYDNEY",
    "CANADA_CENTRAL",
    "CET",
    "CST6CDT",
    "ETC_GMT",
    "ETC_GMT0",
    "ETC_GMT_ADD_0",
    "ETC_GMT_ADD_1",
    "ETC_GMT_ADD_10",
    "ETC_GMT_ADD_11",
    "ETC_GMT_ADD_12",
    "ETC_GMT_ADD_2",
    "ETC_GMT_ADD_3",
    "ETC_GMT_ADD_4",
    "ETC_GMT_ADD_5",
    "ETC_GMT_ADD_6",
    "ETC_GMT_ADD_7",
    "ETC_GMT_ADD_8",
    "ETC_GMT_ADD_9",
    "ETC_GMT_NEG_0",
    "ETC_GMT_NEG_1",
    "ETC_GMT_NEG_10",
    "ETC_GMT_NEG_11",
    "ETC_GMT_NEG_12",
    "ETC_GMT_NEG_13",
    "ETC_GMT_NEG_14",
    "ETC_GMT_NEG_2",
    "ETC_GMT_NEG_3",
    "ETC_GMT_NEG_4",
    "ETC_GMT_NEG_5",
    "ETC_GMT_NEG_6",
    "ETC_GMT_NEG_7",
    "ETC_GMT_NEG_8",
    "ETC_GMT_NEG_9",
    "EUROPE_DUBLIN",
    "EUROPE_LONDON",
    "EUROPE_PARIS",
    "EUROPE_STOCKHOLM",
    "EUROPE_ZURICH",
    "ISRAEL",
    "MEXICO_GENERAL",
    "MST7MDT",
    "PACIFIC_AUCKLAND",
    "US_CENTRAL",
    "US_EASTERN",
    "US_MOUNTAIN",
    "US_PACIFIC",
    "UTC",
]
```
## TypesSearchScopeType

```python
# TypesSearchScopeType usage example

from types_aiobotocore_datazone.literals import TypesSearchScopeType

def get_value() -> TypesSearchScopeType:
    return "ASSET_TYPE"
```

```python
# TypesSearchScopeType definition

TypesSearchScopeType = Literal[
    "ASSET_TYPE",
    "FORM_TYPE",
    "LINEAGE_NODE_TYPE",
]
```
## UserAssignmentType

```python
# UserAssignmentType usage example

from types_aiobotocore_datazone.literals import UserAssignmentType

def get_value() -> UserAssignmentType:
    return "AUTOMATIC"
```

```python
# UserAssignmentType definition

UserAssignmentType = Literal[
    "AUTOMATIC",
    "MANUAL",
]
```
## UserDesignationType

```python
# UserDesignationType usage example

from types_aiobotocore_datazone.literals import UserDesignationType

def get_value() -> UserDesignationType:
    return "PROJECT_CATALOG_CONSUMER"
```

```python
# UserDesignationType definition

UserDesignationType = Literal[
    "PROJECT_CATALOG_CONSUMER",
    "PROJECT_CATALOG_STEWARD",
    "PROJECT_CATALOG_VIEWER",
    "PROJECT_CONTRIBUTOR",
    "PROJECT_OWNER",
]
```
## UserProfileStatusType

```python
# UserProfileStatusType usage example

from types_aiobotocore_datazone.literals import UserProfileStatusType

def get_value() -> UserProfileStatusType:
    return "ACTIVATED"
```

```python
# UserProfileStatusType definition

UserProfileStatusType = Literal[
    "ACTIVATED",
    "ASSIGNED",
    "DEACTIVATED",
    "NOT_ASSIGNED",
]
```
## UserProfileTypeType

```python
# UserProfileTypeType usage example

from types_aiobotocore_datazone.literals import UserProfileTypeType

def get_value() -> UserProfileTypeType:
    return "IAM"
```

```python
# UserProfileTypeType definition

UserProfileTypeType = Literal[
    "IAM",
    "SSO",
]
```
## UserSearchTypeType

```python
# UserSearchTypeType usage example

from types_aiobotocore_datazone.literals import UserSearchTypeType

def get_value() -> UserSearchTypeType:
    return "DATAZONE_IAM_USER"
```

```python
# UserSearchTypeType definition

UserSearchTypeType = Literal[
    "DATAZONE_IAM_USER",
    "DATAZONE_SSO_USER",
    "DATAZONE_USER",
    "SSO_USER",
]
```
## UserTypeType

```python
# UserTypeType usage example

from types_aiobotocore_datazone.literals import UserTypeType

def get_value() -> UserTypeType:
    return "IAM_ROLE"
```

```python
# UserTypeType definition

UserTypeType = Literal[
    "IAM_ROLE",
    "IAM_USER",
    "SSO_USER",
]
```
## DataZoneServiceName

```python
# DataZoneServiceName usage example

from types_aiobotocore_datazone.literals import DataZoneServiceName

def get_value() -> DataZoneServiceName:
    return "datazone"
```

```python
# DataZoneServiceName definition

DataZoneServiceName = Literal[
    "datazone",
]
```
## ServiceName

```python
# ServiceName usage example

from types_aiobotocore_datazone.literals import ServiceName

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
    "apptest",
    "arc-zonal-shift",
    "artifact",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "b2bi",
    "backup",
    "backup-gateway",
    "batch",
    "bcm-data-exports",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
    "bedrock-runtime",
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
    "config",
    "connect",
    "connect-contact-lens",
    "connectcampaigns",
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
    "freetier",
    "fsx",
    "gamelift",
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
    "iot",
    "iot-data",
    "iot-jobs-data",
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
    "lookoutmetrics",
    "lookoutvision",
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
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "neptune-graph",
    "neptunedata",
    "network-firewall",
    "networkmanager",
    "networkmonitor",
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
    "privatenetworks",
    "proton",
    "qapps",
    "qbusiness",
    "qconnect",
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
    "repostspace",
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
    "route53profiles",
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
    "socialmessaging",
    "sqs",
    "ssm",
    "ssm-contacts",
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
    "wisdom",
    "workdocs",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-thin-client",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python
# ResourceServiceName usage example

from types_aiobotocore_datazone.literals import ResourceServiceName

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

from types_aiobotocore_datazone.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_asset_filters"
```

```python
# PaginatorName definition

PaginatorName = Literal[
    "list_asset_filters",
    "list_asset_revisions",
    "list_data_product_revisions",
    "list_data_source_run_activities",
    "list_data_source_runs",
    "list_data_sources",
    "list_domain_units_for_parent",
    "list_domains",
    "list_entity_owners",
    "list_environment_actions",
    "list_environment_blueprint_configurations",
    "list_environment_blueprints",
    "list_environment_profiles",
    "list_environments",
    "list_lineage_node_history",
    "list_metadata_generation_runs",
    "list_notifications",
    "list_policy_grants",
    "list_project_memberships",
    "list_projects",
    "list_subscription_grants",
    "list_subscription_requests",
    "list_subscription_targets",
    "list_subscriptions",
    "list_time_series_data_points",
    "search",
    "search_group_profiles",
    "search_listings",
    "search_types",
    "search_user_profiles",
]
```
## RegionName

```python
# RegionName usage example

from types_aiobotocore_datazone.literals import RegionName

def get_value() -> RegionName:
    return "ap-northeast-1"
```

```python
# RegionName definition

RegionName = Literal[
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ap-southeast-4",
    "ap-southeast-5",
    "ca-central-1",
    "ca-west-1",
    "eu-central-1",
    "eu-north-1",
    "eu-south-1",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "me-south-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```

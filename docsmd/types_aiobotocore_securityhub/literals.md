# Literals

> [Index](../README.md) > [SecurityHub](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SecurityHub](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#securityhub)
    type annotations stubs module [types-aiobotocore-securityhub](https://pypi.org/project/types-aiobotocore-securityhub/).

## ActorSessionMfaStatusType

```python
# ActorSessionMfaStatusType usage example
from types_aiobotocore_securityhub.literals import ActorSessionMfaStatusType

def get_value() -> ActorSessionMfaStatusType:
    return "DISABLED"
```

```python
# ActorSessionMfaStatusType definition
ActorSessionMfaStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## AdminStatusType

```python
# AdminStatusType usage example
from types_aiobotocore_securityhub.literals import AdminStatusType

def get_value() -> AdminStatusType:
    return "DISABLE_IN_PROGRESS"
```

```python
# AdminStatusType definition
AdminStatusType = Literal[
    "DISABLE_IN_PROGRESS",
    "ENABLED",
]
```
## AssociationStatusType

```python
# AssociationStatusType usage example
from types_aiobotocore_securityhub.literals import AssociationStatusType

def get_value() -> AssociationStatusType:
    return "DISABLED"
```

```python
# AssociationStatusType definition
AssociationStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## AssociationTypeType

```python
# AssociationTypeType usage example
from types_aiobotocore_securityhub.literals import AssociationTypeType

def get_value() -> AssociationTypeType:
    return "APPLIED"
```

```python
# AssociationTypeType definition
AssociationTypeType = Literal[
    "APPLIED",
    "INHERITED",
]
```
## AutoEnableStandardsType

```python
# AutoEnableStandardsType usage example
from types_aiobotocore_securityhub.literals import AutoEnableStandardsType

def get_value() -> AutoEnableStandardsType:
    return "DEFAULT"
```

```python
# AutoEnableStandardsType definition
AutoEnableStandardsType = Literal[
    "DEFAULT",
    "NONE",
]
```
## AutomationRulesActionTypeType

```python
# AutomationRulesActionTypeType usage example
from types_aiobotocore_securityhub.literals import AutomationRulesActionTypeType

def get_value() -> AutomationRulesActionTypeType:
    return "FINDING_FIELDS_UPDATE"
```

```python
# AutomationRulesActionTypeType definition
AutomationRulesActionTypeType = Literal[
    "FINDING_FIELDS_UPDATE",
]
```
## AwsIamAccessKeyStatusType

```python
# AwsIamAccessKeyStatusType usage example
from types_aiobotocore_securityhub.literals import AwsIamAccessKeyStatusType

def get_value() -> AwsIamAccessKeyStatusType:
    return "Active"
```

```python
# AwsIamAccessKeyStatusType definition
AwsIamAccessKeyStatusType = Literal[
    "Active",
    "Inactive",
]
```
## AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType

```python
# AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType usage example
from types_aiobotocore_securityhub.literals import AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType

def get_value() -> AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType:
    return "Prefix"
```

```python
# AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType definition
AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType = Literal[
    "Prefix",
    "Suffix",
]
```
## ComplianceStatusType

```python
# ComplianceStatusType usage example
from types_aiobotocore_securityhub.literals import ComplianceStatusType

def get_value() -> ComplianceStatusType:
    return "FAILED"
```

```python
# ComplianceStatusType definition
ComplianceStatusType = Literal[
    "FAILED",
    "NOT_AVAILABLE",
    "PASSED",
    "WARNING",
]
```
## ConfigurationPolicyAssociationStatusType

```python
# ConfigurationPolicyAssociationStatusType usage example
from types_aiobotocore_securityhub.literals import ConfigurationPolicyAssociationStatusType

def get_value() -> ConfigurationPolicyAssociationStatusType:
    return "FAILED"
```

```python
# ConfigurationPolicyAssociationStatusType definition
ConfigurationPolicyAssociationStatusType = Literal[
    "FAILED",
    "PENDING",
    "SUCCESS",
]
```
## ConnectionDirectionType

```python
# ConnectionDirectionType usage example
from types_aiobotocore_securityhub.literals import ConnectionDirectionType

def get_value() -> ConnectionDirectionType:
    return "INBOUND"
```

```python
# ConnectionDirectionType definition
ConnectionDirectionType = Literal[
    "INBOUND",
    "OUTBOUND",
]
```
## ControlFindingGeneratorType

```python
# ControlFindingGeneratorType usage example
from types_aiobotocore_securityhub.literals import ControlFindingGeneratorType

def get_value() -> ControlFindingGeneratorType:
    return "SECURITY_CONTROL"
```

```python
# ControlFindingGeneratorType definition
ControlFindingGeneratorType = Literal[
    "SECURITY_CONTROL",
    "STANDARD_CONTROL",
]
```
## ControlStatusType

```python
# ControlStatusType usage example
from types_aiobotocore_securityhub.literals import ControlStatusType

def get_value() -> ControlStatusType:
    return "DISABLED"
```

```python
# ControlStatusType definition
ControlStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## DateRangeUnitType

```python
# DateRangeUnitType usage example
from types_aiobotocore_securityhub.literals import DateRangeUnitType

def get_value() -> DateRangeUnitType:
    return "DAYS"
```

```python
# DateRangeUnitType definition
DateRangeUnitType = Literal[
    "DAYS",
]
```
## DescribeActionTargetsPaginatorName

```python
# DescribeActionTargetsPaginatorName usage example
from types_aiobotocore_securityhub.literals import DescribeActionTargetsPaginatorName

def get_value() -> DescribeActionTargetsPaginatorName:
    return "describe_action_targets"
```

```python
# DescribeActionTargetsPaginatorName definition
DescribeActionTargetsPaginatorName = Literal[
    "describe_action_targets",
]
```
## DescribeProductsPaginatorName

```python
# DescribeProductsPaginatorName usage example
from types_aiobotocore_securityhub.literals import DescribeProductsPaginatorName

def get_value() -> DescribeProductsPaginatorName:
    return "describe_products"
```

```python
# DescribeProductsPaginatorName definition
DescribeProductsPaginatorName = Literal[
    "describe_products",
]
```
## DescribeStandardsControlsPaginatorName

```python
# DescribeStandardsControlsPaginatorName usage example
from types_aiobotocore_securityhub.literals import DescribeStandardsControlsPaginatorName

def get_value() -> DescribeStandardsControlsPaginatorName:
    return "describe_standards_controls"
```

```python
# DescribeStandardsControlsPaginatorName definition
DescribeStandardsControlsPaginatorName = Literal[
    "describe_standards_controls",
]
```
## DescribeStandardsPaginatorName

```python
# DescribeStandardsPaginatorName usage example
from types_aiobotocore_securityhub.literals import DescribeStandardsPaginatorName

def get_value() -> DescribeStandardsPaginatorName:
    return "describe_standards"
```

```python
# DescribeStandardsPaginatorName definition
DescribeStandardsPaginatorName = Literal[
    "describe_standards",
]
```
## FindingHistoryUpdateSourceTypeType

```python
# FindingHistoryUpdateSourceTypeType usage example
from types_aiobotocore_securityhub.literals import FindingHistoryUpdateSourceTypeType

def get_value() -> FindingHistoryUpdateSourceTypeType:
    return "BATCH_IMPORT_FINDINGS"
```

```python
# FindingHistoryUpdateSourceTypeType definition
FindingHistoryUpdateSourceTypeType = Literal[
    "BATCH_IMPORT_FINDINGS",
    "BATCH_UPDATE_FINDINGS",
]
```
## GetEnabledStandardsPaginatorName

```python
# GetEnabledStandardsPaginatorName usage example
from types_aiobotocore_securityhub.literals import GetEnabledStandardsPaginatorName

def get_value() -> GetEnabledStandardsPaginatorName:
    return "get_enabled_standards"
```

```python
# GetEnabledStandardsPaginatorName definition
GetEnabledStandardsPaginatorName = Literal[
    "get_enabled_standards",
]
```
## GetFindingHistoryPaginatorName

```python
# GetFindingHistoryPaginatorName usage example
from types_aiobotocore_securityhub.literals import GetFindingHistoryPaginatorName

def get_value() -> GetFindingHistoryPaginatorName:
    return "get_finding_history"
```

```python
# GetFindingHistoryPaginatorName definition
GetFindingHistoryPaginatorName = Literal[
    "get_finding_history",
]
```
## GetFindingsPaginatorName

```python
# GetFindingsPaginatorName usage example
from types_aiobotocore_securityhub.literals import GetFindingsPaginatorName

def get_value() -> GetFindingsPaginatorName:
    return "get_findings"
```

```python
# GetFindingsPaginatorName definition
GetFindingsPaginatorName = Literal[
    "get_findings",
]
```
## GetInsightsPaginatorName

```python
# GetInsightsPaginatorName usage example
from types_aiobotocore_securityhub.literals import GetInsightsPaginatorName

def get_value() -> GetInsightsPaginatorName:
    return "get_insights"
```

```python
# GetInsightsPaginatorName definition
GetInsightsPaginatorName = Literal[
    "get_insights",
]
```
## IntegrationTypeType

```python
# IntegrationTypeType usage example
from types_aiobotocore_securityhub.literals import IntegrationTypeType

def get_value() -> IntegrationTypeType:
    return "RECEIVE_FINDINGS_FROM_SECURITY_HUB"
```

```python
# IntegrationTypeType definition
IntegrationTypeType = Literal[
    "RECEIVE_FINDINGS_FROM_SECURITY_HUB",
    "SEND_FINDINGS_TO_SECURITY_HUB",
    "UPDATE_FINDINGS_IN_SECURITY_HUB",
]
```
## ListConfigurationPoliciesPaginatorName

```python
# ListConfigurationPoliciesPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListConfigurationPoliciesPaginatorName

def get_value() -> ListConfigurationPoliciesPaginatorName:
    return "list_configuration_policies"
```

```python
# ListConfigurationPoliciesPaginatorName definition
ListConfigurationPoliciesPaginatorName = Literal[
    "list_configuration_policies",
]
```
## ListConfigurationPolicyAssociationsPaginatorName

```python
# ListConfigurationPolicyAssociationsPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListConfigurationPolicyAssociationsPaginatorName

def get_value() -> ListConfigurationPolicyAssociationsPaginatorName:
    return "list_configuration_policy_associations"
```

```python
# ListConfigurationPolicyAssociationsPaginatorName definition
ListConfigurationPolicyAssociationsPaginatorName = Literal[
    "list_configuration_policy_associations",
]
```
## ListEnabledProductsForImportPaginatorName

```python
# ListEnabledProductsForImportPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListEnabledProductsForImportPaginatorName

def get_value() -> ListEnabledProductsForImportPaginatorName:
    return "list_enabled_products_for_import"
```

```python
# ListEnabledProductsForImportPaginatorName definition
ListEnabledProductsForImportPaginatorName = Literal[
    "list_enabled_products_for_import",
]
```
## ListFindingAggregatorsPaginatorName

```python
# ListFindingAggregatorsPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListFindingAggregatorsPaginatorName

def get_value() -> ListFindingAggregatorsPaginatorName:
    return "list_finding_aggregators"
```

```python
# ListFindingAggregatorsPaginatorName definition
ListFindingAggregatorsPaginatorName = Literal[
    "list_finding_aggregators",
]
```
## ListInvitationsPaginatorName

```python
# ListInvitationsPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListInvitationsPaginatorName

def get_value() -> ListInvitationsPaginatorName:
    return "list_invitations"
```

```python
# ListInvitationsPaginatorName definition
ListInvitationsPaginatorName = Literal[
    "list_invitations",
]
```
## ListMembersPaginatorName

```python
# ListMembersPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListMembersPaginatorName

def get_value() -> ListMembersPaginatorName:
    return "list_members"
```

```python
# ListMembersPaginatorName definition
ListMembersPaginatorName = Literal[
    "list_members",
]
```
## ListOrganizationAdminAccountsPaginatorName

```python
# ListOrganizationAdminAccountsPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListOrganizationAdminAccountsPaginatorName

def get_value() -> ListOrganizationAdminAccountsPaginatorName:
    return "list_organization_admin_accounts"
```

```python
# ListOrganizationAdminAccountsPaginatorName definition
ListOrganizationAdminAccountsPaginatorName = Literal[
    "list_organization_admin_accounts",
]
```
## ListSecurityControlDefinitionsPaginatorName

```python
# ListSecurityControlDefinitionsPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListSecurityControlDefinitionsPaginatorName

def get_value() -> ListSecurityControlDefinitionsPaginatorName:
    return "list_security_control_definitions"
```

```python
# ListSecurityControlDefinitionsPaginatorName definition
ListSecurityControlDefinitionsPaginatorName = Literal[
    "list_security_control_definitions",
]
```
## ListStandardsControlAssociationsPaginatorName

```python
# ListStandardsControlAssociationsPaginatorName usage example
from types_aiobotocore_securityhub.literals import ListStandardsControlAssociationsPaginatorName

def get_value() -> ListStandardsControlAssociationsPaginatorName:
    return "list_standards_control_associations"
```

```python
# ListStandardsControlAssociationsPaginatorName definition
ListStandardsControlAssociationsPaginatorName = Literal[
    "list_standards_control_associations",
]
```
## MalwareStateType

```python
# MalwareStateType usage example
from types_aiobotocore_securityhub.literals import MalwareStateType

def get_value() -> MalwareStateType:
    return "OBSERVED"
```

```python
# MalwareStateType definition
MalwareStateType = Literal[
    "OBSERVED",
    "REMOVAL_FAILED",
    "REMOVED",
]
```
## MalwareTypeType

```python
# MalwareTypeType usage example
from types_aiobotocore_securityhub.literals import MalwareTypeType

def get_value() -> MalwareTypeType:
    return "ADWARE"
```

```python
# MalwareTypeType definition
MalwareTypeType = Literal[
    "ADWARE",
    "BLENDED_THREAT",
    "BOTNET_AGENT",
    "COIN_MINER",
    "EXPLOIT_KIT",
    "KEYLOGGER",
    "MACRO",
    "POTENTIALLY_UNWANTED",
    "RANSOMWARE",
    "REMOTE_ACCESS",
    "ROOTKIT",
    "SPYWARE",
    "TROJAN",
    "VIRUS",
    "WORM",
]
```
## MapFilterComparisonType

```python
# MapFilterComparisonType usage example
from types_aiobotocore_securityhub.literals import MapFilterComparisonType

def get_value() -> MapFilterComparisonType:
    return "CONTAINS"
```

```python
# MapFilterComparisonType definition
MapFilterComparisonType = Literal[
    "CONTAINS",
    "EQUALS",
    "NOT_CONTAINS",
    "NOT_EQUALS",
]
```
## NetworkDirectionType

```python
# NetworkDirectionType usage example
from types_aiobotocore_securityhub.literals import NetworkDirectionType

def get_value() -> NetworkDirectionType:
    return "IN"
```

```python
# NetworkDirectionType definition
NetworkDirectionType = Literal[
    "IN",
    "OUT",
]
```
## OrganizationConfigurationConfigurationTypeType

```python
# OrganizationConfigurationConfigurationTypeType usage example
from types_aiobotocore_securityhub.literals import OrganizationConfigurationConfigurationTypeType

def get_value() -> OrganizationConfigurationConfigurationTypeType:
    return "CENTRAL"
```

```python
# OrganizationConfigurationConfigurationTypeType definition
OrganizationConfigurationConfigurationTypeType = Literal[
    "CENTRAL",
    "LOCAL",
]
```
## OrganizationConfigurationStatusType

```python
# OrganizationConfigurationStatusType usage example
from types_aiobotocore_securityhub.literals import OrganizationConfigurationStatusType

def get_value() -> OrganizationConfigurationStatusType:
    return "ENABLED"
```

```python
# OrganizationConfigurationStatusType definition
OrganizationConfigurationStatusType = Literal[
    "ENABLED",
    "FAILED",
    "PENDING",
]
```
## ParameterValueTypeType

```python
# ParameterValueTypeType usage example
from types_aiobotocore_securityhub.literals import ParameterValueTypeType

def get_value() -> ParameterValueTypeType:
    return "CUSTOM"
```

```python
# ParameterValueTypeType definition
ParameterValueTypeType = Literal[
    "CUSTOM",
    "DEFAULT",
]
```
## PartitionType

```python
# PartitionType usage example
from types_aiobotocore_securityhub.literals import PartitionType

def get_value() -> PartitionType:
    return "aws"
```

```python
# PartitionType definition
PartitionType = Literal[
    "aws",
    "aws-cn",
    "aws-us-gov",
]
```
## RecordStateType

```python
# RecordStateType usage example
from types_aiobotocore_securityhub.literals import RecordStateType

def get_value() -> RecordStateType:
    return "ACTIVE"
```

```python
# RecordStateType definition
RecordStateType = Literal[
    "ACTIVE",
    "ARCHIVED",
]
```
## RegionAvailabilityStatusType

```python
# RegionAvailabilityStatusType usage example
from types_aiobotocore_securityhub.literals import RegionAvailabilityStatusType

def get_value() -> RegionAvailabilityStatusType:
    return "AVAILABLE"
```

```python
# RegionAvailabilityStatusType definition
RegionAvailabilityStatusType = Literal[
    "AVAILABLE",
    "UNAVAILABLE",
]
```
## RuleStatusType

```python
# RuleStatusType usage example
from types_aiobotocore_securityhub.literals import RuleStatusType

def get_value() -> RuleStatusType:
    return "DISABLED"
```

```python
# RuleStatusType definition
RuleStatusType = Literal[
    "DISABLED",
    "ENABLED",
]
```
## SecurityControlPropertyType

```python
# SecurityControlPropertyType usage example
from types_aiobotocore_securityhub.literals import SecurityControlPropertyType

def get_value() -> SecurityControlPropertyType:
    return "Parameters"
```

```python
# SecurityControlPropertyType definition
SecurityControlPropertyType = Literal[
    "Parameters",
]
```
## SeverityLabelType

```python
# SeverityLabelType usage example
from types_aiobotocore_securityhub.literals import SeverityLabelType

def get_value() -> SeverityLabelType:
    return "CRITICAL"
```

```python
# SeverityLabelType definition
SeverityLabelType = Literal[
    "CRITICAL",
    "HIGH",
    "INFORMATIONAL",
    "LOW",
    "MEDIUM",
]
```
## SeverityRatingType

```python
# SeverityRatingType usage example
from types_aiobotocore_securityhub.literals import SeverityRatingType

def get_value() -> SeverityRatingType:
    return "CRITICAL"
```

```python
# SeverityRatingType definition
SeverityRatingType = Literal[
    "CRITICAL",
    "HIGH",
    "LOW",
    "MEDIUM",
]
```
## SortOrderType

```python
# SortOrderType usage example
from types_aiobotocore_securityhub.literals import SortOrderType

def get_value() -> SortOrderType:
    return "asc"
```

```python
# SortOrderType definition
SortOrderType = Literal[
    "asc",
    "desc",
]
```
## StandardsStatusType

```python
# StandardsStatusType usage example
from types_aiobotocore_securityhub.literals import StandardsStatusType

def get_value() -> StandardsStatusType:
    return "DELETING"
```

```python
# StandardsStatusType definition
StandardsStatusType = Literal[
    "DELETING",
    "FAILED",
    "INCOMPLETE",
    "PENDING",
    "READY",
]
```
## StatusReasonCodeType

```python
# StatusReasonCodeType usage example
from types_aiobotocore_securityhub.literals import StatusReasonCodeType

def get_value() -> StatusReasonCodeType:
    return "INTERNAL_ERROR"
```

```python
# StatusReasonCodeType definition
StatusReasonCodeType = Literal[
    "INTERNAL_ERROR",
    "NO_AVAILABLE_CONFIGURATION_RECORDER",
]
```
## StringFilterComparisonType

```python
# StringFilterComparisonType usage example
from types_aiobotocore_securityhub.literals import StringFilterComparisonType

def get_value() -> StringFilterComparisonType:
    return "CONTAINS"
```

```python
# StringFilterComparisonType definition
StringFilterComparisonType = Literal[
    "CONTAINS",
    "EQUALS",
    "NOT_CONTAINS",
    "NOT_EQUALS",
    "PREFIX",
    "PREFIX_NOT_EQUALS",
]
```
## TargetTypeType

```python
# TargetTypeType usage example
from types_aiobotocore_securityhub.literals import TargetTypeType

def get_value() -> TargetTypeType:
    return "ACCOUNT"
```

```python
# TargetTypeType definition
TargetTypeType = Literal[
    "ACCOUNT",
    "ORGANIZATIONAL_UNIT",
    "ROOT",
]
```
## ThreatIntelIndicatorCategoryType

```python
# ThreatIntelIndicatorCategoryType usage example
from types_aiobotocore_securityhub.literals import ThreatIntelIndicatorCategoryType

def get_value() -> ThreatIntelIndicatorCategoryType:
    return "BACKDOOR"
```

```python
# ThreatIntelIndicatorCategoryType definition
ThreatIntelIndicatorCategoryType = Literal[
    "BACKDOOR",
    "CARD_STEALER",
    "COMMAND_AND_CONTROL",
    "DROP_SITE",
    "EXPLOIT_SITE",
    "KEYLOGGER",
]
```
## ThreatIntelIndicatorTypeType

```python
# ThreatIntelIndicatorTypeType usage example
from types_aiobotocore_securityhub.literals import ThreatIntelIndicatorTypeType

def get_value() -> ThreatIntelIndicatorTypeType:
    return "DOMAIN"
```

```python
# ThreatIntelIndicatorTypeType definition
ThreatIntelIndicatorTypeType = Literal[
    "DOMAIN",
    "EMAIL_ADDRESS",
    "HASH_MD5",
    "HASH_SHA1",
    "HASH_SHA256",
    "HASH_SHA512",
    "IPV4_ADDRESS",
    "IPV6_ADDRESS",
    "MUTEX",
    "PROCESS",
    "URL",
]
```
## UnprocessedErrorCodeType

```python
# UnprocessedErrorCodeType usage example
from types_aiobotocore_securityhub.literals import UnprocessedErrorCodeType

def get_value() -> UnprocessedErrorCodeType:
    return "ACCESS_DENIED"
```

```python
# UnprocessedErrorCodeType definition
UnprocessedErrorCodeType = Literal[
    "ACCESS_DENIED",
    "INVALID_INPUT",
    "LIMIT_EXCEEDED",
    "NOT_FOUND",
]
```
## UpdateStatusType

```python
# UpdateStatusType usage example
from types_aiobotocore_securityhub.literals import UpdateStatusType

def get_value() -> UpdateStatusType:
    return "READY"
```

```python
# UpdateStatusType definition
UpdateStatusType = Literal[
    "READY",
    "UPDATING",
]
```
## VerificationStateType

```python
# VerificationStateType usage example
from types_aiobotocore_securityhub.literals import VerificationStateType

def get_value() -> VerificationStateType:
    return "BENIGN_POSITIVE"
```

```python
# VerificationStateType definition
VerificationStateType = Literal[
    "BENIGN_POSITIVE",
    "FALSE_POSITIVE",
    "TRUE_POSITIVE",
    "UNKNOWN",
]
```
## VulnerabilityExploitAvailableType

```python
# VulnerabilityExploitAvailableType usage example
from types_aiobotocore_securityhub.literals import VulnerabilityExploitAvailableType

def get_value() -> VulnerabilityExploitAvailableType:
    return "NO"
```

```python
# VulnerabilityExploitAvailableType definition
VulnerabilityExploitAvailableType = Literal[
    "NO",
    "YES",
]
```
## VulnerabilityFixAvailableType

```python
# VulnerabilityFixAvailableType usage example
from types_aiobotocore_securityhub.literals import VulnerabilityFixAvailableType

def get_value() -> VulnerabilityFixAvailableType:
    return "NO"
```

```python
# VulnerabilityFixAvailableType definition
VulnerabilityFixAvailableType = Literal[
    "NO",
    "PARTIAL",
    "YES",
]
```
## WorkflowStateType

```python
# WorkflowStateType usage example
from types_aiobotocore_securityhub.literals import WorkflowStateType

def get_value() -> WorkflowStateType:
    return "ASSIGNED"
```

```python
# WorkflowStateType definition
WorkflowStateType = Literal[
    "ASSIGNED",
    "DEFERRED",
    "IN_PROGRESS",
    "NEW",
    "RESOLVED",
]
```
## WorkflowStatusType

```python
# WorkflowStatusType usage example
from types_aiobotocore_securityhub.literals import WorkflowStatusType

def get_value() -> WorkflowStatusType:
    return "NEW"
```

```python
# WorkflowStatusType definition
WorkflowStatusType = Literal[
    "NEW",
    "NOTIFIED",
    "RESOLVED",
    "SUPPRESSED",
]
```
## SecurityHubServiceName

```python
# SecurityHubServiceName usage example
from types_aiobotocore_securityhub.literals import SecurityHubServiceName

def get_value() -> SecurityHubServiceName:
    return "securityhub"
```

```python
# SecurityHubServiceName definition
SecurityHubServiceName = Literal[
    "securityhub",
]
```
## ServiceName

```python
# ServiceName usage example
from types_aiobotocore_securityhub.literals import ServiceName

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
    "backupsearch",
    "batch",
    "bcm-data-exports",
    "bcm-pricing-calculator",
    "bedrock",
    "bedrock-agent",
    "bedrock-agent-runtime",
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
    "networkflowmonitor",
    "networkmanager",
    "networkmonitor",
    "notifications",
    "notificationscontacts",
    "oam",
    "observabilityadmin",
    "omics",
    "opensearch",
    "opensearchserverless",
    "opsworks",
    "opsworkscm",
    "organizations",
    "osis",
    "outposts",
    "panorama",
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
    "s3tables",
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
from types_aiobotocore_securityhub.literals import ResourceServiceName

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
from types_aiobotocore_securityhub.literals import PaginatorName

def get_value() -> PaginatorName:
    return "describe_action_targets"
```

```python
# PaginatorName definition
PaginatorName = Literal[
    "describe_action_targets",
    "describe_products",
    "describe_standards",
    "describe_standards_controls",
    "get_enabled_standards",
    "get_finding_history",
    "get_findings",
    "get_insights",
    "list_configuration_policies",
    "list_configuration_policy_associations",
    "list_enabled_products_for_import",
    "list_finding_aggregators",
    "list_invitations",
    "list_members",
    "list_organization_admin_accounts",
    "list_security_control_definitions",
    "list_standards_control_associations",
]
```
## RegionName

```python
# RegionName usage example
from types_aiobotocore_securityhub.literals import RegionName

def get_value() -> RegionName:
    return "af-south-1"
```

```python
# RegionName definition
RegionName = Literal[
    "af-south-1",
    "ap-east-1",
    "ap-northeast-1",
    "ap-northeast-2",
    "ap-northeast-3",
    "ap-south-1",
    "ap-south-2",
    "ap-southeast-1",
    "ap-southeast-2",
    "ap-southeast-3",
    "ap-southeast-4",
    "ap-southeast-5",
    "ap-southeast-7",
    "ca-central-1",
    "ca-west-1",
    "eu-central-1",
    "eu-central-2",
    "eu-north-1",
    "eu-south-1",
    "eu-south-2",
    "eu-west-1",
    "eu-west-2",
    "eu-west-3",
    "il-central-1",
    "me-central-1",
    "me-south-1",
    "mx-central-1",
    "sa-east-1",
    "us-east-1",
    "us-east-2",
    "us-west-1",
    "us-west-2",
]
```

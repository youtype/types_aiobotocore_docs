# Type definitions

> [Index](../README.md) > [ConfigService](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ConfigService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#configservice)
    type annotations stubs module [types-aiobotocore-config](https://pypi.org/project/types-aiobotocore-config/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_config.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## AccountAggregationSourceUnionTypeDef

```python
# AccountAggregationSourceUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import AccountAggregationSourceUnionTypeDef


def get_value() -> AccountAggregationSourceUnionTypeDef:
    return ...


# AccountAggregationSourceUnionTypeDef definition

AccountAggregationSourceUnionTypeDef = Union[
    AccountAggregationSourceTypeDef,  # (1)
    AccountAggregationSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AccountAggregationSourceTypeDef](./type_defs.md#accountaggregationsourcetypedef) 
2. See [:material-code-braces: AccountAggregationSourceOutputTypeDef](./type_defs.md#accountaggregationsourceoutputtypedef) 

## OrganizationAggregationSourceUnionTypeDef

```python
# OrganizationAggregationSourceUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import OrganizationAggregationSourceUnionTypeDef


def get_value() -> OrganizationAggregationSourceUnionTypeDef:
    return ...


# OrganizationAggregationSourceUnionTypeDef definition

OrganizationAggregationSourceUnionTypeDef = Union[
    OrganizationAggregationSourceTypeDef,  # (1)
    OrganizationAggregationSourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OrganizationAggregationSourceTypeDef](./type_defs.md#organizationaggregationsourcetypedef) 
2. See [:material-code-braces: OrganizationAggregationSourceOutputTypeDef](./type_defs.md#organizationaggregationsourceoutputtypedef) 

## OrganizationCustomRuleMetadataUnionTypeDef

```python
# OrganizationCustomRuleMetadataUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import OrganizationCustomRuleMetadataUnionTypeDef


def get_value() -> OrganizationCustomRuleMetadataUnionTypeDef:
    return ...


# OrganizationCustomRuleMetadataUnionTypeDef definition

OrganizationCustomRuleMetadataUnionTypeDef = Union[
    OrganizationCustomRuleMetadataTypeDef,  # (1)
    OrganizationCustomRuleMetadataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OrganizationCustomRuleMetadataTypeDef](./type_defs.md#organizationcustomrulemetadatatypedef) 
2. See [:material-code-braces: OrganizationCustomRuleMetadataOutputTypeDef](./type_defs.md#organizationcustomrulemetadataoutputtypedef) 

## OrganizationManagedRuleMetadataUnionTypeDef

```python
# OrganizationManagedRuleMetadataUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import OrganizationManagedRuleMetadataUnionTypeDef


def get_value() -> OrganizationManagedRuleMetadataUnionTypeDef:
    return ...


# OrganizationManagedRuleMetadataUnionTypeDef definition

OrganizationManagedRuleMetadataUnionTypeDef = Union[
    OrganizationManagedRuleMetadataTypeDef,  # (1)
    OrganizationManagedRuleMetadataOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OrganizationManagedRuleMetadataTypeDef](./type_defs.md#organizationmanagedrulemetadatatypedef) 
2. See [:material-code-braces: OrganizationManagedRuleMetadataOutputTypeDef](./type_defs.md#organizationmanagedrulemetadataoutputtypedef) 

## StaticValueUnionTypeDef

```python
# StaticValueUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import StaticValueUnionTypeDef


def get_value() -> StaticValueUnionTypeDef:
    return ...


# StaticValueUnionTypeDef definition

StaticValueUnionTypeDef = Union[
    StaticValueTypeDef,  # (1)
    StaticValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: StaticValueTypeDef](./type_defs.md#staticvaluetypedef) 
2. See [:material-code-braces: StaticValueOutputTypeDef](./type_defs.md#staticvalueoutputtypedef) 

## AggregatorFiltersUnionTypeDef

```python
# AggregatorFiltersUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import AggregatorFiltersUnionTypeDef


def get_value() -> AggregatorFiltersUnionTypeDef:
    return ...


# AggregatorFiltersUnionTypeDef definition

AggregatorFiltersUnionTypeDef = Union[
    AggregatorFiltersTypeDef,  # (1)
    AggregatorFiltersOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AggregatorFiltersTypeDef](./type_defs.md#aggregatorfilterstypedef) 
2. See [:material-code-braces: AggregatorFiltersOutputTypeDef](./type_defs.md#aggregatorfiltersoutputtypedef) 

## EvaluationUnionTypeDef

```python
# EvaluationUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import EvaluationUnionTypeDef


def get_value() -> EvaluationUnionTypeDef:
    return ...


# EvaluationUnionTypeDef definition

EvaluationUnionTypeDef = Union[
    EvaluationTypeDef,  # (1)
    EvaluationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EvaluationTypeDef](./type_defs.md#evaluationtypedef) 
2. See [:material-code-braces: EvaluationOutputTypeDef](./type_defs.md#evaluationoutputtypedef) 

## ConfigurationRecorderUnionTypeDef

```python
# ConfigurationRecorderUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import ConfigurationRecorderUnionTypeDef


def get_value() -> ConfigurationRecorderUnionTypeDef:
    return ...


# ConfigurationRecorderUnionTypeDef definition

ConfigurationRecorderUnionTypeDef = Union[
    ConfigurationRecorderTypeDef,  # (1)
    ConfigurationRecorderOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfigurationRecorderTypeDef](./type_defs.md#configurationrecordertypedef) 
2. See [:material-code-braces: ConfigurationRecorderOutputTypeDef](./type_defs.md#configurationrecorderoutputtypedef) 

## ConfigRuleUnionTypeDef

```python
# ConfigRuleUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import ConfigRuleUnionTypeDef


def get_value() -> ConfigRuleUnionTypeDef:
    return ...


# ConfigRuleUnionTypeDef definition

ConfigRuleUnionTypeDef = Union[
    ConfigRuleTypeDef,  # (1)
    ConfigRuleOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ConfigRuleTypeDef](./type_defs.md#configruletypedef) 
2. See [:material-code-braces: ConfigRuleOutputTypeDef](./type_defs.md#configruleoutputtypedef) 

## RemediationParameterValueUnionTypeDef

```python
# RemediationParameterValueUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import RemediationParameterValueUnionTypeDef


def get_value() -> RemediationParameterValueUnionTypeDef:
    return ...


# RemediationParameterValueUnionTypeDef definition

RemediationParameterValueUnionTypeDef = Union[
    RemediationParameterValueTypeDef,  # (1)
    RemediationParameterValueOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RemediationParameterValueTypeDef](./type_defs.md#remediationparametervaluetypedef) 
2. See [:material-code-braces: RemediationParameterValueOutputTypeDef](./type_defs.md#remediationparametervalueoutputtypedef) 

## RemediationConfigurationUnionTypeDef

```python
# RemediationConfigurationUnionTypeDef Union usage example

from types_aiobotocore_config.type_defs import RemediationConfigurationUnionTypeDef


def get_value() -> RemediationConfigurationUnionTypeDef:
    return ...


# RemediationConfigurationUnionTypeDef definition

RemediationConfigurationUnionTypeDef = Union[
    RemediationConfigurationTypeDef,  # (1)
    RemediationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RemediationConfigurationTypeDef](./type_defs.md#remediationconfigurationtypedef) 
2. See [:material-code-braces: RemediationConfigurationOutputTypeDef](./type_defs.md#remediationconfigurationoutputtypedef) 



## AccountAggregationSourceOutputTypeDef

```python
# AccountAggregationSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AccountAggregationSourceOutputTypeDef


def get_value() -> AccountAggregationSourceOutputTypeDef:
    return {
        "AccountIds": ...,
    }


# AccountAggregationSourceOutputTypeDef definition

class AccountAggregationSourceOutputTypeDef(TypedDict):
    AccountIds: List[str],
    AllAwsRegions: NotRequired[bool],
    AwsRegions: NotRequired[List[str]],
```

## AccountAggregationSourceTypeDef

```python
# AccountAggregationSourceTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AccountAggregationSourceTypeDef


def get_value() -> AccountAggregationSourceTypeDef:
    return {
        "AccountIds": ...,
    }


# AccountAggregationSourceTypeDef definition

class AccountAggregationSourceTypeDef(TypedDict):
    AccountIds: Sequence[str],
    AllAwsRegions: NotRequired[bool],
    AwsRegions: NotRequired[Sequence[str]],
```

## AggregateConformancePackComplianceTypeDef

```python
# AggregateConformancePackComplianceTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateConformancePackComplianceTypeDef


def get_value() -> AggregateConformancePackComplianceTypeDef:
    return {
        "ComplianceType": ...,
    }


# AggregateConformancePackComplianceTypeDef definition

class AggregateConformancePackComplianceTypeDef(TypedDict):
    ComplianceType: NotRequired[ConformancePackComplianceTypeType],  # (1)
    CompliantRuleCount: NotRequired[int],
    NonCompliantRuleCount: NotRequired[int],
    TotalRuleCount: NotRequired[int],
```

1. See [:material-code-brackets: ConformancePackComplianceTypeType](./literals.md#conformancepackcompliancetypetype) 
## AggregateConformancePackComplianceCountTypeDef

```python
# AggregateConformancePackComplianceCountTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateConformancePackComplianceCountTypeDef


def get_value() -> AggregateConformancePackComplianceCountTypeDef:
    return {
        "CompliantConformancePackCount": ...,
    }


# AggregateConformancePackComplianceCountTypeDef definition

class AggregateConformancePackComplianceCountTypeDef(TypedDict):
    CompliantConformancePackCount: NotRequired[int],
    NonCompliantConformancePackCount: NotRequired[int],
```

## AggregateConformancePackComplianceFiltersTypeDef

```python
# AggregateConformancePackComplianceFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateConformancePackComplianceFiltersTypeDef


def get_value() -> AggregateConformancePackComplianceFiltersTypeDef:
    return {
        "ConformancePackName": ...,
    }


# AggregateConformancePackComplianceFiltersTypeDef definition

class AggregateConformancePackComplianceFiltersTypeDef(TypedDict):
    ConformancePackName: NotRequired[str],
    ComplianceType: NotRequired[ConformancePackComplianceTypeType],  # (1)
    AccountId: NotRequired[str],
    AwsRegion: NotRequired[str],
```

1. See [:material-code-brackets: ConformancePackComplianceTypeType](./literals.md#conformancepackcompliancetypetype) 
## AggregateConformancePackComplianceSummaryFiltersTypeDef

```python
# AggregateConformancePackComplianceSummaryFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateConformancePackComplianceSummaryFiltersTypeDef


def get_value() -> AggregateConformancePackComplianceSummaryFiltersTypeDef:
    return {
        "AccountId": ...,
    }


# AggregateConformancePackComplianceSummaryFiltersTypeDef definition

class AggregateConformancePackComplianceSummaryFiltersTypeDef(TypedDict):
    AccountId: NotRequired[str],
    AwsRegion: NotRequired[str],
```

## AggregateResourceIdentifierTypeDef

```python
# AggregateResourceIdentifierTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateResourceIdentifierTypeDef


def get_value() -> AggregateResourceIdentifierTypeDef:
    return {
        "SourceAccountId": ...,
    }


# AggregateResourceIdentifierTypeDef definition

class AggregateResourceIdentifierTypeDef(TypedDict):
    SourceAccountId: str,
    SourceRegion: str,
    ResourceId: str,
    ResourceType: ResourceTypeType,  # (1)
    ResourceName: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## AggregatedSourceStatusTypeDef

```python
# AggregatedSourceStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregatedSourceStatusTypeDef


def get_value() -> AggregatedSourceStatusTypeDef:
    return {
        "SourceId": ...,
    }


# AggregatedSourceStatusTypeDef definition

class AggregatedSourceStatusTypeDef(TypedDict):
    SourceId: NotRequired[str],
    SourceType: NotRequired[AggregatedSourceTypeType],  # (1)
    AwsRegion: NotRequired[str],
    LastUpdateStatus: NotRequired[AggregatedSourceStatusTypeType],  # (2)
    LastUpdateTime: NotRequired[datetime],
    LastErrorCode: NotRequired[str],
    LastErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: AggregatedSourceTypeType](./literals.md#aggregatedsourcetypetype) 
2. See [:material-code-brackets: AggregatedSourceStatusTypeType](./literals.md#aggregatedsourcestatustypetype) 
## AggregationAuthorizationTypeDef

```python
# AggregationAuthorizationTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregationAuthorizationTypeDef


def get_value() -> AggregationAuthorizationTypeDef:
    return {
        "AggregationAuthorizationArn": ...,
    }


# AggregationAuthorizationTypeDef definition

class AggregationAuthorizationTypeDef(TypedDict):
    AggregationAuthorizationArn: NotRequired[str],
    AuthorizedAccountId: NotRequired[str],
    AuthorizedAwsRegion: NotRequired[str],
    CreationTime: NotRequired[datetime],
```

## AggregatorFilterResourceTypeOutputTypeDef

```python
# AggregatorFilterResourceTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregatorFilterResourceTypeOutputTypeDef


def get_value() -> AggregatorFilterResourceTypeOutputTypeDef:
    return {
        "Type": ...,
    }


# AggregatorFilterResourceTypeOutputTypeDef definition

class AggregatorFilterResourceTypeOutputTypeDef(TypedDict):
    Type: NotRequired[AggregatorFilterTypeType],  # (1)
    Value: NotRequired[List[str]],
```

1. See [:material-code-brackets: AggregatorFilterTypeType](./literals.md#aggregatorfiltertypetype) 
## AggregatorFilterResourceTypeTypeDef

```python
# AggregatorFilterResourceTypeTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregatorFilterResourceTypeTypeDef


def get_value() -> AggregatorFilterResourceTypeTypeDef:
    return {
        "Type": ...,
    }


# AggregatorFilterResourceTypeTypeDef definition

class AggregatorFilterResourceTypeTypeDef(TypedDict):
    Type: NotRequired[AggregatorFilterTypeType],  # (1)
    Value: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AggregatorFilterTypeType](./literals.md#aggregatorfiltertypetype) 
## AggregatorFilterServicePrincipalOutputTypeDef

```python
# AggregatorFilterServicePrincipalOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregatorFilterServicePrincipalOutputTypeDef


def get_value() -> AggregatorFilterServicePrincipalOutputTypeDef:
    return {
        "Type": ...,
    }


# AggregatorFilterServicePrincipalOutputTypeDef definition

class AggregatorFilterServicePrincipalOutputTypeDef(TypedDict):
    Type: NotRequired[AggregatorFilterTypeType],  # (1)
    Value: NotRequired[List[str]],
```

1. See [:material-code-brackets: AggregatorFilterTypeType](./literals.md#aggregatorfiltertypetype) 
## AggregatorFilterServicePrincipalTypeDef

```python
# AggregatorFilterServicePrincipalTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregatorFilterServicePrincipalTypeDef


def get_value() -> AggregatorFilterServicePrincipalTypeDef:
    return {
        "Type": ...,
    }


# AggregatorFilterServicePrincipalTypeDef definition

class AggregatorFilterServicePrincipalTypeDef(TypedDict):
    Type: NotRequired[AggregatorFilterTypeType],  # (1)
    Value: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: AggregatorFilterTypeType](./literals.md#aggregatorfiltertypetype) 
## AssociateResourceTypesRequestTypeDef

```python
# AssociateResourceTypesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AssociateResourceTypesRequestTypeDef


def get_value() -> AssociateResourceTypesRequestTypeDef:
    return {
        "ConfigurationRecorderArn": ...,
    }


# AssociateResourceTypesRequestTypeDef definition

class AssociateResourceTypesRequestTypeDef(TypedDict):
    ConfigurationRecorderArn: str,
    ResourceTypes: Sequence[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResponseMetadataTypeDef


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

## BaseConfigurationItemTypeDef

```python
# BaseConfigurationItemTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import BaseConfigurationItemTypeDef


def get_value() -> BaseConfigurationItemTypeDef:
    return {
        "version": ...,
    }


# BaseConfigurationItemTypeDef definition

class BaseConfigurationItemTypeDef(TypedDict):
    version: NotRequired[str],
    accountId: NotRequired[str],
    configurationItemCaptureTime: NotRequired[datetime],
    configurationItemStatus: NotRequired[ConfigurationItemStatusType],  # (1)
    configurationStateId: NotRequired[str],
    arn: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (2)
    resourceId: NotRequired[str],
    resourceName: NotRequired[str],
    awsRegion: NotRequired[str],
    availabilityZone: NotRequired[str],
    resourceCreationTime: NotRequired[datetime],
    configuration: NotRequired[str],
    supplementaryConfiguration: NotRequired[Dict[str, str]],
    recordingFrequency: NotRequired[RecordingFrequencyType],  # (3)
    configurationItemDeliveryTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ConfigurationItemStatusType](./literals.md#configurationitemstatustype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-brackets: RecordingFrequencyType](./literals.md#recordingfrequencytype) 
## ResourceKeyTypeDef

```python
# ResourceKeyTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceKeyTypeDef


def get_value() -> ResourceKeyTypeDef:
    return {
        "resourceType": ...,
    }


# ResourceKeyTypeDef definition

class ResourceKeyTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    resourceId: str,
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ComplianceContributorCountTypeDef

```python
# ComplianceContributorCountTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ComplianceContributorCountTypeDef


def get_value() -> ComplianceContributorCountTypeDef:
    return {
        "CappedCount": ...,
    }


# ComplianceContributorCountTypeDef definition

class ComplianceContributorCountTypeDef(TypedDict):
    CappedCount: NotRequired[int],
    CapExceeded: NotRequired[bool],
```

## ConfigExportDeliveryInfoTypeDef

```python
# ConfigExportDeliveryInfoTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigExportDeliveryInfoTypeDef


def get_value() -> ConfigExportDeliveryInfoTypeDef:
    return {
        "lastStatus": ...,
    }


# ConfigExportDeliveryInfoTypeDef definition

class ConfigExportDeliveryInfoTypeDef(TypedDict):
    lastStatus: NotRequired[DeliveryStatusType],  # (1)
    lastErrorCode: NotRequired[str],
    lastErrorMessage: NotRequired[str],
    lastAttemptTime: NotRequired[datetime],
    lastSuccessfulTime: NotRequired[datetime],
    nextDeliveryTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DeliveryStatusType](./literals.md#deliverystatustype) 
## ConfigRuleComplianceFiltersTypeDef

```python
# ConfigRuleComplianceFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigRuleComplianceFiltersTypeDef


def get_value() -> ConfigRuleComplianceFiltersTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# ConfigRuleComplianceFiltersTypeDef definition

class ConfigRuleComplianceFiltersTypeDef(TypedDict):
    ConfigRuleName: NotRequired[str],
    ComplianceType: NotRequired[ComplianceTypeType],  # (1)
    AccountId: NotRequired[str],
    AwsRegion: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## ConfigRuleComplianceSummaryFiltersTypeDef

```python
# ConfigRuleComplianceSummaryFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigRuleComplianceSummaryFiltersTypeDef


def get_value() -> ConfigRuleComplianceSummaryFiltersTypeDef:
    return {
        "AccountId": ...,
    }


# ConfigRuleComplianceSummaryFiltersTypeDef definition

class ConfigRuleComplianceSummaryFiltersTypeDef(TypedDict):
    AccountId: NotRequired[str],
    AwsRegion: NotRequired[str],
```

## ConfigRuleEvaluationStatusTypeDef

```python
# ConfigRuleEvaluationStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigRuleEvaluationStatusTypeDef


def get_value() -> ConfigRuleEvaluationStatusTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# ConfigRuleEvaluationStatusTypeDef definition

class ConfigRuleEvaluationStatusTypeDef(TypedDict):
    ConfigRuleName: NotRequired[str],
    ConfigRuleArn: NotRequired[str],
    ConfigRuleId: NotRequired[str],
    LastSuccessfulInvocationTime: NotRequired[datetime],
    LastFailedInvocationTime: NotRequired[datetime],
    LastSuccessfulEvaluationTime: NotRequired[datetime],
    LastFailedEvaluationTime: NotRequired[datetime],
    FirstActivatedTime: NotRequired[datetime],
    LastDeactivatedTime: NotRequired[datetime],
    LastErrorCode: NotRequired[str],
    LastErrorMessage: NotRequired[str],
    FirstEvaluationStarted: NotRequired[bool],
    LastDebugLogDeliveryStatus: NotRequired[str],
    LastDebugLogDeliveryStatusReason: NotRequired[str],
    LastDebugLogDeliveryTime: NotRequired[datetime],
```

## EvaluationModeConfigurationTypeDef

```python
# EvaluationModeConfigurationTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EvaluationModeConfigurationTypeDef


def get_value() -> EvaluationModeConfigurationTypeDef:
    return {
        "Mode": ...,
    }


# EvaluationModeConfigurationTypeDef definition

class EvaluationModeConfigurationTypeDef(TypedDict):
    Mode: NotRequired[EvaluationModeType],  # (1)
```

1. See [:material-code-brackets: EvaluationModeType](./literals.md#evaluationmodetype) 
## ScopeOutputTypeDef

```python
# ScopeOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ScopeOutputTypeDef


def get_value() -> ScopeOutputTypeDef:
    return {
        "ComplianceResourceTypes": ...,
    }


# ScopeOutputTypeDef definition

class ScopeOutputTypeDef(TypedDict):
    ComplianceResourceTypes: NotRequired[List[str]],
    TagKey: NotRequired[str],
    TagValue: NotRequired[str],
    ComplianceResourceId: NotRequired[str],
```

## ScopeTypeDef

```python
# ScopeTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ScopeTypeDef


def get_value() -> ScopeTypeDef:
    return {
        "ComplianceResourceTypes": ...,
    }


# ScopeTypeDef definition

class ScopeTypeDef(TypedDict):
    ComplianceResourceTypes: NotRequired[Sequence[str]],
    TagKey: NotRequired[str],
    TagValue: NotRequired[str],
    ComplianceResourceId: NotRequired[str],
```

## ConfigSnapshotDeliveryPropertiesTypeDef

```python
# ConfigSnapshotDeliveryPropertiesTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigSnapshotDeliveryPropertiesTypeDef


def get_value() -> ConfigSnapshotDeliveryPropertiesTypeDef:
    return {
        "deliveryFrequency": ...,
    }


# ConfigSnapshotDeliveryPropertiesTypeDef definition

class ConfigSnapshotDeliveryPropertiesTypeDef(TypedDict):
    deliveryFrequency: NotRequired[MaximumExecutionFrequencyType],  # (1)
```

1. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
## ConfigStreamDeliveryInfoTypeDef

```python
# ConfigStreamDeliveryInfoTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigStreamDeliveryInfoTypeDef


def get_value() -> ConfigStreamDeliveryInfoTypeDef:
    return {
        "lastStatus": ...,
    }


# ConfigStreamDeliveryInfoTypeDef definition

class ConfigStreamDeliveryInfoTypeDef(TypedDict):
    lastStatus: NotRequired[DeliveryStatusType],  # (1)
    lastErrorCode: NotRequired[str],
    lastErrorMessage: NotRequired[str],
    lastStatusChangeTime: NotRequired[datetime],
```

1. See [:material-code-brackets: DeliveryStatusType](./literals.md#deliverystatustype) 
## OrganizationAggregationSourceOutputTypeDef

```python
# OrganizationAggregationSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationAggregationSourceOutputTypeDef


def get_value() -> OrganizationAggregationSourceOutputTypeDef:
    return {
        "RoleArn": ...,
    }


# OrganizationAggregationSourceOutputTypeDef definition

class OrganizationAggregationSourceOutputTypeDef(TypedDict):
    RoleArn: str,
    AwsRegions: NotRequired[List[str]],
    AllAwsRegions: NotRequired[bool],
```

## RelationshipTypeDef

```python
# RelationshipTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RelationshipTypeDef


def get_value() -> RelationshipTypeDef:
    return {
        "resourceType": ...,
    }


# RelationshipTypeDef definition

class RelationshipTypeDef(TypedDict):
    resourceType: NotRequired[ResourceTypeType],  # (1)
    resourceId: NotRequired[str],
    resourceName: NotRequired[str],
    relationshipName: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ConfigurationRecorderFilterTypeDef

```python
# ConfigurationRecorderFilterTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigurationRecorderFilterTypeDef


def get_value() -> ConfigurationRecorderFilterTypeDef:
    return {
        "filterName": ...,
    }


# ConfigurationRecorderFilterTypeDef definition

class ConfigurationRecorderFilterTypeDef(TypedDict):
    filterName: NotRequired[ConfigurationRecorderFilterNameType],  # (1)
    filterValue: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ConfigurationRecorderFilterNameType](./literals.md#configurationrecorderfilternametype) 
## ConfigurationRecorderStatusTypeDef

```python
# ConfigurationRecorderStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigurationRecorderStatusTypeDef


def get_value() -> ConfigurationRecorderStatusTypeDef:
    return {
        "arn": ...,
    }


# ConfigurationRecorderStatusTypeDef definition

class ConfigurationRecorderStatusTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    lastStartTime: NotRequired[datetime],
    lastStopTime: NotRequired[datetime],
    recording: NotRequired[bool],
    lastStatus: NotRequired[RecorderStatusType],  # (1)
    lastErrorCode: NotRequired[str],
    lastErrorMessage: NotRequired[str],
    lastStatusChangeTime: NotRequired[datetime],
    servicePrincipal: NotRequired[str],
```

1. See [:material-code-brackets: RecorderStatusType](./literals.md#recorderstatustype) 
## ConfigurationRecorderSummaryTypeDef

```python
# ConfigurationRecorderSummaryTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigurationRecorderSummaryTypeDef


def get_value() -> ConfigurationRecorderSummaryTypeDef:
    return {
        "arn": ...,
    }


# ConfigurationRecorderSummaryTypeDef definition

class ConfigurationRecorderSummaryTypeDef(TypedDict):
    arn: str,
    name: str,
    recordingScope: RecordingScopeType,  # (1)
    servicePrincipal: NotRequired[str],
```

1. See [:material-code-brackets: RecordingScopeType](./literals.md#recordingscopetype) 
## ConformancePackComplianceFiltersTypeDef

```python
# ConformancePackComplianceFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackComplianceFiltersTypeDef


def get_value() -> ConformancePackComplianceFiltersTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# ConformancePackComplianceFiltersTypeDef definition

class ConformancePackComplianceFiltersTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
    ComplianceType: NotRequired[ConformancePackComplianceTypeType],  # (1)
```

1. See [:material-code-brackets: ConformancePackComplianceTypeType](./literals.md#conformancepackcompliancetypetype) 
## ConformancePackComplianceScoreTypeDef

```python
# ConformancePackComplianceScoreTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackComplianceScoreTypeDef


def get_value() -> ConformancePackComplianceScoreTypeDef:
    return {
        "Score": ...,
    }


# ConformancePackComplianceScoreTypeDef definition

class ConformancePackComplianceScoreTypeDef(TypedDict):
    Score: NotRequired[str],
    ConformancePackName: NotRequired[str],
    LastUpdatedTime: NotRequired[datetime],
```

## ConformancePackComplianceScoresFiltersTypeDef

```python
# ConformancePackComplianceScoresFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackComplianceScoresFiltersTypeDef


def get_value() -> ConformancePackComplianceScoresFiltersTypeDef:
    return {
        "ConformancePackNames": ...,
    }


# ConformancePackComplianceScoresFiltersTypeDef definition

class ConformancePackComplianceScoresFiltersTypeDef(TypedDict):
    ConformancePackNames: Sequence[str],
```

## ConformancePackComplianceSummaryTypeDef

```python
# ConformancePackComplianceSummaryTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackComplianceSummaryTypeDef


def get_value() -> ConformancePackComplianceSummaryTypeDef:
    return {
        "ConformancePackName": ...,
    }


# ConformancePackComplianceSummaryTypeDef definition

class ConformancePackComplianceSummaryTypeDef(TypedDict):
    ConformancePackName: str,
    ConformancePackComplianceStatus: ConformancePackComplianceTypeType,  # (1)
```

1. See [:material-code-brackets: ConformancePackComplianceTypeType](./literals.md#conformancepackcompliancetypetype) 
## ConformancePackInputParameterTypeDef

```python
# ConformancePackInputParameterTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackInputParameterTypeDef


def get_value() -> ConformancePackInputParameterTypeDef:
    return {
        "ParameterName": ...,
    }


# ConformancePackInputParameterTypeDef definition

class ConformancePackInputParameterTypeDef(TypedDict):
    ParameterName: str,
    ParameterValue: str,
```

## TemplateSSMDocumentDetailsTypeDef

```python
# TemplateSSMDocumentDetailsTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import TemplateSSMDocumentDetailsTypeDef


def get_value() -> TemplateSSMDocumentDetailsTypeDef:
    return {
        "DocumentName": ...,
    }


# TemplateSSMDocumentDetailsTypeDef definition

class TemplateSSMDocumentDetailsTypeDef(TypedDict):
    DocumentName: str,
    DocumentVersion: NotRequired[str],
```

## ConformancePackEvaluationFiltersTypeDef

```python
# ConformancePackEvaluationFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackEvaluationFiltersTypeDef


def get_value() -> ConformancePackEvaluationFiltersTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# ConformancePackEvaluationFiltersTypeDef definition

class ConformancePackEvaluationFiltersTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
    ComplianceType: NotRequired[ConformancePackComplianceTypeType],  # (1)
    ResourceType: NotRequired[str],
    ResourceIds: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ConformancePackComplianceTypeType](./literals.md#conformancepackcompliancetypetype) 
## ConformancePackRuleComplianceTypeDef

```python
# ConformancePackRuleComplianceTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackRuleComplianceTypeDef


def get_value() -> ConformancePackRuleComplianceTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# ConformancePackRuleComplianceTypeDef definition

class ConformancePackRuleComplianceTypeDef(TypedDict):
    ConfigRuleName: NotRequired[str],
    ComplianceType: NotRequired[ConformancePackComplianceTypeType],  # (1)
    Controls: NotRequired[List[str]],
```

1. See [:material-code-brackets: ConformancePackComplianceTypeType](./literals.md#conformancepackcompliancetypetype) 
## ConformancePackStatusDetailTypeDef

```python
# ConformancePackStatusDetailTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackStatusDetailTypeDef


def get_value() -> ConformancePackStatusDetailTypeDef:
    return {
        "ConformancePackName": ...,
    }


# ConformancePackStatusDetailTypeDef definition

class ConformancePackStatusDetailTypeDef(TypedDict):
    ConformancePackName: str,
    ConformancePackId: str,
    ConformancePackArn: str,
    ConformancePackState: ConformancePackStateType,  # (1)
    StackArn: str,
    LastUpdateRequestedTime: datetime,
    ConformancePackStatusReason: NotRequired[str],
    LastUpdateCompletedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ConformancePackStateType](./literals.md#conformancepackstatetype) 
## CustomPolicyDetailsTypeDef

```python
# CustomPolicyDetailsTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import CustomPolicyDetailsTypeDef


def get_value() -> CustomPolicyDetailsTypeDef:
    return {
        "PolicyRuntime": ...,
    }


# CustomPolicyDetailsTypeDef definition

class CustomPolicyDetailsTypeDef(TypedDict):
    PolicyRuntime: str,
    PolicyText: str,
    EnableDebugLogDelivery: NotRequired[bool],
```

## DeleteAggregationAuthorizationRequestTypeDef

```python
# DeleteAggregationAuthorizationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteAggregationAuthorizationRequestTypeDef


def get_value() -> DeleteAggregationAuthorizationRequestTypeDef:
    return {
        "AuthorizedAccountId": ...,
    }


# DeleteAggregationAuthorizationRequestTypeDef definition

class DeleteAggregationAuthorizationRequestTypeDef(TypedDict):
    AuthorizedAccountId: str,
    AuthorizedAwsRegion: str,
```

## DeleteConfigRuleRequestTypeDef

```python
# DeleteConfigRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteConfigRuleRequestTypeDef


def get_value() -> DeleteConfigRuleRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# DeleteConfigRuleRequestTypeDef definition

class DeleteConfigRuleRequestTypeDef(TypedDict):
    ConfigRuleName: str,
```

## DeleteConfigurationAggregatorRequestTypeDef

```python
# DeleteConfigurationAggregatorRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteConfigurationAggregatorRequestTypeDef


def get_value() -> DeleteConfigurationAggregatorRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# DeleteConfigurationAggregatorRequestTypeDef definition

class DeleteConfigurationAggregatorRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
```

## DeleteConfigurationRecorderRequestTypeDef

```python
# DeleteConfigurationRecorderRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteConfigurationRecorderRequestTypeDef


def get_value() -> DeleteConfigurationRecorderRequestTypeDef:
    return {
        "ConfigurationRecorderName": ...,
    }


# DeleteConfigurationRecorderRequestTypeDef definition

class DeleteConfigurationRecorderRequestTypeDef(TypedDict):
    ConfigurationRecorderName: str,
```

## DeleteConformancePackRequestTypeDef

```python
# DeleteConformancePackRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteConformancePackRequestTypeDef


def get_value() -> DeleteConformancePackRequestTypeDef:
    return {
        "ConformancePackName": ...,
    }


# DeleteConformancePackRequestTypeDef definition

class DeleteConformancePackRequestTypeDef(TypedDict):
    ConformancePackName: str,
```

## DeleteDeliveryChannelRequestTypeDef

```python
# DeleteDeliveryChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteDeliveryChannelRequestTypeDef


def get_value() -> DeleteDeliveryChannelRequestTypeDef:
    return {
        "DeliveryChannelName": ...,
    }


# DeleteDeliveryChannelRequestTypeDef definition

class DeleteDeliveryChannelRequestTypeDef(TypedDict):
    DeliveryChannelName: str,
```

## DeleteEvaluationResultsRequestTypeDef

```python
# DeleteEvaluationResultsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteEvaluationResultsRequestTypeDef


def get_value() -> DeleteEvaluationResultsRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# DeleteEvaluationResultsRequestTypeDef definition

class DeleteEvaluationResultsRequestTypeDef(TypedDict):
    ConfigRuleName: str,
```

## DeleteOrganizationConfigRuleRequestTypeDef

```python
# DeleteOrganizationConfigRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteOrganizationConfigRuleRequestTypeDef


def get_value() -> DeleteOrganizationConfigRuleRequestTypeDef:
    return {
        "OrganizationConfigRuleName": ...,
    }


# DeleteOrganizationConfigRuleRequestTypeDef definition

class DeleteOrganizationConfigRuleRequestTypeDef(TypedDict):
    OrganizationConfigRuleName: str,
```

## DeleteOrganizationConformancePackRequestTypeDef

```python
# DeleteOrganizationConformancePackRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteOrganizationConformancePackRequestTypeDef


def get_value() -> DeleteOrganizationConformancePackRequestTypeDef:
    return {
        "OrganizationConformancePackName": ...,
    }


# DeleteOrganizationConformancePackRequestTypeDef definition

class DeleteOrganizationConformancePackRequestTypeDef(TypedDict):
    OrganizationConformancePackName: str,
```

## DeletePendingAggregationRequestRequestTypeDef

```python
# DeletePendingAggregationRequestRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeletePendingAggregationRequestRequestTypeDef


def get_value() -> DeletePendingAggregationRequestRequestTypeDef:
    return {
        "RequesterAccountId": ...,
    }


# DeletePendingAggregationRequestRequestTypeDef definition

class DeletePendingAggregationRequestRequestTypeDef(TypedDict):
    RequesterAccountId: str,
    RequesterAwsRegion: str,
```

## DeleteRemediationConfigurationRequestTypeDef

```python
# DeleteRemediationConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteRemediationConfigurationRequestTypeDef


def get_value() -> DeleteRemediationConfigurationRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# DeleteRemediationConfigurationRequestTypeDef definition

class DeleteRemediationConfigurationRequestTypeDef(TypedDict):
    ConfigRuleName: str,
    ResourceType: NotRequired[str],
```

## RemediationExceptionResourceKeyTypeDef

```python
# RemediationExceptionResourceKeyTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RemediationExceptionResourceKeyTypeDef


def get_value() -> RemediationExceptionResourceKeyTypeDef:
    return {
        "ResourceType": ...,
    }


# RemediationExceptionResourceKeyTypeDef definition

class RemediationExceptionResourceKeyTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
```

## DeleteResourceConfigRequestTypeDef

```python
# DeleteResourceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteResourceConfigRequestTypeDef


def get_value() -> DeleteResourceConfigRequestTypeDef:
    return {
        "ResourceType": ...,
    }


# DeleteResourceConfigRequestTypeDef definition

class DeleteResourceConfigRequestTypeDef(TypedDict):
    ResourceType: str,
    ResourceId: str,
```

## DeleteRetentionConfigurationRequestTypeDef

```python
# DeleteRetentionConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteRetentionConfigurationRequestTypeDef


def get_value() -> DeleteRetentionConfigurationRequestTypeDef:
    return {
        "RetentionConfigurationName": ...,
    }


# DeleteRetentionConfigurationRequestTypeDef definition

class DeleteRetentionConfigurationRequestTypeDef(TypedDict):
    RetentionConfigurationName: str,
```

## DeleteServiceLinkedConfigurationRecorderRequestTypeDef

```python
# DeleteServiceLinkedConfigurationRecorderRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteServiceLinkedConfigurationRecorderRequestTypeDef


def get_value() -> DeleteServiceLinkedConfigurationRecorderRequestTypeDef:
    return {
        "ServicePrincipal": ...,
    }


# DeleteServiceLinkedConfigurationRecorderRequestTypeDef definition

class DeleteServiceLinkedConfigurationRecorderRequestTypeDef(TypedDict):
    ServicePrincipal: str,
```

## DeleteStoredQueryRequestTypeDef

```python
# DeleteStoredQueryRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteStoredQueryRequestTypeDef


def get_value() -> DeleteStoredQueryRequestTypeDef:
    return {
        "QueryName": ...,
    }


# DeleteStoredQueryRequestTypeDef definition

class DeleteStoredQueryRequestTypeDef(TypedDict):
    QueryName: str,
```

## DeliverConfigSnapshotRequestTypeDef

```python
# DeliverConfigSnapshotRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeliverConfigSnapshotRequestTypeDef


def get_value() -> DeliverConfigSnapshotRequestTypeDef:
    return {
        "deliveryChannelName": ...,
    }


# DeliverConfigSnapshotRequestTypeDef definition

class DeliverConfigSnapshotRequestTypeDef(TypedDict):
    deliveryChannelName: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PaginatorConfigTypeDef


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

## DescribeAggregationAuthorizationsRequestTypeDef

```python
# DescribeAggregationAuthorizationsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregationAuthorizationsRequestTypeDef


def get_value() -> DescribeAggregationAuthorizationsRequestTypeDef:
    return {
        "Limit": ...,
    }


# DescribeAggregationAuthorizationsRequestTypeDef definition

class DescribeAggregationAuthorizationsRequestTypeDef(TypedDict):
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeComplianceByConfigRuleRequestTypeDef

```python
# DescribeComplianceByConfigRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeComplianceByConfigRuleRequestTypeDef


def get_value() -> DescribeComplianceByConfigRuleRequestTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# DescribeComplianceByConfigRuleRequestTypeDef definition

class DescribeComplianceByConfigRuleRequestTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
    ComplianceTypes: NotRequired[Sequence[ComplianceTypeType]],  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## DescribeComplianceByResourceRequestTypeDef

```python
# DescribeComplianceByResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeComplianceByResourceRequestTypeDef


def get_value() -> DescribeComplianceByResourceRequestTypeDef:
    return {
        "ResourceType": ...,
    }


# DescribeComplianceByResourceRequestTypeDef definition

class DescribeComplianceByResourceRequestTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    ComplianceTypes: NotRequired[Sequence[ComplianceTypeType]],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## DescribeConfigRuleEvaluationStatusRequestTypeDef

```python
# DescribeConfigRuleEvaluationStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigRuleEvaluationStatusRequestTypeDef


def get_value() -> DescribeConfigRuleEvaluationStatusRequestTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# DescribeConfigRuleEvaluationStatusRequestTypeDef definition

class DescribeConfigRuleEvaluationStatusRequestTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## DescribeConfigRulesFiltersTypeDef

```python
# DescribeConfigRulesFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigRulesFiltersTypeDef


def get_value() -> DescribeConfigRulesFiltersTypeDef:
    return {
        "EvaluationMode": ...,
    }


# DescribeConfigRulesFiltersTypeDef definition

class DescribeConfigRulesFiltersTypeDef(TypedDict):
    EvaluationMode: NotRequired[EvaluationModeType],  # (1)
```

1. See [:material-code-brackets: EvaluationModeType](./literals.md#evaluationmodetype) 
## DescribeConfigurationAggregatorSourcesStatusRequestTypeDef

```python
# DescribeConfigurationAggregatorSourcesStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationAggregatorSourcesStatusRequestTypeDef


def get_value() -> DescribeConfigurationAggregatorSourcesStatusRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# DescribeConfigurationAggregatorSourcesStatusRequestTypeDef definition

class DescribeConfigurationAggregatorSourcesStatusRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    UpdateStatus: NotRequired[Sequence[AggregatedSourceStatusTypeType]],  # (1)
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: AggregatedSourceStatusTypeType](./literals.md#aggregatedsourcestatustypetype) 
## DescribeConfigurationAggregatorsRequestTypeDef

```python
# DescribeConfigurationAggregatorsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationAggregatorsRequestTypeDef


def get_value() -> DescribeConfigurationAggregatorsRequestTypeDef:
    return {
        "ConfigurationAggregatorNames": ...,
    }


# DescribeConfigurationAggregatorsRequestTypeDef definition

class DescribeConfigurationAggregatorsRequestTypeDef(TypedDict):
    ConfigurationAggregatorNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    Limit: NotRequired[int],
```

## DescribeConfigurationRecorderStatusRequestTypeDef

```python
# DescribeConfigurationRecorderStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationRecorderStatusRequestTypeDef


def get_value() -> DescribeConfigurationRecorderStatusRequestTypeDef:
    return {
        "ConfigurationRecorderNames": ...,
    }


# DescribeConfigurationRecorderStatusRequestTypeDef definition

class DescribeConfigurationRecorderStatusRequestTypeDef(TypedDict):
    ConfigurationRecorderNames: NotRequired[Sequence[str]],
    ServicePrincipal: NotRequired[str],
    Arn: NotRequired[str],
```

## DescribeConfigurationRecordersRequestTypeDef

```python
# DescribeConfigurationRecordersRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationRecordersRequestTypeDef


def get_value() -> DescribeConfigurationRecordersRequestTypeDef:
    return {
        "ConfigurationRecorderNames": ...,
    }


# DescribeConfigurationRecordersRequestTypeDef definition

class DescribeConfigurationRecordersRequestTypeDef(TypedDict):
    ConfigurationRecorderNames: NotRequired[Sequence[str]],
    ServicePrincipal: NotRequired[str],
    Arn: NotRequired[str],
```

## DescribeConformancePackStatusRequestTypeDef

```python
# DescribeConformancePackStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConformancePackStatusRequestTypeDef


def get_value() -> DescribeConformancePackStatusRequestTypeDef:
    return {
        "ConformancePackNames": ...,
    }


# DescribeConformancePackStatusRequestTypeDef definition

class DescribeConformancePackStatusRequestTypeDef(TypedDict):
    ConformancePackNames: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeConformancePacksRequestTypeDef

```python
# DescribeConformancePacksRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConformancePacksRequestTypeDef


def get_value() -> DescribeConformancePacksRequestTypeDef:
    return {
        "ConformancePackNames": ...,
    }


# DescribeConformancePacksRequestTypeDef definition

class DescribeConformancePacksRequestTypeDef(TypedDict):
    ConformancePackNames: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeDeliveryChannelStatusRequestTypeDef

```python
# DescribeDeliveryChannelStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeDeliveryChannelStatusRequestTypeDef


def get_value() -> DescribeDeliveryChannelStatusRequestTypeDef:
    return {
        "DeliveryChannelNames": ...,
    }


# DescribeDeliveryChannelStatusRequestTypeDef definition

class DescribeDeliveryChannelStatusRequestTypeDef(TypedDict):
    DeliveryChannelNames: NotRequired[Sequence[str]],
```

## DescribeDeliveryChannelsRequestTypeDef

```python
# DescribeDeliveryChannelsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeDeliveryChannelsRequestTypeDef


def get_value() -> DescribeDeliveryChannelsRequestTypeDef:
    return {
        "DeliveryChannelNames": ...,
    }


# DescribeDeliveryChannelsRequestTypeDef definition

class DescribeDeliveryChannelsRequestTypeDef(TypedDict):
    DeliveryChannelNames: NotRequired[Sequence[str]],
```

## DescribeOrganizationConfigRuleStatusesRequestTypeDef

```python
# DescribeOrganizationConfigRuleStatusesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConfigRuleStatusesRequestTypeDef


def get_value() -> DescribeOrganizationConfigRuleStatusesRequestTypeDef:
    return {
        "OrganizationConfigRuleNames": ...,
    }


# DescribeOrganizationConfigRuleStatusesRequestTypeDef definition

class DescribeOrganizationConfigRuleStatusesRequestTypeDef(TypedDict):
    OrganizationConfigRuleNames: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## OrganizationConfigRuleStatusTypeDef

```python
# OrganizationConfigRuleStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationConfigRuleStatusTypeDef


def get_value() -> OrganizationConfigRuleStatusTypeDef:
    return {
        "OrganizationConfigRuleName": ...,
    }


# OrganizationConfigRuleStatusTypeDef definition

class OrganizationConfigRuleStatusTypeDef(TypedDict):
    OrganizationConfigRuleName: str,
    OrganizationRuleStatus: OrganizationRuleStatusType,  # (1)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    LastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: OrganizationRuleStatusType](./literals.md#organizationrulestatustype) 
## DescribeOrganizationConfigRulesRequestTypeDef

```python
# DescribeOrganizationConfigRulesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConfigRulesRequestTypeDef


def get_value() -> DescribeOrganizationConfigRulesRequestTypeDef:
    return {
        "OrganizationConfigRuleNames": ...,
    }


# DescribeOrganizationConfigRulesRequestTypeDef definition

class DescribeOrganizationConfigRulesRequestTypeDef(TypedDict):
    OrganizationConfigRuleNames: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribeOrganizationConformancePackStatusesRequestTypeDef

```python
# DescribeOrganizationConformancePackStatusesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConformancePackStatusesRequestTypeDef


def get_value() -> DescribeOrganizationConformancePackStatusesRequestTypeDef:
    return {
        "OrganizationConformancePackNames": ...,
    }


# DescribeOrganizationConformancePackStatusesRequestTypeDef definition

class DescribeOrganizationConformancePackStatusesRequestTypeDef(TypedDict):
    OrganizationConformancePackNames: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## OrganizationConformancePackStatusTypeDef

```python
# OrganizationConformancePackStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationConformancePackStatusTypeDef


def get_value() -> OrganizationConformancePackStatusTypeDef:
    return {
        "OrganizationConformancePackName": ...,
    }


# OrganizationConformancePackStatusTypeDef definition

class OrganizationConformancePackStatusTypeDef(TypedDict):
    OrganizationConformancePackName: str,
    Status: OrganizationResourceStatusType,  # (1)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    LastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: OrganizationResourceStatusType](./literals.md#organizationresourcestatustype) 
## DescribeOrganizationConformancePacksRequestTypeDef

```python
# DescribeOrganizationConformancePacksRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConformancePacksRequestTypeDef


def get_value() -> DescribeOrganizationConformancePacksRequestTypeDef:
    return {
        "OrganizationConformancePackNames": ...,
    }


# DescribeOrganizationConformancePacksRequestTypeDef definition

class DescribeOrganizationConformancePacksRequestTypeDef(TypedDict):
    OrganizationConformancePackNames: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## DescribePendingAggregationRequestsRequestTypeDef

```python
# DescribePendingAggregationRequestsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribePendingAggregationRequestsRequestTypeDef


def get_value() -> DescribePendingAggregationRequestsRequestTypeDef:
    return {
        "Limit": ...,
    }


# DescribePendingAggregationRequestsRequestTypeDef definition

class DescribePendingAggregationRequestsRequestTypeDef(TypedDict):
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## PendingAggregationRequestTypeDef

```python
# PendingAggregationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PendingAggregationRequestTypeDef


def get_value() -> PendingAggregationRequestTypeDef:
    return {
        "RequesterAccountId": ...,
    }


# PendingAggregationRequestTypeDef definition

class PendingAggregationRequestTypeDef(TypedDict):
    RequesterAccountId: NotRequired[str],
    RequesterAwsRegion: NotRequired[str],
```

## DescribeRemediationConfigurationsRequestTypeDef

```python
# DescribeRemediationConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRemediationConfigurationsRequestTypeDef


def get_value() -> DescribeRemediationConfigurationsRequestTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# DescribeRemediationConfigurationsRequestTypeDef definition

class DescribeRemediationConfigurationsRequestTypeDef(TypedDict):
    ConfigRuleNames: Sequence[str],
```

## RemediationExceptionTypeDef

```python
# RemediationExceptionTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RemediationExceptionTypeDef


def get_value() -> RemediationExceptionTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# RemediationExceptionTypeDef definition

class RemediationExceptionTypeDef(TypedDict):
    ConfigRuleName: str,
    ResourceType: str,
    ResourceId: str,
    Message: NotRequired[str],
    ExpirationTime: NotRequired[datetime],
```

## DescribeRetentionConfigurationsRequestTypeDef

```python
# DescribeRetentionConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRetentionConfigurationsRequestTypeDef


def get_value() -> DescribeRetentionConfigurationsRequestTypeDef:
    return {
        "RetentionConfigurationNames": ...,
    }


# DescribeRetentionConfigurationsRequestTypeDef definition

class DescribeRetentionConfigurationsRequestTypeDef(TypedDict):
    RetentionConfigurationNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
```

## RetentionConfigurationTypeDef

```python
# RetentionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RetentionConfigurationTypeDef


def get_value() -> RetentionConfigurationTypeDef:
    return {
        "Name": ...,
    }


# RetentionConfigurationTypeDef definition

class RetentionConfigurationTypeDef(TypedDict):
    Name: str,
    RetentionPeriodInDays: int,
```

## DisassociateResourceTypesRequestTypeDef

```python
# DisassociateResourceTypesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DisassociateResourceTypesRequestTypeDef


def get_value() -> DisassociateResourceTypesRequestTypeDef:
    return {
        "ConfigurationRecorderArn": ...,
    }


# DisassociateResourceTypesRequestTypeDef definition

class DisassociateResourceTypesRequestTypeDef(TypedDict):
    ConfigurationRecorderArn: str,
    ResourceTypes: Sequence[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## EvaluationContextTypeDef

```python
# EvaluationContextTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EvaluationContextTypeDef


def get_value() -> EvaluationContextTypeDef:
    return {
        "EvaluationContextIdentifier": ...,
    }


# EvaluationContextTypeDef definition

class EvaluationContextTypeDef(TypedDict):
    EvaluationContextIdentifier: NotRequired[str],
```

## EvaluationOutputTypeDef

```python
# EvaluationOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EvaluationOutputTypeDef


def get_value() -> EvaluationOutputTypeDef:
    return {
        "ComplianceResourceType": ...,
    }


# EvaluationOutputTypeDef definition

class EvaluationOutputTypeDef(TypedDict):
    ComplianceResourceType: str,
    ComplianceResourceId: str,
    ComplianceType: ComplianceTypeType,  # (1)
    OrderingTimestamp: datetime,
    Annotation: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## EvaluationResultQualifierTypeDef

```python
# EvaluationResultQualifierTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EvaluationResultQualifierTypeDef


def get_value() -> EvaluationResultQualifierTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# EvaluationResultQualifierTypeDef definition

class EvaluationResultQualifierTypeDef(TypedDict):
    ConfigRuleName: NotRequired[str],
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    EvaluationMode: NotRequired[EvaluationModeType],  # (1)
```

1. See [:material-code-brackets: EvaluationModeType](./literals.md#evaluationmodetype) 
## EvaluationStatusTypeDef

```python
# EvaluationStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EvaluationStatusTypeDef


def get_value() -> EvaluationStatusTypeDef:
    return {
        "Status": ...,
    }


# EvaluationStatusTypeDef definition

class EvaluationStatusTypeDef(TypedDict):
    Status: ResourceEvaluationStatusType,  # (1)
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: ResourceEvaluationStatusType](./literals.md#resourceevaluationstatustype) 
## ExclusionByResourceTypesOutputTypeDef

```python
# ExclusionByResourceTypesOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ExclusionByResourceTypesOutputTypeDef


def get_value() -> ExclusionByResourceTypesOutputTypeDef:
    return {
        "resourceTypes": ...,
    }


# ExclusionByResourceTypesOutputTypeDef definition

class ExclusionByResourceTypesOutputTypeDef(TypedDict):
    resourceTypes: NotRequired[List[ResourceTypeType]],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ExclusionByResourceTypesTypeDef

```python
# ExclusionByResourceTypesTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ExclusionByResourceTypesTypeDef


def get_value() -> ExclusionByResourceTypesTypeDef:
    return {
        "resourceTypes": ...,
    }


# ExclusionByResourceTypesTypeDef definition

class ExclusionByResourceTypesTypeDef(TypedDict):
    resourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## SsmControlsTypeDef

```python
# SsmControlsTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SsmControlsTypeDef


def get_value() -> SsmControlsTypeDef:
    return {
        "ConcurrentExecutionRatePercentage": ...,
    }


# SsmControlsTypeDef definition

class SsmControlsTypeDef(TypedDict):
    ConcurrentExecutionRatePercentage: NotRequired[int],
    ErrorPercentage: NotRequired[int],
```

## FieldInfoTypeDef

```python
# FieldInfoTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import FieldInfoTypeDef


def get_value() -> FieldInfoTypeDef:
    return {
        "Name": ...,
    }


# FieldInfoTypeDef definition

class FieldInfoTypeDef(TypedDict):
    Name: NotRequired[str],
```

## GetAggregateComplianceDetailsByConfigRuleRequestTypeDef

```python
# GetAggregateComplianceDetailsByConfigRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateComplianceDetailsByConfigRuleRequestTypeDef


def get_value() -> GetAggregateComplianceDetailsByConfigRuleRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# GetAggregateComplianceDetailsByConfigRuleRequestTypeDef definition

class GetAggregateComplianceDetailsByConfigRuleRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    ConfigRuleName: str,
    AccountId: str,
    AwsRegion: str,
    ComplianceType: NotRequired[ComplianceTypeType],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## ResourceCountFiltersTypeDef

```python
# ResourceCountFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceCountFiltersTypeDef


def get_value() -> ResourceCountFiltersTypeDef:
    return {
        "ResourceType": ...,
    }


# ResourceCountFiltersTypeDef definition

class ResourceCountFiltersTypeDef(TypedDict):
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    AccountId: NotRequired[str],
    Region: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## GroupedResourceCountTypeDef

```python
# GroupedResourceCountTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GroupedResourceCountTypeDef


def get_value() -> GroupedResourceCountTypeDef:
    return {
        "GroupName": ...,
    }


# GroupedResourceCountTypeDef definition

class GroupedResourceCountTypeDef(TypedDict):
    GroupName: str,
    ResourceCount: int,
```

## GetComplianceDetailsByConfigRuleRequestTypeDef

```python
# GetComplianceDetailsByConfigRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceDetailsByConfigRuleRequestTypeDef


def get_value() -> GetComplianceDetailsByConfigRuleRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# GetComplianceDetailsByConfigRuleRequestTypeDef definition

class GetComplianceDetailsByConfigRuleRequestTypeDef(TypedDict):
    ConfigRuleName: str,
    ComplianceTypes: NotRequired[Sequence[ComplianceTypeType]],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## GetComplianceDetailsByResourceRequestTypeDef

```python
# GetComplianceDetailsByResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceDetailsByResourceRequestTypeDef


def get_value() -> GetComplianceDetailsByResourceRequestTypeDef:
    return {
        "ResourceType": ...,
    }


# GetComplianceDetailsByResourceRequestTypeDef definition

class GetComplianceDetailsByResourceRequestTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    ComplianceTypes: NotRequired[Sequence[ComplianceTypeType]],  # (1)
    NextToken: NotRequired[str],
    ResourceEvaluationId: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## GetComplianceSummaryByResourceTypeRequestTypeDef

```python
# GetComplianceSummaryByResourceTypeRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceSummaryByResourceTypeRequestTypeDef


def get_value() -> GetComplianceSummaryByResourceTypeRequestTypeDef:
    return {
        "ResourceTypes": ...,
    }


# GetComplianceSummaryByResourceTypeRequestTypeDef definition

class GetComplianceSummaryByResourceTypeRequestTypeDef(TypedDict):
    ResourceTypes: NotRequired[Sequence[str]],
```

## GetConformancePackComplianceSummaryRequestTypeDef

```python
# GetConformancePackComplianceSummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetConformancePackComplianceSummaryRequestTypeDef


def get_value() -> GetConformancePackComplianceSummaryRequestTypeDef:
    return {
        "ConformancePackNames": ...,
    }


# GetConformancePackComplianceSummaryRequestTypeDef definition

class GetConformancePackComplianceSummaryRequestTypeDef(TypedDict):
    ConformancePackNames: Sequence[str],
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetCustomRulePolicyRequestTypeDef

```python
# GetCustomRulePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetCustomRulePolicyRequestTypeDef


def get_value() -> GetCustomRulePolicyRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# GetCustomRulePolicyRequestTypeDef definition

class GetCustomRulePolicyRequestTypeDef(TypedDict):
    ConfigRuleName: NotRequired[str],
```

## GetDiscoveredResourceCountsRequestTypeDef

```python
# GetDiscoveredResourceCountsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetDiscoveredResourceCountsRequestTypeDef


def get_value() -> GetDiscoveredResourceCountsRequestTypeDef:
    return {
        "resourceTypes": ...,
    }


# GetDiscoveredResourceCountsRequestTypeDef definition

class GetDiscoveredResourceCountsRequestTypeDef(TypedDict):
    resourceTypes: NotRequired[Sequence[str]],
    limit: NotRequired[int],
    nextToken: NotRequired[str],
```

## ResourceCountTypeDef

```python
# ResourceCountTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceCountTypeDef


def get_value() -> ResourceCountTypeDef:
    return {
        "resourceType": ...,
    }


# ResourceCountTypeDef definition

class ResourceCountTypeDef(TypedDict):
    resourceType: NotRequired[ResourceTypeType],  # (1)
    count: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## StatusDetailFiltersTypeDef

```python
# StatusDetailFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StatusDetailFiltersTypeDef


def get_value() -> StatusDetailFiltersTypeDef:
    return {
        "AccountId": ...,
    }


# StatusDetailFiltersTypeDef definition

class StatusDetailFiltersTypeDef(TypedDict):
    AccountId: NotRequired[str],
    MemberAccountRuleStatus: NotRequired[MemberAccountRuleStatusType],  # (1)
```

1. See [:material-code-brackets: MemberAccountRuleStatusType](./literals.md#memberaccountrulestatustype) 
## MemberAccountStatusTypeDef

```python
# MemberAccountStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import MemberAccountStatusTypeDef


def get_value() -> MemberAccountStatusTypeDef:
    return {
        "AccountId": ...,
    }


# MemberAccountStatusTypeDef definition

class MemberAccountStatusTypeDef(TypedDict):
    AccountId: str,
    ConfigRuleName: str,
    MemberAccountRuleStatus: MemberAccountRuleStatusType,  # (1)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    LastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: MemberAccountRuleStatusType](./literals.md#memberaccountrulestatustype) 
## OrganizationResourceDetailedStatusFiltersTypeDef

```python
# OrganizationResourceDetailedStatusFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationResourceDetailedStatusFiltersTypeDef


def get_value() -> OrganizationResourceDetailedStatusFiltersTypeDef:
    return {
        "AccountId": ...,
    }


# OrganizationResourceDetailedStatusFiltersTypeDef definition

class OrganizationResourceDetailedStatusFiltersTypeDef(TypedDict):
    AccountId: NotRequired[str],
    Status: NotRequired[OrganizationResourceDetailedStatusType],  # (1)
```

1. See [:material-code-brackets: OrganizationResourceDetailedStatusType](./literals.md#organizationresourcedetailedstatustype) 
## OrganizationConformancePackDetailedStatusTypeDef

```python
# OrganizationConformancePackDetailedStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationConformancePackDetailedStatusTypeDef


def get_value() -> OrganizationConformancePackDetailedStatusTypeDef:
    return {
        "AccountId": ...,
    }


# OrganizationConformancePackDetailedStatusTypeDef definition

class OrganizationConformancePackDetailedStatusTypeDef(TypedDict):
    AccountId: str,
    ConformancePackName: str,
    Status: OrganizationResourceDetailedStatusType,  # (1)
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
    LastUpdateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: OrganizationResourceDetailedStatusType](./literals.md#organizationresourcedetailedstatustype) 
## GetOrganizationCustomRulePolicyRequestTypeDef

```python
# GetOrganizationCustomRulePolicyRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetOrganizationCustomRulePolicyRequestTypeDef


def get_value() -> GetOrganizationCustomRulePolicyRequestTypeDef:
    return {
        "OrganizationConfigRuleName": ...,
    }


# GetOrganizationCustomRulePolicyRequestTypeDef definition

class GetOrganizationCustomRulePolicyRequestTypeDef(TypedDict):
    OrganizationConfigRuleName: str,
```

## GetResourceEvaluationSummaryRequestTypeDef

```python
# GetResourceEvaluationSummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetResourceEvaluationSummaryRequestTypeDef


def get_value() -> GetResourceEvaluationSummaryRequestTypeDef:
    return {
        "ResourceEvaluationId": ...,
    }


# GetResourceEvaluationSummaryRequestTypeDef definition

class GetResourceEvaluationSummaryRequestTypeDef(TypedDict):
    ResourceEvaluationId: str,
```

## ResourceDetailsTypeDef

```python
# ResourceDetailsTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceDetailsTypeDef


def get_value() -> ResourceDetailsTypeDef:
    return {
        "ResourceId": ...,
    }


# ResourceDetailsTypeDef definition

class ResourceDetailsTypeDef(TypedDict):
    ResourceId: str,
    ResourceType: str,
    ResourceConfiguration: str,
    ResourceConfigurationSchemaType: NotRequired[ResourceConfigurationSchemaTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceConfigurationSchemaTypeType](./literals.md#resourceconfigurationschematypetype) 
## GetStoredQueryRequestTypeDef

```python
# GetStoredQueryRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetStoredQueryRequestTypeDef


def get_value() -> GetStoredQueryRequestTypeDef:
    return {
        "QueryName": ...,
    }


# GetStoredQueryRequestTypeDef definition

class GetStoredQueryRequestTypeDef(TypedDict):
    QueryName: str,
```

## StoredQueryTypeDef

```python
# StoredQueryTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StoredQueryTypeDef


def get_value() -> StoredQueryTypeDef:
    return {
        "QueryId": ...,
    }


# StoredQueryTypeDef definition

class StoredQueryTypeDef(TypedDict):
    QueryName: str,
    QueryId: NotRequired[str],
    QueryArn: NotRequired[str],
    Description: NotRequired[str],
    Expression: NotRequired[str],
```

## ResourceFiltersTypeDef

```python
# ResourceFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceFiltersTypeDef


def get_value() -> ResourceFiltersTypeDef:
    return {
        "AccountId": ...,
    }


# ResourceFiltersTypeDef definition

class ResourceFiltersTypeDef(TypedDict):
    AccountId: NotRequired[str],
    ResourceId: NotRequired[str],
    ResourceName: NotRequired[str],
    Region: NotRequired[str],
```

## ListDiscoveredResourcesRequestTypeDef

```python
# ListDiscoveredResourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListDiscoveredResourcesRequestTypeDef


def get_value() -> ListDiscoveredResourcesRequestTypeDef:
    return {
        "resourceType": ...,
    }


# ListDiscoveredResourcesRequestTypeDef definition

class ListDiscoveredResourcesRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    resourceIds: NotRequired[Sequence[str]],
    resourceName: NotRequired[str],
    limit: NotRequired[int],
    includeDeletedResources: NotRequired[bool],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ResourceIdentifierTypeDef

```python
# ResourceIdentifierTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceIdentifierTypeDef


def get_value() -> ResourceIdentifierTypeDef:
    return {
        "resourceType": ...,
    }


# ResourceIdentifierTypeDef definition

class ResourceIdentifierTypeDef(TypedDict):
    resourceType: NotRequired[ResourceTypeType],  # (1)
    resourceId: NotRequired[str],
    resourceName: NotRequired[str],
    resourceDeletionTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ResourceEvaluationTypeDef

```python
# ResourceEvaluationTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceEvaluationTypeDef


def get_value() -> ResourceEvaluationTypeDef:
    return {
        "ResourceEvaluationId": ...,
    }


# ResourceEvaluationTypeDef definition

class ResourceEvaluationTypeDef(TypedDict):
    ResourceEvaluationId: NotRequired[str],
    EvaluationMode: NotRequired[EvaluationModeType],  # (1)
    EvaluationStartTimestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: EvaluationModeType](./literals.md#evaluationmodetype) 
## ListStoredQueriesRequestTypeDef

```python
# ListStoredQueriesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListStoredQueriesRequestTypeDef


def get_value() -> ListStoredQueriesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListStoredQueriesRequestTypeDef definition

class ListStoredQueriesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## StoredQueryMetadataTypeDef

```python
# StoredQueryMetadataTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StoredQueryMetadataTypeDef


def get_value() -> StoredQueryMetadataTypeDef:
    return {
        "QueryId": ...,
    }


# StoredQueryMetadataTypeDef definition

class StoredQueryMetadataTypeDef(TypedDict):
    QueryId: str,
    QueryArn: str,
    QueryName: str,
    Description: NotRequired[str],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## OrganizationAggregationSourceTypeDef

```python
# OrganizationAggregationSourceTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationAggregationSourceTypeDef


def get_value() -> OrganizationAggregationSourceTypeDef:
    return {
        "RoleArn": ...,
    }


# OrganizationAggregationSourceTypeDef definition

class OrganizationAggregationSourceTypeDef(TypedDict):
    RoleArn: str,
    AwsRegions: NotRequired[Sequence[str]],
    AllAwsRegions: NotRequired[bool],
```

## OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef

```python
# OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef


def get_value() -> OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef:
    return {
        "Description": ...,
    }


# OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef definition

class OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef(TypedDict):
    Description: NotRequired[str],
    OrganizationConfigRuleTriggerTypes: NotRequired[List[OrganizationConfigRuleTriggerTypeNoSNType]],  # (1)
    InputParameters: NotRequired[str],
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (2)
    ResourceTypesScope: NotRequired[List[str]],
    ResourceIdScope: NotRequired[str],
    TagKeyScope: NotRequired[str],
    TagValueScope: NotRequired[str],
    PolicyRuntime: NotRequired[str],
    DebugLogDeliveryAccounts: NotRequired[List[str]],
```

1. See [:material-code-brackets: OrganizationConfigRuleTriggerTypeNoSNType](./literals.md#organizationconfigruletriggertypenosntype) 
2. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
## OrganizationCustomRuleMetadataOutputTypeDef

```python
# OrganizationCustomRuleMetadataOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationCustomRuleMetadataOutputTypeDef


def get_value() -> OrganizationCustomRuleMetadataOutputTypeDef:
    return {
        "Description": ...,
    }


# OrganizationCustomRuleMetadataOutputTypeDef definition

class OrganizationCustomRuleMetadataOutputTypeDef(TypedDict):
    LambdaFunctionArn: str,
    OrganizationConfigRuleTriggerTypes: List[OrganizationConfigRuleTriggerTypeType],  # (1)
    Description: NotRequired[str],
    InputParameters: NotRequired[str],
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (2)
    ResourceTypesScope: NotRequired[List[str]],
    ResourceIdScope: NotRequired[str],
    TagKeyScope: NotRequired[str],
    TagValueScope: NotRequired[str],
```

1. See [:material-code-brackets: OrganizationConfigRuleTriggerTypeType](./literals.md#organizationconfigruletriggertypetype) 
2. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
## OrganizationManagedRuleMetadataOutputTypeDef

```python
# OrganizationManagedRuleMetadataOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationManagedRuleMetadataOutputTypeDef


def get_value() -> OrganizationManagedRuleMetadataOutputTypeDef:
    return {
        "Description": ...,
    }


# OrganizationManagedRuleMetadataOutputTypeDef definition

class OrganizationManagedRuleMetadataOutputTypeDef(TypedDict):
    RuleIdentifier: str,
    Description: NotRequired[str],
    InputParameters: NotRequired[str],
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (1)
    ResourceTypesScope: NotRequired[List[str]],
    ResourceIdScope: NotRequired[str],
    TagKeyScope: NotRequired[str],
    TagValueScope: NotRequired[str],
```

1. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
## OrganizationCustomPolicyRuleMetadataTypeDef

```python
# OrganizationCustomPolicyRuleMetadataTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationCustomPolicyRuleMetadataTypeDef


def get_value() -> OrganizationCustomPolicyRuleMetadataTypeDef:
    return {
        "Description": ...,
    }


# OrganizationCustomPolicyRuleMetadataTypeDef definition

class OrganizationCustomPolicyRuleMetadataTypeDef(TypedDict):
    PolicyRuntime: str,
    PolicyText: str,
    Description: NotRequired[str],
    OrganizationConfigRuleTriggerTypes: NotRequired[Sequence[OrganizationConfigRuleTriggerTypeNoSNType]],  # (1)
    InputParameters: NotRequired[str],
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (2)
    ResourceTypesScope: NotRequired[Sequence[str]],
    ResourceIdScope: NotRequired[str],
    TagKeyScope: NotRequired[str],
    TagValueScope: NotRequired[str],
    DebugLogDeliveryAccounts: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: OrganizationConfigRuleTriggerTypeNoSNType](./literals.md#organizationconfigruletriggertypenosntype) 
2. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
## OrganizationCustomRuleMetadataTypeDef

```python
# OrganizationCustomRuleMetadataTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationCustomRuleMetadataTypeDef


def get_value() -> OrganizationCustomRuleMetadataTypeDef:
    return {
        "Description": ...,
    }


# OrganizationCustomRuleMetadataTypeDef definition

class OrganizationCustomRuleMetadataTypeDef(TypedDict):
    LambdaFunctionArn: str,
    OrganizationConfigRuleTriggerTypes: Sequence[OrganizationConfigRuleTriggerTypeType],  # (1)
    Description: NotRequired[str],
    InputParameters: NotRequired[str],
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (2)
    ResourceTypesScope: NotRequired[Sequence[str]],
    ResourceIdScope: NotRequired[str],
    TagKeyScope: NotRequired[str],
    TagValueScope: NotRequired[str],
```

1. See [:material-code-brackets: OrganizationConfigRuleTriggerTypeType](./literals.md#organizationconfigruletriggertypetype) 
2. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
## OrganizationManagedRuleMetadataTypeDef

```python
# OrganizationManagedRuleMetadataTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationManagedRuleMetadataTypeDef


def get_value() -> OrganizationManagedRuleMetadataTypeDef:
    return {
        "Description": ...,
    }


# OrganizationManagedRuleMetadataTypeDef definition

class OrganizationManagedRuleMetadataTypeDef(TypedDict):
    RuleIdentifier: str,
    Description: NotRequired[str],
    InputParameters: NotRequired[str],
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (1)
    ResourceTypesScope: NotRequired[Sequence[str]],
    ResourceIdScope: NotRequired[str],
    TagKeyScope: NotRequired[str],
    TagValueScope: NotRequired[str],
```

1. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
## PutResourceConfigRequestTypeDef

```python
# PutResourceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutResourceConfigRequestTypeDef


def get_value() -> PutResourceConfigRequestTypeDef:
    return {
        "ResourceType": ...,
    }


# PutResourceConfigRequestTypeDef definition

class PutResourceConfigRequestTypeDef(TypedDict):
    ResourceType: str,
    SchemaVersionId: str,
    ResourceId: str,
    Configuration: str,
    ResourceName: NotRequired[str],
    Tags: NotRequired[Mapping[str, str]],
```

## PutRetentionConfigurationRequestTypeDef

```python
# PutRetentionConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutRetentionConfigurationRequestTypeDef


def get_value() -> PutRetentionConfigurationRequestTypeDef:
    return {
        "RetentionPeriodInDays": ...,
    }


# PutRetentionConfigurationRequestTypeDef definition

class PutRetentionConfigurationRequestTypeDef(TypedDict):
    RetentionPeriodInDays: int,
```

## RecordingStrategyTypeDef

```python
# RecordingStrategyTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RecordingStrategyTypeDef


def get_value() -> RecordingStrategyTypeDef:
    return {
        "useOnly": ...,
    }


# RecordingStrategyTypeDef definition

class RecordingStrategyTypeDef(TypedDict):
    useOnly: NotRequired[RecordingStrategyTypeType],  # (1)
```

1. See [:material-code-brackets: RecordingStrategyTypeType](./literals.md#recordingstrategytypetype) 
## RecordingModeOverrideOutputTypeDef

```python
# RecordingModeOverrideOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RecordingModeOverrideOutputTypeDef


def get_value() -> RecordingModeOverrideOutputTypeDef:
    return {
        "description": ...,
    }


# RecordingModeOverrideOutputTypeDef definition

class RecordingModeOverrideOutputTypeDef(TypedDict):
    resourceTypes: List[ResourceTypeType],  # (1)
    recordingFrequency: RecordingFrequencyType,  # (2)
    description: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: RecordingFrequencyType](./literals.md#recordingfrequencytype) 
## RecordingModeOverrideTypeDef

```python
# RecordingModeOverrideTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RecordingModeOverrideTypeDef


def get_value() -> RecordingModeOverrideTypeDef:
    return {
        "description": ...,
    }


# RecordingModeOverrideTypeDef definition

class RecordingModeOverrideTypeDef(TypedDict):
    resourceTypes: Sequence[ResourceTypeType],  # (1)
    recordingFrequency: RecordingFrequencyType,  # (2)
    description: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: RecordingFrequencyType](./literals.md#recordingfrequencytype) 
## RemediationExecutionStepTypeDef

```python
# RemediationExecutionStepTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RemediationExecutionStepTypeDef


def get_value() -> RemediationExecutionStepTypeDef:
    return {
        "Name": ...,
    }


# RemediationExecutionStepTypeDef definition

class RemediationExecutionStepTypeDef(TypedDict):
    Name: NotRequired[str],
    State: NotRequired[RemediationExecutionStepStateType],  # (1)
    ErrorMessage: NotRequired[str],
    StartTime: NotRequired[datetime],
    StopTime: NotRequired[datetime],
```

1. See [:material-code-brackets: RemediationExecutionStepStateType](./literals.md#remediationexecutionstepstatetype) 
## ResourceValueTypeDef

```python
# ResourceValueTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceValueTypeDef


def get_value() -> ResourceValueTypeDef:
    return {
        "Value": ...,
    }


# ResourceValueTypeDef definition

class ResourceValueTypeDef(TypedDict):
    Value: ResourceValueTypeType,  # (1)
```

1. See [:material-code-brackets: ResourceValueTypeType](./literals.md#resourcevaluetypetype) 
## StaticValueOutputTypeDef

```python
# StaticValueOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StaticValueOutputTypeDef


def get_value() -> StaticValueOutputTypeDef:
    return {
        "Values": ...,
    }


# StaticValueOutputTypeDef definition

class StaticValueOutputTypeDef(TypedDict):
    Values: List[str],
```

## SelectAggregateResourceConfigRequestTypeDef

```python
# SelectAggregateResourceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SelectAggregateResourceConfigRequestTypeDef


def get_value() -> SelectAggregateResourceConfigRequestTypeDef:
    return {
        "Expression": ...,
    }


# SelectAggregateResourceConfigRequestTypeDef definition

class SelectAggregateResourceConfigRequestTypeDef(TypedDict):
    Expression: str,
    ConfigurationAggregatorName: str,
    Limit: NotRequired[int],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SelectResourceConfigRequestTypeDef

```python
# SelectResourceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SelectResourceConfigRequestTypeDef


def get_value() -> SelectResourceConfigRequestTypeDef:
    return {
        "Expression": ...,
    }


# SelectResourceConfigRequestTypeDef definition

class SelectResourceConfigRequestTypeDef(TypedDict):
    Expression: str,
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

## SourceDetailTypeDef

```python
# SourceDetailTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SourceDetailTypeDef


def get_value() -> SourceDetailTypeDef:
    return {
        "EventSource": ...,
    }


# SourceDetailTypeDef definition

class SourceDetailTypeDef(TypedDict):
    EventSource: NotRequired[EventSourceType],  # (1)
    MessageType: NotRequired[MessageTypeType],  # (2)
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (3)
```

1. See [:material-code-brackets: EventSourceType](./literals.md#eventsourcetype) 
2. See [:material-code-brackets: MessageTypeType](./literals.md#messagetypetype) 
3. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
## StartConfigRulesEvaluationRequestTypeDef

```python
# StartConfigRulesEvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StartConfigRulesEvaluationRequestTypeDef


def get_value() -> StartConfigRulesEvaluationRequestTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# StartConfigRulesEvaluationRequestTypeDef definition

class StartConfigRulesEvaluationRequestTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
```

## StartConfigurationRecorderRequestTypeDef

```python
# StartConfigurationRecorderRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StartConfigurationRecorderRequestTypeDef


def get_value() -> StartConfigurationRecorderRequestTypeDef:
    return {
        "ConfigurationRecorderName": ...,
    }


# StartConfigurationRecorderRequestTypeDef definition

class StartConfigurationRecorderRequestTypeDef(TypedDict):
    ConfigurationRecorderName: str,
```

## StaticValueTypeDef

```python
# StaticValueTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StaticValueTypeDef


def get_value() -> StaticValueTypeDef:
    return {
        "Values": ...,
    }


# StaticValueTypeDef definition

class StaticValueTypeDef(TypedDict):
    Values: Sequence[str],
```

## StopConfigurationRecorderRequestTypeDef

```python
# StopConfigurationRecorderRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StopConfigurationRecorderRequestTypeDef


def get_value() -> StopConfigurationRecorderRequestTypeDef:
    return {
        "ConfigurationRecorderName": ...,
    }


# StopConfigurationRecorderRequestTypeDef definition

class StopConfigurationRecorderRequestTypeDef(TypedDict):
    ConfigurationRecorderName: str,
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## AggregateComplianceByConformancePackTypeDef

```python
# AggregateComplianceByConformancePackTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateComplianceByConformancePackTypeDef


def get_value() -> AggregateComplianceByConformancePackTypeDef:
    return {
        "ConformancePackName": ...,
    }


# AggregateComplianceByConformancePackTypeDef definition

class AggregateComplianceByConformancePackTypeDef(TypedDict):
    ConformancePackName: NotRequired[str],
    Compliance: NotRequired[AggregateConformancePackComplianceTypeDef],  # (1)
    AccountId: NotRequired[str],
    AwsRegion: NotRequired[str],
```

1. See [:material-code-braces: AggregateConformancePackComplianceTypeDef](./type_defs.md#aggregateconformancepackcompliancetypedef) 
## AggregateConformancePackComplianceSummaryTypeDef

```python
# AggregateConformancePackComplianceSummaryTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateConformancePackComplianceSummaryTypeDef


def get_value() -> AggregateConformancePackComplianceSummaryTypeDef:
    return {
        "ComplianceSummary": ...,
    }


# AggregateConformancePackComplianceSummaryTypeDef definition

class AggregateConformancePackComplianceSummaryTypeDef(TypedDict):
    ComplianceSummary: NotRequired[AggregateConformancePackComplianceCountTypeDef],  # (1)
    GroupName: NotRequired[str],
```

1. See [:material-code-braces: AggregateConformancePackComplianceCountTypeDef](./type_defs.md#aggregateconformancepackcompliancecounttypedef) 
## DescribeAggregateComplianceByConformancePacksRequestTypeDef

```python
# DescribeAggregateComplianceByConformancePacksRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregateComplianceByConformancePacksRequestTypeDef


def get_value() -> DescribeAggregateComplianceByConformancePacksRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# DescribeAggregateComplianceByConformancePacksRequestTypeDef definition

class DescribeAggregateComplianceByConformancePacksRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    Filters: NotRequired[AggregateConformancePackComplianceFiltersTypeDef],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregateConformancePackComplianceFiltersTypeDef](./type_defs.md#aggregateconformancepackcompliancefilterstypedef) 
## GetAggregateConformancePackComplianceSummaryRequestTypeDef

```python
# GetAggregateConformancePackComplianceSummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateConformancePackComplianceSummaryRequestTypeDef


def get_value() -> GetAggregateConformancePackComplianceSummaryRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# GetAggregateConformancePackComplianceSummaryRequestTypeDef definition

class GetAggregateConformancePackComplianceSummaryRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    Filters: NotRequired[AggregateConformancePackComplianceSummaryFiltersTypeDef],  # (1)
    GroupByKey: NotRequired[AggregateConformancePackComplianceSummaryGroupKeyType],  # (2)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregateConformancePackComplianceSummaryFiltersTypeDef](./type_defs.md#aggregateconformancepackcompliancesummaryfilterstypedef) 
2. See [:material-code-brackets: AggregateConformancePackComplianceSummaryGroupKeyType](./literals.md#aggregateconformancepackcompliancesummarygroupkeytype) 
## BatchGetAggregateResourceConfigRequestTypeDef

```python
# BatchGetAggregateResourceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import BatchGetAggregateResourceConfigRequestTypeDef


def get_value() -> BatchGetAggregateResourceConfigRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# BatchGetAggregateResourceConfigRequestTypeDef definition

class BatchGetAggregateResourceConfigRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    ResourceIdentifiers: Sequence[AggregateResourceIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: AggregateResourceIdentifierTypeDef](./type_defs.md#aggregateresourceidentifiertypedef) 
## GetAggregateResourceConfigRequestTypeDef

```python
# GetAggregateResourceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateResourceConfigRequestTypeDef


def get_value() -> GetAggregateResourceConfigRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# GetAggregateResourceConfigRequestTypeDef definition

class GetAggregateResourceConfigRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    ResourceIdentifier: AggregateResourceIdentifierTypeDef,  # (1)
```

1. See [:material-code-braces: AggregateResourceIdentifierTypeDef](./type_defs.md#aggregateresourceidentifiertypedef) 
## AggregatorFiltersOutputTypeDef

```python
# AggregatorFiltersOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregatorFiltersOutputTypeDef


def get_value() -> AggregatorFiltersOutputTypeDef:
    return {
        "ResourceType": ...,
    }


# AggregatorFiltersOutputTypeDef definition

class AggregatorFiltersOutputTypeDef(TypedDict):
    ResourceType: NotRequired[AggregatorFilterResourceTypeOutputTypeDef],  # (1)
    ServicePrincipal: NotRequired[AggregatorFilterServicePrincipalOutputTypeDef],  # (2)
```

1. See [:material-code-braces: AggregatorFilterResourceTypeOutputTypeDef](./type_defs.md#aggregatorfilterresourcetypeoutputtypedef) 
2. See [:material-code-braces: AggregatorFilterServicePrincipalOutputTypeDef](./type_defs.md#aggregatorfilterserviceprincipaloutputtypedef) 
## AggregatorFiltersTypeDef

```python
# AggregatorFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregatorFiltersTypeDef


def get_value() -> AggregatorFiltersTypeDef:
    return {
        "ResourceType": ...,
    }


# AggregatorFiltersTypeDef definition

class AggregatorFiltersTypeDef(TypedDict):
    ResourceType: NotRequired[AggregatorFilterResourceTypeTypeDef],  # (1)
    ServicePrincipal: NotRequired[AggregatorFilterServicePrincipalTypeDef],  # (2)
```

1. See [:material-code-braces: AggregatorFilterResourceTypeTypeDef](./type_defs.md#aggregatorfilterresourcetypetypedef) 
2. See [:material-code-braces: AggregatorFilterServicePrincipalTypeDef](./type_defs.md#aggregatorfilterserviceprincipaltypedef) 
## DeleteServiceLinkedConfigurationRecorderResponseTypeDef

```python
# DeleteServiceLinkedConfigurationRecorderResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteServiceLinkedConfigurationRecorderResponseTypeDef


def get_value() -> DeleteServiceLinkedConfigurationRecorderResponseTypeDef:
    return {
        "Arn": ...,
    }


# DeleteServiceLinkedConfigurationRecorderResponseTypeDef definition

class DeleteServiceLinkedConfigurationRecorderResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeliverConfigSnapshotResponseTypeDef

```python
# DeliverConfigSnapshotResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeliverConfigSnapshotResponseTypeDef


def get_value() -> DeliverConfigSnapshotResponseTypeDef:
    return {
        "configSnapshotId": ...,
    }


# DeliverConfigSnapshotResponseTypeDef definition

class DeliverConfigSnapshotResponseTypeDef(TypedDict):
    configSnapshotId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAggregationAuthorizationsResponseTypeDef

```python
# DescribeAggregationAuthorizationsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregationAuthorizationsResponseTypeDef


def get_value() -> DescribeAggregationAuthorizationsResponseTypeDef:
    return {
        "AggregationAuthorizations": ...,
    }


# DescribeAggregationAuthorizationsResponseTypeDef definition

class DescribeAggregationAuthorizationsResponseTypeDef(TypedDict):
    AggregationAuthorizations: List[AggregationAuthorizationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregationAuthorizationTypeDef](./type_defs.md#aggregationauthorizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationAggregatorSourcesStatusResponseTypeDef

```python
# DescribeConfigurationAggregatorSourcesStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationAggregatorSourcesStatusResponseTypeDef


def get_value() -> DescribeConfigurationAggregatorSourcesStatusResponseTypeDef:
    return {
        "AggregatedSourceStatusList": ...,
    }


# DescribeConfigurationAggregatorSourcesStatusResponseTypeDef definition

class DescribeConfigurationAggregatorSourcesStatusResponseTypeDef(TypedDict):
    AggregatedSourceStatusList: List[AggregatedSourceStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregatedSourceStatusTypeDef](./type_defs.md#aggregatedsourcestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCustomRulePolicyResponseTypeDef

```python
# GetCustomRulePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetCustomRulePolicyResponseTypeDef


def get_value() -> GetCustomRulePolicyResponseTypeDef:
    return {
        "PolicyText": ...,
    }


# GetCustomRulePolicyResponseTypeDef definition

class GetCustomRulePolicyResponseTypeDef(TypedDict):
    PolicyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOrganizationCustomRulePolicyResponseTypeDef

```python
# GetOrganizationCustomRulePolicyResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetOrganizationCustomRulePolicyResponseTypeDef


def get_value() -> GetOrganizationCustomRulePolicyResponseTypeDef:
    return {
        "PolicyText": ...,
    }


# GetOrganizationCustomRulePolicyResponseTypeDef definition

class GetOrganizationCustomRulePolicyResponseTypeDef(TypedDict):
    PolicyText: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAggregateDiscoveredResourcesResponseTypeDef

```python
# ListAggregateDiscoveredResourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListAggregateDiscoveredResourcesResponseTypeDef


def get_value() -> ListAggregateDiscoveredResourcesResponseTypeDef:
    return {
        "ResourceIdentifiers": ...,
    }


# ListAggregateDiscoveredResourcesResponseTypeDef definition

class ListAggregateDiscoveredResourcesResponseTypeDef(TypedDict):
    ResourceIdentifiers: List[AggregateResourceIdentifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregateResourceIdentifierTypeDef](./type_defs.md#aggregateresourceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAggregationAuthorizationResponseTypeDef

```python
# PutAggregationAuthorizationResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutAggregationAuthorizationResponseTypeDef


def get_value() -> PutAggregationAuthorizationResponseTypeDef:
    return {
        "AggregationAuthorization": ...,
    }


# PutAggregationAuthorizationResponseTypeDef definition

class PutAggregationAuthorizationResponseTypeDef(TypedDict):
    AggregationAuthorization: AggregationAuthorizationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AggregationAuthorizationTypeDef](./type_defs.md#aggregationauthorizationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConformancePackResponseTypeDef

```python
# PutConformancePackResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutConformancePackResponseTypeDef


def get_value() -> PutConformancePackResponseTypeDef:
    return {
        "ConformancePackArn": ...,
    }


# PutConformancePackResponseTypeDef definition

class PutConformancePackResponseTypeDef(TypedDict):
    ConformancePackArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutOrganizationConfigRuleResponseTypeDef

```python
# PutOrganizationConfigRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutOrganizationConfigRuleResponseTypeDef


def get_value() -> PutOrganizationConfigRuleResponseTypeDef:
    return {
        "OrganizationConfigRuleArn": ...,
    }


# PutOrganizationConfigRuleResponseTypeDef definition

class PutOrganizationConfigRuleResponseTypeDef(TypedDict):
    OrganizationConfigRuleArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutOrganizationConformancePackResponseTypeDef

```python
# PutOrganizationConformancePackResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutOrganizationConformancePackResponseTypeDef


def get_value() -> PutOrganizationConformancePackResponseTypeDef:
    return {
        "OrganizationConformancePackArn": ...,
    }


# PutOrganizationConformancePackResponseTypeDef definition

class PutOrganizationConformancePackResponseTypeDef(TypedDict):
    OrganizationConformancePackArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutServiceLinkedConfigurationRecorderResponseTypeDef

```python
# PutServiceLinkedConfigurationRecorderResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutServiceLinkedConfigurationRecorderResponseTypeDef


def get_value() -> PutServiceLinkedConfigurationRecorderResponseTypeDef:
    return {
        "Arn": ...,
    }


# PutServiceLinkedConfigurationRecorderResponseTypeDef definition

class PutServiceLinkedConfigurationRecorderResponseTypeDef(TypedDict):
    Arn: str,
    Name: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutStoredQueryResponseTypeDef

```python
# PutStoredQueryResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutStoredQueryResponseTypeDef


def get_value() -> PutStoredQueryResponseTypeDef:
    return {
        "QueryArn": ...,
    }


# PutStoredQueryResponseTypeDef definition

class PutStoredQueryResponseTypeDef(TypedDict):
    QueryArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartResourceEvaluationResponseTypeDef

```python
# StartResourceEvaluationResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StartResourceEvaluationResponseTypeDef


def get_value() -> StartResourceEvaluationResponseTypeDef:
    return {
        "ResourceEvaluationId": ...,
    }


# StartResourceEvaluationResponseTypeDef definition

class StartResourceEvaluationResponseTypeDef(TypedDict):
    ResourceEvaluationId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetAggregateResourceConfigResponseTypeDef

```python
# BatchGetAggregateResourceConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import BatchGetAggregateResourceConfigResponseTypeDef


def get_value() -> BatchGetAggregateResourceConfigResponseTypeDef:
    return {
        "BaseConfigurationItems": ...,
    }


# BatchGetAggregateResourceConfigResponseTypeDef definition

class BatchGetAggregateResourceConfigResponseTypeDef(TypedDict):
    BaseConfigurationItems: List[BaseConfigurationItemTypeDef],  # (1)
    UnprocessedResourceIdentifiers: List[AggregateResourceIdentifierTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BaseConfigurationItemTypeDef](./type_defs.md#baseconfigurationitemtypedef) 
2. See [:material-code-braces: AggregateResourceIdentifierTypeDef](./type_defs.md#aggregateresourceidentifiertypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetResourceConfigRequestTypeDef

```python
# BatchGetResourceConfigRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import BatchGetResourceConfigRequestTypeDef


def get_value() -> BatchGetResourceConfigRequestTypeDef:
    return {
        "resourceKeys": ...,
    }


# BatchGetResourceConfigRequestTypeDef definition

class BatchGetResourceConfigRequestTypeDef(TypedDict):
    resourceKeys: Sequence[ResourceKeyTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
## BatchGetResourceConfigResponseTypeDef

```python
# BatchGetResourceConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import BatchGetResourceConfigResponseTypeDef


def get_value() -> BatchGetResourceConfigResponseTypeDef:
    return {
        "baseConfigurationItems": ...,
    }


# BatchGetResourceConfigResponseTypeDef definition

class BatchGetResourceConfigResponseTypeDef(TypedDict):
    baseConfigurationItems: List[BaseConfigurationItemTypeDef],  # (1)
    unprocessedResourceKeys: List[ResourceKeyTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BaseConfigurationItemTypeDef](./type_defs.md#baseconfigurationitemtypedef) 
2. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRemediationExecutionStatusRequestTypeDef

```python
# DescribeRemediationExecutionStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRemediationExecutionStatusRequestTypeDef


def get_value() -> DescribeRemediationExecutionStatusRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# DescribeRemediationExecutionStatusRequestTypeDef definition

class DescribeRemediationExecutionStatusRequestTypeDef(TypedDict):
    ConfigRuleName: str,
    ResourceKeys: NotRequired[Sequence[ResourceKeyTypeDef]],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
## StartRemediationExecutionRequestTypeDef

```python
# StartRemediationExecutionRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StartRemediationExecutionRequestTypeDef


def get_value() -> StartRemediationExecutionRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# StartRemediationExecutionRequestTypeDef definition

class StartRemediationExecutionRequestTypeDef(TypedDict):
    ConfigRuleName: str,
    ResourceKeys: Sequence[ResourceKeyTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
## StartRemediationExecutionResponseTypeDef

```python
# StartRemediationExecutionResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StartRemediationExecutionResponseTypeDef


def get_value() -> StartRemediationExecutionResponseTypeDef:
    return {
        "FailureMessage": ...,
    }


# StartRemediationExecutionResponseTypeDef definition

class StartRemediationExecutionResponseTypeDef(TypedDict):
    FailureMessage: str,
    FailedItems: List[ResourceKeyTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ComplianceSummaryTypeDef

```python
# ComplianceSummaryTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ComplianceSummaryTypeDef


def get_value() -> ComplianceSummaryTypeDef:
    return {
        "CompliantResourceCount": ...,
    }


# ComplianceSummaryTypeDef definition

class ComplianceSummaryTypeDef(TypedDict):
    CompliantResourceCount: NotRequired[ComplianceContributorCountTypeDef],  # (1)
    NonCompliantResourceCount: NotRequired[ComplianceContributorCountTypeDef],  # (1)
    ComplianceSummaryTimestamp: NotRequired[datetime],
```

1. See [:material-code-braces: ComplianceContributorCountTypeDef](./type_defs.md#compliancecontributorcounttypedef) 
2. See [:material-code-braces: ComplianceContributorCountTypeDef](./type_defs.md#compliancecontributorcounttypedef) 
## ComplianceTypeDef

```python
# ComplianceTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ComplianceTypeDef


def get_value() -> ComplianceTypeDef:
    return {
        "ComplianceType": ...,
    }


# ComplianceTypeDef definition

class ComplianceTypeDef(TypedDict):
    ComplianceType: NotRequired[ComplianceTypeType],  # (1)
    ComplianceContributorCount: NotRequired[ComplianceContributorCountTypeDef],  # (2)
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: ComplianceContributorCountTypeDef](./type_defs.md#compliancecontributorcounttypedef) 
## DescribeAggregateComplianceByConfigRulesRequestTypeDef

```python
# DescribeAggregateComplianceByConfigRulesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregateComplianceByConfigRulesRequestTypeDef


def get_value() -> DescribeAggregateComplianceByConfigRulesRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# DescribeAggregateComplianceByConfigRulesRequestTypeDef definition

class DescribeAggregateComplianceByConfigRulesRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    Filters: NotRequired[ConfigRuleComplianceFiltersTypeDef],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigRuleComplianceFiltersTypeDef](./type_defs.md#configrulecompliancefilterstypedef) 
## GetAggregateConfigRuleComplianceSummaryRequestTypeDef

```python
# GetAggregateConfigRuleComplianceSummaryRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateConfigRuleComplianceSummaryRequestTypeDef


def get_value() -> GetAggregateConfigRuleComplianceSummaryRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# GetAggregateConfigRuleComplianceSummaryRequestTypeDef definition

class GetAggregateConfigRuleComplianceSummaryRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    Filters: NotRequired[ConfigRuleComplianceSummaryFiltersTypeDef],  # (1)
    GroupByKey: NotRequired[ConfigRuleComplianceSummaryGroupKeyType],  # (2)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigRuleComplianceSummaryFiltersTypeDef](./type_defs.md#configrulecompliancesummaryfilterstypedef) 
2. See [:material-code-brackets: ConfigRuleComplianceSummaryGroupKeyType](./literals.md#configrulecompliancesummarygroupkeytype) 
## DescribeConfigRuleEvaluationStatusResponseTypeDef

```python
# DescribeConfigRuleEvaluationStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigRuleEvaluationStatusResponseTypeDef


def get_value() -> DescribeConfigRuleEvaluationStatusResponseTypeDef:
    return {
        "ConfigRulesEvaluationStatus": ...,
    }


# DescribeConfigRuleEvaluationStatusResponseTypeDef definition

class DescribeConfigRuleEvaluationStatusResponseTypeDef(TypedDict):
    ConfigRulesEvaluationStatus: List[ConfigRuleEvaluationStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigRuleEvaluationStatusTypeDef](./type_defs.md#configruleevaluationstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeliveryChannelTypeDef

```python
# DeliveryChannelTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeliveryChannelTypeDef


def get_value() -> DeliveryChannelTypeDef:
    return {
        "name": ...,
    }


# DeliveryChannelTypeDef definition

class DeliveryChannelTypeDef(TypedDict):
    name: NotRequired[str],
    s3BucketName: NotRequired[str],
    s3KeyPrefix: NotRequired[str],
    s3KmsKeyArn: NotRequired[str],
    snsTopicARN: NotRequired[str],
    configSnapshotDeliveryProperties: NotRequired[ConfigSnapshotDeliveryPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: ConfigSnapshotDeliveryPropertiesTypeDef](./type_defs.md#configsnapshotdeliverypropertiestypedef) 
## DeliveryChannelStatusTypeDef

```python
# DeliveryChannelStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeliveryChannelStatusTypeDef


def get_value() -> DeliveryChannelStatusTypeDef:
    return {
        "name": ...,
    }


# DeliveryChannelStatusTypeDef definition

class DeliveryChannelStatusTypeDef(TypedDict):
    name: NotRequired[str],
    configSnapshotDeliveryInfo: NotRequired[ConfigExportDeliveryInfoTypeDef],  # (1)
    configHistoryDeliveryInfo: NotRequired[ConfigExportDeliveryInfoTypeDef],  # (1)
    configStreamDeliveryInfo: NotRequired[ConfigStreamDeliveryInfoTypeDef],  # (3)
```

1. See [:material-code-braces: ConfigExportDeliveryInfoTypeDef](./type_defs.md#configexportdeliveryinfotypedef) 
2. See [:material-code-braces: ConfigExportDeliveryInfoTypeDef](./type_defs.md#configexportdeliveryinfotypedef) 
3. See [:material-code-braces: ConfigStreamDeliveryInfoTypeDef](./type_defs.md#configstreamdeliveryinfotypedef) 
## ConfigurationItemTypeDef

```python
# ConfigurationItemTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigurationItemTypeDef


def get_value() -> ConfigurationItemTypeDef:
    return {
        "version": ...,
    }


# ConfigurationItemTypeDef definition

class ConfigurationItemTypeDef(TypedDict):
    version: NotRequired[str],
    accountId: NotRequired[str],
    configurationItemCaptureTime: NotRequired[datetime],
    configurationItemStatus: NotRequired[ConfigurationItemStatusType],  # (1)
    configurationStateId: NotRequired[str],
    configurationItemMD5Hash: NotRequired[str],
    arn: NotRequired[str],
    resourceType: NotRequired[ResourceTypeType],  # (2)
    resourceId: NotRequired[str],
    resourceName: NotRequired[str],
    awsRegion: NotRequired[str],
    availabilityZone: NotRequired[str],
    resourceCreationTime: NotRequired[datetime],
    tags: NotRequired[Dict[str, str]],
    relatedEvents: NotRequired[List[str]],
    relationships: NotRequired[List[RelationshipTypeDef]],  # (3)
    configuration: NotRequired[str],
    supplementaryConfiguration: NotRequired[Dict[str, str]],
    recordingFrequency: NotRequired[RecordingFrequencyType],  # (4)
    configurationItemDeliveryTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ConfigurationItemStatusType](./literals.md#configurationitemstatustype) 
2. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
3. See [:material-code-braces: RelationshipTypeDef](./type_defs.md#relationshiptypedef) 
4. See [:material-code-brackets: RecordingFrequencyType](./literals.md#recordingfrequencytype) 
## ListConfigurationRecordersRequestTypeDef

```python
# ListConfigurationRecordersRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListConfigurationRecordersRequestTypeDef


def get_value() -> ListConfigurationRecordersRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListConfigurationRecordersRequestTypeDef definition

class ListConfigurationRecordersRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ConfigurationRecorderFilterTypeDef]],  # (1)
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationRecorderFilterTypeDef](./type_defs.md#configurationrecorderfiltertypedef) 
## DescribeConfigurationRecorderStatusResponseTypeDef

```python
# DescribeConfigurationRecorderStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationRecorderStatusResponseTypeDef


def get_value() -> DescribeConfigurationRecorderStatusResponseTypeDef:
    return {
        "ConfigurationRecordersStatus": ...,
    }


# DescribeConfigurationRecorderStatusResponseTypeDef definition

class DescribeConfigurationRecorderStatusResponseTypeDef(TypedDict):
    ConfigurationRecordersStatus: List[ConfigurationRecorderStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationRecorderStatusTypeDef](./type_defs.md#configurationrecorderstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConfigurationRecordersResponseTypeDef

```python
# ListConfigurationRecordersResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListConfigurationRecordersResponseTypeDef


def get_value() -> ListConfigurationRecordersResponseTypeDef:
    return {
        "ConfigurationRecorderSummaries": ...,
    }


# ListConfigurationRecordersResponseTypeDef definition

class ListConfigurationRecordersResponseTypeDef(TypedDict):
    ConfigurationRecorderSummaries: List[ConfigurationRecorderSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationRecorderSummaryTypeDef](./type_defs.md#configurationrecordersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConformancePackComplianceRequestTypeDef

```python
# DescribeConformancePackComplianceRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConformancePackComplianceRequestTypeDef


def get_value() -> DescribeConformancePackComplianceRequestTypeDef:
    return {
        "ConformancePackName": ...,
    }


# DescribeConformancePackComplianceRequestTypeDef definition

class DescribeConformancePackComplianceRequestTypeDef(TypedDict):
    ConformancePackName: str,
    Filters: NotRequired[ConformancePackComplianceFiltersTypeDef],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackComplianceFiltersTypeDef](./type_defs.md#conformancepackcompliancefilterstypedef) 
## ListConformancePackComplianceScoresResponseTypeDef

```python
# ListConformancePackComplianceScoresResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListConformancePackComplianceScoresResponseTypeDef


def get_value() -> ListConformancePackComplianceScoresResponseTypeDef:
    return {
        "NextToken": ...,
    }


# ListConformancePackComplianceScoresResponseTypeDef definition

class ListConformancePackComplianceScoresResponseTypeDef(TypedDict):
    ConformancePackComplianceScores: List[ConformancePackComplianceScoreTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackComplianceScoreTypeDef](./type_defs.md#conformancepackcompliancescoretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConformancePackComplianceScoresRequestTypeDef

```python
# ListConformancePackComplianceScoresRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListConformancePackComplianceScoresRequestTypeDef


def get_value() -> ListConformancePackComplianceScoresRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListConformancePackComplianceScoresRequestTypeDef definition

class ListConformancePackComplianceScoresRequestTypeDef(TypedDict):
    Filters: NotRequired[ConformancePackComplianceScoresFiltersTypeDef],  # (1)
    SortOrder: NotRequired[SortOrderType],  # (2)
    SortBy: NotRequired[SortByType],  # (3)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackComplianceScoresFiltersTypeDef](./type_defs.md#conformancepackcompliancescoresfilterstypedef) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SortByType](./literals.md#sortbytype) 
## GetConformancePackComplianceSummaryResponseTypeDef

```python
# GetConformancePackComplianceSummaryResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetConformancePackComplianceSummaryResponseTypeDef


def get_value() -> GetConformancePackComplianceSummaryResponseTypeDef:
    return {
        "ConformancePackComplianceSummaryList": ...,
    }


# GetConformancePackComplianceSummaryResponseTypeDef definition

class GetConformancePackComplianceSummaryResponseTypeDef(TypedDict):
    ConformancePackComplianceSummaryList: List[ConformancePackComplianceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackComplianceSummaryTypeDef](./type_defs.md#conformancepackcompliancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## OrganizationConformancePackTypeDef

```python
# OrganizationConformancePackTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationConformancePackTypeDef


def get_value() -> OrganizationConformancePackTypeDef:
    return {
        "OrganizationConformancePackName": ...,
    }


# OrganizationConformancePackTypeDef definition

class OrganizationConformancePackTypeDef(TypedDict):
    OrganizationConformancePackName: str,
    OrganizationConformancePackArn: str,
    LastUpdateTime: datetime,
    DeliveryS3Bucket: NotRequired[str],
    DeliveryS3KeyPrefix: NotRequired[str],
    ConformancePackInputParameters: NotRequired[List[ConformancePackInputParameterTypeDef]],  # (1)
    ExcludedAccounts: NotRequired[List[str]],
```

1. See [:material-code-braces: ConformancePackInputParameterTypeDef](./type_defs.md#conformancepackinputparametertypedef) 
## PutOrganizationConformancePackRequestTypeDef

```python
# PutOrganizationConformancePackRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutOrganizationConformancePackRequestTypeDef


def get_value() -> PutOrganizationConformancePackRequestTypeDef:
    return {
        "OrganizationConformancePackName": ...,
    }


# PutOrganizationConformancePackRequestTypeDef definition

class PutOrganizationConformancePackRequestTypeDef(TypedDict):
    OrganizationConformancePackName: str,
    TemplateS3Uri: NotRequired[str],
    TemplateBody: NotRequired[str],
    DeliveryS3Bucket: NotRequired[str],
    DeliveryS3KeyPrefix: NotRequired[str],
    ConformancePackInputParameters: NotRequired[Sequence[ConformancePackInputParameterTypeDef]],  # (1)
    ExcludedAccounts: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ConformancePackInputParameterTypeDef](./type_defs.md#conformancepackinputparametertypedef) 
## ConformancePackDetailTypeDef

```python
# ConformancePackDetailTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackDetailTypeDef


def get_value() -> ConformancePackDetailTypeDef:
    return {
        "ConformancePackName": ...,
    }


# ConformancePackDetailTypeDef definition

class ConformancePackDetailTypeDef(TypedDict):
    ConformancePackName: str,
    ConformancePackArn: str,
    ConformancePackId: str,
    DeliveryS3Bucket: NotRequired[str],
    DeliveryS3KeyPrefix: NotRequired[str],
    ConformancePackInputParameters: NotRequired[List[ConformancePackInputParameterTypeDef]],  # (1)
    LastUpdateRequestedTime: NotRequired[datetime],
    CreatedBy: NotRequired[str],
    TemplateSSMDocumentDetails: NotRequired[TemplateSSMDocumentDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: ConformancePackInputParameterTypeDef](./type_defs.md#conformancepackinputparametertypedef) 
2. See [:material-code-braces: TemplateSSMDocumentDetailsTypeDef](./type_defs.md#templatessmdocumentdetailstypedef) 
## PutConformancePackRequestTypeDef

```python
# PutConformancePackRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutConformancePackRequestTypeDef


def get_value() -> PutConformancePackRequestTypeDef:
    return {
        "ConformancePackName": ...,
    }


# PutConformancePackRequestTypeDef definition

class PutConformancePackRequestTypeDef(TypedDict):
    ConformancePackName: str,
    TemplateS3Uri: NotRequired[str],
    TemplateBody: NotRequired[str],
    DeliveryS3Bucket: NotRequired[str],
    DeliveryS3KeyPrefix: NotRequired[str],
    ConformancePackInputParameters: NotRequired[Sequence[ConformancePackInputParameterTypeDef]],  # (1)
    TemplateSSMDocumentDetails: NotRequired[TemplateSSMDocumentDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: ConformancePackInputParameterTypeDef](./type_defs.md#conformancepackinputparametertypedef) 
2. See [:material-code-braces: TemplateSSMDocumentDetailsTypeDef](./type_defs.md#templatessmdocumentdetailstypedef) 
## GetConformancePackComplianceDetailsRequestTypeDef

```python
# GetConformancePackComplianceDetailsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetConformancePackComplianceDetailsRequestTypeDef


def get_value() -> GetConformancePackComplianceDetailsRequestTypeDef:
    return {
        "ConformancePackName": ...,
    }


# GetConformancePackComplianceDetailsRequestTypeDef definition

class GetConformancePackComplianceDetailsRequestTypeDef(TypedDict):
    ConformancePackName: str,
    Filters: NotRequired[ConformancePackEvaluationFiltersTypeDef],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackEvaluationFiltersTypeDef](./type_defs.md#conformancepackevaluationfilterstypedef) 
## DescribeConformancePackComplianceResponseTypeDef

```python
# DescribeConformancePackComplianceResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConformancePackComplianceResponseTypeDef


def get_value() -> DescribeConformancePackComplianceResponseTypeDef:
    return {
        "ConformancePackName": ...,
    }


# DescribeConformancePackComplianceResponseTypeDef definition

class DescribeConformancePackComplianceResponseTypeDef(TypedDict):
    ConformancePackName: str,
    ConformancePackRuleComplianceList: List[ConformancePackRuleComplianceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackRuleComplianceTypeDef](./type_defs.md#conformancepackrulecompliancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConformancePackStatusResponseTypeDef

```python
# DescribeConformancePackStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConformancePackStatusResponseTypeDef


def get_value() -> DescribeConformancePackStatusResponseTypeDef:
    return {
        "ConformancePackStatusDetails": ...,
    }


# DescribeConformancePackStatusResponseTypeDef definition

class DescribeConformancePackStatusResponseTypeDef(TypedDict):
    ConformancePackStatusDetails: List[ConformancePackStatusDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackStatusDetailTypeDef](./type_defs.md#conformancepackstatusdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRemediationExceptionsRequestTypeDef

```python
# DeleteRemediationExceptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteRemediationExceptionsRequestTypeDef


def get_value() -> DeleteRemediationExceptionsRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# DeleteRemediationExceptionsRequestTypeDef definition

class DeleteRemediationExceptionsRequestTypeDef(TypedDict):
    ConfigRuleName: str,
    ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],  # (1)
```

1. See [:material-code-braces: RemediationExceptionResourceKeyTypeDef](./type_defs.md#remediationexceptionresourcekeytypedef) 
## DescribeRemediationExceptionsRequestTypeDef

```python
# DescribeRemediationExceptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRemediationExceptionsRequestTypeDef


def get_value() -> DescribeRemediationExceptionsRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# DescribeRemediationExceptionsRequestTypeDef definition

class DescribeRemediationExceptionsRequestTypeDef(TypedDict):
    ConfigRuleName: str,
    ResourceKeys: NotRequired[Sequence[RemediationExceptionResourceKeyTypeDef]],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RemediationExceptionResourceKeyTypeDef](./type_defs.md#remediationexceptionresourcekeytypedef) 
## FailedDeleteRemediationExceptionsBatchTypeDef

```python
# FailedDeleteRemediationExceptionsBatchTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import FailedDeleteRemediationExceptionsBatchTypeDef


def get_value() -> FailedDeleteRemediationExceptionsBatchTypeDef:
    return {
        "FailureMessage": ...,
    }


# FailedDeleteRemediationExceptionsBatchTypeDef definition

class FailedDeleteRemediationExceptionsBatchTypeDef(TypedDict):
    FailureMessage: NotRequired[str],
    FailedItems: NotRequired[List[RemediationExceptionResourceKeyTypeDef]],  # (1)
```

1. See [:material-code-braces: RemediationExceptionResourceKeyTypeDef](./type_defs.md#remediationexceptionresourcekeytypedef) 
## DescribeAggregateComplianceByConfigRulesRequestPaginateTypeDef

```python
# DescribeAggregateComplianceByConfigRulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregateComplianceByConfigRulesRequestPaginateTypeDef


def get_value() -> DescribeAggregateComplianceByConfigRulesRequestPaginateTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# DescribeAggregateComplianceByConfigRulesRequestPaginateTypeDef definition

class DescribeAggregateComplianceByConfigRulesRequestPaginateTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    Filters: NotRequired[ConfigRuleComplianceFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ConfigRuleComplianceFiltersTypeDef](./type_defs.md#configrulecompliancefilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAggregateComplianceByConformancePacksRequestPaginateTypeDef

```python
# DescribeAggregateComplianceByConformancePacksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregateComplianceByConformancePacksRequestPaginateTypeDef


def get_value() -> DescribeAggregateComplianceByConformancePacksRequestPaginateTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# DescribeAggregateComplianceByConformancePacksRequestPaginateTypeDef definition

class DescribeAggregateComplianceByConformancePacksRequestPaginateTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    Filters: NotRequired[AggregateConformancePackComplianceFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AggregateConformancePackComplianceFiltersTypeDef](./type_defs.md#aggregateconformancepackcompliancefilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeAggregationAuthorizationsRequestPaginateTypeDef

```python
# DescribeAggregationAuthorizationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregationAuthorizationsRequestPaginateTypeDef


def get_value() -> DescribeAggregationAuthorizationsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# DescribeAggregationAuthorizationsRequestPaginateTypeDef definition

class DescribeAggregationAuthorizationsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeComplianceByConfigRuleRequestPaginateTypeDef

```python
# DescribeComplianceByConfigRuleRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeComplianceByConfigRuleRequestPaginateTypeDef


def get_value() -> DescribeComplianceByConfigRuleRequestPaginateTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# DescribeComplianceByConfigRuleRequestPaginateTypeDef definition

class DescribeComplianceByConfigRuleRequestPaginateTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
    ComplianceTypes: NotRequired[Sequence[ComplianceTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeComplianceByResourceRequestPaginateTypeDef

```python
# DescribeComplianceByResourceRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeComplianceByResourceRequestPaginateTypeDef


def get_value() -> DescribeComplianceByResourceRequestPaginateTypeDef:
    return {
        "ResourceType": ...,
    }


# DescribeComplianceByResourceRequestPaginateTypeDef definition

class DescribeComplianceByResourceRequestPaginateTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    ComplianceTypes: NotRequired[Sequence[ComplianceTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConfigRuleEvaluationStatusRequestPaginateTypeDef

```python
# DescribeConfigRuleEvaluationStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigRuleEvaluationStatusRequestPaginateTypeDef


def get_value() -> DescribeConfigRuleEvaluationStatusRequestPaginateTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# DescribeConfigRuleEvaluationStatusRequestPaginateTypeDef definition

class DescribeConfigRuleEvaluationStatusRequestPaginateTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConfigurationAggregatorSourcesStatusRequestPaginateTypeDef

```python
# DescribeConfigurationAggregatorSourcesStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationAggregatorSourcesStatusRequestPaginateTypeDef


def get_value() -> DescribeConfigurationAggregatorSourcesStatusRequestPaginateTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# DescribeConfigurationAggregatorSourcesStatusRequestPaginateTypeDef definition

class DescribeConfigurationAggregatorSourcesStatusRequestPaginateTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    UpdateStatus: NotRequired[Sequence[AggregatedSourceStatusTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: AggregatedSourceStatusTypeType](./literals.md#aggregatedsourcestatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConfigurationAggregatorsRequestPaginateTypeDef

```python
# DescribeConfigurationAggregatorsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationAggregatorsRequestPaginateTypeDef


def get_value() -> DescribeConfigurationAggregatorsRequestPaginateTypeDef:
    return {
        "ConfigurationAggregatorNames": ...,
    }


# DescribeConfigurationAggregatorsRequestPaginateTypeDef definition

class DescribeConfigurationAggregatorsRequestPaginateTypeDef(TypedDict):
    ConfigurationAggregatorNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConformancePackStatusRequestPaginateTypeDef

```python
# DescribeConformancePackStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConformancePackStatusRequestPaginateTypeDef


def get_value() -> DescribeConformancePackStatusRequestPaginateTypeDef:
    return {
        "ConformancePackNames": ...,
    }


# DescribeConformancePackStatusRequestPaginateTypeDef definition

class DescribeConformancePackStatusRequestPaginateTypeDef(TypedDict):
    ConformancePackNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConformancePacksRequestPaginateTypeDef

```python
# DescribeConformancePacksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConformancePacksRequestPaginateTypeDef


def get_value() -> DescribeConformancePacksRequestPaginateTypeDef:
    return {
        "ConformancePackNames": ...,
    }


# DescribeConformancePacksRequestPaginateTypeDef definition

class DescribeConformancePacksRequestPaginateTypeDef(TypedDict):
    ConformancePackNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOrganizationConfigRuleStatusesRequestPaginateTypeDef

```python
# DescribeOrganizationConfigRuleStatusesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConfigRuleStatusesRequestPaginateTypeDef


def get_value() -> DescribeOrganizationConfigRuleStatusesRequestPaginateTypeDef:
    return {
        "OrganizationConfigRuleNames": ...,
    }


# DescribeOrganizationConfigRuleStatusesRequestPaginateTypeDef definition

class DescribeOrganizationConfigRuleStatusesRequestPaginateTypeDef(TypedDict):
    OrganizationConfigRuleNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOrganizationConfigRulesRequestPaginateTypeDef

```python
# DescribeOrganizationConfigRulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConfigRulesRequestPaginateTypeDef


def get_value() -> DescribeOrganizationConfigRulesRequestPaginateTypeDef:
    return {
        "OrganizationConfigRuleNames": ...,
    }


# DescribeOrganizationConfigRulesRequestPaginateTypeDef definition

class DescribeOrganizationConfigRulesRequestPaginateTypeDef(TypedDict):
    OrganizationConfigRuleNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOrganizationConformancePackStatusesRequestPaginateTypeDef

```python
# DescribeOrganizationConformancePackStatusesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConformancePackStatusesRequestPaginateTypeDef


def get_value() -> DescribeOrganizationConformancePackStatusesRequestPaginateTypeDef:
    return {
        "OrganizationConformancePackNames": ...,
    }


# DescribeOrganizationConformancePackStatusesRequestPaginateTypeDef definition

class DescribeOrganizationConformancePackStatusesRequestPaginateTypeDef(TypedDict):
    OrganizationConformancePackNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeOrganizationConformancePacksRequestPaginateTypeDef

```python
# DescribeOrganizationConformancePacksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConformancePacksRequestPaginateTypeDef


def get_value() -> DescribeOrganizationConformancePacksRequestPaginateTypeDef:
    return {
        "OrganizationConformancePackNames": ...,
    }


# DescribeOrganizationConformancePacksRequestPaginateTypeDef definition

class DescribeOrganizationConformancePacksRequestPaginateTypeDef(TypedDict):
    OrganizationConformancePackNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribePendingAggregationRequestsRequestPaginateTypeDef

```python
# DescribePendingAggregationRequestsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribePendingAggregationRequestsRequestPaginateTypeDef


def get_value() -> DescribePendingAggregationRequestsRequestPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# DescribePendingAggregationRequestsRequestPaginateTypeDef definition

class DescribePendingAggregationRequestsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRemediationExecutionStatusRequestPaginateTypeDef

```python
# DescribeRemediationExecutionStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRemediationExecutionStatusRequestPaginateTypeDef


def get_value() -> DescribeRemediationExecutionStatusRequestPaginateTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# DescribeRemediationExecutionStatusRequestPaginateTypeDef definition

class DescribeRemediationExecutionStatusRequestPaginateTypeDef(TypedDict):
    ConfigRuleName: str,
    ResourceKeys: NotRequired[Sequence[ResourceKeyTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeRetentionConfigurationsRequestPaginateTypeDef

```python
# DescribeRetentionConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRetentionConfigurationsRequestPaginateTypeDef


def get_value() -> DescribeRetentionConfigurationsRequestPaginateTypeDef:
    return {
        "RetentionConfigurationNames": ...,
    }


# DescribeRetentionConfigurationsRequestPaginateTypeDef definition

class DescribeRetentionConfigurationsRequestPaginateTypeDef(TypedDict):
    RetentionConfigurationNames: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetAggregateComplianceDetailsByConfigRuleRequestPaginateTypeDef

```python
# GetAggregateComplianceDetailsByConfigRuleRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateComplianceDetailsByConfigRuleRequestPaginateTypeDef


def get_value() -> GetAggregateComplianceDetailsByConfigRuleRequestPaginateTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# GetAggregateComplianceDetailsByConfigRuleRequestPaginateTypeDef definition

class GetAggregateComplianceDetailsByConfigRuleRequestPaginateTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    ConfigRuleName: str,
    AccountId: str,
    AwsRegion: str,
    ComplianceType: NotRequired[ComplianceTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetComplianceDetailsByConfigRuleRequestPaginateTypeDef

```python
# GetComplianceDetailsByConfigRuleRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceDetailsByConfigRuleRequestPaginateTypeDef


def get_value() -> GetComplianceDetailsByConfigRuleRequestPaginateTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# GetComplianceDetailsByConfigRuleRequestPaginateTypeDef definition

class GetComplianceDetailsByConfigRuleRequestPaginateTypeDef(TypedDict):
    ConfigRuleName: str,
    ComplianceTypes: NotRequired[Sequence[ComplianceTypeType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetComplianceDetailsByResourceRequestPaginateTypeDef

```python
# GetComplianceDetailsByResourceRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceDetailsByResourceRequestPaginateTypeDef


def get_value() -> GetComplianceDetailsByResourceRequestPaginateTypeDef:
    return {
        "ResourceType": ...,
    }


# GetComplianceDetailsByResourceRequestPaginateTypeDef definition

class GetComplianceDetailsByResourceRequestPaginateTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    ComplianceTypes: NotRequired[Sequence[ComplianceTypeType]],  # (1)
    ResourceEvaluationId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetConformancePackComplianceSummaryRequestPaginateTypeDef

```python
# GetConformancePackComplianceSummaryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetConformancePackComplianceSummaryRequestPaginateTypeDef


def get_value() -> GetConformancePackComplianceSummaryRequestPaginateTypeDef:
    return {
        "ConformancePackNames": ...,
    }


# GetConformancePackComplianceSummaryRequestPaginateTypeDef definition

class GetConformancePackComplianceSummaryRequestPaginateTypeDef(TypedDict):
    ConformancePackNames: Sequence[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConfigurationRecordersRequestPaginateTypeDef

```python
# ListConfigurationRecordersRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListConfigurationRecordersRequestPaginateTypeDef


def get_value() -> ListConfigurationRecordersRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListConfigurationRecordersRequestPaginateTypeDef definition

class ListConfigurationRecordersRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[ConfigurationRecorderFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ConfigurationRecorderFilterTypeDef](./type_defs.md#configurationrecorderfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDiscoveredResourcesRequestPaginateTypeDef

```python
# ListDiscoveredResourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListDiscoveredResourcesRequestPaginateTypeDef


def get_value() -> ListDiscoveredResourcesRequestPaginateTypeDef:
    return {
        "resourceType": ...,
    }


# ListDiscoveredResourcesRequestPaginateTypeDef definition

class ListDiscoveredResourcesRequestPaginateTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    resourceIds: NotRequired[Sequence[str]],
    resourceName: NotRequired[str],
    includeDeletedResources: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceRequestPaginateTypeDef

```python
# ListTagsForResourceRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListTagsForResourceRequestPaginateTypeDef


def get_value() -> ListTagsForResourceRequestPaginateTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestPaginateTypeDef definition

class ListTagsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SelectAggregateResourceConfigRequestPaginateTypeDef

```python
# SelectAggregateResourceConfigRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SelectAggregateResourceConfigRequestPaginateTypeDef


def get_value() -> SelectAggregateResourceConfigRequestPaginateTypeDef:
    return {
        "Expression": ...,
    }


# SelectAggregateResourceConfigRequestPaginateTypeDef definition

class SelectAggregateResourceConfigRequestPaginateTypeDef(TypedDict):
    Expression: str,
    ConfigurationAggregatorName: str,
    MaxResults: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SelectResourceConfigRequestPaginateTypeDef

```python
# SelectResourceConfigRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SelectResourceConfigRequestPaginateTypeDef


def get_value() -> SelectResourceConfigRequestPaginateTypeDef:
    return {
        "Expression": ...,
    }


# SelectResourceConfigRequestPaginateTypeDef definition

class SelectResourceConfigRequestPaginateTypeDef(TypedDict):
    Expression: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConfigRulesRequestPaginateTypeDef

```python
# DescribeConfigRulesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigRulesRequestPaginateTypeDef


def get_value() -> DescribeConfigRulesRequestPaginateTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# DescribeConfigRulesRequestPaginateTypeDef definition

class DescribeConfigRulesRequestPaginateTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
    Filters: NotRequired[DescribeConfigRulesFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DescribeConfigRulesFiltersTypeDef](./type_defs.md#describeconfigrulesfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## DescribeConfigRulesRequestTypeDef

```python
# DescribeConfigRulesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigRulesRequestTypeDef


def get_value() -> DescribeConfigRulesRequestTypeDef:
    return {
        "ConfigRuleNames": ...,
    }


# DescribeConfigRulesRequestTypeDef definition

class DescribeConfigRulesRequestTypeDef(TypedDict):
    ConfigRuleNames: NotRequired[Sequence[str]],
    NextToken: NotRequired[str],
    Filters: NotRequired[DescribeConfigRulesFiltersTypeDef],  # (1)
```

1. See [:material-code-braces: DescribeConfigRulesFiltersTypeDef](./type_defs.md#describeconfigrulesfilterstypedef) 
## DescribeOrganizationConfigRuleStatusesResponseTypeDef

```python
# DescribeOrganizationConfigRuleStatusesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConfigRuleStatusesResponseTypeDef


def get_value() -> DescribeOrganizationConfigRuleStatusesResponseTypeDef:
    return {
        "OrganizationConfigRuleStatuses": ...,
    }


# DescribeOrganizationConfigRuleStatusesResponseTypeDef definition

class DescribeOrganizationConfigRuleStatusesResponseTypeDef(TypedDict):
    OrganizationConfigRuleStatuses: List[OrganizationConfigRuleStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationConfigRuleStatusTypeDef](./type_defs.md#organizationconfigrulestatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationConformancePackStatusesResponseTypeDef

```python
# DescribeOrganizationConformancePackStatusesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConformancePackStatusesResponseTypeDef


def get_value() -> DescribeOrganizationConformancePackStatusesResponseTypeDef:
    return {
        "OrganizationConformancePackStatuses": ...,
    }


# DescribeOrganizationConformancePackStatusesResponseTypeDef definition

class DescribeOrganizationConformancePackStatusesResponseTypeDef(TypedDict):
    OrganizationConformancePackStatuses: List[OrganizationConformancePackStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationConformancePackStatusTypeDef](./type_defs.md#organizationconformancepackstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePendingAggregationRequestsResponseTypeDef

```python
# DescribePendingAggregationRequestsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribePendingAggregationRequestsResponseTypeDef


def get_value() -> DescribePendingAggregationRequestsResponseTypeDef:
    return {
        "PendingAggregationRequests": ...,
    }


# DescribePendingAggregationRequestsResponseTypeDef definition

class DescribePendingAggregationRequestsResponseTypeDef(TypedDict):
    PendingAggregationRequests: List[PendingAggregationRequestTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PendingAggregationRequestTypeDef](./type_defs.md#pendingaggregationrequesttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRemediationExceptionsResponseTypeDef

```python
# DescribeRemediationExceptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRemediationExceptionsResponseTypeDef


def get_value() -> DescribeRemediationExceptionsResponseTypeDef:
    return {
        "RemediationExceptions": ...,
    }


# DescribeRemediationExceptionsResponseTypeDef definition

class DescribeRemediationExceptionsResponseTypeDef(TypedDict):
    RemediationExceptions: List[RemediationExceptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RemediationExceptionTypeDef](./type_defs.md#remediationexceptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailedRemediationExceptionBatchTypeDef

```python
# FailedRemediationExceptionBatchTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import FailedRemediationExceptionBatchTypeDef


def get_value() -> FailedRemediationExceptionBatchTypeDef:
    return {
        "FailureMessage": ...,
    }


# FailedRemediationExceptionBatchTypeDef definition

class FailedRemediationExceptionBatchTypeDef(TypedDict):
    FailureMessage: NotRequired[str],
    FailedItems: NotRequired[List[RemediationExceptionTypeDef]],  # (1)
```

1. See [:material-code-braces: RemediationExceptionTypeDef](./type_defs.md#remediationexceptiontypedef) 
## DescribeRetentionConfigurationsResponseTypeDef

```python
# DescribeRetentionConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRetentionConfigurationsResponseTypeDef


def get_value() -> DescribeRetentionConfigurationsResponseTypeDef:
    return {
        "RetentionConfigurations": ...,
    }


# DescribeRetentionConfigurationsResponseTypeDef definition

class DescribeRetentionConfigurationsResponseTypeDef(TypedDict):
    RetentionConfigurations: List[RetentionConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RetentionConfigurationTypeDef](./type_defs.md#retentionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRetentionConfigurationResponseTypeDef

```python
# PutRetentionConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutRetentionConfigurationResponseTypeDef


def get_value() -> PutRetentionConfigurationResponseTypeDef:
    return {
        "RetentionConfiguration": ...,
    }


# PutRetentionConfigurationResponseTypeDef definition

class PutRetentionConfigurationResponseTypeDef(TypedDict):
    RetentionConfiguration: RetentionConfigurationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RetentionConfigurationTypeDef](./type_defs.md#retentionconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEvaluationsResponseTypeDef

```python
# PutEvaluationsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutEvaluationsResponseTypeDef


def get_value() -> PutEvaluationsResponseTypeDef:
    return {
        "FailedEvaluations": ...,
    }


# PutEvaluationsResponseTypeDef definition

class PutEvaluationsResponseTypeDef(TypedDict):
    FailedEvaluations: List[EvaluationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EvaluationOutputTypeDef](./type_defs.md#evaluationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EvaluationResultIdentifierTypeDef

```python
# EvaluationResultIdentifierTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EvaluationResultIdentifierTypeDef


def get_value() -> EvaluationResultIdentifierTypeDef:
    return {
        "EvaluationResultQualifier": ...,
    }


# EvaluationResultIdentifierTypeDef definition

class EvaluationResultIdentifierTypeDef(TypedDict):
    EvaluationResultQualifier: NotRequired[EvaluationResultQualifierTypeDef],  # (1)
    OrderingTimestamp: NotRequired[datetime],
    ResourceEvaluationId: NotRequired[str],
```

1. See [:material-code-braces: EvaluationResultQualifierTypeDef](./type_defs.md#evaluationresultqualifiertypedef) 
## EvaluationTypeDef

```python
# EvaluationTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EvaluationTypeDef


def get_value() -> EvaluationTypeDef:
    return {
        "ComplianceResourceType": ...,
    }


# EvaluationTypeDef definition

class EvaluationTypeDef(TypedDict):
    ComplianceResourceType: str,
    ComplianceResourceId: str,
    ComplianceType: ComplianceTypeType,  # (1)
    OrderingTimestamp: TimestampTypeDef,
    Annotation: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## ExternalEvaluationTypeDef

```python
# ExternalEvaluationTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ExternalEvaluationTypeDef


def get_value() -> ExternalEvaluationTypeDef:
    return {
        "ComplianceResourceType": ...,
    }


# ExternalEvaluationTypeDef definition

class ExternalEvaluationTypeDef(TypedDict):
    ComplianceResourceType: str,
    ComplianceResourceId: str,
    ComplianceType: ComplianceTypeType,  # (1)
    OrderingTimestamp: TimestampTypeDef,
    Annotation: NotRequired[str],
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## GetResourceConfigHistoryRequestPaginateTypeDef

```python
# GetResourceConfigHistoryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetResourceConfigHistoryRequestPaginateTypeDef


def get_value() -> GetResourceConfigHistoryRequestPaginateTypeDef:
    return {
        "resourceType": ...,
    }


# GetResourceConfigHistoryRequestPaginateTypeDef definition

class GetResourceConfigHistoryRequestPaginateTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    resourceId: str,
    laterTime: NotRequired[TimestampTypeDef],
    earlierTime: NotRequired[TimestampTypeDef],
    chronologicalOrder: NotRequired[ChronologicalOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ChronologicalOrderType](./literals.md#chronologicalordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourceConfigHistoryRequestTypeDef

```python
# GetResourceConfigHistoryRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetResourceConfigHistoryRequestTypeDef


def get_value() -> GetResourceConfigHistoryRequestTypeDef:
    return {
        "resourceType": ...,
    }


# GetResourceConfigHistoryRequestTypeDef definition

class GetResourceConfigHistoryRequestTypeDef(TypedDict):
    resourceType: ResourceTypeType,  # (1)
    resourceId: str,
    laterTime: NotRequired[TimestampTypeDef],
    earlierTime: NotRequired[TimestampTypeDef],
    chronologicalOrder: NotRequired[ChronologicalOrderType],  # (2)
    limit: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ChronologicalOrderType](./literals.md#chronologicalordertype) 
## PutRemediationExceptionsRequestTypeDef

```python
# PutRemediationExceptionsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutRemediationExceptionsRequestTypeDef


def get_value() -> PutRemediationExceptionsRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# PutRemediationExceptionsRequestTypeDef definition

class PutRemediationExceptionsRequestTypeDef(TypedDict):
    ConfigRuleName: str,
    ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],  # (1)
    Message: NotRequired[str],
    ExpirationTime: NotRequired[TimestampTypeDef],
```

1. See [:material-code-braces: RemediationExceptionResourceKeyTypeDef](./type_defs.md#remediationexceptionresourcekeytypedef) 
## TimeWindowTypeDef

```python
# TimeWindowTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import TimeWindowTypeDef


def get_value() -> TimeWindowTypeDef:
    return {
        "StartTime": ...,
    }


# TimeWindowTypeDef definition

class TimeWindowTypeDef(TypedDict):
    StartTime: NotRequired[TimestampTypeDef],
    EndTime: NotRequired[TimestampTypeDef],
```

## ExecutionControlsTypeDef

```python
# ExecutionControlsTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ExecutionControlsTypeDef


def get_value() -> ExecutionControlsTypeDef:
    return {
        "SsmControls": ...,
    }


# ExecutionControlsTypeDef definition

class ExecutionControlsTypeDef(TypedDict):
    SsmControls: NotRequired[SsmControlsTypeDef],  # (1)
```

1. See [:material-code-braces: SsmControlsTypeDef](./type_defs.md#ssmcontrolstypedef) 
## QueryInfoTypeDef

```python
# QueryInfoTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import QueryInfoTypeDef


def get_value() -> QueryInfoTypeDef:
    return {
        "SelectFields": ...,
    }


# QueryInfoTypeDef definition

class QueryInfoTypeDef(TypedDict):
    SelectFields: NotRequired[List[FieldInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: FieldInfoTypeDef](./type_defs.md#fieldinfotypedef) 
## GetAggregateDiscoveredResourceCountsRequestTypeDef

```python
# GetAggregateDiscoveredResourceCountsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateDiscoveredResourceCountsRequestTypeDef


def get_value() -> GetAggregateDiscoveredResourceCountsRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# GetAggregateDiscoveredResourceCountsRequestTypeDef definition

class GetAggregateDiscoveredResourceCountsRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    Filters: NotRequired[ResourceCountFiltersTypeDef],  # (1)
    GroupByKey: NotRequired[ResourceCountGroupKeyType],  # (2)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceCountFiltersTypeDef](./type_defs.md#resourcecountfilterstypedef) 
2. See [:material-code-brackets: ResourceCountGroupKeyType](./literals.md#resourcecountgroupkeytype) 
## GetAggregateDiscoveredResourceCountsResponseTypeDef

```python
# GetAggregateDiscoveredResourceCountsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateDiscoveredResourceCountsResponseTypeDef


def get_value() -> GetAggregateDiscoveredResourceCountsResponseTypeDef:
    return {
        "TotalDiscoveredResources": ...,
    }


# GetAggregateDiscoveredResourceCountsResponseTypeDef definition

class GetAggregateDiscoveredResourceCountsResponseTypeDef(TypedDict):
    TotalDiscoveredResources: int,
    GroupByKey: str,
    GroupedResourceCounts: List[GroupedResourceCountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupedResourceCountTypeDef](./type_defs.md#groupedresourcecounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDiscoveredResourceCountsResponseTypeDef

```python
# GetDiscoveredResourceCountsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetDiscoveredResourceCountsResponseTypeDef


def get_value() -> GetDiscoveredResourceCountsResponseTypeDef:
    return {
        "totalDiscoveredResources": ...,
    }


# GetDiscoveredResourceCountsResponseTypeDef definition

class GetDiscoveredResourceCountsResponseTypeDef(TypedDict):
    totalDiscoveredResources: int,
    resourceCounts: List[ResourceCountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceCountTypeDef](./type_defs.md#resourcecounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOrganizationConfigRuleDetailedStatusRequestPaginateTypeDef

```python
# GetOrganizationConfigRuleDetailedStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetOrganizationConfigRuleDetailedStatusRequestPaginateTypeDef


def get_value() -> GetOrganizationConfigRuleDetailedStatusRequestPaginateTypeDef:
    return {
        "OrganizationConfigRuleName": ...,
    }


# GetOrganizationConfigRuleDetailedStatusRequestPaginateTypeDef definition

class GetOrganizationConfigRuleDetailedStatusRequestPaginateTypeDef(TypedDict):
    OrganizationConfigRuleName: str,
    Filters: NotRequired[StatusDetailFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: StatusDetailFiltersTypeDef](./type_defs.md#statusdetailfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetOrganizationConfigRuleDetailedStatusRequestTypeDef

```python
# GetOrganizationConfigRuleDetailedStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetOrganizationConfigRuleDetailedStatusRequestTypeDef


def get_value() -> GetOrganizationConfigRuleDetailedStatusRequestTypeDef:
    return {
        "OrganizationConfigRuleName": ...,
    }


# GetOrganizationConfigRuleDetailedStatusRequestTypeDef definition

class GetOrganizationConfigRuleDetailedStatusRequestTypeDef(TypedDict):
    OrganizationConfigRuleName: str,
    Filters: NotRequired[StatusDetailFiltersTypeDef],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StatusDetailFiltersTypeDef](./type_defs.md#statusdetailfilterstypedef) 
## GetOrganizationConfigRuleDetailedStatusResponseTypeDef

```python
# GetOrganizationConfigRuleDetailedStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetOrganizationConfigRuleDetailedStatusResponseTypeDef


def get_value() -> GetOrganizationConfigRuleDetailedStatusResponseTypeDef:
    return {
        "OrganizationConfigRuleDetailedStatus": ...,
    }


# GetOrganizationConfigRuleDetailedStatusResponseTypeDef definition

class GetOrganizationConfigRuleDetailedStatusResponseTypeDef(TypedDict):
    OrganizationConfigRuleDetailedStatus: List[MemberAccountStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MemberAccountStatusTypeDef](./type_defs.md#memberaccountstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOrganizationConformancePackDetailedStatusRequestPaginateTypeDef

```python
# GetOrganizationConformancePackDetailedStatusRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetOrganizationConformancePackDetailedStatusRequestPaginateTypeDef


def get_value() -> GetOrganizationConformancePackDetailedStatusRequestPaginateTypeDef:
    return {
        "OrganizationConformancePackName": ...,
    }


# GetOrganizationConformancePackDetailedStatusRequestPaginateTypeDef definition

class GetOrganizationConformancePackDetailedStatusRequestPaginateTypeDef(TypedDict):
    OrganizationConformancePackName: str,
    Filters: NotRequired[OrganizationResourceDetailedStatusFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: OrganizationResourceDetailedStatusFiltersTypeDef](./type_defs.md#organizationresourcedetailedstatusfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetOrganizationConformancePackDetailedStatusRequestTypeDef

```python
# GetOrganizationConformancePackDetailedStatusRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetOrganizationConformancePackDetailedStatusRequestTypeDef


def get_value() -> GetOrganizationConformancePackDetailedStatusRequestTypeDef:
    return {
        "OrganizationConformancePackName": ...,
    }


# GetOrganizationConformancePackDetailedStatusRequestTypeDef definition

class GetOrganizationConformancePackDetailedStatusRequestTypeDef(TypedDict):
    OrganizationConformancePackName: str,
    Filters: NotRequired[OrganizationResourceDetailedStatusFiltersTypeDef],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationResourceDetailedStatusFiltersTypeDef](./type_defs.md#organizationresourcedetailedstatusfilterstypedef) 
## GetOrganizationConformancePackDetailedStatusResponseTypeDef

```python
# GetOrganizationConformancePackDetailedStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetOrganizationConformancePackDetailedStatusResponseTypeDef


def get_value() -> GetOrganizationConformancePackDetailedStatusResponseTypeDef:
    return {
        "OrganizationConformancePackDetailedStatuses": ...,
    }


# GetOrganizationConformancePackDetailedStatusResponseTypeDef definition

class GetOrganizationConformancePackDetailedStatusResponseTypeDef(TypedDict):
    OrganizationConformancePackDetailedStatuses: List[OrganizationConformancePackDetailedStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationConformancePackDetailedStatusTypeDef](./type_defs.md#organizationconformancepackdetailedstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceEvaluationSummaryResponseTypeDef

```python
# GetResourceEvaluationSummaryResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetResourceEvaluationSummaryResponseTypeDef


def get_value() -> GetResourceEvaluationSummaryResponseTypeDef:
    return {
        "ResourceEvaluationId": ...,
    }


# GetResourceEvaluationSummaryResponseTypeDef definition

class GetResourceEvaluationSummaryResponseTypeDef(TypedDict):
    ResourceEvaluationId: str,
    EvaluationMode: EvaluationModeType,  # (1)
    EvaluationStatus: EvaluationStatusTypeDef,  # (2)
    EvaluationStartTimestamp: datetime,
    Compliance: ComplianceTypeType,  # (3)
    EvaluationContext: EvaluationContextTypeDef,  # (4)
    ResourceDetails: ResourceDetailsTypeDef,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: EvaluationModeType](./literals.md#evaluationmodetype) 
2. See [:material-code-braces: EvaluationStatusTypeDef](./type_defs.md#evaluationstatustypedef) 
3. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
4. See [:material-code-braces: EvaluationContextTypeDef](./type_defs.md#evaluationcontexttypedef) 
5. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartResourceEvaluationRequestTypeDef

```python
# StartResourceEvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import StartResourceEvaluationRequestTypeDef


def get_value() -> StartResourceEvaluationRequestTypeDef:
    return {
        "ResourceDetails": ...,
    }


# StartResourceEvaluationRequestTypeDef definition

class StartResourceEvaluationRequestTypeDef(TypedDict):
    ResourceDetails: ResourceDetailsTypeDef,  # (1)
    EvaluationMode: EvaluationModeType,  # (2)
    EvaluationContext: NotRequired[EvaluationContextTypeDef],  # (3)
    EvaluationTimeout: NotRequired[int],
    ClientToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceDetailsTypeDef](./type_defs.md#resourcedetailstypedef) 
2. See [:material-code-brackets: EvaluationModeType](./literals.md#evaluationmodetype) 
3. See [:material-code-braces: EvaluationContextTypeDef](./type_defs.md#evaluationcontexttypedef) 
## GetStoredQueryResponseTypeDef

```python
# GetStoredQueryResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetStoredQueryResponseTypeDef


def get_value() -> GetStoredQueryResponseTypeDef:
    return {
        "StoredQuery": ...,
    }


# GetStoredQueryResponseTypeDef definition

class GetStoredQueryResponseTypeDef(TypedDict):
    StoredQuery: StoredQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StoredQueryTypeDef](./type_defs.md#storedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAggregateDiscoveredResourcesRequestPaginateTypeDef

```python
# ListAggregateDiscoveredResourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListAggregateDiscoveredResourcesRequestPaginateTypeDef


def get_value() -> ListAggregateDiscoveredResourcesRequestPaginateTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# ListAggregateDiscoveredResourcesRequestPaginateTypeDef definition

class ListAggregateDiscoveredResourcesRequestPaginateTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    ResourceType: ResourceTypeType,  # (1)
    Filters: NotRequired[ResourceFiltersTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceFiltersTypeDef](./type_defs.md#resourcefilterstypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAggregateDiscoveredResourcesRequestTypeDef

```python
# ListAggregateDiscoveredResourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListAggregateDiscoveredResourcesRequestTypeDef


def get_value() -> ListAggregateDiscoveredResourcesRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# ListAggregateDiscoveredResourcesRequestTypeDef definition

class ListAggregateDiscoveredResourcesRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    ResourceType: ResourceTypeType,  # (1)
    Filters: NotRequired[ResourceFiltersTypeDef],  # (2)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceFiltersTypeDef](./type_defs.md#resourcefilterstypedef) 
## ListDiscoveredResourcesResponseTypeDef

```python
# ListDiscoveredResourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListDiscoveredResourcesResponseTypeDef


def get_value() -> ListDiscoveredResourcesResponseTypeDef:
    return {
        "resourceIdentifiers": ...,
    }


# ListDiscoveredResourcesResponseTypeDef definition

class ListDiscoveredResourcesResponseTypeDef(TypedDict):
    resourceIdentifiers: List[ResourceIdentifierTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceIdentifierTypeDef](./type_defs.md#resourceidentifiertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceEvaluationsResponseTypeDef

```python
# ListResourceEvaluationsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListResourceEvaluationsResponseTypeDef


def get_value() -> ListResourceEvaluationsResponseTypeDef:
    return {
        "ResourceEvaluations": ...,
    }


# ListResourceEvaluationsResponseTypeDef definition

class ListResourceEvaluationsResponseTypeDef(TypedDict):
    ResourceEvaluations: List[ResourceEvaluationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceEvaluationTypeDef](./type_defs.md#resourceevaluationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListStoredQueriesResponseTypeDef

```python
# ListStoredQueriesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListStoredQueriesResponseTypeDef


def get_value() -> ListStoredQueriesResponseTypeDef:
    return {
        "StoredQueryMetadata": ...,
    }


# ListStoredQueriesResponseTypeDef definition

class ListStoredQueriesResponseTypeDef(TypedDict):
    StoredQueryMetadata: List[StoredQueryMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: StoredQueryMetadataTypeDef](./type_defs.md#storedquerymetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutAggregationAuthorizationRequestTypeDef

```python
# PutAggregationAuthorizationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutAggregationAuthorizationRequestTypeDef


def get_value() -> PutAggregationAuthorizationRequestTypeDef:
    return {
        "AuthorizedAccountId": ...,
    }


# PutAggregationAuthorizationRequestTypeDef definition

class PutAggregationAuthorizationRequestTypeDef(TypedDict):
    AuthorizedAccountId: str,
    AuthorizedAwsRegion: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutServiceLinkedConfigurationRecorderRequestTypeDef

```python
# PutServiceLinkedConfigurationRecorderRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutServiceLinkedConfigurationRecorderRequestTypeDef


def get_value() -> PutServiceLinkedConfigurationRecorderRequestTypeDef:
    return {
        "ServicePrincipal": ...,
    }


# PutServiceLinkedConfigurationRecorderRequestTypeDef definition

class PutServiceLinkedConfigurationRecorderRequestTypeDef(TypedDict):
    ServicePrincipal: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutStoredQueryRequestTypeDef

```python
# PutStoredQueryRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutStoredQueryRequestTypeDef


def get_value() -> PutStoredQueryRequestTypeDef:
    return {
        "StoredQuery": ...,
    }


# PutStoredQueryRequestTypeDef definition

class PutStoredQueryRequestTypeDef(TypedDict):
    StoredQuery: StoredQueryTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: StoredQueryTypeDef](./type_defs.md#storedquerytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## OrganizationConfigRuleTypeDef

```python
# OrganizationConfigRuleTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import OrganizationConfigRuleTypeDef


def get_value() -> OrganizationConfigRuleTypeDef:
    return {
        "OrganizationConfigRuleName": ...,
    }


# OrganizationConfigRuleTypeDef definition

class OrganizationConfigRuleTypeDef(TypedDict):
    OrganizationConfigRuleName: str,
    OrganizationConfigRuleArn: str,
    OrganizationManagedRuleMetadata: NotRequired[OrganizationManagedRuleMetadataOutputTypeDef],  # (1)
    OrganizationCustomRuleMetadata: NotRequired[OrganizationCustomRuleMetadataOutputTypeDef],  # (2)
    ExcludedAccounts: NotRequired[List[str]],
    LastUpdateTime: NotRequired[datetime],
    OrganizationCustomPolicyRuleMetadata: NotRequired[OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef],  # (3)
```

1. See [:material-code-braces: OrganizationManagedRuleMetadataOutputTypeDef](./type_defs.md#organizationmanagedrulemetadataoutputtypedef) 
2. See [:material-code-braces: OrganizationCustomRuleMetadataOutputTypeDef](./type_defs.md#organizationcustomrulemetadataoutputtypedef) 
3. See [:material-code-braces: OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef](./type_defs.md#organizationcustompolicyrulemetadatanopolicytypedef) 
## RecordingGroupOutputTypeDef

```python
# RecordingGroupOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RecordingGroupOutputTypeDef


def get_value() -> RecordingGroupOutputTypeDef:
    return {
        "allSupported": ...,
    }


# RecordingGroupOutputTypeDef definition

class RecordingGroupOutputTypeDef(TypedDict):
    allSupported: NotRequired[bool],
    includeGlobalResourceTypes: NotRequired[bool],
    resourceTypes: NotRequired[List[ResourceTypeType]],  # (1)
    exclusionByResourceTypes: NotRequired[ExclusionByResourceTypesOutputTypeDef],  # (2)
    recordingStrategy: NotRequired[RecordingStrategyTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ExclusionByResourceTypesOutputTypeDef](./type_defs.md#exclusionbyresourcetypesoutputtypedef) 
3. See [:material-code-braces: RecordingStrategyTypeDef](./type_defs.md#recordingstrategytypedef) 
## RecordingGroupTypeDef

```python
# RecordingGroupTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RecordingGroupTypeDef


def get_value() -> RecordingGroupTypeDef:
    return {
        "allSupported": ...,
    }


# RecordingGroupTypeDef definition

class RecordingGroupTypeDef(TypedDict):
    allSupported: NotRequired[bool],
    includeGlobalResourceTypes: NotRequired[bool],
    resourceTypes: NotRequired[Sequence[ResourceTypeType]],  # (1)
    exclusionByResourceTypes: NotRequired[ExclusionByResourceTypesTypeDef],  # (2)
    recordingStrategy: NotRequired[RecordingStrategyTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ExclusionByResourceTypesTypeDef](./type_defs.md#exclusionbyresourcetypestypedef) 
3. See [:material-code-braces: RecordingStrategyTypeDef](./type_defs.md#recordingstrategytypedef) 
## RecordingModeOutputTypeDef

```python
# RecordingModeOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RecordingModeOutputTypeDef


def get_value() -> RecordingModeOutputTypeDef:
    return {
        "recordingFrequency": ...,
    }


# RecordingModeOutputTypeDef definition

class RecordingModeOutputTypeDef(TypedDict):
    recordingFrequency: RecordingFrequencyType,  # (1)
    recordingModeOverrides: NotRequired[List[RecordingModeOverrideOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: RecordingFrequencyType](./literals.md#recordingfrequencytype) 
2. See [:material-code-braces: RecordingModeOverrideOutputTypeDef](./type_defs.md#recordingmodeoverrideoutputtypedef) 
## RecordingModeTypeDef

```python
# RecordingModeTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RecordingModeTypeDef


def get_value() -> RecordingModeTypeDef:
    return {
        "recordingFrequency": ...,
    }


# RecordingModeTypeDef definition

class RecordingModeTypeDef(TypedDict):
    recordingFrequency: RecordingFrequencyType,  # (1)
    recordingModeOverrides: NotRequired[Sequence[RecordingModeOverrideTypeDef]],  # (2)
```

1. See [:material-code-brackets: RecordingFrequencyType](./literals.md#recordingfrequencytype) 
2. See [:material-code-braces: RecordingModeOverrideTypeDef](./type_defs.md#recordingmodeoverridetypedef) 
## RemediationExecutionStatusTypeDef

```python
# RemediationExecutionStatusTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RemediationExecutionStatusTypeDef


def get_value() -> RemediationExecutionStatusTypeDef:
    return {
        "ResourceKey": ...,
    }


# RemediationExecutionStatusTypeDef definition

class RemediationExecutionStatusTypeDef(TypedDict):
    ResourceKey: NotRequired[ResourceKeyTypeDef],  # (1)
    State: NotRequired[RemediationExecutionStateType],  # (2)
    StepDetails: NotRequired[List[RemediationExecutionStepTypeDef]],  # (3)
    InvocationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
2. See [:material-code-brackets: RemediationExecutionStateType](./literals.md#remediationexecutionstatetype) 
3. See [:material-code-braces: RemediationExecutionStepTypeDef](./type_defs.md#remediationexecutionsteptypedef) 
## RemediationParameterValueOutputTypeDef

```python
# RemediationParameterValueOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RemediationParameterValueOutputTypeDef


def get_value() -> RemediationParameterValueOutputTypeDef:
    return {
        "ResourceValue": ...,
    }


# RemediationParameterValueOutputTypeDef definition

class RemediationParameterValueOutputTypeDef(TypedDict):
    ResourceValue: NotRequired[ResourceValueTypeDef],  # (1)
    StaticValue: NotRequired[StaticValueOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceValueTypeDef](./type_defs.md#resourcevaluetypedef) 
2. See [:material-code-braces: StaticValueOutputTypeDef](./type_defs.md#staticvalueoutputtypedef) 
## SourceOutputTypeDef

```python
# SourceOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SourceOutputTypeDef


def get_value() -> SourceOutputTypeDef:
    return {
        "Owner": ...,
    }


# SourceOutputTypeDef definition

class SourceOutputTypeDef(TypedDict):
    Owner: OwnerType,  # (1)
    SourceIdentifier: NotRequired[str],
    SourceDetails: NotRequired[List[SourceDetailTypeDef]],  # (2)
    CustomPolicyDetails: NotRequired[CustomPolicyDetailsTypeDef],  # (3)
```

1. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
2. See [:material-code-braces: SourceDetailTypeDef](./type_defs.md#sourcedetailtypedef) 
3. See [:material-code-braces: CustomPolicyDetailsTypeDef](./type_defs.md#custompolicydetailstypedef) 
## SourceTypeDef

```python
# SourceTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SourceTypeDef


def get_value() -> SourceTypeDef:
    return {
        "Owner": ...,
    }


# SourceTypeDef definition

class SourceTypeDef(TypedDict):
    Owner: OwnerType,  # (1)
    SourceIdentifier: NotRequired[str],
    SourceDetails: NotRequired[Sequence[SourceDetailTypeDef]],  # (2)
    CustomPolicyDetails: NotRequired[CustomPolicyDetailsTypeDef],  # (3)
```

1. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
2. See [:material-code-braces: SourceDetailTypeDef](./type_defs.md#sourcedetailtypedef) 
3. See [:material-code-braces: CustomPolicyDetailsTypeDef](./type_defs.md#custompolicydetailstypedef) 
## DescribeAggregateComplianceByConformancePacksResponseTypeDef

```python
# DescribeAggregateComplianceByConformancePacksResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregateComplianceByConformancePacksResponseTypeDef


def get_value() -> DescribeAggregateComplianceByConformancePacksResponseTypeDef:
    return {
        "AggregateComplianceByConformancePacks": ...,
    }


# DescribeAggregateComplianceByConformancePacksResponseTypeDef definition

class DescribeAggregateComplianceByConformancePacksResponseTypeDef(TypedDict):
    AggregateComplianceByConformancePacks: List[AggregateComplianceByConformancePackTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregateComplianceByConformancePackTypeDef](./type_defs.md#aggregatecompliancebyconformancepacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAggregateConformancePackComplianceSummaryResponseTypeDef

```python
# GetAggregateConformancePackComplianceSummaryResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateConformancePackComplianceSummaryResponseTypeDef


def get_value() -> GetAggregateConformancePackComplianceSummaryResponseTypeDef:
    return {
        "AggregateConformancePackComplianceSummaries": ...,
    }


# GetAggregateConformancePackComplianceSummaryResponseTypeDef definition

class GetAggregateConformancePackComplianceSummaryResponseTypeDef(TypedDict):
    AggregateConformancePackComplianceSummaries: List[AggregateConformancePackComplianceSummaryTypeDef],  # (1)
    GroupByKey: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregateConformancePackComplianceSummaryTypeDef](./type_defs.md#aggregateconformancepackcompliancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfigurationAggregatorTypeDef

```python
# ConfigurationAggregatorTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigurationAggregatorTypeDef


def get_value() -> ConfigurationAggregatorTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# ConfigurationAggregatorTypeDef definition

class ConfigurationAggregatorTypeDef(TypedDict):
    ConfigurationAggregatorName: NotRequired[str],
    ConfigurationAggregatorArn: NotRequired[str],
    AccountAggregationSources: NotRequired[List[AccountAggregationSourceOutputTypeDef]],  # (1)
    OrganizationAggregationSource: NotRequired[OrganizationAggregationSourceOutputTypeDef],  # (2)
    CreationTime: NotRequired[datetime],
    LastUpdatedTime: NotRequired[datetime],
    CreatedBy: NotRequired[str],
    AggregatorFilters: NotRequired[AggregatorFiltersOutputTypeDef],  # (3)
```

1. See [:material-code-braces: AccountAggregationSourceOutputTypeDef](./type_defs.md#accountaggregationsourceoutputtypedef) 
2. See [:material-code-braces: OrganizationAggregationSourceOutputTypeDef](./type_defs.md#organizationaggregationsourceoutputtypedef) 
3. See [:material-code-braces: AggregatorFiltersOutputTypeDef](./type_defs.md#aggregatorfiltersoutputtypedef) 
## AggregateComplianceCountTypeDef

```python
# AggregateComplianceCountTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateComplianceCountTypeDef


def get_value() -> AggregateComplianceCountTypeDef:
    return {
        "GroupName": ...,
    }


# AggregateComplianceCountTypeDef definition

class AggregateComplianceCountTypeDef(TypedDict):
    GroupName: NotRequired[str],
    ComplianceSummary: NotRequired[ComplianceSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: ComplianceSummaryTypeDef](./type_defs.md#compliancesummarytypedef) 
## ComplianceSummaryByResourceTypeTypeDef

```python
# ComplianceSummaryByResourceTypeTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ComplianceSummaryByResourceTypeTypeDef


def get_value() -> ComplianceSummaryByResourceTypeTypeDef:
    return {
        "ResourceType": ...,
    }


# ComplianceSummaryByResourceTypeTypeDef definition

class ComplianceSummaryByResourceTypeTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    ComplianceSummary: NotRequired[ComplianceSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: ComplianceSummaryTypeDef](./type_defs.md#compliancesummarytypedef) 
## GetComplianceSummaryByConfigRuleResponseTypeDef

```python
# GetComplianceSummaryByConfigRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceSummaryByConfigRuleResponseTypeDef


def get_value() -> GetComplianceSummaryByConfigRuleResponseTypeDef:
    return {
        "ComplianceSummary": ...,
    }


# GetComplianceSummaryByConfigRuleResponseTypeDef definition

class GetComplianceSummaryByConfigRuleResponseTypeDef(TypedDict):
    ComplianceSummary: ComplianceSummaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComplianceSummaryTypeDef](./type_defs.md#compliancesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AggregateComplianceByConfigRuleTypeDef

```python
# AggregateComplianceByConfigRuleTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateComplianceByConfigRuleTypeDef


def get_value() -> AggregateComplianceByConfigRuleTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# AggregateComplianceByConfigRuleTypeDef definition

class AggregateComplianceByConfigRuleTypeDef(TypedDict):
    ConfigRuleName: NotRequired[str],
    Compliance: NotRequired[ComplianceTypeDef],  # (1)
    AccountId: NotRequired[str],
    AwsRegion: NotRequired[str],
```

1. See [:material-code-braces: ComplianceTypeDef](./type_defs.md#compliancetypedef) 
## ComplianceByConfigRuleTypeDef

```python
# ComplianceByConfigRuleTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ComplianceByConfigRuleTypeDef


def get_value() -> ComplianceByConfigRuleTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# ComplianceByConfigRuleTypeDef definition

class ComplianceByConfigRuleTypeDef(TypedDict):
    ConfigRuleName: NotRequired[str],
    Compliance: NotRequired[ComplianceTypeDef],  # (1)
```

1. See [:material-code-braces: ComplianceTypeDef](./type_defs.md#compliancetypedef) 
## ComplianceByResourceTypeDef

```python
# ComplianceByResourceTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ComplianceByResourceTypeDef


def get_value() -> ComplianceByResourceTypeDef:
    return {
        "ResourceType": ...,
    }


# ComplianceByResourceTypeDef definition

class ComplianceByResourceTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    ResourceId: NotRequired[str],
    Compliance: NotRequired[ComplianceTypeDef],  # (1)
```

1. See [:material-code-braces: ComplianceTypeDef](./type_defs.md#compliancetypedef) 
## DescribeDeliveryChannelsResponseTypeDef

```python
# DescribeDeliveryChannelsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeDeliveryChannelsResponseTypeDef


def get_value() -> DescribeDeliveryChannelsResponseTypeDef:
    return {
        "DeliveryChannels": ...,
    }


# DescribeDeliveryChannelsResponseTypeDef definition

class DescribeDeliveryChannelsResponseTypeDef(TypedDict):
    DeliveryChannels: List[DeliveryChannelTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliveryChannelTypeDef](./type_defs.md#deliverychanneltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutDeliveryChannelRequestTypeDef

```python
# PutDeliveryChannelRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutDeliveryChannelRequestTypeDef


def get_value() -> PutDeliveryChannelRequestTypeDef:
    return {
        "DeliveryChannel": ...,
    }


# PutDeliveryChannelRequestTypeDef definition

class PutDeliveryChannelRequestTypeDef(TypedDict):
    DeliveryChannel: DeliveryChannelTypeDef,  # (1)
```

1. See [:material-code-braces: DeliveryChannelTypeDef](./type_defs.md#deliverychanneltypedef) 
## DescribeDeliveryChannelStatusResponseTypeDef

```python
# DescribeDeliveryChannelStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeDeliveryChannelStatusResponseTypeDef


def get_value() -> DescribeDeliveryChannelStatusResponseTypeDef:
    return {
        "DeliveryChannelsStatus": ...,
    }


# DescribeDeliveryChannelStatusResponseTypeDef definition

class DescribeDeliveryChannelStatusResponseTypeDef(TypedDict):
    DeliveryChannelsStatus: List[DeliveryChannelStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeliveryChannelStatusTypeDef](./type_defs.md#deliverychannelstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAggregateResourceConfigResponseTypeDef

```python
# GetAggregateResourceConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateResourceConfigResponseTypeDef


def get_value() -> GetAggregateResourceConfigResponseTypeDef:
    return {
        "ConfigurationItem": ...,
    }


# GetAggregateResourceConfigResponseTypeDef definition

class GetAggregateResourceConfigResponseTypeDef(TypedDict):
    ConfigurationItem: ConfigurationItemTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationItemTypeDef](./type_defs.md#configurationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceConfigHistoryResponseTypeDef

```python
# GetResourceConfigHistoryResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetResourceConfigHistoryResponseTypeDef


def get_value() -> GetResourceConfigHistoryResponseTypeDef:
    return {
        "configurationItems": ...,
    }


# GetResourceConfigHistoryResponseTypeDef definition

class GetResourceConfigHistoryResponseTypeDef(TypedDict):
    configurationItems: List[ConfigurationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationItemTypeDef](./type_defs.md#configurationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationConformancePacksResponseTypeDef

```python
# DescribeOrganizationConformancePacksResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConformancePacksResponseTypeDef


def get_value() -> DescribeOrganizationConformancePacksResponseTypeDef:
    return {
        "OrganizationConformancePacks": ...,
    }


# DescribeOrganizationConformancePacksResponseTypeDef definition

class DescribeOrganizationConformancePacksResponseTypeDef(TypedDict):
    OrganizationConformancePacks: List[OrganizationConformancePackTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationConformancePackTypeDef](./type_defs.md#organizationconformancepacktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConformancePacksResponseTypeDef

```python
# DescribeConformancePacksResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConformancePacksResponseTypeDef


def get_value() -> DescribeConformancePacksResponseTypeDef:
    return {
        "ConformancePackDetails": ...,
    }


# DescribeConformancePacksResponseTypeDef definition

class DescribeConformancePacksResponseTypeDef(TypedDict):
    ConformancePackDetails: List[ConformancePackDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackDetailTypeDef](./type_defs.md#conformancepackdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteRemediationExceptionsResponseTypeDef

```python
# DeleteRemediationExceptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DeleteRemediationExceptionsResponseTypeDef


def get_value() -> DeleteRemediationExceptionsResponseTypeDef:
    return {
        "FailedBatches": ...,
    }


# DeleteRemediationExceptionsResponseTypeDef definition

class DeleteRemediationExceptionsResponseTypeDef(TypedDict):
    FailedBatches: List[FailedDeleteRemediationExceptionsBatchTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedDeleteRemediationExceptionsBatchTypeDef](./type_defs.md#faileddeleteremediationexceptionsbatchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRemediationExceptionsResponseTypeDef

```python
# PutRemediationExceptionsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutRemediationExceptionsResponseTypeDef


def get_value() -> PutRemediationExceptionsResponseTypeDef:
    return {
        "FailedBatches": ...,
    }


# PutRemediationExceptionsResponseTypeDef definition

class PutRemediationExceptionsResponseTypeDef(TypedDict):
    FailedBatches: List[FailedRemediationExceptionBatchTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedRemediationExceptionBatchTypeDef](./type_defs.md#failedremediationexceptionbatchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AggregateEvaluationResultTypeDef

```python
# AggregateEvaluationResultTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AggregateEvaluationResultTypeDef


def get_value() -> AggregateEvaluationResultTypeDef:
    return {
        "EvaluationResultIdentifier": ...,
    }


# AggregateEvaluationResultTypeDef definition

class AggregateEvaluationResultTypeDef(TypedDict):
    EvaluationResultIdentifier: NotRequired[EvaluationResultIdentifierTypeDef],  # (1)
    ComplianceType: NotRequired[ComplianceTypeType],  # (2)
    ResultRecordedTime: NotRequired[datetime],
    ConfigRuleInvokedTime: NotRequired[datetime],
    Annotation: NotRequired[str],
    AccountId: NotRequired[str],
    AwsRegion: NotRequired[str],
```

1. See [:material-code-braces: EvaluationResultIdentifierTypeDef](./type_defs.md#evaluationresultidentifiertypedef) 
2. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## ConformancePackEvaluationResultTypeDef

```python
# ConformancePackEvaluationResultTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConformancePackEvaluationResultTypeDef


def get_value() -> ConformancePackEvaluationResultTypeDef:
    return {
        "ComplianceType": ...,
    }


# ConformancePackEvaluationResultTypeDef definition

class ConformancePackEvaluationResultTypeDef(TypedDict):
    ComplianceType: ConformancePackComplianceTypeType,  # (1)
    EvaluationResultIdentifier: EvaluationResultIdentifierTypeDef,  # (2)
    ConfigRuleInvokedTime: datetime,
    ResultRecordedTime: datetime,
    Annotation: NotRequired[str],
```

1. See [:material-code-brackets: ConformancePackComplianceTypeType](./literals.md#conformancepackcompliancetypetype) 
2. See [:material-code-braces: EvaluationResultIdentifierTypeDef](./type_defs.md#evaluationresultidentifiertypedef) 
## EvaluationResultTypeDef

```python
# EvaluationResultTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import EvaluationResultTypeDef


def get_value() -> EvaluationResultTypeDef:
    return {
        "EvaluationResultIdentifier": ...,
    }


# EvaluationResultTypeDef definition

class EvaluationResultTypeDef(TypedDict):
    EvaluationResultIdentifier: NotRequired[EvaluationResultIdentifierTypeDef],  # (1)
    ComplianceType: NotRequired[ComplianceTypeType],  # (2)
    ResultRecordedTime: NotRequired[datetime],
    ConfigRuleInvokedTime: NotRequired[datetime],
    Annotation: NotRequired[str],
    ResultToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationResultIdentifierTypeDef](./type_defs.md#evaluationresultidentifiertypedef) 
2. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
## PutExternalEvaluationRequestTypeDef

```python
# PutExternalEvaluationRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutExternalEvaluationRequestTypeDef


def get_value() -> PutExternalEvaluationRequestTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# PutExternalEvaluationRequestTypeDef definition

class PutExternalEvaluationRequestTypeDef(TypedDict):
    ConfigRuleName: str,
    ExternalEvaluation: ExternalEvaluationTypeDef,  # (1)
```

1. See [:material-code-braces: ExternalEvaluationTypeDef](./type_defs.md#externalevaluationtypedef) 
## ResourceEvaluationFiltersTypeDef

```python
# ResourceEvaluationFiltersTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ResourceEvaluationFiltersTypeDef


def get_value() -> ResourceEvaluationFiltersTypeDef:
    return {
        "EvaluationMode": ...,
    }


# ResourceEvaluationFiltersTypeDef definition

class ResourceEvaluationFiltersTypeDef(TypedDict):
    EvaluationMode: NotRequired[EvaluationModeType],  # (1)
    TimeWindow: NotRequired[TimeWindowTypeDef],  # (2)
    EvaluationContextIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: EvaluationModeType](./literals.md#evaluationmodetype) 
2. See [:material-code-braces: TimeWindowTypeDef](./type_defs.md#timewindowtypedef) 
## SelectAggregateResourceConfigResponseTypeDef

```python
# SelectAggregateResourceConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SelectAggregateResourceConfigResponseTypeDef


def get_value() -> SelectAggregateResourceConfigResponseTypeDef:
    return {
        "Results": ...,
    }


# SelectAggregateResourceConfigResponseTypeDef definition

class SelectAggregateResourceConfigResponseTypeDef(TypedDict):
    Results: List[str],
    QueryInfo: QueryInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QueryInfoTypeDef](./type_defs.md#queryinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SelectResourceConfigResponseTypeDef

```python
# SelectResourceConfigResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import SelectResourceConfigResponseTypeDef


def get_value() -> SelectResourceConfigResponseTypeDef:
    return {
        "Results": ...,
    }


# SelectResourceConfigResponseTypeDef definition

class SelectResourceConfigResponseTypeDef(TypedDict):
    Results: List[str],
    QueryInfo: QueryInfoTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: QueryInfoTypeDef](./type_defs.md#queryinfotypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeOrganizationConfigRulesResponseTypeDef

```python
# DescribeOrganizationConfigRulesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeOrganizationConfigRulesResponseTypeDef


def get_value() -> DescribeOrganizationConfigRulesResponseTypeDef:
    return {
        "OrganizationConfigRules": ...,
    }


# DescribeOrganizationConfigRulesResponseTypeDef definition

class DescribeOrganizationConfigRulesResponseTypeDef(TypedDict):
    OrganizationConfigRules: List[OrganizationConfigRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationConfigRuleTypeDef](./type_defs.md#organizationconfigruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutOrganizationConfigRuleRequestTypeDef

```python
# PutOrganizationConfigRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutOrganizationConfigRuleRequestTypeDef


def get_value() -> PutOrganizationConfigRuleRequestTypeDef:
    return {
        "OrganizationConfigRuleName": ...,
    }


# PutOrganizationConfigRuleRequestTypeDef definition

class PutOrganizationConfigRuleRequestTypeDef(TypedDict):
    OrganizationConfigRuleName: str,
    OrganizationManagedRuleMetadata: NotRequired[OrganizationManagedRuleMetadataUnionTypeDef],  # (1)
    OrganizationCustomRuleMetadata: NotRequired[OrganizationCustomRuleMetadataUnionTypeDef],  # (2)
    ExcludedAccounts: NotRequired[Sequence[str]],
    OrganizationCustomPolicyRuleMetadata: NotRequired[OrganizationCustomPolicyRuleMetadataTypeDef],  # (3)
```

1. See [:material-code-braces: OrganizationManagedRuleMetadataTypeDef](./type_defs.md#organizationmanagedrulemetadatatypedef) [:material-code-braces: OrganizationManagedRuleMetadataOutputTypeDef](./type_defs.md#organizationmanagedrulemetadataoutputtypedef) 
2. See [:material-code-braces: OrganizationCustomRuleMetadataTypeDef](./type_defs.md#organizationcustomrulemetadatatypedef) [:material-code-braces: OrganizationCustomRuleMetadataOutputTypeDef](./type_defs.md#organizationcustomrulemetadataoutputtypedef) 
3. See [:material-code-braces: OrganizationCustomPolicyRuleMetadataTypeDef](./type_defs.md#organizationcustompolicyrulemetadatatypedef) 
## ConfigurationRecorderOutputTypeDef

```python
# ConfigurationRecorderOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigurationRecorderOutputTypeDef


def get_value() -> ConfigurationRecorderOutputTypeDef:
    return {
        "arn": ...,
    }


# ConfigurationRecorderOutputTypeDef definition

class ConfigurationRecorderOutputTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    roleARN: NotRequired[str],
    recordingGroup: NotRequired[RecordingGroupOutputTypeDef],  # (1)
    recordingMode: NotRequired[RecordingModeOutputTypeDef],  # (2)
    recordingScope: NotRequired[RecordingScopeType],  # (3)
    servicePrincipal: NotRequired[str],
```

1. See [:material-code-braces: RecordingGroupOutputTypeDef](./type_defs.md#recordinggroupoutputtypedef) 
2. See [:material-code-braces: RecordingModeOutputTypeDef](./type_defs.md#recordingmodeoutputtypedef) 
3. See [:material-code-brackets: RecordingScopeType](./literals.md#recordingscopetype) 
## ConfigurationRecorderTypeDef

```python
# ConfigurationRecorderTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigurationRecorderTypeDef


def get_value() -> ConfigurationRecorderTypeDef:
    return {
        "arn": ...,
    }


# ConfigurationRecorderTypeDef definition

class ConfigurationRecorderTypeDef(TypedDict):
    arn: NotRequired[str],
    name: NotRequired[str],
    roleARN: NotRequired[str],
    recordingGroup: NotRequired[RecordingGroupTypeDef],  # (1)
    recordingMode: NotRequired[RecordingModeTypeDef],  # (2)
    recordingScope: NotRequired[RecordingScopeType],  # (3)
    servicePrincipal: NotRequired[str],
```

1. See [:material-code-braces: RecordingGroupTypeDef](./type_defs.md#recordinggrouptypedef) 
2. See [:material-code-braces: RecordingModeTypeDef](./type_defs.md#recordingmodetypedef) 
3. See [:material-code-brackets: RecordingScopeType](./literals.md#recordingscopetype) 
## DescribeRemediationExecutionStatusResponseTypeDef

```python
# DescribeRemediationExecutionStatusResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRemediationExecutionStatusResponseTypeDef


def get_value() -> DescribeRemediationExecutionStatusResponseTypeDef:
    return {
        "RemediationExecutionStatuses": ...,
    }


# DescribeRemediationExecutionStatusResponseTypeDef definition

class DescribeRemediationExecutionStatusResponseTypeDef(TypedDict):
    RemediationExecutionStatuses: List[RemediationExecutionStatusTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RemediationExecutionStatusTypeDef](./type_defs.md#remediationexecutionstatustypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RemediationConfigurationOutputTypeDef

```python
# RemediationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RemediationConfigurationOutputTypeDef


def get_value() -> RemediationConfigurationOutputTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# RemediationConfigurationOutputTypeDef definition

class RemediationConfigurationOutputTypeDef(TypedDict):
    ConfigRuleName: str,
    TargetType: RemediationTargetTypeType,  # (1)
    TargetId: str,
    TargetVersion: NotRequired[str],
    Parameters: NotRequired[Dict[str, RemediationParameterValueOutputTypeDef]],  # (2)
    ResourceType: NotRequired[str],
    Automatic: NotRequired[bool],
    ExecutionControls: NotRequired[ExecutionControlsTypeDef],  # (3)
    MaximumAutomaticAttempts: NotRequired[int],
    RetryAttemptSeconds: NotRequired[int],
    Arn: NotRequired[str],
    CreatedByService: NotRequired[str],
```

1. See [:material-code-brackets: RemediationTargetTypeType](./literals.md#remediationtargettypetype) 
2. See [:material-code-braces: RemediationParameterValueOutputTypeDef](./type_defs.md#remediationparametervalueoutputtypedef) 
3. See [:material-code-braces: ExecutionControlsTypeDef](./type_defs.md#executioncontrolstypedef) 
## ConfigRuleOutputTypeDef

```python
# ConfigRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigRuleOutputTypeDef


def get_value() -> ConfigRuleOutputTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# ConfigRuleOutputTypeDef definition

class ConfigRuleOutputTypeDef(TypedDict):
    Source: SourceOutputTypeDef,  # (2)
    ConfigRuleName: NotRequired[str],
    ConfigRuleArn: NotRequired[str],
    ConfigRuleId: NotRequired[str],
    Description: NotRequired[str],
    Scope: NotRequired[ScopeOutputTypeDef],  # (1)
    InputParameters: NotRequired[str],
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (3)
    ConfigRuleState: NotRequired[ConfigRuleStateType],  # (4)
    CreatedBy: NotRequired[str],
    EvaluationModes: NotRequired[List[EvaluationModeConfigurationTypeDef]],  # (5)
```

1. See [:material-code-braces: ScopeOutputTypeDef](./type_defs.md#scopeoutputtypedef) 
2. See [:material-code-braces: SourceOutputTypeDef](./type_defs.md#sourceoutputtypedef) 
3. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
4. See [:material-code-brackets: ConfigRuleStateType](./literals.md#configrulestatetype) 
5. See [:material-code-braces: EvaluationModeConfigurationTypeDef](./type_defs.md#evaluationmodeconfigurationtypedef) 
## ConfigRuleTypeDef

```python
# ConfigRuleTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ConfigRuleTypeDef


def get_value() -> ConfigRuleTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# ConfigRuleTypeDef definition

class ConfigRuleTypeDef(TypedDict):
    Source: SourceTypeDef,  # (2)
    ConfigRuleName: NotRequired[str],
    ConfigRuleArn: NotRequired[str],
    ConfigRuleId: NotRequired[str],
    Description: NotRequired[str],
    Scope: NotRequired[ScopeTypeDef],  # (1)
    InputParameters: NotRequired[str],
    MaximumExecutionFrequency: NotRequired[MaximumExecutionFrequencyType],  # (3)
    ConfigRuleState: NotRequired[ConfigRuleStateType],  # (4)
    CreatedBy: NotRequired[str],
    EvaluationModes: NotRequired[Sequence[EvaluationModeConfigurationTypeDef]],  # (5)
```

1. See [:material-code-braces: ScopeTypeDef](./type_defs.md#scopetypedef) 
2. See [:material-code-braces: SourceTypeDef](./type_defs.md#sourcetypedef) 
3. See [:material-code-brackets: MaximumExecutionFrequencyType](./literals.md#maximumexecutionfrequencytype) 
4. See [:material-code-brackets: ConfigRuleStateType](./literals.md#configrulestatetype) 
5. See [:material-code-braces: EvaluationModeConfigurationTypeDef](./type_defs.md#evaluationmodeconfigurationtypedef) 
## RemediationParameterValueTypeDef

```python
# RemediationParameterValueTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RemediationParameterValueTypeDef


def get_value() -> RemediationParameterValueTypeDef:
    return {
        "ResourceValue": ...,
    }


# RemediationParameterValueTypeDef definition

class RemediationParameterValueTypeDef(TypedDict):
    ResourceValue: NotRequired[ResourceValueTypeDef],  # (1)
    StaticValue: NotRequired[StaticValueUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceValueTypeDef](./type_defs.md#resourcevaluetypedef) 
2. See [:material-code-braces: StaticValueTypeDef](./type_defs.md#staticvaluetypedef) [:material-code-braces: StaticValueOutputTypeDef](./type_defs.md#staticvalueoutputtypedef) 
## DescribeConfigurationAggregatorsResponseTypeDef

```python
# DescribeConfigurationAggregatorsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationAggregatorsResponseTypeDef


def get_value() -> DescribeConfigurationAggregatorsResponseTypeDef:
    return {
        "ConfigurationAggregators": ...,
    }


# DescribeConfigurationAggregatorsResponseTypeDef definition

class DescribeConfigurationAggregatorsResponseTypeDef(TypedDict):
    ConfigurationAggregators: List[ConfigurationAggregatorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigurationAggregatorTypeDef](./type_defs.md#configurationaggregatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfigurationAggregatorResponseTypeDef

```python
# PutConfigurationAggregatorResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutConfigurationAggregatorResponseTypeDef


def get_value() -> PutConfigurationAggregatorResponseTypeDef:
    return {
        "ConfigurationAggregator": ...,
    }


# PutConfigurationAggregatorResponseTypeDef definition

class PutConfigurationAggregatorResponseTypeDef(TypedDict):
    ConfigurationAggregator: ConfigurationAggregatorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationAggregatorTypeDef](./type_defs.md#configurationaggregatortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfigurationAggregatorRequestTypeDef

```python
# PutConfigurationAggregatorRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutConfigurationAggregatorRequestTypeDef


def get_value() -> PutConfigurationAggregatorRequestTypeDef:
    return {
        "ConfigurationAggregatorName": ...,
    }


# PutConfigurationAggregatorRequestTypeDef definition

class PutConfigurationAggregatorRequestTypeDef(TypedDict):
    ConfigurationAggregatorName: str,
    AccountAggregationSources: NotRequired[Sequence[AccountAggregationSourceUnionTypeDef]],  # (1)
    OrganizationAggregationSource: NotRequired[OrganizationAggregationSourceUnionTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    AggregatorFilters: NotRequired[AggregatorFiltersUnionTypeDef],  # (4)
```

1. See [:material-code-braces: AccountAggregationSourceTypeDef](./type_defs.md#accountaggregationsourcetypedef) [:material-code-braces: AccountAggregationSourceOutputTypeDef](./type_defs.md#accountaggregationsourceoutputtypedef) 
2. See [:material-code-braces: OrganizationAggregationSourceTypeDef](./type_defs.md#organizationaggregationsourcetypedef) [:material-code-braces: OrganizationAggregationSourceOutputTypeDef](./type_defs.md#organizationaggregationsourceoutputtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: AggregatorFiltersTypeDef](./type_defs.md#aggregatorfilterstypedef) [:material-code-braces: AggregatorFiltersOutputTypeDef](./type_defs.md#aggregatorfiltersoutputtypedef) 
## GetAggregateConfigRuleComplianceSummaryResponseTypeDef

```python
# GetAggregateConfigRuleComplianceSummaryResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateConfigRuleComplianceSummaryResponseTypeDef


def get_value() -> GetAggregateConfigRuleComplianceSummaryResponseTypeDef:
    return {
        "GroupByKey": ...,
    }


# GetAggregateConfigRuleComplianceSummaryResponseTypeDef definition

class GetAggregateConfigRuleComplianceSummaryResponseTypeDef(TypedDict):
    GroupByKey: str,
    AggregateComplianceCounts: List[AggregateComplianceCountTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregateComplianceCountTypeDef](./type_defs.md#aggregatecompliancecounttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComplianceSummaryByResourceTypeResponseTypeDef

```python
# GetComplianceSummaryByResourceTypeResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceSummaryByResourceTypeResponseTypeDef


def get_value() -> GetComplianceSummaryByResourceTypeResponseTypeDef:
    return {
        "ComplianceSummariesByResourceType": ...,
    }


# GetComplianceSummaryByResourceTypeResponseTypeDef definition

class GetComplianceSummaryByResourceTypeResponseTypeDef(TypedDict):
    ComplianceSummariesByResourceType: List[ComplianceSummaryByResourceTypeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ComplianceSummaryByResourceTypeTypeDef](./type_defs.md#compliancesummarybyresourcetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeAggregateComplianceByConfigRulesResponseTypeDef

```python
# DescribeAggregateComplianceByConfigRulesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeAggregateComplianceByConfigRulesResponseTypeDef


def get_value() -> DescribeAggregateComplianceByConfigRulesResponseTypeDef:
    return {
        "AggregateComplianceByConfigRules": ...,
    }


# DescribeAggregateComplianceByConfigRulesResponseTypeDef definition

class DescribeAggregateComplianceByConfigRulesResponseTypeDef(TypedDict):
    AggregateComplianceByConfigRules: List[AggregateComplianceByConfigRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregateComplianceByConfigRuleTypeDef](./type_defs.md#aggregatecompliancebyconfigruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeComplianceByConfigRuleResponseTypeDef

```python
# DescribeComplianceByConfigRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeComplianceByConfigRuleResponseTypeDef


def get_value() -> DescribeComplianceByConfigRuleResponseTypeDef:
    return {
        "ComplianceByConfigRules": ...,
    }


# DescribeComplianceByConfigRuleResponseTypeDef definition

class DescribeComplianceByConfigRuleResponseTypeDef(TypedDict):
    ComplianceByConfigRules: List[ComplianceByConfigRuleTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComplianceByConfigRuleTypeDef](./type_defs.md#compliancebyconfigruletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeComplianceByResourceResponseTypeDef

```python
# DescribeComplianceByResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeComplianceByResourceResponseTypeDef


def get_value() -> DescribeComplianceByResourceResponseTypeDef:
    return {
        "ComplianceByResources": ...,
    }


# DescribeComplianceByResourceResponseTypeDef definition

class DescribeComplianceByResourceResponseTypeDef(TypedDict):
    ComplianceByResources: List[ComplianceByResourceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ComplianceByResourceTypeDef](./type_defs.md#compliancebyresourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAggregateComplianceDetailsByConfigRuleResponseTypeDef

```python
# GetAggregateComplianceDetailsByConfigRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetAggregateComplianceDetailsByConfigRuleResponseTypeDef


def get_value() -> GetAggregateComplianceDetailsByConfigRuleResponseTypeDef:
    return {
        "AggregateEvaluationResults": ...,
    }


# GetAggregateComplianceDetailsByConfigRuleResponseTypeDef definition

class GetAggregateComplianceDetailsByConfigRuleResponseTypeDef(TypedDict):
    AggregateEvaluationResults: List[AggregateEvaluationResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: AggregateEvaluationResultTypeDef](./type_defs.md#aggregateevaluationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConformancePackComplianceDetailsResponseTypeDef

```python
# GetConformancePackComplianceDetailsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetConformancePackComplianceDetailsResponseTypeDef


def get_value() -> GetConformancePackComplianceDetailsResponseTypeDef:
    return {
        "ConformancePackName": ...,
    }


# GetConformancePackComplianceDetailsResponseTypeDef definition

class GetConformancePackComplianceDetailsResponseTypeDef(TypedDict):
    ConformancePackName: str,
    ConformancePackRuleEvaluationResults: List[ConformancePackEvaluationResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConformancePackEvaluationResultTypeDef](./type_defs.md#conformancepackevaluationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComplianceDetailsByConfigRuleResponseTypeDef

```python
# GetComplianceDetailsByConfigRuleResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceDetailsByConfigRuleResponseTypeDef


def get_value() -> GetComplianceDetailsByConfigRuleResponseTypeDef:
    return {
        "EvaluationResults": ...,
    }


# GetComplianceDetailsByConfigRuleResponseTypeDef definition

class GetComplianceDetailsByConfigRuleResponseTypeDef(TypedDict):
    EvaluationResults: List[EvaluationResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetComplianceDetailsByResourceResponseTypeDef

```python
# GetComplianceDetailsByResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import GetComplianceDetailsByResourceResponseTypeDef


def get_value() -> GetComplianceDetailsByResourceResponseTypeDef:
    return {
        "EvaluationResults": ...,
    }


# GetComplianceDetailsByResourceResponseTypeDef definition

class GetComplianceDetailsByResourceResponseTypeDef(TypedDict):
    EvaluationResults: List[EvaluationResultTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EvaluationResultTypeDef](./type_defs.md#evaluationresulttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEvaluationsRequestTypeDef

```python
# PutEvaluationsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutEvaluationsRequestTypeDef


def get_value() -> PutEvaluationsRequestTypeDef:
    return {
        "ResultToken": ...,
    }


# PutEvaluationsRequestTypeDef definition

class PutEvaluationsRequestTypeDef(TypedDict):
    ResultToken: str,
    Evaluations: NotRequired[Sequence[EvaluationUnionTypeDef]],  # (1)
    TestMode: NotRequired[bool],
```

1. See [:material-code-braces: EvaluationTypeDef](./type_defs.md#evaluationtypedef) [:material-code-braces: EvaluationOutputTypeDef](./type_defs.md#evaluationoutputtypedef) 
## ListResourceEvaluationsRequestPaginateTypeDef

```python
# ListResourceEvaluationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListResourceEvaluationsRequestPaginateTypeDef


def get_value() -> ListResourceEvaluationsRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListResourceEvaluationsRequestPaginateTypeDef definition

class ListResourceEvaluationsRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[ResourceEvaluationFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ResourceEvaluationFiltersTypeDef](./type_defs.md#resourceevaluationfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceEvaluationsRequestTypeDef

```python
# ListResourceEvaluationsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import ListResourceEvaluationsRequestTypeDef


def get_value() -> ListResourceEvaluationsRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListResourceEvaluationsRequestTypeDef definition

class ListResourceEvaluationsRequestTypeDef(TypedDict):
    Filters: NotRequired[ResourceEvaluationFiltersTypeDef],  # (1)
    Limit: NotRequired[int],
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceEvaluationFiltersTypeDef](./type_defs.md#resourceevaluationfilterstypedef) 
## AssociateResourceTypesResponseTypeDef

```python
# AssociateResourceTypesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import AssociateResourceTypesResponseTypeDef


def get_value() -> AssociateResourceTypesResponseTypeDef:
    return {
        "ConfigurationRecorder": ...,
    }


# AssociateResourceTypesResponseTypeDef definition

class AssociateResourceTypesResponseTypeDef(TypedDict):
    ConfigurationRecorder: ConfigurationRecorderOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationRecorderOutputTypeDef](./type_defs.md#configurationrecorderoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConfigurationRecordersResponseTypeDef

```python
# DescribeConfigurationRecordersResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigurationRecordersResponseTypeDef


def get_value() -> DescribeConfigurationRecordersResponseTypeDef:
    return {
        "ConfigurationRecorders": ...,
    }


# DescribeConfigurationRecordersResponseTypeDef definition

class DescribeConfigurationRecordersResponseTypeDef(TypedDict):
    ConfigurationRecorders: List[ConfigurationRecorderOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationRecorderOutputTypeDef](./type_defs.md#configurationrecorderoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateResourceTypesResponseTypeDef

```python
# DisassociateResourceTypesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DisassociateResourceTypesResponseTypeDef


def get_value() -> DisassociateResourceTypesResponseTypeDef:
    return {
        "ConfigurationRecorder": ...,
    }


# DisassociateResourceTypesResponseTypeDef definition

class DisassociateResourceTypesResponseTypeDef(TypedDict):
    ConfigurationRecorder: ConfigurationRecorderOutputTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConfigurationRecorderOutputTypeDef](./type_defs.md#configurationrecorderoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRemediationConfigurationsResponseTypeDef

```python
# DescribeRemediationConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeRemediationConfigurationsResponseTypeDef


def get_value() -> DescribeRemediationConfigurationsResponseTypeDef:
    return {
        "RemediationConfigurations": ...,
    }


# DescribeRemediationConfigurationsResponseTypeDef definition

class DescribeRemediationConfigurationsResponseTypeDef(TypedDict):
    RemediationConfigurations: List[RemediationConfigurationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RemediationConfigurationOutputTypeDef](./type_defs.md#remediationconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailedRemediationBatchTypeDef

```python
# FailedRemediationBatchTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import FailedRemediationBatchTypeDef


def get_value() -> FailedRemediationBatchTypeDef:
    return {
        "FailureMessage": ...,
    }


# FailedRemediationBatchTypeDef definition

class FailedRemediationBatchTypeDef(TypedDict):
    FailureMessage: NotRequired[str],
    FailedItems: NotRequired[List[RemediationConfigurationOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: RemediationConfigurationOutputTypeDef](./type_defs.md#remediationconfigurationoutputtypedef) 
## DescribeConfigRulesResponseTypeDef

```python
# DescribeConfigRulesResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import DescribeConfigRulesResponseTypeDef


def get_value() -> DescribeConfigRulesResponseTypeDef:
    return {
        "ConfigRules": ...,
    }


# DescribeConfigRulesResponseTypeDef definition

class DescribeConfigRulesResponseTypeDef(TypedDict):
    ConfigRules: List[ConfigRuleOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ConfigRuleOutputTypeDef](./type_defs.md#configruleoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfigurationRecorderRequestTypeDef

```python
# PutConfigurationRecorderRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutConfigurationRecorderRequestTypeDef


def get_value() -> PutConfigurationRecorderRequestTypeDef:
    return {
        "ConfigurationRecorder": ...,
    }


# PutConfigurationRecorderRequestTypeDef definition

class PutConfigurationRecorderRequestTypeDef(TypedDict):
    ConfigurationRecorder: ConfigurationRecorderUnionTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ConfigurationRecorderTypeDef](./type_defs.md#configurationrecordertypedef) [:material-code-braces: ConfigurationRecorderOutputTypeDef](./type_defs.md#configurationrecorderoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## PutRemediationConfigurationsResponseTypeDef

```python
# PutRemediationConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutRemediationConfigurationsResponseTypeDef


def get_value() -> PutRemediationConfigurationsResponseTypeDef:
    return {
        "FailedBatches": ...,
    }


# PutRemediationConfigurationsResponseTypeDef definition

class PutRemediationConfigurationsResponseTypeDef(TypedDict):
    FailedBatches: List[FailedRemediationBatchTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedRemediationBatchTypeDef](./type_defs.md#failedremediationbatchtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutConfigRuleRequestTypeDef

```python
# PutConfigRuleRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutConfigRuleRequestTypeDef


def get_value() -> PutConfigRuleRequestTypeDef:
    return {
        "ConfigRule": ...,
    }


# PutConfigRuleRequestTypeDef definition

class PutConfigRuleRequestTypeDef(TypedDict):
    ConfigRule: ConfigRuleUnionTypeDef,  # (1)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: ConfigRuleTypeDef](./type_defs.md#configruletypedef) [:material-code-braces: ConfigRuleOutputTypeDef](./type_defs.md#configruleoutputtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RemediationConfigurationTypeDef

```python
# RemediationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import RemediationConfigurationTypeDef


def get_value() -> RemediationConfigurationTypeDef:
    return {
        "ConfigRuleName": ...,
    }


# RemediationConfigurationTypeDef definition

class RemediationConfigurationTypeDef(TypedDict):
    ConfigRuleName: str,
    TargetType: RemediationTargetTypeType,  # (1)
    TargetId: str,
    TargetVersion: NotRequired[str],
    Parameters: NotRequired[Mapping[str, RemediationParameterValueUnionTypeDef]],  # (2)
    ResourceType: NotRequired[str],
    Automatic: NotRequired[bool],
    ExecutionControls: NotRequired[ExecutionControlsTypeDef],  # (3)
    MaximumAutomaticAttempts: NotRequired[int],
    RetryAttemptSeconds: NotRequired[int],
    Arn: NotRequired[str],
    CreatedByService: NotRequired[str],
```

1. See [:material-code-brackets: RemediationTargetTypeType](./literals.md#remediationtargettypetype) 
2. See [:material-code-braces: RemediationParameterValueTypeDef](./type_defs.md#remediationparametervaluetypedef) [:material-code-braces: RemediationParameterValueOutputTypeDef](./type_defs.md#remediationparametervalueoutputtypedef) 
3. See [:material-code-braces: ExecutionControlsTypeDef](./type_defs.md#executioncontrolstypedef) 
## PutRemediationConfigurationsRequestTypeDef

```python
# PutRemediationConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_config.type_defs import PutRemediationConfigurationsRequestTypeDef


def get_value() -> PutRemediationConfigurationsRequestTypeDef:
    return {
        "RemediationConfigurations": ...,
    }


# PutRemediationConfigurationsRequestTypeDef definition

class PutRemediationConfigurationsRequestTypeDef(TypedDict):
    RemediationConfigurations: Sequence[RemediationConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: RemediationConfigurationTypeDef](./type_defs.md#remediationconfigurationtypedef) [:material-code-braces: RemediationConfigurationOutputTypeDef](./type_defs.md#remediationconfigurationoutputtypedef) 

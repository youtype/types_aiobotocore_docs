# Type definitions

> [Index](../README.md) > [LicenseManager](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LicenseManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#licensemanager)
    type annotations stubs module [types-aiobotocore-license-manager](https://pypi.org/project/types-aiobotocore-license-manager/).

## ProductInformationFilterUnionTypeDef

```python
# ProductInformationFilterUnionTypeDef Union usage example

from types_aiobotocore_license_manager.type_defs import ProductInformationFilterUnionTypeDef


def get_value() -> ProductInformationFilterUnionTypeDef:
    return ...


# ProductInformationFilterUnionTypeDef definition

ProductInformationFilterUnionTypeDef = Union[
    ProductInformationFilterTypeDef,  # (1)
    ProductInformationFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProductInformationFilterTypeDef](./type_defs.md#productinformationfiltertypedef) 
2. See [:material-code-braces: ProductInformationFilterOutputTypeDef](./type_defs.md#productinformationfilteroutputtypedef) 

## ReportContextUnionTypeDef

```python
# ReportContextUnionTypeDef Union usage example

from types_aiobotocore_license_manager.type_defs import ReportContextUnionTypeDef


def get_value() -> ReportContextUnionTypeDef:
    return ...


# ReportContextUnionTypeDef definition

ReportContextUnionTypeDef = Union[
    ReportContextTypeDef,  # (1)
    ReportContextOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ReportContextTypeDef](./type_defs.md#reportcontexttypedef) 
2. See [:material-code-braces: ReportContextOutputTypeDef](./type_defs.md#reportcontextoutputtypedef) 

## ProductInformationUnionTypeDef

```python
# ProductInformationUnionTypeDef Union usage example

from types_aiobotocore_license_manager.type_defs import ProductInformationUnionTypeDef


def get_value() -> ProductInformationUnionTypeDef:
    return ...


# ProductInformationUnionTypeDef definition

ProductInformationUnionTypeDef = Union[
    ProductInformationTypeDef,  # (1)
    ProductInformationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProductInformationTypeDef](./type_defs.md#productinformationtypedef) 
2. See [:material-code-braces: ProductInformationOutputTypeDef](./type_defs.md#productinformationoutputtypedef) 



## AcceptGrantRequestTypeDef

```python
# AcceptGrantRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import AcceptGrantRequestTypeDef


def get_value() -> AcceptGrantRequestTypeDef:
    return {
        "GrantArn": ...,
    }


# AcceptGrantRequestTypeDef definition

class AcceptGrantRequestTypeDef(TypedDict):
    GrantArn: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ResponseMetadataTypeDef


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

## AutomatedDiscoveryInformationTypeDef

```python
# AutomatedDiscoveryInformationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import AutomatedDiscoveryInformationTypeDef


def get_value() -> AutomatedDiscoveryInformationTypeDef:
    return {
        "LastRunTime": ...,
    }


# AutomatedDiscoveryInformationTypeDef definition

class AutomatedDiscoveryInformationTypeDef(TypedDict):
    LastRunTime: NotRequired[datetime],
```

## BorrowConfigurationTypeDef

```python
# BorrowConfigurationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import BorrowConfigurationTypeDef


def get_value() -> BorrowConfigurationTypeDef:
    return {
        "AllowEarlyCheckIn": ...,
    }


# BorrowConfigurationTypeDef definition

class BorrowConfigurationTypeDef(TypedDict):
    AllowEarlyCheckIn: bool,
    MaxTimeToLiveInMinutes: int,
```

## CheckInLicenseRequestTypeDef

```python
# CheckInLicenseRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CheckInLicenseRequestTypeDef


def get_value() -> CheckInLicenseRequestTypeDef:
    return {
        "LicenseConsumptionToken": ...,
    }


# CheckInLicenseRequestTypeDef definition

class CheckInLicenseRequestTypeDef(TypedDict):
    LicenseConsumptionToken: str,
    Beneficiary: NotRequired[str],
```

## EntitlementDataTypeDef

```python
# EntitlementDataTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import EntitlementDataTypeDef


def get_value() -> EntitlementDataTypeDef:
    return {
        "Name": ...,
    }


# EntitlementDataTypeDef definition

class EntitlementDataTypeDef(TypedDict):
    Name: str,
    Unit: EntitlementDataUnitType,  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: EntitlementDataUnitType](./literals.md#entitlementdataunittype) 
## MetadataTypeDef

```python
# MetadataTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import MetadataTypeDef


def get_value() -> MetadataTypeDef:
    return {
        "Name": ...,
    }


# MetadataTypeDef definition

class MetadataTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
```

## ConsumedLicenseSummaryTypeDef

```python
# ConsumedLicenseSummaryTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ConsumedLicenseSummaryTypeDef


def get_value() -> ConsumedLicenseSummaryTypeDef:
    return {
        "ResourceType": ...,
    }


# ConsumedLicenseSummaryTypeDef definition

class ConsumedLicenseSummaryTypeDef(TypedDict):
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    ConsumedLicenses: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ProvisionalConfigurationTypeDef

```python
# ProvisionalConfigurationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ProvisionalConfigurationTypeDef


def get_value() -> ProvisionalConfigurationTypeDef:
    return {
        "MaxTimeToLiveInMinutes": ...,
    }


# ProvisionalConfigurationTypeDef definition

class ProvisionalConfigurationTypeDef(TypedDict):
    MaxTimeToLiveInMinutes: int,
```

## CreateGrantRequestTypeDef

```python
# CreateGrantRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateGrantRequestTypeDef


def get_value() -> CreateGrantRequestTypeDef:
    return {
        "ClientToken": ...,
    }


# CreateGrantRequestTypeDef definition

class CreateGrantRequestTypeDef(TypedDict):
    ClientToken: str,
    GrantName: str,
    LicenseArn: str,
    Principals: Sequence[str],
    HomeRegion: str,
    AllowedOperations: Sequence[AllowedOperationType],  # (1)
```

1. See [:material-code-brackets: AllowedOperationType](./literals.md#allowedoperationtype) 
## OptionsTypeDef

```python
# OptionsTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import OptionsTypeDef


def get_value() -> OptionsTypeDef:
    return {
        "ActivationOverrideBehavior": ...,
    }


# OptionsTypeDef definition

class OptionsTypeDef(TypedDict):
    ActivationOverrideBehavior: NotRequired[ActivationOverrideBehaviorType],  # (1)
```

1. See [:material-code-brackets: ActivationOverrideBehaviorType](./literals.md#activationoverridebehaviortype) 
## TagTypeDef

```python
# TagTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import TagTypeDef


def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }


# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## LicenseConversionContextTypeDef

```python
# LicenseConversionContextTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseConversionContextTypeDef


def get_value() -> LicenseConversionContextTypeDef:
    return {
        "UsageOperation": ...,
    }


# LicenseConversionContextTypeDef definition

class LicenseConversionContextTypeDef(TypedDict):
    UsageOperation: NotRequired[str],
```

## ReportFrequencyTypeDef

```python
# ReportFrequencyTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ReportFrequencyTypeDef


def get_value() -> ReportFrequencyTypeDef:
    return {
        "value": ...,
    }


# ReportFrequencyTypeDef definition

class ReportFrequencyTypeDef(TypedDict):
    value: NotRequired[int],
    period: NotRequired[ReportFrequencyTypeType],  # (1)
```

1. See [:material-code-brackets: ReportFrequencyTypeType](./literals.md#reportfrequencytypetype) 
## DatetimeRangeTypeDef

```python
# DatetimeRangeTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import DatetimeRangeTypeDef


def get_value() -> DatetimeRangeTypeDef:
    return {
        "Begin": ...,
    }


# DatetimeRangeTypeDef definition

class DatetimeRangeTypeDef(TypedDict):
    Begin: str,
    End: NotRequired[str],
```

## EntitlementTypeDef

```python
# EntitlementTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import EntitlementTypeDef


def get_value() -> EntitlementTypeDef:
    return {
        "Name": ...,
    }


# EntitlementTypeDef definition

class EntitlementTypeDef(TypedDict):
    Name: str,
    Unit: EntitlementUnitType,  # (1)
    Value: NotRequired[str],
    MaxCount: NotRequired[int],
    Overage: NotRequired[bool],
    AllowCheckIn: NotRequired[bool],
```

1. See [:material-code-brackets: EntitlementUnitType](./literals.md#entitlementunittype) 
## IssuerTypeDef

```python
# IssuerTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import IssuerTypeDef


def get_value() -> IssuerTypeDef:
    return {
        "Name": ...,
    }


# IssuerTypeDef definition

class IssuerTypeDef(TypedDict):
    Name: str,
    SignKey: NotRequired[str],
```

## CreateTokenRequestTypeDef

```python
# CreateTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateTokenRequestTypeDef


def get_value() -> CreateTokenRequestTypeDef:
    return {
        "LicenseArn": ...,
    }


# CreateTokenRequestTypeDef definition

class CreateTokenRequestTypeDef(TypedDict):
    LicenseArn: str,
    ClientToken: str,
    RoleArns: NotRequired[Sequence[str]],
    ExpirationInDays: NotRequired[int],
    TokenProperties: NotRequired[Sequence[str]],
```

## DeleteGrantRequestTypeDef

```python
# DeleteGrantRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import DeleteGrantRequestTypeDef


def get_value() -> DeleteGrantRequestTypeDef:
    return {
        "GrantArn": ...,
    }


# DeleteGrantRequestTypeDef definition

class DeleteGrantRequestTypeDef(TypedDict):
    GrantArn: str,
    Version: str,
    StatusReason: NotRequired[str],
```

## DeleteLicenseConfigurationRequestTypeDef

```python
# DeleteLicenseConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import DeleteLicenseConfigurationRequestTypeDef


def get_value() -> DeleteLicenseConfigurationRequestTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# DeleteLicenseConfigurationRequestTypeDef definition

class DeleteLicenseConfigurationRequestTypeDef(TypedDict):
    LicenseConfigurationArn: str,
```

## DeleteLicenseManagerReportGeneratorRequestTypeDef

```python
# DeleteLicenseManagerReportGeneratorRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import DeleteLicenseManagerReportGeneratorRequestTypeDef


def get_value() -> DeleteLicenseManagerReportGeneratorRequestTypeDef:
    return {
        "LicenseManagerReportGeneratorArn": ...,
    }


# DeleteLicenseManagerReportGeneratorRequestTypeDef definition

class DeleteLicenseManagerReportGeneratorRequestTypeDef(TypedDict):
    LicenseManagerReportGeneratorArn: str,
```

## DeleteLicenseRequestTypeDef

```python
# DeleteLicenseRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import DeleteLicenseRequestTypeDef


def get_value() -> DeleteLicenseRequestTypeDef:
    return {
        "LicenseArn": ...,
    }


# DeleteLicenseRequestTypeDef definition

class DeleteLicenseRequestTypeDef(TypedDict):
    LicenseArn: str,
    SourceVersion: str,
```

## DeleteTokenRequestTypeDef

```python
# DeleteTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import DeleteTokenRequestTypeDef


def get_value() -> DeleteTokenRequestTypeDef:
    return {
        "TokenId": ...,
    }


# DeleteTokenRequestTypeDef definition

class DeleteTokenRequestTypeDef(TypedDict):
    TokenId: str,
```

## EntitlementUsageTypeDef

```python
# EntitlementUsageTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import EntitlementUsageTypeDef


def get_value() -> EntitlementUsageTypeDef:
    return {
        "Name": ...,
    }


# EntitlementUsageTypeDef definition

class EntitlementUsageTypeDef(TypedDict):
    Name: str,
    ConsumedValue: str,
    Unit: EntitlementDataUnitType,  # (1)
    MaxCount: NotRequired[str],
```

1. See [:material-code-brackets: EntitlementDataUnitType](./literals.md#entitlementdataunittype) 
## ExtendLicenseConsumptionRequestTypeDef

```python
# ExtendLicenseConsumptionRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ExtendLicenseConsumptionRequestTypeDef


def get_value() -> ExtendLicenseConsumptionRequestTypeDef:
    return {
        "LicenseConsumptionToken": ...,
    }


# ExtendLicenseConsumptionRequestTypeDef definition

class ExtendLicenseConsumptionRequestTypeDef(TypedDict):
    LicenseConsumptionToken: str,
    DryRun: NotRequired[bool],
```

## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "Name": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    Name: NotRequired[str],
    Values: NotRequired[Sequence[str]],
```

## GetAccessTokenRequestTypeDef

```python
# GetAccessTokenRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetAccessTokenRequestTypeDef


def get_value() -> GetAccessTokenRequestTypeDef:
    return {
        "Token": ...,
    }


# GetAccessTokenRequestTypeDef definition

class GetAccessTokenRequestTypeDef(TypedDict):
    Token: str,
    TokenProperties: NotRequired[Sequence[str]],
```

## GetGrantRequestTypeDef

```python
# GetGrantRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetGrantRequestTypeDef


def get_value() -> GetGrantRequestTypeDef:
    return {
        "GrantArn": ...,
    }


# GetGrantRequestTypeDef definition

class GetGrantRequestTypeDef(TypedDict):
    GrantArn: str,
    Version: NotRequired[str],
```

## GetLicenseConfigurationRequestTypeDef

```python
# GetLicenseConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseConfigurationRequestTypeDef


def get_value() -> GetLicenseConfigurationRequestTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# GetLicenseConfigurationRequestTypeDef definition

class GetLicenseConfigurationRequestTypeDef(TypedDict):
    LicenseConfigurationArn: str,
```

## ManagedResourceSummaryTypeDef

```python
# ManagedResourceSummaryTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ManagedResourceSummaryTypeDef


def get_value() -> ManagedResourceSummaryTypeDef:
    return {
        "ResourceType": ...,
    }


# ManagedResourceSummaryTypeDef definition

class ManagedResourceSummaryTypeDef(TypedDict):
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    AssociationCount: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## GetLicenseConversionTaskRequestTypeDef

```python
# GetLicenseConversionTaskRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseConversionTaskRequestTypeDef


def get_value() -> GetLicenseConversionTaskRequestTypeDef:
    return {
        "LicenseConversionTaskId": ...,
    }


# GetLicenseConversionTaskRequestTypeDef definition

class GetLicenseConversionTaskRequestTypeDef(TypedDict):
    LicenseConversionTaskId: str,
```

## GetLicenseManagerReportGeneratorRequestTypeDef

```python
# GetLicenseManagerReportGeneratorRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseManagerReportGeneratorRequestTypeDef


def get_value() -> GetLicenseManagerReportGeneratorRequestTypeDef:
    return {
        "LicenseManagerReportGeneratorArn": ...,
    }


# GetLicenseManagerReportGeneratorRequestTypeDef definition

class GetLicenseManagerReportGeneratorRequestTypeDef(TypedDict):
    LicenseManagerReportGeneratorArn: str,
```

## GetLicenseRequestTypeDef

```python
# GetLicenseRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseRequestTypeDef


def get_value() -> GetLicenseRequestTypeDef:
    return {
        "LicenseArn": ...,
    }


# GetLicenseRequestTypeDef definition

class GetLicenseRequestTypeDef(TypedDict):
    LicenseArn: str,
    Version: NotRequired[str],
```

## GetLicenseUsageRequestTypeDef

```python
# GetLicenseUsageRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseUsageRequestTypeDef


def get_value() -> GetLicenseUsageRequestTypeDef:
    return {
        "LicenseArn": ...,
    }


# GetLicenseUsageRequestTypeDef definition

class GetLicenseUsageRequestTypeDef(TypedDict):
    LicenseArn: str,
```

## OrganizationConfigurationTypeDef

```python
# OrganizationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import OrganizationConfigurationTypeDef


def get_value() -> OrganizationConfigurationTypeDef:
    return {
        "EnableIntegration": ...,
    }


# OrganizationConfigurationTypeDef definition

class OrganizationConfigurationTypeDef(TypedDict):
    EnableIntegration: bool,
```

## IssuerDetailsTypeDef

```python
# IssuerDetailsTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import IssuerDetailsTypeDef


def get_value() -> IssuerDetailsTypeDef:
    return {
        "Name": ...,
    }


# IssuerDetailsTypeDef definition

class IssuerDetailsTypeDef(TypedDict):
    Name: NotRequired[str],
    SignKey: NotRequired[str],
    KeyFingerprint: NotRequired[str],
```

## ReceivedMetadataTypeDef

```python
# ReceivedMetadataTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ReceivedMetadataTypeDef


def get_value() -> ReceivedMetadataTypeDef:
    return {
        "ReceivedStatus": ...,
    }


# ReceivedMetadataTypeDef definition

class ReceivedMetadataTypeDef(TypedDict):
    ReceivedStatus: NotRequired[ReceivedStatusType],  # (1)
    ReceivedStatusReason: NotRequired[str],
    AllowedOperations: NotRequired[List[AllowedOperationType]],  # (2)
```

1. See [:material-code-brackets: ReceivedStatusType](./literals.md#receivedstatustype) 
2. See [:material-code-brackets: AllowedOperationType](./literals.md#allowedoperationtype) 
## InventoryFilterTypeDef

```python
# InventoryFilterTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import InventoryFilterTypeDef


def get_value() -> InventoryFilterTypeDef:
    return {
        "Name": ...,
    }


# InventoryFilterTypeDef definition

class InventoryFilterTypeDef(TypedDict):
    Name: str,
    Condition: InventoryFilterConditionType,  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: InventoryFilterConditionType](./literals.md#inventoryfilterconditiontype) 
## LicenseConfigurationAssociationTypeDef

```python
# LicenseConfigurationAssociationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseConfigurationAssociationTypeDef


def get_value() -> LicenseConfigurationAssociationTypeDef:
    return {
        "ResourceArn": ...,
    }


# LicenseConfigurationAssociationTypeDef definition

class LicenseConfigurationAssociationTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    ResourceOwnerId: NotRequired[str],
    AssociationTime: NotRequired[datetime],
    AmiAssociationScope: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## LicenseConfigurationUsageTypeDef

```python
# LicenseConfigurationUsageTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseConfigurationUsageTypeDef


def get_value() -> LicenseConfigurationUsageTypeDef:
    return {
        "ResourceArn": ...,
    }


# LicenseConfigurationUsageTypeDef definition

class LicenseConfigurationUsageTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    ResourceStatus: NotRequired[str],
    ResourceOwnerId: NotRequired[str],
    AssociationTime: NotRequired[datetime],
    ConsumedLicenses: NotRequired[int],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## LicenseSpecificationTypeDef

```python
# LicenseSpecificationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseSpecificationTypeDef


def get_value() -> LicenseSpecificationTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# LicenseSpecificationTypeDef definition

class LicenseSpecificationTypeDef(TypedDict):
    LicenseConfigurationArn: str,
    AmiAssociationScope: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import PaginatorConfigTypeDef


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

## ListAssociationsForLicenseConfigurationRequestTypeDef

```python
# ListAssociationsForLicenseConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListAssociationsForLicenseConfigurationRequestTypeDef


def get_value() -> ListAssociationsForLicenseConfigurationRequestTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# ListAssociationsForLicenseConfigurationRequestTypeDef definition

class ListAssociationsForLicenseConfigurationRequestTypeDef(TypedDict):
    LicenseConfigurationArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListFailuresForLicenseConfigurationOperationsRequestTypeDef

```python
# ListFailuresForLicenseConfigurationOperationsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListFailuresForLicenseConfigurationOperationsRequestTypeDef


def get_value() -> ListFailuresForLicenseConfigurationOperationsRequestTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# ListFailuresForLicenseConfigurationOperationsRequestTypeDef definition

class ListFailuresForLicenseConfigurationOperationsRequestTypeDef(TypedDict):
    LicenseConfigurationArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLicenseSpecificationsForResourceRequestTypeDef

```python
# ListLicenseSpecificationsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseSpecificationsForResourceRequestTypeDef


def get_value() -> ListLicenseSpecificationsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListLicenseSpecificationsForResourceRequestTypeDef definition

class ListLicenseSpecificationsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLicenseVersionsRequestTypeDef

```python
# ListLicenseVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseVersionsRequestTypeDef


def get_value() -> ListLicenseVersionsRequestTypeDef:
    return {
        "LicenseArn": ...,
    }


# ListLicenseVersionsRequestTypeDef definition

class ListLicenseVersionsRequestTypeDef(TypedDict):
    LicenseArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ResourceInventoryTypeDef

```python
# ResourceInventoryTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ResourceInventoryTypeDef


def get_value() -> ResourceInventoryTypeDef:
    return {
        "ResourceId": ...,
    }


# ResourceInventoryTypeDef definition

class ResourceInventoryTypeDef(TypedDict):
    ResourceId: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    ResourceArn: NotRequired[str],
    Platform: NotRequired[str],
    PlatformVersion: NotRequired[str],
    ResourceOwningAccountId: NotRequired[str],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TokenDataTypeDef

```python
# TokenDataTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import TokenDataTypeDef


def get_value() -> TokenDataTypeDef:
    return {
        "TokenId": ...,
    }


# TokenDataTypeDef definition

class TokenDataTypeDef(TypedDict):
    TokenId: NotRequired[str],
    TokenType: NotRequired[str],
    LicenseArn: NotRequired[str],
    ExpirationTime: NotRequired[str],
    TokenProperties: NotRequired[List[str]],
    RoleArns: NotRequired[List[str]],
    Status: NotRequired[str],
```

## ProductInformationFilterOutputTypeDef

```python
# ProductInformationFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ProductInformationFilterOutputTypeDef


def get_value() -> ProductInformationFilterOutputTypeDef:
    return {
        "ProductInformationFilterName": ...,
    }


# ProductInformationFilterOutputTypeDef definition

class ProductInformationFilterOutputTypeDef(TypedDict):
    ProductInformationFilterName: str,
    ProductInformationFilterComparator: str,
    ProductInformationFilterValue: NotRequired[List[str]],
```

## ProductInformationFilterTypeDef

```python
# ProductInformationFilterTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ProductInformationFilterTypeDef


def get_value() -> ProductInformationFilterTypeDef:
    return {
        "ProductInformationFilterName": ...,
    }


# ProductInformationFilterTypeDef definition

class ProductInformationFilterTypeDef(TypedDict):
    ProductInformationFilterName: str,
    ProductInformationFilterComparator: str,
    ProductInformationFilterValue: NotRequired[Sequence[str]],
```

## RejectGrantRequestTypeDef

```python
# RejectGrantRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import RejectGrantRequestTypeDef


def get_value() -> RejectGrantRequestTypeDef:
    return {
        "GrantArn": ...,
    }


# RejectGrantRequestTypeDef definition

class RejectGrantRequestTypeDef(TypedDict):
    GrantArn: str,
```

## ReportContextOutputTypeDef

```python
# ReportContextOutputTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ReportContextOutputTypeDef


def get_value() -> ReportContextOutputTypeDef:
    return {
        "licenseConfigurationArns": ...,
    }


# ReportContextOutputTypeDef definition

class ReportContextOutputTypeDef(TypedDict):
    licenseConfigurationArns: List[str],
```

## ReportContextTypeDef

```python
# ReportContextTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ReportContextTypeDef


def get_value() -> ReportContextTypeDef:
    return {
        "licenseConfigurationArns": ...,
    }


# ReportContextTypeDef definition

class ReportContextTypeDef(TypedDict):
    licenseConfigurationArns: Sequence[str],
```

## S3LocationTypeDef

```python
# S3LocationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import S3LocationTypeDef


def get_value() -> S3LocationTypeDef:
    return {
        "bucket": ...,
    }


# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    bucket: NotRequired[str],
    keyPrefix: NotRequired[str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## AcceptGrantResponseTypeDef

```python
# AcceptGrantResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import AcceptGrantResponseTypeDef


def get_value() -> AcceptGrantResponseTypeDef:
    return {
        "GrantArn": ...,
    }


# AcceptGrantResponseTypeDef definition

class AcceptGrantResponseTypeDef(TypedDict):
    GrantArn: str,
    Status: GrantStatusType,  # (1)
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GrantStatusType](./literals.md#grantstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGrantResponseTypeDef

```python
# CreateGrantResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateGrantResponseTypeDef


def get_value() -> CreateGrantResponseTypeDef:
    return {
        "GrantArn": ...,
    }


# CreateGrantResponseTypeDef definition

class CreateGrantResponseTypeDef(TypedDict):
    GrantArn: str,
    Status: GrantStatusType,  # (1)
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GrantStatusType](./literals.md#grantstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGrantVersionResponseTypeDef

```python
# CreateGrantVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateGrantVersionResponseTypeDef


def get_value() -> CreateGrantVersionResponseTypeDef:
    return {
        "GrantArn": ...,
    }


# CreateGrantVersionResponseTypeDef definition

class CreateGrantVersionResponseTypeDef(TypedDict):
    GrantArn: str,
    Status: GrantStatusType,  # (1)
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GrantStatusType](./literals.md#grantstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseConfigurationResponseTypeDef

```python
# CreateLicenseConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseConfigurationResponseTypeDef


def get_value() -> CreateLicenseConfigurationResponseTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# CreateLicenseConfigurationResponseTypeDef definition

class CreateLicenseConfigurationResponseTypeDef(TypedDict):
    LicenseConfigurationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseConversionTaskForResourceResponseTypeDef

```python
# CreateLicenseConversionTaskForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseConversionTaskForResourceResponseTypeDef


def get_value() -> CreateLicenseConversionTaskForResourceResponseTypeDef:
    return {
        "LicenseConversionTaskId": ...,
    }


# CreateLicenseConversionTaskForResourceResponseTypeDef definition

class CreateLicenseConversionTaskForResourceResponseTypeDef(TypedDict):
    LicenseConversionTaskId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseManagerReportGeneratorResponseTypeDef

```python
# CreateLicenseManagerReportGeneratorResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseManagerReportGeneratorResponseTypeDef


def get_value() -> CreateLicenseManagerReportGeneratorResponseTypeDef:
    return {
        "LicenseManagerReportGeneratorArn": ...,
    }


# CreateLicenseManagerReportGeneratorResponseTypeDef definition

class CreateLicenseManagerReportGeneratorResponseTypeDef(TypedDict):
    LicenseManagerReportGeneratorArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseResponseTypeDef

```python
# CreateLicenseResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseResponseTypeDef


def get_value() -> CreateLicenseResponseTypeDef:
    return {
        "LicenseArn": ...,
    }


# CreateLicenseResponseTypeDef definition

class CreateLicenseResponseTypeDef(TypedDict):
    LicenseArn: str,
    Status: LicenseStatusType,  # (1)
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LicenseStatusType](./literals.md#licensestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseVersionResponseTypeDef

```python
# CreateLicenseVersionResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseVersionResponseTypeDef


def get_value() -> CreateLicenseVersionResponseTypeDef:
    return {
        "LicenseArn": ...,
    }


# CreateLicenseVersionResponseTypeDef definition

class CreateLicenseVersionResponseTypeDef(TypedDict):
    LicenseArn: str,
    Version: str,
    Status: LicenseStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LicenseStatusType](./literals.md#licensestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTokenResponseTypeDef

```python
# CreateTokenResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateTokenResponseTypeDef


def get_value() -> CreateTokenResponseTypeDef:
    return {
        "TokenId": ...,
    }


# CreateTokenResponseTypeDef definition

class CreateTokenResponseTypeDef(TypedDict):
    TokenId: str,
    TokenType: TokenTypeType,  # (1)
    Token: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TokenTypeType](./literals.md#tokentypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGrantResponseTypeDef

```python
# DeleteGrantResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import DeleteGrantResponseTypeDef


def get_value() -> DeleteGrantResponseTypeDef:
    return {
        "GrantArn": ...,
    }


# DeleteGrantResponseTypeDef definition

class DeleteGrantResponseTypeDef(TypedDict):
    GrantArn: str,
    Status: GrantStatusType,  # (1)
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GrantStatusType](./literals.md#grantstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteLicenseResponseTypeDef

```python
# DeleteLicenseResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import DeleteLicenseResponseTypeDef


def get_value() -> DeleteLicenseResponseTypeDef:
    return {
        "Status": ...,
    }


# DeleteLicenseResponseTypeDef definition

class DeleteLicenseResponseTypeDef(TypedDict):
    Status: LicenseDeletionStatusType,  # (1)
    DeletionDate: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LicenseDeletionStatusType](./literals.md#licensedeletionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExtendLicenseConsumptionResponseTypeDef

```python
# ExtendLicenseConsumptionResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ExtendLicenseConsumptionResponseTypeDef


def get_value() -> ExtendLicenseConsumptionResponseTypeDef:
    return {
        "LicenseConsumptionToken": ...,
    }


# ExtendLicenseConsumptionResponseTypeDef definition

class ExtendLicenseConsumptionResponseTypeDef(TypedDict):
    LicenseConsumptionToken: str,
    Expiration: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAccessTokenResponseTypeDef

```python
# GetAccessTokenResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetAccessTokenResponseTypeDef


def get_value() -> GetAccessTokenResponseTypeDef:
    return {
        "AccessToken": ...,
    }


# GetAccessTokenResponseTypeDef definition

class GetAccessTokenResponseTypeDef(TypedDict):
    AccessToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectGrantResponseTypeDef

```python
# RejectGrantResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import RejectGrantResponseTypeDef


def get_value() -> RejectGrantResponseTypeDef:
    return {
        "GrantArn": ...,
    }


# RejectGrantResponseTypeDef definition

class RejectGrantResponseTypeDef(TypedDict):
    GrantArn: str,
    Status: GrantStatusType,  # (1)
    Version: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GrantStatusType](./literals.md#grantstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CheckoutLicenseRequestTypeDef

```python
# CheckoutLicenseRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CheckoutLicenseRequestTypeDef


def get_value() -> CheckoutLicenseRequestTypeDef:
    return {
        "ProductSKU": ...,
    }


# CheckoutLicenseRequestTypeDef definition

class CheckoutLicenseRequestTypeDef(TypedDict):
    ProductSKU: str,
    CheckoutType: CheckoutTypeType,  # (1)
    KeyFingerprint: str,
    Entitlements: Sequence[EntitlementDataTypeDef],  # (2)
    ClientToken: str,
    Beneficiary: NotRequired[str],
    NodeId: NotRequired[str],
```

1. See [:material-code-brackets: CheckoutTypeType](./literals.md#checkouttypetype) 
2. See [:material-code-braces: EntitlementDataTypeDef](./type_defs.md#entitlementdatatypedef) 
## CheckoutLicenseResponseTypeDef

```python
# CheckoutLicenseResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CheckoutLicenseResponseTypeDef


def get_value() -> CheckoutLicenseResponseTypeDef:
    return {
        "CheckoutType": ...,
    }


# CheckoutLicenseResponseTypeDef definition

class CheckoutLicenseResponseTypeDef(TypedDict):
    CheckoutType: CheckoutTypeType,  # (1)
    LicenseConsumptionToken: str,
    EntitlementsAllowed: List[EntitlementDataTypeDef],  # (2)
    SignedToken: str,
    NodeId: str,
    IssuedAt: str,
    Expiration: str,
    LicenseArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: CheckoutTypeType](./literals.md#checkouttypetype) 
2. See [:material-code-braces: EntitlementDataTypeDef](./type_defs.md#entitlementdatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CheckoutBorrowLicenseRequestTypeDef

```python
# CheckoutBorrowLicenseRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CheckoutBorrowLicenseRequestTypeDef


def get_value() -> CheckoutBorrowLicenseRequestTypeDef:
    return {
        "LicenseArn": ...,
    }


# CheckoutBorrowLicenseRequestTypeDef definition

class CheckoutBorrowLicenseRequestTypeDef(TypedDict):
    LicenseArn: str,
    Entitlements: Sequence[EntitlementDataTypeDef],  # (1)
    DigitalSignatureMethod: DigitalSignatureMethodType,  # (2)
    ClientToken: str,
    NodeId: NotRequired[str],
    CheckoutMetadata: NotRequired[Sequence[MetadataTypeDef]],  # (3)
```

1. See [:material-code-braces: EntitlementDataTypeDef](./type_defs.md#entitlementdatatypedef) 
2. See [:material-code-brackets: DigitalSignatureMethodType](./literals.md#digitalsignaturemethodtype) 
3. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
## CheckoutBorrowLicenseResponseTypeDef

```python
# CheckoutBorrowLicenseResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CheckoutBorrowLicenseResponseTypeDef


def get_value() -> CheckoutBorrowLicenseResponseTypeDef:
    return {
        "LicenseArn": ...,
    }


# CheckoutBorrowLicenseResponseTypeDef definition

class CheckoutBorrowLicenseResponseTypeDef(TypedDict):
    LicenseArn: str,
    LicenseConsumptionToken: str,
    EntitlementsAllowed: List[EntitlementDataTypeDef],  # (1)
    NodeId: str,
    SignedToken: str,
    IssuedAt: str,
    Expiration: str,
    CheckoutMetadata: List[MetadataTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EntitlementDataTypeDef](./type_defs.md#entitlementdatatypedef) 
2. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LicenseOperationFailureTypeDef

```python
# LicenseOperationFailureTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseOperationFailureTypeDef


def get_value() -> LicenseOperationFailureTypeDef:
    return {
        "ResourceArn": ...,
    }


# LicenseOperationFailureTypeDef definition

class LicenseOperationFailureTypeDef(TypedDict):
    ResourceArn: NotRequired[str],
    ResourceType: NotRequired[ResourceTypeType],  # (1)
    ErrorMessage: NotRequired[str],
    FailureTime: NotRequired[datetime],
    OperationName: NotRequired[str],
    ResourceOwnerId: NotRequired[str],
    OperationRequestedBy: NotRequired[str],
    MetadataList: NotRequired[List[MetadataTypeDef]],  # (2)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
## ConsumptionConfigurationTypeDef

```python
# ConsumptionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ConsumptionConfigurationTypeDef


def get_value() -> ConsumptionConfigurationTypeDef:
    return {
        "RenewType": ...,
    }


# ConsumptionConfigurationTypeDef definition

class ConsumptionConfigurationTypeDef(TypedDict):
    RenewType: NotRequired[RenewTypeType],  # (1)
    ProvisionalConfiguration: NotRequired[ProvisionalConfigurationTypeDef],  # (2)
    BorrowConfiguration: NotRequired[BorrowConfigurationTypeDef],  # (3)
```

1. See [:material-code-brackets: RenewTypeType](./literals.md#renewtypetype) 
2. See [:material-code-braces: ProvisionalConfigurationTypeDef](./type_defs.md#provisionalconfigurationtypedef) 
3. See [:material-code-braces: BorrowConfigurationTypeDef](./type_defs.md#borrowconfigurationtypedef) 
## CreateGrantVersionRequestTypeDef

```python
# CreateGrantVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateGrantVersionRequestTypeDef


def get_value() -> CreateGrantVersionRequestTypeDef:
    return {
        "ClientToken": ...,
    }


# CreateGrantVersionRequestTypeDef definition

class CreateGrantVersionRequestTypeDef(TypedDict):
    ClientToken: str,
    GrantArn: str,
    GrantName: NotRequired[str],
    AllowedOperations: NotRequired[Sequence[AllowedOperationType]],  # (1)
    Status: NotRequired[GrantStatusType],  # (2)
    StatusReason: NotRequired[str],
    SourceVersion: NotRequired[str],
    Options: NotRequired[OptionsTypeDef],  # (3)
```

1. See [:material-code-brackets: AllowedOperationType](./literals.md#allowedoperationtype) 
2. See [:material-code-brackets: GrantStatusType](./literals.md#grantstatustype) 
3. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
## GrantTypeDef

```python
# GrantTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GrantTypeDef


def get_value() -> GrantTypeDef:
    return {
        "GrantArn": ...,
    }


# GrantTypeDef definition

class GrantTypeDef(TypedDict):
    GrantArn: str,
    GrantName: str,
    ParentArn: str,
    LicenseArn: str,
    GranteePrincipalArn: str,
    HomeRegion: str,
    GrantStatus: GrantStatusType,  # (1)
    Version: str,
    GrantedOperations: List[AllowedOperationType],  # (2)
    StatusReason: NotRequired[str],
    Options: NotRequired[OptionsTypeDef],  # (3)
```

1. See [:material-code-brackets: GrantStatusType](./literals.md#grantstatustype) 
2. See [:material-code-brackets: AllowedOperationType](./literals.md#allowedoperationtype) 
3. See [:material-code-braces: OptionsTypeDef](./type_defs.md#optionstypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import TagResourceRequestTypeDef


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
## CreateLicenseConversionTaskForResourceRequestTypeDef

```python
# CreateLicenseConversionTaskForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseConversionTaskForResourceRequestTypeDef


def get_value() -> CreateLicenseConversionTaskForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# CreateLicenseConversionTaskForResourceRequestTypeDef definition

class CreateLicenseConversionTaskForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    SourceLicenseContext: LicenseConversionContextTypeDef,  # (1)
    DestinationLicenseContext: LicenseConversionContextTypeDef,  # (1)
```

1. See [:material-code-braces: LicenseConversionContextTypeDef](./type_defs.md#licenseconversioncontexttypedef) 
2. See [:material-code-braces: LicenseConversionContextTypeDef](./type_defs.md#licenseconversioncontexttypedef) 
## GetLicenseConversionTaskResponseTypeDef

```python
# GetLicenseConversionTaskResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseConversionTaskResponseTypeDef


def get_value() -> GetLicenseConversionTaskResponseTypeDef:
    return {
        "LicenseConversionTaskId": ...,
    }


# GetLicenseConversionTaskResponseTypeDef definition

class GetLicenseConversionTaskResponseTypeDef(TypedDict):
    LicenseConversionTaskId: str,
    ResourceArn: str,
    SourceLicenseContext: LicenseConversionContextTypeDef,  # (1)
    DestinationLicenseContext: LicenseConversionContextTypeDef,  # (1)
    StatusMessage: str,
    Status: LicenseConversionTaskStatusType,  # (3)
    StartTime: datetime,
    LicenseConversionTime: datetime,
    EndTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LicenseConversionContextTypeDef](./type_defs.md#licenseconversioncontexttypedef) 
2. See [:material-code-braces: LicenseConversionContextTypeDef](./type_defs.md#licenseconversioncontexttypedef) 
3. See [:material-code-brackets: LicenseConversionTaskStatusType](./literals.md#licenseconversiontaskstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LicenseConversionTaskTypeDef

```python
# LicenseConversionTaskTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseConversionTaskTypeDef


def get_value() -> LicenseConversionTaskTypeDef:
    return {
        "LicenseConversionTaskId": ...,
    }


# LicenseConversionTaskTypeDef definition

class LicenseConversionTaskTypeDef(TypedDict):
    LicenseConversionTaskId: NotRequired[str],
    ResourceArn: NotRequired[str],
    SourceLicenseContext: NotRequired[LicenseConversionContextTypeDef],  # (1)
    DestinationLicenseContext: NotRequired[LicenseConversionContextTypeDef],  # (1)
    Status: NotRequired[LicenseConversionTaskStatusType],  # (3)
    StatusMessage: NotRequired[str],
    StartTime: NotRequired[datetime],
    LicenseConversionTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
```

1. See [:material-code-braces: LicenseConversionContextTypeDef](./type_defs.md#licenseconversioncontexttypedef) 
2. See [:material-code-braces: LicenseConversionContextTypeDef](./type_defs.md#licenseconversioncontexttypedef) 
3. See [:material-code-brackets: LicenseConversionTaskStatusType](./literals.md#licenseconversiontaskstatustype) 
## LicenseUsageTypeDef

```python
# LicenseUsageTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseUsageTypeDef


def get_value() -> LicenseUsageTypeDef:
    return {
        "EntitlementUsages": ...,
    }


# LicenseUsageTypeDef definition

class LicenseUsageTypeDef(TypedDict):
    EntitlementUsages: NotRequired[List[EntitlementUsageTypeDef]],  # (1)
```

1. See [:material-code-braces: EntitlementUsageTypeDef](./type_defs.md#entitlementusagetypedef) 
## ListDistributedGrantsRequestTypeDef

```python
# ListDistributedGrantsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListDistributedGrantsRequestTypeDef


def get_value() -> ListDistributedGrantsRequestTypeDef:
    return {
        "GrantArns": ...,
    }


# ListDistributedGrantsRequestTypeDef definition

class ListDistributedGrantsRequestTypeDef(TypedDict):
    GrantArns: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListLicenseConfigurationsRequestTypeDef

```python
# ListLicenseConfigurationsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseConfigurationsRequestTypeDef


def get_value() -> ListLicenseConfigurationsRequestTypeDef:
    return {
        "LicenseConfigurationArns": ...,
    }


# ListLicenseConfigurationsRequestTypeDef definition

class ListLicenseConfigurationsRequestTypeDef(TypedDict):
    LicenseConfigurationArns: NotRequired[Sequence[str]],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListLicenseConversionTasksRequestTypeDef

```python
# ListLicenseConversionTasksRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseConversionTasksRequestTypeDef


def get_value() -> ListLicenseConversionTasksRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListLicenseConversionTasksRequestTypeDef definition

class ListLicenseConversionTasksRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListLicenseManagerReportGeneratorsRequestTypeDef

```python
# ListLicenseManagerReportGeneratorsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseManagerReportGeneratorsRequestTypeDef


def get_value() -> ListLicenseManagerReportGeneratorsRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListLicenseManagerReportGeneratorsRequestTypeDef definition

class ListLicenseManagerReportGeneratorsRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListLicensesRequestTypeDef

```python
# ListLicensesRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicensesRequestTypeDef


def get_value() -> ListLicensesRequestTypeDef:
    return {
        "LicenseArns": ...,
    }


# ListLicensesRequestTypeDef definition

class ListLicensesRequestTypeDef(TypedDict):
    LicenseArns: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListReceivedGrantsForOrganizationRequestTypeDef

```python
# ListReceivedGrantsForOrganizationRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListReceivedGrantsForOrganizationRequestTypeDef


def get_value() -> ListReceivedGrantsForOrganizationRequestTypeDef:
    return {
        "LicenseArn": ...,
    }


# ListReceivedGrantsForOrganizationRequestTypeDef definition

class ListReceivedGrantsForOrganizationRequestTypeDef(TypedDict):
    LicenseArn: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListReceivedGrantsRequestTypeDef

```python
# ListReceivedGrantsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListReceivedGrantsRequestTypeDef


def get_value() -> ListReceivedGrantsRequestTypeDef:
    return {
        "GrantArns": ...,
    }


# ListReceivedGrantsRequestTypeDef definition

class ListReceivedGrantsRequestTypeDef(TypedDict):
    GrantArns: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListReceivedLicensesForOrganizationRequestTypeDef

```python
# ListReceivedLicensesForOrganizationRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListReceivedLicensesForOrganizationRequestTypeDef


def get_value() -> ListReceivedLicensesForOrganizationRequestTypeDef:
    return {
        "Filters": ...,
    }


# ListReceivedLicensesForOrganizationRequestTypeDef definition

class ListReceivedLicensesForOrganizationRequestTypeDef(TypedDict):
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListReceivedLicensesRequestTypeDef

```python
# ListReceivedLicensesRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListReceivedLicensesRequestTypeDef


def get_value() -> ListReceivedLicensesRequestTypeDef:
    return {
        "LicenseArns": ...,
    }


# ListReceivedLicensesRequestTypeDef definition

class ListReceivedLicensesRequestTypeDef(TypedDict):
    LicenseArns: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListTokensRequestTypeDef

```python
# ListTokensRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListTokensRequestTypeDef


def get_value() -> ListTokensRequestTypeDef:
    return {
        "TokenIds": ...,
    }


# ListTokensRequestTypeDef definition

class ListTokensRequestTypeDef(TypedDict):
    TokenIds: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## ListUsageForLicenseConfigurationRequestTypeDef

```python
# ListUsageForLicenseConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListUsageForLicenseConfigurationRequestTypeDef


def get_value() -> ListUsageForLicenseConfigurationRequestTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# ListUsageForLicenseConfigurationRequestTypeDef definition

class ListUsageForLicenseConfigurationRequestTypeDef(TypedDict):
    LicenseConfigurationArn: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## GetServiceSettingsResponseTypeDef

```python
# GetServiceSettingsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetServiceSettingsResponseTypeDef


def get_value() -> GetServiceSettingsResponseTypeDef:
    return {
        "S3BucketArn": ...,
    }


# GetServiceSettingsResponseTypeDef definition

class GetServiceSettingsResponseTypeDef(TypedDict):
    S3BucketArn: str,
    SnsTopicArn: str,
    OrganizationConfiguration: OrganizationConfigurationTypeDef,  # (1)
    EnableCrossAccountsDiscovery: bool,
    LicenseManagerResourceShareArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationConfigurationTypeDef](./type_defs.md#organizationconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceSettingsRequestTypeDef

```python
# UpdateServiceSettingsRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import UpdateServiceSettingsRequestTypeDef


def get_value() -> UpdateServiceSettingsRequestTypeDef:
    return {
        "S3BucketArn": ...,
    }


# UpdateServiceSettingsRequestTypeDef definition

class UpdateServiceSettingsRequestTypeDef(TypedDict):
    S3BucketArn: NotRequired[str],
    SnsTopicArn: NotRequired[str],
    OrganizationConfiguration: NotRequired[OrganizationConfigurationTypeDef],  # (1)
    EnableCrossAccountsDiscovery: NotRequired[bool],
```

1. See [:material-code-braces: OrganizationConfigurationTypeDef](./type_defs.md#organizationconfigurationtypedef) 
## ListResourceInventoryRequestTypeDef

```python
# ListResourceInventoryRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListResourceInventoryRequestTypeDef


def get_value() -> ListResourceInventoryRequestTypeDef:
    return {
        "MaxResults": ...,
    }


# ListResourceInventoryRequestTypeDef definition

class ListResourceInventoryRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    Filters: NotRequired[Sequence[InventoryFilterTypeDef]],  # (1)
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
## ListAssociationsForLicenseConfigurationResponseTypeDef

```python
# ListAssociationsForLicenseConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListAssociationsForLicenseConfigurationResponseTypeDef


def get_value() -> ListAssociationsForLicenseConfigurationResponseTypeDef:
    return {
        "LicenseConfigurationAssociations": ...,
    }


# ListAssociationsForLicenseConfigurationResponseTypeDef definition

class ListAssociationsForLicenseConfigurationResponseTypeDef(TypedDict):
    LicenseConfigurationAssociations: List[LicenseConfigurationAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseConfigurationAssociationTypeDef](./type_defs.md#licenseconfigurationassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListUsageForLicenseConfigurationResponseTypeDef

```python
# ListUsageForLicenseConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListUsageForLicenseConfigurationResponseTypeDef


def get_value() -> ListUsageForLicenseConfigurationResponseTypeDef:
    return {
        "LicenseConfigurationUsageList": ...,
    }


# ListUsageForLicenseConfigurationResponseTypeDef definition

class ListUsageForLicenseConfigurationResponseTypeDef(TypedDict):
    LicenseConfigurationUsageList: List[LicenseConfigurationUsageTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseConfigurationUsageTypeDef](./type_defs.md#licenseconfigurationusagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicenseSpecificationsForResourceResponseTypeDef

```python
# ListLicenseSpecificationsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseSpecificationsForResourceResponseTypeDef


def get_value() -> ListLicenseSpecificationsForResourceResponseTypeDef:
    return {
        "LicenseSpecifications": ...,
    }


# ListLicenseSpecificationsForResourceResponseTypeDef definition

class ListLicenseSpecificationsForResourceResponseTypeDef(TypedDict):
    LicenseSpecifications: List[LicenseSpecificationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseSpecificationTypeDef](./type_defs.md#licensespecificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLicenseSpecificationsForResourceRequestTypeDef

```python
# UpdateLicenseSpecificationsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import UpdateLicenseSpecificationsForResourceRequestTypeDef


def get_value() -> UpdateLicenseSpecificationsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UpdateLicenseSpecificationsForResourceRequestTypeDef definition

class UpdateLicenseSpecificationsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    AddLicenseSpecifications: NotRequired[Sequence[LicenseSpecificationTypeDef]],  # (1)
    RemoveLicenseSpecifications: NotRequired[Sequence[LicenseSpecificationTypeDef]],  # (1)
```

1. See [:material-code-braces: LicenseSpecificationTypeDef](./type_defs.md#licensespecificationtypedef) 
2. See [:material-code-braces: LicenseSpecificationTypeDef](./type_defs.md#licensespecificationtypedef) 
## ListAssociationsForLicenseConfigurationRequestPaginateTypeDef

```python
# ListAssociationsForLicenseConfigurationRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListAssociationsForLicenseConfigurationRequestPaginateTypeDef


def get_value() -> ListAssociationsForLicenseConfigurationRequestPaginateTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# ListAssociationsForLicenseConfigurationRequestPaginateTypeDef definition

class ListAssociationsForLicenseConfigurationRequestPaginateTypeDef(TypedDict):
    LicenseConfigurationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLicenseConfigurationsRequestPaginateTypeDef

```python
# ListLicenseConfigurationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseConfigurationsRequestPaginateTypeDef


def get_value() -> ListLicenseConfigurationsRequestPaginateTypeDef:
    return {
        "LicenseConfigurationArns": ...,
    }


# ListLicenseConfigurationsRequestPaginateTypeDef definition

class ListLicenseConfigurationsRequestPaginateTypeDef(TypedDict):
    LicenseConfigurationArns: NotRequired[Sequence[str]],
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLicenseSpecificationsForResourceRequestPaginateTypeDef

```python
# ListLicenseSpecificationsForResourceRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseSpecificationsForResourceRequestPaginateTypeDef


def get_value() -> ListLicenseSpecificationsForResourceRequestPaginateTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListLicenseSpecificationsForResourceRequestPaginateTypeDef definition

class ListLicenseSpecificationsForResourceRequestPaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceInventoryRequestPaginateTypeDef

```python
# ListResourceInventoryRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListResourceInventoryRequestPaginateTypeDef


def get_value() -> ListResourceInventoryRequestPaginateTypeDef:
    return {
        "Filters": ...,
    }


# ListResourceInventoryRequestPaginateTypeDef definition

class ListResourceInventoryRequestPaginateTypeDef(TypedDict):
    Filters: NotRequired[Sequence[InventoryFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: InventoryFilterTypeDef](./type_defs.md#inventoryfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListUsageForLicenseConfigurationRequestPaginateTypeDef

```python
# ListUsageForLicenseConfigurationRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListUsageForLicenseConfigurationRequestPaginateTypeDef


def get_value() -> ListUsageForLicenseConfigurationRequestPaginateTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# ListUsageForLicenseConfigurationRequestPaginateTypeDef definition

class ListUsageForLicenseConfigurationRequestPaginateTypeDef(TypedDict):
    LicenseConfigurationArn: str,
    Filters: NotRequired[Sequence[FilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceInventoryResponseTypeDef

```python
# ListResourceInventoryResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListResourceInventoryResponseTypeDef


def get_value() -> ListResourceInventoryResponseTypeDef:
    return {
        "ResourceInventoryList": ...,
    }


# ListResourceInventoryResponseTypeDef definition

class ListResourceInventoryResponseTypeDef(TypedDict):
    ResourceInventoryList: List[ResourceInventoryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceInventoryTypeDef](./type_defs.md#resourceinventorytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTokensResponseTypeDef

```python
# ListTokensResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListTokensResponseTypeDef


def get_value() -> ListTokensResponseTypeDef:
    return {
        "Tokens": ...,
    }


# ListTokensResponseTypeDef definition

class ListTokensResponseTypeDef(TypedDict):
    Tokens: List[TokenDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TokenDataTypeDef](./type_defs.md#tokendatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProductInformationOutputTypeDef

```python
# ProductInformationOutputTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ProductInformationOutputTypeDef


def get_value() -> ProductInformationOutputTypeDef:
    return {
        "ResourceType": ...,
    }


# ProductInformationOutputTypeDef definition

class ProductInformationOutputTypeDef(TypedDict):
    ResourceType: str,
    ProductInformationFilterList: List[ProductInformationFilterOutputTypeDef],  # (1)
```

1. See [:material-code-braces: ProductInformationFilterOutputTypeDef](./type_defs.md#productinformationfilteroutputtypedef) 
## ReportGeneratorTypeDef

```python
# ReportGeneratorTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ReportGeneratorTypeDef


def get_value() -> ReportGeneratorTypeDef:
    return {
        "ReportGeneratorName": ...,
    }


# ReportGeneratorTypeDef definition

class ReportGeneratorTypeDef(TypedDict):
    ReportGeneratorName: NotRequired[str],
    ReportType: NotRequired[List[ReportTypeType]],  # (1)
    ReportContext: NotRequired[ReportContextOutputTypeDef],  # (2)
    ReportFrequency: NotRequired[ReportFrequencyTypeDef],  # (3)
    LicenseManagerReportGeneratorArn: NotRequired[str],
    LastRunStatus: NotRequired[str],
    LastRunFailureReason: NotRequired[str],
    LastReportGenerationTime: NotRequired[str],
    ReportCreatorAccount: NotRequired[str],
    Description: NotRequired[str],
    S3Location: NotRequired[S3LocationTypeDef],  # (4)
    CreateTime: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (5)
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ReportContextOutputTypeDef](./type_defs.md#reportcontextoutputtypedef) 
3. See [:material-code-braces: ReportFrequencyTypeDef](./type_defs.md#reportfrequencytypedef) 
4. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListFailuresForLicenseConfigurationOperationsResponseTypeDef

```python
# ListFailuresForLicenseConfigurationOperationsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListFailuresForLicenseConfigurationOperationsResponseTypeDef


def get_value() -> ListFailuresForLicenseConfigurationOperationsResponseTypeDef:
    return {
        "LicenseOperationFailureList": ...,
    }


# ListFailuresForLicenseConfigurationOperationsResponseTypeDef definition

class ListFailuresForLicenseConfigurationOperationsResponseTypeDef(TypedDict):
    LicenseOperationFailureList: List[LicenseOperationFailureTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseOperationFailureTypeDef](./type_defs.md#licenseoperationfailuretypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseRequestTypeDef

```python
# CreateLicenseRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseRequestTypeDef


def get_value() -> CreateLicenseRequestTypeDef:
    return {
        "LicenseName": ...,
    }


# CreateLicenseRequestTypeDef definition

class CreateLicenseRequestTypeDef(TypedDict):
    LicenseName: str,
    ProductName: str,
    ProductSKU: str,
    Issuer: IssuerTypeDef,  # (1)
    HomeRegion: str,
    Validity: DatetimeRangeTypeDef,  # (2)
    Entitlements: Sequence[EntitlementTypeDef],  # (3)
    Beneficiary: str,
    ConsumptionConfiguration: ConsumptionConfigurationTypeDef,  # (4)
    ClientToken: str,
    LicenseMetadata: NotRequired[Sequence[MetadataTypeDef]],  # (5)
```

1. See [:material-code-braces: IssuerTypeDef](./type_defs.md#issuertypedef) 
2. See [:material-code-braces: DatetimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
3. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
4. See [:material-code-braces: ConsumptionConfigurationTypeDef](./type_defs.md#consumptionconfigurationtypedef) 
5. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
## CreateLicenseVersionRequestTypeDef

```python
# CreateLicenseVersionRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseVersionRequestTypeDef


def get_value() -> CreateLicenseVersionRequestTypeDef:
    return {
        "LicenseArn": ...,
    }


# CreateLicenseVersionRequestTypeDef definition

class CreateLicenseVersionRequestTypeDef(TypedDict):
    LicenseArn: str,
    LicenseName: str,
    ProductName: str,
    Issuer: IssuerTypeDef,  # (1)
    HomeRegion: str,
    Validity: DatetimeRangeTypeDef,  # (2)
    Entitlements: Sequence[EntitlementTypeDef],  # (3)
    ConsumptionConfiguration: ConsumptionConfigurationTypeDef,  # (4)
    Status: LicenseStatusType,  # (5)
    ClientToken: str,
    LicenseMetadata: NotRequired[Sequence[MetadataTypeDef]],  # (6)
    SourceVersion: NotRequired[str],
```

1. See [:material-code-braces: IssuerTypeDef](./type_defs.md#issuertypedef) 
2. See [:material-code-braces: DatetimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
3. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
4. See [:material-code-braces: ConsumptionConfigurationTypeDef](./type_defs.md#consumptionconfigurationtypedef) 
5. See [:material-code-brackets: LicenseStatusType](./literals.md#licensestatustype) 
6. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
## GrantedLicenseTypeDef

```python
# GrantedLicenseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GrantedLicenseTypeDef


def get_value() -> GrantedLicenseTypeDef:
    return {
        "LicenseArn": ...,
    }


# GrantedLicenseTypeDef definition

class GrantedLicenseTypeDef(TypedDict):
    LicenseArn: NotRequired[str],
    LicenseName: NotRequired[str],
    ProductName: NotRequired[str],
    ProductSKU: NotRequired[str],
    Issuer: NotRequired[IssuerDetailsTypeDef],  # (1)
    HomeRegion: NotRequired[str],
    Status: NotRequired[LicenseStatusType],  # (2)
    Validity: NotRequired[DatetimeRangeTypeDef],  # (3)
    Beneficiary: NotRequired[str],
    Entitlements: NotRequired[List[EntitlementTypeDef]],  # (4)
    ConsumptionConfiguration: NotRequired[ConsumptionConfigurationTypeDef],  # (5)
    LicenseMetadata: NotRequired[List[MetadataTypeDef]],  # (6)
    CreateTime: NotRequired[str],
    Version: NotRequired[str],
    ReceivedMetadata: NotRequired[ReceivedMetadataTypeDef],  # (7)
```

1. See [:material-code-braces: IssuerDetailsTypeDef](./type_defs.md#issuerdetailstypedef) 
2. See [:material-code-brackets: LicenseStatusType](./literals.md#licensestatustype) 
3. See [:material-code-braces: DatetimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
4. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
5. See [:material-code-braces: ConsumptionConfigurationTypeDef](./type_defs.md#consumptionconfigurationtypedef) 
6. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
7. See [:material-code-braces: ReceivedMetadataTypeDef](./type_defs.md#receivedmetadatatypedef) 
## LicenseTypeDef

```python
# LicenseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseTypeDef


def get_value() -> LicenseTypeDef:
    return {
        "LicenseArn": ...,
    }


# LicenseTypeDef definition

class LicenseTypeDef(TypedDict):
    LicenseArn: NotRequired[str],
    LicenseName: NotRequired[str],
    ProductName: NotRequired[str],
    ProductSKU: NotRequired[str],
    Issuer: NotRequired[IssuerDetailsTypeDef],  # (1)
    HomeRegion: NotRequired[str],
    Status: NotRequired[LicenseStatusType],  # (2)
    Validity: NotRequired[DatetimeRangeTypeDef],  # (3)
    Beneficiary: NotRequired[str],
    Entitlements: NotRequired[List[EntitlementTypeDef]],  # (4)
    ConsumptionConfiguration: NotRequired[ConsumptionConfigurationTypeDef],  # (5)
    LicenseMetadata: NotRequired[List[MetadataTypeDef]],  # (6)
    CreateTime: NotRequired[str],
    Version: NotRequired[str],
```

1. See [:material-code-braces: IssuerDetailsTypeDef](./type_defs.md#issuerdetailstypedef) 
2. See [:material-code-brackets: LicenseStatusType](./literals.md#licensestatustype) 
3. See [:material-code-braces: DatetimeRangeTypeDef](./type_defs.md#datetimerangetypedef) 
4. See [:material-code-braces: EntitlementTypeDef](./type_defs.md#entitlementtypedef) 
5. See [:material-code-braces: ConsumptionConfigurationTypeDef](./type_defs.md#consumptionconfigurationtypedef) 
6. See [:material-code-braces: MetadataTypeDef](./type_defs.md#metadatatypedef) 
## GetGrantResponseTypeDef

```python
# GetGrantResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetGrantResponseTypeDef


def get_value() -> GetGrantResponseTypeDef:
    return {
        "Grant": ...,
    }


# GetGrantResponseTypeDef definition

class GetGrantResponseTypeDef(TypedDict):
    Grant: GrantTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDistributedGrantsResponseTypeDef

```python
# ListDistributedGrantsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListDistributedGrantsResponseTypeDef


def get_value() -> ListDistributedGrantsResponseTypeDef:
    return {
        "Grants": ...,
    }


# ListDistributedGrantsResponseTypeDef definition

class ListDistributedGrantsResponseTypeDef(TypedDict):
    Grants: List[GrantTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReceivedGrantsForOrganizationResponseTypeDef

```python
# ListReceivedGrantsForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListReceivedGrantsForOrganizationResponseTypeDef


def get_value() -> ListReceivedGrantsForOrganizationResponseTypeDef:
    return {
        "Grants": ...,
    }


# ListReceivedGrantsForOrganizationResponseTypeDef definition

class ListReceivedGrantsForOrganizationResponseTypeDef(TypedDict):
    Grants: List[GrantTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReceivedGrantsResponseTypeDef

```python
# ListReceivedGrantsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListReceivedGrantsResponseTypeDef


def get_value() -> ListReceivedGrantsResponseTypeDef:
    return {
        "Grants": ...,
    }


# ListReceivedGrantsResponseTypeDef definition

class ListReceivedGrantsResponseTypeDef(TypedDict):
    Grants: List[GrantTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GrantTypeDef](./type_defs.md#granttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicenseConversionTasksResponseTypeDef

```python
# ListLicenseConversionTasksResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseConversionTasksResponseTypeDef


def get_value() -> ListLicenseConversionTasksResponseTypeDef:
    return {
        "LicenseConversionTasks": ...,
    }


# ListLicenseConversionTasksResponseTypeDef definition

class ListLicenseConversionTasksResponseTypeDef(TypedDict):
    LicenseConversionTasks: List[LicenseConversionTaskTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseConversionTaskTypeDef](./type_defs.md#licenseconversiontasktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLicenseUsageResponseTypeDef

```python
# GetLicenseUsageResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseUsageResponseTypeDef


def get_value() -> GetLicenseUsageResponseTypeDef:
    return {
        "LicenseUsage": ...,
    }


# GetLicenseUsageResponseTypeDef definition

class GetLicenseUsageResponseTypeDef(TypedDict):
    LicenseUsage: LicenseUsageTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LicenseUsageTypeDef](./type_defs.md#licenseusagetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLicenseConfigurationResponseTypeDef

```python
# GetLicenseConfigurationResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseConfigurationResponseTypeDef


def get_value() -> GetLicenseConfigurationResponseTypeDef:
    return {
        "LicenseConfigurationId": ...,
    }


# GetLicenseConfigurationResponseTypeDef definition

class GetLicenseConfigurationResponseTypeDef(TypedDict):
    LicenseConfigurationId: str,
    LicenseConfigurationArn: str,
    Name: str,
    Description: str,
    LicenseCountingType: LicenseCountingTypeType,  # (1)
    LicenseRules: List[str],
    LicenseCount: int,
    LicenseCountHardLimit: bool,
    ConsumedLicenses: int,
    Status: str,
    OwnerAccountId: str,
    ConsumedLicenseSummaryList: List[ConsumedLicenseSummaryTypeDef],  # (2)
    ManagedResourceSummaryList: List[ManagedResourceSummaryTypeDef],  # (3)
    Tags: List[TagTypeDef],  # (4)
    ProductInformationList: List[ProductInformationOutputTypeDef],  # (5)
    AutomatedDiscoveryInformation: AutomatedDiscoveryInformationTypeDef,  # (6)
    DisassociateWhenNotFound: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: LicenseCountingTypeType](./literals.md#licensecountingtypetype) 
2. See [:material-code-braces: ConsumedLicenseSummaryTypeDef](./type_defs.md#consumedlicensesummarytypedef) 
3. See [:material-code-braces: ManagedResourceSummaryTypeDef](./type_defs.md#managedresourcesummarytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: ProductInformationOutputTypeDef](./type_defs.md#productinformationoutputtypedef) 
6. See [:material-code-braces: AutomatedDiscoveryInformationTypeDef](./type_defs.md#automateddiscoveryinformationtypedef) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LicenseConfigurationTypeDef

```python
# LicenseConfigurationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import LicenseConfigurationTypeDef


def get_value() -> LicenseConfigurationTypeDef:
    return {
        "LicenseConfigurationId": ...,
    }


# LicenseConfigurationTypeDef definition

class LicenseConfigurationTypeDef(TypedDict):
    LicenseConfigurationId: NotRequired[str],
    LicenseConfigurationArn: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    LicenseCountingType: NotRequired[LicenseCountingTypeType],  # (1)
    LicenseRules: NotRequired[List[str]],
    LicenseCount: NotRequired[int],
    LicenseCountHardLimit: NotRequired[bool],
    DisassociateWhenNotFound: NotRequired[bool],
    ConsumedLicenses: NotRequired[int],
    Status: NotRequired[str],
    OwnerAccountId: NotRequired[str],
    ConsumedLicenseSummaryList: NotRequired[List[ConsumedLicenseSummaryTypeDef]],  # (2)
    ManagedResourceSummaryList: NotRequired[List[ManagedResourceSummaryTypeDef]],  # (3)
    ProductInformationList: NotRequired[List[ProductInformationOutputTypeDef]],  # (4)
    AutomatedDiscoveryInformation: NotRequired[AutomatedDiscoveryInformationTypeDef],  # (5)
```

1. See [:material-code-brackets: LicenseCountingTypeType](./literals.md#licensecountingtypetype) 
2. See [:material-code-braces: ConsumedLicenseSummaryTypeDef](./type_defs.md#consumedlicensesummarytypedef) 
3. See [:material-code-braces: ManagedResourceSummaryTypeDef](./type_defs.md#managedresourcesummarytypedef) 
4. See [:material-code-braces: ProductInformationOutputTypeDef](./type_defs.md#productinformationoutputtypedef) 
5. See [:material-code-braces: AutomatedDiscoveryInformationTypeDef](./type_defs.md#automateddiscoveryinformationtypedef) 
## ProductInformationTypeDef

```python
# ProductInformationTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ProductInformationTypeDef


def get_value() -> ProductInformationTypeDef:
    return {
        "ResourceType": ...,
    }


# ProductInformationTypeDef definition

class ProductInformationTypeDef(TypedDict):
    ResourceType: str,
    ProductInformationFilterList: Sequence[ProductInformationFilterUnionTypeDef],  # (1)
```

1. See [:material-code-braces: ProductInformationFilterTypeDef](./type_defs.md#productinformationfiltertypedef) [:material-code-braces: ProductInformationFilterOutputTypeDef](./type_defs.md#productinformationfilteroutputtypedef) 
## CreateLicenseManagerReportGeneratorRequestTypeDef

```python
# CreateLicenseManagerReportGeneratorRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseManagerReportGeneratorRequestTypeDef


def get_value() -> CreateLicenseManagerReportGeneratorRequestTypeDef:
    return {
        "ReportGeneratorName": ...,
    }


# CreateLicenseManagerReportGeneratorRequestTypeDef definition

class CreateLicenseManagerReportGeneratorRequestTypeDef(TypedDict):
    ReportGeneratorName: str,
    Type: Sequence[ReportTypeType],  # (1)
    ReportContext: ReportContextUnionTypeDef,  # (2)
    ReportFrequency: ReportFrequencyTypeDef,  # (3)
    ClientToken: str,
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ReportContextTypeDef](./type_defs.md#reportcontexttypedef) [:material-code-braces: ReportContextOutputTypeDef](./type_defs.md#reportcontextoutputtypedef) 
3. See [:material-code-braces: ReportFrequencyTypeDef](./type_defs.md#reportfrequencytypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdateLicenseManagerReportGeneratorRequestTypeDef

```python
# UpdateLicenseManagerReportGeneratorRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import UpdateLicenseManagerReportGeneratorRequestTypeDef


def get_value() -> UpdateLicenseManagerReportGeneratorRequestTypeDef:
    return {
        "LicenseManagerReportGeneratorArn": ...,
    }


# UpdateLicenseManagerReportGeneratorRequestTypeDef definition

class UpdateLicenseManagerReportGeneratorRequestTypeDef(TypedDict):
    LicenseManagerReportGeneratorArn: str,
    ReportGeneratorName: str,
    Type: Sequence[ReportTypeType],  # (1)
    ReportContext: ReportContextUnionTypeDef,  # (2)
    ReportFrequency: ReportFrequencyTypeDef,  # (3)
    ClientToken: str,
    Description: NotRequired[str],
```

1. See [:material-code-brackets: ReportTypeType](./literals.md#reporttypetype) 
2. See [:material-code-braces: ReportContextTypeDef](./type_defs.md#reportcontexttypedef) [:material-code-braces: ReportContextOutputTypeDef](./type_defs.md#reportcontextoutputtypedef) 
3. See [:material-code-braces: ReportFrequencyTypeDef](./type_defs.md#reportfrequencytypedef) 
## GetLicenseManagerReportGeneratorResponseTypeDef

```python
# GetLicenseManagerReportGeneratorResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseManagerReportGeneratorResponseTypeDef


def get_value() -> GetLicenseManagerReportGeneratorResponseTypeDef:
    return {
        "ReportGenerator": ...,
    }


# GetLicenseManagerReportGeneratorResponseTypeDef definition

class GetLicenseManagerReportGeneratorResponseTypeDef(TypedDict):
    ReportGenerator: ReportGeneratorTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReportGeneratorTypeDef](./type_defs.md#reportgeneratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicenseManagerReportGeneratorsResponseTypeDef

```python
# ListLicenseManagerReportGeneratorsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseManagerReportGeneratorsResponseTypeDef


def get_value() -> ListLicenseManagerReportGeneratorsResponseTypeDef:
    return {
        "ReportGenerators": ...,
    }


# ListLicenseManagerReportGeneratorsResponseTypeDef definition

class ListLicenseManagerReportGeneratorsResponseTypeDef(TypedDict):
    ReportGenerators: List[ReportGeneratorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReportGeneratorTypeDef](./type_defs.md#reportgeneratortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReceivedLicensesForOrganizationResponseTypeDef

```python
# ListReceivedLicensesForOrganizationResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListReceivedLicensesForOrganizationResponseTypeDef


def get_value() -> ListReceivedLicensesForOrganizationResponseTypeDef:
    return {
        "Licenses": ...,
    }


# ListReceivedLicensesForOrganizationResponseTypeDef definition

class ListReceivedLicensesForOrganizationResponseTypeDef(TypedDict):
    Licenses: List[GrantedLicenseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GrantedLicenseTypeDef](./type_defs.md#grantedlicensetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReceivedLicensesResponseTypeDef

```python
# ListReceivedLicensesResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListReceivedLicensesResponseTypeDef


def get_value() -> ListReceivedLicensesResponseTypeDef:
    return {
        "Licenses": ...,
    }


# ListReceivedLicensesResponseTypeDef definition

class ListReceivedLicensesResponseTypeDef(TypedDict):
    Licenses: List[GrantedLicenseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GrantedLicenseTypeDef](./type_defs.md#grantedlicensetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLicenseResponseTypeDef

```python
# GetLicenseResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import GetLicenseResponseTypeDef


def get_value() -> GetLicenseResponseTypeDef:
    return {
        "License": ...,
    }


# GetLicenseResponseTypeDef definition

class GetLicenseResponseTypeDef(TypedDict):
    License: LicenseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LicenseTypeDef](./type_defs.md#licensetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicenseVersionsResponseTypeDef

```python
# ListLicenseVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseVersionsResponseTypeDef


def get_value() -> ListLicenseVersionsResponseTypeDef:
    return {
        "Licenses": ...,
    }


# ListLicenseVersionsResponseTypeDef definition

class ListLicenseVersionsResponseTypeDef(TypedDict):
    Licenses: List[LicenseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseTypeDef](./type_defs.md#licensetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicensesResponseTypeDef

```python
# ListLicensesResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicensesResponseTypeDef


def get_value() -> ListLicensesResponseTypeDef:
    return {
        "Licenses": ...,
    }


# ListLicensesResponseTypeDef definition

class ListLicensesResponseTypeDef(TypedDict):
    Licenses: List[LicenseTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseTypeDef](./type_defs.md#licensetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLicenseConfigurationsResponseTypeDef

```python
# ListLicenseConfigurationsResponseTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import ListLicenseConfigurationsResponseTypeDef


def get_value() -> ListLicenseConfigurationsResponseTypeDef:
    return {
        "LicenseConfigurations": ...,
    }


# ListLicenseConfigurationsResponseTypeDef definition

class ListLicenseConfigurationsResponseTypeDef(TypedDict):
    LicenseConfigurations: List[LicenseConfigurationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: LicenseConfigurationTypeDef](./type_defs.md#licenseconfigurationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateLicenseConfigurationRequestTypeDef

```python
# CreateLicenseConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import CreateLicenseConfigurationRequestTypeDef


def get_value() -> CreateLicenseConfigurationRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateLicenseConfigurationRequestTypeDef definition

class CreateLicenseConfigurationRequestTypeDef(TypedDict):
    Name: str,
    LicenseCountingType: LicenseCountingTypeType,  # (1)
    Description: NotRequired[str],
    LicenseCount: NotRequired[int],
    LicenseCountHardLimit: NotRequired[bool],
    LicenseRules: NotRequired[Sequence[str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    DisassociateWhenNotFound: NotRequired[bool],
    ProductInformationList: NotRequired[Sequence[ProductInformationUnionTypeDef]],  # (3)
```

1. See [:material-code-brackets: LicenseCountingTypeType](./literals.md#licensecountingtypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ProductInformationTypeDef](./type_defs.md#productinformationtypedef) [:material-code-braces: ProductInformationOutputTypeDef](./type_defs.md#productinformationoutputtypedef) 
## UpdateLicenseConfigurationRequestTypeDef

```python
# UpdateLicenseConfigurationRequestTypeDef TypedDict usage example

from types_aiobotocore_license_manager.type_defs import UpdateLicenseConfigurationRequestTypeDef


def get_value() -> UpdateLicenseConfigurationRequestTypeDef:
    return {
        "LicenseConfigurationArn": ...,
    }


# UpdateLicenseConfigurationRequestTypeDef definition

class UpdateLicenseConfigurationRequestTypeDef(TypedDict):
    LicenseConfigurationArn: str,
    LicenseConfigurationStatus: NotRequired[LicenseConfigurationStatusType],  # (1)
    LicenseRules: NotRequired[Sequence[str]],
    LicenseCount: NotRequired[int],
    LicenseCountHardLimit: NotRequired[bool],
    Name: NotRequired[str],
    Description: NotRequired[str],
    ProductInformationList: NotRequired[Sequence[ProductInformationUnionTypeDef]],  # (2)
    DisassociateWhenNotFound: NotRequired[bool],
```

1. See [:material-code-brackets: LicenseConfigurationStatusType](./literals.md#licenseconfigurationstatustype) 
2. See [:material-code-braces: ProductInformationTypeDef](./type_defs.md#productinformationtypedef) [:material-code-braces: ProductInformationOutputTypeDef](./type_defs.md#productinformationoutputtypedef) 

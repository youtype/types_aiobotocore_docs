# Type definitions

> [Index](../README.md) > [DataZone](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DataZone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#datazone)
    type annotations stubs module [types-aiobotocore-datazone](https://pypi.org/project/types-aiobotocore-datazone/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import BlobTypeDef


def get_value() -> BlobTypeDef:
    return ...


# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```


## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## DataProductItemUnionTypeDef

```python
# DataProductItemUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import DataProductItemUnionTypeDef


def get_value() -> DataProductItemUnionTypeDef:
    return ...


# DataProductItemUnionTypeDef definition

DataProductItemUnionTypeDef = Union[
    DataProductItemTypeDef,  # (1)
    DataProductItemOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataProductItemTypeDef](./type_defs.md#dataproductitemtypedef) 
2. See [:material-code-braces: DataProductItemOutputTypeDef](./type_defs.md#dataproductitemoutputtypedef) 

## LakeFormationConfigurationUnionTypeDef

```python
# LakeFormationConfigurationUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import LakeFormationConfigurationUnionTypeDef


def get_value() -> LakeFormationConfigurationUnionTypeDef:
    return ...


# LakeFormationConfigurationUnionTypeDef definition

LakeFormationConfigurationUnionTypeDef = Union[
    LakeFormationConfigurationTypeDef,  # (1)
    LakeFormationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 
2. See [:material-code-braces: LakeFormationConfigurationOutputTypeDef](./type_defs.md#lakeformationconfigurationoutputtypedef) 

## PhysicalConnectionRequirementsUnionTypeDef

```python
# PhysicalConnectionRequirementsUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import PhysicalConnectionRequirementsUnionTypeDef


def get_value() -> PhysicalConnectionRequirementsUnionTypeDef:
    return ...


# PhysicalConnectionRequirementsUnionTypeDef definition

PhysicalConnectionRequirementsUnionTypeDef = Union[
    PhysicalConnectionRequirementsTypeDef,  # (1)
    PhysicalConnectionRequirementsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PhysicalConnectionRequirementsTypeDef](./type_defs.md#physicalconnectionrequirementstypedef) 
2. See [:material-code-braces: PhysicalConnectionRequirementsOutputTypeDef](./type_defs.md#physicalconnectionrequirementsoutputtypedef) 

## TermRelationsUnionTypeDef

```python
# TermRelationsUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import TermRelationsUnionTypeDef


def get_value() -> TermRelationsUnionTypeDef:
    return ...


# TermRelationsUnionTypeDef definition

TermRelationsUnionTypeDef = Union[
    TermRelationsTypeDef,  # (1)
    TermRelationsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: TermRelationsTypeDef](./type_defs.md#termrelationstypedef) 
2. See [:material-code-braces: TermRelationsOutputTypeDef](./type_defs.md#termrelationsoutputtypedef) 

## EnvironmentConfigurationUserParameterUnionTypeDef

```python
# EnvironmentConfigurationUserParameterUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationUserParameterUnionTypeDef


def get_value() -> EnvironmentConfigurationUserParameterUnionTypeDef:
    return ...


# EnvironmentConfigurationUserParameterUnionTypeDef definition

EnvironmentConfigurationUserParameterUnionTypeDef = Union[
    EnvironmentConfigurationUserParameterTypeDef,  # (1)
    EnvironmentConfigurationUserParameterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EnvironmentConfigurationUserParameterTypeDef](./type_defs.md#environmentconfigurationuserparametertypedef) 
2. See [:material-code-braces: EnvironmentConfigurationUserParameterOutputTypeDef](./type_defs.md#environmentconfigurationuserparameteroutputtypedef) 

## EnvironmentDeploymentDetailsUnionTypeDef

```python
# EnvironmentDeploymentDetailsUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import EnvironmentDeploymentDetailsUnionTypeDef


def get_value() -> EnvironmentDeploymentDetailsUnionTypeDef:
    return ...


# EnvironmentDeploymentDetailsUnionTypeDef definition

EnvironmentDeploymentDetailsUnionTypeDef = Union[
    EnvironmentDeploymentDetailsTypeDef,  # (1)
    EnvironmentDeploymentDetailsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EnvironmentDeploymentDetailsTypeDef](./type_defs.md#environmentdeploymentdetailstypedef) 
2. See [:material-code-braces: EnvironmentDeploymentDetailsOutputTypeDef](./type_defs.md#environmentdeploymentdetailsoutputtypedef) 

## EnvironmentConfigurationParametersDetailsUnionTypeDef

```python
# EnvironmentConfigurationParametersDetailsUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationParametersDetailsUnionTypeDef


def get_value() -> EnvironmentConfigurationParametersDetailsUnionTypeDef:
    return ...


# EnvironmentConfigurationParametersDetailsUnionTypeDef definition

EnvironmentConfigurationParametersDetailsUnionTypeDef = Union[
    EnvironmentConfigurationParametersDetailsTypeDef,  # (1)
    EnvironmentConfigurationParametersDetailsOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EnvironmentConfigurationParametersDetailsTypeDef](./type_defs.md#environmentconfigurationparametersdetailstypedef) 
2. See [:material-code-braces: EnvironmentConfigurationParametersDetailsOutputTypeDef](./type_defs.md#environmentconfigurationparametersdetailsoutputtypedef) 

## RelationalFilterConfigurationUnionTypeDef

```python
# RelationalFilterConfigurationUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import RelationalFilterConfigurationUnionTypeDef


def get_value() -> RelationalFilterConfigurationUnionTypeDef:
    return ...


# RelationalFilterConfigurationUnionTypeDef definition

RelationalFilterConfigurationUnionTypeDef = Union[
    RelationalFilterConfigurationTypeDef,  # (1)
    RelationalFilterConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RelationalFilterConfigurationTypeDef](./type_defs.md#relationalfilterconfigurationtypedef) 
2. See [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 

## OAuth2PropertiesUnionTypeDef

```python
# OAuth2PropertiesUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import OAuth2PropertiesUnionTypeDef


def get_value() -> OAuth2PropertiesUnionTypeDef:
    return ...


# OAuth2PropertiesUnionTypeDef definition

OAuth2PropertiesUnionTypeDef = Union[
    OAuth2PropertiesTypeDef,  # (1)
    OAuth2PropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: OAuth2PropertiesTypeDef](./type_defs.md#oauth2propertiestypedef) 
2. See [:material-code-braces: OAuth2PropertiesOutputTypeDef](./type_defs.md#oauth2propertiesoutputtypedef) 

## PolicyGrantDetailUnionTypeDef

```python
# PolicyGrantDetailUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import PolicyGrantDetailUnionTypeDef


def get_value() -> PolicyGrantDetailUnionTypeDef:
    return ...


# PolicyGrantDetailUnionTypeDef definition

PolicyGrantDetailUnionTypeDef = Union[
    PolicyGrantDetailTypeDef,  # (1)
    PolicyGrantDetailOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PolicyGrantDetailTypeDef](./type_defs.md#policygrantdetailtypedef) 
2. See [:material-code-braces: PolicyGrantDetailOutputTypeDef](./type_defs.md#policygrantdetailoutputtypedef) 

## RuleScopeUnionTypeDef

```python
# RuleScopeUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import RuleScopeUnionTypeDef


def get_value() -> RuleScopeUnionTypeDef:
    return ...


# RuleScopeUnionTypeDef definition

RuleScopeUnionTypeDef = Union[
    RuleScopeTypeDef,  # (1)
    RuleScopeOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleScopeTypeDef](./type_defs.md#rulescopetypedef) 
2. See [:material-code-braces: RuleScopeOutputTypeDef](./type_defs.md#rulescopeoutputtypedef) 

## ProvisioningConfigurationUnionTypeDef

```python
# ProvisioningConfigurationUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import ProvisioningConfigurationUnionTypeDef


def get_value() -> ProvisioningConfigurationUnionTypeDef:
    return ...


# ProvisioningConfigurationUnionTypeDef definition

ProvisioningConfigurationUnionTypeDef = Union[
    ProvisioningConfigurationTypeDef,  # (1)
    ProvisioningConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProvisioningConfigurationTypeDef](./type_defs.md#provisioningconfigurationtypedef) 
2. See [:material-code-braces: ProvisioningConfigurationOutputTypeDef](./type_defs.md#provisioningconfigurationoutputtypedef) 

## RuleDetailUnionTypeDef

```python
# RuleDetailUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import RuleDetailUnionTypeDef


def get_value() -> RuleDetailUnionTypeDef:
    return ...


# RuleDetailUnionTypeDef definition

RuleDetailUnionTypeDef = Union[
    RuleDetailTypeDef,  # (1)
    RuleDetailOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RuleDetailTypeDef](./type_defs.md#ruledetailtypedef) 
2. See [:material-code-braces: RuleDetailOutputTypeDef](./type_defs.md#ruledetailoutputtypedef) 

## PolicyGrantPrincipalUnionTypeDef

```python
# PolicyGrantPrincipalUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import PolicyGrantPrincipalUnionTypeDef


def get_value() -> PolicyGrantPrincipalUnionTypeDef:
    return ...


# PolicyGrantPrincipalUnionTypeDef definition

PolicyGrantPrincipalUnionTypeDef = Union[
    PolicyGrantPrincipalTypeDef,  # (1)
    PolicyGrantPrincipalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: PolicyGrantPrincipalTypeDef](./type_defs.md#policygrantprincipaltypedef) 
2. See [:material-code-braces: PolicyGrantPrincipalOutputTypeDef](./type_defs.md#policygrantprincipaloutputtypedef) 

## EnvironmentConfigurationUnionTypeDef

```python
# EnvironmentConfigurationUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationUnionTypeDef


def get_value() -> EnvironmentConfigurationUnionTypeDef:
    return ...


# EnvironmentConfigurationUnionTypeDef definition

EnvironmentConfigurationUnionTypeDef = Union[
    EnvironmentConfigurationTypeDef,  # (1)
    EnvironmentConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: EnvironmentConfigurationTypeDef](./type_defs.md#environmentconfigurationtypedef) 
2. See [:material-code-braces: EnvironmentConfigurationOutputTypeDef](./type_defs.md#environmentconfigurationoutputtypedef) 

## AssetFilterConfigurationUnionTypeDef

```python
# AssetFilterConfigurationUnionTypeDef Union usage example

from types_aiobotocore_datazone.type_defs import AssetFilterConfigurationUnionTypeDef


def get_value() -> AssetFilterConfigurationUnionTypeDef:
    return ...


# AssetFilterConfigurationUnionTypeDef definition

AssetFilterConfigurationUnionTypeDef = Union[
    AssetFilterConfigurationTypeDef,  # (1)
    AssetFilterConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: AssetFilterConfigurationTypeDef](./type_defs.md#assetfilterconfigurationtypedef) 
2. See [:material-code-braces: AssetFilterConfigurationOutputTypeDef](./type_defs.md#assetfilterconfigurationoutputtypedef) 



## AcceptChoiceTypeDef

```python
# AcceptChoiceTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AcceptChoiceTypeDef


def get_value() -> AcceptChoiceTypeDef:
    return {
        "editedValue": ...,
    }


# AcceptChoiceTypeDef definition

class AcceptChoiceTypeDef(TypedDict):
    predictionTarget: str,
    editedValue: NotRequired[str],
    predictionChoice: NotRequired[int],
```

## AcceptRuleTypeDef

```python
# AcceptRuleTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AcceptRuleTypeDef


def get_value() -> AcceptRuleTypeDef:
    return {
        "rule": ...,
    }


# AcceptRuleTypeDef definition

class AcceptRuleTypeDef(TypedDict):
    rule: NotRequired[AcceptRuleBehaviorType],  # (1)
    threshold: NotRequired[float],
```

1. See [:material-code-brackets: AcceptRuleBehaviorType](./literals.md#acceptrulebehaviortype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ResponseMetadataTypeDef


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

## AcceptedAssetScopeTypeDef

```python
# AcceptedAssetScopeTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AcceptedAssetScopeTypeDef


def get_value() -> AcceptedAssetScopeTypeDef:
    return {
        "assetId": ...,
    }


# AcceptedAssetScopeTypeDef definition

class AcceptedAssetScopeTypeDef(TypedDict):
    assetId: str,
    filterIds: Sequence[str],
```

## FormOutputTypeDef

```python
# FormOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FormOutputTypeDef


def get_value() -> FormOutputTypeDef:
    return {
        "content": ...,
    }


# FormOutputTypeDef definition

class FormOutputTypeDef(TypedDict):
    formName: str,
    content: NotRequired[str],
    typeName: NotRequired[str],
    typeRevision: NotRequired[str],
```

## AwsConsoleLinkParametersTypeDef

```python
# AwsConsoleLinkParametersTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AwsConsoleLinkParametersTypeDef


def get_value() -> AwsConsoleLinkParametersTypeDef:
    return {
        "uri": ...,
    }


# AwsConsoleLinkParametersTypeDef definition

class AwsConsoleLinkParametersTypeDef(TypedDict):
    uri: NotRequired[str],
```

## AddToProjectMemberPoolPolicyGrantDetailTypeDef

```python
# AddToProjectMemberPoolPolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AddToProjectMemberPoolPolicyGrantDetailTypeDef


def get_value() -> AddToProjectMemberPoolPolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# AddToProjectMemberPoolPolicyGrantDetailTypeDef definition

class AddToProjectMemberPoolPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## ColumnFilterConfigurationOutputTypeDef

```python
# ColumnFilterConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ColumnFilterConfigurationOutputTypeDef


def get_value() -> ColumnFilterConfigurationOutputTypeDef:
    return {
        "includedColumnNames": ...,
    }


# ColumnFilterConfigurationOutputTypeDef definition

class ColumnFilterConfigurationOutputTypeDef(TypedDict):
    includedColumnNames: NotRequired[List[str]],
```

## ColumnFilterConfigurationTypeDef

```python
# ColumnFilterConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ColumnFilterConfigurationTypeDef


def get_value() -> ColumnFilterConfigurationTypeDef:
    return {
        "includedColumnNames": ...,
    }


# ColumnFilterConfigurationTypeDef definition

class ColumnFilterConfigurationTypeDef(TypedDict):
    includedColumnNames: NotRequired[Sequence[str]],
```

## AssetFilterSummaryTypeDef

```python
# AssetFilterSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetFilterSummaryTypeDef


def get_value() -> AssetFilterSummaryTypeDef:
    return {
        "assetId": ...,
    }


# AssetFilterSummaryTypeDef definition

class AssetFilterSummaryTypeDef(TypedDict):
    assetId: str,
    domainId: str,
    id: str,
    name: str,
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    effectiveColumnNames: NotRequired[List[str]],
    effectiveRowFilter: NotRequired[str],
    errorMessage: NotRequired[str],
    status: NotRequired[FilterStatusType],  # (1)
```

1. See [:material-code-brackets: FilterStatusType](./literals.md#filterstatustype) 
## AssetInDataProductListingItemTypeDef

```python
# AssetInDataProductListingItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetInDataProductListingItemTypeDef


def get_value() -> AssetInDataProductListingItemTypeDef:
    return {
        "entityId": ...,
    }


# AssetInDataProductListingItemTypeDef definition

class AssetInDataProductListingItemTypeDef(TypedDict):
    entityId: NotRequired[str],
    entityRevision: NotRequired[str],
    entityType: NotRequired[str],
```

## TimeSeriesDataPointSummaryFormOutputTypeDef

```python
# TimeSeriesDataPointSummaryFormOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import TimeSeriesDataPointSummaryFormOutputTypeDef


def get_value() -> TimeSeriesDataPointSummaryFormOutputTypeDef:
    return {
        "contentSummary": ...,
    }


# TimeSeriesDataPointSummaryFormOutputTypeDef definition

class TimeSeriesDataPointSummaryFormOutputTypeDef(TypedDict):
    formName: str,
    timestamp: datetime,
    typeIdentifier: str,
    contentSummary: NotRequired[str],
    id: NotRequired[str],
    typeRevision: NotRequired[str],
```

## AssetListingDetailsTypeDef

```python
# AssetListingDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetListingDetailsTypeDef


def get_value() -> AssetListingDetailsTypeDef:
    return {
        "listingId": ...,
    }


# AssetListingDetailsTypeDef definition

class AssetListingDetailsTypeDef(TypedDict):
    listingId: str,
    listingStatus: ListingStatusType,  # (1)
```

1. See [:material-code-brackets: ListingStatusType](./literals.md#listingstatustype) 
## DetailedGlossaryTermTypeDef

```python
# DetailedGlossaryTermTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DetailedGlossaryTermTypeDef


def get_value() -> DetailedGlossaryTermTypeDef:
    return {
        "name": ...,
    }


# DetailedGlossaryTermTypeDef definition

class DetailedGlossaryTermTypeDef(TypedDict):
    name: NotRequired[str],
    shortDescription: NotRequired[str],
```

## AssetRevisionTypeDef

```python
# AssetRevisionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetRevisionTypeDef


def get_value() -> AssetRevisionTypeDef:
    return {
        "createdAt": ...,
    }


# AssetRevisionTypeDef definition

class AssetRevisionTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    domainId: NotRequired[str],
    id: NotRequired[str],
    revision: NotRequired[str],
```

## AssetScopeTypeDef

```python
# AssetScopeTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetScopeTypeDef


def get_value() -> AssetScopeTypeDef:
    return {
        "assetId": ...,
    }


# AssetScopeTypeDef definition

class AssetScopeTypeDef(TypedDict):
    assetId: str,
    filterIds: List[str],
    status: str,
    errorMessage: NotRequired[str],
```

## AssetTargetNameMapTypeDef

```python
# AssetTargetNameMapTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetTargetNameMapTypeDef


def get_value() -> AssetTargetNameMapTypeDef:
    return {
        "assetId": ...,
    }


# AssetTargetNameMapTypeDef definition

class AssetTargetNameMapTypeDef(TypedDict):
    assetId: str,
    targetName: str,
```

## FormEntryOutputTypeDef

```python
# FormEntryOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FormEntryOutputTypeDef


def get_value() -> FormEntryOutputTypeDef:
    return {
        "required": ...,
    }


# FormEntryOutputTypeDef definition

class FormEntryOutputTypeDef(TypedDict):
    typeName: str,
    typeRevision: str,
    required: NotRequired[bool],
```

## AssetTypesForRuleOutputTypeDef

```python
# AssetTypesForRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetTypesForRuleOutputTypeDef


def get_value() -> AssetTypesForRuleOutputTypeDef:
    return {
        "selectionMode": ...,
    }


# AssetTypesForRuleOutputTypeDef definition

class AssetTypesForRuleOutputTypeDef(TypedDict):
    selectionMode: RuleScopeSelectionModeType,  # (1)
    specificAssetTypes: NotRequired[List[str]],
```

1. See [:material-code-brackets: RuleScopeSelectionModeType](./literals.md#rulescopeselectionmodetype) 
## AssetTypesForRuleTypeDef

```python
# AssetTypesForRuleTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetTypesForRuleTypeDef


def get_value() -> AssetTypesForRuleTypeDef:
    return {
        "selectionMode": ...,
    }


# AssetTypesForRuleTypeDef definition

class AssetTypesForRuleTypeDef(TypedDict):
    selectionMode: RuleScopeSelectionModeType,  # (1)
    specificAssetTypes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: RuleScopeSelectionModeType](./literals.md#rulescopeselectionmodetype) 
## AssociateEnvironmentRoleInputTypeDef

```python
# AssociateEnvironmentRoleInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssociateEnvironmentRoleInputTypeDef


def get_value() -> AssociateEnvironmentRoleInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# AssociateEnvironmentRoleInputTypeDef definition

class AssociateEnvironmentRoleInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    environmentRoleArn: str,
```

## AthenaPropertiesInputTypeDef

```python
# AthenaPropertiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AthenaPropertiesInputTypeDef


def get_value() -> AthenaPropertiesInputTypeDef:
    return {
        "workgroupName": ...,
    }


# AthenaPropertiesInputTypeDef definition

class AthenaPropertiesInputTypeDef(TypedDict):
    workgroupName: NotRequired[str],
```

## AthenaPropertiesOutputTypeDef

```python
# AthenaPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AthenaPropertiesOutputTypeDef


def get_value() -> AthenaPropertiesOutputTypeDef:
    return {
        "workgroupName": ...,
    }


# AthenaPropertiesOutputTypeDef definition

class AthenaPropertiesOutputTypeDef(TypedDict):
    workgroupName: NotRequired[str],
```

## AthenaPropertiesPatchTypeDef

```python
# AthenaPropertiesPatchTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AthenaPropertiesPatchTypeDef


def get_value() -> AthenaPropertiesPatchTypeDef:
    return {
        "workgroupName": ...,
    }


# AthenaPropertiesPatchTypeDef definition

class AthenaPropertiesPatchTypeDef(TypedDict):
    workgroupName: NotRequired[str],
```

## BasicAuthenticationCredentialsTypeDef

```python
# BasicAuthenticationCredentialsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import BasicAuthenticationCredentialsTypeDef


def get_value() -> BasicAuthenticationCredentialsTypeDef:
    return {
        "password": ...,
    }


# BasicAuthenticationCredentialsTypeDef definition

class BasicAuthenticationCredentialsTypeDef(TypedDict):
    password: NotRequired[str],
    userName: NotRequired[str],
```

## AuthorizationCodePropertiesTypeDef

```python
# AuthorizationCodePropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AuthorizationCodePropertiesTypeDef


def get_value() -> AuthorizationCodePropertiesTypeDef:
    return {
        "authorizationCode": ...,
    }


# AuthorizationCodePropertiesTypeDef definition

class AuthorizationCodePropertiesTypeDef(TypedDict):
    authorizationCode: NotRequired[str],
    redirectUri: NotRequired[str],
```

## AwsAccountTypeDef

```python
# AwsAccountTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AwsAccountTypeDef


def get_value() -> AwsAccountTypeDef:
    return {
        "awsAccountId": ...,
    }


# AwsAccountTypeDef definition

class AwsAccountTypeDef(TypedDict):
    awsAccountId: NotRequired[str],
    awsAccountIdPath: NotRequired[str],
```

## AwsLocationTypeDef

```python
# AwsLocationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AwsLocationTypeDef


def get_value() -> AwsLocationTypeDef:
    return {
        "accessRole": ...,
    }


# AwsLocationTypeDef definition

class AwsLocationTypeDef(TypedDict):
    accessRole: NotRequired[str],
    awsAccountId: NotRequired[str],
    awsRegion: NotRequired[str],
    iamConnectionId: NotRequired[str],
```

## BusinessNameGenerationConfigurationTypeDef

```python
# BusinessNameGenerationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import BusinessNameGenerationConfigurationTypeDef


def get_value() -> BusinessNameGenerationConfigurationTypeDef:
    return {
        "enabled": ...,
    }


# BusinessNameGenerationConfigurationTypeDef definition

class BusinessNameGenerationConfigurationTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## CancelMetadataGenerationRunInputTypeDef

```python
# CancelMetadataGenerationRunInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CancelMetadataGenerationRunInputTypeDef


def get_value() -> CancelMetadataGenerationRunInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CancelMetadataGenerationRunInputTypeDef definition

class CancelMetadataGenerationRunInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## CancelSubscriptionInputTypeDef

```python
# CancelSubscriptionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CancelSubscriptionInputTypeDef


def get_value() -> CancelSubscriptionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CancelSubscriptionInputTypeDef definition

class CancelSubscriptionInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## CloudFormationPropertiesTypeDef

```python
# CloudFormationPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CloudFormationPropertiesTypeDef


def get_value() -> CloudFormationPropertiesTypeDef:
    return {
        "templateUrl": ...,
    }


# CloudFormationPropertiesTypeDef definition

class CloudFormationPropertiesTypeDef(TypedDict):
    templateUrl: str,
```

## ConfigurableActionParameterTypeDef

```python
# ConfigurableActionParameterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ConfigurableActionParameterTypeDef


def get_value() -> ConfigurableActionParameterTypeDef:
    return {
        "key": ...,
    }


# ConfigurableActionParameterTypeDef definition

class ConfigurableActionParameterTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## ConnectionCredentialsTypeDef

```python
# ConnectionCredentialsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ConnectionCredentialsTypeDef


def get_value() -> ConnectionCredentialsTypeDef:
    return {
        "accessKeyId": ...,
    }


# ConnectionCredentialsTypeDef definition

class ConnectionCredentialsTypeDef(TypedDict):
    accessKeyId: NotRequired[str],
    expiration: NotRequired[datetime],
    secretAccessKey: NotRequired[str],
    sessionToken: NotRequired[str],
```

## HyperPodPropertiesInputTypeDef

```python
# HyperPodPropertiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import HyperPodPropertiesInputTypeDef


def get_value() -> HyperPodPropertiesInputTypeDef:
    return {
        "clusterName": ...,
    }


# HyperPodPropertiesInputTypeDef definition

class HyperPodPropertiesInputTypeDef(TypedDict):
    clusterName: str,
```

## IamPropertiesInputTypeDef

```python
# IamPropertiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import IamPropertiesInputTypeDef


def get_value() -> IamPropertiesInputTypeDef:
    return {
        "glueLineageSyncEnabled": ...,
    }


# IamPropertiesInputTypeDef definition

class IamPropertiesInputTypeDef(TypedDict):
    glueLineageSyncEnabled: NotRequired[bool],
```

## SparkEmrPropertiesInputTypeDef

```python
# SparkEmrPropertiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SparkEmrPropertiesInputTypeDef


def get_value() -> SparkEmrPropertiesInputTypeDef:
    return {
        "computeArn": ...,
    }


# SparkEmrPropertiesInputTypeDef definition

class SparkEmrPropertiesInputTypeDef(TypedDict):
    computeArn: NotRequired[str],
    instanceProfileArn: NotRequired[str],
    javaVirtualEnv: NotRequired[str],
    logUri: NotRequired[str],
    pythonVirtualEnv: NotRequired[str],
    runtimeRole: NotRequired[str],
    trustedCertificatesS3Uri: NotRequired[str],
```

## GluePropertiesOutputTypeDef

```python
# GluePropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GluePropertiesOutputTypeDef


def get_value() -> GluePropertiesOutputTypeDef:
    return {
        "errorMessage": ...,
    }


# GluePropertiesOutputTypeDef definition

class GluePropertiesOutputTypeDef(TypedDict):
    errorMessage: NotRequired[str],
    status: NotRequired[ConnectionStatusType],  # (1)
```

1. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
## HyperPodPropertiesOutputTypeDef

```python
# HyperPodPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import HyperPodPropertiesOutputTypeDef


def get_value() -> HyperPodPropertiesOutputTypeDef:
    return {
        "clusterArn": ...,
    }


# HyperPodPropertiesOutputTypeDef definition

class HyperPodPropertiesOutputTypeDef(TypedDict):
    clusterName: str,
    clusterArn: NotRequired[str],
    orchestrator: NotRequired[HyperPodOrchestratorType],  # (1)
```

1. See [:material-code-brackets: HyperPodOrchestratorType](./literals.md#hyperpodorchestratortype) 
## IamPropertiesOutputTypeDef

```python
# IamPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import IamPropertiesOutputTypeDef


def get_value() -> IamPropertiesOutputTypeDef:
    return {
        "environmentId": ...,
    }


# IamPropertiesOutputTypeDef definition

class IamPropertiesOutputTypeDef(TypedDict):
    environmentId: NotRequired[str],
    glueLineageSyncEnabled: NotRequired[bool],
```

## IamPropertiesPatchTypeDef

```python
# IamPropertiesPatchTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import IamPropertiesPatchTypeDef


def get_value() -> IamPropertiesPatchTypeDef:
    return {
        "glueLineageSyncEnabled": ...,
    }


# IamPropertiesPatchTypeDef definition

class IamPropertiesPatchTypeDef(TypedDict):
    glueLineageSyncEnabled: NotRequired[bool],
```

## SparkEmrPropertiesPatchTypeDef

```python
# SparkEmrPropertiesPatchTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SparkEmrPropertiesPatchTypeDef


def get_value() -> SparkEmrPropertiesPatchTypeDef:
    return {
        "computeArn": ...,
    }


# SparkEmrPropertiesPatchTypeDef definition

class SparkEmrPropertiesPatchTypeDef(TypedDict):
    computeArn: NotRequired[str],
    instanceProfileArn: NotRequired[str],
    javaVirtualEnv: NotRequired[str],
    logUri: NotRequired[str],
    pythonVirtualEnv: NotRequired[str],
    runtimeRole: NotRequired[str],
    trustedCertificatesS3Uri: NotRequired[str],
```

## FormInputTypeDef

```python
# FormInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FormInputTypeDef


def get_value() -> FormInputTypeDef:
    return {
        "content": ...,
    }


# FormInputTypeDef definition

class FormInputTypeDef(TypedDict):
    formName: str,
    content: NotRequired[str],
    typeIdentifier: NotRequired[str],
    typeRevision: NotRequired[str],
```

## FormEntryInputTypeDef

```python
# FormEntryInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FormEntryInputTypeDef


def get_value() -> FormEntryInputTypeDef:
    return {
        "required": ...,
    }


# FormEntryInputTypeDef definition

class FormEntryInputTypeDef(TypedDict):
    typeIdentifier: str,
    typeRevision: str,
    required: NotRequired[bool],
```

## CreateAssetTypePolicyGrantDetailTypeDef

```python
# CreateAssetTypePolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetTypePolicyGrantDetailTypeDef


def get_value() -> CreateAssetTypePolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# CreateAssetTypePolicyGrantDetailTypeDef definition

class CreateAssetTypePolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## DataProductItemOutputTypeDef

```python
# DataProductItemOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataProductItemOutputTypeDef


def get_value() -> DataProductItemOutputTypeDef:
    return {
        "glossaryTerms": ...,
    }


# DataProductItemOutputTypeDef definition

class DataProductItemOutputTypeDef(TypedDict):
    identifier: str,
    itemType: DataProductItemTypeType,  # (1)
    glossaryTerms: NotRequired[List[str]],
    revision: NotRequired[str],
```

1. See [:material-code-brackets: DataProductItemTypeType](./literals.md#dataproductitemtypetype) 
## RecommendationConfigurationTypeDef

```python
# RecommendationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RecommendationConfigurationTypeDef


def get_value() -> RecommendationConfigurationTypeDef:
    return {
        "enableBusinessNameGeneration": ...,
    }


# RecommendationConfigurationTypeDef definition

class RecommendationConfigurationTypeDef(TypedDict):
    enableBusinessNameGeneration: NotRequired[bool],
```

## ScheduleConfigurationTypeDef

```python
# ScheduleConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ScheduleConfigurationTypeDef


def get_value() -> ScheduleConfigurationTypeDef:
    return {
        "schedule": ...,
    }


# ScheduleConfigurationTypeDef definition

class ScheduleConfigurationTypeDef(TypedDict):
    schedule: NotRequired[str],
    timezone: NotRequired[TimezoneType],  # (1)
```

1. See [:material-code-brackets: TimezoneType](./literals.md#timezonetype) 
## DataSourceErrorMessageTypeDef

```python
# DataSourceErrorMessageTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataSourceErrorMessageTypeDef


def get_value() -> DataSourceErrorMessageTypeDef:
    return {
        "errorDetail": ...,
    }


# DataSourceErrorMessageTypeDef definition

class DataSourceErrorMessageTypeDef(TypedDict):
    errorType: DataSourceErrorTypeType,  # (1)
    errorDetail: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceErrorTypeType](./literals.md#datasourceerrortypetype) 
## SingleSignOnTypeDef

```python
# SingleSignOnTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SingleSignOnTypeDef


def get_value() -> SingleSignOnTypeDef:
    return {
        "type": ...,
    }


# SingleSignOnTypeDef definition

class SingleSignOnTypeDef(TypedDict):
    type: NotRequired[AuthTypeType],  # (1)
    userAssignment: NotRequired[UserAssignmentType],  # (2)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-brackets: UserAssignmentType](./literals.md#userassignmenttype) 
## CreateDomainUnitInputTypeDef

```python
# CreateDomainUnitInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDomainUnitInputTypeDef


def get_value() -> CreateDomainUnitInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateDomainUnitInputTypeDef definition

class CreateDomainUnitInputTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    parentDomainUnitIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## CreateDomainUnitPolicyGrantDetailTypeDef

```python
# CreateDomainUnitPolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDomainUnitPolicyGrantDetailTypeDef


def get_value() -> CreateDomainUnitPolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# CreateDomainUnitPolicyGrantDetailTypeDef definition

class CreateDomainUnitPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## EnvironmentParameterTypeDef

```python
# EnvironmentParameterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentParameterTypeDef


def get_value() -> EnvironmentParameterTypeDef:
    return {
        "name": ...,
    }


# EnvironmentParameterTypeDef definition

class EnvironmentParameterTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## CustomParameterTypeDef

```python
# CustomParameterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CustomParameterTypeDef


def get_value() -> CustomParameterTypeDef:
    return {
        "defaultValue": ...,
    }


# CustomParameterTypeDef definition

class CustomParameterTypeDef(TypedDict):
    fieldType: str,
    keyName: str,
    defaultValue: NotRequired[str],
    description: NotRequired[str],
    isEditable: NotRequired[bool],
    isOptional: NotRequired[bool],
```

## DeploymentPropertiesTypeDef

```python
# DeploymentPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeploymentPropertiesTypeDef


def get_value() -> DeploymentPropertiesTypeDef:
    return {
        "endTimeoutMinutes": ...,
    }


# DeploymentPropertiesTypeDef definition

class DeploymentPropertiesTypeDef(TypedDict):
    endTimeoutMinutes: NotRequired[int],
    startTimeoutMinutes: NotRequired[int],
```

## ResourceTypeDef

```python
# ResourceTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ResourceTypeDef


def get_value() -> ResourceTypeDef:
    return {
        "name": ...,
    }


# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    type: str,
    value: str,
    name: NotRequired[str],
    provider: NotRequired[str],
```

## CreateEnvironmentProfilePolicyGrantDetailTypeDef

```python
# CreateEnvironmentProfilePolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateEnvironmentProfilePolicyGrantDetailTypeDef


def get_value() -> CreateEnvironmentProfilePolicyGrantDetailTypeDef:
    return {
        "domainUnitId": ...,
    }


# CreateEnvironmentProfilePolicyGrantDetailTypeDef definition

class CreateEnvironmentProfilePolicyGrantDetailTypeDef(TypedDict):
    domainUnitId: NotRequired[str],
```

## ModelTypeDef

```python
# ModelTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ModelTypeDef


def get_value() -> ModelTypeDef:
    return {
        "smithy": ...,
    }


# ModelTypeDef definition

class ModelTypeDef(TypedDict):
    smithy: NotRequired[str],
```

## CreateFormTypePolicyGrantDetailTypeDef

```python
# CreateFormTypePolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateFormTypePolicyGrantDetailTypeDef


def get_value() -> CreateFormTypePolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# CreateFormTypePolicyGrantDetailTypeDef definition

class CreateFormTypePolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## CreateGlossaryInputTypeDef

```python
# CreateGlossaryInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateGlossaryInputTypeDef


def get_value() -> CreateGlossaryInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateGlossaryInputTypeDef definition

class CreateGlossaryInputTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    owningProjectIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    status: NotRequired[GlossaryStatusType],  # (1)
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
## CreateGlossaryPolicyGrantDetailTypeDef

```python
# CreateGlossaryPolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateGlossaryPolicyGrantDetailTypeDef


def get_value() -> CreateGlossaryPolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# CreateGlossaryPolicyGrantDetailTypeDef definition

class CreateGlossaryPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## TermRelationsOutputTypeDef

```python
# TermRelationsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import TermRelationsOutputTypeDef


def get_value() -> TermRelationsOutputTypeDef:
    return {
        "classifies": ...,
    }


# TermRelationsOutputTypeDef definition

class TermRelationsOutputTypeDef(TypedDict):
    classifies: NotRequired[List[str]],
    isA: NotRequired[List[str]],
```

## CreateGroupProfileInputTypeDef

```python
# CreateGroupProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateGroupProfileInputTypeDef


def get_value() -> CreateGroupProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateGroupProfileInputTypeDef definition

class CreateGroupProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: str,
    clientToken: NotRequired[str],
```

## CreateListingChangeSetInputTypeDef

```python
# CreateListingChangeSetInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateListingChangeSetInputTypeDef


def get_value() -> CreateListingChangeSetInputTypeDef:
    return {
        "action": ...,
    }


# CreateListingChangeSetInputTypeDef definition

class CreateListingChangeSetInputTypeDef(TypedDict):
    action: ChangeActionType,  # (1)
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: EntityTypeType,  # (2)
    clientToken: NotRequired[str],
    entityRevision: NotRequired[str],
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
## CreateProjectFromProjectProfilePolicyGrantDetailOutputTypeDef

```python
# CreateProjectFromProjectProfilePolicyGrantDetailOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateProjectFromProjectProfilePolicyGrantDetailOutputTypeDef


def get_value() -> CreateProjectFromProjectProfilePolicyGrantDetailOutputTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# CreateProjectFromProjectProfilePolicyGrantDetailOutputTypeDef definition

class CreateProjectFromProjectProfilePolicyGrantDetailOutputTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
    projectProfiles: NotRequired[List[str]],
```

## CreateProjectFromProjectProfilePolicyGrantDetailTypeDef

```python
# CreateProjectFromProjectProfilePolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateProjectFromProjectProfilePolicyGrantDetailTypeDef


def get_value() -> CreateProjectFromProjectProfilePolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# CreateProjectFromProjectProfilePolicyGrantDetailTypeDef definition

class CreateProjectFromProjectProfilePolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
    projectProfiles: NotRequired[Sequence[str]],
```

## MemberTypeDef

```python
# MemberTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import MemberTypeDef


def get_value() -> MemberTypeDef:
    return {
        "groupIdentifier": ...,
    }


# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    groupIdentifier: NotRequired[str],
    userIdentifier: NotRequired[str],
```

## ProjectDeletionErrorTypeDef

```python
# ProjectDeletionErrorTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProjectDeletionErrorTypeDef


def get_value() -> ProjectDeletionErrorTypeDef:
    return {
        "code": ...,
    }


# ProjectDeletionErrorTypeDef definition

class ProjectDeletionErrorTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```

## CreateProjectPolicyGrantDetailTypeDef

```python
# CreateProjectPolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateProjectPolicyGrantDetailTypeDef


def get_value() -> CreateProjectPolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# CreateProjectPolicyGrantDetailTypeDef definition

class CreateProjectPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## SubscribedListingInputTypeDef

```python
# SubscribedListingInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedListingInputTypeDef


def get_value() -> SubscribedListingInputTypeDef:
    return {
        "identifier": ...,
    }


# SubscribedListingInputTypeDef definition

class SubscribedListingInputTypeDef(TypedDict):
    identifier: str,
```

## SubscriptionTargetFormTypeDef

```python
# SubscriptionTargetFormTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscriptionTargetFormTypeDef


def get_value() -> SubscriptionTargetFormTypeDef:
    return {
        "content": ...,
    }


# SubscriptionTargetFormTypeDef definition

class SubscriptionTargetFormTypeDef(TypedDict):
    content: str,
    formName: str,
```

## CreateUserProfileInputTypeDef

```python
# CreateUserProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateUserProfileInputTypeDef


def get_value() -> CreateUserProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateUserProfileInputTypeDef definition

class CreateUserProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    userIdentifier: str,
    clientToken: NotRequired[str],
    userType: NotRequired[UserTypeType],  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## DataProductItemTypeDef

```python
# DataProductItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataProductItemTypeDef


def get_value() -> DataProductItemTypeDef:
    return {
        "glossaryTerms": ...,
    }


# DataProductItemTypeDef definition

class DataProductItemTypeDef(TypedDict):
    identifier: str,
    itemType: DataProductItemTypeType,  # (1)
    glossaryTerms: NotRequired[Sequence[str]],
    revision: NotRequired[str],
```

1. See [:material-code-brackets: DataProductItemTypeType](./literals.md#dataproductitemtypetype) 
## DataProductListingItemAdditionalAttributesTypeDef

```python
# DataProductListingItemAdditionalAttributesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataProductListingItemAdditionalAttributesTypeDef


def get_value() -> DataProductListingItemAdditionalAttributesTypeDef:
    return {
        "forms": ...,
    }


# DataProductListingItemAdditionalAttributesTypeDef definition

class DataProductListingItemAdditionalAttributesTypeDef(TypedDict):
    forms: NotRequired[str],
```

## DataProductResultItemTypeDef

```python
# DataProductResultItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataProductResultItemTypeDef


def get_value() -> DataProductResultItemTypeDef:
    return {
        "createdAt": ...,
    }


# DataProductResultItemTypeDef definition

class DataProductResultItemTypeDef(TypedDict):
    domainId: str,
    id: str,
    name: str,
    owningProjectId: str,
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    firstRevisionCreatedAt: NotRequired[datetime],
    firstRevisionCreatedBy: NotRequired[str],
    glossaryTerms: NotRequired[List[str]],
```

## DataProductRevisionTypeDef

```python
# DataProductRevisionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataProductRevisionTypeDef


def get_value() -> DataProductRevisionTypeDef:
    return {
        "createdAt": ...,
    }


# DataProductRevisionTypeDef definition

class DataProductRevisionTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    domainId: NotRequired[str],
    id: NotRequired[str],
    revision: NotRequired[str],
```

## SageMakerRunConfigurationInputTypeDef

```python
# SageMakerRunConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SageMakerRunConfigurationInputTypeDef


def get_value() -> SageMakerRunConfigurationInputTypeDef:
    return {
        "trackingAssets": ...,
    }


# SageMakerRunConfigurationInputTypeDef definition

class SageMakerRunConfigurationInputTypeDef(TypedDict):
    trackingAssets: Mapping[str, Sequence[str]],
```

## SageMakerRunConfigurationOutputTypeDef

```python
# SageMakerRunConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SageMakerRunConfigurationOutputTypeDef


def get_value() -> SageMakerRunConfigurationOutputTypeDef:
    return {
        "accountId": ...,
    }


# SageMakerRunConfigurationOutputTypeDef definition

class SageMakerRunConfigurationOutputTypeDef(TypedDict):
    trackingAssets: Dict[str, List[str]],
    accountId: NotRequired[str],
    region: NotRequired[str],
```

## LineageInfoTypeDef

```python
# LineageInfoTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LineageInfoTypeDef


def get_value() -> LineageInfoTypeDef:
    return {
        "errorMessage": ...,
    }


# LineageInfoTypeDef definition

class LineageInfoTypeDef(TypedDict):
    errorMessage: NotRequired[str],
    eventId: NotRequired[str],
    eventStatus: NotRequired[LineageEventProcessingStatusType],  # (1)
```

1. See [:material-code-brackets: LineageEventProcessingStatusType](./literals.md#lineageeventprocessingstatustype) 
## DataSourceRunLineageSummaryTypeDef

```python
# DataSourceRunLineageSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataSourceRunLineageSummaryTypeDef


def get_value() -> DataSourceRunLineageSummaryTypeDef:
    return {
        "importStatus": ...,
    }


# DataSourceRunLineageSummaryTypeDef definition

class DataSourceRunLineageSummaryTypeDef(TypedDict):
    importStatus: NotRequired[LineageImportStatusType],  # (1)
```

1. See [:material-code-brackets: LineageImportStatusType](./literals.md#lineageimportstatustype) 
## RunStatisticsForAssetsTypeDef

```python
# RunStatisticsForAssetsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RunStatisticsForAssetsTypeDef


def get_value() -> RunStatisticsForAssetsTypeDef:
    return {
        "added": ...,
    }


# RunStatisticsForAssetsTypeDef definition

class RunStatisticsForAssetsTypeDef(TypedDict):
    added: NotRequired[int],
    failed: NotRequired[int],
    skipped: NotRequired[int],
    unchanged: NotRequired[int],
    updated: NotRequired[int],
```

## DeleteAssetFilterInputTypeDef

```python
# DeleteAssetFilterInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteAssetFilterInputTypeDef


def get_value() -> DeleteAssetFilterInputTypeDef:
    return {
        "assetIdentifier": ...,
    }


# DeleteAssetFilterInputTypeDef definition

class DeleteAssetFilterInputTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    identifier: str,
```

## DeleteAssetInputTypeDef

```python
# DeleteAssetInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteAssetInputTypeDef


def get_value() -> DeleteAssetInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteAssetInputTypeDef definition

class DeleteAssetInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteAssetTypeInputTypeDef

```python
# DeleteAssetTypeInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteAssetTypeInputTypeDef


def get_value() -> DeleteAssetTypeInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteAssetTypeInputTypeDef definition

class DeleteAssetTypeInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteConnectionInputTypeDef

```python
# DeleteConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteConnectionInputTypeDef


def get_value() -> DeleteConnectionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteConnectionInputTypeDef definition

class DeleteConnectionInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteDataProductInputTypeDef

```python
# DeleteDataProductInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteDataProductInputTypeDef


def get_value() -> DeleteDataProductInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteDataProductInputTypeDef definition

class DeleteDataProductInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteDataSourceInputTypeDef

```python
# DeleteDataSourceInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteDataSourceInputTypeDef


def get_value() -> DeleteDataSourceInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteDataSourceInputTypeDef definition

class DeleteDataSourceInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    clientToken: NotRequired[str],
    retainPermissionsOnRevokeFailure: NotRequired[bool],
```

## DeleteDomainInputTypeDef

```python
# DeleteDomainInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteDomainInputTypeDef


def get_value() -> DeleteDomainInputTypeDef:
    return {
        "identifier": ...,
    }


# DeleteDomainInputTypeDef definition

class DeleteDomainInputTypeDef(TypedDict):
    identifier: str,
    clientToken: NotRequired[str],
    skipDeletionCheck: NotRequired[bool],
```

## DeleteDomainUnitInputTypeDef

```python
# DeleteDomainUnitInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteDomainUnitInputTypeDef


def get_value() -> DeleteDomainUnitInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteDomainUnitInputTypeDef definition

class DeleteDomainUnitInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteEnvironmentActionInputTypeDef

```python
# DeleteEnvironmentActionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteEnvironmentActionInputTypeDef


def get_value() -> DeleteEnvironmentActionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteEnvironmentActionInputTypeDef definition

class DeleteEnvironmentActionInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
```

## DeleteEnvironmentBlueprintConfigurationInputTypeDef

```python
# DeleteEnvironmentBlueprintConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteEnvironmentBlueprintConfigurationInputTypeDef


def get_value() -> DeleteEnvironmentBlueprintConfigurationInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteEnvironmentBlueprintConfigurationInputTypeDef definition

class DeleteEnvironmentBlueprintConfigurationInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentBlueprintIdentifier: str,
```

## DeleteEnvironmentInputTypeDef

```python
# DeleteEnvironmentInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteEnvironmentInputTypeDef


def get_value() -> DeleteEnvironmentInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteEnvironmentInputTypeDef definition

class DeleteEnvironmentInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteEnvironmentProfileInputTypeDef

```python
# DeleteEnvironmentProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteEnvironmentProfileInputTypeDef


def get_value() -> DeleteEnvironmentProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteEnvironmentProfileInputTypeDef definition

class DeleteEnvironmentProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteFormTypeInputTypeDef

```python
# DeleteFormTypeInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteFormTypeInputTypeDef


def get_value() -> DeleteFormTypeInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteFormTypeInputTypeDef definition

class DeleteFormTypeInputTypeDef(TypedDict):
    domainIdentifier: str,
    formTypeIdentifier: str,
```

## DeleteGlossaryInputTypeDef

```python
# DeleteGlossaryInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteGlossaryInputTypeDef


def get_value() -> DeleteGlossaryInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteGlossaryInputTypeDef definition

class DeleteGlossaryInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteGlossaryTermInputTypeDef

```python
# DeleteGlossaryTermInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteGlossaryTermInputTypeDef


def get_value() -> DeleteGlossaryTermInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteGlossaryTermInputTypeDef definition

class DeleteGlossaryTermInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteListingInputTypeDef

```python
# DeleteListingInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteListingInputTypeDef


def get_value() -> DeleteListingInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteListingInputTypeDef definition

class DeleteListingInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteProjectInputTypeDef

```python
# DeleteProjectInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteProjectInputTypeDef


def get_value() -> DeleteProjectInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteProjectInputTypeDef definition

class DeleteProjectInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    skipDeletionCheck: NotRequired[bool],
```

## DeleteProjectProfileInputTypeDef

```python
# DeleteProjectProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteProjectProfileInputTypeDef


def get_value() -> DeleteProjectProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteProjectProfileInputTypeDef definition

class DeleteProjectProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteRuleInputTypeDef

```python
# DeleteRuleInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteRuleInputTypeDef


def get_value() -> DeleteRuleInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteRuleInputTypeDef definition

class DeleteRuleInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteSubscriptionGrantInputTypeDef

```python
# DeleteSubscriptionGrantInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteSubscriptionGrantInputTypeDef


def get_value() -> DeleteSubscriptionGrantInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteSubscriptionGrantInputTypeDef definition

class DeleteSubscriptionGrantInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteSubscriptionRequestInputTypeDef

```python
# DeleteSubscriptionRequestInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteSubscriptionRequestInputTypeDef


def get_value() -> DeleteSubscriptionRequestInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteSubscriptionRequestInputTypeDef definition

class DeleteSubscriptionRequestInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteSubscriptionTargetInputTypeDef

```python
# DeleteSubscriptionTargetInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteSubscriptionTargetInputTypeDef


def get_value() -> DeleteSubscriptionTargetInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteSubscriptionTargetInputTypeDef definition

class DeleteSubscriptionTargetInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
```

## DeleteTimeSeriesDataPointsInputTypeDef

```python
# DeleteTimeSeriesDataPointsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteTimeSeriesDataPointsInputTypeDef


def get_value() -> DeleteTimeSeriesDataPointsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteTimeSeriesDataPointsInputTypeDef definition

class DeleteTimeSeriesDataPointsInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    formName: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
## EnvironmentErrorTypeDef

```python
# EnvironmentErrorTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentErrorTypeDef


def get_value() -> EnvironmentErrorTypeDef:
    return {
        "code": ...,
    }


# EnvironmentErrorTypeDef definition

class EnvironmentErrorTypeDef(TypedDict):
    message: str,
    code: NotRequired[str],
```

## DisassociateEnvironmentRoleInputTypeDef

```python
# DisassociateEnvironmentRoleInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DisassociateEnvironmentRoleInputTypeDef


def get_value() -> DisassociateEnvironmentRoleInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DisassociateEnvironmentRoleInputTypeDef definition

class DisassociateEnvironmentRoleInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    environmentRoleArn: str,
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainSummaryTypeDef


def get_value() -> DomainSummaryTypeDef:
    return {
        "arn": ...,
    }


# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    id: str,
    managedAccountId: str,
    name: str,
    status: DomainStatusType,  # (2)
    description: NotRequired[str],
    domainVersion: NotRequired[DomainVersionType],  # (1)
    lastUpdatedAt: NotRequired[datetime],
    portalUrl: NotRequired[str],
```

1. See [:material-code-brackets: DomainVersionType](./literals.md#domainversiontype) 
2. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
## DomainUnitFilterForProjectTypeDef

```python
# DomainUnitFilterForProjectTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitFilterForProjectTypeDef


def get_value() -> DomainUnitFilterForProjectTypeDef:
    return {
        "domainUnit": ...,
    }


# DomainUnitFilterForProjectTypeDef definition

class DomainUnitFilterForProjectTypeDef(TypedDict):
    domainUnit: str,
    includeChildDomainUnits: NotRequired[bool],
```

## DomainUnitGrantFilterOutputTypeDef

```python
# DomainUnitGrantFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitGrantFilterOutputTypeDef


def get_value() -> DomainUnitGrantFilterOutputTypeDef:
    return {
        "allDomainUnitsGrantFilter": ...,
    }


# DomainUnitGrantFilterOutputTypeDef definition

class DomainUnitGrantFilterOutputTypeDef(TypedDict):
    allDomainUnitsGrantFilter: NotRequired[Dict[str, Any]],
```

## DomainUnitGrantFilterTypeDef

```python
# DomainUnitGrantFilterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitGrantFilterTypeDef


def get_value() -> DomainUnitGrantFilterTypeDef:
    return {
        "allDomainUnitsGrantFilter": ...,
    }


# DomainUnitGrantFilterTypeDef definition

class DomainUnitGrantFilterTypeDef(TypedDict):
    allDomainUnitsGrantFilter: NotRequired[Mapping[str, Any]],
```

## DomainUnitGroupPropertiesTypeDef

```python
# DomainUnitGroupPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitGroupPropertiesTypeDef


def get_value() -> DomainUnitGroupPropertiesTypeDef:
    return {
        "groupId": ...,
    }


# DomainUnitGroupPropertiesTypeDef definition

class DomainUnitGroupPropertiesTypeDef(TypedDict):
    groupId: NotRequired[str],
```

## DomainUnitUserPropertiesTypeDef

```python
# DomainUnitUserPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitUserPropertiesTypeDef


def get_value() -> DomainUnitUserPropertiesTypeDef:
    return {
        "userId": ...,
    }


# DomainUnitUserPropertiesTypeDef definition

class DomainUnitUserPropertiesTypeDef(TypedDict):
    userId: NotRequired[str],
```

## DomainUnitSummaryTypeDef

```python
# DomainUnitSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitSummaryTypeDef


def get_value() -> DomainUnitSummaryTypeDef:
    return {
        "id": ...,
    }


# DomainUnitSummaryTypeDef definition

class DomainUnitSummaryTypeDef(TypedDict):
    id: str,
    name: str,
```

## DomainUnitTargetTypeDef

```python
# DomainUnitTargetTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitTargetTypeDef


def get_value() -> DomainUnitTargetTypeDef:
    return {
        "domainUnitId": ...,
    }


# DomainUnitTargetTypeDef definition

class DomainUnitTargetTypeDef(TypedDict):
    domainUnitId: str,
    includeChildDomainUnits: NotRequired[bool],
```

## RegionTypeDef

```python
# RegionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RegionTypeDef


def get_value() -> RegionTypeDef:
    return {
        "regionName": ...,
    }


# RegionTypeDef definition

class RegionTypeDef(TypedDict):
    regionName: NotRequired[str],
    regionNamePath: NotRequired[str],
```

## EnvironmentConfigurationParameterTypeDef

```python
# EnvironmentConfigurationParameterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationParameterTypeDef


def get_value() -> EnvironmentConfigurationParameterTypeDef:
    return {
        "isEditable": ...,
    }


# EnvironmentConfigurationParameterTypeDef definition

class EnvironmentConfigurationParameterTypeDef(TypedDict):
    isEditable: NotRequired[bool],
    name: NotRequired[str],
    value: NotRequired[str],
```

## EnvironmentProfileSummaryTypeDef

```python
# EnvironmentProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentProfileSummaryTypeDef


def get_value() -> EnvironmentProfileSummaryTypeDef:
    return {
        "awsAccountId": ...,
    }


# EnvironmentProfileSummaryTypeDef definition

class EnvironmentProfileSummaryTypeDef(TypedDict):
    createdBy: str,
    domainId: str,
    environmentBlueprintId: str,
    id: str,
    name: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    projectId: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

## EnvironmentSummaryTypeDef

```python
# EnvironmentSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentSummaryTypeDef


def get_value() -> EnvironmentSummaryTypeDef:
    return {
        "awsAccountId": ...,
    }


# EnvironmentSummaryTypeDef definition

class EnvironmentSummaryTypeDef(TypedDict):
    createdBy: str,
    domainId: str,
    name: str,
    projectId: str,
    provider: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    environmentProfileId: NotRequired[str],
    id: NotRequired[str],
    status: NotRequired[EnvironmentStatusType],  # (1)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
## EqualToExpressionTypeDef

```python
# EqualToExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EqualToExpressionTypeDef


def get_value() -> EqualToExpressionTypeDef:
    return {
        "columnName": ...,
    }


# EqualToExpressionTypeDef definition

class EqualToExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## FailureCauseTypeDef

```python
# FailureCauseTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FailureCauseTypeDef


def get_value() -> FailureCauseTypeDef:
    return {
        "message": ...,
    }


# FailureCauseTypeDef definition

class FailureCauseTypeDef(TypedDict):
    message: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FilterTypeDef


def get_value() -> FilterTypeDef:
    return {
        "attribute": ...,
    }


# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    attribute: str,
    value: str,
```

## FilterExpressionTypeDef

```python
# FilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FilterExpressionTypeDef


def get_value() -> FilterExpressionTypeDef:
    return {
        "expression": ...,
    }


# FilterExpressionTypeDef definition

class FilterExpressionTypeDef(TypedDict):
    expression: str,
    type: FilterExpressionTypeType,  # (1)
```

1. See [:material-code-brackets: FilterExpressionTypeType](./literals.md#filterexpressiontypetype) 
## ImportTypeDef

```python
# ImportTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ImportTypeDef


def get_value() -> ImportTypeDef:
    return {
        "name": ...,
    }


# ImportTypeDef definition

class ImportTypeDef(TypedDict):
    name: str,
    revision: str,
```

## GetAssetFilterInputTypeDef

```python
# GetAssetFilterInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetAssetFilterInputTypeDef


def get_value() -> GetAssetFilterInputTypeDef:
    return {
        "assetIdentifier": ...,
    }


# GetAssetFilterInputTypeDef definition

class GetAssetFilterInputTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    identifier: str,
```

## GetAssetInputTypeDef

```python
# GetAssetInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetAssetInputTypeDef


def get_value() -> GetAssetInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetAssetInputTypeDef definition

class GetAssetInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    revision: NotRequired[str],
```

## GetAssetTypeInputTypeDef

```python
# GetAssetTypeInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetAssetTypeInputTypeDef


def get_value() -> GetAssetTypeInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetAssetTypeInputTypeDef definition

class GetAssetTypeInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    revision: NotRequired[str],
```

## GetConnectionInputTypeDef

```python
# GetConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetConnectionInputTypeDef


def get_value() -> GetConnectionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetConnectionInputTypeDef definition

class GetConnectionInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    withSecret: NotRequired[bool],
```

## GetDataProductInputTypeDef

```python
# GetDataProductInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDataProductInputTypeDef


def get_value() -> GetDataProductInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetDataProductInputTypeDef definition

class GetDataProductInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    revision: NotRequired[str],
```

## GetDataSourceInputTypeDef

```python
# GetDataSourceInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDataSourceInputTypeDef


def get_value() -> GetDataSourceInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetDataSourceInputTypeDef definition

class GetDataSourceInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetDataSourceRunInputTypeDef

```python
# GetDataSourceRunInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDataSourceRunInputTypeDef


def get_value() -> GetDataSourceRunInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetDataSourceRunInputTypeDef definition

class GetDataSourceRunInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetDomainInputTypeDef

```python
# GetDomainInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDomainInputTypeDef


def get_value() -> GetDomainInputTypeDef:
    return {
        "identifier": ...,
    }


# GetDomainInputTypeDef definition

class GetDomainInputTypeDef(TypedDict):
    identifier: str,
```

## GetDomainUnitInputTypeDef

```python
# GetDomainUnitInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDomainUnitInputTypeDef


def get_value() -> GetDomainUnitInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetDomainUnitInputTypeDef definition

class GetDomainUnitInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetEnvironmentActionInputTypeDef

```python
# GetEnvironmentActionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentActionInputTypeDef


def get_value() -> GetEnvironmentActionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetEnvironmentActionInputTypeDef definition

class GetEnvironmentActionInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
```

## GetEnvironmentBlueprintConfigurationInputTypeDef

```python
# GetEnvironmentBlueprintConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentBlueprintConfigurationInputTypeDef


def get_value() -> GetEnvironmentBlueprintConfigurationInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetEnvironmentBlueprintConfigurationInputTypeDef definition

class GetEnvironmentBlueprintConfigurationInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentBlueprintIdentifier: str,
```

## GetEnvironmentBlueprintInputTypeDef

```python
# GetEnvironmentBlueprintInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentBlueprintInputTypeDef


def get_value() -> GetEnvironmentBlueprintInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetEnvironmentBlueprintInputTypeDef definition

class GetEnvironmentBlueprintInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetEnvironmentCredentialsInputTypeDef

```python
# GetEnvironmentCredentialsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentCredentialsInputTypeDef


def get_value() -> GetEnvironmentCredentialsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetEnvironmentCredentialsInputTypeDef definition

class GetEnvironmentCredentialsInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
```

## GetEnvironmentInputTypeDef

```python
# GetEnvironmentInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentInputTypeDef


def get_value() -> GetEnvironmentInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetEnvironmentInputTypeDef definition

class GetEnvironmentInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetEnvironmentProfileInputTypeDef

```python
# GetEnvironmentProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentProfileInputTypeDef


def get_value() -> GetEnvironmentProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetEnvironmentProfileInputTypeDef definition

class GetEnvironmentProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetFormTypeInputTypeDef

```python
# GetFormTypeInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetFormTypeInputTypeDef


def get_value() -> GetFormTypeInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetFormTypeInputTypeDef definition

class GetFormTypeInputTypeDef(TypedDict):
    domainIdentifier: str,
    formTypeIdentifier: str,
    revision: NotRequired[str],
```

## GetGlossaryInputTypeDef

```python
# GetGlossaryInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetGlossaryInputTypeDef


def get_value() -> GetGlossaryInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetGlossaryInputTypeDef definition

class GetGlossaryInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetGlossaryTermInputTypeDef

```python
# GetGlossaryTermInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetGlossaryTermInputTypeDef


def get_value() -> GetGlossaryTermInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetGlossaryTermInputTypeDef definition

class GetGlossaryTermInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetGroupProfileInputTypeDef

```python
# GetGroupProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetGroupProfileInputTypeDef


def get_value() -> GetGroupProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetGroupProfileInputTypeDef definition

class GetGroupProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: str,
```

## GetIamPortalLoginUrlInputTypeDef

```python
# GetIamPortalLoginUrlInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetIamPortalLoginUrlInputTypeDef


def get_value() -> GetIamPortalLoginUrlInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetIamPortalLoginUrlInputTypeDef definition

class GetIamPortalLoginUrlInputTypeDef(TypedDict):
    domainIdentifier: str,
```

## GetJobRunInputTypeDef

```python
# GetJobRunInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetJobRunInputTypeDef


def get_value() -> GetJobRunInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetJobRunInputTypeDef definition

class GetJobRunInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## JobRunErrorTypeDef

```python
# JobRunErrorTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import JobRunErrorTypeDef


def get_value() -> JobRunErrorTypeDef:
    return {
        "message": ...,
    }


# JobRunErrorTypeDef definition

class JobRunErrorTypeDef(TypedDict):
    message: str,
```

## GetLineageEventInputTypeDef

```python
# GetLineageEventInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetLineageEventInputTypeDef


def get_value() -> GetLineageEventInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetLineageEventInputTypeDef definition

class GetLineageEventInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## LineageNodeReferenceTypeDef

```python
# LineageNodeReferenceTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LineageNodeReferenceTypeDef


def get_value() -> LineageNodeReferenceTypeDef:
    return {
        "eventTimestamp": ...,
    }


# LineageNodeReferenceTypeDef definition

class LineageNodeReferenceTypeDef(TypedDict):
    eventTimestamp: NotRequired[datetime],
    id: NotRequired[str],
```

## GetListingInputTypeDef

```python
# GetListingInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetListingInputTypeDef


def get_value() -> GetListingInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetListingInputTypeDef definition

class GetListingInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    listingRevision: NotRequired[str],
```

## GetMetadataGenerationRunInputTypeDef

```python
# GetMetadataGenerationRunInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetMetadataGenerationRunInputTypeDef


def get_value() -> GetMetadataGenerationRunInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetMetadataGenerationRunInputTypeDef definition

class GetMetadataGenerationRunInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## MetadataGenerationRunTargetTypeDef

```python
# MetadataGenerationRunTargetTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import MetadataGenerationRunTargetTypeDef


def get_value() -> MetadataGenerationRunTargetTypeDef:
    return {
        "identifier": ...,
    }


# MetadataGenerationRunTargetTypeDef definition

class MetadataGenerationRunTargetTypeDef(TypedDict):
    identifier: str,
    type: MetadataGenerationTargetTypeType,  # (1)
    revision: NotRequired[str],
```

1. See [:material-code-brackets: MetadataGenerationTargetTypeType](./literals.md#metadatagenerationtargettypetype) 
## GetProjectInputTypeDef

```python
# GetProjectInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetProjectInputTypeDef


def get_value() -> GetProjectInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetProjectInputTypeDef definition

class GetProjectInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetProjectProfileInputTypeDef

```python
# GetProjectProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetProjectProfileInputTypeDef


def get_value() -> GetProjectProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetProjectProfileInputTypeDef definition

class GetProjectProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetRuleInputTypeDef

```python
# GetRuleInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetRuleInputTypeDef


def get_value() -> GetRuleInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetRuleInputTypeDef definition

class GetRuleInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    revision: NotRequired[str],
```

## GetSubscriptionGrantInputTypeDef

```python
# GetSubscriptionGrantInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetSubscriptionGrantInputTypeDef


def get_value() -> GetSubscriptionGrantInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetSubscriptionGrantInputTypeDef definition

class GetSubscriptionGrantInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetSubscriptionInputTypeDef

```python
# GetSubscriptionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetSubscriptionInputTypeDef


def get_value() -> GetSubscriptionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetSubscriptionInputTypeDef definition

class GetSubscriptionInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetSubscriptionRequestDetailsInputTypeDef

```python
# GetSubscriptionRequestDetailsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetSubscriptionRequestDetailsInputTypeDef


def get_value() -> GetSubscriptionRequestDetailsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetSubscriptionRequestDetailsInputTypeDef definition

class GetSubscriptionRequestDetailsInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetSubscriptionTargetInputTypeDef

```python
# GetSubscriptionTargetInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetSubscriptionTargetInputTypeDef


def get_value() -> GetSubscriptionTargetInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetSubscriptionTargetInputTypeDef definition

class GetSubscriptionTargetInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
```

## GetTimeSeriesDataPointInputTypeDef

```python
# GetTimeSeriesDataPointInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetTimeSeriesDataPointInputTypeDef


def get_value() -> GetTimeSeriesDataPointInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetTimeSeriesDataPointInputTypeDef definition

class GetTimeSeriesDataPointInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    formName: str,
    identifier: str,
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
## TimeSeriesDataPointFormOutputTypeDef

```python
# TimeSeriesDataPointFormOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import TimeSeriesDataPointFormOutputTypeDef


def get_value() -> TimeSeriesDataPointFormOutputTypeDef:
    return {
        "content": ...,
    }


# TimeSeriesDataPointFormOutputTypeDef definition

class TimeSeriesDataPointFormOutputTypeDef(TypedDict):
    formName: str,
    timestamp: datetime,
    typeIdentifier: str,
    content: NotRequired[str],
    id: NotRequired[str],
    typeRevision: NotRequired[str],
```

## GetUserProfileInputTypeDef

```python
# GetUserProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetUserProfileInputTypeDef


def get_value() -> GetUserProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetUserProfileInputTypeDef definition

class GetUserProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    userIdentifier: str,
    type: NotRequired[UserProfileTypeType],  # (1)
```

1. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
## GlossaryItemTypeDef

```python
# GlossaryItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlossaryItemTypeDef


def get_value() -> GlossaryItemTypeDef:
    return {
        "createdAt": ...,
    }


# GlossaryItemTypeDef definition

class GlossaryItemTypeDef(TypedDict):
    domainId: str,
    id: str,
    name: str,
    owningProjectId: str,
    status: GlossaryStatusType,  # (1)
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
## PhysicalConnectionRequirementsOutputTypeDef

```python
# PhysicalConnectionRequirementsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PhysicalConnectionRequirementsOutputTypeDef


def get_value() -> PhysicalConnectionRequirementsOutputTypeDef:
    return {
        "availabilityZone": ...,
    }


# PhysicalConnectionRequirementsOutputTypeDef definition

class PhysicalConnectionRequirementsOutputTypeDef(TypedDict):
    availabilityZone: NotRequired[str],
    securityGroupIdList: NotRequired[List[str]],
    subnetId: NotRequired[str],
    subnetIdList: NotRequired[List[str]],
```

## GlueOAuth2CredentialsTypeDef

```python
# GlueOAuth2CredentialsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlueOAuth2CredentialsTypeDef


def get_value() -> GlueOAuth2CredentialsTypeDef:
    return {
        "accessToken": ...,
    }


# GlueOAuth2CredentialsTypeDef definition

class GlueOAuth2CredentialsTypeDef(TypedDict):
    accessToken: NotRequired[str],
    jwtToken: NotRequired[str],
    refreshToken: NotRequired[str],
    userManagedClientApplicationClientSecret: NotRequired[str],
```

## SelfGrantStatusDetailTypeDef

```python
# SelfGrantStatusDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SelfGrantStatusDetailTypeDef


def get_value() -> SelfGrantStatusDetailTypeDef:
    return {
        "databaseName": ...,
    }


# SelfGrantStatusDetailTypeDef definition

class SelfGrantStatusDetailTypeDef(TypedDict):
    databaseName: str,
    status: SelfGrantStatusType,  # (1)
    failureCause: NotRequired[str],
    schemaName: NotRequired[str],
```

1. See [:material-code-brackets: SelfGrantStatusType](./literals.md#selfgrantstatustype) 
## ListingRevisionInputTypeDef

```python
# ListingRevisionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListingRevisionInputTypeDef


def get_value() -> ListingRevisionInputTypeDef:
    return {
        "identifier": ...,
    }


# ListingRevisionInputTypeDef definition

class ListingRevisionInputTypeDef(TypedDict):
    identifier: str,
    revision: str,
```

## ListingRevisionTypeDef

```python
# ListingRevisionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListingRevisionTypeDef


def get_value() -> ListingRevisionTypeDef:
    return {
        "id": ...,
    }


# ListingRevisionTypeDef definition

class ListingRevisionTypeDef(TypedDict):
    id: str,
    revision: str,
```

## GreaterThanExpressionTypeDef

```python
# GreaterThanExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GreaterThanExpressionTypeDef


def get_value() -> GreaterThanExpressionTypeDef:
    return {
        "columnName": ...,
    }


# GreaterThanExpressionTypeDef definition

class GreaterThanExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## GreaterThanOrEqualToExpressionTypeDef

```python
# GreaterThanOrEqualToExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GreaterThanOrEqualToExpressionTypeDef


def get_value() -> GreaterThanOrEqualToExpressionTypeDef:
    return {
        "columnName": ...,
    }


# GreaterThanOrEqualToExpressionTypeDef definition

class GreaterThanOrEqualToExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## GroupDetailsTypeDef

```python
# GroupDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GroupDetailsTypeDef


def get_value() -> GroupDetailsTypeDef:
    return {
        "groupId": ...,
    }


# GroupDetailsTypeDef definition

class GroupDetailsTypeDef(TypedDict):
    groupId: str,
```

## GroupPolicyGrantPrincipalTypeDef

```python
# GroupPolicyGrantPrincipalTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GroupPolicyGrantPrincipalTypeDef


def get_value() -> GroupPolicyGrantPrincipalTypeDef:
    return {
        "groupIdentifier": ...,
    }


# GroupPolicyGrantPrincipalTypeDef definition

class GroupPolicyGrantPrincipalTypeDef(TypedDict):
    groupIdentifier: NotRequired[str],
```

## GroupProfileSummaryTypeDef

```python
# GroupProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GroupProfileSummaryTypeDef


def get_value() -> GroupProfileSummaryTypeDef:
    return {
        "domainId": ...,
    }


# GroupProfileSummaryTypeDef definition

class GroupProfileSummaryTypeDef(TypedDict):
    domainId: NotRequired[str],
    groupName: NotRequired[str],
    id: NotRequired[str],
    status: NotRequired[GroupProfileStatusType],  # (1)
```

1. See [:material-code-brackets: GroupProfileStatusType](./literals.md#groupprofilestatustype) 
## IamUserProfileDetailsTypeDef

```python
# IamUserProfileDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import IamUserProfileDetailsTypeDef


def get_value() -> IamUserProfileDetailsTypeDef:
    return {
        "arn": ...,
    }


# IamUserProfileDetailsTypeDef definition

class IamUserProfileDetailsTypeDef(TypedDict):
    arn: NotRequired[str],
```

## InExpressionOutputTypeDef

```python
# InExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import InExpressionOutputTypeDef


def get_value() -> InExpressionOutputTypeDef:
    return {
        "columnName": ...,
    }


# InExpressionOutputTypeDef definition

class InExpressionOutputTypeDef(TypedDict):
    columnName: str,
    values: List[str],
```

## InExpressionTypeDef

```python
# InExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import InExpressionTypeDef


def get_value() -> InExpressionTypeDef:
    return {
        "columnName": ...,
    }


# InExpressionTypeDef definition

class InExpressionTypeDef(TypedDict):
    columnName: str,
    values: Sequence[str],
```

## IsNotNullExpressionTypeDef

```python
# IsNotNullExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import IsNotNullExpressionTypeDef


def get_value() -> IsNotNullExpressionTypeDef:
    return {
        "columnName": ...,
    }


# IsNotNullExpressionTypeDef definition

class IsNotNullExpressionTypeDef(TypedDict):
    columnName: str,
```

## IsNullExpressionTypeDef

```python
# IsNullExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import IsNullExpressionTypeDef


def get_value() -> IsNullExpressionTypeDef:
    return {
        "columnName": ...,
    }


# IsNullExpressionTypeDef definition

class IsNullExpressionTypeDef(TypedDict):
    columnName: str,
```

## LakeFormationConfigurationOutputTypeDef

```python
# LakeFormationConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LakeFormationConfigurationOutputTypeDef


def get_value() -> LakeFormationConfigurationOutputTypeDef:
    return {
        "locationRegistrationExcludeS3Locations": ...,
    }


# LakeFormationConfigurationOutputTypeDef definition

class LakeFormationConfigurationOutputTypeDef(TypedDict):
    locationRegistrationExcludeS3Locations: NotRequired[List[str]],
    locationRegistrationRole: NotRequired[str],
```

## LakeFormationConfigurationTypeDef

```python
# LakeFormationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LakeFormationConfigurationTypeDef


def get_value() -> LakeFormationConfigurationTypeDef:
    return {
        "locationRegistrationExcludeS3Locations": ...,
    }


# LakeFormationConfigurationTypeDef definition

class LakeFormationConfigurationTypeDef(TypedDict):
    locationRegistrationExcludeS3Locations: NotRequired[Sequence[str]],
    locationRegistrationRole: NotRequired[str],
```

## LessThanExpressionTypeDef

```python
# LessThanExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LessThanExpressionTypeDef


def get_value() -> LessThanExpressionTypeDef:
    return {
        "columnName": ...,
    }


# LessThanExpressionTypeDef definition

class LessThanExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## LessThanOrEqualToExpressionTypeDef

```python
# LessThanOrEqualToExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LessThanOrEqualToExpressionTypeDef


def get_value() -> LessThanOrEqualToExpressionTypeDef:
    return {
        "columnName": ...,
    }


# LessThanOrEqualToExpressionTypeDef definition

class LessThanOrEqualToExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## LikeExpressionTypeDef

```python
# LikeExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LikeExpressionTypeDef


def get_value() -> LikeExpressionTypeDef:
    return {
        "columnName": ...,
    }


# LikeExpressionTypeDef definition

class LikeExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## LineageNodeSummaryTypeDef

```python
# LineageNodeSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LineageNodeSummaryTypeDef


def get_value() -> LineageNodeSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# LineageNodeSummaryTypeDef definition

class LineageNodeSummaryTypeDef(TypedDict):
    domainId: str,
    id: str,
    typeName: str,
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    eventTimestamp: NotRequired[datetime],
    name: NotRequired[str],
    sourceIdentifier: NotRequired[str],
    typeRevision: NotRequired[str],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

## LineageSqlQueryRunDetailsTypeDef

```python
# LineageSqlQueryRunDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LineageSqlQueryRunDetailsTypeDef


def get_value() -> LineageSqlQueryRunDetailsTypeDef:
    return {
        "errorMessages": ...,
    }


# LineageSqlQueryRunDetailsTypeDef definition

class LineageSqlQueryRunDetailsTypeDef(TypedDict):
    errorMessages: NotRequired[List[str]],
    numQueriesFailed: NotRequired[int],
    queryEndTime: NotRequired[datetime],
    queryStartTime: NotRequired[datetime],
    totalQueriesProcessed: NotRequired[int],
```

## LineageSyncScheduleTypeDef

```python
# LineageSyncScheduleTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LineageSyncScheduleTypeDef


def get_value() -> LineageSyncScheduleTypeDef:
    return {
        "schedule": ...,
    }


# LineageSyncScheduleTypeDef definition

class LineageSyncScheduleTypeDef(TypedDict):
    schedule: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PaginatorConfigTypeDef


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

## ListAssetFiltersInputTypeDef

```python
# ListAssetFiltersInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListAssetFiltersInputTypeDef


def get_value() -> ListAssetFiltersInputTypeDef:
    return {
        "assetIdentifier": ...,
    }


# ListAssetFiltersInputTypeDef definition

class ListAssetFiltersInputTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[FilterStatusType],  # (1)
```

1. See [:material-code-brackets: FilterStatusType](./literals.md#filterstatustype) 
## ListAssetRevisionsInputTypeDef

```python
# ListAssetRevisionsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListAssetRevisionsInputTypeDef


def get_value() -> ListAssetRevisionsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListAssetRevisionsInputTypeDef definition

class ListAssetRevisionsInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListConnectionsInputTypeDef

```python
# ListConnectionsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListConnectionsInputTypeDef


def get_value() -> ListConnectionsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListConnectionsInputTypeDef definition

class ListConnectionsInputTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    environmentIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortFieldConnectionType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    type: NotRequired[ConnectionTypeType],  # (3)
```

1. See [:material-code-brackets: SortFieldConnectionType](./literals.md#sortfieldconnectiontype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
## ListDataProductRevisionsInputTypeDef

```python
# ListDataProductRevisionsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataProductRevisionsInputTypeDef


def get_value() -> ListDataProductRevisionsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListDataProductRevisionsInputTypeDef definition

class ListDataProductRevisionsInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataSourceRunActivitiesInputTypeDef

```python
# ListDataSourceRunActivitiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourceRunActivitiesInputTypeDef


def get_value() -> ListDataSourceRunActivitiesInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListDataSourceRunActivitiesInputTypeDef definition

class ListDataSourceRunActivitiesInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[DataAssetActivityStatusType],  # (1)
```

1. See [:material-code-brackets: DataAssetActivityStatusType](./literals.md#dataassetactivitystatustype) 
## ListDataSourceRunsInputTypeDef

```python
# ListDataSourceRunsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourceRunsInputTypeDef


def get_value() -> ListDataSourceRunsInputTypeDef:
    return {
        "dataSourceIdentifier": ...,
    }


# ListDataSourceRunsInputTypeDef definition

class ListDataSourceRunsInputTypeDef(TypedDict):
    dataSourceIdentifier: str,
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[DataSourceRunStatusType],  # (1)
```

1. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
## ListDataSourcesInputTypeDef

```python
# ListDataSourcesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourcesInputTypeDef


def get_value() -> ListDataSourcesInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListDataSourcesInputTypeDef definition

class ListDataSourcesInputTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    connectionIdentifier: NotRequired[str],
    environmentIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    status: NotRequired[DataSourceStatusType],  # (1)
    type: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## ListDomainUnitsForParentInputTypeDef

```python
# ListDomainUnitsForParentInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDomainUnitsForParentInputTypeDef


def get_value() -> ListDomainUnitsForParentInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListDomainUnitsForParentInputTypeDef definition

class ListDomainUnitsForParentInputTypeDef(TypedDict):
    domainIdentifier: str,
    parentDomainUnitIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDomainsInputTypeDef

```python
# ListDomainsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDomainsInputTypeDef


def get_value() -> ListDomainsInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListDomainsInputTypeDef definition

class ListDomainsInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[DomainStatusType],  # (1)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
## ListEntityOwnersInputTypeDef

```python
# ListEntityOwnersInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEntityOwnersInputTypeDef


def get_value() -> ListEntityOwnersInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEntityOwnersInputTypeDef definition

class ListEntityOwnersInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: DataZoneEntityTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: DataZoneEntityTypeType](./literals.md#datazoneentitytypetype) 
## ListEnvironmentActionsInputTypeDef

```python
# ListEnvironmentActionsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentActionsInputTypeDef


def get_value() -> ListEnvironmentActionsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentActionsInputTypeDef definition

class ListEnvironmentActionsInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEnvironmentBlueprintConfigurationsInputTypeDef

```python
# ListEnvironmentBlueprintConfigurationsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentBlueprintConfigurationsInputTypeDef


def get_value() -> ListEnvironmentBlueprintConfigurationsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentBlueprintConfigurationsInputTypeDef definition

class ListEnvironmentBlueprintConfigurationsInputTypeDef(TypedDict):
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEnvironmentBlueprintsInputTypeDef

```python
# ListEnvironmentBlueprintsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentBlueprintsInputTypeDef


def get_value() -> ListEnvironmentBlueprintsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentBlueprintsInputTypeDef definition

class ListEnvironmentBlueprintsInputTypeDef(TypedDict):
    domainIdentifier: str,
    managed: NotRequired[bool],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListEnvironmentProfilesInputTypeDef

```python
# ListEnvironmentProfilesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentProfilesInputTypeDef


def get_value() -> ListEnvironmentProfilesInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentProfilesInputTypeDef definition

class ListEnvironmentProfilesInputTypeDef(TypedDict):
    domainIdentifier: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    environmentBlueprintIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    projectIdentifier: NotRequired[str],
```

## ListEnvironmentsInputTypeDef

```python
# ListEnvironmentsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentsInputTypeDef


def get_value() -> ListEnvironmentsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentsInputTypeDef definition

class ListEnvironmentsInputTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    environmentBlueprintIdentifier: NotRequired[str],
    environmentProfileIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    provider: NotRequired[str],
    status: NotRequired[EnvironmentStatusType],  # (1)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
## ListJobRunsInputTypeDef

```python
# ListJobRunsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListJobRunsInputTypeDef


def get_value() -> ListJobRunsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListJobRunsInputTypeDef definition

class ListJobRunsInputTypeDef(TypedDict):
    domainIdentifier: str,
    jobIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortOrder: NotRequired[SortOrderType],  # (1)
    status: NotRequired[JobRunStatusType],  # (2)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: JobRunStatusType](./literals.md#jobrunstatustype) 
## ListMetadataGenerationRunsInputTypeDef

```python
# ListMetadataGenerationRunsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListMetadataGenerationRunsInputTypeDef


def get_value() -> ListMetadataGenerationRunsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListMetadataGenerationRunsInputTypeDef definition

class ListMetadataGenerationRunsInputTypeDef(TypedDict):
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[MetadataGenerationRunStatusType],  # (1)
    type: NotRequired[MetadataGenerationRunTypeType],  # (2)
```

1. See [:material-code-brackets: MetadataGenerationRunStatusType](./literals.md#metadatagenerationrunstatustype) 
2. See [:material-code-brackets: MetadataGenerationRunTypeType](./literals.md#metadatagenerationruntypetype) 
## ListPolicyGrantsInputTypeDef

```python
# ListPolicyGrantsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListPolicyGrantsInputTypeDef


def get_value() -> ListPolicyGrantsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListPolicyGrantsInputTypeDef definition

class ListPolicyGrantsInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TargetEntityTypeType,  # (1)
    policyType: ManagedPolicyTypeType,  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: TargetEntityTypeType](./literals.md#targetentitytypetype) 
2. See [:material-code-brackets: ManagedPolicyTypeType](./literals.md#managedpolicytypetype) 
## ListProjectMembershipsInputTypeDef

```python
# ListProjectMembershipsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectMembershipsInputTypeDef


def get_value() -> ListProjectMembershipsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListProjectMembershipsInputTypeDef definition

class ListProjectMembershipsInputTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortFieldProjectType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SortFieldProjectType](./literals.md#sortfieldprojecttype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListProjectProfilesInputTypeDef

```python
# ListProjectProfilesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectProfilesInputTypeDef


def get_value() -> ListProjectProfilesInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListProjectProfilesInputTypeDef definition

class ListProjectProfilesInputTypeDef(TypedDict):
    domainIdentifier: str,
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortFieldProjectType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SortFieldProjectType](./literals.md#sortfieldprojecttype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ProjectProfileSummaryTypeDef

```python
# ProjectProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProjectProfileSummaryTypeDef


def get_value() -> ProjectProfileSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# ProjectProfileSummaryTypeDef definition

class ProjectProfileSummaryTypeDef(TypedDict):
    createdBy: str,
    domainId: str,
    id: str,
    name: str,
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    domainUnitId: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    status: NotRequired[StatusType],  # (1)
```

1. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## ListProjectsInputTypeDef

```python
# ListProjectsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectsInputTypeDef


def get_value() -> ListProjectsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListProjectsInputTypeDef definition

class ListProjectsInputTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    userIdentifier: NotRequired[str],
```

## ListRulesInputTypeDef

```python
# ListRulesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListRulesInputTypeDef


def get_value() -> ListRulesInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListRulesInputTypeDef definition

class ListRulesInputTypeDef(TypedDict):
    domainIdentifier: str,
    targetIdentifier: str,
    targetType: RuleTargetTypeType,  # (1)
    action: NotRequired[RuleActionType],  # (2)
    assetTypes: NotRequired[Sequence[str]],
    dataProduct: NotRequired[bool],
    includeCascaded: NotRequired[bool],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    projectIds: NotRequired[Sequence[str]],
    ruleType: NotRequired[RuleTypeType],  # (3)
```

1. See [:material-code-brackets: RuleTargetTypeType](./literals.md#ruletargettypetype) 
2. See [:material-code-brackets: RuleActionType](./literals.md#ruleactiontype) 
3. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
## ListSubscriptionGrantsInputTypeDef

```python
# ListSubscriptionGrantsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionGrantsInputTypeDef


def get_value() -> ListSubscriptionGrantsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListSubscriptionGrantsInputTypeDef definition

class ListSubscriptionGrantsInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    owningProjectId: NotRequired[str],
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    subscribedListingId: NotRequired[str],
    subscriptionId: NotRequired[str],
    subscriptionTargetId: NotRequired[str],
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListSubscriptionRequestsInputTypeDef

```python
# ListSubscriptionRequestsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionRequestsInputTypeDef


def get_value() -> ListSubscriptionRequestsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListSubscriptionRequestsInputTypeDef definition

class ListSubscriptionRequestsInputTypeDef(TypedDict):
    domainIdentifier: str,
    approverProjectId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    owningProjectId: NotRequired[str],
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    status: NotRequired[SubscriptionRequestStatusType],  # (3)
    subscribedListingId: NotRequired[str],
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
## ListSubscriptionTargetsInputTypeDef

```python
# ListSubscriptionTargetsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionTargetsInputTypeDef


def get_value() -> ListSubscriptionTargetsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListSubscriptionTargetsInputTypeDef definition

class ListSubscriptionTargetsInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListSubscriptionsInputTypeDef

```python
# ListSubscriptionsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionsInputTypeDef


def get_value() -> ListSubscriptionsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListSubscriptionsInputTypeDef definition

class ListSubscriptionsInputTypeDef(TypedDict):
    domainIdentifier: str,
    approverProjectId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    owningProjectId: NotRequired[str],
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    status: NotRequired[SubscriptionStatusType],  # (3)
    subscribedListingId: NotRequired[str],
    subscriptionRequestIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## UserDetailsTypeDef

```python
# UserDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UserDetailsTypeDef


def get_value() -> UserDetailsTypeDef:
    return {
        "userId": ...,
    }


# UserDetailsTypeDef definition

class UserDetailsTypeDef(TypedDict):
    userId: str,
```

## MetadataFormReferenceTypeDef

```python
# MetadataFormReferenceTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import MetadataFormReferenceTypeDef


def get_value() -> MetadataFormReferenceTypeDef:
    return {
        "typeIdentifier": ...,
    }


# MetadataFormReferenceTypeDef definition

class MetadataFormReferenceTypeDef(TypedDict):
    typeIdentifier: str,
    typeRevision: str,
```

## MetadataFormSummaryTypeDef

```python
# MetadataFormSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import MetadataFormSummaryTypeDef


def get_value() -> MetadataFormSummaryTypeDef:
    return {
        "formName": ...,
    }


# MetadataFormSummaryTypeDef definition

class MetadataFormSummaryTypeDef(TypedDict):
    typeName: str,
    typeRevision: str,
    formName: NotRequired[str],
```

## NameIdentifierTypeDef

```python
# NameIdentifierTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import NameIdentifierTypeDef


def get_value() -> NameIdentifierTypeDef:
    return {
        "name": ...,
    }


# NameIdentifierTypeDef definition

class NameIdentifierTypeDef(TypedDict):
    name: NotRequired[str],
    namespace: NotRequired[str],
```

## NotEqualToExpressionTypeDef

```python
# NotEqualToExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import NotEqualToExpressionTypeDef


def get_value() -> NotEqualToExpressionTypeDef:
    return {
        "columnName": ...,
    }


# NotEqualToExpressionTypeDef definition

class NotEqualToExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## NotInExpressionOutputTypeDef

```python
# NotInExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import NotInExpressionOutputTypeDef


def get_value() -> NotInExpressionOutputTypeDef:
    return {
        "columnName": ...,
    }


# NotInExpressionOutputTypeDef definition

class NotInExpressionOutputTypeDef(TypedDict):
    columnName: str,
    values: List[str],
```

## NotInExpressionTypeDef

```python
# NotInExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import NotInExpressionTypeDef


def get_value() -> NotInExpressionTypeDef:
    return {
        "columnName": ...,
    }


# NotInExpressionTypeDef definition

class NotInExpressionTypeDef(TypedDict):
    columnName: str,
    values: Sequence[str],
```

## NotLikeExpressionTypeDef

```python
# NotLikeExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import NotLikeExpressionTypeDef


def get_value() -> NotLikeExpressionTypeDef:
    return {
        "columnName": ...,
    }


# NotLikeExpressionTypeDef definition

class NotLikeExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## NotificationResourceTypeDef

```python
# NotificationResourceTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import NotificationResourceTypeDef


def get_value() -> NotificationResourceTypeDef:
    return {
        "id": ...,
    }


# NotificationResourceTypeDef definition

class NotificationResourceTypeDef(TypedDict):
    id: str,
    type: NotificationResourceTypeType,  # (1)
    name: NotRequired[str],
```

1. See [:material-code-brackets: NotificationResourceTypeType](./literals.md#notificationresourcetypetype) 
## OAuth2ClientApplicationTypeDef

```python
# OAuth2ClientApplicationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OAuth2ClientApplicationTypeDef


def get_value() -> OAuth2ClientApplicationTypeDef:
    return {
        "aWSManagedClientApplicationReference": ...,
    }


# OAuth2ClientApplicationTypeDef definition

class OAuth2ClientApplicationTypeDef(TypedDict):
    aWSManagedClientApplicationReference: NotRequired[str],
    userManagedClientApplicationClientId: NotRequired[str],
```

## OverrideDomainUnitOwnersPolicyGrantDetailTypeDef

```python
# OverrideDomainUnitOwnersPolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OverrideDomainUnitOwnersPolicyGrantDetailTypeDef


def get_value() -> OverrideDomainUnitOwnersPolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# OverrideDomainUnitOwnersPolicyGrantDetailTypeDef definition

class OverrideDomainUnitOwnersPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## OverrideProjectOwnersPolicyGrantDetailTypeDef

```python
# OverrideProjectOwnersPolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OverrideProjectOwnersPolicyGrantDetailTypeDef


def get_value() -> OverrideProjectOwnersPolicyGrantDetailTypeDef:
    return {
        "includeChildDomainUnits": ...,
    }


# OverrideProjectOwnersPolicyGrantDetailTypeDef definition

class OverrideProjectOwnersPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## OwnerGroupPropertiesOutputTypeDef

```python
# OwnerGroupPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OwnerGroupPropertiesOutputTypeDef


def get_value() -> OwnerGroupPropertiesOutputTypeDef:
    return {
        "groupId": ...,
    }


# OwnerGroupPropertiesOutputTypeDef definition

class OwnerGroupPropertiesOutputTypeDef(TypedDict):
    groupId: NotRequired[str],
```

## OwnerGroupPropertiesTypeDef

```python
# OwnerGroupPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OwnerGroupPropertiesTypeDef


def get_value() -> OwnerGroupPropertiesTypeDef:
    return {
        "groupIdentifier": ...,
    }


# OwnerGroupPropertiesTypeDef definition

class OwnerGroupPropertiesTypeDef(TypedDict):
    groupIdentifier: str,
```

## OwnerUserPropertiesOutputTypeDef

```python
# OwnerUserPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OwnerUserPropertiesOutputTypeDef


def get_value() -> OwnerUserPropertiesOutputTypeDef:
    return {
        "userId": ...,
    }


# OwnerUserPropertiesOutputTypeDef definition

class OwnerUserPropertiesOutputTypeDef(TypedDict):
    userId: NotRequired[str],
```

## OwnerUserPropertiesTypeDef

```python
# OwnerUserPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OwnerUserPropertiesTypeDef


def get_value() -> OwnerUserPropertiesTypeDef:
    return {
        "userIdentifier": ...,
    }


# OwnerUserPropertiesTypeDef definition

class OwnerUserPropertiesTypeDef(TypedDict):
    userIdentifier: str,
```

## PhysicalConnectionRequirementsTypeDef

```python
# PhysicalConnectionRequirementsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PhysicalConnectionRequirementsTypeDef


def get_value() -> PhysicalConnectionRequirementsTypeDef:
    return {
        "availabilityZone": ...,
    }


# PhysicalConnectionRequirementsTypeDef definition

class PhysicalConnectionRequirementsTypeDef(TypedDict):
    availabilityZone: NotRequired[str],
    securityGroupIdList: NotRequired[Sequence[str]],
    subnetId: NotRequired[str],
    subnetIdList: NotRequired[Sequence[str]],
```

## UserPolicyGrantPrincipalOutputTypeDef

```python
# UserPolicyGrantPrincipalOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UserPolicyGrantPrincipalOutputTypeDef


def get_value() -> UserPolicyGrantPrincipalOutputTypeDef:
    return {
        "allUsersGrantFilter": ...,
    }


# UserPolicyGrantPrincipalOutputTypeDef definition

class UserPolicyGrantPrincipalOutputTypeDef(TypedDict):
    allUsersGrantFilter: NotRequired[Dict[str, Any]],
    userIdentifier: NotRequired[str],
```

## UserPolicyGrantPrincipalTypeDef

```python
# UserPolicyGrantPrincipalTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UserPolicyGrantPrincipalTypeDef


def get_value() -> UserPolicyGrantPrincipalTypeDef:
    return {
        "allUsersGrantFilter": ...,
    }


# UserPolicyGrantPrincipalTypeDef definition

class UserPolicyGrantPrincipalTypeDef(TypedDict):
    allUsersGrantFilter: NotRequired[Mapping[str, Any]],
    userIdentifier: NotRequired[str],
```

## ProjectsForRuleOutputTypeDef

```python
# ProjectsForRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProjectsForRuleOutputTypeDef


def get_value() -> ProjectsForRuleOutputTypeDef:
    return {
        "selectionMode": ...,
    }


# ProjectsForRuleOutputTypeDef definition

class ProjectsForRuleOutputTypeDef(TypedDict):
    selectionMode: RuleScopeSelectionModeType,  # (1)
    specificProjects: NotRequired[List[str]],
```

1. See [:material-code-brackets: RuleScopeSelectionModeType](./literals.md#rulescopeselectionmodetype) 
## ProjectsForRuleTypeDef

```python
# ProjectsForRuleTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProjectsForRuleTypeDef


def get_value() -> ProjectsForRuleTypeDef:
    return {
        "selectionMode": ...,
    }


# ProjectsForRuleTypeDef definition

class ProjectsForRuleTypeDef(TypedDict):
    selectionMode: RuleScopeSelectionModeType,  # (1)
    specificProjects: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: RuleScopeSelectionModeType](./literals.md#rulescopeselectionmodetype) 
## RedshiftClusterStorageTypeDef

```python
# RedshiftClusterStorageTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftClusterStorageTypeDef


def get_value() -> RedshiftClusterStorageTypeDef:
    return {
        "clusterName": ...,
    }


# RedshiftClusterStorageTypeDef definition

class RedshiftClusterStorageTypeDef(TypedDict):
    clusterName: str,
```

## RedshiftCredentialConfigurationTypeDef

```python
# RedshiftCredentialConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftCredentialConfigurationTypeDef


def get_value() -> RedshiftCredentialConfigurationTypeDef:
    return {
        "secretManagerArn": ...,
    }


# RedshiftCredentialConfigurationTypeDef definition

class RedshiftCredentialConfigurationTypeDef(TypedDict):
    secretManagerArn: str,
```

## UsernamePasswordTypeDef

```python
# UsernamePasswordTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UsernamePasswordTypeDef


def get_value() -> UsernamePasswordTypeDef:
    return {
        "password": ...,
    }


# UsernamePasswordTypeDef definition

class UsernamePasswordTypeDef(TypedDict):
    password: str,
    username: str,
```

## RedshiftStoragePropertiesTypeDef

```python
# RedshiftStoragePropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftStoragePropertiesTypeDef


def get_value() -> RedshiftStoragePropertiesTypeDef:
    return {
        "clusterName": ...,
    }


# RedshiftStoragePropertiesTypeDef definition

class RedshiftStoragePropertiesTypeDef(TypedDict):
    clusterName: NotRequired[str],
    workgroupName: NotRequired[str],
```

## RedshiftServerlessStorageTypeDef

```python
# RedshiftServerlessStorageTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftServerlessStorageTypeDef


def get_value() -> RedshiftServerlessStorageTypeDef:
    return {
        "workgroupName": ...,
    }


# RedshiftServerlessStorageTypeDef definition

class RedshiftServerlessStorageTypeDef(TypedDict):
    workgroupName: str,
```

## RejectChoiceTypeDef

```python
# RejectChoiceTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RejectChoiceTypeDef


def get_value() -> RejectChoiceTypeDef:
    return {
        "predictionChoices": ...,
    }


# RejectChoiceTypeDef definition

class RejectChoiceTypeDef(TypedDict):
    predictionTarget: str,
    predictionChoices: NotRequired[Sequence[int]],
```

## RejectRuleTypeDef

```python
# RejectRuleTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RejectRuleTypeDef


def get_value() -> RejectRuleTypeDef:
    return {
        "rule": ...,
    }


# RejectRuleTypeDef definition

class RejectRuleTypeDef(TypedDict):
    rule: NotRequired[RejectRuleBehaviorType],  # (1)
    threshold: NotRequired[float],
```

1. See [:material-code-brackets: RejectRuleBehaviorType](./literals.md#rejectrulebehaviortype) 
## RejectSubscriptionRequestInputTypeDef

```python
# RejectSubscriptionRequestInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RejectSubscriptionRequestInputTypeDef


def get_value() -> RejectSubscriptionRequestInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# RejectSubscriptionRequestInputTypeDef definition

class RejectSubscriptionRequestInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    decisionComment: NotRequired[str],
```

## RevokeSubscriptionInputTypeDef

```python
# RevokeSubscriptionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RevokeSubscriptionInputTypeDef


def get_value() -> RevokeSubscriptionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# RevokeSubscriptionInputTypeDef definition

class RevokeSubscriptionInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    retainPermissions: NotRequired[bool],
```

## SearchGroupProfilesInputTypeDef

```python
# SearchGroupProfilesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchGroupProfilesInputTypeDef


def get_value() -> SearchGroupProfilesInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchGroupProfilesInputTypeDef definition

class SearchGroupProfilesInputTypeDef(TypedDict):
    domainIdentifier: str,
    groupType: GroupSearchTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    searchText: NotRequired[str],
```

1. See [:material-code-brackets: GroupSearchTypeType](./literals.md#groupsearchtypetype) 
## SearchInItemTypeDef

```python
# SearchInItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchInItemTypeDef


def get_value() -> SearchInItemTypeDef:
    return {
        "attribute": ...,
    }


# SearchInItemTypeDef definition

class SearchInItemTypeDef(TypedDict):
    attribute: str,
```

## SearchSortTypeDef

```python
# SearchSortTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchSortTypeDef


def get_value() -> SearchSortTypeDef:
    return {
        "attribute": ...,
    }


# SearchSortTypeDef definition

class SearchSortTypeDef(TypedDict):
    attribute: str,
    order: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SearchUserProfilesInputTypeDef

```python
# SearchUserProfilesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchUserProfilesInputTypeDef


def get_value() -> SearchUserProfilesInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchUserProfilesInputTypeDef definition

class SearchUserProfilesInputTypeDef(TypedDict):
    domainIdentifier: str,
    userType: UserSearchTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    searchText: NotRequired[str],
```

1. See [:material-code-brackets: UserSearchTypeType](./literals.md#usersearchtypetype) 
## SparkGlueArgsTypeDef

```python
# SparkGlueArgsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SparkGlueArgsTypeDef


def get_value() -> SparkGlueArgsTypeDef:
    return {
        "connection": ...,
    }


# SparkGlueArgsTypeDef definition

class SparkGlueArgsTypeDef(TypedDict):
    connection: NotRequired[str],
```

## SsoUserProfileDetailsTypeDef

```python
# SsoUserProfileDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SsoUserProfileDetailsTypeDef


def get_value() -> SsoUserProfileDetailsTypeDef:
    return {
        "firstName": ...,
    }


# SsoUserProfileDetailsTypeDef definition

class SsoUserProfileDetailsTypeDef(TypedDict):
    firstName: NotRequired[str],
    lastName: NotRequired[str],
    username: NotRequired[str],
```

## StartDataSourceRunInputTypeDef

```python
# StartDataSourceRunInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import StartDataSourceRunInputTypeDef


def get_value() -> StartDataSourceRunInputTypeDef:
    return {
        "dataSourceIdentifier": ...,
    }


# StartDataSourceRunInputTypeDef definition

class StartDataSourceRunInputTypeDef(TypedDict):
    dataSourceIdentifier: str,
    domainIdentifier: str,
    clientToken: NotRequired[str],
```

## SubscribedProjectInputTypeDef

```python
# SubscribedProjectInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedProjectInputTypeDef


def get_value() -> SubscribedProjectInputTypeDef:
    return {
        "identifier": ...,
    }


# SubscribedProjectInputTypeDef definition

class SubscribedProjectInputTypeDef(TypedDict):
    identifier: NotRequired[str],
```

## SubscribedProjectTypeDef

```python
# SubscribedProjectTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedProjectTypeDef


def get_value() -> SubscribedProjectTypeDef:
    return {
        "id": ...,
    }


# SubscribedProjectTypeDef definition

class SubscribedProjectTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## TermRelationsTypeDef

```python
# TermRelationsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import TermRelationsTypeDef


def get_value() -> TermRelationsTypeDef:
    return {
        "classifies": ...,
    }


# TermRelationsTypeDef definition

class TermRelationsTypeDef(TypedDict):
    classifies: NotRequired[Sequence[str]],
    isA: NotRequired[Sequence[str]],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateDomainUnitInputTypeDef

```python
# UpdateDomainUnitInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateDomainUnitInputTypeDef


def get_value() -> UpdateDomainUnitInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateDomainUnitInputTypeDef definition

class UpdateDomainUnitInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    name: NotRequired[str],
```

## UpdateEnvironmentInputTypeDef

```python
# UpdateEnvironmentInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateEnvironmentInputTypeDef


def get_value() -> UpdateEnvironmentInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateEnvironmentInputTypeDef definition

class UpdateEnvironmentInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    glossaryTerms: NotRequired[Sequence[str]],
    name: NotRequired[str],
```

## UpdateGlossaryInputTypeDef

```python
# UpdateGlossaryInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateGlossaryInputTypeDef


def get_value() -> UpdateGlossaryInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateGlossaryInputTypeDef definition

class UpdateGlossaryInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[GlossaryStatusType],  # (1)
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
## UpdateGroupProfileInputTypeDef

```python
# UpdateGroupProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateGroupProfileInputTypeDef


def get_value() -> UpdateGroupProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateGroupProfileInputTypeDef definition

class UpdateGroupProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: str,
    status: GroupProfileStatusType,  # (1)
```

1. See [:material-code-brackets: GroupProfileStatusType](./literals.md#groupprofilestatustype) 
## UpdateSubscriptionRequestInputTypeDef

```python
# UpdateSubscriptionRequestInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateSubscriptionRequestInputTypeDef


def get_value() -> UpdateSubscriptionRequestInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateSubscriptionRequestInputTypeDef definition

class UpdateSubscriptionRequestInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    requestReason: str,
```

## UpdateUserProfileInputTypeDef

```python
# UpdateUserProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateUserProfileInputTypeDef


def get_value() -> UpdateUserProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateUserProfileInputTypeDef definition

class UpdateUserProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    status: UserProfileStatusType,  # (1)
    userIdentifier: str,
    type: NotRequired[UserProfileTypeType],  # (2)
```

1. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
2. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
## AcceptPredictionsInputTypeDef

```python
# AcceptPredictionsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AcceptPredictionsInputTypeDef


def get_value() -> AcceptPredictionsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# AcceptPredictionsInputTypeDef definition

class AcceptPredictionsInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    acceptChoices: NotRequired[Sequence[AcceptChoiceTypeDef]],  # (1)
    acceptRule: NotRequired[AcceptRuleTypeDef],  # (2)
    clientToken: NotRequired[str],
    revision: NotRequired[str],
```

1. See [:material-code-braces: AcceptChoiceTypeDef](./type_defs.md#acceptchoicetypedef) 
2. See [:material-code-braces: AcceptRuleTypeDef](./type_defs.md#acceptruletypedef) 
## AcceptPredictionsOutputTypeDef

```python
# AcceptPredictionsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AcceptPredictionsOutputTypeDef


def get_value() -> AcceptPredictionsOutputTypeDef:
    return {
        "assetId": ...,
    }


# AcceptPredictionsOutputTypeDef definition

class AcceptPredictionsOutputTypeDef(TypedDict):
    assetId: str,
    domainId: str,
    revision: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFormTypeOutputTypeDef

```python
# CreateFormTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateFormTypeOutputTypeDef


def get_value() -> CreateFormTypeOutputTypeDef:
    return {
        "description": ...,
    }


# CreateFormTypeOutputTypeDef definition

class CreateFormTypeOutputTypeDef(TypedDict):
    description: str,
    domainId: str,
    name: str,
    originDomainId: str,
    originProjectId: str,
    owningProjectId: str,
    revision: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGlossaryOutputTypeDef

```python
# CreateGlossaryOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateGlossaryOutputTypeDef


def get_value() -> CreateGlossaryOutputTypeDef:
    return {
        "description": ...,
    }


# CreateGlossaryOutputTypeDef definition

class CreateGlossaryOutputTypeDef(TypedDict):
    description: str,
    domainId: str,
    id: str,
    name: str,
    owningProjectId: str,
    status: GlossaryStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupProfileOutputTypeDef

```python
# CreateGroupProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateGroupProfileOutputTypeDef


def get_value() -> CreateGroupProfileOutputTypeDef:
    return {
        "domainId": ...,
    }


# CreateGroupProfileOutputTypeDef definition

class CreateGroupProfileOutputTypeDef(TypedDict):
    domainId: str,
    groupName: str,
    id: str,
    status: GroupProfileStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GroupProfileStatusType](./literals.md#groupprofilestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateListingChangeSetOutputTypeDef

```python
# CreateListingChangeSetOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateListingChangeSetOutputTypeDef


def get_value() -> CreateListingChangeSetOutputTypeDef:
    return {
        "listingId": ...,
    }


# CreateListingChangeSetOutputTypeDef definition

class CreateListingChangeSetOutputTypeDef(TypedDict):
    listingId: str,
    listingRevision: str,
    status: ListingStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ListingStatusType](./literals.md#listingstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteConnectionOutputTypeDef

```python
# DeleteConnectionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteConnectionOutputTypeDef


def get_value() -> DeleteConnectionOutputTypeDef:
    return {
        "status": ...,
    }


# DeleteConnectionOutputTypeDef definition

class DeleteConnectionOutputTypeDef(TypedDict):
    status: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainOutputTypeDef

```python
# DeleteDomainOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteDomainOutputTypeDef


def get_value() -> DeleteDomainOutputTypeDef:
    return {
        "status": ...,
    }


# DeleteDomainOutputTypeDef definition

class DeleteDomainOutputTypeDef(TypedDict):
    status: DomainStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentCredentialsOutputTypeDef

```python
# GetEnvironmentCredentialsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentCredentialsOutputTypeDef


def get_value() -> GetEnvironmentCredentialsOutputTypeDef:
    return {
        "accessKeyId": ...,
    }


# GetEnvironmentCredentialsOutputTypeDef definition

class GetEnvironmentCredentialsOutputTypeDef(TypedDict):
    accessKeyId: str,
    expiration: datetime,
    secretAccessKey: str,
    sessionToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGlossaryOutputTypeDef

```python
# GetGlossaryOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetGlossaryOutputTypeDef


def get_value() -> GetGlossaryOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetGlossaryOutputTypeDef definition

class GetGlossaryOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    id: str,
    name: str,
    owningProjectId: str,
    status: GlossaryStatusType,  # (1)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupProfileOutputTypeDef

```python
# GetGroupProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetGroupProfileOutputTypeDef


def get_value() -> GetGroupProfileOutputTypeDef:
    return {
        "domainId": ...,
    }


# GetGroupProfileOutputTypeDef definition

class GetGroupProfileOutputTypeDef(TypedDict):
    domainId: str,
    groupName: str,
    id: str,
    status: GroupProfileStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GroupProfileStatusType](./literals.md#groupprofilestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetIamPortalLoginUrlOutputTypeDef

```python
# GetIamPortalLoginUrlOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetIamPortalLoginUrlOutputTypeDef


def get_value() -> GetIamPortalLoginUrlOutputTypeDef:
    return {
        "authCodeUrl": ...,
    }


# GetIamPortalLoginUrlOutputTypeDef definition

class GetIamPortalLoginUrlOutputTypeDef(TypedDict):
    authCodeUrl: str,
    userProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLineageEventOutputTypeDef

```python
# GetLineageEventOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetLineageEventOutputTypeDef


def get_value() -> GetLineageEventOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetLineageEventOutputTypeDef definition

class GetLineageEventOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    event: StreamingBody,
    eventTime: datetime,
    id: str,
    processingStatus: LineageEventProcessingStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: LineageEventProcessingStatusType](./literals.md#lineageeventprocessingstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostLineageEventOutputTypeDef

```python
# PostLineageEventOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PostLineageEventOutputTypeDef


def get_value() -> PostLineageEventOutputTypeDef:
    return {
        "domainId": ...,
    }


# PostLineageEventOutputTypeDef definition

class PostLineageEventOutputTypeDef(TypedDict):
    domainId: str,
    id: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectPredictionsOutputTypeDef

```python
# RejectPredictionsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RejectPredictionsOutputTypeDef


def get_value() -> RejectPredictionsOutputTypeDef:
    return {
        "assetId": ...,
    }


# RejectPredictionsOutputTypeDef definition

class RejectPredictionsOutputTypeDef(TypedDict):
    assetId: str,
    assetRevision: str,
    domainId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartMetadataGenerationRunOutputTypeDef

```python
# StartMetadataGenerationRunOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import StartMetadataGenerationRunOutputTypeDef


def get_value() -> StartMetadataGenerationRunOutputTypeDef:
    return {
        "createdAt": ...,
    }


# StartMetadataGenerationRunOutputTypeDef definition

class StartMetadataGenerationRunOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    id: str,
    owningProjectId: str,
    status: MetadataGenerationRunStatusType,  # (1)
    type: MetadataGenerationRunTypeType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: MetadataGenerationRunStatusType](./literals.md#metadatagenerationrunstatustype) 
2. See [:material-code-brackets: MetadataGenerationRunTypeType](./literals.md#metadatagenerationruntypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlossaryOutputTypeDef

```python
# UpdateGlossaryOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateGlossaryOutputTypeDef


def get_value() -> UpdateGlossaryOutputTypeDef:
    return {
        "description": ...,
    }


# UpdateGlossaryOutputTypeDef definition

class UpdateGlossaryOutputTypeDef(TypedDict):
    description: str,
    domainId: str,
    id: str,
    name: str,
    owningProjectId: str,
    status: GlossaryStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGroupProfileOutputTypeDef

```python
# UpdateGroupProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateGroupProfileOutputTypeDef


def get_value() -> UpdateGroupProfileOutputTypeDef:
    return {
        "domainId": ...,
    }


# UpdateGroupProfileOutputTypeDef definition

class UpdateGroupProfileOutputTypeDef(TypedDict):
    domainId: str,
    groupName: str,
    id: str,
    status: GroupProfileStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: GroupProfileStatusType](./literals.md#groupprofilestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcceptSubscriptionRequestInputTypeDef

```python
# AcceptSubscriptionRequestInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AcceptSubscriptionRequestInputTypeDef


def get_value() -> AcceptSubscriptionRequestInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# AcceptSubscriptionRequestInputTypeDef definition

class AcceptSubscriptionRequestInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    assetScopes: NotRequired[Sequence[AcceptedAssetScopeTypeDef]],  # (1)
    decisionComment: NotRequired[str],
```

1. See [:material-code-braces: AcceptedAssetScopeTypeDef](./type_defs.md#acceptedassetscopetypedef) 
## ActionParametersTypeDef

```python
# ActionParametersTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ActionParametersTypeDef


def get_value() -> ActionParametersTypeDef:
    return {
        "awsConsoleLink": ...,
    }


# ActionParametersTypeDef definition

class ActionParametersTypeDef(TypedDict):
    awsConsoleLink: NotRequired[AwsConsoleLinkParametersTypeDef],  # (1)
```

1. See [:material-code-braces: AwsConsoleLinkParametersTypeDef](./type_defs.md#awsconsolelinkparameterstypedef) 
## ListAssetFiltersOutputTypeDef

```python
# ListAssetFiltersOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListAssetFiltersOutputTypeDef


def get_value() -> ListAssetFiltersOutputTypeDef:
    return {
        "items": ...,
    }


# ListAssetFiltersOutputTypeDef definition

class ListAssetFiltersOutputTypeDef(TypedDict):
    items: List[AssetFilterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetFilterSummaryTypeDef](./type_defs.md#assetfiltersummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetItemAdditionalAttributesTypeDef

```python
# AssetItemAdditionalAttributesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetItemAdditionalAttributesTypeDef


def get_value() -> AssetItemAdditionalAttributesTypeDef:
    return {
        "formsOutput": ...,
    }


# AssetItemAdditionalAttributesTypeDef definition

class AssetItemAdditionalAttributesTypeDef(TypedDict):
    formsOutput: NotRequired[List[FormOutputTypeDef]],  # (1)
    latestTimeSeriesDataPointFormsOutput: NotRequired[List[TimeSeriesDataPointSummaryFormOutputTypeDef]],  # (2)
    readOnlyFormsOutput: NotRequired[List[FormOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: TimeSeriesDataPointSummaryFormOutputTypeDef](./type_defs.md#timeseriesdatapointsummaryformoutputtypedef) 
3. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
## AssetListingItemAdditionalAttributesTypeDef

```python
# AssetListingItemAdditionalAttributesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetListingItemAdditionalAttributesTypeDef


def get_value() -> AssetListingItemAdditionalAttributesTypeDef:
    return {
        "forms": ...,
    }


# AssetListingItemAdditionalAttributesTypeDef definition

class AssetListingItemAdditionalAttributesTypeDef(TypedDict):
    forms: NotRequired[str],
    latestTimeSeriesDataPointForms: NotRequired[List[TimeSeriesDataPointSummaryFormOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: TimeSeriesDataPointSummaryFormOutputTypeDef](./type_defs.md#timeseriesdatapointsummaryformoutputtypedef) 
## ListTimeSeriesDataPointsOutputTypeDef

```python
# ListTimeSeriesDataPointsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListTimeSeriesDataPointsOutputTypeDef


def get_value() -> ListTimeSeriesDataPointsOutputTypeDef:
    return {
        "items": ...,
    }


# ListTimeSeriesDataPointsOutputTypeDef definition

class ListTimeSeriesDataPointsOutputTypeDef(TypedDict):
    items: List[TimeSeriesDataPointSummaryFormOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: TimeSeriesDataPointSummaryFormOutputTypeDef](./type_defs.md#timeseriesdatapointsummaryformoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssetOutputTypeDef

```python
# GetAssetOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetAssetOutputTypeDef


def get_value() -> GetAssetOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetAssetOutputTypeDef definition

class GetAssetOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    externalIdentifier: str,
    firstRevisionCreatedAt: datetime,
    firstRevisionCreatedBy: str,
    formsOutput: List[FormOutputTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    latestTimeSeriesDataPointFormsOutput: List[TimeSeriesDataPointSummaryFormOutputTypeDef],  # (2)
    listing: AssetListingDetailsTypeDef,  # (3)
    name: str,
    owningProjectId: str,
    readOnlyFormsOutput: List[FormOutputTypeDef],  # (1)
    revision: str,
    typeIdentifier: str,
    typeRevision: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: TimeSeriesDataPointSummaryFormOutputTypeDef](./type_defs.md#timeseriesdatapointsummaryformoutputtypedef) 
3. See [:material-code-braces: AssetListingDetailsTypeDef](./type_defs.md#assetlistingdetailstypedef) 
4. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetListingTypeDef

```python
# AssetListingTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetListingTypeDef


def get_value() -> AssetListingTypeDef:
    return {
        "assetId": ...,
    }


# AssetListingTypeDef definition

class AssetListingTypeDef(TypedDict):
    assetId: NotRequired[str],
    assetRevision: NotRequired[str],
    assetType: NotRequired[str],
    createdAt: NotRequired[datetime],
    forms: NotRequired[str],
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (1)
    latestTimeSeriesDataPointForms: NotRequired[List[TimeSeriesDataPointSummaryFormOutputTypeDef]],  # (2)
    owningProjectId: NotRequired[str],
```

1. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
2. See [:material-code-braces: TimeSeriesDataPointSummaryFormOutputTypeDef](./type_defs.md#timeseriesdatapointsummaryformoutputtypedef) 
## ListingSummaryItemTypeDef

```python
# ListingSummaryItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListingSummaryItemTypeDef


def get_value() -> ListingSummaryItemTypeDef:
    return {
        "glossaryTerms": ...,
    }


# ListingSummaryItemTypeDef definition

class ListingSummaryItemTypeDef(TypedDict):
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (1)
    listingId: NotRequired[str],
    listingRevision: NotRequired[str],
```

1. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
## ListingSummaryTypeDef

```python
# ListingSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListingSummaryTypeDef


def get_value() -> ListingSummaryTypeDef:
    return {
        "glossaryTerms": ...,
    }


# ListingSummaryTypeDef definition

class ListingSummaryTypeDef(TypedDict):
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (1)
    listingId: NotRequired[str],
    listingRevision: NotRequired[str],
```

1. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
## SubscribedProductListingTypeDef

```python
# SubscribedProductListingTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedProductListingTypeDef


def get_value() -> SubscribedProductListingTypeDef:
    return {
        "assetListings": ...,
    }


# SubscribedProductListingTypeDef definition

class SubscribedProductListingTypeDef(TypedDict):
    assetListings: NotRequired[List[AssetInDataProductListingItemTypeDef]],  # (1)
    description: NotRequired[str],
    entityId: NotRequired[str],
    entityRevision: NotRequired[str],
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (2)
    name: NotRequired[str],
```

1. See [:material-code-braces: AssetInDataProductListingItemTypeDef](./type_defs.md#assetindataproductlistingitemtypedef) 
2. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
## ListAssetRevisionsOutputTypeDef

```python
# ListAssetRevisionsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListAssetRevisionsOutputTypeDef


def get_value() -> ListAssetRevisionsOutputTypeDef:
    return {
        "items": ...,
    }


# ListAssetRevisionsOutputTypeDef definition

class ListAssetRevisionsOutputTypeDef(TypedDict):
    items: List[AssetRevisionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AssetRevisionTypeDef](./type_defs.md#assetrevisiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscribedAssetListingTypeDef

```python
# SubscribedAssetListingTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedAssetListingTypeDef


def get_value() -> SubscribedAssetListingTypeDef:
    return {
        "assetScope": ...,
    }


# SubscribedAssetListingTypeDef definition

class SubscribedAssetListingTypeDef(TypedDict):
    assetScope: NotRequired[AssetScopeTypeDef],  # (1)
    entityId: NotRequired[str],
    entityRevision: NotRequired[str],
    entityType: NotRequired[str],
    forms: NotRequired[str],
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (2)
```

1. See [:material-code-braces: AssetScopeTypeDef](./type_defs.md#assetscopetypedef) 
2. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
## AssetTypeItemTypeDef

```python
# AssetTypeItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetTypeItemTypeDef


def get_value() -> AssetTypeItemTypeDef:
    return {
        "createdAt": ...,
    }


# AssetTypeItemTypeDef definition

class AssetTypeItemTypeDef(TypedDict):
    domainId: str,
    formsOutput: Dict[str, FormEntryOutputTypeDef],  # (1)
    name: str,
    owningProjectId: str,
    revision: str,
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    originDomainId: NotRequired[str],
    originProjectId: NotRequired[str],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-braces: FormEntryOutputTypeDef](./type_defs.md#formentryoutputtypedef) 
## CreateAssetTypeOutputTypeDef

```python
# CreateAssetTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetTypeOutputTypeDef


def get_value() -> CreateAssetTypeOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CreateAssetTypeOutputTypeDef definition

class CreateAssetTypeOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    formsOutput: Dict[str, FormEntryOutputTypeDef],  # (1)
    name: str,
    originDomainId: str,
    originProjectId: str,
    owningProjectId: str,
    revision: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FormEntryOutputTypeDef](./type_defs.md#formentryoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssetTypeOutputTypeDef

```python
# GetAssetTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetAssetTypeOutputTypeDef


def get_value() -> GetAssetTypeOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetAssetTypeOutputTypeDef definition

class GetAssetTypeOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    formsOutput: Dict[str, FormEntryOutputTypeDef],  # (1)
    name: str,
    originDomainId: str,
    originProjectId: str,
    owningProjectId: str,
    revision: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FormEntryOutputTypeDef](./type_defs.md#formentryoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LineageNodeTypeItemTypeDef

```python
# LineageNodeTypeItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LineageNodeTypeItemTypeDef


def get_value() -> LineageNodeTypeItemTypeDef:
    return {
        "createdAt": ...,
    }


# LineageNodeTypeItemTypeDef definition

class LineageNodeTypeItemTypeDef(TypedDict):
    domainId: str,
    formsOutput: Dict[str, FormEntryOutputTypeDef],  # (1)
    revision: str,
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-braces: FormEntryOutputTypeDef](./type_defs.md#formentryoutputtypedef) 
## AuthenticationConfigurationPatchTypeDef

```python
# AuthenticationConfigurationPatchTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AuthenticationConfigurationPatchTypeDef


def get_value() -> AuthenticationConfigurationPatchTypeDef:
    return {
        "basicAuthenticationCredentials": ...,
    }


# AuthenticationConfigurationPatchTypeDef definition

class AuthenticationConfigurationPatchTypeDef(TypedDict):
    basicAuthenticationCredentials: NotRequired[BasicAuthenticationCredentialsTypeDef],  # (1)
    secretArn: NotRequired[str],
```

1. See [:material-code-braces: BasicAuthenticationCredentialsTypeDef](./type_defs.md#basicauthenticationcredentialstypedef) 
## PostLineageEventInputTypeDef

```python
# PostLineageEventInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PostLineageEventInputTypeDef


def get_value() -> PostLineageEventInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# PostLineageEventInputTypeDef definition

class PostLineageEventInputTypeDef(TypedDict):
    domainIdentifier: str,
    event: BlobTypeDef,
    clientToken: NotRequired[str],
```

## PredictionConfigurationTypeDef

```python
# PredictionConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PredictionConfigurationTypeDef


def get_value() -> PredictionConfigurationTypeDef:
    return {
        "businessNameGeneration": ...,
    }


# PredictionConfigurationTypeDef definition

class PredictionConfigurationTypeDef(TypedDict):
    businessNameGeneration: NotRequired[BusinessNameGenerationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: BusinessNameGenerationConfigurationTypeDef](./type_defs.md#businessnamegenerationconfigurationtypedef) 
## ProvisioningPropertiesTypeDef

```python
# ProvisioningPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProvisioningPropertiesTypeDef


def get_value() -> ProvisioningPropertiesTypeDef:
    return {
        "cloudFormation": ...,
    }


# ProvisioningPropertiesTypeDef definition

class ProvisioningPropertiesTypeDef(TypedDict):
    cloudFormation: NotRequired[CloudFormationPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: CloudFormationPropertiesTypeDef](./type_defs.md#cloudformationpropertiestypedef) 
## ConfigurableEnvironmentActionTypeDef

```python
# ConfigurableEnvironmentActionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ConfigurableEnvironmentActionTypeDef


def get_value() -> ConfigurableEnvironmentActionTypeDef:
    return {
        "auth": ...,
    }


# ConfigurableEnvironmentActionTypeDef definition

class ConfigurableEnvironmentActionTypeDef(TypedDict):
    parameters: List[ConfigurableActionParameterTypeDef],  # (2)
    type: str,
    auth: NotRequired[ConfigurableActionTypeAuthorizationType],  # (1)
```

1. See [:material-code-brackets: ConfigurableActionTypeAuthorizationType](./literals.md#configurableactiontypeauthorizationtype) 
2. See [:material-code-braces: ConfigurableActionParameterTypeDef](./type_defs.md#configurableactionparametertypedef) 
## CreateAssetTypeInputTypeDef

```python
# CreateAssetTypeInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetTypeInputTypeDef


def get_value() -> CreateAssetTypeInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateAssetTypeInputTypeDef definition

class CreateAssetTypeInputTypeDef(TypedDict):
    domainIdentifier: str,
    formsInput: Mapping[str, FormEntryInputTypeDef],  # (1)
    name: str,
    owningProjectIdentifier: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: FormEntryInputTypeDef](./type_defs.md#formentryinputtypedef) 
## CreateDataProductOutputTypeDef

```python
# CreateDataProductOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDataProductOutputTypeDef


def get_value() -> CreateDataProductOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CreateDataProductOutputTypeDef definition

class CreateDataProductOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    firstRevisionCreatedAt: datetime,
    firstRevisionCreatedBy: str,
    formsOutput: List[FormOutputTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    items: List[DataProductItemOutputTypeDef],  # (2)
    name: str,
    owningProjectId: str,
    revision: str,
    status: DataProductStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: DataProductItemOutputTypeDef](./type_defs.md#dataproductitemoutputtypedef) 
3. See [:material-code-brackets: DataProductStatusType](./literals.md#dataproductstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataProductRevisionOutputTypeDef

```python
# CreateDataProductRevisionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDataProductRevisionOutputTypeDef


def get_value() -> CreateDataProductRevisionOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CreateDataProductRevisionOutputTypeDef definition

class CreateDataProductRevisionOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    firstRevisionCreatedAt: datetime,
    firstRevisionCreatedBy: str,
    formsOutput: List[FormOutputTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    items: List[DataProductItemOutputTypeDef],  # (2)
    name: str,
    owningProjectId: str,
    revision: str,
    status: DataProductStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: DataProductItemOutputTypeDef](./type_defs.md#dataproductitemoutputtypedef) 
3. See [:material-code-brackets: DataProductStatusType](./literals.md#dataproductstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataProductOutputTypeDef

```python
# GetDataProductOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDataProductOutputTypeDef


def get_value() -> GetDataProductOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetDataProductOutputTypeDef definition

class GetDataProductOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    firstRevisionCreatedAt: datetime,
    firstRevisionCreatedBy: str,
    formsOutput: List[FormOutputTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    items: List[DataProductItemOutputTypeDef],  # (2)
    name: str,
    owningProjectId: str,
    revision: str,
    status: DataProductStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: DataProductItemOutputTypeDef](./type_defs.md#dataproductitemoutputtypedef) 
3. See [:material-code-brackets: DataProductStatusType](./literals.md#dataproductstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceSummaryTypeDef

```python
# DataSourceSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataSourceSummaryTypeDef


def get_value() -> DataSourceSummaryTypeDef:
    return {
        "connectionId": ...,
    }


# DataSourceSummaryTypeDef definition

class DataSourceSummaryTypeDef(TypedDict):
    dataSourceId: str,
    domainId: str,
    name: str,
    status: DataSourceStatusType,  # (5)
    type: str,
    connectionId: NotRequired[str],
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    enableSetting: NotRequired[EnableSettingType],  # (1)
    environmentId: NotRequired[str],
    lastRunAssetCount: NotRequired[int],
    lastRunAt: NotRequired[datetime],
    lastRunErrorMessage: NotRequired[DataSourceErrorMessageTypeDef],  # (2)
    lastRunStatus: NotRequired[DataSourceRunStatusType],  # (3)
    schedule: NotRequired[ScheduleConfigurationTypeDef],  # (4)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
2. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
3. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
4. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
5. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## CreateDomainInputTypeDef

```python
# CreateDomainInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDomainInputTypeDef


def get_value() -> CreateDomainInputTypeDef:
    return {
        "domainExecutionRole": ...,
    }


# CreateDomainInputTypeDef definition

class CreateDomainInputTypeDef(TypedDict):
    domainExecutionRole: str,
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    domainVersion: NotRequired[DomainVersionType],  # (1)
    kmsKeyIdentifier: NotRequired[str],
    serviceRole: NotRequired[str],
    singleSignOn: NotRequired[SingleSignOnTypeDef],  # (2)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DomainVersionType](./literals.md#domainversiontype) 
2. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
## CreateDomainOutputTypeDef

```python
# CreateDomainOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDomainOutputTypeDef


def get_value() -> CreateDomainOutputTypeDef:
    return {
        "arn": ...,
    }


# CreateDomainOutputTypeDef definition

class CreateDomainOutputTypeDef(TypedDict):
    arn: str,
    description: str,
    domainExecutionRole: str,
    domainVersion: DomainVersionType,  # (1)
    id: str,
    kmsKeyIdentifier: str,
    name: str,
    portalUrl: str,
    rootDomainUnitId: str,
    serviceRole: str,
    singleSignOn: SingleSignOnTypeDef,  # (2)
    status: DomainStatusType,  # (3)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DomainVersionType](./literals.md#domainversiontype) 
2. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
3. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainOutputTypeDef

```python
# GetDomainOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDomainOutputTypeDef


def get_value() -> GetDomainOutputTypeDef:
    return {
        "arn": ...,
    }


# GetDomainOutputTypeDef definition

class GetDomainOutputTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    description: str,
    domainExecutionRole: str,
    domainVersion: DomainVersionType,  # (1)
    id: str,
    kmsKeyIdentifier: str,
    lastUpdatedAt: datetime,
    name: str,
    portalUrl: str,
    rootDomainUnitId: str,
    serviceRole: str,
    singleSignOn: SingleSignOnTypeDef,  # (2)
    status: DomainStatusType,  # (3)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: DomainVersionType](./literals.md#domainversiontype) 
2. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
3. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainInputTypeDef

```python
# UpdateDomainInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateDomainInputTypeDef


def get_value() -> UpdateDomainInputTypeDef:
    return {
        "identifier": ...,
    }


# UpdateDomainInputTypeDef definition

class UpdateDomainInputTypeDef(TypedDict):
    identifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    domainExecutionRole: NotRequired[str],
    name: NotRequired[str],
    serviceRole: NotRequired[str],
    singleSignOn: NotRequired[SingleSignOnTypeDef],  # (1)
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
## UpdateDomainOutputTypeDef

```python
# UpdateDomainOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateDomainOutputTypeDef


def get_value() -> UpdateDomainOutputTypeDef:
    return {
        "description": ...,
    }


# UpdateDomainOutputTypeDef definition

class UpdateDomainOutputTypeDef(TypedDict):
    description: str,
    domainExecutionRole: str,
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    rootDomainUnitId: str,
    serviceRole: str,
    singleSignOn: SingleSignOnTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentInputTypeDef

```python
# CreateEnvironmentInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateEnvironmentInputTypeDef


def get_value() -> CreateEnvironmentInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateEnvironmentInputTypeDef definition

class CreateEnvironmentInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentProfileIdentifier: str,
    name: str,
    projectIdentifier: str,
    deploymentOrder: NotRequired[int],
    description: NotRequired[str],
    environmentAccountIdentifier: NotRequired[str],
    environmentAccountRegion: NotRequired[str],
    environmentBlueprintIdentifier: NotRequired[str],
    environmentConfigurationId: NotRequired[str],
    glossaryTerms: NotRequired[Sequence[str]],
    userParameters: NotRequired[Sequence[EnvironmentParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
## CreateEnvironmentProfileInputTypeDef

```python
# CreateEnvironmentProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateEnvironmentProfileInputTypeDef


def get_value() -> CreateEnvironmentProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateEnvironmentProfileInputTypeDef definition

class CreateEnvironmentProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentBlueprintIdentifier: str,
    name: str,
    projectIdentifier: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    description: NotRequired[str],
    userParameters: NotRequired[Sequence[EnvironmentParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
## EnvironmentConfigurationUserParameterOutputTypeDef

```python
# EnvironmentConfigurationUserParameterOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationUserParameterOutputTypeDef


def get_value() -> EnvironmentConfigurationUserParameterOutputTypeDef:
    return {
        "environmentConfigurationName": ...,
    }


# EnvironmentConfigurationUserParameterOutputTypeDef definition

class EnvironmentConfigurationUserParameterOutputTypeDef(TypedDict):
    environmentConfigurationName: NotRequired[str],
    environmentParameters: NotRequired[List[EnvironmentParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
## EnvironmentConfigurationUserParameterTypeDef

```python
# EnvironmentConfigurationUserParameterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationUserParameterTypeDef


def get_value() -> EnvironmentConfigurationUserParameterTypeDef:
    return {
        "environmentConfigurationName": ...,
    }


# EnvironmentConfigurationUserParameterTypeDef definition

class EnvironmentConfigurationUserParameterTypeDef(TypedDict):
    environmentConfigurationName: NotRequired[str],
    environmentParameters: NotRequired[Sequence[EnvironmentParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
## UpdateEnvironmentProfileInputTypeDef

```python
# UpdateEnvironmentProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateEnvironmentProfileInputTypeDef


def get_value() -> UpdateEnvironmentProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateEnvironmentProfileInputTypeDef definition

class UpdateEnvironmentProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
    userParameters: NotRequired[Sequence[EnvironmentParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
## CreateEnvironmentProfileOutputTypeDef

```python
# CreateEnvironmentProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateEnvironmentProfileOutputTypeDef


def get_value() -> CreateEnvironmentProfileOutputTypeDef:
    return {
        "awsAccountId": ...,
    }


# CreateEnvironmentProfileOutputTypeDef definition

class CreateEnvironmentProfileOutputTypeDef(TypedDict):
    awsAccountId: str,
    awsAccountRegion: str,
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    environmentBlueprintId: str,
    id: str,
    name: str,
    projectId: str,
    updatedAt: datetime,
    userParameters: List[CustomParameterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomParameterTypeDef](./type_defs.md#customparametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentProfileOutputTypeDef

```python
# GetEnvironmentProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentProfileOutputTypeDef


def get_value() -> GetEnvironmentProfileOutputTypeDef:
    return {
        "awsAccountId": ...,
    }


# GetEnvironmentProfileOutputTypeDef definition

class GetEnvironmentProfileOutputTypeDef(TypedDict):
    awsAccountId: str,
    awsAccountRegion: str,
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    environmentBlueprintId: str,
    id: str,
    name: str,
    projectId: str,
    updatedAt: datetime,
    userParameters: List[CustomParameterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomParameterTypeDef](./type_defs.md#customparametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentProfileOutputTypeDef

```python
# UpdateEnvironmentProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateEnvironmentProfileOutputTypeDef


def get_value() -> UpdateEnvironmentProfileOutputTypeDef:
    return {
        "awsAccountId": ...,
    }


# UpdateEnvironmentProfileOutputTypeDef definition

class UpdateEnvironmentProfileOutputTypeDef(TypedDict):
    awsAccountId: str,
    awsAccountRegion: str,
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    environmentBlueprintId: str,
    id: str,
    name: str,
    projectId: str,
    updatedAt: datetime,
    userParameters: List[CustomParameterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CustomParameterTypeDef](./type_defs.md#customparametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateFormTypeInputTypeDef

```python
# CreateFormTypeInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateFormTypeInputTypeDef


def get_value() -> CreateFormTypeInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateFormTypeInputTypeDef definition

class CreateFormTypeInputTypeDef(TypedDict):
    domainIdentifier: str,
    model: ModelTypeDef,  # (1)
    name: str,
    owningProjectIdentifier: str,
    description: NotRequired[str],
    status: NotRequired[FormTypeStatusType],  # (2)
```

1. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
2. See [:material-code-brackets: FormTypeStatusType](./literals.md#formtypestatustype) 
## CreateGlossaryTermOutputTypeDef

```python
# CreateGlossaryTermOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateGlossaryTermOutputTypeDef


def get_value() -> CreateGlossaryTermOutputTypeDef:
    return {
        "domainId": ...,
    }


# CreateGlossaryTermOutputTypeDef definition

class CreateGlossaryTermOutputTypeDef(TypedDict):
    domainId: str,
    glossaryId: str,
    id: str,
    longDescription: str,
    name: str,
    shortDescription: str,
    status: GlossaryTermStatusType,  # (1)
    termRelations: TermRelationsOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsOutputTypeDef](./type_defs.md#termrelationsoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGlossaryTermOutputTypeDef

```python
# GetGlossaryTermOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetGlossaryTermOutputTypeDef


def get_value() -> GetGlossaryTermOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetGlossaryTermOutputTypeDef definition

class GetGlossaryTermOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    glossaryId: str,
    id: str,
    longDescription: str,
    name: str,
    shortDescription: str,
    status: GlossaryTermStatusType,  # (1)
    termRelations: TermRelationsOutputTypeDef,  # (2)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsOutputTypeDef](./type_defs.md#termrelationsoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GlossaryTermItemTypeDef

```python
# GlossaryTermItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlossaryTermItemTypeDef


def get_value() -> GlossaryTermItemTypeDef:
    return {
        "createdAt": ...,
    }


# GlossaryTermItemTypeDef definition

class GlossaryTermItemTypeDef(TypedDict):
    domainId: str,
    glossaryId: str,
    id: str,
    name: str,
    status: GlossaryTermStatusType,  # (1)
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    longDescription: NotRequired[str],
    shortDescription: NotRequired[str],
    termRelations: NotRequired[TermRelationsOutputTypeDef],  # (2)
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsOutputTypeDef](./type_defs.md#termrelationsoutputtypedef) 
## UpdateGlossaryTermOutputTypeDef

```python
# UpdateGlossaryTermOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateGlossaryTermOutputTypeDef


def get_value() -> UpdateGlossaryTermOutputTypeDef:
    return {
        "domainId": ...,
    }


# UpdateGlossaryTermOutputTypeDef definition

class UpdateGlossaryTermOutputTypeDef(TypedDict):
    domainId: str,
    glossaryId: str,
    id: str,
    longDescription: str,
    name: str,
    shortDescription: str,
    status: GlossaryTermStatusType,  # (1)
    termRelations: TermRelationsOutputTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsOutputTypeDef](./type_defs.md#termrelationsoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectMembershipInputTypeDef

```python
# CreateProjectMembershipInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateProjectMembershipInputTypeDef


def get_value() -> CreateProjectMembershipInputTypeDef:
    return {
        "designation": ...,
    }


# CreateProjectMembershipInputTypeDef definition

class CreateProjectMembershipInputTypeDef(TypedDict):
    designation: UserDesignationType,  # (1)
    domainIdentifier: str,
    member: MemberTypeDef,  # (2)
    projectIdentifier: str,
```

1. See [:material-code-brackets: UserDesignationType](./literals.md#userdesignationtype) 
2. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
## DeleteProjectMembershipInputTypeDef

```python
# DeleteProjectMembershipInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteProjectMembershipInputTypeDef


def get_value() -> DeleteProjectMembershipInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# DeleteProjectMembershipInputTypeDef definition

class DeleteProjectMembershipInputTypeDef(TypedDict):
    domainIdentifier: str,
    member: MemberTypeDef,  # (1)
    projectIdentifier: str,
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
## ProjectSummaryTypeDef

```python
# ProjectSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProjectSummaryTypeDef


def get_value() -> ProjectSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# ProjectSummaryTypeDef definition

class ProjectSummaryTypeDef(TypedDict):
    createdBy: str,
    domainId: str,
    id: str,
    name: str,
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    domainUnitId: NotRequired[str],
    failureReasons: NotRequired[List[ProjectDeletionErrorTypeDef]],  # (1)
    projectStatus: NotRequired[ProjectStatusType],  # (2)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: ProjectDeletionErrorTypeDef](./type_defs.md#projectdeletionerrortypedef) 
2. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
## CreateSubscriptionTargetInputTypeDef

```python
# CreateSubscriptionTargetInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateSubscriptionTargetInputTypeDef


def get_value() -> CreateSubscriptionTargetInputTypeDef:
    return {
        "applicableAssetTypes": ...,
    }


# CreateSubscriptionTargetInputTypeDef definition

class CreateSubscriptionTargetInputTypeDef(TypedDict):
    applicableAssetTypes: Sequence[str],
    authorizedPrincipals: Sequence[str],
    domainIdentifier: str,
    environmentIdentifier: str,
    manageAccessRole: str,
    name: str,
    subscriptionTargetConfig: Sequence[SubscriptionTargetFormTypeDef],  # (1)
    type: str,
    clientToken: NotRequired[str],
    provider: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
## CreateSubscriptionTargetOutputTypeDef

```python
# CreateSubscriptionTargetOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateSubscriptionTargetOutputTypeDef


def get_value() -> CreateSubscriptionTargetOutputTypeDef:
    return {
        "applicableAssetTypes": ...,
    }


# CreateSubscriptionTargetOutputTypeDef definition

class CreateSubscriptionTargetOutputTypeDef(TypedDict):
    applicableAssetTypes: List[str],
    authorizedPrincipals: List[str],
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    environmentId: str,
    id: str,
    manageAccessRole: str,
    name: str,
    projectId: str,
    provider: str,
    subscriptionTargetConfig: List[SubscriptionTargetFormTypeDef],  # (1)
    type: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionTargetOutputTypeDef

```python
# GetSubscriptionTargetOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetSubscriptionTargetOutputTypeDef


def get_value() -> GetSubscriptionTargetOutputTypeDef:
    return {
        "applicableAssetTypes": ...,
    }


# GetSubscriptionTargetOutputTypeDef definition

class GetSubscriptionTargetOutputTypeDef(TypedDict):
    applicableAssetTypes: List[str],
    authorizedPrincipals: List[str],
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    environmentId: str,
    id: str,
    manageAccessRole: str,
    name: str,
    projectId: str,
    provider: str,
    subscriptionTargetConfig: List[SubscriptionTargetFormTypeDef],  # (1)
    type: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscriptionTargetSummaryTypeDef

```python
# SubscriptionTargetSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscriptionTargetSummaryTypeDef


def get_value() -> SubscriptionTargetSummaryTypeDef:
    return {
        "applicableAssetTypes": ...,
    }


# SubscriptionTargetSummaryTypeDef definition

class SubscriptionTargetSummaryTypeDef(TypedDict):
    applicableAssetTypes: List[str],
    authorizedPrincipals: List[str],
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    environmentId: str,
    id: str,
    name: str,
    projectId: str,
    provider: str,
    subscriptionTargetConfig: List[SubscriptionTargetFormTypeDef],  # (1)
    type: str,
    manageAccessRole: NotRequired[str],
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
## UpdateSubscriptionTargetInputTypeDef

```python
# UpdateSubscriptionTargetInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateSubscriptionTargetInputTypeDef


def get_value() -> UpdateSubscriptionTargetInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateSubscriptionTargetInputTypeDef definition

class UpdateSubscriptionTargetInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
    applicableAssetTypes: NotRequired[Sequence[str]],
    authorizedPrincipals: NotRequired[Sequence[str]],
    manageAccessRole: NotRequired[str],
    name: NotRequired[str],
    provider: NotRequired[str],
    subscriptionTargetConfig: NotRequired[Sequence[SubscriptionTargetFormTypeDef]],  # (1)
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
## UpdateSubscriptionTargetOutputTypeDef

```python
# UpdateSubscriptionTargetOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateSubscriptionTargetOutputTypeDef


def get_value() -> UpdateSubscriptionTargetOutputTypeDef:
    return {
        "applicableAssetTypes": ...,
    }


# UpdateSubscriptionTargetOutputTypeDef definition

class UpdateSubscriptionTargetOutputTypeDef(TypedDict):
    applicableAssetTypes: List[str],
    authorizedPrincipals: List[str],
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    environmentId: str,
    id: str,
    manageAccessRole: str,
    name: str,
    projectId: str,
    provider: str,
    subscriptionTargetConfig: List[SubscriptionTargetFormTypeDef],  # (1)
    type: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataProductRevisionsOutputTypeDef

```python
# ListDataProductRevisionsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataProductRevisionsOutputTypeDef


def get_value() -> ListDataProductRevisionsOutputTypeDef:
    return {
        "items": ...,
    }


# ListDataProductRevisionsOutputTypeDef definition

class ListDataProductRevisionsOutputTypeDef(TypedDict):
    items: List[DataProductRevisionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataProductRevisionTypeDef](./type_defs.md#dataproductrevisiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceRunActivityTypeDef

```python
# DataSourceRunActivityTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataSourceRunActivityTypeDef


def get_value() -> DataSourceRunActivityTypeDef:
    return {
        "createdAt": ...,
    }


# DataSourceRunActivityTypeDef definition

class DataSourceRunActivityTypeDef(TypedDict):
    createdAt: datetime,
    dataAssetStatus: DataAssetActivityStatusType,  # (1)
    dataSourceRunId: str,
    database: str,
    projectId: str,
    technicalName: str,
    updatedAt: datetime,
    dataAssetId: NotRequired[str],
    errorMessage: NotRequired[DataSourceErrorMessageTypeDef],  # (2)
    lineageSummary: NotRequired[LineageInfoTypeDef],  # (3)
    technicalDescription: NotRequired[str],
```

1. See [:material-code-brackets: DataAssetActivityStatusType](./literals.md#dataassetactivitystatustype) 
2. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
3. See [:material-code-braces: LineageInfoTypeDef](./type_defs.md#lineageinfotypedef) 
## DataSourceRunSummaryTypeDef

```python
# DataSourceRunSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataSourceRunSummaryTypeDef


def get_value() -> DataSourceRunSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# DataSourceRunSummaryTypeDef definition

class DataSourceRunSummaryTypeDef(TypedDict):
    createdAt: datetime,
    dataSourceId: str,
    id: str,
    projectId: str,
    status: DataSourceRunStatusType,  # (4)
    type: DataSourceRunTypeType,  # (5)
    updatedAt: datetime,
    errorMessage: NotRequired[DataSourceErrorMessageTypeDef],  # (1)
    lineageSummary: NotRequired[DataSourceRunLineageSummaryTypeDef],  # (2)
    runStatisticsForAssets: NotRequired[RunStatisticsForAssetsTypeDef],  # (3)
    startedAt: NotRequired[datetime],
    stoppedAt: NotRequired[datetime],
```

1. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
2. See [:material-code-braces: DataSourceRunLineageSummaryTypeDef](./type_defs.md#datasourcerunlineagesummarytypedef) 
3. See [:material-code-braces: RunStatisticsForAssetsTypeDef](./type_defs.md#runstatisticsforassetstypedef) 
4. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
5. See [:material-code-brackets: DataSourceRunTypeType](./literals.md#datasourceruntypetype) 
## GetDataSourceRunOutputTypeDef

```python
# GetDataSourceRunOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDataSourceRunOutputTypeDef


def get_value() -> GetDataSourceRunOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetDataSourceRunOutputTypeDef definition

class GetDataSourceRunOutputTypeDef(TypedDict):
    createdAt: datetime,
    dataSourceConfigurationSnapshot: str,
    dataSourceId: str,
    domainId: str,
    errorMessage: DataSourceErrorMessageTypeDef,  # (1)
    id: str,
    lineageSummary: DataSourceRunLineageSummaryTypeDef,  # (2)
    projectId: str,
    runStatisticsForAssets: RunStatisticsForAssetsTypeDef,  # (3)
    startedAt: datetime,
    status: DataSourceRunStatusType,  # (4)
    stoppedAt: datetime,
    type: DataSourceRunTypeType,  # (5)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
2. See [:material-code-braces: DataSourceRunLineageSummaryTypeDef](./type_defs.md#datasourcerunlineagesummarytypedef) 
3. See [:material-code-braces: RunStatisticsForAssetsTypeDef](./type_defs.md#runstatisticsforassetstypedef) 
4. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
5. See [:material-code-brackets: DataSourceRunTypeType](./literals.md#datasourceruntypetype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartDataSourceRunOutputTypeDef

```python
# StartDataSourceRunOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import StartDataSourceRunOutputTypeDef


def get_value() -> StartDataSourceRunOutputTypeDef:
    return {
        "createdAt": ...,
    }


# StartDataSourceRunOutputTypeDef definition

class StartDataSourceRunOutputTypeDef(TypedDict):
    createdAt: datetime,
    dataSourceConfigurationSnapshot: str,
    dataSourceId: str,
    domainId: str,
    errorMessage: DataSourceErrorMessageTypeDef,  # (1)
    id: str,
    projectId: str,
    runStatisticsForAssets: RunStatisticsForAssetsTypeDef,  # (2)
    startedAt: datetime,
    status: DataSourceRunStatusType,  # (3)
    stoppedAt: datetime,
    type: DataSourceRunTypeType,  # (4)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
2. See [:material-code-braces: RunStatisticsForAssetsTypeDef](./type_defs.md#runstatisticsforassetstypedef) 
3. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
4. See [:material-code-brackets: DataSourceRunTypeType](./literals.md#datasourceruntypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentTypeDef

```python
# DeploymentTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeploymentTypeDef


def get_value() -> DeploymentTypeDef:
    return {
        "deploymentId": ...,
    }


# DeploymentTypeDef definition

class DeploymentTypeDef(TypedDict):
    deploymentId: NotRequired[str],
    deploymentStatus: NotRequired[DeploymentStatusType],  # (1)
    deploymentType: NotRequired[DeploymentTypeType],  # (2)
    failureReason: NotRequired[EnvironmentErrorTypeDef],  # (3)
    isDeploymentComplete: NotRequired[bool],
    messages: NotRequired[List[str]],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-brackets: DeploymentTypeType](./literals.md#deploymenttypetype) 
3. See [:material-code-braces: EnvironmentErrorTypeDef](./type_defs.md#environmenterrortypedef) 
## EnvironmentDeploymentDetailsOutputTypeDef

```python
# EnvironmentDeploymentDetailsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentDeploymentDetailsOutputTypeDef


def get_value() -> EnvironmentDeploymentDetailsOutputTypeDef:
    return {
        "environmentFailureReasons": ...,
    }


# EnvironmentDeploymentDetailsOutputTypeDef definition

class EnvironmentDeploymentDetailsOutputTypeDef(TypedDict):
    environmentFailureReasons: NotRequired[Dict[str, List[EnvironmentErrorTypeDef]]],  # (1)
    overallDeploymentStatus: NotRequired[OverallDeploymentStatusType],  # (2)
```

1. See [:material-code-braces: EnvironmentErrorTypeDef](./type_defs.md#environmenterrortypedef) 
2. See [:material-code-brackets: OverallDeploymentStatusType](./literals.md#overalldeploymentstatustype) 
## EnvironmentDeploymentDetailsTypeDef

```python
# EnvironmentDeploymentDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentDeploymentDetailsTypeDef


def get_value() -> EnvironmentDeploymentDetailsTypeDef:
    return {
        "environmentFailureReasons": ...,
    }


# EnvironmentDeploymentDetailsTypeDef definition

class EnvironmentDeploymentDetailsTypeDef(TypedDict):
    environmentFailureReasons: NotRequired[Mapping[str, Sequence[EnvironmentErrorTypeDef]]],  # (1)
    overallDeploymentStatus: NotRequired[OverallDeploymentStatusType],  # (2)
```

1. See [:material-code-braces: EnvironmentErrorTypeDef](./type_defs.md#environmenterrortypedef) 
2. See [:material-code-brackets: OverallDeploymentStatusType](./literals.md#overalldeploymentstatustype) 
## ListDomainsOutputTypeDef

```python
# ListDomainsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDomainsOutputTypeDef


def get_value() -> ListDomainsOutputTypeDef:
    return {
        "items": ...,
    }


# ListDomainsOutputTypeDef definition

class ListDomainsOutputTypeDef(TypedDict):
    items: List[DomainSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainSummaryTypeDef](./type_defs.md#domainsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProjectGrantFilterTypeDef

```python
# ProjectGrantFilterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProjectGrantFilterTypeDef


def get_value() -> ProjectGrantFilterTypeDef:
    return {
        "domainUnitFilter": ...,
    }


# ProjectGrantFilterTypeDef definition

class ProjectGrantFilterTypeDef(TypedDict):
    domainUnitFilter: NotRequired[DomainUnitFilterForProjectTypeDef],  # (1)
```

1. See [:material-code-braces: DomainUnitFilterForProjectTypeDef](./type_defs.md#domainunitfilterforprojecttypedef) 
## DomainUnitPolicyGrantPrincipalOutputTypeDef

```python
# DomainUnitPolicyGrantPrincipalOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitPolicyGrantPrincipalOutputTypeDef


def get_value() -> DomainUnitPolicyGrantPrincipalOutputTypeDef:
    return {
        "domainUnitDesignation": ...,
    }


# DomainUnitPolicyGrantPrincipalOutputTypeDef definition

class DomainUnitPolicyGrantPrincipalOutputTypeDef(TypedDict):
    domainUnitDesignation: DomainUnitDesignationType,  # (1)
    domainUnitGrantFilter: NotRequired[DomainUnitGrantFilterOutputTypeDef],  # (2)
    domainUnitIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: DomainUnitDesignationType](./literals.md#domainunitdesignationtype) 
2. See [:material-code-braces: DomainUnitGrantFilterOutputTypeDef](./type_defs.md#domainunitgrantfilteroutputtypedef) 
## DomainUnitPolicyGrantPrincipalTypeDef

```python
# DomainUnitPolicyGrantPrincipalTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitPolicyGrantPrincipalTypeDef


def get_value() -> DomainUnitPolicyGrantPrincipalTypeDef:
    return {
        "domainUnitDesignation": ...,
    }


# DomainUnitPolicyGrantPrincipalTypeDef definition

class DomainUnitPolicyGrantPrincipalTypeDef(TypedDict):
    domainUnitDesignation: DomainUnitDesignationType,  # (1)
    domainUnitGrantFilter: NotRequired[DomainUnitGrantFilterTypeDef],  # (2)
    domainUnitIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: DomainUnitDesignationType](./literals.md#domainunitdesignationtype) 
2. See [:material-code-braces: DomainUnitGrantFilterTypeDef](./type_defs.md#domainunitgrantfiltertypedef) 
## DomainUnitOwnerPropertiesTypeDef

```python
# DomainUnitOwnerPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DomainUnitOwnerPropertiesTypeDef


def get_value() -> DomainUnitOwnerPropertiesTypeDef:
    return {
        "group": ...,
    }


# DomainUnitOwnerPropertiesTypeDef definition

class DomainUnitOwnerPropertiesTypeDef(TypedDict):
    group: NotRequired[DomainUnitGroupPropertiesTypeDef],  # (1)
    user: NotRequired[DomainUnitUserPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: DomainUnitGroupPropertiesTypeDef](./type_defs.md#domainunitgrouppropertiestypedef) 
2. See [:material-code-braces: DomainUnitUserPropertiesTypeDef](./type_defs.md#domainunituserpropertiestypedef) 
## ListDomainUnitsForParentOutputTypeDef

```python
# ListDomainUnitsForParentOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDomainUnitsForParentOutputTypeDef


def get_value() -> ListDomainUnitsForParentOutputTypeDef:
    return {
        "items": ...,
    }


# ListDomainUnitsForParentOutputTypeDef definition

class ListDomainUnitsForParentOutputTypeDef(TypedDict):
    items: List[DomainUnitSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainUnitSummaryTypeDef](./type_defs.md#domainunitsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleTargetTypeDef

```python
# RuleTargetTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RuleTargetTypeDef


def get_value() -> RuleTargetTypeDef:
    return {
        "domainUnitTarget": ...,
    }


# RuleTargetTypeDef definition

class RuleTargetTypeDef(TypedDict):
    domainUnitTarget: NotRequired[DomainUnitTargetTypeDef],  # (1)
```

1. See [:material-code-braces: DomainUnitTargetTypeDef](./type_defs.md#domainunittargettypedef) 
## EnvironmentConfigurationParametersDetailsOutputTypeDef

```python
# EnvironmentConfigurationParametersDetailsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationParametersDetailsOutputTypeDef


def get_value() -> EnvironmentConfigurationParametersDetailsOutputTypeDef:
    return {
        "parameterOverrides": ...,
    }


# EnvironmentConfigurationParametersDetailsOutputTypeDef definition

class EnvironmentConfigurationParametersDetailsOutputTypeDef(TypedDict):
    parameterOverrides: NotRequired[List[EnvironmentConfigurationParameterTypeDef]],  # (1)
    resolvedParameters: NotRequired[List[EnvironmentConfigurationParameterTypeDef]],  # (1)
    ssmPath: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentConfigurationParameterTypeDef](./type_defs.md#environmentconfigurationparametertypedef) 
2. See [:material-code-braces: EnvironmentConfigurationParameterTypeDef](./type_defs.md#environmentconfigurationparametertypedef) 
## EnvironmentConfigurationParametersDetailsTypeDef

```python
# EnvironmentConfigurationParametersDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationParametersDetailsTypeDef


def get_value() -> EnvironmentConfigurationParametersDetailsTypeDef:
    return {
        "parameterOverrides": ...,
    }


# EnvironmentConfigurationParametersDetailsTypeDef definition

class EnvironmentConfigurationParametersDetailsTypeDef(TypedDict):
    parameterOverrides: NotRequired[Sequence[EnvironmentConfigurationParameterTypeDef]],  # (1)
    resolvedParameters: NotRequired[Sequence[EnvironmentConfigurationParameterTypeDef]],  # (1)
    ssmPath: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentConfigurationParameterTypeDef](./type_defs.md#environmentconfigurationparametertypedef) 
2. See [:material-code-braces: EnvironmentConfigurationParameterTypeDef](./type_defs.md#environmentconfigurationparametertypedef) 
## ListEnvironmentProfilesOutputTypeDef

```python
# ListEnvironmentProfilesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentProfilesOutputTypeDef


def get_value() -> ListEnvironmentProfilesOutputTypeDef:
    return {
        "items": ...,
    }


# ListEnvironmentProfilesOutputTypeDef definition

class ListEnvironmentProfilesOutputTypeDef(TypedDict):
    items: List[EnvironmentProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentProfileSummaryTypeDef](./type_defs.md#environmentprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsOutputTypeDef

```python
# ListEnvironmentsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentsOutputTypeDef


def get_value() -> ListEnvironmentsOutputTypeDef:
    return {
        "items": ...,
    }


# ListEnvironmentsOutputTypeDef definition

class ListEnvironmentsOutputTypeDef(TypedDict):
    items: List[EnvironmentSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentSummaryTypeDef](./type_defs.md#environmentsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscribedAssetTypeDef

```python
# SubscribedAssetTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedAssetTypeDef


def get_value() -> SubscribedAssetTypeDef:
    return {
        "assetId": ...,
    }


# SubscribedAssetTypeDef definition

class SubscribedAssetTypeDef(TypedDict):
    assetId: str,
    assetRevision: str,
    status: SubscriptionGrantStatusType,  # (3)
    assetScope: NotRequired[AssetScopeTypeDef],  # (1)
    failureCause: NotRequired[FailureCauseTypeDef],  # (2)
    failureTimestamp: NotRequired[datetime],
    grantedTimestamp: NotRequired[datetime],
    targetName: NotRequired[str],
```

1. See [:material-code-braces: AssetScopeTypeDef](./type_defs.md#assetscopetypedef) 
2. See [:material-code-braces: FailureCauseTypeDef](./type_defs.md#failurecausetypedef) 
3. See [:material-code-brackets: SubscriptionGrantStatusType](./literals.md#subscriptiongrantstatustype) 
## UpdateSubscriptionGrantStatusInputTypeDef

```python
# UpdateSubscriptionGrantStatusInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateSubscriptionGrantStatusInputTypeDef


def get_value() -> UpdateSubscriptionGrantStatusInputTypeDef:
    return {
        "assetIdentifier": ...,
    }


# UpdateSubscriptionGrantStatusInputTypeDef definition

class UpdateSubscriptionGrantStatusInputTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    identifier: str,
    status: SubscriptionGrantStatusType,  # (1)
    failureCause: NotRequired[FailureCauseTypeDef],  # (2)
    targetName: NotRequired[str],
```

1. See [:material-code-brackets: SubscriptionGrantStatusType](./literals.md#subscriptiongrantstatustype) 
2. See [:material-code-braces: FailureCauseTypeDef](./type_defs.md#failurecausetypedef) 
## FilterClausePaginatorTypeDef

```python
# FilterClausePaginatorTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FilterClausePaginatorTypeDef


def get_value() -> FilterClausePaginatorTypeDef:
    return {
        "and": ...,
    }


# FilterClausePaginatorTypeDef definition

class FilterClausePaginatorTypeDef(TypedDict):
    and: NotRequired[Sequence[Mapping[str, Any]]],
    filter: NotRequired[FilterTypeDef],  # (1)
    or: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## FilterClauseTypeDef

```python
# FilterClauseTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FilterClauseTypeDef


def get_value() -> FilterClauseTypeDef:
    return {
        "and": ...,
    }


# FilterClauseTypeDef definition

class FilterClauseTypeDef(TypedDict):
    and: NotRequired[Sequence[Mapping[str, Any]]],
    filter: NotRequired[FilterTypeDef],  # (1)
    or: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## RelationalFilterConfigurationOutputTypeDef

```python
# RelationalFilterConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RelationalFilterConfigurationOutputTypeDef


def get_value() -> RelationalFilterConfigurationOutputTypeDef:
    return {
        "databaseName": ...,
    }


# RelationalFilterConfigurationOutputTypeDef definition

class RelationalFilterConfigurationOutputTypeDef(TypedDict):
    databaseName: str,
    filterExpressions: NotRequired[List[FilterExpressionTypeDef]],  # (1)
    schemaName: NotRequired[str],
```

1. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) 
## RelationalFilterConfigurationTypeDef

```python
# RelationalFilterConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RelationalFilterConfigurationTypeDef


def get_value() -> RelationalFilterConfigurationTypeDef:
    return {
        "databaseName": ...,
    }


# RelationalFilterConfigurationTypeDef definition

class RelationalFilterConfigurationTypeDef(TypedDict):
    databaseName: str,
    filterExpressions: NotRequired[Sequence[FilterExpressionTypeDef]],  # (1)
    schemaName: NotRequired[str],
```

1. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) 
## FormTypeDataTypeDef

```python
# FormTypeDataTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import FormTypeDataTypeDef


def get_value() -> FormTypeDataTypeDef:
    return {
        "createdAt": ...,
    }


# FormTypeDataTypeDef definition

class FormTypeDataTypeDef(TypedDict):
    domainId: str,
    name: str,
    revision: str,
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    imports: NotRequired[List[ImportTypeDef]],  # (1)
    model: NotRequired[ModelTypeDef],  # (2)
    originDomainId: NotRequired[str],
    originProjectId: NotRequired[str],
    owningProjectId: NotRequired[str],
    status: NotRequired[FormTypeStatusType],  # (3)
```

1. See [:material-code-braces: ImportTypeDef](./type_defs.md#importtypedef) 
2. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
3. See [:material-code-brackets: FormTypeStatusType](./literals.md#formtypestatustype) 
## GetFormTypeOutputTypeDef

```python
# GetFormTypeOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetFormTypeOutputTypeDef


def get_value() -> GetFormTypeOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetFormTypeOutputTypeDef definition

class GetFormTypeOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    imports: List[ImportTypeDef],  # (1)
    model: ModelTypeDef,  # (2)
    name: str,
    originDomainId: str,
    originProjectId: str,
    owningProjectId: str,
    revision: str,
    status: FormTypeStatusType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ImportTypeDef](./type_defs.md#importtypedef) 
2. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
3. See [:material-code-brackets: FormTypeStatusType](./literals.md#formtypestatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## JobRunSummaryTypeDef

```python
# JobRunSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import JobRunSummaryTypeDef


def get_value() -> JobRunSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# JobRunSummaryTypeDef definition

class JobRunSummaryTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    domainId: NotRequired[str],
    endTime: NotRequired[datetime],
    error: NotRequired[JobRunErrorTypeDef],  # (1)
    jobId: NotRequired[str],
    jobType: NotRequired[JobTypeType],  # (2)
    runId: NotRequired[str],
    runMode: NotRequired[JobRunModeType],  # (3)
    startTime: NotRequired[datetime],
    status: NotRequired[JobRunStatusType],  # (4)
```

1. See [:material-code-braces: JobRunErrorTypeDef](./type_defs.md#jobrunerrortypedef) 
2. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
3. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype) 
4. See [:material-code-brackets: JobRunStatusType](./literals.md#jobrunstatustype) 
## GetLineageNodeInputTypeDef

```python
# GetLineageNodeInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetLineageNodeInputTypeDef


def get_value() -> GetLineageNodeInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# GetLineageNodeInputTypeDef definition

class GetLineageNodeInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    eventTimestamp: NotRequired[TimestampTypeDef],
```

## ListLineageEventsInputTypeDef

```python
# ListLineageEventsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListLineageEventsInputTypeDef


def get_value() -> ListLineageEventsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListLineageEventsInputTypeDef definition

class ListLineageEventsInputTypeDef(TypedDict):
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    processingStatus: NotRequired[LineageEventProcessingStatusType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    timestampAfter: NotRequired[TimestampTypeDef],
    timestampBefore: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: LineageEventProcessingStatusType](./literals.md#lineageeventprocessingstatustype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListLineageNodeHistoryInputTypeDef

```python
# ListLineageNodeHistoryInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListLineageNodeHistoryInputTypeDef


def get_value() -> ListLineageNodeHistoryInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListLineageNodeHistoryInputTypeDef definition

class ListLineageNodeHistoryInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    direction: NotRequired[EdgeDirectionType],  # (1)
    eventTimestampGTE: NotRequired[TimestampTypeDef],
    eventTimestampLTE: NotRequired[TimestampTypeDef],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: EdgeDirectionType](./literals.md#edgedirectiontype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListNotificationsInputTypeDef

```python
# ListNotificationsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListNotificationsInputTypeDef


def get_value() -> ListNotificationsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListNotificationsInputTypeDef definition

class ListNotificationsInputTypeDef(TypedDict):
    domainIdentifier: str,
    type: NotificationTypeType,  # (1)
    afterTimestamp: NotRequired[TimestampTypeDef],
    beforeTimestamp: NotRequired[TimestampTypeDef],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    subjects: NotRequired[Sequence[str]],
    taskStatus: NotRequired[TaskStatusType],  # (2)
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
## ListTimeSeriesDataPointsInputTypeDef

```python
# ListTimeSeriesDataPointsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListTimeSeriesDataPointsInputTypeDef


def get_value() -> ListTimeSeriesDataPointsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListTimeSeriesDataPointsInputTypeDef definition

class ListTimeSeriesDataPointsInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    formName: str,
    endedAt: NotRequired[TimestampTypeDef],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    startedAt: NotRequired[TimestampTypeDef],
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
## TimeSeriesDataPointFormInputTypeDef

```python
# TimeSeriesDataPointFormInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import TimeSeriesDataPointFormInputTypeDef


def get_value() -> TimeSeriesDataPointFormInputTypeDef:
    return {
        "content": ...,
    }


# TimeSeriesDataPointFormInputTypeDef definition

class TimeSeriesDataPointFormInputTypeDef(TypedDict):
    formName: str,
    timestamp: TimestampTypeDef,
    typeIdentifier: str,
    content: NotRequired[str],
    typeRevision: NotRequired[str],
```

## GetLineageNodeOutputTypeDef

```python
# GetLineageNodeOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetLineageNodeOutputTypeDef


def get_value() -> GetLineageNodeOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetLineageNodeOutputTypeDef definition

class GetLineageNodeOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    downstreamNodes: List[LineageNodeReferenceTypeDef],  # (1)
    eventTimestamp: datetime,
    formsOutput: List[FormOutputTypeDef],  # (2)
    id: str,
    name: str,
    sourceIdentifier: str,
    typeName: str,
    typeRevision: str,
    updatedAt: datetime,
    updatedBy: str,
    upstreamNodes: List[LineageNodeReferenceTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: LineageNodeReferenceTypeDef](./type_defs.md#lineagenodereferencetypedef) 
2. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
3. See [:material-code-braces: LineageNodeReferenceTypeDef](./type_defs.md#lineagenodereferencetypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetMetadataGenerationRunOutputTypeDef

```python
# GetMetadataGenerationRunOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetMetadataGenerationRunOutputTypeDef


def get_value() -> GetMetadataGenerationRunOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetMetadataGenerationRunOutputTypeDef definition

class GetMetadataGenerationRunOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    id: str,
    owningProjectId: str,
    status: MetadataGenerationRunStatusType,  # (1)
    target: MetadataGenerationRunTargetTypeDef,  # (2)
    type: MetadataGenerationRunTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: MetadataGenerationRunStatusType](./literals.md#metadatagenerationrunstatustype) 
2. See [:material-code-braces: MetadataGenerationRunTargetTypeDef](./type_defs.md#metadatagenerationruntargettypedef) 
3. See [:material-code-brackets: MetadataGenerationRunTypeType](./literals.md#metadatagenerationruntypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MetadataGenerationRunItemTypeDef

```python
# MetadataGenerationRunItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import MetadataGenerationRunItemTypeDef


def get_value() -> MetadataGenerationRunItemTypeDef:
    return {
        "createdAt": ...,
    }


# MetadataGenerationRunItemTypeDef definition

class MetadataGenerationRunItemTypeDef(TypedDict):
    domainId: str,
    id: str,
    owningProjectId: str,
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    status: NotRequired[MetadataGenerationRunStatusType],  # (1)
    target: NotRequired[MetadataGenerationRunTargetTypeDef],  # (2)
    type: NotRequired[MetadataGenerationRunTypeType],  # (3)
```

1. See [:material-code-brackets: MetadataGenerationRunStatusType](./literals.md#metadatagenerationrunstatustype) 
2. See [:material-code-braces: MetadataGenerationRunTargetTypeDef](./type_defs.md#metadatagenerationruntargettypedef) 
3. See [:material-code-brackets: MetadataGenerationRunTypeType](./literals.md#metadatagenerationruntypetype) 
## StartMetadataGenerationRunInputTypeDef

```python
# StartMetadataGenerationRunInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import StartMetadataGenerationRunInputTypeDef


def get_value() -> StartMetadataGenerationRunInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# StartMetadataGenerationRunInputTypeDef definition

class StartMetadataGenerationRunInputTypeDef(TypedDict):
    domainIdentifier: str,
    owningProjectIdentifier: str,
    target: MetadataGenerationRunTargetTypeDef,  # (1)
    type: MetadataGenerationRunTypeType,  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: MetadataGenerationRunTargetTypeDef](./type_defs.md#metadatagenerationruntargettypedef) 
2. See [:material-code-brackets: MetadataGenerationRunTypeType](./literals.md#metadatagenerationruntypetype) 
## GetTimeSeriesDataPointOutputTypeDef

```python
# GetTimeSeriesDataPointOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetTimeSeriesDataPointOutputTypeDef


def get_value() -> GetTimeSeriesDataPointOutputTypeDef:
    return {
        "domainId": ...,
    }


# GetTimeSeriesDataPointOutputTypeDef definition

class GetTimeSeriesDataPointOutputTypeDef(TypedDict):
    domainId: str,
    entityId: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    form: TimeSeriesDataPointFormOutputTypeDef,  # (2)
    formName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
2. See [:material-code-braces: TimeSeriesDataPointFormOutputTypeDef](./type_defs.md#timeseriesdatapointformoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostTimeSeriesDataPointsOutputTypeDef

```python
# PostTimeSeriesDataPointsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PostTimeSeriesDataPointsOutputTypeDef


def get_value() -> PostTimeSeriesDataPointsOutputTypeDef:
    return {
        "domainId": ...,
    }


# PostTimeSeriesDataPointsOutputTypeDef definition

class PostTimeSeriesDataPointsOutputTypeDef(TypedDict):
    domainId: str,
    entityId: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    forms: List[TimeSeriesDataPointFormOutputTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
2. See [:material-code-braces: TimeSeriesDataPointFormOutputTypeDef](./type_defs.md#timeseriesdatapointformoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GlueSelfGrantStatusOutputTypeDef

```python
# GlueSelfGrantStatusOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlueSelfGrantStatusOutputTypeDef


def get_value() -> GlueSelfGrantStatusOutputTypeDef:
    return {
        "selfGrantStatusDetails": ...,
    }


# GlueSelfGrantStatusOutputTypeDef definition

class GlueSelfGrantStatusOutputTypeDef(TypedDict):
    selfGrantStatusDetails: List[SelfGrantStatusDetailTypeDef],  # (1)
```

1. See [:material-code-braces: SelfGrantStatusDetailTypeDef](./type_defs.md#selfgrantstatusdetailtypedef) 
## RedshiftSelfGrantStatusOutputTypeDef

```python
# RedshiftSelfGrantStatusOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftSelfGrantStatusOutputTypeDef


def get_value() -> RedshiftSelfGrantStatusOutputTypeDef:
    return {
        "selfGrantStatusDetails": ...,
    }


# RedshiftSelfGrantStatusOutputTypeDef definition

class RedshiftSelfGrantStatusOutputTypeDef(TypedDict):
    selfGrantStatusDetails: List[SelfGrantStatusDetailTypeDef],  # (1)
```

1. See [:material-code-braces: SelfGrantStatusDetailTypeDef](./type_defs.md#selfgrantstatusdetailtypedef) 
## GrantedEntityInputTypeDef

```python
# GrantedEntityInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GrantedEntityInputTypeDef


def get_value() -> GrantedEntityInputTypeDef:
    return {
        "listing": ...,
    }


# GrantedEntityInputTypeDef definition

class GrantedEntityInputTypeDef(TypedDict):
    listing: NotRequired[ListingRevisionInputTypeDef],  # (1)
```

1. See [:material-code-braces: ListingRevisionInputTypeDef](./type_defs.md#listingrevisioninputtypedef) 
## GrantedEntityTypeDef

```python
# GrantedEntityTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GrantedEntityTypeDef


def get_value() -> GrantedEntityTypeDef:
    return {
        "listing": ...,
    }


# GrantedEntityTypeDef definition

class GrantedEntityTypeDef(TypedDict):
    listing: NotRequired[ListingRevisionTypeDef],  # (1)
```

1. See [:material-code-braces: ListingRevisionTypeDef](./type_defs.md#listingrevisiontypedef) 
## SearchGroupProfilesOutputTypeDef

```python
# SearchGroupProfilesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchGroupProfilesOutputTypeDef


def get_value() -> SearchGroupProfilesOutputTypeDef:
    return {
        "items": ...,
    }


# SearchGroupProfilesOutputTypeDef definition

class SearchGroupProfilesOutputTypeDef(TypedDict):
    items: List[GroupProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupProfileSummaryTypeDef](./type_defs.md#groupprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisioningConfigurationOutputTypeDef

```python
# ProvisioningConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProvisioningConfigurationOutputTypeDef


def get_value() -> ProvisioningConfigurationOutputTypeDef:
    return {
        "lakeFormationConfiguration": ...,
    }


# ProvisioningConfigurationOutputTypeDef definition

class ProvisioningConfigurationOutputTypeDef(TypedDict):
    lakeFormationConfiguration: NotRequired[LakeFormationConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: LakeFormationConfigurationOutputTypeDef](./type_defs.md#lakeformationconfigurationoutputtypedef) 
## ListLineageNodeHistoryOutputTypeDef

```python
# ListLineageNodeHistoryOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListLineageNodeHistoryOutputTypeDef


def get_value() -> ListLineageNodeHistoryOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListLineageNodeHistoryOutputTypeDef definition

class ListLineageNodeHistoryOutputTypeDef(TypedDict):
    nodes: List[LineageNodeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LineageNodeSummaryTypeDef](./type_defs.md#lineagenodesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LineageRunDetailsTypeDef

```python
# LineageRunDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LineageRunDetailsTypeDef


def get_value() -> LineageRunDetailsTypeDef:
    return {
        "sqlQueryRunDetails": ...,
    }


# LineageRunDetailsTypeDef definition

class LineageRunDetailsTypeDef(TypedDict):
    sqlQueryRunDetails: NotRequired[LineageSqlQueryRunDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: LineageSqlQueryRunDetailsTypeDef](./type_defs.md#lineagesqlqueryrundetailstypedef) 
## RedshiftLineageSyncConfigurationInputTypeDef

```python
# RedshiftLineageSyncConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftLineageSyncConfigurationInputTypeDef


def get_value() -> RedshiftLineageSyncConfigurationInputTypeDef:
    return {
        "enabled": ...,
    }


# RedshiftLineageSyncConfigurationInputTypeDef definition

class RedshiftLineageSyncConfigurationInputTypeDef(TypedDict):
    enabled: NotRequired[bool],
    schedule: NotRequired[LineageSyncScheduleTypeDef],  # (1)
```

1. See [:material-code-braces: LineageSyncScheduleTypeDef](./type_defs.md#lineagesyncscheduletypedef) 
## RedshiftLineageSyncConfigurationOutputTypeDef

```python
# RedshiftLineageSyncConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftLineageSyncConfigurationOutputTypeDef


def get_value() -> RedshiftLineageSyncConfigurationOutputTypeDef:
    return {
        "enabled": ...,
    }


# RedshiftLineageSyncConfigurationOutputTypeDef definition

class RedshiftLineageSyncConfigurationOutputTypeDef(TypedDict):
    enabled: NotRequired[bool],
    lineageJobId: NotRequired[str],
    schedule: NotRequired[LineageSyncScheduleTypeDef],  # (1)
```

1. See [:material-code-braces: LineageSyncScheduleTypeDef](./type_defs.md#lineagesyncscheduletypedef) 
## ListAssetFiltersInputPaginateTypeDef

```python
# ListAssetFiltersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListAssetFiltersInputPaginateTypeDef


def get_value() -> ListAssetFiltersInputPaginateTypeDef:
    return {
        "assetIdentifier": ...,
    }


# ListAssetFiltersInputPaginateTypeDef definition

class ListAssetFiltersInputPaginateTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    status: NotRequired[FilterStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterStatusType](./literals.md#filterstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetRevisionsInputPaginateTypeDef

```python
# ListAssetRevisionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListAssetRevisionsInputPaginateTypeDef


def get_value() -> ListAssetRevisionsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListAssetRevisionsInputPaginateTypeDef definition

class ListAssetRevisionsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConnectionsInputPaginateTypeDef

```python
# ListConnectionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListConnectionsInputPaginateTypeDef


def get_value() -> ListConnectionsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListConnectionsInputPaginateTypeDef definition

class ListConnectionsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    environmentIdentifier: NotRequired[str],
    name: NotRequired[str],
    sortBy: NotRequired[SortFieldConnectionType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    type: NotRequired[ConnectionTypeType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: SortFieldConnectionType](./literals.md#sortfieldconnectiontype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataProductRevisionsInputPaginateTypeDef

```python
# ListDataProductRevisionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataProductRevisionsInputPaginateTypeDef


def get_value() -> ListDataProductRevisionsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListDataProductRevisionsInputPaginateTypeDef definition

class ListDataProductRevisionsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourceRunActivitiesInputPaginateTypeDef

```python
# ListDataSourceRunActivitiesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourceRunActivitiesInputPaginateTypeDef


def get_value() -> ListDataSourceRunActivitiesInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListDataSourceRunActivitiesInputPaginateTypeDef definition

class ListDataSourceRunActivitiesInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    status: NotRequired[DataAssetActivityStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataAssetActivityStatusType](./literals.md#dataassetactivitystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourceRunsInputPaginateTypeDef

```python
# ListDataSourceRunsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourceRunsInputPaginateTypeDef


def get_value() -> ListDataSourceRunsInputPaginateTypeDef:
    return {
        "dataSourceIdentifier": ...,
    }


# ListDataSourceRunsInputPaginateTypeDef definition

class ListDataSourceRunsInputPaginateTypeDef(TypedDict):
    dataSourceIdentifier: str,
    domainIdentifier: str,
    status: NotRequired[DataSourceRunStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourcesInputPaginateTypeDef

```python
# ListDataSourcesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourcesInputPaginateTypeDef


def get_value() -> ListDataSourcesInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListDataSourcesInputPaginateTypeDef definition

class ListDataSourcesInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    connectionIdentifier: NotRequired[str],
    environmentIdentifier: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[DataSourceStatusType],  # (1)
    type: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainUnitsForParentInputPaginateTypeDef

```python
# ListDomainUnitsForParentInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDomainUnitsForParentInputPaginateTypeDef


def get_value() -> ListDomainUnitsForParentInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListDomainUnitsForParentInputPaginateTypeDef definition

class ListDomainUnitsForParentInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    parentDomainUnitIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsInputPaginateTypeDef

```python
# ListDomainsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDomainsInputPaginateTypeDef


def get_value() -> ListDomainsInputPaginateTypeDef:
    return {
        "status": ...,
    }


# ListDomainsInputPaginateTypeDef definition

class ListDomainsInputPaginateTypeDef(TypedDict):
    status: NotRequired[DomainStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntityOwnersInputPaginateTypeDef

```python
# ListEntityOwnersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEntityOwnersInputPaginateTypeDef


def get_value() -> ListEntityOwnersInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEntityOwnersInputPaginateTypeDef definition

class ListEntityOwnersInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: DataZoneEntityTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataZoneEntityTypeType](./literals.md#datazoneentitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentActionsInputPaginateTypeDef

```python
# ListEnvironmentActionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentActionsInputPaginateTypeDef


def get_value() -> ListEnvironmentActionsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentActionsInputPaginateTypeDef definition

class ListEnvironmentActionsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentBlueprintConfigurationsInputPaginateTypeDef

```python
# ListEnvironmentBlueprintConfigurationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentBlueprintConfigurationsInputPaginateTypeDef


def get_value() -> ListEnvironmentBlueprintConfigurationsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentBlueprintConfigurationsInputPaginateTypeDef definition

class ListEnvironmentBlueprintConfigurationsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentBlueprintsInputPaginateTypeDef

```python
# ListEnvironmentBlueprintsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentBlueprintsInputPaginateTypeDef


def get_value() -> ListEnvironmentBlueprintsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentBlueprintsInputPaginateTypeDef definition

class ListEnvironmentBlueprintsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    managed: NotRequired[bool],
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentProfilesInputPaginateTypeDef

```python
# ListEnvironmentProfilesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentProfilesInputPaginateTypeDef


def get_value() -> ListEnvironmentProfilesInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentProfilesInputPaginateTypeDef definition

class ListEnvironmentProfilesInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    environmentBlueprintIdentifier: NotRequired[str],
    name: NotRequired[str],
    projectIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsInputPaginateTypeDef

```python
# ListEnvironmentsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentsInputPaginateTypeDef


def get_value() -> ListEnvironmentsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListEnvironmentsInputPaginateTypeDef definition

class ListEnvironmentsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    environmentBlueprintIdentifier: NotRequired[str],
    environmentProfileIdentifier: NotRequired[str],
    name: NotRequired[str],
    provider: NotRequired[str],
    status: NotRequired[EnvironmentStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListJobRunsInputPaginateTypeDef

```python
# ListJobRunsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListJobRunsInputPaginateTypeDef


def get_value() -> ListJobRunsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListJobRunsInputPaginateTypeDef definition

class ListJobRunsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    jobIdentifier: str,
    sortOrder: NotRequired[SortOrderType],  # (1)
    status: NotRequired[JobRunStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: JobRunStatusType](./literals.md#jobrunstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLineageEventsInputPaginateTypeDef

```python
# ListLineageEventsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListLineageEventsInputPaginateTypeDef


def get_value() -> ListLineageEventsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListLineageEventsInputPaginateTypeDef definition

class ListLineageEventsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    processingStatus: NotRequired[LineageEventProcessingStatusType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    timestampAfter: NotRequired[TimestampTypeDef],
    timestampBefore: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: LineageEventProcessingStatusType](./literals.md#lineageeventprocessingstatustype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLineageNodeHistoryInputPaginateTypeDef

```python
# ListLineageNodeHistoryInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListLineageNodeHistoryInputPaginateTypeDef


def get_value() -> ListLineageNodeHistoryInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListLineageNodeHistoryInputPaginateTypeDef definition

class ListLineageNodeHistoryInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    direction: NotRequired[EdgeDirectionType],  # (1)
    eventTimestampGTE: NotRequired[TimestampTypeDef],
    eventTimestampLTE: NotRequired[TimestampTypeDef],
    sortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: EdgeDirectionType](./literals.md#edgedirectiontype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListMetadataGenerationRunsInputPaginateTypeDef

```python
# ListMetadataGenerationRunsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListMetadataGenerationRunsInputPaginateTypeDef


def get_value() -> ListMetadataGenerationRunsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListMetadataGenerationRunsInputPaginateTypeDef definition

class ListMetadataGenerationRunsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    status: NotRequired[MetadataGenerationRunStatusType],  # (1)
    type: NotRequired[MetadataGenerationRunTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MetadataGenerationRunStatusType](./literals.md#metadatagenerationrunstatustype) 
2. See [:material-code-brackets: MetadataGenerationRunTypeType](./literals.md#metadatagenerationruntypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationsInputPaginateTypeDef

```python
# ListNotificationsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListNotificationsInputPaginateTypeDef


def get_value() -> ListNotificationsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListNotificationsInputPaginateTypeDef definition

class ListNotificationsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    type: NotificationTypeType,  # (1)
    afterTimestamp: NotRequired[TimestampTypeDef],
    beforeTimestamp: NotRequired[TimestampTypeDef],
    subjects: NotRequired[Sequence[str]],
    taskStatus: NotRequired[TaskStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPolicyGrantsInputPaginateTypeDef

```python
# ListPolicyGrantsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListPolicyGrantsInputPaginateTypeDef


def get_value() -> ListPolicyGrantsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListPolicyGrantsInputPaginateTypeDef definition

class ListPolicyGrantsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TargetEntityTypeType,  # (1)
    policyType: ManagedPolicyTypeType,  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: TargetEntityTypeType](./literals.md#targetentitytypetype) 
2. See [:material-code-brackets: ManagedPolicyTypeType](./literals.md#managedpolicytypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectMembershipsInputPaginateTypeDef

```python
# ListProjectMembershipsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectMembershipsInputPaginateTypeDef


def get_value() -> ListProjectMembershipsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListProjectMembershipsInputPaginateTypeDef definition

class ListProjectMembershipsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    sortBy: NotRequired[SortFieldProjectType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortFieldProjectType](./literals.md#sortfieldprojecttype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectProfilesInputPaginateTypeDef

```python
# ListProjectProfilesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectProfilesInputPaginateTypeDef


def get_value() -> ListProjectProfilesInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListProjectProfilesInputPaginateTypeDef definition

class ListProjectProfilesInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    name: NotRequired[str],
    sortBy: NotRequired[SortFieldProjectType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortFieldProjectType](./literals.md#sortfieldprojecttype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsInputPaginateTypeDef

```python
# ListProjectsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectsInputPaginateTypeDef


def get_value() -> ListProjectsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListProjectsInputPaginateTypeDef definition

class ListProjectsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: NotRequired[str],
    name: NotRequired[str],
    userIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesInputPaginateTypeDef

```python
# ListRulesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListRulesInputPaginateTypeDef


def get_value() -> ListRulesInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListRulesInputPaginateTypeDef definition

class ListRulesInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    targetIdentifier: str,
    targetType: RuleTargetTypeType,  # (1)
    action: NotRequired[RuleActionType],  # (2)
    assetTypes: NotRequired[Sequence[str]],
    dataProduct: NotRequired[bool],
    includeCascaded: NotRequired[bool],
    projectIds: NotRequired[Sequence[str]],
    ruleType: NotRequired[RuleTypeType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: RuleTargetTypeType](./literals.md#ruletargettypetype) 
2. See [:material-code-brackets: RuleActionType](./literals.md#ruleactiontype) 
3. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionGrantsInputPaginateTypeDef

```python
# ListSubscriptionGrantsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionGrantsInputPaginateTypeDef


def get_value() -> ListSubscriptionGrantsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListSubscriptionGrantsInputPaginateTypeDef definition

class ListSubscriptionGrantsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    environmentId: NotRequired[str],
    owningProjectId: NotRequired[str],
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    subscribedListingId: NotRequired[str],
    subscriptionId: NotRequired[str],
    subscriptionTargetId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionRequestsInputPaginateTypeDef

```python
# ListSubscriptionRequestsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionRequestsInputPaginateTypeDef


def get_value() -> ListSubscriptionRequestsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListSubscriptionRequestsInputPaginateTypeDef definition

class ListSubscriptionRequestsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    approverProjectId: NotRequired[str],
    owningProjectId: NotRequired[str],
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    status: NotRequired[SubscriptionRequestStatusType],  # (3)
    subscribedListingId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionTargetsInputPaginateTypeDef

```python
# ListSubscriptionTargetsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionTargetsInputPaginateTypeDef


def get_value() -> ListSubscriptionTargetsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListSubscriptionTargetsInputPaginateTypeDef definition

class ListSubscriptionTargetsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionsInputPaginateTypeDef

```python
# ListSubscriptionsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionsInputPaginateTypeDef


def get_value() -> ListSubscriptionsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListSubscriptionsInputPaginateTypeDef definition

class ListSubscriptionsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    approverProjectId: NotRequired[str],
    owningProjectId: NotRequired[str],
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    status: NotRequired[SubscriptionStatusType],  # (3)
    subscribedListingId: NotRequired[str],
    subscriptionRequestIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTimeSeriesDataPointsInputPaginateTypeDef

```python
# ListTimeSeriesDataPointsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListTimeSeriesDataPointsInputPaginateTypeDef


def get_value() -> ListTimeSeriesDataPointsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# ListTimeSeriesDataPointsInputPaginateTypeDef definition

class ListTimeSeriesDataPointsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    formName: str,
    endedAt: NotRequired[TimestampTypeDef],
    startedAt: NotRequired[TimestampTypeDef],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchGroupProfilesInputPaginateTypeDef

```python
# SearchGroupProfilesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchGroupProfilesInputPaginateTypeDef


def get_value() -> SearchGroupProfilesInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchGroupProfilesInputPaginateTypeDef definition

class SearchGroupProfilesInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    groupType: GroupSearchTypeType,  # (1)
    searchText: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: GroupSearchTypeType](./literals.md#groupsearchtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchUserProfilesInputPaginateTypeDef

```python
# SearchUserProfilesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchUserProfilesInputPaginateTypeDef


def get_value() -> SearchUserProfilesInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchUserProfilesInputPaginateTypeDef definition

class SearchUserProfilesInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    userType: UserSearchTypeType,  # (1)
    searchText: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UserSearchTypeType](./literals.md#usersearchtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectProfilesOutputTypeDef

```python
# ListProjectProfilesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectProfilesOutputTypeDef


def get_value() -> ListProjectProfilesOutputTypeDef:
    return {
        "items": ...,
    }


# ListProjectProfilesOutputTypeDef definition

class ListProjectProfilesOutputTypeDef(TypedDict):
    items: List[ProjectProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectProfileSummaryTypeDef](./type_defs.md#projectprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## MemberDetailsTypeDef

```python
# MemberDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import MemberDetailsTypeDef


def get_value() -> MemberDetailsTypeDef:
    return {
        "group": ...,
    }


# MemberDetailsTypeDef definition

class MemberDetailsTypeDef(TypedDict):
    group: NotRequired[GroupDetailsTypeDef],  # (1)
    user: NotRequired[UserDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: GroupDetailsTypeDef](./type_defs.md#groupdetailstypedef) 
2. See [:material-code-braces: UserDetailsTypeDef](./type_defs.md#userdetailstypedef) 
## MetadataFormEnforcementDetailOutputTypeDef

```python
# MetadataFormEnforcementDetailOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import MetadataFormEnforcementDetailOutputTypeDef


def get_value() -> MetadataFormEnforcementDetailOutputTypeDef:
    return {
        "requiredMetadataForms": ...,
    }


# MetadataFormEnforcementDetailOutputTypeDef definition

class MetadataFormEnforcementDetailOutputTypeDef(TypedDict):
    requiredMetadataForms: NotRequired[List[MetadataFormReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: MetadataFormReferenceTypeDef](./type_defs.md#metadataformreferencetypedef) 
## MetadataFormEnforcementDetailTypeDef

```python
# MetadataFormEnforcementDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import MetadataFormEnforcementDetailTypeDef


def get_value() -> MetadataFormEnforcementDetailTypeDef:
    return {
        "requiredMetadataForms": ...,
    }


# MetadataFormEnforcementDetailTypeDef definition

class MetadataFormEnforcementDetailTypeDef(TypedDict):
    requiredMetadataForms: NotRequired[Sequence[MetadataFormReferenceTypeDef]],  # (1)
```

1. See [:material-code-braces: MetadataFormReferenceTypeDef](./type_defs.md#metadataformreferencetypedef) 
## OpenLineageRunEventSummaryTypeDef

```python
# OpenLineageRunEventSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OpenLineageRunEventSummaryTypeDef


def get_value() -> OpenLineageRunEventSummaryTypeDef:
    return {
        "eventType": ...,
    }


# OpenLineageRunEventSummaryTypeDef definition

class OpenLineageRunEventSummaryTypeDef(TypedDict):
    eventType: NotRequired[OpenLineageRunStateType],  # (1)
    inputs: NotRequired[List[NameIdentifierTypeDef]],  # (2)
    job: NotRequired[NameIdentifierTypeDef],  # (3)
    outputs: NotRequired[List[NameIdentifierTypeDef]],  # (2)
    runId: NotRequired[str],
```

1. See [:material-code-brackets: OpenLineageRunStateType](./literals.md#openlineagerunstatetype) 
2. See [:material-code-braces: NameIdentifierTypeDef](./type_defs.md#nameidentifiertypedef) 
3. See [:material-code-braces: NameIdentifierTypeDef](./type_defs.md#nameidentifiertypedef) 
4. See [:material-code-braces: NameIdentifierTypeDef](./type_defs.md#nameidentifiertypedef) 
## RowFilterExpressionOutputTypeDef

```python
# RowFilterExpressionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RowFilterExpressionOutputTypeDef


def get_value() -> RowFilterExpressionOutputTypeDef:
    return {
        "equalTo": ...,
    }


# RowFilterExpressionOutputTypeDef definition

class RowFilterExpressionOutputTypeDef(TypedDict):
    equalTo: NotRequired[EqualToExpressionTypeDef],  # (1)
    greaterThan: NotRequired[GreaterThanExpressionTypeDef],  # (2)
    greaterThanOrEqualTo: NotRequired[GreaterThanOrEqualToExpressionTypeDef],  # (3)
    in: NotRequired[InExpressionOutputTypeDef],  # (4)
    isNotNull: NotRequired[IsNotNullExpressionTypeDef],  # (5)
    isNull: NotRequired[IsNullExpressionTypeDef],  # (6)
    lessThan: NotRequired[LessThanExpressionTypeDef],  # (7)
    lessThanOrEqualTo: NotRequired[LessThanOrEqualToExpressionTypeDef],  # (8)
    like: NotRequired[LikeExpressionTypeDef],  # (9)
    notEqualTo: NotRequired[NotEqualToExpressionTypeDef],  # (10)
    notIn: NotRequired[NotInExpressionOutputTypeDef],  # (11)
    notLike: NotRequired[NotLikeExpressionTypeDef],  # (12)
```

1. See [:material-code-braces: EqualToExpressionTypeDef](./type_defs.md#equaltoexpressiontypedef) 
2. See [:material-code-braces: GreaterThanExpressionTypeDef](./type_defs.md#greaterthanexpressiontypedef) 
3. See [:material-code-braces: GreaterThanOrEqualToExpressionTypeDef](./type_defs.md#greaterthanorequaltoexpressiontypedef) 
4. See [:material-code-braces: InExpressionOutputTypeDef](./type_defs.md#inexpressionoutputtypedef) 
5. See [:material-code-braces: IsNotNullExpressionTypeDef](./type_defs.md#isnotnullexpressiontypedef) 
6. See [:material-code-braces: IsNullExpressionTypeDef](./type_defs.md#isnullexpressiontypedef) 
7. See [:material-code-braces: LessThanExpressionTypeDef](./type_defs.md#lessthanexpressiontypedef) 
8. See [:material-code-braces: LessThanOrEqualToExpressionTypeDef](./type_defs.md#lessthanorequaltoexpressiontypedef) 
9. See [:material-code-braces: LikeExpressionTypeDef](./type_defs.md#likeexpressiontypedef) 
10. See [:material-code-braces: NotEqualToExpressionTypeDef](./type_defs.md#notequaltoexpressiontypedef) 
11. See [:material-code-braces: NotInExpressionOutputTypeDef](./type_defs.md#notinexpressionoutputtypedef) 
12. See [:material-code-braces: NotLikeExpressionTypeDef](./type_defs.md#notlikeexpressiontypedef) 
## RowFilterExpressionTypeDef

```python
# RowFilterExpressionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RowFilterExpressionTypeDef


def get_value() -> RowFilterExpressionTypeDef:
    return {
        "equalTo": ...,
    }


# RowFilterExpressionTypeDef definition

class RowFilterExpressionTypeDef(TypedDict):
    equalTo: NotRequired[EqualToExpressionTypeDef],  # (1)
    greaterThan: NotRequired[GreaterThanExpressionTypeDef],  # (2)
    greaterThanOrEqualTo: NotRequired[GreaterThanOrEqualToExpressionTypeDef],  # (3)
    in: NotRequired[InExpressionTypeDef],  # (4)
    isNotNull: NotRequired[IsNotNullExpressionTypeDef],  # (5)
    isNull: NotRequired[IsNullExpressionTypeDef],  # (6)
    lessThan: NotRequired[LessThanExpressionTypeDef],  # (7)
    lessThanOrEqualTo: NotRequired[LessThanOrEqualToExpressionTypeDef],  # (8)
    like: NotRequired[LikeExpressionTypeDef],  # (9)
    notEqualTo: NotRequired[NotEqualToExpressionTypeDef],  # (10)
    notIn: NotRequired[NotInExpressionTypeDef],  # (11)
    notLike: NotRequired[NotLikeExpressionTypeDef],  # (12)
```

1. See [:material-code-braces: EqualToExpressionTypeDef](./type_defs.md#equaltoexpressiontypedef) 
2. See [:material-code-braces: GreaterThanExpressionTypeDef](./type_defs.md#greaterthanexpressiontypedef) 
3. See [:material-code-braces: GreaterThanOrEqualToExpressionTypeDef](./type_defs.md#greaterthanorequaltoexpressiontypedef) 
4. See [:material-code-braces: InExpressionTypeDef](./type_defs.md#inexpressiontypedef) 
5. See [:material-code-braces: IsNotNullExpressionTypeDef](./type_defs.md#isnotnullexpressiontypedef) 
6. See [:material-code-braces: IsNullExpressionTypeDef](./type_defs.md#isnullexpressiontypedef) 
7. See [:material-code-braces: LessThanExpressionTypeDef](./type_defs.md#lessthanexpressiontypedef) 
8. See [:material-code-braces: LessThanOrEqualToExpressionTypeDef](./type_defs.md#lessthanorequaltoexpressiontypedef) 
9. See [:material-code-braces: LikeExpressionTypeDef](./type_defs.md#likeexpressiontypedef) 
10. See [:material-code-braces: NotEqualToExpressionTypeDef](./type_defs.md#notequaltoexpressiontypedef) 
11. See [:material-code-braces: NotInExpressionTypeDef](./type_defs.md#notinexpressiontypedef) 
12. See [:material-code-braces: NotLikeExpressionTypeDef](./type_defs.md#notlikeexpressiontypedef) 
## TopicTypeDef

```python
# TopicTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import TopicTypeDef


def get_value() -> TopicTypeDef:
    return {
        "resource": ...,
    }


# TopicTypeDef definition

class TopicTypeDef(TypedDict):
    resource: NotificationResourceTypeDef,  # (1)
    role: NotificationRoleType,  # (2)
    subject: str,
```

1. See [:material-code-braces: NotificationResourceTypeDef](./type_defs.md#notificationresourcetypedef) 
2. See [:material-code-brackets: NotificationRoleType](./literals.md#notificationroletype) 
## OAuth2PropertiesOutputTypeDef

```python
# OAuth2PropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OAuth2PropertiesOutputTypeDef


def get_value() -> OAuth2PropertiesOutputTypeDef:
    return {
        "authorizationCodeProperties": ...,
    }


# OAuth2PropertiesOutputTypeDef definition

class OAuth2PropertiesOutputTypeDef(TypedDict):
    authorizationCodeProperties: NotRequired[AuthorizationCodePropertiesTypeDef],  # (1)
    oAuth2ClientApplication: NotRequired[OAuth2ClientApplicationTypeDef],  # (2)
    oAuth2Credentials: NotRequired[GlueOAuth2CredentialsTypeDef],  # (3)
    oAuth2GrantType: NotRequired[OAuth2GrantTypeType],  # (4)
    tokenUrl: NotRequired[str],
    tokenUrlParametersMap: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: AuthorizationCodePropertiesTypeDef](./type_defs.md#authorizationcodepropertiestypedef) 
2. See [:material-code-braces: OAuth2ClientApplicationTypeDef](./type_defs.md#oauth2clientapplicationtypedef) 
3. See [:material-code-braces: GlueOAuth2CredentialsTypeDef](./type_defs.md#glueoauth2credentialstypedef) 
4. See [:material-code-brackets: OAuth2GrantTypeType](./literals.md#oauth2granttypetype) 
## OAuth2PropertiesTypeDef

```python
# OAuth2PropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OAuth2PropertiesTypeDef


def get_value() -> OAuth2PropertiesTypeDef:
    return {
        "authorizationCodeProperties": ...,
    }


# OAuth2PropertiesTypeDef definition

class OAuth2PropertiesTypeDef(TypedDict):
    authorizationCodeProperties: NotRequired[AuthorizationCodePropertiesTypeDef],  # (1)
    oAuth2ClientApplication: NotRequired[OAuth2ClientApplicationTypeDef],  # (2)
    oAuth2Credentials: NotRequired[GlueOAuth2CredentialsTypeDef],  # (3)
    oAuth2GrantType: NotRequired[OAuth2GrantTypeType],  # (4)
    tokenUrl: NotRequired[str],
    tokenUrlParametersMap: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: AuthorizationCodePropertiesTypeDef](./type_defs.md#authorizationcodepropertiestypedef) 
2. See [:material-code-braces: OAuth2ClientApplicationTypeDef](./type_defs.md#oauth2clientapplicationtypedef) 
3. See [:material-code-braces: GlueOAuth2CredentialsTypeDef](./type_defs.md#glueoauth2credentialstypedef) 
4. See [:material-code-brackets: OAuth2GrantTypeType](./literals.md#oauth2granttypetype) 
## PolicyGrantDetailOutputTypeDef

```python
# PolicyGrantDetailOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PolicyGrantDetailOutputTypeDef


def get_value() -> PolicyGrantDetailOutputTypeDef:
    return {
        "addToProjectMemberPool": ...,
    }


# PolicyGrantDetailOutputTypeDef definition

class PolicyGrantDetailOutputTypeDef(TypedDict):
    addToProjectMemberPool: NotRequired[AddToProjectMemberPoolPolicyGrantDetailTypeDef],  # (1)
    createAssetType: NotRequired[CreateAssetTypePolicyGrantDetailTypeDef],  # (2)
    createDomainUnit: NotRequired[CreateDomainUnitPolicyGrantDetailTypeDef],  # (3)
    createEnvironment: NotRequired[Dict[str, Any]],
    createEnvironmentFromBlueprint: NotRequired[Dict[str, Any]],
    createEnvironmentProfile: NotRequired[CreateEnvironmentProfilePolicyGrantDetailTypeDef],  # (4)
    createFormType: NotRequired[CreateFormTypePolicyGrantDetailTypeDef],  # (5)
    createGlossary: NotRequired[CreateGlossaryPolicyGrantDetailTypeDef],  # (6)
    createProject: NotRequired[CreateProjectPolicyGrantDetailTypeDef],  # (7)
    createProjectFromProjectProfile: NotRequired[CreateProjectFromProjectProfilePolicyGrantDetailOutputTypeDef],  # (8)
    delegateCreateEnvironmentProfile: NotRequired[Dict[str, Any]],
    overrideDomainUnitOwners: NotRequired[OverrideDomainUnitOwnersPolicyGrantDetailTypeDef],  # (9)
    overrideProjectOwners: NotRequired[OverrideProjectOwnersPolicyGrantDetailTypeDef],  # (10)
```

1. See [:material-code-braces: AddToProjectMemberPoolPolicyGrantDetailTypeDef](./type_defs.md#addtoprojectmemberpoolpolicygrantdetailtypedef) 
2. See [:material-code-braces: CreateAssetTypePolicyGrantDetailTypeDef](./type_defs.md#createassettypepolicygrantdetailtypedef) 
3. See [:material-code-braces: CreateDomainUnitPolicyGrantDetailTypeDef](./type_defs.md#createdomainunitpolicygrantdetailtypedef) 
4. See [:material-code-braces: CreateEnvironmentProfilePolicyGrantDetailTypeDef](./type_defs.md#createenvironmentprofilepolicygrantdetailtypedef) 
5. See [:material-code-braces: CreateFormTypePolicyGrantDetailTypeDef](./type_defs.md#createformtypepolicygrantdetailtypedef) 
6. See [:material-code-braces: CreateGlossaryPolicyGrantDetailTypeDef](./type_defs.md#createglossarypolicygrantdetailtypedef) 
7. See [:material-code-braces: CreateProjectPolicyGrantDetailTypeDef](./type_defs.md#createprojectpolicygrantdetailtypedef) 
8. See [:material-code-braces: CreateProjectFromProjectProfilePolicyGrantDetailOutputTypeDef](./type_defs.md#createprojectfromprojectprofilepolicygrantdetailoutputtypedef) 
9. See [:material-code-braces: OverrideDomainUnitOwnersPolicyGrantDetailTypeDef](./type_defs.md#overridedomainunitownerspolicygrantdetailtypedef) 
10. See [:material-code-braces: OverrideProjectOwnersPolicyGrantDetailTypeDef](./type_defs.md#overrideprojectownerspolicygrantdetailtypedef) 
## PolicyGrantDetailTypeDef

```python
# PolicyGrantDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PolicyGrantDetailTypeDef


def get_value() -> PolicyGrantDetailTypeDef:
    return {
        "addToProjectMemberPool": ...,
    }


# PolicyGrantDetailTypeDef definition

class PolicyGrantDetailTypeDef(TypedDict):
    addToProjectMemberPool: NotRequired[AddToProjectMemberPoolPolicyGrantDetailTypeDef],  # (1)
    createAssetType: NotRequired[CreateAssetTypePolicyGrantDetailTypeDef],  # (2)
    createDomainUnit: NotRequired[CreateDomainUnitPolicyGrantDetailTypeDef],  # (3)
    createEnvironment: NotRequired[Mapping[str, Any]],
    createEnvironmentFromBlueprint: NotRequired[Mapping[str, Any]],
    createEnvironmentProfile: NotRequired[CreateEnvironmentProfilePolicyGrantDetailTypeDef],  # (4)
    createFormType: NotRequired[CreateFormTypePolicyGrantDetailTypeDef],  # (5)
    createGlossary: NotRequired[CreateGlossaryPolicyGrantDetailTypeDef],  # (6)
    createProject: NotRequired[CreateProjectPolicyGrantDetailTypeDef],  # (7)
    createProjectFromProjectProfile: NotRequired[CreateProjectFromProjectProfilePolicyGrantDetailTypeDef],  # (8)
    delegateCreateEnvironmentProfile: NotRequired[Mapping[str, Any]],
    overrideDomainUnitOwners: NotRequired[OverrideDomainUnitOwnersPolicyGrantDetailTypeDef],  # (9)
    overrideProjectOwners: NotRequired[OverrideProjectOwnersPolicyGrantDetailTypeDef],  # (10)
```

1. See [:material-code-braces: AddToProjectMemberPoolPolicyGrantDetailTypeDef](./type_defs.md#addtoprojectmemberpoolpolicygrantdetailtypedef) 
2. See [:material-code-braces: CreateAssetTypePolicyGrantDetailTypeDef](./type_defs.md#createassettypepolicygrantdetailtypedef) 
3. See [:material-code-braces: CreateDomainUnitPolicyGrantDetailTypeDef](./type_defs.md#createdomainunitpolicygrantdetailtypedef) 
4. See [:material-code-braces: CreateEnvironmentProfilePolicyGrantDetailTypeDef](./type_defs.md#createenvironmentprofilepolicygrantdetailtypedef) 
5. See [:material-code-braces: CreateFormTypePolicyGrantDetailTypeDef](./type_defs.md#createformtypepolicygrantdetailtypedef) 
6. See [:material-code-braces: CreateGlossaryPolicyGrantDetailTypeDef](./type_defs.md#createglossarypolicygrantdetailtypedef) 
7. See [:material-code-braces: CreateProjectPolicyGrantDetailTypeDef](./type_defs.md#createprojectpolicygrantdetailtypedef) 
8. See [:material-code-braces: CreateProjectFromProjectProfilePolicyGrantDetailTypeDef](./type_defs.md#createprojectfromprojectprofilepolicygrantdetailtypedef) 
9. See [:material-code-braces: OverrideDomainUnitOwnersPolicyGrantDetailTypeDef](./type_defs.md#overridedomainunitownerspolicygrantdetailtypedef) 
10. See [:material-code-braces: OverrideProjectOwnersPolicyGrantDetailTypeDef](./type_defs.md#overrideprojectownerspolicygrantdetailtypedef) 
## OwnerPropertiesOutputTypeDef

```python
# OwnerPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OwnerPropertiesOutputTypeDef


def get_value() -> OwnerPropertiesOutputTypeDef:
    return {
        "group": ...,
    }


# OwnerPropertiesOutputTypeDef definition

class OwnerPropertiesOutputTypeDef(TypedDict):
    group: NotRequired[OwnerGroupPropertiesOutputTypeDef],  # (1)
    user: NotRequired[OwnerUserPropertiesOutputTypeDef],  # (2)
```

1. See [:material-code-braces: OwnerGroupPropertiesOutputTypeDef](./type_defs.md#ownergrouppropertiesoutputtypedef) 
2. See [:material-code-braces: OwnerUserPropertiesOutputTypeDef](./type_defs.md#owneruserpropertiesoutputtypedef) 
## OwnerPropertiesTypeDef

```python
# OwnerPropertiesTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import OwnerPropertiesTypeDef


def get_value() -> OwnerPropertiesTypeDef:
    return {
        "group": ...,
    }


# OwnerPropertiesTypeDef definition

class OwnerPropertiesTypeDef(TypedDict):
    group: NotRequired[OwnerGroupPropertiesTypeDef],  # (1)
    user: NotRequired[OwnerUserPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: OwnerGroupPropertiesTypeDef](./type_defs.md#ownergrouppropertiestypedef) 
2. See [:material-code-braces: OwnerUserPropertiesTypeDef](./type_defs.md#owneruserpropertiestypedef) 
## RuleScopeOutputTypeDef

```python
# RuleScopeOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RuleScopeOutputTypeDef


def get_value() -> RuleScopeOutputTypeDef:
    return {
        "assetType": ...,
    }


# RuleScopeOutputTypeDef definition

class RuleScopeOutputTypeDef(TypedDict):
    assetType: NotRequired[AssetTypesForRuleOutputTypeDef],  # (1)
    dataProduct: NotRequired[bool],
    project: NotRequired[ProjectsForRuleOutputTypeDef],  # (2)
```

1. See [:material-code-braces: AssetTypesForRuleOutputTypeDef](./type_defs.md#assettypesforruleoutputtypedef) 
2. See [:material-code-braces: ProjectsForRuleOutputTypeDef](./type_defs.md#projectsforruleoutputtypedef) 
## RuleScopeTypeDef

```python
# RuleScopeTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RuleScopeTypeDef


def get_value() -> RuleScopeTypeDef:
    return {
        "assetType": ...,
    }


# RuleScopeTypeDef definition

class RuleScopeTypeDef(TypedDict):
    assetType: NotRequired[AssetTypesForRuleTypeDef],  # (1)
    dataProduct: NotRequired[bool],
    project: NotRequired[ProjectsForRuleTypeDef],  # (2)
```

1. See [:material-code-braces: AssetTypesForRuleTypeDef](./type_defs.md#assettypesforruletypedef) 
2. See [:material-code-braces: ProjectsForRuleTypeDef](./type_defs.md#projectsforruletypedef) 
## RedshiftCredentialsTypeDef

```python
# RedshiftCredentialsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftCredentialsTypeDef


def get_value() -> RedshiftCredentialsTypeDef:
    return {
        "secretArn": ...,
    }


# RedshiftCredentialsTypeDef definition

class RedshiftCredentialsTypeDef(TypedDict):
    secretArn: NotRequired[str],
    usernamePassword: NotRequired[UsernamePasswordTypeDef],  # (1)
```

1. See [:material-code-braces: UsernamePasswordTypeDef](./type_defs.md#usernamepasswordtypedef) 
## SparkEmrPropertiesOutputTypeDef

```python
# SparkEmrPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SparkEmrPropertiesOutputTypeDef


def get_value() -> SparkEmrPropertiesOutputTypeDef:
    return {
        "computeArn": ...,
    }


# SparkEmrPropertiesOutputTypeDef definition

class SparkEmrPropertiesOutputTypeDef(TypedDict):
    computeArn: NotRequired[str],
    credentials: NotRequired[UsernamePasswordTypeDef],  # (1)
    credentialsExpiration: NotRequired[datetime],
    governanceType: NotRequired[GovernanceTypeType],  # (2)
    instanceProfileArn: NotRequired[str],
    javaVirtualEnv: NotRequired[str],
    livyEndpoint: NotRequired[str],
    logUri: NotRequired[str],
    pythonVirtualEnv: NotRequired[str],
    runtimeRole: NotRequired[str],
    trustedCertificatesS3Uri: NotRequired[str],
```

1. See [:material-code-braces: UsernamePasswordTypeDef](./type_defs.md#usernamepasswordtypedef) 
2. See [:material-code-brackets: GovernanceTypeType](./literals.md#governancetypetype) 
## RedshiftStorageTypeDef

```python
# RedshiftStorageTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftStorageTypeDef


def get_value() -> RedshiftStorageTypeDef:
    return {
        "redshiftClusterSource": ...,
    }


# RedshiftStorageTypeDef definition

class RedshiftStorageTypeDef(TypedDict):
    redshiftClusterSource: NotRequired[RedshiftClusterStorageTypeDef],  # (1)
    redshiftServerlessSource: NotRequired[RedshiftServerlessStorageTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftClusterStorageTypeDef](./type_defs.md#redshiftclusterstoragetypedef) 
2. See [:material-code-braces: RedshiftServerlessStorageTypeDef](./type_defs.md#redshiftserverlessstoragetypedef) 
## RejectPredictionsInputTypeDef

```python
# RejectPredictionsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RejectPredictionsInputTypeDef


def get_value() -> RejectPredictionsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# RejectPredictionsInputTypeDef definition

class RejectPredictionsInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    clientToken: NotRequired[str],
    rejectChoices: NotRequired[Sequence[RejectChoiceTypeDef]],  # (1)
    rejectRule: NotRequired[RejectRuleTypeDef],  # (2)
    revision: NotRequired[str],
```

1. See [:material-code-braces: RejectChoiceTypeDef](./type_defs.md#rejectchoicetypedef) 
2. See [:material-code-braces: RejectRuleTypeDef](./type_defs.md#rejectruletypedef) 
## SparkGluePropertiesInputTypeDef

```python
# SparkGluePropertiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SparkGluePropertiesInputTypeDef


def get_value() -> SparkGluePropertiesInputTypeDef:
    return {
        "additionalArgs": ...,
    }


# SparkGluePropertiesInputTypeDef definition

class SparkGluePropertiesInputTypeDef(TypedDict):
    additionalArgs: NotRequired[SparkGlueArgsTypeDef],  # (1)
    glueConnectionName: NotRequired[str],
    glueVersion: NotRequired[str],
    idleTimeout: NotRequired[int],
    javaVirtualEnv: NotRequired[str],
    numberOfWorkers: NotRequired[int],
    pythonVirtualEnv: NotRequired[str],
    workerType: NotRequired[str],
```

1. See [:material-code-braces: SparkGlueArgsTypeDef](./type_defs.md#sparkglueargstypedef) 
## SparkGluePropertiesOutputTypeDef

```python
# SparkGluePropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SparkGluePropertiesOutputTypeDef


def get_value() -> SparkGluePropertiesOutputTypeDef:
    return {
        "additionalArgs": ...,
    }


# SparkGluePropertiesOutputTypeDef definition

class SparkGluePropertiesOutputTypeDef(TypedDict):
    additionalArgs: NotRequired[SparkGlueArgsTypeDef],  # (1)
    glueConnectionName: NotRequired[str],
    glueVersion: NotRequired[str],
    idleTimeout: NotRequired[int],
    javaVirtualEnv: NotRequired[str],
    numberOfWorkers: NotRequired[int],
    pythonVirtualEnv: NotRequired[str],
    workerType: NotRequired[str],
```

1. See [:material-code-braces: SparkGlueArgsTypeDef](./type_defs.md#sparkglueargstypedef) 
## UserProfileDetailsTypeDef

```python
# UserProfileDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UserProfileDetailsTypeDef


def get_value() -> UserProfileDetailsTypeDef:
    return {
        "iam": ...,
    }


# UserProfileDetailsTypeDef definition

class UserProfileDetailsTypeDef(TypedDict):
    iam: NotRequired[IamUserProfileDetailsTypeDef],  # (1)
    sso: NotRequired[SsoUserProfileDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: IamUserProfileDetailsTypeDef](./type_defs.md#iamuserprofiledetailstypedef) 
2. See [:material-code-braces: SsoUserProfileDetailsTypeDef](./type_defs.md#ssouserprofiledetailstypedef) 
## SubscribedPrincipalInputTypeDef

```python
# SubscribedPrincipalInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedPrincipalInputTypeDef


def get_value() -> SubscribedPrincipalInputTypeDef:
    return {
        "project": ...,
    }


# SubscribedPrincipalInputTypeDef definition

class SubscribedPrincipalInputTypeDef(TypedDict):
    project: NotRequired[SubscribedProjectInputTypeDef],  # (1)
```

1. See [:material-code-braces: SubscribedProjectInputTypeDef](./type_defs.md#subscribedprojectinputtypedef) 
## SubscribedPrincipalTypeDef

```python
# SubscribedPrincipalTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedPrincipalTypeDef


def get_value() -> SubscribedPrincipalTypeDef:
    return {
        "project": ...,
    }


# SubscribedPrincipalTypeDef definition

class SubscribedPrincipalTypeDef(TypedDict):
    project: NotRequired[SubscribedProjectTypeDef],  # (1)
```

1. See [:material-code-braces: SubscribedProjectTypeDef](./type_defs.md#subscribedprojecttypedef) 
## CreateEnvironmentActionInputTypeDef

```python
# CreateEnvironmentActionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateEnvironmentActionInputTypeDef


def get_value() -> CreateEnvironmentActionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateEnvironmentActionInputTypeDef definition

class CreateEnvironmentActionInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    name: str,
    parameters: ActionParametersTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: ActionParametersTypeDef](./type_defs.md#actionparameterstypedef) 
## CreateEnvironmentActionOutputTypeDef

```python
# CreateEnvironmentActionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateEnvironmentActionOutputTypeDef


def get_value() -> CreateEnvironmentActionOutputTypeDef:
    return {
        "description": ...,
    }


# CreateEnvironmentActionOutputTypeDef definition

class CreateEnvironmentActionOutputTypeDef(TypedDict):
    description: str,
    domainId: str,
    environmentId: str,
    id: str,
    name: str,
    parameters: ActionParametersTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionParametersTypeDef](./type_defs.md#actionparameterstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentActionSummaryTypeDef

```python
# EnvironmentActionSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentActionSummaryTypeDef


def get_value() -> EnvironmentActionSummaryTypeDef:
    return {
        "description": ...,
    }


# EnvironmentActionSummaryTypeDef definition

class EnvironmentActionSummaryTypeDef(TypedDict):
    domainId: str,
    environmentId: str,
    id: str,
    name: str,
    parameters: ActionParametersTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: ActionParametersTypeDef](./type_defs.md#actionparameterstypedef) 
## GetEnvironmentActionOutputTypeDef

```python
# GetEnvironmentActionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentActionOutputTypeDef


def get_value() -> GetEnvironmentActionOutputTypeDef:
    return {
        "description": ...,
    }


# GetEnvironmentActionOutputTypeDef definition

class GetEnvironmentActionOutputTypeDef(TypedDict):
    description: str,
    domainId: str,
    environmentId: str,
    id: str,
    name: str,
    parameters: ActionParametersTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionParametersTypeDef](./type_defs.md#actionparameterstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentActionInputTypeDef

```python
# UpdateEnvironmentActionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateEnvironmentActionInputTypeDef


def get_value() -> UpdateEnvironmentActionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateEnvironmentActionInputTypeDef definition

class UpdateEnvironmentActionInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    name: NotRequired[str],
    parameters: NotRequired[ActionParametersTypeDef],  # (1)
```

1. See [:material-code-braces: ActionParametersTypeDef](./type_defs.md#actionparameterstypedef) 
## UpdateEnvironmentActionOutputTypeDef

```python
# UpdateEnvironmentActionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateEnvironmentActionOutputTypeDef


def get_value() -> UpdateEnvironmentActionOutputTypeDef:
    return {
        "description": ...,
    }


# UpdateEnvironmentActionOutputTypeDef definition

class UpdateEnvironmentActionOutputTypeDef(TypedDict):
    description: str,
    domainId: str,
    environmentId: str,
    id: str,
    name: str,
    parameters: ActionParametersTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ActionParametersTypeDef](./type_defs.md#actionparameterstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetItemTypeDef

```python
# AssetItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetItemTypeDef


def get_value() -> AssetItemTypeDef:
    return {
        "additionalAttributes": ...,
    }


# AssetItemTypeDef definition

class AssetItemTypeDef(TypedDict):
    domainId: str,
    identifier: str,
    name: str,
    owningProjectId: str,
    typeIdentifier: str,
    typeRevision: str,
    additionalAttributes: NotRequired[AssetItemAdditionalAttributesTypeDef],  # (1)
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    description: NotRequired[str],
    externalIdentifier: NotRequired[str],
    firstRevisionCreatedAt: NotRequired[datetime],
    firstRevisionCreatedBy: NotRequired[str],
    glossaryTerms: NotRequired[List[str]],
```

1. See [:material-code-braces: AssetItemAdditionalAttributesTypeDef](./type_defs.md#assetitemadditionalattributestypedef) 
## AssetListingItemTypeDef

```python
# AssetListingItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetListingItemTypeDef


def get_value() -> AssetListingItemTypeDef:
    return {
        "additionalAttributes": ...,
    }


# AssetListingItemTypeDef definition

class AssetListingItemTypeDef(TypedDict):
    additionalAttributes: NotRequired[AssetListingItemAdditionalAttributesTypeDef],  # (1)
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    entityId: NotRequired[str],
    entityRevision: NotRequired[str],
    entityType: NotRequired[str],
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (2)
    listingCreatedBy: NotRequired[str],
    listingId: NotRequired[str],
    listingRevision: NotRequired[str],
    listingUpdatedBy: NotRequired[str],
    name: NotRequired[str],
    owningProjectId: NotRequired[str],
```

1. See [:material-code-braces: AssetListingItemAdditionalAttributesTypeDef](./type_defs.md#assetlistingitemadditionalattributestypedef) 
2. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
## DataProductListingItemTypeDef

```python
# DataProductListingItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataProductListingItemTypeDef


def get_value() -> DataProductListingItemTypeDef:
    return {
        "additionalAttributes": ...,
    }


# DataProductListingItemTypeDef definition

class DataProductListingItemTypeDef(TypedDict):
    additionalAttributes: NotRequired[DataProductListingItemAdditionalAttributesTypeDef],  # (1)
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    entityId: NotRequired[str],
    entityRevision: NotRequired[str],
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (2)
    items: NotRequired[List[ListingSummaryItemTypeDef]],  # (3)
    listingCreatedBy: NotRequired[str],
    listingId: NotRequired[str],
    listingRevision: NotRequired[str],
    listingUpdatedBy: NotRequired[str],
    name: NotRequired[str],
    owningProjectId: NotRequired[str],
```

1. See [:material-code-braces: DataProductListingItemAdditionalAttributesTypeDef](./type_defs.md#dataproductlistingitemadditionalattributestypedef) 
2. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
3. See [:material-code-braces: ListingSummaryItemTypeDef](./type_defs.md#listingsummaryitemtypedef) 
## DataProductListingTypeDef

```python
# DataProductListingTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataProductListingTypeDef


def get_value() -> DataProductListingTypeDef:
    return {
        "createdAt": ...,
    }


# DataProductListingTypeDef definition

class DataProductListingTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    dataProductId: NotRequired[str],
    dataProductRevision: NotRequired[str],
    forms: NotRequired[str],
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (1)
    items: NotRequired[List[ListingSummaryTypeDef]],  # (2)
    owningProjectId: NotRequired[str],
```

1. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
2. See [:material-code-braces: ListingSummaryTypeDef](./type_defs.md#listingsummarytypedef) 
## SubscribedListingItemTypeDef

```python
# SubscribedListingItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedListingItemTypeDef


def get_value() -> SubscribedListingItemTypeDef:
    return {
        "assetListing": ...,
    }


# SubscribedListingItemTypeDef definition

class SubscribedListingItemTypeDef(TypedDict):
    assetListing: NotRequired[SubscribedAssetListingTypeDef],  # (1)
    productListing: NotRequired[SubscribedProductListingTypeDef],  # (2)
```

1. See [:material-code-braces: SubscribedAssetListingTypeDef](./type_defs.md#subscribedassetlistingtypedef) 
2. See [:material-code-braces: SubscribedProductListingTypeDef](./type_defs.md#subscribedproductlistingtypedef) 
## GlueConnectionPatchTypeDef

```python
# GlueConnectionPatchTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlueConnectionPatchTypeDef


def get_value() -> GlueConnectionPatchTypeDef:
    return {
        "authenticationConfiguration": ...,
    }


# GlueConnectionPatchTypeDef definition

class GlueConnectionPatchTypeDef(TypedDict):
    authenticationConfiguration: NotRequired[AuthenticationConfigurationPatchTypeDef],  # (1)
    connectionProperties: NotRequired[Mapping[str, str]],
    description: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationConfigurationPatchTypeDef](./type_defs.md#authenticationconfigurationpatchtypedef) 
## CreateAssetInputTypeDef

```python
# CreateAssetInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetInputTypeDef


def get_value() -> CreateAssetInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateAssetInputTypeDef definition

class CreateAssetInputTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    owningProjectIdentifier: str,
    typeIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    externalIdentifier: NotRequired[str],
    formsInput: NotRequired[Sequence[FormInputTypeDef]],  # (1)
    glossaryTerms: NotRequired[Sequence[str]],
    predictionConfiguration: NotRequired[PredictionConfigurationTypeDef],  # (2)
    typeRevision: NotRequired[str],
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: PredictionConfigurationTypeDef](./type_defs.md#predictionconfigurationtypedef) 
## CreateAssetOutputTypeDef

```python
# CreateAssetOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetOutputTypeDef


def get_value() -> CreateAssetOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CreateAssetOutputTypeDef definition

class CreateAssetOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    externalIdentifier: str,
    firstRevisionCreatedAt: datetime,
    firstRevisionCreatedBy: str,
    formsOutput: List[FormOutputTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    latestTimeSeriesDataPointFormsOutput: List[TimeSeriesDataPointSummaryFormOutputTypeDef],  # (2)
    listing: AssetListingDetailsTypeDef,  # (3)
    name: str,
    owningProjectId: str,
    predictionConfiguration: PredictionConfigurationTypeDef,  # (4)
    readOnlyFormsOutput: List[FormOutputTypeDef],  # (1)
    revision: str,
    typeIdentifier: str,
    typeRevision: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: TimeSeriesDataPointSummaryFormOutputTypeDef](./type_defs.md#timeseriesdatapointsummaryformoutputtypedef) 
3. See [:material-code-braces: AssetListingDetailsTypeDef](./type_defs.md#assetlistingdetailstypedef) 
4. See [:material-code-braces: PredictionConfigurationTypeDef](./type_defs.md#predictionconfigurationtypedef) 
5. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateAssetRevisionInputTypeDef

```python
# CreateAssetRevisionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetRevisionInputTypeDef


def get_value() -> CreateAssetRevisionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateAssetRevisionInputTypeDef definition

class CreateAssetRevisionInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    formsInput: NotRequired[Sequence[FormInputTypeDef]],  # (1)
    glossaryTerms: NotRequired[Sequence[str]],
    predictionConfiguration: NotRequired[PredictionConfigurationTypeDef],  # (2)
    typeRevision: NotRequired[str],
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: PredictionConfigurationTypeDef](./type_defs.md#predictionconfigurationtypedef) 
## CreateAssetRevisionOutputTypeDef

```python
# CreateAssetRevisionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetRevisionOutputTypeDef


def get_value() -> CreateAssetRevisionOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CreateAssetRevisionOutputTypeDef definition

class CreateAssetRevisionOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    externalIdentifier: str,
    firstRevisionCreatedAt: datetime,
    firstRevisionCreatedBy: str,
    formsOutput: List[FormOutputTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    latestTimeSeriesDataPointFormsOutput: List[TimeSeriesDataPointSummaryFormOutputTypeDef],  # (2)
    listing: AssetListingDetailsTypeDef,  # (3)
    name: str,
    owningProjectId: str,
    predictionConfiguration: PredictionConfigurationTypeDef,  # (4)
    readOnlyFormsOutput: List[FormOutputTypeDef],  # (1)
    revision: str,
    typeIdentifier: str,
    typeRevision: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: TimeSeriesDataPointSummaryFormOutputTypeDef](./type_defs.md#timeseriesdatapointsummaryformoutputtypedef) 
3. See [:material-code-braces: AssetListingDetailsTypeDef](./type_defs.md#assetlistingdetailstypedef) 
4. See [:material-code-braces: PredictionConfigurationTypeDef](./type_defs.md#predictionconfigurationtypedef) 
5. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentBlueprintSummaryTypeDef

```python
# EnvironmentBlueprintSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentBlueprintSummaryTypeDef


def get_value() -> EnvironmentBlueprintSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# EnvironmentBlueprintSummaryTypeDef definition

class EnvironmentBlueprintSummaryTypeDef(TypedDict):
    id: str,
    name: str,
    provider: str,
    provisioningProperties: ProvisioningPropertiesTypeDef,  # (1)
    createdAt: NotRequired[datetime],
    description: NotRequired[str],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: ProvisioningPropertiesTypeDef](./type_defs.md#provisioningpropertiestypedef) 
## GetEnvironmentBlueprintOutputTypeDef

```python
# GetEnvironmentBlueprintOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentBlueprintOutputTypeDef


def get_value() -> GetEnvironmentBlueprintOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetEnvironmentBlueprintOutputTypeDef definition

class GetEnvironmentBlueprintOutputTypeDef(TypedDict):
    createdAt: datetime,
    deploymentProperties: DeploymentPropertiesTypeDef,  # (1)
    description: str,
    glossaryTerms: List[str],
    id: str,
    name: str,
    provider: str,
    provisioningProperties: ProvisioningPropertiesTypeDef,  # (2)
    updatedAt: datetime,
    userParameters: List[CustomParameterTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: DeploymentPropertiesTypeDef](./type_defs.md#deploymentpropertiestypedef) 
2. See [:material-code-braces: ProvisioningPropertiesTypeDef](./type_defs.md#provisioningpropertiestypedef) 
3. See [:material-code-braces: CustomParameterTypeDef](./type_defs.md#customparametertypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSourcesOutputTypeDef

```python
# ListDataSourcesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourcesOutputTypeDef


def get_value() -> ListDataSourcesOutputTypeDef:
    return {
        "items": ...,
    }


# ListDataSourcesOutputTypeDef definition

class ListDataSourcesOutputTypeDef(TypedDict):
    items: List[DataSourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceSummaryTypeDef](./type_defs.md#datasourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectsOutputTypeDef

```python
# ListProjectsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectsOutputTypeDef


def get_value() -> ListProjectsOutputTypeDef:
    return {
        "items": ...,
    }


# ListProjectsOutputTypeDef definition

class ListProjectsOutputTypeDef(TypedDict):
    items: List[ProjectSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectSummaryTypeDef](./type_defs.md#projectsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscriptionTargetsOutputTypeDef

```python
# ListSubscriptionTargetsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionTargetsOutputTypeDef


def get_value() -> ListSubscriptionTargetsOutputTypeDef:
    return {
        "items": ...,
    }


# ListSubscriptionTargetsOutputTypeDef definition

class ListSubscriptionTargetsOutputTypeDef(TypedDict):
    items: List[SubscriptionTargetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTargetSummaryTypeDef](./type_defs.md#subscriptiontargetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateDataProductInputTypeDef

```python
# CreateDataProductInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDataProductInputTypeDef


def get_value() -> CreateDataProductInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateDataProductInputTypeDef definition

class CreateDataProductInputTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    owningProjectIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    formsInput: NotRequired[Sequence[FormInputTypeDef]],  # (1)
    glossaryTerms: NotRequired[Sequence[str]],
    items: NotRequired[Sequence[DataProductItemUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: DataProductItemTypeDef](./type_defs.md#dataproductitemtypedef) [:material-code-braces: DataProductItemOutputTypeDef](./type_defs.md#dataproductitemoutputtypedef) 
## CreateDataProductRevisionInputTypeDef

```python
# CreateDataProductRevisionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDataProductRevisionInputTypeDef


def get_value() -> CreateDataProductRevisionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateDataProductRevisionInputTypeDef definition

class CreateDataProductRevisionInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    formsInput: NotRequired[Sequence[FormInputTypeDef]],  # (1)
    glossaryTerms: NotRequired[Sequence[str]],
    items: NotRequired[Sequence[DataProductItemUnionTypeDef]],  # (2)
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: DataProductItemTypeDef](./type_defs.md#dataproductitemtypedef) [:material-code-braces: DataProductItemOutputTypeDef](./type_defs.md#dataproductitemoutputtypedef) 
## ListDataSourceRunActivitiesOutputTypeDef

```python
# ListDataSourceRunActivitiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourceRunActivitiesOutputTypeDef


def get_value() -> ListDataSourceRunActivitiesOutputTypeDef:
    return {
        "items": ...,
    }


# ListDataSourceRunActivitiesOutputTypeDef definition

class ListDataSourceRunActivitiesOutputTypeDef(TypedDict):
    items: List[DataSourceRunActivityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceRunActivityTypeDef](./type_defs.md#datasourcerunactivitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSourceRunsOutputTypeDef

```python
# ListDataSourceRunsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListDataSourceRunsOutputTypeDef


def get_value() -> ListDataSourceRunsOutputTypeDef:
    return {
        "items": ...,
    }


# ListDataSourceRunsOutputTypeDef definition

class ListDataSourceRunsOutputTypeDef(TypedDict):
    items: List[DataSourceRunSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceRunSummaryTypeDef](./type_defs.md#datasourcerunsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentOutputTypeDef

```python
# CreateEnvironmentOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateEnvironmentOutputTypeDef


def get_value() -> CreateEnvironmentOutputTypeDef:
    return {
        "awsAccountId": ...,
    }


# CreateEnvironmentOutputTypeDef definition

class CreateEnvironmentOutputTypeDef(TypedDict):
    awsAccountId: str,
    awsAccountRegion: str,
    createdAt: datetime,
    createdBy: str,
    deploymentProperties: DeploymentPropertiesTypeDef,  # (1)
    description: str,
    domainId: str,
    environmentActions: List[ConfigurableEnvironmentActionTypeDef],  # (2)
    environmentBlueprintId: str,
    environmentProfileId: str,
    glossaryTerms: List[str],
    id: str,
    lastDeployment: DeploymentTypeDef,  # (3)
    name: str,
    projectId: str,
    provider: str,
    provisionedResources: List[ResourceTypeDef],  # (4)
    provisioningProperties: ProvisioningPropertiesTypeDef,  # (5)
    status: EnvironmentStatusType,  # (6)
    updatedAt: datetime,
    userParameters: List[CustomParameterTypeDef],  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: DeploymentPropertiesTypeDef](./type_defs.md#deploymentpropertiestypedef) 
2. See [:material-code-braces: ConfigurableEnvironmentActionTypeDef](./type_defs.md#configurableenvironmentactiontypedef) 
3. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
4. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
5. See [:material-code-braces: ProvisioningPropertiesTypeDef](./type_defs.md#provisioningpropertiestypedef) 
6. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
7. See [:material-code-braces: CustomParameterTypeDef](./type_defs.md#customparametertypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentOutputTypeDef

```python
# GetEnvironmentOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentOutputTypeDef


def get_value() -> GetEnvironmentOutputTypeDef:
    return {
        "awsAccountId": ...,
    }


# GetEnvironmentOutputTypeDef definition

class GetEnvironmentOutputTypeDef(TypedDict):
    awsAccountId: str,
    awsAccountRegion: str,
    createdAt: datetime,
    createdBy: str,
    deploymentProperties: DeploymentPropertiesTypeDef,  # (1)
    description: str,
    domainId: str,
    environmentActions: List[ConfigurableEnvironmentActionTypeDef],  # (2)
    environmentBlueprintId: str,
    environmentProfileId: str,
    glossaryTerms: List[str],
    id: str,
    lastDeployment: DeploymentTypeDef,  # (3)
    name: str,
    projectId: str,
    provider: str,
    provisionedResources: List[ResourceTypeDef],  # (4)
    provisioningProperties: ProvisioningPropertiesTypeDef,  # (5)
    status: EnvironmentStatusType,  # (6)
    updatedAt: datetime,
    userParameters: List[CustomParameterTypeDef],  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: DeploymentPropertiesTypeDef](./type_defs.md#deploymentpropertiestypedef) 
2. See [:material-code-braces: ConfigurableEnvironmentActionTypeDef](./type_defs.md#configurableenvironmentactiontypedef) 
3. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
4. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
5. See [:material-code-braces: ProvisioningPropertiesTypeDef](./type_defs.md#provisioningpropertiestypedef) 
6. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
7. See [:material-code-braces: CustomParameterTypeDef](./type_defs.md#customparametertypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentOutputTypeDef

```python
# UpdateEnvironmentOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateEnvironmentOutputTypeDef


def get_value() -> UpdateEnvironmentOutputTypeDef:
    return {
        "awsAccountId": ...,
    }


# UpdateEnvironmentOutputTypeDef definition

class UpdateEnvironmentOutputTypeDef(TypedDict):
    awsAccountId: str,
    awsAccountRegion: str,
    createdAt: datetime,
    createdBy: str,
    deploymentProperties: DeploymentPropertiesTypeDef,  # (1)
    description: str,
    domainId: str,
    environmentActions: List[ConfigurableEnvironmentActionTypeDef],  # (2)
    environmentBlueprintId: str,
    environmentProfileId: str,
    glossaryTerms: List[str],
    id: str,
    lastDeployment: DeploymentTypeDef,  # (3)
    name: str,
    projectId: str,
    provider: str,
    provisionedResources: List[ResourceTypeDef],  # (4)
    provisioningProperties: ProvisioningPropertiesTypeDef,  # (5)
    status: EnvironmentStatusType,  # (6)
    updatedAt: datetime,
    userParameters: List[CustomParameterTypeDef],  # (7)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: DeploymentPropertiesTypeDef](./type_defs.md#deploymentpropertiestypedef) 
2. See [:material-code-braces: ConfigurableEnvironmentActionTypeDef](./type_defs.md#configurableenvironmentactiontypedef) 
3. See [:material-code-braces: DeploymentTypeDef](./type_defs.md#deploymenttypedef) 
4. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
5. See [:material-code-braces: ProvisioningPropertiesTypeDef](./type_defs.md#provisioningpropertiestypedef) 
6. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
7. See [:material-code-braces: CustomParameterTypeDef](./type_defs.md#customparametertypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectOutputTypeDef

```python
# CreateProjectOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateProjectOutputTypeDef


def get_value() -> CreateProjectOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CreateProjectOutputTypeDef definition

class CreateProjectOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentDeploymentDetails: EnvironmentDeploymentDetailsOutputTypeDef,  # (1)
    failureReasons: List[ProjectDeletionErrorTypeDef],  # (2)
    glossaryTerms: List[str],
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    projectProfileId: str,
    projectStatus: ProjectStatusType,  # (3)
    userParameters: List[EnvironmentConfigurationUserParameterOutputTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: EnvironmentDeploymentDetailsOutputTypeDef](./type_defs.md#environmentdeploymentdetailsoutputtypedef) 
2. See [:material-code-braces: ProjectDeletionErrorTypeDef](./type_defs.md#projectdeletionerrortypedef) 
3. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
4. See [:material-code-braces: EnvironmentConfigurationUserParameterOutputTypeDef](./type_defs.md#environmentconfigurationuserparameteroutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProjectOutputTypeDef

```python
# GetProjectOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetProjectOutputTypeDef


def get_value() -> GetProjectOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetProjectOutputTypeDef definition

class GetProjectOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentDeploymentDetails: EnvironmentDeploymentDetailsOutputTypeDef,  # (1)
    failureReasons: List[ProjectDeletionErrorTypeDef],  # (2)
    glossaryTerms: List[str],
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    projectProfileId: str,
    projectStatus: ProjectStatusType,  # (3)
    userParameters: List[EnvironmentConfigurationUserParameterOutputTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: EnvironmentDeploymentDetailsOutputTypeDef](./type_defs.md#environmentdeploymentdetailsoutputtypedef) 
2. See [:material-code-braces: ProjectDeletionErrorTypeDef](./type_defs.md#projectdeletionerrortypedef) 
3. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
4. See [:material-code-braces: EnvironmentConfigurationUserParameterOutputTypeDef](./type_defs.md#environmentconfigurationuserparameteroutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectOutputTypeDef

```python
# UpdateProjectOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateProjectOutputTypeDef


def get_value() -> UpdateProjectOutputTypeDef:
    return {
        "createdAt": ...,
    }


# UpdateProjectOutputTypeDef definition

class UpdateProjectOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentDeploymentDetails: EnvironmentDeploymentDetailsOutputTypeDef,  # (1)
    failureReasons: List[ProjectDeletionErrorTypeDef],  # (2)
    glossaryTerms: List[str],
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    projectProfileId: str,
    projectStatus: ProjectStatusType,  # (3)
    userParameters: List[EnvironmentConfigurationUserParameterOutputTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: EnvironmentDeploymentDetailsOutputTypeDef](./type_defs.md#environmentdeploymentdetailsoutputtypedef) 
2. See [:material-code-braces: ProjectDeletionErrorTypeDef](./type_defs.md#projectdeletionerrortypedef) 
3. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
4. See [:material-code-braces: EnvironmentConfigurationUserParameterOutputTypeDef](./type_defs.md#environmentconfigurationuserparameteroutputtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProjectPolicyGrantPrincipalTypeDef

```python
# ProjectPolicyGrantPrincipalTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProjectPolicyGrantPrincipalTypeDef


def get_value() -> ProjectPolicyGrantPrincipalTypeDef:
    return {
        "projectDesignation": ...,
    }


# ProjectPolicyGrantPrincipalTypeDef definition

class ProjectPolicyGrantPrincipalTypeDef(TypedDict):
    projectDesignation: ProjectDesignationType,  # (1)
    projectGrantFilter: NotRequired[ProjectGrantFilterTypeDef],  # (2)
    projectIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: ProjectDesignationType](./literals.md#projectdesignationtype) 
2. See [:material-code-braces: ProjectGrantFilterTypeDef](./type_defs.md#projectgrantfiltertypedef) 
## CreateDomainUnitOutputTypeDef

```python
# CreateDomainUnitOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDomainUnitOutputTypeDef


def get_value() -> CreateDomainUnitOutputTypeDef:
    return {
        "ancestorDomainUnitIds": ...,
    }


# CreateDomainUnitOutputTypeDef definition

class CreateDomainUnitOutputTypeDef(TypedDict):
    ancestorDomainUnitIds: List[str],
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    id: str,
    name: str,
    owners: List[DomainUnitOwnerPropertiesTypeDef],  # (1)
    parentDomainUnitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainUnitOwnerPropertiesTypeDef](./type_defs.md#domainunitownerpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainUnitOutputTypeDef

```python
# GetDomainUnitOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDomainUnitOutputTypeDef


def get_value() -> GetDomainUnitOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetDomainUnitOutputTypeDef definition

class GetDomainUnitOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    id: str,
    lastUpdatedAt: datetime,
    lastUpdatedBy: str,
    name: str,
    owners: List[DomainUnitOwnerPropertiesTypeDef],  # (1)
    parentDomainUnitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainUnitOwnerPropertiesTypeDef](./type_defs.md#domainunitownerpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainUnitOutputTypeDef

```python
# UpdateDomainUnitOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateDomainUnitOutputTypeDef


def get_value() -> UpdateDomainUnitOutputTypeDef:
    return {
        "createdAt": ...,
    }


# UpdateDomainUnitOutputTypeDef definition

class UpdateDomainUnitOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    id: str,
    lastUpdatedAt: datetime,
    lastUpdatedBy: str,
    name: str,
    owners: List[DomainUnitOwnerPropertiesTypeDef],  # (1)
    parentDomainUnitId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DomainUnitOwnerPropertiesTypeDef](./type_defs.md#domainunitownerpropertiestypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentConfigurationOutputTypeDef

```python
# EnvironmentConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationOutputTypeDef


def get_value() -> EnvironmentConfigurationOutputTypeDef:
    return {
        "awsAccount": ...,
    }


# EnvironmentConfigurationOutputTypeDef definition

class EnvironmentConfigurationOutputTypeDef(TypedDict):
    awsAccount: AwsAccountTypeDef,  # (1)
    awsRegion: RegionTypeDef,  # (2)
    environmentBlueprintId: str,
    name: str,
    configurationParameters: NotRequired[EnvironmentConfigurationParametersDetailsOutputTypeDef],  # (3)
    deploymentMode: NotRequired[DeploymentModeType],  # (4)
    deploymentOrder: NotRequired[int],
    description: NotRequired[str],
    id: NotRequired[str],
```

1. See [:material-code-braces: AwsAccountTypeDef](./type_defs.md#awsaccounttypedef) 
2. See [:material-code-braces: RegionTypeDef](./type_defs.md#regiontypedef) 
3. See [:material-code-braces: EnvironmentConfigurationParametersDetailsOutputTypeDef](./type_defs.md#environmentconfigurationparametersdetailsoutputtypedef) 
4. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
## SearchInputPaginateTypeDef

```python
# SearchInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchInputPaginateTypeDef


def get_value() -> SearchInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchInputPaginateTypeDef definition

class SearchInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    searchScope: InventorySearchScopeType,  # (1)
    additionalAttributes: NotRequired[Sequence[SearchOutputAdditionalAttributeType]],  # (2)
    filters: NotRequired[FilterClausePaginatorTypeDef],  # (3)
    owningProjectIdentifier: NotRequired[str],
    searchIn: NotRequired[Sequence[SearchInItemTypeDef]],  # (4)
    searchText: NotRequired[str],
    sort: NotRequired[SearchSortTypeDef],  # (5)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: InventorySearchScopeType](./literals.md#inventorysearchscopetype) 
2. See [:material-code-brackets: SearchOutputAdditionalAttributeType](./literals.md#searchoutputadditionalattributetype) 
3. See [:material-code-braces: FilterClausePaginatorTypeDef](./type_defs.md#filterclausepaginatortypedef) 
4. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
5. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchListingsInputPaginateTypeDef

```python
# SearchListingsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchListingsInputPaginateTypeDef


def get_value() -> SearchListingsInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchListingsInputPaginateTypeDef definition

class SearchListingsInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    additionalAttributes: NotRequired[Sequence[SearchOutputAdditionalAttributeType]],  # (1)
    filters: NotRequired[FilterClausePaginatorTypeDef],  # (2)
    searchIn: NotRequired[Sequence[SearchInItemTypeDef]],  # (3)
    searchText: NotRequired[str],
    sort: NotRequired[SearchSortTypeDef],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: SearchOutputAdditionalAttributeType](./literals.md#searchoutputadditionalattributetype) 
2. See [:material-code-braces: FilterClausePaginatorTypeDef](./type_defs.md#filterclausepaginatortypedef) 
3. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
4. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchTypesInputPaginateTypeDef

```python
# SearchTypesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchTypesInputPaginateTypeDef


def get_value() -> SearchTypesInputPaginateTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchTypesInputPaginateTypeDef definition

class SearchTypesInputPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    managed: bool,
    searchScope: TypesSearchScopeType,  # (1)
    filters: NotRequired[FilterClausePaginatorTypeDef],  # (2)
    searchIn: NotRequired[Sequence[SearchInItemTypeDef]],  # (3)
    searchText: NotRequired[str],
    sort: NotRequired[SearchSortTypeDef],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: TypesSearchScopeType](./literals.md#typessearchscopetype) 
2. See [:material-code-braces: FilterClausePaginatorTypeDef](./type_defs.md#filterclausepaginatortypedef) 
3. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
4. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchInputTypeDef

```python
# SearchInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchInputTypeDef


def get_value() -> SearchInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchInputTypeDef definition

class SearchInputTypeDef(TypedDict):
    domainIdentifier: str,
    searchScope: InventorySearchScopeType,  # (1)
    additionalAttributes: NotRequired[Sequence[SearchOutputAdditionalAttributeType]],  # (2)
    filters: NotRequired[FilterClauseTypeDef],  # (3)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    owningProjectIdentifier: NotRequired[str],
    searchIn: NotRequired[Sequence[SearchInItemTypeDef]],  # (4)
    searchText: NotRequired[str],
    sort: NotRequired[SearchSortTypeDef],  # (5)
```

1. See [:material-code-brackets: InventorySearchScopeType](./literals.md#inventorysearchscopetype) 
2. See [:material-code-brackets: SearchOutputAdditionalAttributeType](./literals.md#searchoutputadditionalattributetype) 
3. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
4. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
5. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
## SearchListingsInputTypeDef

```python
# SearchListingsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchListingsInputTypeDef


def get_value() -> SearchListingsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchListingsInputTypeDef definition

class SearchListingsInputTypeDef(TypedDict):
    domainIdentifier: str,
    additionalAttributes: NotRequired[Sequence[SearchOutputAdditionalAttributeType]],  # (1)
    filters: NotRequired[FilterClauseTypeDef],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    searchIn: NotRequired[Sequence[SearchInItemTypeDef]],  # (3)
    searchText: NotRequired[str],
    sort: NotRequired[SearchSortTypeDef],  # (4)
```

1. See [:material-code-brackets: SearchOutputAdditionalAttributeType](./literals.md#searchoutputadditionalattributetype) 
2. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
3. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
4. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
## SearchTypesInputTypeDef

```python
# SearchTypesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchTypesInputTypeDef


def get_value() -> SearchTypesInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# SearchTypesInputTypeDef definition

class SearchTypesInputTypeDef(TypedDict):
    domainIdentifier: str,
    managed: bool,
    searchScope: TypesSearchScopeType,  # (1)
    filters: NotRequired[FilterClauseTypeDef],  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    searchIn: NotRequired[Sequence[SearchInItemTypeDef]],  # (3)
    searchText: NotRequired[str],
    sort: NotRequired[SearchSortTypeDef],  # (4)
```

1. See [:material-code-brackets: TypesSearchScopeType](./literals.md#typessearchscopetype) 
2. See [:material-code-braces: FilterClauseTypeDef](./type_defs.md#filterclausetypedef) 
3. See [:material-code-braces: SearchInItemTypeDef](./type_defs.md#searchinitemtypedef) 
4. See [:material-code-braces: SearchSortTypeDef](./type_defs.md#searchsorttypedef) 
## GlueRunConfigurationOutputTypeDef

```python
# GlueRunConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlueRunConfigurationOutputTypeDef


def get_value() -> GlueRunConfigurationOutputTypeDef:
    return {
        "accountId": ...,
    }


# GlueRunConfigurationOutputTypeDef definition

class GlueRunConfigurationOutputTypeDef(TypedDict):
    relationalFilterConfigurations: List[RelationalFilterConfigurationOutputTypeDef],  # (1)
    accountId: NotRequired[str],
    autoImportDataQualityResult: NotRequired[bool],
    catalogName: NotRequired[str],
    dataAccessRole: NotRequired[str],
    region: NotRequired[str],
```

1. See [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 
## SearchTypesResultItemTypeDef

```python
# SearchTypesResultItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchTypesResultItemTypeDef


def get_value() -> SearchTypesResultItemTypeDef:
    return {
        "assetTypeItem": ...,
    }


# SearchTypesResultItemTypeDef definition

class SearchTypesResultItemTypeDef(TypedDict):
    assetTypeItem: NotRequired[AssetTypeItemTypeDef],  # (1)
    formTypeItem: NotRequired[FormTypeDataTypeDef],  # (2)
    lineageNodeTypeItem: NotRequired[LineageNodeTypeItemTypeDef],  # (3)
```

1. See [:material-code-braces: AssetTypeItemTypeDef](./type_defs.md#assettypeitemtypedef) 
2. See [:material-code-braces: FormTypeDataTypeDef](./type_defs.md#formtypedatatypedef) 
3. See [:material-code-braces: LineageNodeTypeItemTypeDef](./type_defs.md#lineagenodetypeitemtypedef) 
## ListJobRunsOutputTypeDef

```python
# ListJobRunsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListJobRunsOutputTypeDef


def get_value() -> ListJobRunsOutputTypeDef:
    return {
        "items": ...,
    }


# ListJobRunsOutputTypeDef definition

class ListJobRunsOutputTypeDef(TypedDict):
    items: List[JobRunSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: JobRunSummaryTypeDef](./type_defs.md#jobrunsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PostTimeSeriesDataPointsInputTypeDef

```python
# PostTimeSeriesDataPointsInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PostTimeSeriesDataPointsInputTypeDef


def get_value() -> PostTimeSeriesDataPointsInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# PostTimeSeriesDataPointsInputTypeDef definition

class PostTimeSeriesDataPointsInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    forms: Sequence[TimeSeriesDataPointFormInputTypeDef],  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
2. See [:material-code-braces: TimeSeriesDataPointFormInputTypeDef](./type_defs.md#timeseriesdatapointforminputtypedef) 
## ListMetadataGenerationRunsOutputTypeDef

```python
# ListMetadataGenerationRunsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListMetadataGenerationRunsOutputTypeDef


def get_value() -> ListMetadataGenerationRunsOutputTypeDef:
    return {
        "items": ...,
    }


# ListMetadataGenerationRunsOutputTypeDef definition

class ListMetadataGenerationRunsOutputTypeDef(TypedDict):
    items: List[MetadataGenerationRunItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: MetadataGenerationRunItemTypeDef](./type_defs.md#metadatagenerationrunitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SelfGrantStatusOutputTypeDef

```python
# SelfGrantStatusOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SelfGrantStatusOutputTypeDef


def get_value() -> SelfGrantStatusOutputTypeDef:
    return {
        "glueSelfGrantStatus": ...,
    }


# SelfGrantStatusOutputTypeDef definition

class SelfGrantStatusOutputTypeDef(TypedDict):
    glueSelfGrantStatus: NotRequired[GlueSelfGrantStatusOutputTypeDef],  # (1)
    redshiftSelfGrantStatus: NotRequired[RedshiftSelfGrantStatusOutputTypeDef],  # (2)
```

1. See [:material-code-braces: GlueSelfGrantStatusOutputTypeDef](./type_defs.md#glueselfgrantstatusoutputtypedef) 
2. See [:material-code-braces: RedshiftSelfGrantStatusOutputTypeDef](./type_defs.md#redshiftselfgrantstatusoutputtypedef) 
## CreateSubscriptionGrantInputTypeDef

```python
# CreateSubscriptionGrantInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateSubscriptionGrantInputTypeDef


def get_value() -> CreateSubscriptionGrantInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateSubscriptionGrantInputTypeDef definition

class CreateSubscriptionGrantInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    grantedEntity: GrantedEntityInputTypeDef,  # (1)
    assetTargetNames: NotRequired[Sequence[AssetTargetNameMapTypeDef]],  # (2)
    clientToken: NotRequired[str],
    subscriptionTargetIdentifier: NotRequired[str],
```

1. See [:material-code-braces: GrantedEntityInputTypeDef](./type_defs.md#grantedentityinputtypedef) 
2. See [:material-code-braces: AssetTargetNameMapTypeDef](./type_defs.md#assettargetnamemaptypedef) 
## CreateSubscriptionGrantOutputTypeDef

```python
# CreateSubscriptionGrantOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateSubscriptionGrantOutputTypeDef


def get_value() -> CreateSubscriptionGrantOutputTypeDef:
    return {
        "assets": ...,
    }


# CreateSubscriptionGrantOutputTypeDef definition

class CreateSubscriptionGrantOutputTypeDef(TypedDict):
    assets: List[SubscribedAssetTypeDef],  # (1)
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    grantedEntity: GrantedEntityTypeDef,  # (2)
    id: str,
    status: SubscriptionGrantOverallStatusType,  # (3)
    subscriptionId: str,
    subscriptionTargetId: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SubscribedAssetTypeDef](./type_defs.md#subscribedassettypedef) 
2. See [:material-code-braces: GrantedEntityTypeDef](./type_defs.md#grantedentitytypedef) 
3. See [:material-code-brackets: SubscriptionGrantOverallStatusType](./literals.md#subscriptiongrantoverallstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteSubscriptionGrantOutputTypeDef

```python
# DeleteSubscriptionGrantOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteSubscriptionGrantOutputTypeDef


def get_value() -> DeleteSubscriptionGrantOutputTypeDef:
    return {
        "assets": ...,
    }


# DeleteSubscriptionGrantOutputTypeDef definition

class DeleteSubscriptionGrantOutputTypeDef(TypedDict):
    assets: List[SubscribedAssetTypeDef],  # (1)
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    grantedEntity: GrantedEntityTypeDef,  # (2)
    id: str,
    status: SubscriptionGrantOverallStatusType,  # (3)
    subscriptionId: str,
    subscriptionTargetId: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SubscribedAssetTypeDef](./type_defs.md#subscribedassettypedef) 
2. See [:material-code-braces: GrantedEntityTypeDef](./type_defs.md#grantedentitytypedef) 
3. See [:material-code-brackets: SubscriptionGrantOverallStatusType](./literals.md#subscriptiongrantoverallstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionGrantOutputTypeDef

```python
# GetSubscriptionGrantOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetSubscriptionGrantOutputTypeDef


def get_value() -> GetSubscriptionGrantOutputTypeDef:
    return {
        "assets": ...,
    }


# GetSubscriptionGrantOutputTypeDef definition

class GetSubscriptionGrantOutputTypeDef(TypedDict):
    assets: List[SubscribedAssetTypeDef],  # (1)
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    grantedEntity: GrantedEntityTypeDef,  # (2)
    id: str,
    status: SubscriptionGrantOverallStatusType,  # (3)
    subscriptionId: str,
    subscriptionTargetId: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SubscribedAssetTypeDef](./type_defs.md#subscribedassettypedef) 
2. See [:material-code-braces: GrantedEntityTypeDef](./type_defs.md#grantedentitytypedef) 
3. See [:material-code-brackets: SubscriptionGrantOverallStatusType](./literals.md#subscriptiongrantoverallstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscriptionGrantSummaryTypeDef

```python
# SubscriptionGrantSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscriptionGrantSummaryTypeDef


def get_value() -> SubscriptionGrantSummaryTypeDef:
    return {
        "assets": ...,
    }


# SubscriptionGrantSummaryTypeDef definition

class SubscriptionGrantSummaryTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    grantedEntity: GrantedEntityTypeDef,  # (2)
    id: str,
    status: SubscriptionGrantOverallStatusType,  # (3)
    subscriptionTargetId: str,
    updatedAt: datetime,
    assets: NotRequired[List[SubscribedAssetTypeDef]],  # (1)
    subscriptionId: NotRequired[str],
    updatedBy: NotRequired[str],
```

1. See [:material-code-braces: SubscribedAssetTypeDef](./type_defs.md#subscribedassettypedef) 
2. See [:material-code-braces: GrantedEntityTypeDef](./type_defs.md#grantedentitytypedef) 
3. See [:material-code-brackets: SubscriptionGrantOverallStatusType](./literals.md#subscriptiongrantoverallstatustype) 
## UpdateSubscriptionGrantStatusOutputTypeDef

```python
# UpdateSubscriptionGrantStatusOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateSubscriptionGrantStatusOutputTypeDef


def get_value() -> UpdateSubscriptionGrantStatusOutputTypeDef:
    return {
        "assets": ...,
    }


# UpdateSubscriptionGrantStatusOutputTypeDef definition

class UpdateSubscriptionGrantStatusOutputTypeDef(TypedDict):
    assets: List[SubscribedAssetTypeDef],  # (1)
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    grantedEntity: GrantedEntityTypeDef,  # (2)
    id: str,
    status: SubscriptionGrantOverallStatusType,  # (3)
    subscriptionId: str,
    subscriptionTargetId: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: SubscribedAssetTypeDef](./type_defs.md#subscribedassettypedef) 
2. See [:material-code-braces: GrantedEntityTypeDef](./type_defs.md#grantedentitytypedef) 
3. See [:material-code-brackets: SubscriptionGrantOverallStatusType](./literals.md#subscriptiongrantoverallstatustype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentBlueprintConfigurationItemTypeDef

```python
# EnvironmentBlueprintConfigurationItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentBlueprintConfigurationItemTypeDef


def get_value() -> EnvironmentBlueprintConfigurationItemTypeDef:
    return {
        "createdAt": ...,
    }


# EnvironmentBlueprintConfigurationItemTypeDef definition

class EnvironmentBlueprintConfigurationItemTypeDef(TypedDict):
    domainId: str,
    environmentBlueprintId: str,
    createdAt: NotRequired[datetime],
    enabledRegions: NotRequired[List[str]],
    environmentRolePermissionBoundary: NotRequired[str],
    manageAccessRoleArn: NotRequired[str],
    provisioningConfigurations: NotRequired[List[ProvisioningConfigurationOutputTypeDef]],  # (1)
    provisioningRoleArn: NotRequired[str],
    regionalParameters: NotRequired[Dict[str, Dict[str, str]]],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: ProvisioningConfigurationOutputTypeDef](./type_defs.md#provisioningconfigurationoutputtypedef) 
## GetEnvironmentBlueprintConfigurationOutputTypeDef

```python
# GetEnvironmentBlueprintConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetEnvironmentBlueprintConfigurationOutputTypeDef


def get_value() -> GetEnvironmentBlueprintConfigurationOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetEnvironmentBlueprintConfigurationOutputTypeDef definition

class GetEnvironmentBlueprintConfigurationOutputTypeDef(TypedDict):
    createdAt: datetime,
    domainId: str,
    enabledRegions: List[str],
    environmentBlueprintId: str,
    environmentRolePermissionBoundary: str,
    manageAccessRoleArn: str,
    provisioningConfigurations: List[ProvisioningConfigurationOutputTypeDef],  # (1)
    provisioningRoleArn: str,
    regionalParameters: Dict[str, Dict[str, str]],
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisioningConfigurationOutputTypeDef](./type_defs.md#provisioningconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutEnvironmentBlueprintConfigurationOutputTypeDef

```python
# PutEnvironmentBlueprintConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PutEnvironmentBlueprintConfigurationOutputTypeDef


def get_value() -> PutEnvironmentBlueprintConfigurationOutputTypeDef:
    return {
        "createdAt": ...,
    }


# PutEnvironmentBlueprintConfigurationOutputTypeDef definition

class PutEnvironmentBlueprintConfigurationOutputTypeDef(TypedDict):
    createdAt: datetime,
    domainId: str,
    enabledRegions: List[str],
    environmentBlueprintId: str,
    environmentRolePermissionBoundary: str,
    manageAccessRoleArn: str,
    provisioningConfigurations: List[ProvisioningConfigurationOutputTypeDef],  # (1)
    provisioningRoleArn: str,
    regionalParameters: Dict[str, Dict[str, str]],
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisioningConfigurationOutputTypeDef](./type_defs.md#provisioningconfigurationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisioningConfigurationTypeDef

```python
# ProvisioningConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProvisioningConfigurationTypeDef


def get_value() -> ProvisioningConfigurationTypeDef:
    return {
        "lakeFormationConfiguration": ...,
    }


# ProvisioningConfigurationTypeDef definition

class ProvisioningConfigurationTypeDef(TypedDict):
    lakeFormationConfiguration: NotRequired[LakeFormationConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) [:material-code-braces: LakeFormationConfigurationOutputTypeDef](./type_defs.md#lakeformationconfigurationoutputtypedef) 
## JobRunDetailsTypeDef

```python
# JobRunDetailsTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import JobRunDetailsTypeDef


def get_value() -> JobRunDetailsTypeDef:
    return {
        "lineageRunDetails": ...,
    }


# JobRunDetailsTypeDef definition

class JobRunDetailsTypeDef(TypedDict):
    lineageRunDetails: NotRequired[LineageRunDetailsTypeDef],  # (1)
```

1. See [:material-code-braces: LineageRunDetailsTypeDef](./type_defs.md#lineagerundetailstypedef) 
## ProjectMemberTypeDef

```python
# ProjectMemberTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ProjectMemberTypeDef


def get_value() -> ProjectMemberTypeDef:
    return {
        "designation": ...,
    }


# ProjectMemberTypeDef definition

class ProjectMemberTypeDef(TypedDict):
    designation: UserDesignationType,  # (1)
    memberDetails: MemberDetailsTypeDef,  # (2)
```

1. See [:material-code-brackets: UserDesignationType](./literals.md#userdesignationtype) 
2. See [:material-code-braces: MemberDetailsTypeDef](./type_defs.md#memberdetailstypedef) 
## RuleDetailOutputTypeDef

```python
# RuleDetailOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RuleDetailOutputTypeDef


def get_value() -> RuleDetailOutputTypeDef:
    return {
        "metadataFormEnforcementDetail": ...,
    }


# RuleDetailOutputTypeDef definition

class RuleDetailOutputTypeDef(TypedDict):
    metadataFormEnforcementDetail: NotRequired[MetadataFormEnforcementDetailOutputTypeDef],  # (1)
```

1. See [:material-code-braces: MetadataFormEnforcementDetailOutputTypeDef](./type_defs.md#metadataformenforcementdetailoutputtypedef) 
## RuleDetailTypeDef

```python
# RuleDetailTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RuleDetailTypeDef


def get_value() -> RuleDetailTypeDef:
    return {
        "metadataFormEnforcementDetail": ...,
    }


# RuleDetailTypeDef definition

class RuleDetailTypeDef(TypedDict):
    metadataFormEnforcementDetail: NotRequired[MetadataFormEnforcementDetailTypeDef],  # (1)
```

1. See [:material-code-braces: MetadataFormEnforcementDetailTypeDef](./type_defs.md#metadataformenforcementdetailtypedef) 
## EventSummaryTypeDef

```python
# EventSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EventSummaryTypeDef


def get_value() -> EventSummaryTypeDef:
    return {
        "openLineageRunEventSummary": ...,
    }


# EventSummaryTypeDef definition

class EventSummaryTypeDef(TypedDict):
    openLineageRunEventSummary: NotRequired[OpenLineageRunEventSummaryTypeDef],  # (1)
```

1. See [:material-code-braces: OpenLineageRunEventSummaryTypeDef](./type_defs.md#openlineageruneventsummarytypedef) 
## RowFilterOutputTypeDef

```python
# RowFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RowFilterOutputTypeDef


def get_value() -> RowFilterOutputTypeDef:
    return {
        "and": ...,
    }


# RowFilterOutputTypeDef definition

class RowFilterOutputTypeDef(TypedDict):
    and: NotRequired[List[Dict[str, Any]]],
    expression: NotRequired[RowFilterExpressionOutputTypeDef],  # (1)
    or: NotRequired[List[Dict[str, Any]]],
```

1. See [:material-code-braces: RowFilterExpressionOutputTypeDef](./type_defs.md#rowfilterexpressionoutputtypedef) 
## RowFilterTypeDef

```python
# RowFilterTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RowFilterTypeDef


def get_value() -> RowFilterTypeDef:
    return {
        "and": ...,
    }


# RowFilterTypeDef definition

class RowFilterTypeDef(TypedDict):
    and: NotRequired[Sequence[Mapping[str, Any]]],
    expression: NotRequired[RowFilterExpressionTypeDef],  # (1)
    or: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: RowFilterExpressionTypeDef](./type_defs.md#rowfilterexpressiontypedef) 
## NotificationOutputTypeDef

```python
# NotificationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import NotificationOutputTypeDef


def get_value() -> NotificationOutputTypeDef:
    return {
        "actionLink": ...,
    }


# NotificationOutputTypeDef definition

class NotificationOutputTypeDef(TypedDict):
    actionLink: str,
    creationTimestamp: datetime,
    domainIdentifier: str,
    identifier: str,
    lastUpdatedTimestamp: datetime,
    message: str,
    title: str,
    topic: TopicTypeDef,  # (2)
    type: NotificationTypeType,  # (3)
    metadata: NotRequired[Dict[str, str]],
    status: NotRequired[TaskStatusType],  # (1)
```

1. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
2. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 
3. See [:material-code-brackets: NotificationTypeType](./literals.md#notificationtypetype) 
## AuthenticationConfigurationTypeDef

```python
# AuthenticationConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AuthenticationConfigurationTypeDef


def get_value() -> AuthenticationConfigurationTypeDef:
    return {
        "authenticationType": ...,
    }


# AuthenticationConfigurationTypeDef definition

class AuthenticationConfigurationTypeDef(TypedDict):
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    oAuth2Properties: NotRequired[OAuth2PropertiesOutputTypeDef],  # (2)
    secretArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: OAuth2PropertiesOutputTypeDef](./type_defs.md#oauth2propertiesoutputtypedef) 
## ListEntityOwnersOutputTypeDef

```python
# ListEntityOwnersOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEntityOwnersOutputTypeDef


def get_value() -> ListEntityOwnersOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListEntityOwnersOutputTypeDef definition

class ListEntityOwnersOutputTypeDef(TypedDict):
    owners: List[OwnerPropertiesOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OwnerPropertiesOutputTypeDef](./type_defs.md#ownerpropertiesoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddEntityOwnerInputTypeDef

```python
# AddEntityOwnerInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AddEntityOwnerInputTypeDef


def get_value() -> AddEntityOwnerInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# AddEntityOwnerInputTypeDef definition

class AddEntityOwnerInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: DataZoneEntityTypeType,  # (1)
    owner: OwnerPropertiesTypeDef,  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: DataZoneEntityTypeType](./literals.md#datazoneentitytypetype) 
2. See [:material-code-braces: OwnerPropertiesTypeDef](./type_defs.md#ownerpropertiestypedef) 
## RemoveEntityOwnerInputTypeDef

```python
# RemoveEntityOwnerInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RemoveEntityOwnerInputTypeDef


def get_value() -> RemoveEntityOwnerInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# RemoveEntityOwnerInputTypeDef definition

class RemoveEntityOwnerInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: DataZoneEntityTypeType,  # (1)
    owner: OwnerPropertiesTypeDef,  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: DataZoneEntityTypeType](./literals.md#datazoneentitytypetype) 
2. See [:material-code-braces: OwnerPropertiesTypeDef](./type_defs.md#ownerpropertiestypedef) 
## RuleSummaryTypeDef

```python
# RuleSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RuleSummaryTypeDef


def get_value() -> RuleSummaryTypeDef:
    return {
        "action": ...,
    }


# RuleSummaryTypeDef definition

class RuleSummaryTypeDef(TypedDict):
    action: NotRequired[RuleActionType],  # (1)
    identifier: NotRequired[str],
    lastUpdatedBy: NotRequired[str],
    name: NotRequired[str],
    revision: NotRequired[str],
    ruleType: NotRequired[RuleTypeType],  # (2)
    scope: NotRequired[RuleScopeOutputTypeDef],  # (3)
    target: NotRequired[RuleTargetTypeDef],  # (4)
    targetType: NotRequired[RuleTargetTypeType],  # (5)
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-brackets: RuleActionType](./literals.md#ruleactiontype) 
2. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
3. See [:material-code-braces: RuleScopeOutputTypeDef](./type_defs.md#rulescopeoutputtypedef) 
4. See [:material-code-braces: RuleTargetTypeDef](./type_defs.md#ruletargettypedef) 
5. See [:material-code-brackets: RuleTargetTypeType](./literals.md#ruletargettypetype) 
## RedshiftPropertiesInputTypeDef

```python
# RedshiftPropertiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftPropertiesInputTypeDef


def get_value() -> RedshiftPropertiesInputTypeDef:
    return {
        "credentials": ...,
    }


# RedshiftPropertiesInputTypeDef definition

class RedshiftPropertiesInputTypeDef(TypedDict):
    credentials: NotRequired[RedshiftCredentialsTypeDef],  # (1)
    databaseName: NotRequired[str],
    host: NotRequired[str],
    lineageSync: NotRequired[RedshiftLineageSyncConfigurationInputTypeDef],  # (2)
    port: NotRequired[int],
    storage: NotRequired[RedshiftStoragePropertiesTypeDef],  # (3)
```

1. See [:material-code-braces: RedshiftCredentialsTypeDef](./type_defs.md#redshiftcredentialstypedef) 
2. See [:material-code-braces: RedshiftLineageSyncConfigurationInputTypeDef](./type_defs.md#redshiftlineagesyncconfigurationinputtypedef) 
3. See [:material-code-braces: RedshiftStoragePropertiesTypeDef](./type_defs.md#redshiftstoragepropertiestypedef) 
## RedshiftPropertiesOutputTypeDef

```python
# RedshiftPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftPropertiesOutputTypeDef


def get_value() -> RedshiftPropertiesOutputTypeDef:
    return {
        "credentials": ...,
    }


# RedshiftPropertiesOutputTypeDef definition

class RedshiftPropertiesOutputTypeDef(TypedDict):
    credentials: NotRequired[RedshiftCredentialsTypeDef],  # (1)
    databaseName: NotRequired[str],
    isProvisionedSecret: NotRequired[bool],
    jdbcIamUrl: NotRequired[str],
    jdbcUrl: NotRequired[str],
    lineageSync: NotRequired[RedshiftLineageSyncConfigurationOutputTypeDef],  # (2)
    redshiftTempDir: NotRequired[str],
    status: NotRequired[ConnectionStatusType],  # (3)
    storage: NotRequired[RedshiftStoragePropertiesTypeDef],  # (4)
```

1. See [:material-code-braces: RedshiftCredentialsTypeDef](./type_defs.md#redshiftcredentialstypedef) 
2. See [:material-code-braces: RedshiftLineageSyncConfigurationOutputTypeDef](./type_defs.md#redshiftlineagesyncconfigurationoutputtypedef) 
3. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
4. See [:material-code-braces: RedshiftStoragePropertiesTypeDef](./type_defs.md#redshiftstoragepropertiestypedef) 
## RedshiftPropertiesPatchTypeDef

```python
# RedshiftPropertiesPatchTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftPropertiesPatchTypeDef


def get_value() -> RedshiftPropertiesPatchTypeDef:
    return {
        "credentials": ...,
    }


# RedshiftPropertiesPatchTypeDef definition

class RedshiftPropertiesPatchTypeDef(TypedDict):
    credentials: NotRequired[RedshiftCredentialsTypeDef],  # (1)
    databaseName: NotRequired[str],
    host: NotRequired[str],
    lineageSync: NotRequired[RedshiftLineageSyncConfigurationInputTypeDef],  # (2)
    port: NotRequired[int],
    storage: NotRequired[RedshiftStoragePropertiesTypeDef],  # (3)
```

1. See [:material-code-braces: RedshiftCredentialsTypeDef](./type_defs.md#redshiftcredentialstypedef) 
2. See [:material-code-braces: RedshiftLineageSyncConfigurationInputTypeDef](./type_defs.md#redshiftlineagesyncconfigurationinputtypedef) 
3. See [:material-code-braces: RedshiftStoragePropertiesTypeDef](./type_defs.md#redshiftstoragepropertiestypedef) 
## RedshiftRunConfigurationOutputTypeDef

```python
# RedshiftRunConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftRunConfigurationOutputTypeDef


def get_value() -> RedshiftRunConfigurationOutputTypeDef:
    return {
        "accountId": ...,
    }


# RedshiftRunConfigurationOutputTypeDef definition

class RedshiftRunConfigurationOutputTypeDef(TypedDict):
    redshiftStorage: RedshiftStorageTypeDef,  # (2)
    relationalFilterConfigurations: List[RelationalFilterConfigurationOutputTypeDef],  # (3)
    accountId: NotRequired[str],
    dataAccessRole: NotRequired[str],
    redshiftCredentialConfiguration: NotRequired[RedshiftCredentialConfigurationTypeDef],  # (1)
    region: NotRequired[str],
```

1. See [:material-code-braces: RedshiftCredentialConfigurationTypeDef](./type_defs.md#redshiftcredentialconfigurationtypedef) 
2. See [:material-code-braces: RedshiftStorageTypeDef](./type_defs.md#redshiftstoragetypedef) 
3. See [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 
## CreateUserProfileOutputTypeDef

```python
# CreateUserProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateUserProfileOutputTypeDef


def get_value() -> CreateUserProfileOutputTypeDef:
    return {
        "details": ...,
    }


# CreateUserProfileOutputTypeDef definition

class CreateUserProfileOutputTypeDef(TypedDict):
    details: UserProfileDetailsTypeDef,  # (1)
    domainId: str,
    id: str,
    status: UserProfileStatusType,  # (2)
    type: UserProfileTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: UserProfileDetailsTypeDef](./type_defs.md#userprofiledetailstypedef) 
2. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
3. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetUserProfileOutputTypeDef

```python
# GetUserProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetUserProfileOutputTypeDef


def get_value() -> GetUserProfileOutputTypeDef:
    return {
        "details": ...,
    }


# GetUserProfileOutputTypeDef definition

class GetUserProfileOutputTypeDef(TypedDict):
    details: UserProfileDetailsTypeDef,  # (1)
    domainId: str,
    id: str,
    status: UserProfileStatusType,  # (2)
    type: UserProfileTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: UserProfileDetailsTypeDef](./type_defs.md#userprofiledetailstypedef) 
2. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
3. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateUserProfileOutputTypeDef

```python
# UpdateUserProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateUserProfileOutputTypeDef


def get_value() -> UpdateUserProfileOutputTypeDef:
    return {
        "details": ...,
    }


# UpdateUserProfileOutputTypeDef definition

class UpdateUserProfileOutputTypeDef(TypedDict):
    details: UserProfileDetailsTypeDef,  # (1)
    domainId: str,
    id: str,
    status: UserProfileStatusType,  # (2)
    type: UserProfileTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: UserProfileDetailsTypeDef](./type_defs.md#userprofiledetailstypedef) 
2. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
3. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UserProfileSummaryTypeDef

```python
# UserProfileSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UserProfileSummaryTypeDef


def get_value() -> UserProfileSummaryTypeDef:
    return {
        "details": ...,
    }


# UserProfileSummaryTypeDef definition

class UserProfileSummaryTypeDef(TypedDict):
    details: NotRequired[UserProfileDetailsTypeDef],  # (1)
    domainId: NotRequired[str],
    id: NotRequired[str],
    status: NotRequired[UserProfileStatusType],  # (2)
    type: NotRequired[UserProfileTypeType],  # (3)
```

1. See [:material-code-braces: UserProfileDetailsTypeDef](./type_defs.md#userprofiledetailstypedef) 
2. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
3. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
## CreateSubscriptionRequestInputTypeDef

```python
# CreateSubscriptionRequestInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateSubscriptionRequestInputTypeDef


def get_value() -> CreateSubscriptionRequestInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateSubscriptionRequestInputTypeDef definition

class CreateSubscriptionRequestInputTypeDef(TypedDict):
    domainIdentifier: str,
    requestReason: str,
    subscribedListings: Sequence[SubscribedListingInputTypeDef],  # (1)
    subscribedPrincipals: Sequence[SubscribedPrincipalInputTypeDef],  # (2)
    clientToken: NotRequired[str],
    metadataForms: NotRequired[Sequence[FormInputTypeDef]],  # (3)
```

1. See [:material-code-braces: SubscribedListingInputTypeDef](./type_defs.md#subscribedlistinginputtypedef) 
2. See [:material-code-braces: SubscribedPrincipalInputTypeDef](./type_defs.md#subscribedprincipalinputtypedef) 
3. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
## CreateGlossaryTermInputTypeDef

```python
# CreateGlossaryTermInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateGlossaryTermInputTypeDef


def get_value() -> CreateGlossaryTermInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateGlossaryTermInputTypeDef definition

class CreateGlossaryTermInputTypeDef(TypedDict):
    domainIdentifier: str,
    glossaryIdentifier: str,
    name: str,
    clientToken: NotRequired[str],
    longDescription: NotRequired[str],
    shortDescription: NotRequired[str],
    status: NotRequired[GlossaryTermStatusType],  # (1)
    termRelations: NotRequired[TermRelationsUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsTypeDef](./type_defs.md#termrelationstypedef) [:material-code-braces: TermRelationsOutputTypeDef](./type_defs.md#termrelationsoutputtypedef) 
## UpdateGlossaryTermInputTypeDef

```python
# UpdateGlossaryTermInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateGlossaryTermInputTypeDef


def get_value() -> UpdateGlossaryTermInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateGlossaryTermInputTypeDef definition

class UpdateGlossaryTermInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    glossaryIdentifier: NotRequired[str],
    longDescription: NotRequired[str],
    name: NotRequired[str],
    shortDescription: NotRequired[str],
    status: NotRequired[GlossaryTermStatusType],  # (1)
    termRelations: NotRequired[TermRelationsUnionTypeDef],  # (2)
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsTypeDef](./type_defs.md#termrelationstypedef) [:material-code-braces: TermRelationsOutputTypeDef](./type_defs.md#termrelationsoutputtypedef) 
## ListEnvironmentActionsOutputTypeDef

```python
# ListEnvironmentActionsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentActionsOutputTypeDef


def get_value() -> ListEnvironmentActionsOutputTypeDef:
    return {
        "items": ...,
    }


# ListEnvironmentActionsOutputTypeDef definition

class ListEnvironmentActionsOutputTypeDef(TypedDict):
    items: List[EnvironmentActionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentActionSummaryTypeDef](./type_defs.md#environmentactionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchInventoryResultItemTypeDef

```python
# SearchInventoryResultItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchInventoryResultItemTypeDef


def get_value() -> SearchInventoryResultItemTypeDef:
    return {
        "assetItem": ...,
    }


# SearchInventoryResultItemTypeDef definition

class SearchInventoryResultItemTypeDef(TypedDict):
    assetItem: NotRequired[AssetItemTypeDef],  # (1)
    dataProductItem: NotRequired[DataProductResultItemTypeDef],  # (2)
    glossaryItem: NotRequired[GlossaryItemTypeDef],  # (3)
    glossaryTermItem: NotRequired[GlossaryTermItemTypeDef],  # (4)
```

1. See [:material-code-braces: AssetItemTypeDef](./type_defs.md#assetitemtypedef) 
2. See [:material-code-braces: DataProductResultItemTypeDef](./type_defs.md#dataproductresultitemtypedef) 
3. See [:material-code-braces: GlossaryItemTypeDef](./type_defs.md#glossaryitemtypedef) 
4. See [:material-code-braces: GlossaryTermItemTypeDef](./type_defs.md#glossarytermitemtypedef) 
## SearchResultItemTypeDef

```python
# SearchResultItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchResultItemTypeDef


def get_value() -> SearchResultItemTypeDef:
    return {
        "assetListing": ...,
    }


# SearchResultItemTypeDef definition

class SearchResultItemTypeDef(TypedDict):
    assetListing: NotRequired[AssetListingItemTypeDef],  # (1)
    dataProductListing: NotRequired[DataProductListingItemTypeDef],  # (2)
```

1. See [:material-code-braces: AssetListingItemTypeDef](./type_defs.md#assetlistingitemtypedef) 
2. See [:material-code-braces: DataProductListingItemTypeDef](./type_defs.md#dataproductlistingitemtypedef) 
## ListingItemTypeDef

```python
# ListingItemTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListingItemTypeDef


def get_value() -> ListingItemTypeDef:
    return {
        "assetListing": ...,
    }


# ListingItemTypeDef definition

class ListingItemTypeDef(TypedDict):
    assetListing: NotRequired[AssetListingTypeDef],  # (1)
    dataProductListing: NotRequired[DataProductListingTypeDef],  # (2)
```

1. See [:material-code-braces: AssetListingTypeDef](./type_defs.md#assetlistingtypedef) 
2. See [:material-code-braces: DataProductListingTypeDef](./type_defs.md#dataproductlistingtypedef) 
## SubscribedListingTypeDef

```python
# SubscribedListingTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscribedListingTypeDef


def get_value() -> SubscribedListingTypeDef:
    return {
        "description": ...,
    }


# SubscribedListingTypeDef definition

class SubscribedListingTypeDef(TypedDict):
    description: str,
    id: str,
    item: SubscribedListingItemTypeDef,  # (1)
    name: str,
    ownerProjectId: str,
    ownerProjectName: NotRequired[str],
    revision: NotRequired[str],
```

1. See [:material-code-braces: SubscribedListingItemTypeDef](./type_defs.md#subscribedlistingitemtypedef) 
## GluePropertiesPatchTypeDef

```python
# GluePropertiesPatchTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GluePropertiesPatchTypeDef


def get_value() -> GluePropertiesPatchTypeDef:
    return {
        "glueConnectionInput": ...,
    }


# GluePropertiesPatchTypeDef definition

class GluePropertiesPatchTypeDef(TypedDict):
    glueConnectionInput: NotRequired[GlueConnectionPatchTypeDef],  # (1)
```

1. See [:material-code-braces: GlueConnectionPatchTypeDef](./type_defs.md#glueconnectionpatchtypedef) 
## ListEnvironmentBlueprintsOutputTypeDef

```python
# ListEnvironmentBlueprintsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentBlueprintsOutputTypeDef


def get_value() -> ListEnvironmentBlueprintsOutputTypeDef:
    return {
        "items": ...,
    }


# ListEnvironmentBlueprintsOutputTypeDef definition

class ListEnvironmentBlueprintsOutputTypeDef(TypedDict):
    items: List[EnvironmentBlueprintSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentBlueprintSummaryTypeDef](./type_defs.md#environmentblueprintsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProjectInputTypeDef

```python
# CreateProjectInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateProjectInputTypeDef


def get_value() -> CreateProjectInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateProjectInputTypeDef definition

class CreateProjectInputTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    description: NotRequired[str],
    domainUnitId: NotRequired[str],
    glossaryTerms: NotRequired[Sequence[str]],
    projectProfileId: NotRequired[str],
    userParameters: NotRequired[Sequence[EnvironmentConfigurationUserParameterUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: EnvironmentConfigurationUserParameterTypeDef](./type_defs.md#environmentconfigurationuserparametertypedef) [:material-code-braces: EnvironmentConfigurationUserParameterOutputTypeDef](./type_defs.md#environmentconfigurationuserparameteroutputtypedef) 
## UpdateProjectInputTypeDef

```python
# UpdateProjectInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateProjectInputTypeDef


def get_value() -> UpdateProjectInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateProjectInputTypeDef definition

class UpdateProjectInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    environmentDeploymentDetails: NotRequired[EnvironmentDeploymentDetailsUnionTypeDef],  # (1)
    glossaryTerms: NotRequired[Sequence[str]],
    name: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentDeploymentDetailsTypeDef](./type_defs.md#environmentdeploymentdetailstypedef) [:material-code-braces: EnvironmentDeploymentDetailsOutputTypeDef](./type_defs.md#environmentdeploymentdetailsoutputtypedef) 
## PolicyGrantPrincipalOutputTypeDef

```python
# PolicyGrantPrincipalOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PolicyGrantPrincipalOutputTypeDef


def get_value() -> PolicyGrantPrincipalOutputTypeDef:
    return {
        "domainUnit": ...,
    }


# PolicyGrantPrincipalOutputTypeDef definition

class PolicyGrantPrincipalOutputTypeDef(TypedDict):
    domainUnit: NotRequired[DomainUnitPolicyGrantPrincipalOutputTypeDef],  # (1)
    group: NotRequired[GroupPolicyGrantPrincipalTypeDef],  # (2)
    project: NotRequired[ProjectPolicyGrantPrincipalTypeDef],  # (3)
    user: NotRequired[UserPolicyGrantPrincipalOutputTypeDef],  # (4)
```

1. See [:material-code-braces: DomainUnitPolicyGrantPrincipalOutputTypeDef](./type_defs.md#domainunitpolicygrantprincipaloutputtypedef) 
2. See [:material-code-braces: GroupPolicyGrantPrincipalTypeDef](./type_defs.md#grouppolicygrantprincipaltypedef) 
3. See [:material-code-braces: ProjectPolicyGrantPrincipalTypeDef](./type_defs.md#projectpolicygrantprincipaltypedef) 
4. See [:material-code-braces: UserPolicyGrantPrincipalOutputTypeDef](./type_defs.md#userpolicygrantprincipaloutputtypedef) 
## PolicyGrantPrincipalTypeDef

```python
# PolicyGrantPrincipalTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PolicyGrantPrincipalTypeDef


def get_value() -> PolicyGrantPrincipalTypeDef:
    return {
        "domainUnit": ...,
    }


# PolicyGrantPrincipalTypeDef definition

class PolicyGrantPrincipalTypeDef(TypedDict):
    domainUnit: NotRequired[DomainUnitPolicyGrantPrincipalTypeDef],  # (1)
    group: NotRequired[GroupPolicyGrantPrincipalTypeDef],  # (2)
    project: NotRequired[ProjectPolicyGrantPrincipalTypeDef],  # (3)
    user: NotRequired[UserPolicyGrantPrincipalTypeDef],  # (4)
```

1. See [:material-code-braces: DomainUnitPolicyGrantPrincipalTypeDef](./type_defs.md#domainunitpolicygrantprincipaltypedef) 
2. See [:material-code-braces: GroupPolicyGrantPrincipalTypeDef](./type_defs.md#grouppolicygrantprincipaltypedef) 
3. See [:material-code-braces: ProjectPolicyGrantPrincipalTypeDef](./type_defs.md#projectpolicygrantprincipaltypedef) 
4. See [:material-code-braces: UserPolicyGrantPrincipalTypeDef](./type_defs.md#userpolicygrantprincipaltypedef) 
## CreateProjectProfileOutputTypeDef

```python
# CreateProjectProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateProjectProfileOutputTypeDef


def get_value() -> CreateProjectProfileOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CreateProjectProfileOutputTypeDef definition

class CreateProjectProfileOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentConfigurations: List[EnvironmentConfigurationOutputTypeDef],  # (1)
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EnvironmentConfigurationOutputTypeDef](./type_defs.md#environmentconfigurationoutputtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProjectProfileOutputTypeDef

```python
# GetProjectProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetProjectProfileOutputTypeDef


def get_value() -> GetProjectProfileOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetProjectProfileOutputTypeDef definition

class GetProjectProfileOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentConfigurations: List[EnvironmentConfigurationOutputTypeDef],  # (1)
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EnvironmentConfigurationOutputTypeDef](./type_defs.md#environmentconfigurationoutputtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProjectProfileOutputTypeDef

```python
# UpdateProjectProfileOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateProjectProfileOutputTypeDef


def get_value() -> UpdateProjectProfileOutputTypeDef:
    return {
        "createdAt": ...,
    }


# UpdateProjectProfileOutputTypeDef definition

class UpdateProjectProfileOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentConfigurations: List[EnvironmentConfigurationOutputTypeDef],  # (1)
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: EnvironmentConfigurationOutputTypeDef](./type_defs.md#environmentconfigurationoutputtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnvironmentConfigurationTypeDef

```python
# EnvironmentConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import EnvironmentConfigurationTypeDef


def get_value() -> EnvironmentConfigurationTypeDef:
    return {
        "awsAccount": ...,
    }


# EnvironmentConfigurationTypeDef definition

class EnvironmentConfigurationTypeDef(TypedDict):
    awsAccount: AwsAccountTypeDef,  # (1)
    awsRegion: RegionTypeDef,  # (2)
    environmentBlueprintId: str,
    name: str,
    configurationParameters: NotRequired[EnvironmentConfigurationParametersDetailsUnionTypeDef],  # (3)
    deploymentMode: NotRequired[DeploymentModeType],  # (4)
    deploymentOrder: NotRequired[int],
    description: NotRequired[str],
    id: NotRequired[str],
```

1. See [:material-code-braces: AwsAccountTypeDef](./type_defs.md#awsaccounttypedef) 
2. See [:material-code-braces: RegionTypeDef](./type_defs.md#regiontypedef) 
3. See [:material-code-braces: EnvironmentConfigurationParametersDetailsTypeDef](./type_defs.md#environmentconfigurationparametersdetailstypedef) [:material-code-braces: EnvironmentConfigurationParametersDetailsOutputTypeDef](./type_defs.md#environmentconfigurationparametersdetailsoutputtypedef) 
4. See [:material-code-brackets: DeploymentModeType](./literals.md#deploymentmodetype) 
## GlueRunConfigurationInputTypeDef

```python
# GlueRunConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlueRunConfigurationInputTypeDef


def get_value() -> GlueRunConfigurationInputTypeDef:
    return {
        "autoImportDataQualityResult": ...,
    }


# GlueRunConfigurationInputTypeDef definition

class GlueRunConfigurationInputTypeDef(TypedDict):
    relationalFilterConfigurations: Sequence[RelationalFilterConfigurationUnionTypeDef],  # (1)
    autoImportDataQualityResult: NotRequired[bool],
    catalogName: NotRequired[str],
    dataAccessRole: NotRequired[str],
```

1. See [:material-code-braces: RelationalFilterConfigurationTypeDef](./type_defs.md#relationalfilterconfigurationtypedef) [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 
## RedshiftRunConfigurationInputTypeDef

```python
# RedshiftRunConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RedshiftRunConfigurationInputTypeDef


def get_value() -> RedshiftRunConfigurationInputTypeDef:
    return {
        "dataAccessRole": ...,
    }


# RedshiftRunConfigurationInputTypeDef definition

class RedshiftRunConfigurationInputTypeDef(TypedDict):
    relationalFilterConfigurations: Sequence[RelationalFilterConfigurationUnionTypeDef],  # (3)
    dataAccessRole: NotRequired[str],
    redshiftCredentialConfiguration: NotRequired[RedshiftCredentialConfigurationTypeDef],  # (1)
    redshiftStorage: NotRequired[RedshiftStorageTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftCredentialConfigurationTypeDef](./type_defs.md#redshiftcredentialconfigurationtypedef) 
2. See [:material-code-braces: RedshiftStorageTypeDef](./type_defs.md#redshiftstoragetypedef) 
3. See [:material-code-braces: RelationalFilterConfigurationTypeDef](./type_defs.md#relationalfilterconfigurationtypedef) [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 
## SearchTypesOutputTypeDef

```python
# SearchTypesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchTypesOutputTypeDef


def get_value() -> SearchTypesOutputTypeDef:
    return {
        "items": ...,
    }


# SearchTypesOutputTypeDef definition

class SearchTypesOutputTypeDef(TypedDict):
    items: List[SearchTypesResultItemTypeDef],  # (1)
    totalMatchCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchTypesResultItemTypeDef](./type_defs.md#searchtypesresultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscriptionGrantsOutputTypeDef

```python
# ListSubscriptionGrantsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionGrantsOutputTypeDef


def get_value() -> ListSubscriptionGrantsOutputTypeDef:
    return {
        "items": ...,
    }


# ListSubscriptionGrantsOutputTypeDef definition

class ListSubscriptionGrantsOutputTypeDef(TypedDict):
    items: List[SubscriptionGrantSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionGrantSummaryTypeDef](./type_defs.md#subscriptiongrantsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentBlueprintConfigurationsOutputTypeDef

```python
# ListEnvironmentBlueprintConfigurationsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListEnvironmentBlueprintConfigurationsOutputTypeDef


def get_value() -> ListEnvironmentBlueprintConfigurationsOutputTypeDef:
    return {
        "items": ...,
    }


# ListEnvironmentBlueprintConfigurationsOutputTypeDef definition

class ListEnvironmentBlueprintConfigurationsOutputTypeDef(TypedDict):
    items: List[EnvironmentBlueprintConfigurationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentBlueprintConfigurationItemTypeDef](./type_defs.md#environmentblueprintconfigurationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetJobRunOutputTypeDef

```python
# GetJobRunOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetJobRunOutputTypeDef


def get_value() -> GetJobRunOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetJobRunOutputTypeDef definition

class GetJobRunOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    details: JobRunDetailsTypeDef,  # (1)
    domainId: str,
    endTime: datetime,
    error: JobRunErrorTypeDef,  # (2)
    id: str,
    jobId: str,
    jobType: JobTypeType,  # (3)
    runMode: JobRunModeType,  # (4)
    startTime: datetime,
    status: JobRunStatusType,  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: JobRunDetailsTypeDef](./type_defs.md#jobrundetailstypedef) 
2. See [:material-code-braces: JobRunErrorTypeDef](./type_defs.md#jobrunerrortypedef) 
3. See [:material-code-brackets: JobTypeType](./literals.md#jobtypetype) 
4. See [:material-code-brackets: JobRunModeType](./literals.md#jobrunmodetype) 
5. See [:material-code-brackets: JobRunStatusType](./literals.md#jobrunstatustype) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectMembershipsOutputTypeDef

```python
# ListProjectMembershipsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListProjectMembershipsOutputTypeDef


def get_value() -> ListProjectMembershipsOutputTypeDef:
    return {
        "members": ...,
    }


# ListProjectMembershipsOutputTypeDef definition

class ListProjectMembershipsOutputTypeDef(TypedDict):
    members: List[ProjectMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectMemberTypeDef](./type_defs.md#projectmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRuleOutputTypeDef

```python
# CreateRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateRuleOutputTypeDef


def get_value() -> CreateRuleOutputTypeDef:
    return {
        "action": ...,
    }


# CreateRuleOutputTypeDef definition

class CreateRuleOutputTypeDef(TypedDict):
    action: RuleActionType,  # (1)
    createdAt: datetime,
    createdBy: str,
    description: str,
    detail: RuleDetailOutputTypeDef,  # (2)
    identifier: str,
    name: str,
    ruleType: RuleTypeType,  # (3)
    scope: RuleScopeOutputTypeDef,  # (4)
    target: RuleTargetTypeDef,  # (5)
    targetType: RuleTargetTypeType,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: RuleActionType](./literals.md#ruleactiontype) 
2. See [:material-code-braces: RuleDetailOutputTypeDef](./type_defs.md#ruledetailoutputtypedef) 
3. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
4. See [:material-code-braces: RuleScopeOutputTypeDef](./type_defs.md#rulescopeoutputtypedef) 
5. See [:material-code-braces: RuleTargetTypeDef](./type_defs.md#ruletargettypedef) 
6. See [:material-code-brackets: RuleTargetTypeType](./literals.md#ruletargettypetype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRuleOutputTypeDef

```python
# GetRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetRuleOutputTypeDef


def get_value() -> GetRuleOutputTypeDef:
    return {
        "action": ...,
    }


# GetRuleOutputTypeDef definition

class GetRuleOutputTypeDef(TypedDict):
    action: RuleActionType,  # (1)
    createdAt: datetime,
    createdBy: str,
    description: str,
    detail: RuleDetailOutputTypeDef,  # (2)
    identifier: str,
    lastUpdatedBy: str,
    name: str,
    revision: str,
    ruleType: RuleTypeType,  # (3)
    scope: RuleScopeOutputTypeDef,  # (4)
    target: RuleTargetTypeDef,  # (5)
    targetType: RuleTargetTypeType,  # (6)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-brackets: RuleActionType](./literals.md#ruleactiontype) 
2. See [:material-code-braces: RuleDetailOutputTypeDef](./type_defs.md#ruledetailoutputtypedef) 
3. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
4. See [:material-code-braces: RuleScopeOutputTypeDef](./type_defs.md#rulescopeoutputtypedef) 
5. See [:material-code-braces: RuleTargetTypeDef](./type_defs.md#ruletargettypedef) 
6. See [:material-code-brackets: RuleTargetTypeType](./literals.md#ruletargettypetype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRuleOutputTypeDef

```python
# UpdateRuleOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateRuleOutputTypeDef


def get_value() -> UpdateRuleOutputTypeDef:
    return {
        "action": ...,
    }


# UpdateRuleOutputTypeDef definition

class UpdateRuleOutputTypeDef(TypedDict):
    action: RuleActionType,  # (1)
    createdAt: datetime,
    createdBy: str,
    description: str,
    detail: RuleDetailOutputTypeDef,  # (2)
    identifier: str,
    lastUpdatedBy: str,
    name: str,
    revision: str,
    ruleType: RuleTypeType,  # (3)
    scope: RuleScopeOutputTypeDef,  # (4)
    target: RuleTargetTypeDef,  # (5)
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-brackets: RuleActionType](./literals.md#ruleactiontype) 
2. See [:material-code-braces: RuleDetailOutputTypeDef](./type_defs.md#ruledetailoutputtypedef) 
3. See [:material-code-brackets: RuleTypeType](./literals.md#ruletypetype) 
4. See [:material-code-braces: RuleScopeOutputTypeDef](./type_defs.md#rulescopeoutputtypedef) 
5. See [:material-code-braces: RuleTargetTypeDef](./type_defs.md#ruletargettypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LineageEventSummaryTypeDef

```python
# LineageEventSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import LineageEventSummaryTypeDef


def get_value() -> LineageEventSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# LineageEventSummaryTypeDef definition

class LineageEventSummaryTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    domainId: NotRequired[str],
    eventSummary: NotRequired[EventSummaryTypeDef],  # (1)
    eventTime: NotRequired[datetime],
    id: NotRequired[str],
    processingStatus: NotRequired[LineageEventProcessingStatusType],  # (2)
```

1. See [:material-code-braces: EventSummaryTypeDef](./type_defs.md#eventsummarytypedef) 
2. See [:material-code-brackets: LineageEventProcessingStatusType](./literals.md#lineageeventprocessingstatustype) 
## RowFilterConfigurationOutputTypeDef

```python
# RowFilterConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RowFilterConfigurationOutputTypeDef


def get_value() -> RowFilterConfigurationOutputTypeDef:
    return {
        "rowFilter": ...,
    }


# RowFilterConfigurationOutputTypeDef definition

class RowFilterConfigurationOutputTypeDef(TypedDict):
    rowFilter: RowFilterOutputTypeDef,  # (1)
    sensitive: NotRequired[bool],
```

1. See [:material-code-braces: RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef) 
## RowFilterConfigurationTypeDef

```python
# RowFilterConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RowFilterConfigurationTypeDef


def get_value() -> RowFilterConfigurationTypeDef:
    return {
        "rowFilter": ...,
    }


# RowFilterConfigurationTypeDef definition

class RowFilterConfigurationTypeDef(TypedDict):
    rowFilter: RowFilterTypeDef,  # (1)
    sensitive: NotRequired[bool],
```

1. See [:material-code-braces: RowFilterTypeDef](./type_defs.md#rowfiltertypedef) 
## ListNotificationsOutputTypeDef

```python
# ListNotificationsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListNotificationsOutputTypeDef


def get_value() -> ListNotificationsOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListNotificationsOutputTypeDef definition

class ListNotificationsOutputTypeDef(TypedDict):
    notifications: List[NotificationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationOutputTypeDef](./type_defs.md#notificationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GlueConnectionTypeDef

```python
# GlueConnectionTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlueConnectionTypeDef


def get_value() -> GlueConnectionTypeDef:
    return {
        "athenaProperties": ...,
    }


# GlueConnectionTypeDef definition

class GlueConnectionTypeDef(TypedDict):
    athenaProperties: NotRequired[Dict[str, str]],
    authenticationConfiguration: NotRequired[AuthenticationConfigurationTypeDef],  # (1)
    compatibleComputeEnvironments: NotRequired[List[ComputeEnvironmentsType]],  # (2)
    connectionProperties: NotRequired[Dict[str, str]],
    connectionSchemaVersion: NotRequired[int],
    connectionType: NotRequired[ConnectionTypeType],  # (3)
    creationTime: NotRequired[datetime],
    description: NotRequired[str],
    lastConnectionValidationTime: NotRequired[datetime],
    lastUpdatedBy: NotRequired[str],
    lastUpdatedTime: NotRequired[datetime],
    matchCriteria: NotRequired[List[str]],
    name: NotRequired[str],
    physicalConnectionRequirements: NotRequired[PhysicalConnectionRequirementsOutputTypeDef],  # (4)
    pythonProperties: NotRequired[Dict[str, str]],
    sparkProperties: NotRequired[Dict[str, str]],
    status: NotRequired[ConnectionStatusType],  # (5)
    statusReason: NotRequired[str],
```

1. See [:material-code-braces: AuthenticationConfigurationTypeDef](./type_defs.md#authenticationconfigurationtypedef) 
2. See [:material-code-brackets: ComputeEnvironmentsType](./literals.md#computeenvironmentstype) 
3. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
4. See [:material-code-braces: PhysicalConnectionRequirementsOutputTypeDef](./type_defs.md#physicalconnectionrequirementsoutputtypedef) 
5. See [:material-code-brackets: ConnectionStatusType](./literals.md#connectionstatustype) 
## AuthenticationConfigurationInputTypeDef

```python
# AuthenticationConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AuthenticationConfigurationInputTypeDef


def get_value() -> AuthenticationConfigurationInputTypeDef:
    return {
        "authenticationType": ...,
    }


# AuthenticationConfigurationInputTypeDef definition

class AuthenticationConfigurationInputTypeDef(TypedDict):
    authenticationType: NotRequired[AuthenticationTypeType],  # (1)
    basicAuthenticationCredentials: NotRequired[BasicAuthenticationCredentialsTypeDef],  # (2)
    customAuthenticationCredentials: NotRequired[Mapping[str, str]],
    kmsKeyArn: NotRequired[str],
    oAuth2Properties: NotRequired[OAuth2PropertiesUnionTypeDef],  # (3)
    secretArn: NotRequired[str],
```

1. See [:material-code-brackets: AuthenticationTypeType](./literals.md#authenticationtypetype) 
2. See [:material-code-braces: BasicAuthenticationCredentialsTypeDef](./type_defs.md#basicauthenticationcredentialstypedef) 
3. See [:material-code-braces: OAuth2PropertiesTypeDef](./type_defs.md#oauth2propertiestypedef) [:material-code-braces: OAuth2PropertiesOutputTypeDef](./type_defs.md#oauth2propertiesoutputtypedef) 
## ListRulesOutputTypeDef

```python
# ListRulesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListRulesOutputTypeDef


def get_value() -> ListRulesOutputTypeDef:
    return {
        "items": ...,
    }


# ListRulesOutputTypeDef definition

class ListRulesOutputTypeDef(TypedDict):
    items: List[RuleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RuleSummaryTypeDef](./type_defs.md#rulesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionPropertiesOutputTypeDef

```python
# ConnectionPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ConnectionPropertiesOutputTypeDef


def get_value() -> ConnectionPropertiesOutputTypeDef:
    return {
        "athenaProperties": ...,
    }


# ConnectionPropertiesOutputTypeDef definition

class ConnectionPropertiesOutputTypeDef(TypedDict):
    athenaProperties: NotRequired[AthenaPropertiesOutputTypeDef],  # (1)
    glueProperties: NotRequired[GluePropertiesOutputTypeDef],  # (2)
    hyperPodProperties: NotRequired[HyperPodPropertiesOutputTypeDef],  # (3)
    iamProperties: NotRequired[IamPropertiesOutputTypeDef],  # (4)
    redshiftProperties: NotRequired[RedshiftPropertiesOutputTypeDef],  # (5)
    sparkEmrProperties: NotRequired[SparkEmrPropertiesOutputTypeDef],  # (6)
    sparkGlueProperties: NotRequired[SparkGluePropertiesOutputTypeDef],  # (7)
```

1. See [:material-code-braces: AthenaPropertiesOutputTypeDef](./type_defs.md#athenapropertiesoutputtypedef) 
2. See [:material-code-braces: GluePropertiesOutputTypeDef](./type_defs.md#gluepropertiesoutputtypedef) 
3. See [:material-code-braces: HyperPodPropertiesOutputTypeDef](./type_defs.md#hyperpodpropertiesoutputtypedef) 
4. See [:material-code-braces: IamPropertiesOutputTypeDef](./type_defs.md#iampropertiesoutputtypedef) 
5. See [:material-code-braces: RedshiftPropertiesOutputTypeDef](./type_defs.md#redshiftpropertiesoutputtypedef) 
6. See [:material-code-braces: SparkEmrPropertiesOutputTypeDef](./type_defs.md#sparkemrpropertiesoutputtypedef) 
7. See [:material-code-braces: SparkGluePropertiesOutputTypeDef](./type_defs.md#sparkgluepropertiesoutputtypedef) 
## DataSourceConfigurationOutputTypeDef

```python
# DataSourceConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataSourceConfigurationOutputTypeDef


def get_value() -> DataSourceConfigurationOutputTypeDef:
    return {
        "glueRunConfiguration": ...,
    }


# DataSourceConfigurationOutputTypeDef definition

class DataSourceConfigurationOutputTypeDef(TypedDict):
    glueRunConfiguration: NotRequired[GlueRunConfigurationOutputTypeDef],  # (1)
    redshiftRunConfiguration: NotRequired[RedshiftRunConfigurationOutputTypeDef],  # (2)
    sageMakerRunConfiguration: NotRequired[SageMakerRunConfigurationOutputTypeDef],  # (3)
```

1. See [:material-code-braces: GlueRunConfigurationOutputTypeDef](./type_defs.md#gluerunconfigurationoutputtypedef) 
2. See [:material-code-braces: RedshiftRunConfigurationOutputTypeDef](./type_defs.md#redshiftrunconfigurationoutputtypedef) 
3. See [:material-code-braces: SageMakerRunConfigurationOutputTypeDef](./type_defs.md#sagemakerrunconfigurationoutputtypedef) 
## SearchUserProfilesOutputTypeDef

```python
# SearchUserProfilesOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchUserProfilesOutputTypeDef


def get_value() -> SearchUserProfilesOutputTypeDef:
    return {
        "items": ...,
    }


# SearchUserProfilesOutputTypeDef definition

class SearchUserProfilesOutputTypeDef(TypedDict):
    items: List[UserProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: UserProfileSummaryTypeDef](./type_defs.md#userprofilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchOutputTypeDef

```python
# SearchOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchOutputTypeDef


def get_value() -> SearchOutputTypeDef:
    return {
        "items": ...,
    }


# SearchOutputTypeDef definition

class SearchOutputTypeDef(TypedDict):
    items: List[SearchInventoryResultItemTypeDef],  # (1)
    totalMatchCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchInventoryResultItemTypeDef](./type_defs.md#searchinventoryresultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchListingsOutputTypeDef

```python
# SearchListingsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SearchListingsOutputTypeDef


def get_value() -> SearchListingsOutputTypeDef:
    return {
        "items": ...,
    }


# SearchListingsOutputTypeDef definition

class SearchListingsOutputTypeDef(TypedDict):
    items: List[SearchResultItemTypeDef],  # (1)
    totalMatchCount: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SearchResultItemTypeDef](./type_defs.md#searchresultitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetListingOutputTypeDef

```python
# GetListingOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetListingOutputTypeDef


def get_value() -> GetListingOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetListingOutputTypeDef definition

class GetListingOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    id: str,
    item: ListingItemTypeDef,  # (1)
    listingRevision: str,
    name: str,
    status: ListingStatusType,  # (2)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ListingItemTypeDef](./type_defs.md#listingitemtypedef) 
2. See [:material-code-brackets: ListingStatusType](./literals.md#listingstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcceptSubscriptionRequestOutputTypeDef

```python
# AcceptSubscriptionRequestOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AcceptSubscriptionRequestOutputTypeDef


def get_value() -> AcceptSubscriptionRequestOutputTypeDef:
    return {
        "createdAt": ...,
    }


# AcceptSubscriptionRequestOutputTypeDef definition

class AcceptSubscriptionRequestOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    existingSubscriptionId: str,
    id: str,
    metadataForms: List[FormOutputTypeDef],  # (1)
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (2)
    subscribedListings: List[SubscribedListingTypeDef],  # (3)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (4)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
3. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
4. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelSubscriptionOutputTypeDef

```python
# CancelSubscriptionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CancelSubscriptionOutputTypeDef


def get_value() -> CancelSubscriptionOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CancelSubscriptionOutputTypeDef definition

class CancelSubscriptionOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    id: str,
    retainPermissions: bool,
    status: SubscriptionStatusType,  # (1)
    subscribedListing: SubscribedListingTypeDef,  # (2)
    subscribedPrincipal: SubscribedPrincipalTypeDef,  # (3)
    subscriptionRequestId: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSubscriptionRequestOutputTypeDef

```python
# CreateSubscriptionRequestOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateSubscriptionRequestOutputTypeDef


def get_value() -> CreateSubscriptionRequestOutputTypeDef:
    return {
        "createdAt": ...,
    }


# CreateSubscriptionRequestOutputTypeDef definition

class CreateSubscriptionRequestOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    existingSubscriptionId: str,
    id: str,
    metadataForms: List[FormOutputTypeDef],  # (1)
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (2)
    subscribedListings: List[SubscribedListingTypeDef],  # (3)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (4)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
3. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
4. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionOutputTypeDef

```python
# GetSubscriptionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetSubscriptionOutputTypeDef


def get_value() -> GetSubscriptionOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetSubscriptionOutputTypeDef definition

class GetSubscriptionOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    id: str,
    retainPermissions: bool,
    status: SubscriptionStatusType,  # (1)
    subscribedListing: SubscribedListingTypeDef,  # (2)
    subscribedPrincipal: SubscribedPrincipalTypeDef,  # (3)
    subscriptionRequestId: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionRequestDetailsOutputTypeDef

```python
# GetSubscriptionRequestDetailsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetSubscriptionRequestDetailsOutputTypeDef


def get_value() -> GetSubscriptionRequestDetailsOutputTypeDef:
    return {
        "createdAt": ...,
    }


# GetSubscriptionRequestDetailsOutputTypeDef definition

class GetSubscriptionRequestDetailsOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    existingSubscriptionId: str,
    id: str,
    metadataForms: List[FormOutputTypeDef],  # (1)
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (2)
    subscribedListings: List[SubscribedListingTypeDef],  # (3)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (4)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
3. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
4. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectSubscriptionRequestOutputTypeDef

```python
# RejectSubscriptionRequestOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RejectSubscriptionRequestOutputTypeDef


def get_value() -> RejectSubscriptionRequestOutputTypeDef:
    return {
        "createdAt": ...,
    }


# RejectSubscriptionRequestOutputTypeDef definition

class RejectSubscriptionRequestOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    existingSubscriptionId: str,
    id: str,
    metadataForms: List[FormOutputTypeDef],  # (1)
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (2)
    subscribedListings: List[SubscribedListingTypeDef],  # (3)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (4)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
3. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
4. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RevokeSubscriptionOutputTypeDef

```python
# RevokeSubscriptionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RevokeSubscriptionOutputTypeDef


def get_value() -> RevokeSubscriptionOutputTypeDef:
    return {
        "createdAt": ...,
    }


# RevokeSubscriptionOutputTypeDef definition

class RevokeSubscriptionOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    id: str,
    retainPermissions: bool,
    status: SubscriptionStatusType,  # (1)
    subscribedListing: SubscribedListingTypeDef,  # (2)
    subscribedPrincipal: SubscribedPrincipalTypeDef,  # (3)
    subscriptionRequestId: str,
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscriptionRequestSummaryTypeDef

```python
# SubscriptionRequestSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscriptionRequestSummaryTypeDef


def get_value() -> SubscriptionRequestSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# SubscriptionRequestSummaryTypeDef definition

class SubscriptionRequestSummaryTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    id: str,
    requestReason: str,
    status: SubscriptionRequestStatusType,  # (2)
    subscribedListings: List[SubscribedListingTypeDef],  # (3)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (4)
    updatedAt: datetime,
    decisionComment: NotRequired[str],
    existingSubscriptionId: NotRequired[str],
    metadataFormsSummary: NotRequired[List[MetadataFormSummaryTypeDef]],  # (1)
    reviewerId: NotRequired[str],
    updatedBy: NotRequired[str],
```

1. See [:material-code-braces: MetadataFormSummaryTypeDef](./type_defs.md#metadataformsummarytypedef) 
2. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
3. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
4. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
## SubscriptionSummaryTypeDef

```python
# SubscriptionSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import SubscriptionSummaryTypeDef


def get_value() -> SubscriptionSummaryTypeDef:
    return {
        "createdAt": ...,
    }


# SubscriptionSummaryTypeDef definition

class SubscriptionSummaryTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    id: str,
    status: SubscriptionStatusType,  # (1)
    subscribedListing: SubscribedListingTypeDef,  # (2)
    subscribedPrincipal: SubscribedPrincipalTypeDef,  # (3)
    updatedAt: datetime,
    retainPermissions: NotRequired[bool],
    subscriptionRequestId: NotRequired[str],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: SubscriptionStatusType](./literals.md#subscriptionstatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
## UpdateSubscriptionRequestOutputTypeDef

```python
# UpdateSubscriptionRequestOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateSubscriptionRequestOutputTypeDef


def get_value() -> UpdateSubscriptionRequestOutputTypeDef:
    return {
        "createdAt": ...,
    }


# UpdateSubscriptionRequestOutputTypeDef definition

class UpdateSubscriptionRequestOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    existingSubscriptionId: str,
    id: str,
    metadataForms: List[FormOutputTypeDef],  # (1)
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (2)
    subscribedListings: List[SubscribedListingTypeDef],  # (3)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (4)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
3. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
4. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionPropertiesPatchTypeDef

```python
# ConnectionPropertiesPatchTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ConnectionPropertiesPatchTypeDef


def get_value() -> ConnectionPropertiesPatchTypeDef:
    return {
        "athenaProperties": ...,
    }


# ConnectionPropertiesPatchTypeDef definition

class ConnectionPropertiesPatchTypeDef(TypedDict):
    athenaProperties: NotRequired[AthenaPropertiesPatchTypeDef],  # (1)
    glueProperties: NotRequired[GluePropertiesPatchTypeDef],  # (2)
    iamProperties: NotRequired[IamPropertiesPatchTypeDef],  # (3)
    redshiftProperties: NotRequired[RedshiftPropertiesPatchTypeDef],  # (4)
    sparkEmrProperties: NotRequired[SparkEmrPropertiesPatchTypeDef],  # (5)
```

1. See [:material-code-braces: AthenaPropertiesPatchTypeDef](./type_defs.md#athenapropertiespatchtypedef) 
2. See [:material-code-braces: GluePropertiesPatchTypeDef](./type_defs.md#gluepropertiespatchtypedef) 
3. See [:material-code-braces: IamPropertiesPatchTypeDef](./type_defs.md#iampropertiespatchtypedef) 
4. See [:material-code-braces: RedshiftPropertiesPatchTypeDef](./type_defs.md#redshiftpropertiespatchtypedef) 
5. See [:material-code-braces: SparkEmrPropertiesPatchTypeDef](./type_defs.md#sparkemrpropertiespatchtypedef) 
## PolicyGrantMemberTypeDef

```python
# PolicyGrantMemberTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PolicyGrantMemberTypeDef


def get_value() -> PolicyGrantMemberTypeDef:
    return {
        "createdAt": ...,
    }


# PolicyGrantMemberTypeDef definition

class PolicyGrantMemberTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    detail: NotRequired[PolicyGrantDetailOutputTypeDef],  # (1)
    principal: NotRequired[PolicyGrantPrincipalOutputTypeDef],  # (2)
```

1. See [:material-code-braces: PolicyGrantDetailOutputTypeDef](./type_defs.md#policygrantdetailoutputtypedef) 
2. See [:material-code-braces: PolicyGrantPrincipalOutputTypeDef](./type_defs.md#policygrantprincipaloutputtypedef) 
## DataSourceConfigurationInputTypeDef

```python
# DataSourceConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DataSourceConfigurationInputTypeDef


def get_value() -> DataSourceConfigurationInputTypeDef:
    return {
        "glueRunConfiguration": ...,
    }


# DataSourceConfigurationInputTypeDef definition

class DataSourceConfigurationInputTypeDef(TypedDict):
    glueRunConfiguration: NotRequired[GlueRunConfigurationInputTypeDef],  # (1)
    redshiftRunConfiguration: NotRequired[RedshiftRunConfigurationInputTypeDef],  # (2)
    sageMakerRunConfiguration: NotRequired[SageMakerRunConfigurationInputTypeDef],  # (3)
```

1. See [:material-code-braces: GlueRunConfigurationInputTypeDef](./type_defs.md#gluerunconfigurationinputtypedef) 
2. See [:material-code-braces: RedshiftRunConfigurationInputTypeDef](./type_defs.md#redshiftrunconfigurationinputtypedef) 
3. See [:material-code-braces: SageMakerRunConfigurationInputTypeDef](./type_defs.md#sagemakerrunconfigurationinputtypedef) 
## PutEnvironmentBlueprintConfigurationInputTypeDef

```python
# PutEnvironmentBlueprintConfigurationInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PutEnvironmentBlueprintConfigurationInputTypeDef


def get_value() -> PutEnvironmentBlueprintConfigurationInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# PutEnvironmentBlueprintConfigurationInputTypeDef definition

class PutEnvironmentBlueprintConfigurationInputTypeDef(TypedDict):
    domainIdentifier: str,
    enabledRegions: Sequence[str],
    environmentBlueprintIdentifier: str,
    environmentRolePermissionBoundary: NotRequired[str],
    manageAccessRoleArn: NotRequired[str],
    provisioningConfigurations: NotRequired[Sequence[ProvisioningConfigurationUnionTypeDef]],  # (1)
    provisioningRoleArn: NotRequired[str],
    regionalParameters: NotRequired[Mapping[str, Mapping[str, str]]],
```

1. See [:material-code-braces: ProvisioningConfigurationTypeDef](./type_defs.md#provisioningconfigurationtypedef) [:material-code-braces: ProvisioningConfigurationOutputTypeDef](./type_defs.md#provisioningconfigurationoutputtypedef) 
## CreateRuleInputTypeDef

```python
# CreateRuleInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateRuleInputTypeDef


def get_value() -> CreateRuleInputTypeDef:
    return {
        "action": ...,
    }


# CreateRuleInputTypeDef definition

class CreateRuleInputTypeDef(TypedDict):
    action: RuleActionType,  # (1)
    detail: RuleDetailUnionTypeDef,  # (2)
    domainIdentifier: str,
    name: str,
    scope: RuleScopeUnionTypeDef,  # (3)
    target: RuleTargetTypeDef,  # (4)
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-brackets: RuleActionType](./literals.md#ruleactiontype) 
2. See [:material-code-braces: RuleDetailTypeDef](./type_defs.md#ruledetailtypedef) [:material-code-braces: RuleDetailOutputTypeDef](./type_defs.md#ruledetailoutputtypedef) 
3. See [:material-code-braces: RuleScopeTypeDef](./type_defs.md#rulescopetypedef) [:material-code-braces: RuleScopeOutputTypeDef](./type_defs.md#rulescopeoutputtypedef) 
4. See [:material-code-braces: RuleTargetTypeDef](./type_defs.md#ruletargettypedef) 
## UpdateRuleInputTypeDef

```python
# UpdateRuleInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateRuleInputTypeDef


def get_value() -> UpdateRuleInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateRuleInputTypeDef definition

class UpdateRuleInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    detail: NotRequired[RuleDetailUnionTypeDef],  # (1)
    includeChildDomainUnits: NotRequired[bool],
    name: NotRequired[str],
    scope: NotRequired[RuleScopeUnionTypeDef],  # (2)
```

1. See [:material-code-braces: RuleDetailTypeDef](./type_defs.md#ruledetailtypedef) [:material-code-braces: RuleDetailOutputTypeDef](./type_defs.md#ruledetailoutputtypedef) 
2. See [:material-code-braces: RuleScopeTypeDef](./type_defs.md#rulescopetypedef) [:material-code-braces: RuleScopeOutputTypeDef](./type_defs.md#rulescopeoutputtypedef) 
## ListLineageEventsOutputTypeDef

```python
# ListLineageEventsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListLineageEventsOutputTypeDef


def get_value() -> ListLineageEventsOutputTypeDef:
    return {
        "items": ...,
    }


# ListLineageEventsOutputTypeDef definition

class ListLineageEventsOutputTypeDef(TypedDict):
    items: List[LineageEventSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LineageEventSummaryTypeDef](./type_defs.md#lineageeventsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssetFilterConfigurationOutputTypeDef

```python
# AssetFilterConfigurationOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetFilterConfigurationOutputTypeDef


def get_value() -> AssetFilterConfigurationOutputTypeDef:
    return {
        "columnConfiguration": ...,
    }


# AssetFilterConfigurationOutputTypeDef definition

class AssetFilterConfigurationOutputTypeDef(TypedDict):
    columnConfiguration: NotRequired[ColumnFilterConfigurationOutputTypeDef],  # (1)
    rowConfiguration: NotRequired[RowFilterConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnFilterConfigurationOutputTypeDef](./type_defs.md#columnfilterconfigurationoutputtypedef) 
2. See [:material-code-braces: RowFilterConfigurationOutputTypeDef](./type_defs.md#rowfilterconfigurationoutputtypedef) 
## AssetFilterConfigurationTypeDef

```python
# AssetFilterConfigurationTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AssetFilterConfigurationTypeDef


def get_value() -> AssetFilterConfigurationTypeDef:
    return {
        "columnConfiguration": ...,
    }


# AssetFilterConfigurationTypeDef definition

class AssetFilterConfigurationTypeDef(TypedDict):
    columnConfiguration: NotRequired[ColumnFilterConfigurationTypeDef],  # (1)
    rowConfiguration: NotRequired[RowFilterConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnFilterConfigurationTypeDef](./type_defs.md#columnfilterconfigurationtypedef) 
2. See [:material-code-braces: RowFilterConfigurationTypeDef](./type_defs.md#rowfilterconfigurationtypedef) 
## PhysicalEndpointTypeDef

```python
# PhysicalEndpointTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import PhysicalEndpointTypeDef


def get_value() -> PhysicalEndpointTypeDef:
    return {
        "awsLocation": ...,
    }


# PhysicalEndpointTypeDef definition

class PhysicalEndpointTypeDef(TypedDict):
    awsLocation: NotRequired[AwsLocationTypeDef],  # (1)
    glueConnection: NotRequired[GlueConnectionTypeDef],  # (2)
    glueConnectionName: NotRequired[str],
    host: NotRequired[str],
    port: NotRequired[int],
    protocol: NotRequired[ProtocolType],  # (3)
    stage: NotRequired[str],
```

1. See [:material-code-braces: AwsLocationTypeDef](./type_defs.md#awslocationtypedef) 
2. See [:material-code-braces: GlueConnectionTypeDef](./type_defs.md#glueconnectiontypedef) 
3. See [:material-code-brackets: ProtocolType](./literals.md#protocoltype) 
## GlueConnectionInputTypeDef

```python
# GlueConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GlueConnectionInputTypeDef


def get_value() -> GlueConnectionInputTypeDef:
    return {
        "athenaProperties": ...,
    }


# GlueConnectionInputTypeDef definition

class GlueConnectionInputTypeDef(TypedDict):
    athenaProperties: NotRequired[Mapping[str, str]],
    authenticationConfiguration: NotRequired[AuthenticationConfigurationInputTypeDef],  # (1)
    connectionProperties: NotRequired[Mapping[str, str]],
    connectionType: NotRequired[GlueConnectionTypeType],  # (2)
    description: NotRequired[str],
    matchCriteria: NotRequired[str],
    name: NotRequired[str],
    physicalConnectionRequirements: NotRequired[PhysicalConnectionRequirementsUnionTypeDef],  # (3)
    pythonProperties: NotRequired[Mapping[str, str]],
    sparkProperties: NotRequired[Mapping[str, str]],
    validateCredentials: NotRequired[bool],
    validateForComputeEnvironments: NotRequired[Sequence[ComputeEnvironmentsType]],  # (4)
```

1. See [:material-code-braces: AuthenticationConfigurationInputTypeDef](./type_defs.md#authenticationconfigurationinputtypedef) 
2. See [:material-code-brackets: GlueConnectionTypeType](./literals.md#glueconnectiontypetype) 
3. See [:material-code-braces: PhysicalConnectionRequirementsTypeDef](./type_defs.md#physicalconnectionrequirementstypedef) [:material-code-braces: PhysicalConnectionRequirementsOutputTypeDef](./type_defs.md#physicalconnectionrequirementsoutputtypedef) 
4. See [:material-code-brackets: ComputeEnvironmentsType](./literals.md#computeenvironmentstype) 
## CreateDataSourceOutputTypeDef

```python
# CreateDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDataSourceOutputTypeDef


def get_value() -> CreateDataSourceOutputTypeDef:
    return {
        "assetFormsOutput": ...,
    }


# CreateDataSourceOutputTypeDef definition

class CreateDataSourceOutputTypeDef(TypedDict):
    assetFormsOutput: List[FormOutputTypeDef],  # (1)
    configuration: DataSourceConfigurationOutputTypeDef,  # (2)
    connectionId: str,
    createdAt: datetime,
    description: str,
    domainId: str,
    enableSetting: EnableSettingType,  # (3)
    environmentId: str,
    errorMessage: DataSourceErrorMessageTypeDef,  # (4)
    id: str,
    lastRunAt: datetime,
    lastRunErrorMessage: DataSourceErrorMessageTypeDef,  # (4)
    lastRunStatus: DataSourceRunStatusType,  # (6)
    name: str,
    projectId: str,
    publishOnImport: bool,
    recommendation: RecommendationConfigurationTypeDef,  # (7)
    schedule: ScheduleConfigurationTypeDef,  # (8)
    status: DataSourceStatusType,  # (9)
    type: str,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
5. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
6. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
7. See [:material-code-braces: RecommendationConfigurationTypeDef](./type_defs.md#recommendationconfigurationtypedef) 
8. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
9. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDataSourceOutputTypeDef

```python
# DeleteDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import DeleteDataSourceOutputTypeDef


def get_value() -> DeleteDataSourceOutputTypeDef:
    return {
        "assetFormsOutput": ...,
    }


# DeleteDataSourceOutputTypeDef definition

class DeleteDataSourceOutputTypeDef(TypedDict):
    assetFormsOutput: List[FormOutputTypeDef],  # (1)
    configuration: DataSourceConfigurationOutputTypeDef,  # (2)
    connectionId: str,
    createdAt: datetime,
    description: str,
    domainId: str,
    enableSetting: EnableSettingType,  # (3)
    environmentId: str,
    errorMessage: DataSourceErrorMessageTypeDef,  # (4)
    id: str,
    lastRunAt: datetime,
    lastRunErrorMessage: DataSourceErrorMessageTypeDef,  # (4)
    lastRunStatus: DataSourceRunStatusType,  # (6)
    name: str,
    projectId: str,
    publishOnImport: bool,
    retainPermissionsOnRevokeFailure: bool,
    schedule: ScheduleConfigurationTypeDef,  # (7)
    selfGrantStatus: SelfGrantStatusOutputTypeDef,  # (8)
    status: DataSourceStatusType,  # (9)
    type: str,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (10)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
5. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
6. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
7. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
8. See [:material-code-braces: SelfGrantStatusOutputTypeDef](./type_defs.md#selfgrantstatusoutputtypedef) 
9. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
10. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataSourceOutputTypeDef

```python
# GetDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetDataSourceOutputTypeDef


def get_value() -> GetDataSourceOutputTypeDef:
    return {
        "assetFormsOutput": ...,
    }


# GetDataSourceOutputTypeDef definition

class GetDataSourceOutputTypeDef(TypedDict):
    assetFormsOutput: List[FormOutputTypeDef],  # (1)
    configuration: DataSourceConfigurationOutputTypeDef,  # (2)
    connectionId: str,
    createdAt: datetime,
    description: str,
    domainId: str,
    enableSetting: EnableSettingType,  # (3)
    environmentId: str,
    errorMessage: DataSourceErrorMessageTypeDef,  # (4)
    id: str,
    lastRunAssetCount: int,
    lastRunAt: datetime,
    lastRunErrorMessage: DataSourceErrorMessageTypeDef,  # (4)
    lastRunStatus: DataSourceRunStatusType,  # (6)
    name: str,
    projectId: str,
    publishOnImport: bool,
    recommendation: RecommendationConfigurationTypeDef,  # (7)
    schedule: ScheduleConfigurationTypeDef,  # (8)
    selfGrantStatus: SelfGrantStatusOutputTypeDef,  # (9)
    status: DataSourceStatusType,  # (10)
    type: str,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
5. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
6. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
7. See [:material-code-braces: RecommendationConfigurationTypeDef](./type_defs.md#recommendationconfigurationtypedef) 
8. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
9. See [:material-code-braces: SelfGrantStatusOutputTypeDef](./type_defs.md#selfgrantstatusoutputtypedef) 
10. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDataSourceOutputTypeDef

```python
# UpdateDataSourceOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateDataSourceOutputTypeDef


def get_value() -> UpdateDataSourceOutputTypeDef:
    return {
        "assetFormsOutput": ...,
    }


# UpdateDataSourceOutputTypeDef definition

class UpdateDataSourceOutputTypeDef(TypedDict):
    assetFormsOutput: List[FormOutputTypeDef],  # (1)
    configuration: DataSourceConfigurationOutputTypeDef,  # (2)
    connectionId: str,
    createdAt: datetime,
    description: str,
    domainId: str,
    enableSetting: EnableSettingType,  # (3)
    environmentId: str,
    errorMessage: DataSourceErrorMessageTypeDef,  # (4)
    id: str,
    lastRunAt: datetime,
    lastRunErrorMessage: DataSourceErrorMessageTypeDef,  # (4)
    lastRunStatus: DataSourceRunStatusType,  # (6)
    name: str,
    projectId: str,
    publishOnImport: bool,
    recommendation: RecommendationConfigurationTypeDef,  # (7)
    retainPermissionsOnRevokeFailure: bool,
    schedule: ScheduleConfigurationTypeDef,  # (8)
    selfGrantStatus: SelfGrantStatusOutputTypeDef,  # (9)
    status: DataSourceStatusType,  # (10)
    type: str,
    updatedAt: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (11)
```

1. See [:material-code-braces: FormOutputTypeDef](./type_defs.md#formoutputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationOutputTypeDef](./type_defs.md#datasourceconfigurationoutputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
5. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
6. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
7. See [:material-code-braces: RecommendationConfigurationTypeDef](./type_defs.md#recommendationconfigurationtypedef) 
8. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
9. See [:material-code-braces: SelfGrantStatusOutputTypeDef](./type_defs.md#selfgrantstatusoutputtypedef) 
10. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
11. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscriptionRequestsOutputTypeDef

```python
# ListSubscriptionRequestsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionRequestsOutputTypeDef


def get_value() -> ListSubscriptionRequestsOutputTypeDef:
    return {
        "items": ...,
    }


# ListSubscriptionRequestsOutputTypeDef definition

class ListSubscriptionRequestsOutputTypeDef(TypedDict):
    items: List[SubscriptionRequestSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionRequestSummaryTypeDef](./type_defs.md#subscriptionrequestsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscriptionsOutputTypeDef

```python
# ListSubscriptionsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListSubscriptionsOutputTypeDef


def get_value() -> ListSubscriptionsOutputTypeDef:
    return {
        "items": ...,
    }


# ListSubscriptionsOutputTypeDef definition

class ListSubscriptionsOutputTypeDef(TypedDict):
    items: List[SubscriptionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionSummaryTypeDef](./type_defs.md#subscriptionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectionInputTypeDef

```python
# UpdateConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateConnectionInputTypeDef


def get_value() -> UpdateConnectionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateConnectionInputTypeDef definition

class UpdateConnectionInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    awsLocation: NotRequired[AwsLocationTypeDef],  # (1)
    description: NotRequired[str],
    props: NotRequired[ConnectionPropertiesPatchTypeDef],  # (2)
```

1. See [:material-code-braces: AwsLocationTypeDef](./type_defs.md#awslocationtypedef) 
2. See [:material-code-braces: ConnectionPropertiesPatchTypeDef](./type_defs.md#connectionpropertiespatchtypedef) 
## ListPolicyGrantsOutputTypeDef

```python
# ListPolicyGrantsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListPolicyGrantsOutputTypeDef


def get_value() -> ListPolicyGrantsOutputTypeDef:
    return {
        "grantList": ...,
    }


# ListPolicyGrantsOutputTypeDef definition

class ListPolicyGrantsOutputTypeDef(TypedDict):
    grantList: List[PolicyGrantMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyGrantMemberTypeDef](./type_defs.md#policygrantmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddPolicyGrantInputTypeDef

```python
# AddPolicyGrantInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import AddPolicyGrantInputTypeDef


def get_value() -> AddPolicyGrantInputTypeDef:
    return {
        "detail": ...,
    }


# AddPolicyGrantInputTypeDef definition

class AddPolicyGrantInputTypeDef(TypedDict):
    detail: PolicyGrantDetailUnionTypeDef,  # (1)
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TargetEntityTypeType,  # (2)
    policyType: ManagedPolicyTypeType,  # (3)
    principal: PolicyGrantPrincipalUnionTypeDef,  # (4)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyGrantDetailTypeDef](./type_defs.md#policygrantdetailtypedef) [:material-code-braces: PolicyGrantDetailOutputTypeDef](./type_defs.md#policygrantdetailoutputtypedef) 
2. See [:material-code-brackets: TargetEntityTypeType](./literals.md#targetentitytypetype) 
3. See [:material-code-brackets: ManagedPolicyTypeType](./literals.md#managedpolicytypetype) 
4. See [:material-code-braces: PolicyGrantPrincipalTypeDef](./type_defs.md#policygrantprincipaltypedef) [:material-code-braces: PolicyGrantPrincipalOutputTypeDef](./type_defs.md#policygrantprincipaloutputtypedef) 
## RemovePolicyGrantInputTypeDef

```python
# RemovePolicyGrantInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import RemovePolicyGrantInputTypeDef


def get_value() -> RemovePolicyGrantInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# RemovePolicyGrantInputTypeDef definition

class RemovePolicyGrantInputTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TargetEntityTypeType,  # (1)
    policyType: ManagedPolicyTypeType,  # (2)
    principal: PolicyGrantPrincipalUnionTypeDef,  # (3)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TargetEntityTypeType](./literals.md#targetentitytypetype) 
2. See [:material-code-brackets: ManagedPolicyTypeType](./literals.md#managedpolicytypetype) 
3. See [:material-code-braces: PolicyGrantPrincipalTypeDef](./type_defs.md#policygrantprincipaltypedef) [:material-code-braces: PolicyGrantPrincipalOutputTypeDef](./type_defs.md#policygrantprincipaloutputtypedef) 
## CreateProjectProfileInputTypeDef

```python
# CreateProjectProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateProjectProfileInputTypeDef


def get_value() -> CreateProjectProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateProjectProfileInputTypeDef definition

class CreateProjectProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    description: NotRequired[str],
    domainUnitIdentifier: NotRequired[str],
    environmentConfigurations: NotRequired[Sequence[EnvironmentConfigurationUnionTypeDef]],  # (1)
    status: NotRequired[StatusType],  # (2)
```

1. See [:material-code-braces: EnvironmentConfigurationTypeDef](./type_defs.md#environmentconfigurationtypedef) [:material-code-braces: EnvironmentConfigurationOutputTypeDef](./type_defs.md#environmentconfigurationoutputtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## UpdateProjectProfileInputTypeDef

```python
# UpdateProjectProfileInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateProjectProfileInputTypeDef


def get_value() -> UpdateProjectProfileInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateProjectProfileInputTypeDef definition

class UpdateProjectProfileInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    domainUnitIdentifier: NotRequired[str],
    environmentConfigurations: NotRequired[Sequence[EnvironmentConfigurationUnionTypeDef]],  # (1)
    name: NotRequired[str],
    status: NotRequired[StatusType],  # (2)
```

1. See [:material-code-braces: EnvironmentConfigurationTypeDef](./type_defs.md#environmentconfigurationtypedef) [:material-code-braces: EnvironmentConfigurationOutputTypeDef](./type_defs.md#environmentconfigurationoutputtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
## CreateDataSourceInputTypeDef

```python
# CreateDataSourceInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateDataSourceInputTypeDef


def get_value() -> CreateDataSourceInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateDataSourceInputTypeDef definition

class CreateDataSourceInputTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    projectIdentifier: str,
    type: str,
    assetFormsInput: NotRequired[Sequence[FormInputTypeDef]],  # (1)
    clientToken: NotRequired[str],
    configuration: NotRequired[DataSourceConfigurationInputTypeDef],  # (2)
    connectionIdentifier: NotRequired[str],
    description: NotRequired[str],
    enableSetting: NotRequired[EnableSettingType],  # (3)
    environmentIdentifier: NotRequired[str],
    publishOnImport: NotRequired[bool],
    recommendation: NotRequired[RecommendationConfigurationTypeDef],  # (4)
    schedule: NotRequired[ScheduleConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationInputTypeDef](./type_defs.md#datasourceconfigurationinputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: RecommendationConfigurationTypeDef](./type_defs.md#recommendationconfigurationtypedef) 
5. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
## UpdateDataSourceInputTypeDef

```python
# UpdateDataSourceInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateDataSourceInputTypeDef


def get_value() -> UpdateDataSourceInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# UpdateDataSourceInputTypeDef definition

class UpdateDataSourceInputTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    assetFormsInput: NotRequired[Sequence[FormInputTypeDef]],  # (1)
    configuration: NotRequired[DataSourceConfigurationInputTypeDef],  # (2)
    description: NotRequired[str],
    enableSetting: NotRequired[EnableSettingType],  # (3)
    name: NotRequired[str],
    publishOnImport: NotRequired[bool],
    recommendation: NotRequired[RecommendationConfigurationTypeDef],  # (4)
    retainPermissionsOnRevokeFailure: NotRequired[bool],
    schedule: NotRequired[ScheduleConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationInputTypeDef](./type_defs.md#datasourceconfigurationinputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: RecommendationConfigurationTypeDef](./type_defs.md#recommendationconfigurationtypedef) 
5. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
## CreateAssetFilterOutputTypeDef

```python
# CreateAssetFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetFilterOutputTypeDef


def get_value() -> CreateAssetFilterOutputTypeDef:
    return {
        "assetId": ...,
    }


# CreateAssetFilterOutputTypeDef definition

class CreateAssetFilterOutputTypeDef(TypedDict):
    assetId: str,
    configuration: AssetFilterConfigurationOutputTypeDef,  # (1)
    createdAt: datetime,
    description: str,
    domainId: str,
    effectiveColumnNames: List[str],
    effectiveRowFilter: str,
    errorMessage: str,
    id: str,
    name: str,
    status: FilterStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssetFilterConfigurationOutputTypeDef](./type_defs.md#assetfilterconfigurationoutputtypedef) 
2. See [:material-code-brackets: FilterStatusType](./literals.md#filterstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAssetFilterOutputTypeDef

```python
# GetAssetFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetAssetFilterOutputTypeDef


def get_value() -> GetAssetFilterOutputTypeDef:
    return {
        "assetId": ...,
    }


# GetAssetFilterOutputTypeDef definition

class GetAssetFilterOutputTypeDef(TypedDict):
    assetId: str,
    configuration: AssetFilterConfigurationOutputTypeDef,  # (1)
    createdAt: datetime,
    description: str,
    domainId: str,
    effectiveColumnNames: List[str],
    effectiveRowFilter: str,
    errorMessage: str,
    id: str,
    name: str,
    status: FilterStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssetFilterConfigurationOutputTypeDef](./type_defs.md#assetfilterconfigurationoutputtypedef) 
2. See [:material-code-brackets: FilterStatusType](./literals.md#filterstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateAssetFilterOutputTypeDef

```python
# UpdateAssetFilterOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateAssetFilterOutputTypeDef


def get_value() -> UpdateAssetFilterOutputTypeDef:
    return {
        "assetId": ...,
    }


# UpdateAssetFilterOutputTypeDef definition

class UpdateAssetFilterOutputTypeDef(TypedDict):
    assetId: str,
    configuration: AssetFilterConfigurationOutputTypeDef,  # (1)
    createdAt: datetime,
    description: str,
    domainId: str,
    effectiveColumnNames: List[str],
    effectiveRowFilter: str,
    errorMessage: str,
    id: str,
    name: str,
    status: FilterStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: AssetFilterConfigurationOutputTypeDef](./type_defs.md#assetfilterconfigurationoutputtypedef) 
2. See [:material-code-brackets: FilterStatusType](./literals.md#filterstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionSummaryTypeDef

```python
# ConnectionSummaryTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ConnectionSummaryTypeDef


def get_value() -> ConnectionSummaryTypeDef:
    return {
        "connectionId": ...,
    }


# ConnectionSummaryTypeDef definition

class ConnectionSummaryTypeDef(TypedDict):
    connectionId: str,
    domainId: str,
    domainUnitId: str,
    name: str,
    physicalEndpoints: List[PhysicalEndpointTypeDef],  # (1)
    type: ConnectionTypeType,  # (3)
    environmentId: NotRequired[str],
    projectId: NotRequired[str],
    props: NotRequired[ConnectionPropertiesOutputTypeDef],  # (2)
```

1. See [:material-code-braces: PhysicalEndpointTypeDef](./type_defs.md#physicalendpointtypedef) 
2. See [:material-code-braces: ConnectionPropertiesOutputTypeDef](./type_defs.md#connectionpropertiesoutputtypedef) 
3. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
## CreateConnectionOutputTypeDef

```python
# CreateConnectionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateConnectionOutputTypeDef


def get_value() -> CreateConnectionOutputTypeDef:
    return {
        "connectionId": ...,
    }


# CreateConnectionOutputTypeDef definition

class CreateConnectionOutputTypeDef(TypedDict):
    connectionId: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentId: str,
    name: str,
    physicalEndpoints: List[PhysicalEndpointTypeDef],  # (1)
    projectId: str,
    props: ConnectionPropertiesOutputTypeDef,  # (2)
    type: ConnectionTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: PhysicalEndpointTypeDef](./type_defs.md#physicalendpointtypedef) 
2. See [:material-code-braces: ConnectionPropertiesOutputTypeDef](./type_defs.md#connectionpropertiesoutputtypedef) 
3. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetConnectionOutputTypeDef

```python
# GetConnectionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GetConnectionOutputTypeDef


def get_value() -> GetConnectionOutputTypeDef:
    return {
        "connectionCredentials": ...,
    }


# GetConnectionOutputTypeDef definition

class GetConnectionOutputTypeDef(TypedDict):
    connectionCredentials: ConnectionCredentialsTypeDef,  # (1)
    connectionId: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentId: str,
    environmentUserRole: str,
    name: str,
    physicalEndpoints: List[PhysicalEndpointTypeDef],  # (2)
    projectId: str,
    props: ConnectionPropertiesOutputTypeDef,  # (3)
    type: ConnectionTypeType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ConnectionCredentialsTypeDef](./type_defs.md#connectioncredentialstypedef) 
2. See [:material-code-braces: PhysicalEndpointTypeDef](./type_defs.md#physicalendpointtypedef) 
3. See [:material-code-braces: ConnectionPropertiesOutputTypeDef](./type_defs.md#connectionpropertiesoutputtypedef) 
4. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConnectionOutputTypeDef

```python
# UpdateConnectionOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateConnectionOutputTypeDef


def get_value() -> UpdateConnectionOutputTypeDef:
    return {
        "connectionId": ...,
    }


# UpdateConnectionOutputTypeDef definition

class UpdateConnectionOutputTypeDef(TypedDict):
    connectionId: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    environmentId: str,
    name: str,
    physicalEndpoints: List[PhysicalEndpointTypeDef],  # (1)
    projectId: str,
    props: ConnectionPropertiesOutputTypeDef,  # (2)
    type: ConnectionTypeType,  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: PhysicalEndpointTypeDef](./type_defs.md#physicalendpointtypedef) 
2. See [:material-code-braces: ConnectionPropertiesOutputTypeDef](./type_defs.md#connectionpropertiesoutputtypedef) 
3. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GluePropertiesInputTypeDef

```python
# GluePropertiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import GluePropertiesInputTypeDef


def get_value() -> GluePropertiesInputTypeDef:
    return {
        "glueConnectionInput": ...,
    }


# GluePropertiesInputTypeDef definition

class GluePropertiesInputTypeDef(TypedDict):
    glueConnectionInput: NotRequired[GlueConnectionInputTypeDef],  # (1)
```

1. See [:material-code-braces: GlueConnectionInputTypeDef](./type_defs.md#glueconnectioninputtypedef) 
## CreateAssetFilterInputTypeDef

```python
# CreateAssetFilterInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateAssetFilterInputTypeDef


def get_value() -> CreateAssetFilterInputTypeDef:
    return {
        "assetIdentifier": ...,
    }


# CreateAssetFilterInputTypeDef definition

class CreateAssetFilterInputTypeDef(TypedDict):
    assetIdentifier: str,
    configuration: AssetFilterConfigurationUnionTypeDef,  # (1)
    domainIdentifier: str,
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: AssetFilterConfigurationTypeDef](./type_defs.md#assetfilterconfigurationtypedef) [:material-code-braces: AssetFilterConfigurationOutputTypeDef](./type_defs.md#assetfilterconfigurationoutputtypedef) 
## UpdateAssetFilterInputTypeDef

```python
# UpdateAssetFilterInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import UpdateAssetFilterInputTypeDef


def get_value() -> UpdateAssetFilterInputTypeDef:
    return {
        "assetIdentifier": ...,
    }


# UpdateAssetFilterInputTypeDef definition

class UpdateAssetFilterInputTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    identifier: str,
    configuration: NotRequired[AssetFilterConfigurationUnionTypeDef],  # (1)
    description: NotRequired[str],
    name: NotRequired[str],
```

1. See [:material-code-braces: AssetFilterConfigurationTypeDef](./type_defs.md#assetfilterconfigurationtypedef) [:material-code-braces: AssetFilterConfigurationOutputTypeDef](./type_defs.md#assetfilterconfigurationoutputtypedef) 
## ListConnectionsOutputTypeDef

```python
# ListConnectionsOutputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ListConnectionsOutputTypeDef


def get_value() -> ListConnectionsOutputTypeDef:
    return {
        "items": ...,
    }


# ListConnectionsOutputTypeDef definition

class ListConnectionsOutputTypeDef(TypedDict):
    items: List[ConnectionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ConnectionSummaryTypeDef](./type_defs.md#connectionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConnectionPropertiesInputTypeDef

```python
# ConnectionPropertiesInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import ConnectionPropertiesInputTypeDef


def get_value() -> ConnectionPropertiesInputTypeDef:
    return {
        "athenaProperties": ...,
    }


# ConnectionPropertiesInputTypeDef definition

class ConnectionPropertiesInputTypeDef(TypedDict):
    athenaProperties: NotRequired[AthenaPropertiesInputTypeDef],  # (1)
    glueProperties: NotRequired[GluePropertiesInputTypeDef],  # (2)
    hyperPodProperties: NotRequired[HyperPodPropertiesInputTypeDef],  # (3)
    iamProperties: NotRequired[IamPropertiesInputTypeDef],  # (4)
    redshiftProperties: NotRequired[RedshiftPropertiesInputTypeDef],  # (5)
    sparkEmrProperties: NotRequired[SparkEmrPropertiesInputTypeDef],  # (6)
    sparkGlueProperties: NotRequired[SparkGluePropertiesInputTypeDef],  # (7)
```

1. See [:material-code-braces: AthenaPropertiesInputTypeDef](./type_defs.md#athenapropertiesinputtypedef) 
2. See [:material-code-braces: GluePropertiesInputTypeDef](./type_defs.md#gluepropertiesinputtypedef) 
3. See [:material-code-braces: HyperPodPropertiesInputTypeDef](./type_defs.md#hyperpodpropertiesinputtypedef) 
4. See [:material-code-braces: IamPropertiesInputTypeDef](./type_defs.md#iampropertiesinputtypedef) 
5. See [:material-code-braces: RedshiftPropertiesInputTypeDef](./type_defs.md#redshiftpropertiesinputtypedef) 
6. See [:material-code-braces: SparkEmrPropertiesInputTypeDef](./type_defs.md#sparkemrpropertiesinputtypedef) 
7. See [:material-code-braces: SparkGluePropertiesInputTypeDef](./type_defs.md#sparkgluepropertiesinputtypedef) 
## CreateConnectionInputTypeDef

```python
# CreateConnectionInputTypeDef TypedDict usage example

from types_aiobotocore_datazone.type_defs import CreateConnectionInputTypeDef


def get_value() -> CreateConnectionInputTypeDef:
    return {
        "domainIdentifier": ...,
    }


# CreateConnectionInputTypeDef definition

class CreateConnectionInputTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    name: str,
    awsLocation: NotRequired[AwsLocationTypeDef],  # (1)
    clientToken: NotRequired[str],
    description: NotRequired[str],
    props: NotRequired[ConnectionPropertiesInputTypeDef],  # (2)
```

1. See [:material-code-braces: AwsLocationTypeDef](./type_defs.md#awslocationtypedef) 
2. See [:material-code-braces: ConnectionPropertiesInputTypeDef](./type_defs.md#connectionpropertiesinputtypedef) 

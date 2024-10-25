# Type definitions

> [Index](../README.md) > [DataZone](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [DataZone](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
    type annotations stubs module [types-aiobotocore-datazone](https://pypi.org/project/types-aiobotocore-datazone/).

## BlobTypeDef

```python
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
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```


## ColumnFilterConfigurationUnionTypeDef

```python
# ColumnFilterConfigurationUnionTypeDef definition

ColumnFilterConfigurationUnionTypeDef = Union[
    ColumnFilterConfigurationTypeDef,  # (1)
    ColumnFilterConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ColumnFilterConfigurationTypeDef](./type_defs.md#columnfilterconfigurationtypedef) 
2. See [:material-code-braces: ColumnFilterConfigurationOutputTypeDef](./type_defs.md#columnfilterconfigurationoutputtypedef) 

## DataProductItemUnionTypeDef

```python
# DataProductItemUnionTypeDef definition

DataProductItemUnionTypeDef = Union[
    DataProductItemTypeDef,  # (1)
    DataProductItemOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DataProductItemTypeDef](./type_defs.md#dataproductitemtypedef) 
2. See [:material-code-braces: DataProductItemOutputTypeDef](./type_defs.md#dataproductitemoutputtypedef) 

## DomainUnitGrantFilterUnionTypeDef

```python
# DomainUnitGrantFilterUnionTypeDef definition

DomainUnitGrantFilterUnionTypeDef = Union[
    DomainUnitGrantFilterTypeDef,  # (1)
    DomainUnitGrantFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DomainUnitGrantFilterTypeDef](./type_defs.md#domainunitgrantfiltertypedef) 
2. See [:material-code-braces: DomainUnitGrantFilterOutputTypeDef](./type_defs.md#domainunitgrantfilteroutputtypedef) 

## InExpressionUnionTypeDef

```python
# InExpressionUnionTypeDef definition

InExpressionUnionTypeDef = Union[
    InExpressionTypeDef,  # (1)
    InExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: InExpressionTypeDef](./type_defs.md#inexpressiontypedef) 
2. See [:material-code-braces: InExpressionOutputTypeDef](./type_defs.md#inexpressionoutputtypedef) 

## LakeFormationConfigurationUnionTypeDef

```python
# LakeFormationConfigurationUnionTypeDef definition

LakeFormationConfigurationUnionTypeDef = Union[
    LakeFormationConfigurationTypeDef,  # (1)
    LakeFormationConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) 
2. See [:material-code-braces: LakeFormationConfigurationOutputTypeDef](./type_defs.md#lakeformationconfigurationoutputtypedef) 

## NotInExpressionUnionTypeDef

```python
# NotInExpressionUnionTypeDef definition

NotInExpressionUnionTypeDef = Union[
    NotInExpressionTypeDef,  # (1)
    NotInExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: NotInExpressionTypeDef](./type_defs.md#notinexpressiontypedef) 
2. See [:material-code-braces: NotInExpressionOutputTypeDef](./type_defs.md#notinexpressionoutputtypedef) 

## UserPolicyGrantPrincipalUnionTypeDef

```python
# UserPolicyGrantPrincipalUnionTypeDef definition

UserPolicyGrantPrincipalUnionTypeDef = Union[
    UserPolicyGrantPrincipalTypeDef,  # (1)
    UserPolicyGrantPrincipalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: UserPolicyGrantPrincipalTypeDef](./type_defs.md#userpolicygrantprincipaltypedef) 
2. See [:material-code-braces: UserPolicyGrantPrincipalOutputTypeDef](./type_defs.md#userpolicygrantprincipaloutputtypedef) 

## RelationalFilterConfigurationUnionTypeDef

```python
# RelationalFilterConfigurationUnionTypeDef definition

RelationalFilterConfigurationUnionTypeDef = Union[
    RelationalFilterConfigurationTypeDef,  # (1)
    RelationalFilterConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RelationalFilterConfigurationTypeDef](./type_defs.md#relationalfilterconfigurationtypedef) 
2. See [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 

## DomainUnitPolicyGrantPrincipalUnionTypeDef

```python
# DomainUnitPolicyGrantPrincipalUnionTypeDef definition

DomainUnitPolicyGrantPrincipalUnionTypeDef = Union[
    DomainUnitPolicyGrantPrincipalTypeDef,  # (1)
    DomainUnitPolicyGrantPrincipalOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: DomainUnitPolicyGrantPrincipalTypeDef](./type_defs.md#domainunitpolicygrantprincipaltypedef) 
2. See [:material-code-braces: DomainUnitPolicyGrantPrincipalOutputTypeDef](./type_defs.md#domainunitpolicygrantprincipaloutputtypedef) 

## ProvisioningConfigurationUnionTypeDef

```python
# ProvisioningConfigurationUnionTypeDef definition

ProvisioningConfigurationUnionTypeDef = Union[
    ProvisioningConfigurationTypeDef,  # (1)
    ProvisioningConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ProvisioningConfigurationTypeDef](./type_defs.md#provisioningconfigurationtypedef) 
2. See [:material-code-braces: ProvisioningConfigurationOutputTypeDef](./type_defs.md#provisioningconfigurationoutputtypedef) 

## RowFilterExpressionUnionTypeDef

```python
# RowFilterExpressionUnionTypeDef definition

RowFilterExpressionUnionTypeDef = Union[
    RowFilterExpressionTypeDef,  # (1)
    RowFilterExpressionOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RowFilterExpressionTypeDef](./type_defs.md#rowfilterexpressiontypedef) 
2. See [:material-code-braces: RowFilterExpressionOutputTypeDef](./type_defs.md#rowfilterexpressionoutputtypedef) 

## RowFilterUnionTypeDef

```python
# RowFilterUnionTypeDef definition

RowFilterUnionTypeDef = Union[
    RowFilterTypeDef,  # (1)
    RowFilterOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RowFilterTypeDef](./type_defs.md#rowfiltertypedef) 
2. See [:material-code-braces: RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef) 

## RowFilterConfigurationUnionTypeDef

```python
# RowFilterConfigurationUnionTypeDef definition

RowFilterConfigurationUnionTypeDef = Union[
    RowFilterConfigurationTypeDef,  # (1)
    RowFilterConfigurationOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: RowFilterConfigurationTypeDef](./type_defs.md#rowfilterconfigurationtypedef) 
2. See [:material-code-braces: RowFilterConfigurationOutputTypeDef](./type_defs.md#rowfilterconfigurationoutputtypedef) 



## AcceptChoiceTypeDef

```python
# AcceptChoiceTypeDef definition

class AcceptChoiceTypeDef(TypedDict):
    predictionTarget: str,
    editedValue: NotRequired[str],
    predictionChoice: NotRequired[int],
```

## AcceptRuleTypeDef

```python
# AcceptRuleTypeDef definition

class AcceptRuleTypeDef(TypedDict):
    rule: NotRequired[AcceptRuleBehaviorType],  # (1)
    threshold: NotRequired[float],
```

1. See [:material-code-brackets: AcceptRuleBehaviorType](./literals.md#acceptrulebehaviortype) 
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

## AcceptedAssetScopeTypeDef

```python
# AcceptedAssetScopeTypeDef definition

class AcceptedAssetScopeTypeDef(TypedDict):
    assetId: str,
    filterIds: Sequence[str],
```

## AwsConsoleLinkParametersTypeDef

```python
# AwsConsoleLinkParametersTypeDef definition

class AwsConsoleLinkParametersTypeDef(TypedDict):
    uri: NotRequired[str],
```

## AddToProjectMemberPoolPolicyGrantDetailTypeDef

```python
# AddToProjectMemberPoolPolicyGrantDetailTypeDef definition

class AddToProjectMemberPoolPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## ColumnFilterConfigurationOutputTypeDef

```python
# ColumnFilterConfigurationOutputTypeDef definition

class ColumnFilterConfigurationOutputTypeDef(TypedDict):
    includedColumnNames: NotRequired[List[str]],
```

## AssetFilterSummaryTypeDef

```python
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
# AssetInDataProductListingItemTypeDef definition

class AssetInDataProductListingItemTypeDef(TypedDict):
    entityId: NotRequired[str],
    entityRevision: NotRequired[str],
    entityType: NotRequired[str],
```

## FormOutputTypeDef

```python
# FormOutputTypeDef definition

class FormOutputTypeDef(TypedDict):
    formName: str,
    content: NotRequired[str],
    typeName: NotRequired[str],
    typeRevision: NotRequired[str],
```

## TimeSeriesDataPointSummaryFormOutputTypeDef

```python
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
# AssetListingDetailsTypeDef definition

class AssetListingDetailsTypeDef(TypedDict):
    listingId: str,
    listingStatus: ListingStatusType,  # (1)
```

1. See [:material-code-brackets: ListingStatusType](./literals.md#listingstatustype) 
## DetailedGlossaryTermTypeDef

```python
# DetailedGlossaryTermTypeDef definition

class DetailedGlossaryTermTypeDef(TypedDict):
    name: NotRequired[str],
    shortDescription: NotRequired[str],
```

## AssetRevisionTypeDef

```python
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
# AssetScopeTypeDef definition

class AssetScopeTypeDef(TypedDict):
    assetId: str,
    filterIds: List[str],
    status: str,
    errorMessage: NotRequired[str],
```

## AssetTargetNameMapTypeDef

```python
# AssetTargetNameMapTypeDef definition

class AssetTargetNameMapTypeDef(TypedDict):
    assetId: str,
    targetName: str,
```

## FormEntryOutputTypeDef

```python
# FormEntryOutputTypeDef definition

class FormEntryOutputTypeDef(TypedDict):
    typeName: str,
    typeRevision: str,
    required: NotRequired[bool],
```

## AssociateEnvironmentRoleInputRequestTypeDef

```python
# AssociateEnvironmentRoleInputRequestTypeDef definition

class AssociateEnvironmentRoleInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    environmentRoleArn: str,
```

## BusinessNameGenerationConfigurationTypeDef

```python
# BusinessNameGenerationConfigurationTypeDef definition

class BusinessNameGenerationConfigurationTypeDef(TypedDict):
    enabled: NotRequired[bool],
```

## CancelMetadataGenerationRunInputRequestTypeDef

```python
# CancelMetadataGenerationRunInputRequestTypeDef definition

class CancelMetadataGenerationRunInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## CancelSubscriptionInputRequestTypeDef

```python
# CancelSubscriptionInputRequestTypeDef definition

class CancelSubscriptionInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## CloudFormationPropertiesTypeDef

```python
# CloudFormationPropertiesTypeDef definition

class CloudFormationPropertiesTypeDef(TypedDict):
    templateUrl: str,
```

## ColumnFilterConfigurationTypeDef

```python
# ColumnFilterConfigurationTypeDef definition

class ColumnFilterConfigurationTypeDef(TypedDict):
    includedColumnNames: NotRequired[Sequence[str]],
```

## ConfigurableActionParameterTypeDef

```python
# ConfigurableActionParameterTypeDef definition

class ConfigurableActionParameterTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## FormInputTypeDef

```python
# FormInputTypeDef definition

class FormInputTypeDef(TypedDict):
    formName: str,
    content: NotRequired[str],
    typeIdentifier: NotRequired[str],
    typeRevision: NotRequired[str],
```

## FormEntryInputTypeDef

```python
# FormEntryInputTypeDef definition

class FormEntryInputTypeDef(TypedDict):
    typeIdentifier: str,
    typeRevision: str,
    required: NotRequired[bool],
```

## CreateAssetTypePolicyGrantDetailTypeDef

```python
# CreateAssetTypePolicyGrantDetailTypeDef definition

class CreateAssetTypePolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## DataProductItemOutputTypeDef

```python
# DataProductItemOutputTypeDef definition

class DataProductItemOutputTypeDef(TypedDict):
    identifier: str,
    itemType: DataProductItemTypeType,  # (1)
    glossaryTerms: NotRequired[List[str]],
    revision: NotRequired[str],
```

1. See [:material-code-brackets: DataProductItemTypeType](./literals.md#dataproductitemtypetype) 
## DataProductItemTypeDef

```python
# DataProductItemTypeDef definition

class DataProductItemTypeDef(TypedDict):
    identifier: str,
    itemType: DataProductItemTypeType,  # (1)
    glossaryTerms: NotRequired[Sequence[str]],
    revision: NotRequired[str],
```

1. See [:material-code-brackets: DataProductItemTypeType](./literals.md#dataproductitemtypetype) 
## RecommendationConfigurationTypeDef

```python
# RecommendationConfigurationTypeDef definition

class RecommendationConfigurationTypeDef(TypedDict):
    enableBusinessNameGeneration: NotRequired[bool],
```

## ScheduleConfigurationTypeDef

```python
# ScheduleConfigurationTypeDef definition

class ScheduleConfigurationTypeDef(TypedDict):
    schedule: NotRequired[str],
    timezone: NotRequired[TimezoneType],  # (1)
```

1. See [:material-code-brackets: TimezoneType](./literals.md#timezonetype) 
## DataSourceErrorMessageTypeDef

```python
# DataSourceErrorMessageTypeDef definition

class DataSourceErrorMessageTypeDef(TypedDict):
    errorType: DataSourceErrorTypeType,  # (1)
    errorDetail: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceErrorTypeType](./literals.md#datasourceerrortypetype) 
## SingleSignOnTypeDef

```python
# SingleSignOnTypeDef definition

class SingleSignOnTypeDef(TypedDict):
    type: NotRequired[AuthTypeType],  # (1)
    userAssignment: NotRequired[UserAssignmentType],  # (2)
```

1. See [:material-code-brackets: AuthTypeType](./literals.md#authtypetype) 
2. See [:material-code-brackets: UserAssignmentType](./literals.md#userassignmenttype) 
## CreateDomainUnitInputRequestTypeDef

```python
# CreateDomainUnitInputRequestTypeDef definition

class CreateDomainUnitInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    parentDomainUnitIdentifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

## CreateDomainUnitPolicyGrantDetailTypeDef

```python
# CreateDomainUnitPolicyGrantDetailTypeDef definition

class CreateDomainUnitPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## EnvironmentParameterTypeDef

```python
# EnvironmentParameterTypeDef definition

class EnvironmentParameterTypeDef(TypedDict):
    name: NotRequired[str],
    value: NotRequired[str],
```

## CustomParameterTypeDef

```python
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
# DeploymentPropertiesTypeDef definition

class DeploymentPropertiesTypeDef(TypedDict):
    endTimeoutMinutes: NotRequired[int],
    startTimeoutMinutes: NotRequired[int],
```

## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    type: str,
    value: str,
    name: NotRequired[str],
    provider: NotRequired[str],
```

## CreateEnvironmentProfilePolicyGrantDetailTypeDef

```python
# CreateEnvironmentProfilePolicyGrantDetailTypeDef definition

class CreateEnvironmentProfilePolicyGrantDetailTypeDef(TypedDict):
    domainUnitId: NotRequired[str],
```

## ModelTypeDef

```python
# ModelTypeDef definition

class ModelTypeDef(TypedDict):
    smithy: NotRequired[str],
```

## CreateFormTypePolicyGrantDetailTypeDef

```python
# CreateFormTypePolicyGrantDetailTypeDef definition

class CreateFormTypePolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## CreateGlossaryInputRequestTypeDef

```python
# CreateGlossaryInputRequestTypeDef definition

class CreateGlossaryInputRequestTypeDef(TypedDict):
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
# CreateGlossaryPolicyGrantDetailTypeDef definition

class CreateGlossaryPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## TermRelationsTypeDef

```python
# TermRelationsTypeDef definition

class TermRelationsTypeDef(TypedDict):
    classifies: NotRequired[Sequence[str]],
    isA: NotRequired[Sequence[str]],
```

## TermRelationsOutputTypeDef

```python
# TermRelationsOutputTypeDef definition

class TermRelationsOutputTypeDef(TypedDict):
    classifies: NotRequired[List[str]],
    isA: NotRequired[List[str]],
```

## CreateGroupProfileInputRequestTypeDef

```python
# CreateGroupProfileInputRequestTypeDef definition

class CreateGroupProfileInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: str,
    clientToken: NotRequired[str],
```

## CreateListingChangeSetInputRequestTypeDef

```python
# CreateListingChangeSetInputRequestTypeDef definition

class CreateListingChangeSetInputRequestTypeDef(TypedDict):
    action: ChangeActionType,  # (1)
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: EntityTypeType,  # (2)
    clientToken: NotRequired[str],
    entityRevision: NotRequired[str],
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-brackets: EntityTypeType](./literals.md#entitytypetype) 
## CreateProjectInputRequestTypeDef

```python
# CreateProjectInputRequestTypeDef definition

class CreateProjectInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    name: str,
    description: NotRequired[str],
    domainUnitId: NotRequired[str],
    glossaryTerms: NotRequired[Sequence[str]],
```

## MemberTypeDef

```python
# MemberTypeDef definition

class MemberTypeDef(TypedDict):
    groupIdentifier: NotRequired[str],
    userIdentifier: NotRequired[str],
```

## ProjectDeletionErrorTypeDef

```python
# ProjectDeletionErrorTypeDef definition

class ProjectDeletionErrorTypeDef(TypedDict):
    code: NotRequired[str],
    message: NotRequired[str],
```

## CreateProjectPolicyGrantDetailTypeDef

```python
# CreateProjectPolicyGrantDetailTypeDef definition

class CreateProjectPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## SubscribedListingInputTypeDef

```python
# SubscribedListingInputTypeDef definition

class SubscribedListingInputTypeDef(TypedDict):
    identifier: str,
```

## SubscriptionTargetFormTypeDef

```python
# SubscriptionTargetFormTypeDef definition

class SubscriptionTargetFormTypeDef(TypedDict):
    content: str,
    formName: str,
```

## CreateUserProfileInputRequestTypeDef

```python
# CreateUserProfileInputRequestTypeDef definition

class CreateUserProfileInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    userIdentifier: str,
    clientToken: NotRequired[str],
    userType: NotRequired[UserTypeType],  # (1)
```

1. See [:material-code-brackets: UserTypeType](./literals.md#usertypetype) 
## DataProductListingItemAdditionalAttributesTypeDef

```python
# DataProductListingItemAdditionalAttributesTypeDef definition

class DataProductListingItemAdditionalAttributesTypeDef(TypedDict):
    forms: NotRequired[str],
```

## DataProductResultItemTypeDef

```python
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
# DataProductRevisionTypeDef definition

class DataProductRevisionTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    domainId: NotRequired[str],
    id: NotRequired[str],
    revision: NotRequired[str],
```

## RunStatisticsForAssetsTypeDef

```python
# RunStatisticsForAssetsTypeDef definition

class RunStatisticsForAssetsTypeDef(TypedDict):
    added: NotRequired[int],
    failed: NotRequired[int],
    skipped: NotRequired[int],
    unchanged: NotRequired[int],
    updated: NotRequired[int],
```

## DeleteAssetFilterInputRequestTypeDef

```python
# DeleteAssetFilterInputRequestTypeDef definition

class DeleteAssetFilterInputRequestTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    identifier: str,
```

## DeleteAssetInputRequestTypeDef

```python
# DeleteAssetInputRequestTypeDef definition

class DeleteAssetInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteAssetTypeInputRequestTypeDef

```python
# DeleteAssetTypeInputRequestTypeDef definition

class DeleteAssetTypeInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteDataProductInputRequestTypeDef

```python
# DeleteDataProductInputRequestTypeDef definition

class DeleteDataProductInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteDataSourceInputRequestTypeDef

```python
# DeleteDataSourceInputRequestTypeDef definition

class DeleteDataSourceInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    clientToken: NotRequired[str],
    retainPermissionsOnRevokeFailure: NotRequired[bool],
```

## DeleteDomainInputRequestTypeDef

```python
# DeleteDomainInputRequestTypeDef definition

class DeleteDomainInputRequestTypeDef(TypedDict):
    identifier: str,
    clientToken: NotRequired[str],
    skipDeletionCheck: NotRequired[bool],
```

## DeleteDomainUnitInputRequestTypeDef

```python
# DeleteDomainUnitInputRequestTypeDef definition

class DeleteDomainUnitInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteEnvironmentActionInputRequestTypeDef

```python
# DeleteEnvironmentActionInputRequestTypeDef definition

class DeleteEnvironmentActionInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
```

## DeleteEnvironmentBlueprintConfigurationInputRequestTypeDef

```python
# DeleteEnvironmentBlueprintConfigurationInputRequestTypeDef definition

class DeleteEnvironmentBlueprintConfigurationInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentBlueprintIdentifier: str,
```

## DeleteEnvironmentInputRequestTypeDef

```python
# DeleteEnvironmentInputRequestTypeDef definition

class DeleteEnvironmentInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteEnvironmentProfileInputRequestTypeDef

```python
# DeleteEnvironmentProfileInputRequestTypeDef definition

class DeleteEnvironmentProfileInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteFormTypeInputRequestTypeDef

```python
# DeleteFormTypeInputRequestTypeDef definition

class DeleteFormTypeInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    formTypeIdentifier: str,
```

## DeleteGlossaryInputRequestTypeDef

```python
# DeleteGlossaryInputRequestTypeDef definition

class DeleteGlossaryInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteGlossaryTermInputRequestTypeDef

```python
# DeleteGlossaryTermInputRequestTypeDef definition

class DeleteGlossaryTermInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteListingInputRequestTypeDef

```python
# DeleteListingInputRequestTypeDef definition

class DeleteListingInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteProjectInputRequestTypeDef

```python
# DeleteProjectInputRequestTypeDef definition

class DeleteProjectInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    skipDeletionCheck: NotRequired[bool],
```

## DeleteSubscriptionGrantInputRequestTypeDef

```python
# DeleteSubscriptionGrantInputRequestTypeDef definition

class DeleteSubscriptionGrantInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteSubscriptionRequestInputRequestTypeDef

```python
# DeleteSubscriptionRequestInputRequestTypeDef definition

class DeleteSubscriptionRequestInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## DeleteSubscriptionTargetInputRequestTypeDef

```python
# DeleteSubscriptionTargetInputRequestTypeDef definition

class DeleteSubscriptionTargetInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
```

## DeleteTimeSeriesDataPointsInputRequestTypeDef

```python
# DeleteTimeSeriesDataPointsInputRequestTypeDef definition

class DeleteTimeSeriesDataPointsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    formName: str,
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
## EnvironmentErrorTypeDef

```python
# EnvironmentErrorTypeDef definition

class EnvironmentErrorTypeDef(TypedDict):
    message: str,
    code: NotRequired[str],
```

## DisassociateEnvironmentRoleInputRequestTypeDef

```python
# DisassociateEnvironmentRoleInputRequestTypeDef definition

class DisassociateEnvironmentRoleInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    environmentRoleArn: str,
```

## DomainSummaryTypeDef

```python
# DomainSummaryTypeDef definition

class DomainSummaryTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    id: str,
    managedAccountId: str,
    name: str,
    status: DomainStatusType,  # (1)
    description: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    portalUrl: NotRequired[str],
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
## DomainUnitFilterForProjectTypeDef

```python
# DomainUnitFilterForProjectTypeDef definition

class DomainUnitFilterForProjectTypeDef(TypedDict):
    domainUnit: str,
    includeChildDomainUnits: NotRequired[bool],
```

## DomainUnitGrantFilterOutputTypeDef

```python
# DomainUnitGrantFilterOutputTypeDef definition

class DomainUnitGrantFilterOutputTypeDef(TypedDict):
    allDomainUnitsGrantFilter: NotRequired[Dict[str, Any]],
```

## DomainUnitGrantFilterTypeDef

```python
# DomainUnitGrantFilterTypeDef definition

class DomainUnitGrantFilterTypeDef(TypedDict):
    allDomainUnitsGrantFilter: NotRequired[Mapping[str, Any]],
```

## DomainUnitGroupPropertiesTypeDef

```python
# DomainUnitGroupPropertiesTypeDef definition

class DomainUnitGroupPropertiesTypeDef(TypedDict):
    groupId: NotRequired[str],
```

## DomainUnitUserPropertiesTypeDef

```python
# DomainUnitUserPropertiesTypeDef definition

class DomainUnitUserPropertiesTypeDef(TypedDict):
    userId: NotRequired[str],
```

## DomainUnitSummaryTypeDef

```python
# DomainUnitSummaryTypeDef definition

class DomainUnitSummaryTypeDef(TypedDict):
    id: str,
    name: str,
```

## EnvironmentProfileSummaryTypeDef

```python
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
# EqualToExpressionTypeDef definition

class EqualToExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## FailureCauseTypeDef

```python
# FailureCauseTypeDef definition

class FailureCauseTypeDef(TypedDict):
    message: NotRequired[str],
```

## FilterTypeDef

```python
# FilterTypeDef definition

class FilterTypeDef(TypedDict):
    attribute: str,
    value: str,
```

## FilterExpressionTypeDef

```python
# FilterExpressionTypeDef definition

class FilterExpressionTypeDef(TypedDict):
    expression: str,
    type: FilterExpressionTypeType,  # (1)
```

1. See [:material-code-brackets: FilterExpressionTypeType](./literals.md#filterexpressiontypetype) 
## ImportTypeDef

```python
# ImportTypeDef definition

class ImportTypeDef(TypedDict):
    name: str,
    revision: str,
```

## GetAssetFilterInputRequestTypeDef

```python
# GetAssetFilterInputRequestTypeDef definition

class GetAssetFilterInputRequestTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    identifier: str,
```

## GetAssetInputRequestTypeDef

```python
# GetAssetInputRequestTypeDef definition

class GetAssetInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    revision: NotRequired[str],
```

## GetAssetTypeInputRequestTypeDef

```python
# GetAssetTypeInputRequestTypeDef definition

class GetAssetTypeInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    revision: NotRequired[str],
```

## GetDataProductInputRequestTypeDef

```python
# GetDataProductInputRequestTypeDef definition

class GetDataProductInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    revision: NotRequired[str],
```

## GetDataSourceInputRequestTypeDef

```python
# GetDataSourceInputRequestTypeDef definition

class GetDataSourceInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetDataSourceRunInputRequestTypeDef

```python
# GetDataSourceRunInputRequestTypeDef definition

class GetDataSourceRunInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetDomainInputRequestTypeDef

```python
# GetDomainInputRequestTypeDef definition

class GetDomainInputRequestTypeDef(TypedDict):
    identifier: str,
```

## GetDomainUnitInputRequestTypeDef

```python
# GetDomainUnitInputRequestTypeDef definition

class GetDomainUnitInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetEnvironmentActionInputRequestTypeDef

```python
# GetEnvironmentActionInputRequestTypeDef definition

class GetEnvironmentActionInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
```

## GetEnvironmentBlueprintConfigurationInputRequestTypeDef

```python
# GetEnvironmentBlueprintConfigurationInputRequestTypeDef definition

class GetEnvironmentBlueprintConfigurationInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentBlueprintIdentifier: str,
```

## GetEnvironmentBlueprintInputRequestTypeDef

```python
# GetEnvironmentBlueprintInputRequestTypeDef definition

class GetEnvironmentBlueprintInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetEnvironmentCredentialsInputRequestTypeDef

```python
# GetEnvironmentCredentialsInputRequestTypeDef definition

class GetEnvironmentCredentialsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
```

## GetEnvironmentInputRequestTypeDef

```python
# GetEnvironmentInputRequestTypeDef definition

class GetEnvironmentInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetEnvironmentProfileInputRequestTypeDef

```python
# GetEnvironmentProfileInputRequestTypeDef definition

class GetEnvironmentProfileInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetFormTypeInputRequestTypeDef

```python
# GetFormTypeInputRequestTypeDef definition

class GetFormTypeInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    formTypeIdentifier: str,
    revision: NotRequired[str],
```

## GetGlossaryInputRequestTypeDef

```python
# GetGlossaryInputRequestTypeDef definition

class GetGlossaryInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetGlossaryTermInputRequestTypeDef

```python
# GetGlossaryTermInputRequestTypeDef definition

class GetGlossaryTermInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetGroupProfileInputRequestTypeDef

```python
# GetGroupProfileInputRequestTypeDef definition

class GetGroupProfileInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: str,
```

## GetIamPortalLoginUrlInputRequestTypeDef

```python
# GetIamPortalLoginUrlInputRequestTypeDef definition

class GetIamPortalLoginUrlInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
```

## LineageNodeReferenceTypeDef

```python
# LineageNodeReferenceTypeDef definition

class LineageNodeReferenceTypeDef(TypedDict):
    eventTimestamp: NotRequired[datetime],
    id: NotRequired[str],
```

## GetListingInputRequestTypeDef

```python
# GetListingInputRequestTypeDef definition

class GetListingInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    listingRevision: NotRequired[str],
```

## GetMetadataGenerationRunInputRequestTypeDef

```python
# GetMetadataGenerationRunInputRequestTypeDef definition

class GetMetadataGenerationRunInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## MetadataGenerationRunTargetTypeDef

```python
# MetadataGenerationRunTargetTypeDef definition

class MetadataGenerationRunTargetTypeDef(TypedDict):
    identifier: str,
    type: MetadataGenerationTargetTypeType,  # (1)
    revision: NotRequired[str],
```

1. See [:material-code-brackets: MetadataGenerationTargetTypeType](./literals.md#metadatagenerationtargettypetype) 
## GetProjectInputRequestTypeDef

```python
# GetProjectInputRequestTypeDef definition

class GetProjectInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetSubscriptionGrantInputRequestTypeDef

```python
# GetSubscriptionGrantInputRequestTypeDef definition

class GetSubscriptionGrantInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetSubscriptionInputRequestTypeDef

```python
# GetSubscriptionInputRequestTypeDef definition

class GetSubscriptionInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetSubscriptionRequestDetailsInputRequestTypeDef

```python
# GetSubscriptionRequestDetailsInputRequestTypeDef definition

class GetSubscriptionRequestDetailsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
```

## GetSubscriptionTargetInputRequestTypeDef

```python
# GetSubscriptionTargetInputRequestTypeDef definition

class GetSubscriptionTargetInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    identifier: str,
```

## GetTimeSeriesDataPointInputRequestTypeDef

```python
# GetTimeSeriesDataPointInputRequestTypeDef definition

class GetTimeSeriesDataPointInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TimeSeriesEntityTypeType,  # (1)
    formName: str,
    identifier: str,
```

1. See [:material-code-brackets: TimeSeriesEntityTypeType](./literals.md#timeseriesentitytypetype) 
## TimeSeriesDataPointFormOutputTypeDef

```python
# TimeSeriesDataPointFormOutputTypeDef definition

class TimeSeriesDataPointFormOutputTypeDef(TypedDict):
    formName: str,
    timestamp: datetime,
    typeIdentifier: str,
    content: NotRequired[str],
    id: NotRequired[str],
    typeRevision: NotRequired[str],
```

## GetUserProfileInputRequestTypeDef

```python
# GetUserProfileInputRequestTypeDef definition

class GetUserProfileInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    userIdentifier: str,
    type: NotRequired[UserProfileTypeType],  # (1)
```

1. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
## GlossaryItemTypeDef

```python
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
## SelfGrantStatusDetailTypeDef

```python
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
# ListingRevisionInputTypeDef definition

class ListingRevisionInputTypeDef(TypedDict):
    identifier: str,
    revision: str,
```

## ListingRevisionTypeDef

```python
# ListingRevisionTypeDef definition

class ListingRevisionTypeDef(TypedDict):
    id: str,
    revision: str,
```

## GreaterThanExpressionTypeDef

```python
# GreaterThanExpressionTypeDef definition

class GreaterThanExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## GreaterThanOrEqualToExpressionTypeDef

```python
# GreaterThanOrEqualToExpressionTypeDef definition

class GreaterThanOrEqualToExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## GroupDetailsTypeDef

```python
# GroupDetailsTypeDef definition

class GroupDetailsTypeDef(TypedDict):
    groupId: str,
```

## GroupPolicyGrantPrincipalTypeDef

```python
# GroupPolicyGrantPrincipalTypeDef definition

class GroupPolicyGrantPrincipalTypeDef(TypedDict):
    groupIdentifier: NotRequired[str],
```

## GroupProfileSummaryTypeDef

```python
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
# IamUserProfileDetailsTypeDef definition

class IamUserProfileDetailsTypeDef(TypedDict):
    arn: NotRequired[str],
```

## InExpressionOutputTypeDef

```python
# InExpressionOutputTypeDef definition

class InExpressionOutputTypeDef(TypedDict):
    columnName: str,
    values: List[str],
```

## InExpressionTypeDef

```python
# InExpressionTypeDef definition

class InExpressionTypeDef(TypedDict):
    columnName: str,
    values: Sequence[str],
```

## IsNotNullExpressionTypeDef

```python
# IsNotNullExpressionTypeDef definition

class IsNotNullExpressionTypeDef(TypedDict):
    columnName: str,
```

## IsNullExpressionTypeDef

```python
# IsNullExpressionTypeDef definition

class IsNullExpressionTypeDef(TypedDict):
    columnName: str,
```

## LakeFormationConfigurationOutputTypeDef

```python
# LakeFormationConfigurationOutputTypeDef definition

class LakeFormationConfigurationOutputTypeDef(TypedDict):
    locationRegistrationExcludeS3Locations: NotRequired[List[str]],
    locationRegistrationRole: NotRequired[str],
```

## LakeFormationConfigurationTypeDef

```python
# LakeFormationConfigurationTypeDef definition

class LakeFormationConfigurationTypeDef(TypedDict):
    locationRegistrationExcludeS3Locations: NotRequired[Sequence[str]],
    locationRegistrationRole: NotRequired[str],
```

## LessThanExpressionTypeDef

```python
# LessThanExpressionTypeDef definition

class LessThanExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## LessThanOrEqualToExpressionTypeDef

```python
# LessThanOrEqualToExpressionTypeDef definition

class LessThanOrEqualToExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## LikeExpressionTypeDef

```python
# LikeExpressionTypeDef definition

class LikeExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## LineageNodeSummaryTypeDef

```python
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

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAssetFiltersInputRequestTypeDef

```python
# ListAssetFiltersInputRequestTypeDef definition

class ListAssetFiltersInputRequestTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[FilterStatusType],  # (1)
```

1. See [:material-code-brackets: FilterStatusType](./literals.md#filterstatustype) 
## ListAssetRevisionsInputRequestTypeDef

```python
# ListAssetRevisionsInputRequestTypeDef definition

class ListAssetRevisionsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataProductRevisionsInputRequestTypeDef

```python
# ListDataProductRevisionsInputRequestTypeDef definition

class ListDataProductRevisionsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDataSourceRunActivitiesInputRequestTypeDef

```python
# ListDataSourceRunActivitiesInputRequestTypeDef definition

class ListDataSourceRunActivitiesInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[DataAssetActivityStatusType],  # (1)
```

1. See [:material-code-brackets: DataAssetActivityStatusType](./literals.md#dataassetactivitystatustype) 
## ListDataSourceRunsInputRequestTypeDef

```python
# ListDataSourceRunsInputRequestTypeDef definition

class ListDataSourceRunsInputRequestTypeDef(TypedDict):
    dataSourceIdentifier: str,
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[DataSourceRunStatusType],  # (1)
```

1. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
## ListDataSourcesInputRequestTypeDef

```python
# ListDataSourcesInputRequestTypeDef definition

class ListDataSourcesInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    environmentIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    status: NotRequired[DataSourceStatusType],  # (1)
    type: NotRequired[str],
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
## ListDomainUnitsForParentInputRequestTypeDef

```python
# ListDomainUnitsForParentInputRequestTypeDef definition

class ListDomainUnitsForParentInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    parentDomainUnitIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListDomainsInputRequestTypeDef

```python
# ListDomainsInputRequestTypeDef definition

class ListDomainsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[DomainStatusType],  # (1)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
## ListEntityOwnersInputRequestTypeDef

```python
# ListEntityOwnersInputRequestTypeDef definition

class ListEntityOwnersInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: DataZoneEntityTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: DataZoneEntityTypeType](./literals.md#datazoneentitytypetype) 
## ListEnvironmentActionsInputRequestTypeDef

```python
# ListEnvironmentActionsInputRequestTypeDef definition

class ListEnvironmentActionsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEnvironmentBlueprintConfigurationsInputRequestTypeDef

```python
# ListEnvironmentBlueprintConfigurationsInputRequestTypeDef definition

class ListEnvironmentBlueprintConfigurationsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListEnvironmentBlueprintsInputRequestTypeDef

```python
# ListEnvironmentBlueprintsInputRequestTypeDef definition

class ListEnvironmentBlueprintsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    managed: NotRequired[bool],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
```

## ListEnvironmentProfilesInputRequestTypeDef

```python
# ListEnvironmentProfilesInputRequestTypeDef definition

class ListEnvironmentProfilesInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    environmentBlueprintIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    projectIdentifier: NotRequired[str],
```

## ListEnvironmentsInputRequestTypeDef

```python
# ListEnvironmentsInputRequestTypeDef definition

class ListEnvironmentsInputRequestTypeDef(TypedDict):
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
## ListMetadataGenerationRunsInputRequestTypeDef

```python
# ListMetadataGenerationRunsInputRequestTypeDef definition

class ListMetadataGenerationRunsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    status: NotRequired[MetadataGenerationRunStatusType],  # (1)
    type: NotRequired[MetadataGenerationRunTypeType],  # (2)
```

1. See [:material-code-brackets: MetadataGenerationRunStatusType](./literals.md#metadatagenerationrunstatustype) 
2. See [:material-code-brackets: MetadataGenerationRunTypeType](./literals.md#metadatagenerationruntypetype) 
## ListPolicyGrantsInputRequestTypeDef

```python
# ListPolicyGrantsInputRequestTypeDef definition

class ListPolicyGrantsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TargetEntityTypeType,  # (1)
    policyType: ManagedPolicyTypeType,  # (2)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-brackets: TargetEntityTypeType](./literals.md#targetentitytypetype) 
2. See [:material-code-brackets: ManagedPolicyTypeType](./literals.md#managedpolicytypetype) 
## ListProjectMembershipsInputRequestTypeDef

```python
# ListProjectMembershipsInputRequestTypeDef definition

class ListProjectMembershipsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortFieldProjectType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SortFieldProjectType](./literals.md#sortfieldprojecttype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListProjectsInputRequestTypeDef

```python
# ListProjectsInputRequestTypeDef definition

class ListProjectsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    name: NotRequired[str],
    nextToken: NotRequired[str],
    userIdentifier: NotRequired[str],
```

## ListSubscriptionGrantsInputRequestTypeDef

```python
# ListSubscriptionGrantsInputRequestTypeDef definition

class ListSubscriptionGrantsInputRequestTypeDef(TypedDict):
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
## ListSubscriptionRequestsInputRequestTypeDef

```python
# ListSubscriptionRequestsInputRequestTypeDef definition

class ListSubscriptionRequestsInputRequestTypeDef(TypedDict):
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
## ListSubscriptionTargetsInputRequestTypeDef

```python
# ListSubscriptionTargetsInputRequestTypeDef definition

class ListSubscriptionTargetsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ListSubscriptionsInputRequestTypeDef

```python
# ListSubscriptionsInputRequestTypeDef definition

class ListSubscriptionsInputRequestTypeDef(TypedDict):
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
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## UserDetailsTypeDef

```python
# UserDetailsTypeDef definition

class UserDetailsTypeDef(TypedDict):
    userId: str,
```

## NotEqualToExpressionTypeDef

```python
# NotEqualToExpressionTypeDef definition

class NotEqualToExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## NotInExpressionOutputTypeDef

```python
# NotInExpressionOutputTypeDef definition

class NotInExpressionOutputTypeDef(TypedDict):
    columnName: str,
    values: List[str],
```

## NotInExpressionTypeDef

```python
# NotInExpressionTypeDef definition

class NotInExpressionTypeDef(TypedDict):
    columnName: str,
    values: Sequence[str],
```

## NotLikeExpressionTypeDef

```python
# NotLikeExpressionTypeDef definition

class NotLikeExpressionTypeDef(TypedDict):
    columnName: str,
    value: str,
```

## NotificationResourceTypeDef

```python
# NotificationResourceTypeDef definition

class NotificationResourceTypeDef(TypedDict):
    id: str,
    type: NotificationResourceTypeType,  # (1)
    name: NotRequired[str],
```

1. See [:material-code-brackets: NotificationResourceTypeType](./literals.md#notificationresourcetypetype) 
## OverrideDomainUnitOwnersPolicyGrantDetailTypeDef

```python
# OverrideDomainUnitOwnersPolicyGrantDetailTypeDef definition

class OverrideDomainUnitOwnersPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## OverrideProjectOwnersPolicyGrantDetailTypeDef

```python
# OverrideProjectOwnersPolicyGrantDetailTypeDef definition

class OverrideProjectOwnersPolicyGrantDetailTypeDef(TypedDict):
    includeChildDomainUnits: NotRequired[bool],
```

## OwnerGroupPropertiesOutputTypeDef

```python
# OwnerGroupPropertiesOutputTypeDef definition

class OwnerGroupPropertiesOutputTypeDef(TypedDict):
    groupId: NotRequired[str],
```

## OwnerGroupPropertiesTypeDef

```python
# OwnerGroupPropertiesTypeDef definition

class OwnerGroupPropertiesTypeDef(TypedDict):
    groupIdentifier: str,
```

## OwnerUserPropertiesOutputTypeDef

```python
# OwnerUserPropertiesOutputTypeDef definition

class OwnerUserPropertiesOutputTypeDef(TypedDict):
    userId: NotRequired[str],
```

## OwnerUserPropertiesTypeDef

```python
# OwnerUserPropertiesTypeDef definition

class OwnerUserPropertiesTypeDef(TypedDict):
    userIdentifier: str,
```

## UserPolicyGrantPrincipalOutputTypeDef

```python
# UserPolicyGrantPrincipalOutputTypeDef definition

class UserPolicyGrantPrincipalOutputTypeDef(TypedDict):
    allUsersGrantFilter: NotRequired[Dict[str, Any]],
    userIdentifier: NotRequired[str],
```

## RedshiftClusterStorageTypeDef

```python
# RedshiftClusterStorageTypeDef definition

class RedshiftClusterStorageTypeDef(TypedDict):
    clusterName: str,
```

## RedshiftCredentialConfigurationTypeDef

```python
# RedshiftCredentialConfigurationTypeDef definition

class RedshiftCredentialConfigurationTypeDef(TypedDict):
    secretManagerArn: str,
```

## RedshiftServerlessStorageTypeDef

```python
# RedshiftServerlessStorageTypeDef definition

class RedshiftServerlessStorageTypeDef(TypedDict):
    workgroupName: str,
```

## RejectChoiceTypeDef

```python
# RejectChoiceTypeDef definition

class RejectChoiceTypeDef(TypedDict):
    predictionTarget: str,
    predictionChoices: NotRequired[Sequence[int]],
```

## RejectRuleTypeDef

```python
# RejectRuleTypeDef definition

class RejectRuleTypeDef(TypedDict):
    rule: NotRequired[RejectRuleBehaviorType],  # (1)
    threshold: NotRequired[float],
```

1. See [:material-code-brackets: RejectRuleBehaviorType](./literals.md#rejectrulebehaviortype) 
## RejectSubscriptionRequestInputRequestTypeDef

```python
# RejectSubscriptionRequestInputRequestTypeDef definition

class RejectSubscriptionRequestInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    decisionComment: NotRequired[str],
```

## RevokeSubscriptionInputRequestTypeDef

```python
# RevokeSubscriptionInputRequestTypeDef definition

class RevokeSubscriptionInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    retainPermissions: NotRequired[bool],
```

## SearchGroupProfilesInputRequestTypeDef

```python
# SearchGroupProfilesInputRequestTypeDef definition

class SearchGroupProfilesInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    groupType: GroupSearchTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    searchText: NotRequired[str],
```

1. See [:material-code-brackets: GroupSearchTypeType](./literals.md#groupsearchtypetype) 
## SearchInItemTypeDef

```python
# SearchInItemTypeDef definition

class SearchInItemTypeDef(TypedDict):
    attribute: str,
```

## SearchSortTypeDef

```python
# SearchSortTypeDef definition

class SearchSortTypeDef(TypedDict):
    attribute: str,
    order: NotRequired[SortOrderType],  # (1)
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## SearchUserProfilesInputRequestTypeDef

```python
# SearchUserProfilesInputRequestTypeDef definition

class SearchUserProfilesInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    userType: UserSearchTypeType,  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    searchText: NotRequired[str],
```

1. See [:material-code-brackets: UserSearchTypeType](./literals.md#usersearchtypetype) 
## SsoUserProfileDetailsTypeDef

```python
# SsoUserProfileDetailsTypeDef definition

class SsoUserProfileDetailsTypeDef(TypedDict):
    firstName: NotRequired[str],
    lastName: NotRequired[str],
    username: NotRequired[str],
```

## StartDataSourceRunInputRequestTypeDef

```python
# StartDataSourceRunInputRequestTypeDef definition

class StartDataSourceRunInputRequestTypeDef(TypedDict):
    dataSourceIdentifier: str,
    domainIdentifier: str,
    clientToken: NotRequired[str],
```

## SubscribedProjectInputTypeDef

```python
# SubscribedProjectInputTypeDef definition

class SubscribedProjectInputTypeDef(TypedDict):
    identifier: NotRequired[str],
```

## SubscribedProjectTypeDef

```python
# SubscribedProjectTypeDef definition

class SubscribedProjectTypeDef(TypedDict):
    id: NotRequired[str],
    name: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateDomainUnitInputRequestTypeDef

```python
# UpdateDomainUnitInputRequestTypeDef definition

class UpdateDomainUnitInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    name: NotRequired[str],
```

## UpdateEnvironmentInputRequestTypeDef

```python
# UpdateEnvironmentInputRequestTypeDef definition

class UpdateEnvironmentInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    glossaryTerms: NotRequired[Sequence[str]],
    name: NotRequired[str],
```

## UpdateGlossaryInputRequestTypeDef

```python
# UpdateGlossaryInputRequestTypeDef definition

class UpdateGlossaryInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[GlossaryStatusType],  # (1)
```

1. See [:material-code-brackets: GlossaryStatusType](./literals.md#glossarystatustype) 
## UpdateGroupProfileInputRequestTypeDef

```python
# UpdateGroupProfileInputRequestTypeDef definition

class UpdateGroupProfileInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: str,
    status: GroupProfileStatusType,  # (1)
```

1. See [:material-code-brackets: GroupProfileStatusType](./literals.md#groupprofilestatustype) 
## UpdateProjectInputRequestTypeDef

```python
# UpdateProjectInputRequestTypeDef definition

class UpdateProjectInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    description: NotRequired[str],
    glossaryTerms: NotRequired[Sequence[str]],
    name: NotRequired[str],
```

## UpdateSubscriptionRequestInputRequestTypeDef

```python
# UpdateSubscriptionRequestInputRequestTypeDef definition

class UpdateSubscriptionRequestInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    requestReason: str,
```

## UpdateUserProfileInputRequestTypeDef

```python
# UpdateUserProfileInputRequestTypeDef definition

class UpdateUserProfileInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    status: UserProfileStatusType,  # (1)
    userIdentifier: str,
    type: NotRequired[UserProfileTypeType],  # (2)
```

1. See [:material-code-brackets: UserProfileStatusType](./literals.md#userprofilestatustype) 
2. See [:material-code-brackets: UserProfileTypeType](./literals.md#userprofiletypetype) 
## UserPolicyGrantPrincipalTypeDef

```python
# UserPolicyGrantPrincipalTypeDef definition

class UserPolicyGrantPrincipalTypeDef(TypedDict):
    allUsersGrantFilter: NotRequired[Mapping[str, Any]],
    userIdentifier: NotRequired[str],
```

## AcceptPredictionsInputRequestTypeDef

```python
# AcceptPredictionsInputRequestTypeDef definition

class AcceptPredictionsInputRequestTypeDef(TypedDict):
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
# CreateListingChangeSetOutputTypeDef definition

class CreateListingChangeSetOutputTypeDef(TypedDict):
    listingId: str,
    listingRevision: str,
    status: ListingStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ListingStatusType](./literals.md#listingstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDomainOutputTypeDef

```python
# DeleteDomainOutputTypeDef definition

class DeleteDomainOutputTypeDef(TypedDict):
    status: DomainStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEnvironmentCredentialsOutputTypeDef

```python
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
# GetIamPortalLoginUrlOutputTypeDef definition

class GetIamPortalLoginUrlOutputTypeDef(TypedDict):
    authCodeUrl: str,
    userProfileId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectPredictionsOutputTypeDef

```python
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
## AcceptSubscriptionRequestInputRequestTypeDef

```python
# AcceptSubscriptionRequestInputRequestTypeDef definition

class AcceptSubscriptionRequestInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    assetScopes: NotRequired[Sequence[AcceptedAssetScopeTypeDef]],  # (1)
    decisionComment: NotRequired[str],
```

1. See [:material-code-braces: AcceptedAssetScopeTypeDef](./type_defs.md#acceptedassetscopetypedef) 
## ActionParametersTypeDef

```python
# ActionParametersTypeDef definition

class ActionParametersTypeDef(TypedDict):
    awsConsoleLink: NotRequired[AwsConsoleLinkParametersTypeDef],  # (1)
```

1. See [:material-code-braces: AwsConsoleLinkParametersTypeDef](./type_defs.md#awsconsolelinkparameterstypedef) 
## ListAssetFiltersOutputTypeDef

```python
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
# AssetListingItemAdditionalAttributesTypeDef definition

class AssetListingItemAdditionalAttributesTypeDef(TypedDict):
    forms: NotRequired[str],
    latestTimeSeriesDataPointForms: NotRequired[List[TimeSeriesDataPointSummaryFormOutputTypeDef]],  # (1)
```

1. See [:material-code-braces: TimeSeriesDataPointSummaryFormOutputTypeDef](./type_defs.md#timeseriesdatapointsummaryformoutputtypedef) 
## ListTimeSeriesDataPointsOutputTypeDef

```python
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
# ListingSummaryItemTypeDef definition

class ListingSummaryItemTypeDef(TypedDict):
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (1)
    listingId: NotRequired[str],
    listingRevision: NotRequired[str],
```

1. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
## ListingSummaryTypeDef

```python
# ListingSummaryTypeDef definition

class ListingSummaryTypeDef(TypedDict):
    glossaryTerms: NotRequired[List[DetailedGlossaryTermTypeDef]],  # (1)
    listingId: NotRequired[str],
    listingRevision: NotRequired[str],
```

1. See [:material-code-braces: DetailedGlossaryTermTypeDef](./type_defs.md#detailedglossarytermtypedef) 
## SubscribedProductListingTypeDef

```python
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
## PostLineageEventInputRequestTypeDef

```python
# PostLineageEventInputRequestTypeDef definition

class PostLineageEventInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    event: BlobTypeDef,
    clientToken: NotRequired[str],
```

## PredictionConfigurationTypeDef

```python
# PredictionConfigurationTypeDef definition

class PredictionConfigurationTypeDef(TypedDict):
    businessNameGeneration: NotRequired[BusinessNameGenerationConfigurationTypeDef],  # (1)
```

1. See [:material-code-braces: BusinessNameGenerationConfigurationTypeDef](./type_defs.md#businessnamegenerationconfigurationtypedef) 
## ProvisioningPropertiesTypeDef

```python
# ProvisioningPropertiesTypeDef definition

class ProvisioningPropertiesTypeDef(TypedDict):
    cloudFormation: NotRequired[CloudFormationPropertiesTypeDef],  # (1)
```

1. See [:material-code-braces: CloudFormationPropertiesTypeDef](./type_defs.md#cloudformationpropertiestypedef) 
## ConfigurableEnvironmentActionTypeDef

```python
# ConfigurableEnvironmentActionTypeDef definition

class ConfigurableEnvironmentActionTypeDef(TypedDict):
    parameters: List[ConfigurableActionParameterTypeDef],  # (2)
    type: str,
    auth: NotRequired[ConfigurableActionTypeAuthorizationType],  # (1)
```

1. See [:material-code-brackets: ConfigurableActionTypeAuthorizationType](./literals.md#configurableactiontypeauthorizationtype) 
2. See [:material-code-braces: ConfigurableActionParameterTypeDef](./type_defs.md#configurableactionparametertypedef) 
## CreateAssetTypeInputRequestTypeDef

```python
# CreateAssetTypeInputRequestTypeDef definition

class CreateAssetTypeInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    formsInput: Mapping[str, FormEntryInputTypeDef],  # (1)
    name: str,
    owningProjectIdentifier: str,
    description: NotRequired[str],
```

1. See [:material-code-braces: FormEntryInputTypeDef](./type_defs.md#formentryinputtypedef) 
## CreateDataProductOutputTypeDef

```python
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
## CreateDataProductRevisionInputRequestTypeDef

```python
# CreateDataProductRevisionInputRequestTypeDef definition

class CreateDataProductRevisionInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    formsInput: NotRequired[Sequence[FormInputTypeDef]],  # (1)
    glossaryTerms: NotRequired[Sequence[str]],
    items: NotRequired[Sequence[DataProductItemTypeDef]],  # (2)
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: DataProductItemTypeDef](./type_defs.md#dataproductitemtypedef) 
## DataSourceRunActivityTypeDef

```python
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
    technicalDescription: NotRequired[str],
```

1. See [:material-code-brackets: DataAssetActivityStatusType](./literals.md#dataassetactivitystatustype) 
2. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
## DataSourceSummaryTypeDef

```python
# DataSourceSummaryTypeDef definition

class DataSourceSummaryTypeDef(TypedDict):
    dataSourceId: str,
    domainId: str,
    environmentId: str,
    name: str,
    status: DataSourceStatusType,  # (5)
    type: str,
    createdAt: NotRequired[datetime],
    enableSetting: NotRequired[EnableSettingType],  # (1)
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
## CreateDomainInputRequestTypeDef

```python
# CreateDomainInputRequestTypeDef definition

class CreateDomainInputRequestTypeDef(TypedDict):
    domainExecutionRole: str,
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    kmsKeyIdentifier: NotRequired[str],
    singleSignOn: NotRequired[SingleSignOnTypeDef],  # (1)
    tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
## CreateDomainOutputTypeDef

```python
# CreateDomainOutputTypeDef definition

class CreateDomainOutputTypeDef(TypedDict):
    arn: str,
    description: str,
    domainExecutionRole: str,
    id: str,
    kmsKeyIdentifier: str,
    name: str,
    portalUrl: str,
    rootDomainUnitId: str,
    singleSignOn: SingleSignOnTypeDef,  # (1)
    status: DomainStatusType,  # (2)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
2. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDomainOutputTypeDef

```python
# GetDomainOutputTypeDef definition

class GetDomainOutputTypeDef(TypedDict):
    arn: str,
    createdAt: datetime,
    description: str,
    domainExecutionRole: str,
    id: str,
    kmsKeyIdentifier: str,
    lastUpdatedAt: datetime,
    name: str,
    portalUrl: str,
    rootDomainUnitId: str,
    singleSignOn: SingleSignOnTypeDef,  # (1)
    status: DomainStatusType,  # (2)
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
2. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateDomainInputRequestTypeDef

```python
# UpdateDomainInputRequestTypeDef definition

class UpdateDomainInputRequestTypeDef(TypedDict):
    identifier: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
    domainExecutionRole: NotRequired[str],
    name: NotRequired[str],
    singleSignOn: NotRequired[SingleSignOnTypeDef],  # (1)
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
## UpdateDomainOutputTypeDef

```python
# UpdateDomainOutputTypeDef definition

class UpdateDomainOutputTypeDef(TypedDict):
    description: str,
    domainExecutionRole: str,
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    rootDomainUnitId: str,
    singleSignOn: SingleSignOnTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: SingleSignOnTypeDef](./type_defs.md#singlesignontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentInputRequestTypeDef

```python
# CreateEnvironmentInputRequestTypeDef definition

class CreateEnvironmentInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentProfileIdentifier: str,
    name: str,
    projectIdentifier: str,
    description: NotRequired[str],
    environmentAccountIdentifier: NotRequired[str],
    environmentAccountRegion: NotRequired[str],
    environmentBlueprintIdentifier: NotRequired[str],
    glossaryTerms: NotRequired[Sequence[str]],
    userParameters: NotRequired[Sequence[EnvironmentParameterTypeDef]],  # (1)
```

1. See [:material-code-braces: EnvironmentParameterTypeDef](./type_defs.md#environmentparametertypedef) 
## CreateEnvironmentProfileInputRequestTypeDef

```python
# CreateEnvironmentProfileInputRequestTypeDef definition

class CreateEnvironmentProfileInputRequestTypeDef(TypedDict):
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
## UpdateEnvironmentProfileInputRequestTypeDef

```python
# UpdateEnvironmentProfileInputRequestTypeDef definition

class UpdateEnvironmentProfileInputRequestTypeDef(TypedDict):
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
## CreateFormTypeInputRequestTypeDef

```python
# CreateFormTypeInputRequestTypeDef definition

class CreateFormTypeInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    model: ModelTypeDef,  # (1)
    name: str,
    owningProjectIdentifier: str,
    description: NotRequired[str],
    status: NotRequired[FormTypeStatusType],  # (2)
```

1. See [:material-code-braces: ModelTypeDef](./type_defs.md#modeltypedef) 
2. See [:material-code-brackets: FormTypeStatusType](./literals.md#formtypestatustype) 
## CreateGlossaryTermInputRequestTypeDef

```python
# CreateGlossaryTermInputRequestTypeDef definition

class CreateGlossaryTermInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    glossaryIdentifier: str,
    name: str,
    clientToken: NotRequired[str],
    longDescription: NotRequired[str],
    shortDescription: NotRequired[str],
    status: NotRequired[GlossaryTermStatusType],  # (1)
    termRelations: NotRequired[TermRelationsTypeDef],  # (2)
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsTypeDef](./type_defs.md#termrelationstypedef) 
## UpdateGlossaryTermInputRequestTypeDef

```python
# UpdateGlossaryTermInputRequestTypeDef definition

class UpdateGlossaryTermInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    glossaryIdentifier: NotRequired[str],
    longDescription: NotRequired[str],
    name: NotRequired[str],
    shortDescription: NotRequired[str],
    status: NotRequired[GlossaryTermStatusType],  # (1)
    termRelations: NotRequired[TermRelationsTypeDef],  # (2)
```

1. See [:material-code-brackets: GlossaryTermStatusType](./literals.md#glossarytermstatustype) 
2. See [:material-code-braces: TermRelationsTypeDef](./type_defs.md#termrelationstypedef) 
## CreateGlossaryTermOutputTypeDef

```python
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
## CreateProjectMembershipInputRequestTypeDef

```python
# CreateProjectMembershipInputRequestTypeDef definition

class CreateProjectMembershipInputRequestTypeDef(TypedDict):
    designation: UserDesignationType,  # (1)
    domainIdentifier: str,
    member: MemberTypeDef,  # (2)
    projectIdentifier: str,
```

1. See [:material-code-brackets: UserDesignationType](./literals.md#userdesignationtype) 
2. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
## DeleteProjectMembershipInputRequestTypeDef

```python
# DeleteProjectMembershipInputRequestTypeDef definition

class DeleteProjectMembershipInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    member: MemberTypeDef,  # (1)
    projectIdentifier: str,
```

1. See [:material-code-braces: MemberTypeDef](./type_defs.md#membertypedef) 
## CreateProjectOutputTypeDef

```python
# CreateProjectOutputTypeDef definition

class CreateProjectOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    failureReasons: List[ProjectDeletionErrorTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    projectStatus: ProjectStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProjectDeletionErrorTypeDef](./type_defs.md#projectdeletionerrortypedef) 
2. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProjectOutputTypeDef

```python
# GetProjectOutputTypeDef definition

class GetProjectOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    failureReasons: List[ProjectDeletionErrorTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    projectStatus: ProjectStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProjectDeletionErrorTypeDef](./type_defs.md#projectdeletionerrortypedef) 
2. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProjectSummaryTypeDef

```python
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
## UpdateProjectOutputTypeDef

```python
# UpdateProjectOutputTypeDef definition

class UpdateProjectOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    description: str,
    domainId: str,
    domainUnitId: str,
    failureReasons: List[ProjectDeletionErrorTypeDef],  # (1)
    glossaryTerms: List[str],
    id: str,
    lastUpdatedAt: datetime,
    name: str,
    projectStatus: ProjectStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProjectDeletionErrorTypeDef](./type_defs.md#projectdeletionerrortypedef) 
2. See [:material-code-brackets: ProjectStatusType](./literals.md#projectstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSubscriptionTargetInputRequestTypeDef

```python
# CreateSubscriptionTargetInputRequestTypeDef definition

class CreateSubscriptionTargetInputRequestTypeDef(TypedDict):
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
# SubscriptionTargetSummaryTypeDef definition

class SubscriptionTargetSummaryTypeDef(TypedDict):
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
    updatedAt: NotRequired[datetime],
    updatedBy: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTargetFormTypeDef](./type_defs.md#subscriptiontargetformtypedef) 
## UpdateSubscriptionTargetInputRequestTypeDef

```python
# UpdateSubscriptionTargetInputRequestTypeDef definition

class UpdateSubscriptionTargetInputRequestTypeDef(TypedDict):
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
# ListDataProductRevisionsOutputTypeDef definition

class ListDataProductRevisionsOutputTypeDef(TypedDict):
    items: List[DataProductRevisionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataProductRevisionTypeDef](./type_defs.md#dataproductrevisiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceRunSummaryTypeDef

```python
# DataSourceRunSummaryTypeDef definition

class DataSourceRunSummaryTypeDef(TypedDict):
    createdAt: datetime,
    dataSourceId: str,
    id: str,
    projectId: str,
    status: DataSourceRunStatusType,  # (3)
    type: DataSourceRunTypeType,  # (4)
    updatedAt: datetime,
    errorMessage: NotRequired[DataSourceErrorMessageTypeDef],  # (1)
    runStatisticsForAssets: NotRequired[RunStatisticsForAssetsTypeDef],  # (2)
    startedAt: NotRequired[datetime],
    stoppedAt: NotRequired[datetime],
```

1. See [:material-code-braces: DataSourceErrorMessageTypeDef](./type_defs.md#datasourceerrormessagetypedef) 
2. See [:material-code-braces: RunStatisticsForAssetsTypeDef](./type_defs.md#runstatisticsforassetstypedef) 
3. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
4. See [:material-code-brackets: DataSourceRunTypeType](./literals.md#datasourceruntypetype) 
## GetDataSourceRunOutputTypeDef

```python
# GetDataSourceRunOutputTypeDef definition

class GetDataSourceRunOutputTypeDef(TypedDict):
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
## StartDataSourceRunOutputTypeDef

```python
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
## ListDomainsOutputTypeDef

```python
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
# ProjectGrantFilterTypeDef definition

class ProjectGrantFilterTypeDef(TypedDict):
    domainUnitFilter: NotRequired[DomainUnitFilterForProjectTypeDef],  # (1)
```

1. See [:material-code-braces: DomainUnitFilterForProjectTypeDef](./type_defs.md#domainunitfilterforprojecttypedef) 
## DomainUnitPolicyGrantPrincipalOutputTypeDef

```python
# DomainUnitPolicyGrantPrincipalOutputTypeDef definition

class DomainUnitPolicyGrantPrincipalOutputTypeDef(TypedDict):
    domainUnitDesignation: DomainUnitDesignationType,  # (1)
    domainUnitGrantFilter: NotRequired[DomainUnitGrantFilterOutputTypeDef],  # (2)
    domainUnitIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: DomainUnitDesignationType](./literals.md#domainunitdesignationtype) 
2. See [:material-code-braces: DomainUnitGrantFilterOutputTypeDef](./type_defs.md#domainunitgrantfilteroutputtypedef) 
## DomainUnitOwnerPropertiesTypeDef

```python
# DomainUnitOwnerPropertiesTypeDef definition

class DomainUnitOwnerPropertiesTypeDef(TypedDict):
    group: NotRequired[DomainUnitGroupPropertiesTypeDef],  # (1)
    user: NotRequired[DomainUnitUserPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: DomainUnitGroupPropertiesTypeDef](./type_defs.md#domainunitgrouppropertiestypedef) 
2. See [:material-code-braces: DomainUnitUserPropertiesTypeDef](./type_defs.md#domainunituserpropertiestypedef) 
## ListDomainUnitsForParentOutputTypeDef

```python
# ListDomainUnitsForParentOutputTypeDef definition

class ListDomainUnitsForParentOutputTypeDef(TypedDict):
    items: List[DomainUnitSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DomainUnitSummaryTypeDef](./type_defs.md#domainunitsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentProfilesOutputTypeDef

```python
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
## UpdateSubscriptionGrantStatusInputRequestTypeDef

```python
# UpdateSubscriptionGrantStatusInputRequestTypeDef definition

class UpdateSubscriptionGrantStatusInputRequestTypeDef(TypedDict):
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
# FilterClausePaginatorTypeDef definition

class FilterClausePaginatorTypeDef(TypedDict):
    and: NotRequired[Sequence[Mapping[str, Any]]],
    filter: NotRequired[FilterTypeDef],  # (1)
    or: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## FilterClauseTypeDef

```python
# FilterClauseTypeDef definition

class FilterClauseTypeDef(TypedDict):
    and: NotRequired[Sequence[Mapping[str, Any]]],
    filter: NotRequired[FilterTypeDef],  # (1)
    or: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
## RelationalFilterConfigurationOutputTypeDef

```python
# RelationalFilterConfigurationOutputTypeDef definition

class RelationalFilterConfigurationOutputTypeDef(TypedDict):
    databaseName: str,
    filterExpressions: NotRequired[List[FilterExpressionTypeDef]],  # (1)
    schemaName: NotRequired[str],
```

1. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) 
## RelationalFilterConfigurationTypeDef

```python
# RelationalFilterConfigurationTypeDef definition

class RelationalFilterConfigurationTypeDef(TypedDict):
    databaseName: str,
    filterExpressions: NotRequired[Sequence[FilterExpressionTypeDef]],  # (1)
    schemaName: NotRequired[str],
```

1. See [:material-code-braces: FilterExpressionTypeDef](./type_defs.md#filterexpressiontypedef) 
## FormTypeDataTypeDef

```python
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
## GetLineageNodeInputRequestTypeDef

```python
# GetLineageNodeInputRequestTypeDef definition

class GetLineageNodeInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    eventTimestamp: NotRequired[TimestampTypeDef],
```

## ListLineageNodeHistoryInputRequestTypeDef

```python
# ListLineageNodeHistoryInputRequestTypeDef definition

class ListLineageNodeHistoryInputRequestTypeDef(TypedDict):
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
## ListNotificationsInputRequestTypeDef

```python
# ListNotificationsInputRequestTypeDef definition

class ListNotificationsInputRequestTypeDef(TypedDict):
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
## ListTimeSeriesDataPointsInputRequestTypeDef

```python
# ListTimeSeriesDataPointsInputRequestTypeDef definition

class ListTimeSeriesDataPointsInputRequestTypeDef(TypedDict):
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
## StartMetadataGenerationRunInputRequestTypeDef

```python
# StartMetadataGenerationRunInputRequestTypeDef definition

class StartMetadataGenerationRunInputRequestTypeDef(TypedDict):
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
# GlueSelfGrantStatusOutputTypeDef definition

class GlueSelfGrantStatusOutputTypeDef(TypedDict):
    selfGrantStatusDetails: List[SelfGrantStatusDetailTypeDef],  # (1)
```

1. See [:material-code-braces: SelfGrantStatusDetailTypeDef](./type_defs.md#selfgrantstatusdetailtypedef) 
## RedshiftSelfGrantStatusOutputTypeDef

```python
# RedshiftSelfGrantStatusOutputTypeDef definition

class RedshiftSelfGrantStatusOutputTypeDef(TypedDict):
    selfGrantStatusDetails: List[SelfGrantStatusDetailTypeDef],  # (1)
```

1. See [:material-code-braces: SelfGrantStatusDetailTypeDef](./type_defs.md#selfgrantstatusdetailtypedef) 
## GrantedEntityInputTypeDef

```python
# GrantedEntityInputTypeDef definition

class GrantedEntityInputTypeDef(TypedDict):
    listing: NotRequired[ListingRevisionInputTypeDef],  # (1)
```

1. See [:material-code-braces: ListingRevisionInputTypeDef](./type_defs.md#listingrevisioninputtypedef) 
## GrantedEntityTypeDef

```python
# GrantedEntityTypeDef definition

class GrantedEntityTypeDef(TypedDict):
    listing: NotRequired[ListingRevisionTypeDef],  # (1)
```

1. See [:material-code-braces: ListingRevisionTypeDef](./type_defs.md#listingrevisiontypedef) 
## SearchGroupProfilesOutputTypeDef

```python
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
# ProvisioningConfigurationOutputTypeDef definition

class ProvisioningConfigurationOutputTypeDef(TypedDict):
    lakeFormationConfiguration: NotRequired[LakeFormationConfigurationOutputTypeDef],  # (1)
```

1. See [:material-code-braces: LakeFormationConfigurationOutputTypeDef](./type_defs.md#lakeformationconfigurationoutputtypedef) 
## ListLineageNodeHistoryOutputTypeDef

```python
# ListLineageNodeHistoryOutputTypeDef definition

class ListLineageNodeHistoryOutputTypeDef(TypedDict):
    nodes: List[LineageNodeSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: LineageNodeSummaryTypeDef](./type_defs.md#lineagenodesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssetFiltersInputListAssetFiltersPaginateTypeDef

```python
# ListAssetFiltersInputListAssetFiltersPaginateTypeDef definition

class ListAssetFiltersInputListAssetFiltersPaginateTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    status: NotRequired[FilterStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: FilterStatusType](./literals.md#filterstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef

```python
# ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef definition

class ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataProductRevisionsInputListDataProductRevisionsPaginateTypeDef

```python
# ListDataProductRevisionsInputListDataProductRevisionsPaginateTypeDef definition

class ListDataProductRevisionsInputListDataProductRevisionsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef

```python
# ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef definition

class ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    status: NotRequired[DataAssetActivityStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataAssetActivityStatusType](./literals.md#dataassetactivitystatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef

```python
# ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef definition

class ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef(TypedDict):
    dataSourceIdentifier: str,
    domainIdentifier: str,
    status: NotRequired[DataSourceRunStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataSourceRunStatusType](./literals.md#datasourcerunstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataSourcesInputListDataSourcesPaginateTypeDef

```python
# ListDataSourcesInputListDataSourcesPaginateTypeDef definition

class ListDataSourcesInputListDataSourcesPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    environmentIdentifier: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[DataSourceStatusType],  # (1)
    type: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataSourceStatusType](./literals.md#datasourcestatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainUnitsForParentInputListDomainUnitsForParentPaginateTypeDef

```python
# ListDomainUnitsForParentInputListDomainUnitsForParentPaginateTypeDef definition

class ListDomainUnitsForParentInputListDomainUnitsForParentPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    parentDomainUnitIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDomainsInputListDomainsPaginateTypeDef

```python
# ListDomainsInputListDomainsPaginateTypeDef definition

class ListDomainsInputListDomainsPaginateTypeDef(TypedDict):
    status: NotRequired[DomainStatusType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DomainStatusType](./literals.md#domainstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEntityOwnersInputListEntityOwnersPaginateTypeDef

```python
# ListEntityOwnersInputListEntityOwnersPaginateTypeDef definition

class ListEntityOwnersInputListEntityOwnersPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: DataZoneEntityTypeType,  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: DataZoneEntityTypeType](./literals.md#datazoneentitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentActionsInputListEnvironmentActionsPaginateTypeDef

```python
# ListEnvironmentActionsInputListEnvironmentActionsPaginateTypeDef definition

class ListEnvironmentActionsInputListEnvironmentActionsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentBlueprintConfigurationsInputListEnvironmentBlueprintConfigurationsPaginateTypeDef

```python
# ListEnvironmentBlueprintConfigurationsInputListEnvironmentBlueprintConfigurationsPaginateTypeDef definition

class ListEnvironmentBlueprintConfigurationsInputListEnvironmentBlueprintConfigurationsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentBlueprintsInputListEnvironmentBlueprintsPaginateTypeDef

```python
# ListEnvironmentBlueprintsInputListEnvironmentBlueprintsPaginateTypeDef definition

class ListEnvironmentBlueprintsInputListEnvironmentBlueprintsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    managed: NotRequired[bool],
    name: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentProfilesInputListEnvironmentProfilesPaginateTypeDef

```python
# ListEnvironmentProfilesInputListEnvironmentProfilesPaginateTypeDef definition

class ListEnvironmentProfilesInputListEnvironmentProfilesPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    awsAccountId: NotRequired[str],
    awsAccountRegion: NotRequired[str],
    environmentBlueprintIdentifier: NotRequired[str],
    name: NotRequired[str],
    projectIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsInputListEnvironmentsPaginateTypeDef

```python
# ListEnvironmentsInputListEnvironmentsPaginateTypeDef definition

class ListEnvironmentsInputListEnvironmentsPaginateTypeDef(TypedDict):
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
## ListLineageNodeHistoryInputListLineageNodeHistoryPaginateTypeDef

```python
# ListLineageNodeHistoryInputListLineageNodeHistoryPaginateTypeDef definition

class ListLineageNodeHistoryInputListLineageNodeHistoryPaginateTypeDef(TypedDict):
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
## ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef

```python
# ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef definition

class ListMetadataGenerationRunsInputListMetadataGenerationRunsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    status: NotRequired[MetadataGenerationRunStatusType],  # (1)
    type: NotRequired[MetadataGenerationRunTypeType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: MetadataGenerationRunStatusType](./literals.md#metadatagenerationrunstatustype) 
2. See [:material-code-brackets: MetadataGenerationRunTypeType](./literals.md#metadatagenerationruntypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNotificationsInputListNotificationsPaginateTypeDef

```python
# ListNotificationsInputListNotificationsPaginateTypeDef definition

class ListNotificationsInputListNotificationsPaginateTypeDef(TypedDict):
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
## ListPolicyGrantsInputListPolicyGrantsPaginateTypeDef

```python
# ListPolicyGrantsInputListPolicyGrantsPaginateTypeDef definition

class ListPolicyGrantsInputListPolicyGrantsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TargetEntityTypeType,  # (1)
    policyType: ManagedPolicyTypeType,  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: TargetEntityTypeType](./literals.md#targetentitytypetype) 
2. See [:material-code-brackets: ManagedPolicyTypeType](./literals.md#managedpolicytypetype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef

```python
# ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef definition

class ListProjectMembershipsInputListProjectMembershipsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    projectIdentifier: str,
    sortBy: NotRequired[SortFieldProjectType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortFieldProjectType](./literals.md#sortfieldprojecttype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProjectsInputListProjectsPaginateTypeDef

```python
# ListProjectsInputListProjectsPaginateTypeDef definition

class ListProjectsInputListProjectsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    groupIdentifier: NotRequired[str],
    name: NotRequired[str],
    userIdentifier: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionGrantsInputListSubscriptionGrantsPaginateTypeDef

```python
# ListSubscriptionGrantsInputListSubscriptionGrantsPaginateTypeDef definition

class ListSubscriptionGrantsInputListSubscriptionGrantsPaginateTypeDef(TypedDict):
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
## ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef

```python
# ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef definition

class ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef(TypedDict):
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
## ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef

```python
# ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef definition

class ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    sortBy: NotRequired[SortKeyType],  # (1)
    sortOrder: NotRequired[SortOrderType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: SortKeyType](./literals.md#sortkeytype) 
2. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionsInputListSubscriptionsPaginateTypeDef

```python
# ListSubscriptionsInputListSubscriptionsPaginateTypeDef definition

class ListSubscriptionsInputListSubscriptionsPaginateTypeDef(TypedDict):
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
## ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef

```python
# ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef definition

class ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef(TypedDict):
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
## SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef

```python
# SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef definition

class SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    groupType: GroupSearchTypeType,  # (1)
    searchText: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: GroupSearchTypeType](./literals.md#groupsearchtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchUserProfilesInputSearchUserProfilesPaginateTypeDef

```python
# SearchUserProfilesInputSearchUserProfilesPaginateTypeDef definition

class SearchUserProfilesInputSearchUserProfilesPaginateTypeDef(TypedDict):
    domainIdentifier: str,
    userType: UserSearchTypeType,  # (1)
    searchText: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: UserSearchTypeType](./literals.md#usersearchtypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## MemberDetailsTypeDef

```python
# MemberDetailsTypeDef definition

class MemberDetailsTypeDef(TypedDict):
    group: NotRequired[GroupDetailsTypeDef],  # (1)
    user: NotRequired[UserDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: GroupDetailsTypeDef](./type_defs.md#groupdetailstypedef) 
2. See [:material-code-braces: UserDetailsTypeDef](./type_defs.md#userdetailstypedef) 
## RowFilterExpressionOutputTypeDef

```python
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
## TopicTypeDef

```python
# TopicTypeDef definition

class TopicTypeDef(TypedDict):
    resource: NotificationResourceTypeDef,  # (1)
    role: NotificationRoleType,  # (2)
    subject: str,
```

1. See [:material-code-braces: NotificationResourceTypeDef](./type_defs.md#notificationresourcetypedef) 
2. See [:material-code-brackets: NotificationRoleType](./literals.md#notificationroletype) 
## PolicyGrantDetailOutputTypeDef

```python
# PolicyGrantDetailOutputTypeDef definition

class PolicyGrantDetailOutputTypeDef(TypedDict):
    addToProjectMemberPool: NotRequired[AddToProjectMemberPoolPolicyGrantDetailTypeDef],  # (1)
    createAssetType: NotRequired[CreateAssetTypePolicyGrantDetailTypeDef],  # (2)
    createDomainUnit: NotRequired[CreateDomainUnitPolicyGrantDetailTypeDef],  # (3)
    createEnvironment: NotRequired[Dict[str, Any]],
    createEnvironmentProfile: NotRequired[CreateEnvironmentProfilePolicyGrantDetailTypeDef],  # (4)
    createFormType: NotRequired[CreateFormTypePolicyGrantDetailTypeDef],  # (5)
    createGlossary: NotRequired[CreateGlossaryPolicyGrantDetailTypeDef],  # (6)
    createProject: NotRequired[CreateProjectPolicyGrantDetailTypeDef],  # (7)
    delegateCreateEnvironmentProfile: NotRequired[Dict[str, Any]],
    overrideDomainUnitOwners: NotRequired[OverrideDomainUnitOwnersPolicyGrantDetailTypeDef],  # (8)
    overrideProjectOwners: NotRequired[OverrideProjectOwnersPolicyGrantDetailTypeDef],  # (9)
```

1. See [:material-code-braces: AddToProjectMemberPoolPolicyGrantDetailTypeDef](./type_defs.md#addtoprojectmemberpoolpolicygrantdetailtypedef) 
2. See [:material-code-braces: CreateAssetTypePolicyGrantDetailTypeDef](./type_defs.md#createassettypepolicygrantdetailtypedef) 
3. See [:material-code-braces: CreateDomainUnitPolicyGrantDetailTypeDef](./type_defs.md#createdomainunitpolicygrantdetailtypedef) 
4. See [:material-code-braces: CreateEnvironmentProfilePolicyGrantDetailTypeDef](./type_defs.md#createenvironmentprofilepolicygrantdetailtypedef) 
5. See [:material-code-braces: CreateFormTypePolicyGrantDetailTypeDef](./type_defs.md#createformtypepolicygrantdetailtypedef) 
6. See [:material-code-braces: CreateGlossaryPolicyGrantDetailTypeDef](./type_defs.md#createglossarypolicygrantdetailtypedef) 
7. See [:material-code-braces: CreateProjectPolicyGrantDetailTypeDef](./type_defs.md#createprojectpolicygrantdetailtypedef) 
8. See [:material-code-braces: OverrideDomainUnitOwnersPolicyGrantDetailTypeDef](./type_defs.md#overridedomainunitownerspolicygrantdetailtypedef) 
9. See [:material-code-braces: OverrideProjectOwnersPolicyGrantDetailTypeDef](./type_defs.md#overrideprojectownerspolicygrantdetailtypedef) 
## PolicyGrantDetailTypeDef

```python
# PolicyGrantDetailTypeDef definition

class PolicyGrantDetailTypeDef(TypedDict):
    addToProjectMemberPool: NotRequired[AddToProjectMemberPoolPolicyGrantDetailTypeDef],  # (1)
    createAssetType: NotRequired[CreateAssetTypePolicyGrantDetailTypeDef],  # (2)
    createDomainUnit: NotRequired[CreateDomainUnitPolicyGrantDetailTypeDef],  # (3)
    createEnvironment: NotRequired[Mapping[str, Any]],
    createEnvironmentProfile: NotRequired[CreateEnvironmentProfilePolicyGrantDetailTypeDef],  # (4)
    createFormType: NotRequired[CreateFormTypePolicyGrantDetailTypeDef],  # (5)
    createGlossary: NotRequired[CreateGlossaryPolicyGrantDetailTypeDef],  # (6)
    createProject: NotRequired[CreateProjectPolicyGrantDetailTypeDef],  # (7)
    delegateCreateEnvironmentProfile: NotRequired[Mapping[str, Any]],
    overrideDomainUnitOwners: NotRequired[OverrideDomainUnitOwnersPolicyGrantDetailTypeDef],  # (8)
    overrideProjectOwners: NotRequired[OverrideProjectOwnersPolicyGrantDetailTypeDef],  # (9)
```

1. See [:material-code-braces: AddToProjectMemberPoolPolicyGrantDetailTypeDef](./type_defs.md#addtoprojectmemberpoolpolicygrantdetailtypedef) 
2. See [:material-code-braces: CreateAssetTypePolicyGrantDetailTypeDef](./type_defs.md#createassettypepolicygrantdetailtypedef) 
3. See [:material-code-braces: CreateDomainUnitPolicyGrantDetailTypeDef](./type_defs.md#createdomainunitpolicygrantdetailtypedef) 
4. See [:material-code-braces: CreateEnvironmentProfilePolicyGrantDetailTypeDef](./type_defs.md#createenvironmentprofilepolicygrantdetailtypedef) 
5. See [:material-code-braces: CreateFormTypePolicyGrantDetailTypeDef](./type_defs.md#createformtypepolicygrantdetailtypedef) 
6. See [:material-code-braces: CreateGlossaryPolicyGrantDetailTypeDef](./type_defs.md#createglossarypolicygrantdetailtypedef) 
7. See [:material-code-braces: CreateProjectPolicyGrantDetailTypeDef](./type_defs.md#createprojectpolicygrantdetailtypedef) 
8. See [:material-code-braces: OverrideDomainUnitOwnersPolicyGrantDetailTypeDef](./type_defs.md#overridedomainunitownerspolicygrantdetailtypedef) 
9. See [:material-code-braces: OverrideProjectOwnersPolicyGrantDetailTypeDef](./type_defs.md#overrideprojectownerspolicygrantdetailtypedef) 
## OwnerPropertiesOutputTypeDef

```python
# OwnerPropertiesOutputTypeDef definition

class OwnerPropertiesOutputTypeDef(TypedDict):
    group: NotRequired[OwnerGroupPropertiesOutputTypeDef],  # (1)
    user: NotRequired[OwnerUserPropertiesOutputTypeDef],  # (2)
```

1. See [:material-code-braces: OwnerGroupPropertiesOutputTypeDef](./type_defs.md#ownergrouppropertiesoutputtypedef) 
2. See [:material-code-braces: OwnerUserPropertiesOutputTypeDef](./type_defs.md#owneruserpropertiesoutputtypedef) 
## OwnerPropertiesTypeDef

```python
# OwnerPropertiesTypeDef definition

class OwnerPropertiesTypeDef(TypedDict):
    group: NotRequired[OwnerGroupPropertiesTypeDef],  # (1)
    user: NotRequired[OwnerUserPropertiesTypeDef],  # (2)
```

1. See [:material-code-braces: OwnerGroupPropertiesTypeDef](./type_defs.md#ownergrouppropertiestypedef) 
2. See [:material-code-braces: OwnerUserPropertiesTypeDef](./type_defs.md#owneruserpropertiestypedef) 
## RedshiftStorageTypeDef

```python
# RedshiftStorageTypeDef definition

class RedshiftStorageTypeDef(TypedDict):
    redshiftClusterSource: NotRequired[RedshiftClusterStorageTypeDef],  # (1)
    redshiftServerlessSource: NotRequired[RedshiftServerlessStorageTypeDef],  # (2)
```

1. See [:material-code-braces: RedshiftClusterStorageTypeDef](./type_defs.md#redshiftclusterstoragetypedef) 
2. See [:material-code-braces: RedshiftServerlessStorageTypeDef](./type_defs.md#redshiftserverlessstoragetypedef) 
## RejectPredictionsInputRequestTypeDef

```python
# RejectPredictionsInputRequestTypeDef definition

class RejectPredictionsInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    identifier: str,
    clientToken: NotRequired[str],
    rejectChoices: NotRequired[Sequence[RejectChoiceTypeDef]],  # (1)
    rejectRule: NotRequired[RejectRuleTypeDef],  # (2)
    revision: NotRequired[str],
```

1. See [:material-code-braces: RejectChoiceTypeDef](./type_defs.md#rejectchoicetypedef) 
2. See [:material-code-braces: RejectRuleTypeDef](./type_defs.md#rejectruletypedef) 
## UserProfileDetailsTypeDef

```python
# UserProfileDetailsTypeDef definition

class UserProfileDetailsTypeDef(TypedDict):
    iam: NotRequired[IamUserProfileDetailsTypeDef],  # (1)
    sso: NotRequired[SsoUserProfileDetailsTypeDef],  # (2)
```

1. See [:material-code-braces: IamUserProfileDetailsTypeDef](./type_defs.md#iamuserprofiledetailstypedef) 
2. See [:material-code-braces: SsoUserProfileDetailsTypeDef](./type_defs.md#ssouserprofiledetailstypedef) 
## SubscribedPrincipalInputTypeDef

```python
# SubscribedPrincipalInputTypeDef definition

class SubscribedPrincipalInputTypeDef(TypedDict):
    project: NotRequired[SubscribedProjectInputTypeDef],  # (1)
```

1. See [:material-code-braces: SubscribedProjectInputTypeDef](./type_defs.md#subscribedprojectinputtypedef) 
## SubscribedPrincipalTypeDef

```python
# SubscribedPrincipalTypeDef definition

class SubscribedPrincipalTypeDef(TypedDict):
    project: NotRequired[SubscribedProjectTypeDef],  # (1)
```

1. See [:material-code-braces: SubscribedProjectTypeDef](./type_defs.md#subscribedprojecttypedef) 
## CreateEnvironmentActionInputRequestTypeDef

```python
# CreateEnvironmentActionInputRequestTypeDef definition

class CreateEnvironmentActionInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    name: str,
    parameters: ActionParametersTypeDef,  # (1)
    description: NotRequired[str],
```

1. See [:material-code-braces: ActionParametersTypeDef](./type_defs.md#actionparameterstypedef) 
## CreateEnvironmentActionOutputTypeDef

```python
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
## UpdateEnvironmentActionInputRequestTypeDef

```python
# UpdateEnvironmentActionInputRequestTypeDef definition

class UpdateEnvironmentActionInputRequestTypeDef(TypedDict):
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
# SubscribedListingItemTypeDef definition

class SubscribedListingItemTypeDef(TypedDict):
    assetListing: NotRequired[SubscribedAssetListingTypeDef],  # (1)
    productListing: NotRequired[SubscribedProductListingTypeDef],  # (2)
```

1. See [:material-code-braces: SubscribedAssetListingTypeDef](./type_defs.md#subscribedassetlistingtypedef) 
2. See [:material-code-braces: SubscribedProductListingTypeDef](./type_defs.md#subscribedproductlistingtypedef) 
## CreateAssetInputRequestTypeDef

```python
# CreateAssetInputRequestTypeDef definition

class CreateAssetInputRequestTypeDef(TypedDict):
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
## CreateAssetRevisionInputRequestTypeDef

```python
# CreateAssetRevisionInputRequestTypeDef definition

class CreateAssetRevisionInputRequestTypeDef(TypedDict):
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
## CreateDataProductInputRequestTypeDef

```python
# CreateDataProductInputRequestTypeDef definition

class CreateDataProductInputRequestTypeDef(TypedDict):
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
## ListDataSourceRunActivitiesOutputTypeDef

```python
# ListDataSourceRunActivitiesOutputTypeDef definition

class ListDataSourceRunActivitiesOutputTypeDef(TypedDict):
    items: List[DataSourceRunActivityTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DataSourceRunActivityTypeDef](./type_defs.md#datasourcerunactivitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSourcesOutputTypeDef

```python
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
# ListSubscriptionTargetsOutputTypeDef definition

class ListSubscriptionTargetsOutputTypeDef(TypedDict):
    items: List[SubscriptionTargetSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTargetSummaryTypeDef](./type_defs.md#subscriptiontargetsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataSourceRunsOutputTypeDef

```python
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
## ProjectPolicyGrantPrincipalTypeDef

```python
# ProjectPolicyGrantPrincipalTypeDef definition

class ProjectPolicyGrantPrincipalTypeDef(TypedDict):
    projectDesignation: ProjectDesignationType,  # (1)
    projectGrantFilter: NotRequired[ProjectGrantFilterTypeDef],  # (2)
    projectIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: ProjectDesignationType](./literals.md#projectdesignationtype) 
2. See [:material-code-braces: ProjectGrantFilterTypeDef](./type_defs.md#projectgrantfiltertypedef) 
## DomainUnitPolicyGrantPrincipalTypeDef

```python
# DomainUnitPolicyGrantPrincipalTypeDef definition

class DomainUnitPolicyGrantPrincipalTypeDef(TypedDict):
    domainUnitDesignation: DomainUnitDesignationType,  # (1)
    domainUnitGrantFilter: NotRequired[DomainUnitGrantFilterUnionTypeDef],  # (2)
    domainUnitIdentifier: NotRequired[str],
```

1. See [:material-code-brackets: DomainUnitDesignationType](./literals.md#domainunitdesignationtype) 
2. See [:material-code-braces: DomainUnitGrantFilterTypeDef](./type_defs.md#domainunitgrantfiltertypedef) [:material-code-braces: DomainUnitGrantFilterOutputTypeDef](./type_defs.md#domainunitgrantfilteroutputtypedef) 
## CreateDomainUnitOutputTypeDef

```python
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
## SearchInputSearchPaginateTypeDef

```python
# SearchInputSearchPaginateTypeDef definition

class SearchInputSearchPaginateTypeDef(TypedDict):
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
## SearchListingsInputSearchListingsPaginateTypeDef

```python
# SearchListingsInputSearchListingsPaginateTypeDef definition

class SearchListingsInputSearchListingsPaginateTypeDef(TypedDict):
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
## SearchTypesInputSearchTypesPaginateTypeDef

```python
# SearchTypesInputSearchTypesPaginateTypeDef definition

class SearchTypesInputSearchTypesPaginateTypeDef(TypedDict):
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
## SearchInputRequestTypeDef

```python
# SearchInputRequestTypeDef definition

class SearchInputRequestTypeDef(TypedDict):
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
## SearchListingsInputRequestTypeDef

```python
# SearchListingsInputRequestTypeDef definition

class SearchListingsInputRequestTypeDef(TypedDict):
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
## SearchTypesInputRequestTypeDef

```python
# SearchTypesInputRequestTypeDef definition

class SearchTypesInputRequestTypeDef(TypedDict):
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
# GlueRunConfigurationOutputTypeDef definition

class GlueRunConfigurationOutputTypeDef(TypedDict):
    relationalFilterConfigurations: List[RelationalFilterConfigurationOutputTypeDef],  # (1)
    accountId: NotRequired[str],
    autoImportDataQualityResult: NotRequired[bool],
    dataAccessRole: NotRequired[str],
    region: NotRequired[str],
```

1. See [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 
## SearchTypesResultItemTypeDef

```python
# SearchTypesResultItemTypeDef definition

class SearchTypesResultItemTypeDef(TypedDict):
    assetTypeItem: NotRequired[AssetTypeItemTypeDef],  # (1)
    formTypeItem: NotRequired[FormTypeDataTypeDef],  # (2)
    lineageNodeTypeItem: NotRequired[LineageNodeTypeItemTypeDef],  # (3)
```

1. See [:material-code-braces: AssetTypeItemTypeDef](./type_defs.md#assettypeitemtypedef) 
2. See [:material-code-braces: FormTypeDataTypeDef](./type_defs.md#formtypedatatypedef) 
3. See [:material-code-braces: LineageNodeTypeItemTypeDef](./type_defs.md#lineagenodetypeitemtypedef) 
## PostTimeSeriesDataPointsInputRequestTypeDef

```python
# PostTimeSeriesDataPointsInputRequestTypeDef definition

class PostTimeSeriesDataPointsInputRequestTypeDef(TypedDict):
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
# SelfGrantStatusOutputTypeDef definition

class SelfGrantStatusOutputTypeDef(TypedDict):
    glueSelfGrantStatus: NotRequired[GlueSelfGrantStatusOutputTypeDef],  # (1)
    redshiftSelfGrantStatus: NotRequired[RedshiftSelfGrantStatusOutputTypeDef],  # (2)
```

1. See [:material-code-braces: GlueSelfGrantStatusOutputTypeDef](./type_defs.md#glueselfgrantstatusoutputtypedef) 
2. See [:material-code-braces: RedshiftSelfGrantStatusOutputTypeDef](./type_defs.md#redshiftselfgrantstatusoutputtypedef) 
## CreateSubscriptionGrantInputRequestTypeDef

```python
# CreateSubscriptionGrantInputRequestTypeDef definition

class CreateSubscriptionGrantInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    grantedEntity: GrantedEntityInputTypeDef,  # (1)
    subscriptionTargetIdentifier: str,
    assetTargetNames: NotRequired[Sequence[AssetTargetNameMapTypeDef]],  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: GrantedEntityInputTypeDef](./type_defs.md#grantedentityinputtypedef) 
2. See [:material-code-braces: AssetTargetNameMapTypeDef](./type_defs.md#assettargetnamemaptypedef) 
## CreateSubscriptionGrantOutputTypeDef

```python
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
# EnvironmentBlueprintConfigurationItemTypeDef definition

class EnvironmentBlueprintConfigurationItemTypeDef(TypedDict):
    domainId: str,
    environmentBlueprintId: str,
    createdAt: NotRequired[datetime],
    enabledRegions: NotRequired[List[str]],
    manageAccessRoleArn: NotRequired[str],
    provisioningConfigurations: NotRequired[List[ProvisioningConfigurationOutputTypeDef]],  # (1)
    provisioningRoleArn: NotRequired[str],
    regionalParameters: NotRequired[Dict[str, Dict[str, str]]],
    updatedAt: NotRequired[datetime],
```

1. See [:material-code-braces: ProvisioningConfigurationOutputTypeDef](./type_defs.md#provisioningconfigurationoutputtypedef) 
## GetEnvironmentBlueprintConfigurationOutputTypeDef

```python
# GetEnvironmentBlueprintConfigurationOutputTypeDef definition

class GetEnvironmentBlueprintConfigurationOutputTypeDef(TypedDict):
    createdAt: datetime,
    domainId: str,
    enabledRegions: List[str],
    environmentBlueprintId: str,
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
# PutEnvironmentBlueprintConfigurationOutputTypeDef definition

class PutEnvironmentBlueprintConfigurationOutputTypeDef(TypedDict):
    createdAt: datetime,
    domainId: str,
    enabledRegions: List[str],
    environmentBlueprintId: str,
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
# ProvisioningConfigurationTypeDef definition

class ProvisioningConfigurationTypeDef(TypedDict):
    lakeFormationConfiguration: NotRequired[LakeFormationConfigurationUnionTypeDef],  # (1)
```

1. See [:material-code-braces: LakeFormationConfigurationTypeDef](./type_defs.md#lakeformationconfigurationtypedef) [:material-code-braces: LakeFormationConfigurationOutputTypeDef](./type_defs.md#lakeformationconfigurationoutputtypedef) 
## ProjectMemberTypeDef

```python
# ProjectMemberTypeDef definition

class ProjectMemberTypeDef(TypedDict):
    designation: UserDesignationType,  # (1)
    memberDetails: MemberDetailsTypeDef,  # (2)
```

1. See [:material-code-brackets: UserDesignationType](./literals.md#userdesignationtype) 
2. See [:material-code-braces: MemberDetailsTypeDef](./type_defs.md#memberdetailstypedef) 
## RowFilterExpressionTypeDef

```python
# RowFilterExpressionTypeDef definition

class RowFilterExpressionTypeDef(TypedDict):
    equalTo: NotRequired[EqualToExpressionTypeDef],  # (1)
    greaterThan: NotRequired[GreaterThanExpressionTypeDef],  # (2)
    greaterThanOrEqualTo: NotRequired[GreaterThanOrEqualToExpressionTypeDef],  # (3)
    in: NotRequired[InExpressionUnionTypeDef],  # (4)
    isNotNull: NotRequired[IsNotNullExpressionTypeDef],  # (5)
    isNull: NotRequired[IsNullExpressionTypeDef],  # (6)
    lessThan: NotRequired[LessThanExpressionTypeDef],  # (7)
    lessThanOrEqualTo: NotRequired[LessThanOrEqualToExpressionTypeDef],  # (8)
    like: NotRequired[LikeExpressionTypeDef],  # (9)
    notEqualTo: NotRequired[NotEqualToExpressionTypeDef],  # (10)
    notIn: NotRequired[NotInExpressionUnionTypeDef],  # (11)
    notLike: NotRequired[NotLikeExpressionTypeDef],  # (12)
```

1. See [:material-code-braces: EqualToExpressionTypeDef](./type_defs.md#equaltoexpressiontypedef) 
2. See [:material-code-braces: GreaterThanExpressionTypeDef](./type_defs.md#greaterthanexpressiontypedef) 
3. See [:material-code-braces: GreaterThanOrEqualToExpressionTypeDef](./type_defs.md#greaterthanorequaltoexpressiontypedef) 
4. See [:material-code-braces: InExpressionTypeDef](./type_defs.md#inexpressiontypedef) [:material-code-braces: InExpressionOutputTypeDef](./type_defs.md#inexpressionoutputtypedef) 
5. See [:material-code-braces: IsNotNullExpressionTypeDef](./type_defs.md#isnotnullexpressiontypedef) 
6. See [:material-code-braces: IsNullExpressionTypeDef](./type_defs.md#isnullexpressiontypedef) 
7. See [:material-code-braces: LessThanExpressionTypeDef](./type_defs.md#lessthanexpressiontypedef) 
8. See [:material-code-braces: LessThanOrEqualToExpressionTypeDef](./type_defs.md#lessthanorequaltoexpressiontypedef) 
9. See [:material-code-braces: LikeExpressionTypeDef](./type_defs.md#likeexpressiontypedef) 
10. See [:material-code-braces: NotEqualToExpressionTypeDef](./type_defs.md#notequaltoexpressiontypedef) 
11. See [:material-code-braces: NotInExpressionTypeDef](./type_defs.md#notinexpressiontypedef) [:material-code-braces: NotInExpressionOutputTypeDef](./type_defs.md#notinexpressionoutputtypedef) 
12. See [:material-code-braces: NotLikeExpressionTypeDef](./type_defs.md#notlikeexpressiontypedef) 
## RowFilterOutputTypeDef

```python
# RowFilterOutputTypeDef definition

class RowFilterOutputTypeDef(TypedDict):
    and: NotRequired[List[Dict[str, Any]]],
    expression: NotRequired[RowFilterExpressionOutputTypeDef],  # (1)
    or: NotRequired[List[Dict[str, Any]]],
```

1. See [:material-code-braces: RowFilterExpressionOutputTypeDef](./type_defs.md#rowfilterexpressionoutputtypedef) 
## NotificationOutputTypeDef

```python
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
## ListEntityOwnersOutputTypeDef

```python
# ListEntityOwnersOutputTypeDef definition

class ListEntityOwnersOutputTypeDef(TypedDict):
    owners: List[OwnerPropertiesOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OwnerPropertiesOutputTypeDef](./type_defs.md#ownerpropertiesoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddEntityOwnerInputRequestTypeDef

```python
# AddEntityOwnerInputRequestTypeDef definition

class AddEntityOwnerInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: DataZoneEntityTypeType,  # (1)
    owner: OwnerPropertiesTypeDef,  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: DataZoneEntityTypeType](./literals.md#datazoneentitytypetype) 
2. See [:material-code-braces: OwnerPropertiesTypeDef](./type_defs.md#ownerpropertiestypedef) 
## RemoveEntityOwnerInputRequestTypeDef

```python
# RemoveEntityOwnerInputRequestTypeDef definition

class RemoveEntityOwnerInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: DataZoneEntityTypeType,  # (1)
    owner: OwnerPropertiesTypeDef,  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: DataZoneEntityTypeType](./literals.md#datazoneentitytypetype) 
2. See [:material-code-braces: OwnerPropertiesTypeDef](./type_defs.md#ownerpropertiestypedef) 
## RedshiftRunConfigurationInputTypeDef

```python
# RedshiftRunConfigurationInputTypeDef definition

class RedshiftRunConfigurationInputTypeDef(TypedDict):
    redshiftCredentialConfiguration: RedshiftCredentialConfigurationTypeDef,  # (1)
    redshiftStorage: RedshiftStorageTypeDef,  # (2)
    relationalFilterConfigurations: Sequence[RelationalFilterConfigurationTypeDef],  # (3)
    dataAccessRole: NotRequired[str],
```

1. See [:material-code-braces: RedshiftCredentialConfigurationTypeDef](./type_defs.md#redshiftcredentialconfigurationtypedef) 
2. See [:material-code-braces: RedshiftStorageTypeDef](./type_defs.md#redshiftstoragetypedef) 
3. See [:material-code-braces: RelationalFilterConfigurationTypeDef](./type_defs.md#relationalfilterconfigurationtypedef) 
## RedshiftRunConfigurationOutputTypeDef

```python
# RedshiftRunConfigurationOutputTypeDef definition

class RedshiftRunConfigurationOutputTypeDef(TypedDict):
    redshiftCredentialConfiguration: RedshiftCredentialConfigurationTypeDef,  # (1)
    redshiftStorage: RedshiftStorageTypeDef,  # (2)
    relationalFilterConfigurations: List[RelationalFilterConfigurationOutputTypeDef],  # (3)
    accountId: NotRequired[str],
    dataAccessRole: NotRequired[str],
    region: NotRequired[str],
```

1. See [:material-code-braces: RedshiftCredentialConfigurationTypeDef](./type_defs.md#redshiftcredentialconfigurationtypedef) 
2. See [:material-code-braces: RedshiftStorageTypeDef](./type_defs.md#redshiftstoragetypedef) 
3. See [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 
## CreateUserProfileOutputTypeDef

```python
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
## CreateSubscriptionRequestInputRequestTypeDef

```python
# CreateSubscriptionRequestInputRequestTypeDef definition

class CreateSubscriptionRequestInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    requestReason: str,
    subscribedListings: Sequence[SubscribedListingInputTypeDef],  # (1)
    subscribedPrincipals: Sequence[SubscribedPrincipalInputTypeDef],  # (2)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: SubscribedListingInputTypeDef](./type_defs.md#subscribedlistinginputtypedef) 
2. See [:material-code-braces: SubscribedPrincipalInputTypeDef](./type_defs.md#subscribedprincipalinputtypedef) 
## ListEnvironmentActionsOutputTypeDef

```python
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
# SearchResultItemTypeDef definition

class SearchResultItemTypeDef(TypedDict):
    assetListing: NotRequired[AssetListingItemTypeDef],  # (1)
    dataProductListing: NotRequired[DataProductListingItemTypeDef],  # (2)
```

1. See [:material-code-braces: AssetListingItemTypeDef](./type_defs.md#assetlistingitemtypedef) 
2. See [:material-code-braces: DataProductListingItemTypeDef](./type_defs.md#dataproductlistingitemtypedef) 
## ListingItemTypeDef

```python
# ListingItemTypeDef definition

class ListingItemTypeDef(TypedDict):
    assetListing: NotRequired[AssetListingTypeDef],  # (1)
    dataProductListing: NotRequired[DataProductListingTypeDef],  # (2)
```

1. See [:material-code-braces: AssetListingTypeDef](./type_defs.md#assetlistingtypedef) 
2. See [:material-code-braces: DataProductListingTypeDef](./type_defs.md#dataproductlistingtypedef) 
## SubscribedListingTypeDef

```python
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
## ListEnvironmentBlueprintsOutputTypeDef

```python
# ListEnvironmentBlueprintsOutputTypeDef definition

class ListEnvironmentBlueprintsOutputTypeDef(TypedDict):
    items: List[EnvironmentBlueprintSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentBlueprintSummaryTypeDef](./type_defs.md#environmentblueprintsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyGrantPrincipalOutputTypeDef

```python
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
## GlueRunConfigurationInputTypeDef

```python
# GlueRunConfigurationInputTypeDef definition

class GlueRunConfigurationInputTypeDef(TypedDict):
    relationalFilterConfigurations: Sequence[RelationalFilterConfigurationUnionTypeDef],  # (1)
    autoImportDataQualityResult: NotRequired[bool],
    dataAccessRole: NotRequired[str],
```

1. See [:material-code-braces: RelationalFilterConfigurationTypeDef](./type_defs.md#relationalfilterconfigurationtypedef) [:material-code-braces: RelationalFilterConfigurationOutputTypeDef](./type_defs.md#relationalfilterconfigurationoutputtypedef) 
## SearchTypesOutputTypeDef

```python
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
# ListEnvironmentBlueprintConfigurationsOutputTypeDef definition

class ListEnvironmentBlueprintConfigurationsOutputTypeDef(TypedDict):
    items: List[EnvironmentBlueprintConfigurationItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentBlueprintConfigurationItemTypeDef](./type_defs.md#environmentblueprintconfigurationitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProjectMembershipsOutputTypeDef

```python
# ListProjectMembershipsOutputTypeDef definition

class ListProjectMembershipsOutputTypeDef(TypedDict):
    members: List[ProjectMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ProjectMemberTypeDef](./type_defs.md#projectmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RowFilterConfigurationOutputTypeDef

```python
# RowFilterConfigurationOutputTypeDef definition

class RowFilterConfigurationOutputTypeDef(TypedDict):
    rowFilter: RowFilterOutputTypeDef,  # (1)
    sensitive: NotRequired[bool],
```

1. See [:material-code-braces: RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef) 
## ListNotificationsOutputTypeDef

```python
# ListNotificationsOutputTypeDef definition

class ListNotificationsOutputTypeDef(TypedDict):
    notifications: List[NotificationOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: NotificationOutputTypeDef](./type_defs.md#notificationoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DataSourceConfigurationOutputTypeDef

```python
# DataSourceConfigurationOutputTypeDef definition

class DataSourceConfigurationOutputTypeDef(TypedDict):
    glueRunConfiguration: NotRequired[GlueRunConfigurationOutputTypeDef],  # (1)
    redshiftRunConfiguration: NotRequired[RedshiftRunConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: GlueRunConfigurationOutputTypeDef](./type_defs.md#gluerunconfigurationoutputtypedef) 
2. See [:material-code-braces: RedshiftRunConfigurationOutputTypeDef](./type_defs.md#redshiftrunconfigurationoutputtypedef) 
## SearchUserProfilesOutputTypeDef

```python
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
# AcceptSubscriptionRequestOutputTypeDef definition

class AcceptSubscriptionRequestOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    id: str,
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (1)
    subscribedListings: List[SubscribedListingTypeDef],  # (2)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (3)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CancelSubscriptionOutputTypeDef

```python
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
# CreateSubscriptionRequestOutputTypeDef definition

class CreateSubscriptionRequestOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    id: str,
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (1)
    subscribedListings: List[SubscribedListingTypeDef],  # (2)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (3)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionOutputTypeDef

```python
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
# GetSubscriptionRequestDetailsOutputTypeDef definition

class GetSubscriptionRequestDetailsOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    id: str,
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (1)
    subscribedListings: List[SubscribedListingTypeDef],  # (2)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (3)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectSubscriptionRequestOutputTypeDef

```python
# RejectSubscriptionRequestOutputTypeDef definition

class RejectSubscriptionRequestOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    id: str,
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (1)
    subscribedListings: List[SubscribedListingTypeDef],  # (2)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (3)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RevokeSubscriptionOutputTypeDef

```python
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
# SubscriptionRequestSummaryTypeDef definition

class SubscriptionRequestSummaryTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    domainId: str,
    id: str,
    requestReason: str,
    status: SubscriptionRequestStatusType,  # (1)
    subscribedListings: List[SubscribedListingTypeDef],  # (2)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (3)
    updatedAt: datetime,
    decisionComment: NotRequired[str],
    reviewerId: NotRequired[str],
    updatedBy: NotRequired[str],
```

1. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
## SubscriptionSummaryTypeDef

```python
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
# UpdateSubscriptionRequestOutputTypeDef definition

class UpdateSubscriptionRequestOutputTypeDef(TypedDict):
    createdAt: datetime,
    createdBy: str,
    decisionComment: str,
    domainId: str,
    id: str,
    requestReason: str,
    reviewerId: str,
    status: SubscriptionRequestStatusType,  # (1)
    subscribedListings: List[SubscribedListingTypeDef],  # (2)
    subscribedPrincipals: List[SubscribedPrincipalTypeDef],  # (3)
    updatedAt: datetime,
    updatedBy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: SubscriptionRequestStatusType](./literals.md#subscriptionrequeststatustype) 
2. See [:material-code-braces: SubscribedListingTypeDef](./type_defs.md#subscribedlistingtypedef) 
3. See [:material-code-braces: SubscribedPrincipalTypeDef](./type_defs.md#subscribedprincipaltypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PolicyGrantMemberTypeDef

```python
# PolicyGrantMemberTypeDef definition

class PolicyGrantMemberTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    detail: NotRequired[PolicyGrantDetailOutputTypeDef],  # (1)
    principal: NotRequired[PolicyGrantPrincipalOutputTypeDef],  # (2)
```

1. See [:material-code-braces: PolicyGrantDetailOutputTypeDef](./type_defs.md#policygrantdetailoutputtypedef) 
2. See [:material-code-braces: PolicyGrantPrincipalOutputTypeDef](./type_defs.md#policygrantprincipaloutputtypedef) 
## PolicyGrantPrincipalTypeDef

```python
# PolicyGrantPrincipalTypeDef definition

class PolicyGrantPrincipalTypeDef(TypedDict):
    domainUnit: NotRequired[DomainUnitPolicyGrantPrincipalUnionTypeDef],  # (1)
    group: NotRequired[GroupPolicyGrantPrincipalTypeDef],  # (2)
    project: NotRequired[ProjectPolicyGrantPrincipalTypeDef],  # (3)
    user: NotRequired[UserPolicyGrantPrincipalUnionTypeDef],  # (4)
```

1. See [:material-code-braces: DomainUnitPolicyGrantPrincipalTypeDef](./type_defs.md#domainunitpolicygrantprincipaltypedef) [:material-code-braces: DomainUnitPolicyGrantPrincipalOutputTypeDef](./type_defs.md#domainunitpolicygrantprincipaloutputtypedef) 
2. See [:material-code-braces: GroupPolicyGrantPrincipalTypeDef](./type_defs.md#grouppolicygrantprincipaltypedef) 
3. See [:material-code-braces: ProjectPolicyGrantPrincipalTypeDef](./type_defs.md#projectpolicygrantprincipaltypedef) 
4. See [:material-code-braces: UserPolicyGrantPrincipalTypeDef](./type_defs.md#userpolicygrantprincipaltypedef) [:material-code-braces: UserPolicyGrantPrincipalOutputTypeDef](./type_defs.md#userpolicygrantprincipaloutputtypedef) 
## DataSourceConfigurationInputTypeDef

```python
# DataSourceConfigurationInputTypeDef definition

class DataSourceConfigurationInputTypeDef(TypedDict):
    glueRunConfiguration: NotRequired[GlueRunConfigurationInputTypeDef],  # (1)
    redshiftRunConfiguration: NotRequired[RedshiftRunConfigurationInputTypeDef],  # (2)
```

1. See [:material-code-braces: GlueRunConfigurationInputTypeDef](./type_defs.md#gluerunconfigurationinputtypedef) 
2. See [:material-code-braces: RedshiftRunConfigurationInputTypeDef](./type_defs.md#redshiftrunconfigurationinputtypedef) 
## PutEnvironmentBlueprintConfigurationInputRequestTypeDef

```python
# PutEnvironmentBlueprintConfigurationInputRequestTypeDef definition

class PutEnvironmentBlueprintConfigurationInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    enabledRegions: Sequence[str],
    environmentBlueprintIdentifier: str,
    manageAccessRoleArn: NotRequired[str],
    provisioningConfigurations: NotRequired[Sequence[ProvisioningConfigurationUnionTypeDef]],  # (1)
    provisioningRoleArn: NotRequired[str],
    regionalParameters: NotRequired[Mapping[str, Mapping[str, str]]],
```

1. See [:material-code-braces: ProvisioningConfigurationTypeDef](./type_defs.md#provisioningconfigurationtypedef) [:material-code-braces: ProvisioningConfigurationOutputTypeDef](./type_defs.md#provisioningconfigurationoutputtypedef) 
## RowFilterTypeDef

```python
# RowFilterTypeDef definition

class RowFilterTypeDef(TypedDict):
    and: NotRequired[Sequence[Mapping[str, Any]]],
    expression: NotRequired[RowFilterExpressionUnionTypeDef],  # (1)
    or: NotRequired[Sequence[Mapping[str, Any]]],
```

1. See [:material-code-braces: RowFilterExpressionTypeDef](./type_defs.md#rowfilterexpressiontypedef) [:material-code-braces: RowFilterExpressionOutputTypeDef](./type_defs.md#rowfilterexpressionoutputtypedef) 
## AssetFilterConfigurationOutputTypeDef

```python
# AssetFilterConfigurationOutputTypeDef definition

class AssetFilterConfigurationOutputTypeDef(TypedDict):
    columnConfiguration: NotRequired[ColumnFilterConfigurationOutputTypeDef],  # (1)
    rowConfiguration: NotRequired[RowFilterConfigurationOutputTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnFilterConfigurationOutputTypeDef](./type_defs.md#columnfilterconfigurationoutputtypedef) 
2. See [:material-code-braces: RowFilterConfigurationOutputTypeDef](./type_defs.md#rowfilterconfigurationoutputtypedef) 
## CreateDataSourceOutputTypeDef

```python
# CreateDataSourceOutputTypeDef definition

class CreateDataSourceOutputTypeDef(TypedDict):
    assetFormsOutput: List[FormOutputTypeDef],  # (1)
    configuration: DataSourceConfigurationOutputTypeDef,  # (2)
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
# DeleteDataSourceOutputTypeDef definition

class DeleteDataSourceOutputTypeDef(TypedDict):
    assetFormsOutput: List[FormOutputTypeDef],  # (1)
    configuration: DataSourceConfigurationOutputTypeDef,  # (2)
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
# GetDataSourceOutputTypeDef definition

class GetDataSourceOutputTypeDef(TypedDict):
    assetFormsOutput: List[FormOutputTypeDef],  # (1)
    configuration: DataSourceConfigurationOutputTypeDef,  # (2)
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
# UpdateDataSourceOutputTypeDef definition

class UpdateDataSourceOutputTypeDef(TypedDict):
    assetFormsOutput: List[FormOutputTypeDef],  # (1)
    configuration: DataSourceConfigurationOutputTypeDef,  # (2)
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
# ListSubscriptionsOutputTypeDef definition

class ListSubscriptionsOutputTypeDef(TypedDict):
    items: List[SubscriptionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionSummaryTypeDef](./type_defs.md#subscriptionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPolicyGrantsOutputTypeDef

```python
# ListPolicyGrantsOutputTypeDef definition

class ListPolicyGrantsOutputTypeDef(TypedDict):
    grantList: List[PolicyGrantMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyGrantMemberTypeDef](./type_defs.md#policygrantmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AddPolicyGrantInputRequestTypeDef

```python
# AddPolicyGrantInputRequestTypeDef definition

class AddPolicyGrantInputRequestTypeDef(TypedDict):
    detail: PolicyGrantDetailTypeDef,  # (1)
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TargetEntityTypeType,  # (2)
    policyType: ManagedPolicyTypeType,  # (3)
    principal: PolicyGrantPrincipalTypeDef,  # (4)
    clientToken: NotRequired[str],
```

1. See [:material-code-braces: PolicyGrantDetailTypeDef](./type_defs.md#policygrantdetailtypedef) 
2. See [:material-code-brackets: TargetEntityTypeType](./literals.md#targetentitytypetype) 
3. See [:material-code-brackets: ManagedPolicyTypeType](./literals.md#managedpolicytypetype) 
4. See [:material-code-braces: PolicyGrantPrincipalTypeDef](./type_defs.md#policygrantprincipaltypedef) 
## RemovePolicyGrantInputRequestTypeDef

```python
# RemovePolicyGrantInputRequestTypeDef definition

class RemovePolicyGrantInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    entityIdentifier: str,
    entityType: TargetEntityTypeType,  # (1)
    policyType: ManagedPolicyTypeType,  # (2)
    principal: PolicyGrantPrincipalTypeDef,  # (3)
    clientToken: NotRequired[str],
```

1. See [:material-code-brackets: TargetEntityTypeType](./literals.md#targetentitytypetype) 
2. See [:material-code-brackets: ManagedPolicyTypeType](./literals.md#managedpolicytypetype) 
3. See [:material-code-braces: PolicyGrantPrincipalTypeDef](./type_defs.md#policygrantprincipaltypedef) 
## CreateDataSourceInputRequestTypeDef

```python
# CreateDataSourceInputRequestTypeDef definition

class CreateDataSourceInputRequestTypeDef(TypedDict):
    domainIdentifier: str,
    environmentIdentifier: str,
    name: str,
    projectIdentifier: str,
    type: str,
    assetFormsInput: NotRequired[Sequence[FormInputTypeDef]],  # (1)
    clientToken: NotRequired[str],
    configuration: NotRequired[DataSourceConfigurationInputTypeDef],  # (2)
    description: NotRequired[str],
    enableSetting: NotRequired[EnableSettingType],  # (3)
    publishOnImport: NotRequired[bool],
    recommendation: NotRequired[RecommendationConfigurationTypeDef],  # (4)
    schedule: NotRequired[ScheduleConfigurationTypeDef],  # (5)
```

1. See [:material-code-braces: FormInputTypeDef](./type_defs.md#forminputtypedef) 
2. See [:material-code-braces: DataSourceConfigurationInputTypeDef](./type_defs.md#datasourceconfigurationinputtypedef) 
3. See [:material-code-brackets: EnableSettingType](./literals.md#enablesettingtype) 
4. See [:material-code-braces: RecommendationConfigurationTypeDef](./type_defs.md#recommendationconfigurationtypedef) 
5. See [:material-code-braces: ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef) 
## UpdateDataSourceInputRequestTypeDef

```python
# UpdateDataSourceInputRequestTypeDef definition

class UpdateDataSourceInputRequestTypeDef(TypedDict):
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
## RowFilterConfigurationTypeDef

```python
# RowFilterConfigurationTypeDef definition

class RowFilterConfigurationTypeDef(TypedDict):
    rowFilter: RowFilterUnionTypeDef,  # (1)
    sensitive: NotRequired[bool],
```

1. See [:material-code-braces: RowFilterTypeDef](./type_defs.md#rowfiltertypedef) [:material-code-braces: RowFilterOutputTypeDef](./type_defs.md#rowfilteroutputtypedef) 
## AssetFilterConfigurationTypeDef

```python
# AssetFilterConfigurationTypeDef definition

class AssetFilterConfigurationTypeDef(TypedDict):
    columnConfiguration: NotRequired[ColumnFilterConfigurationUnionTypeDef],  # (1)
    rowConfiguration: NotRequired[RowFilterConfigurationUnionTypeDef],  # (2)
```

1. See [:material-code-braces: ColumnFilterConfigurationTypeDef](./type_defs.md#columnfilterconfigurationtypedef) [:material-code-braces: ColumnFilterConfigurationOutputTypeDef](./type_defs.md#columnfilterconfigurationoutputtypedef) 
2. See [:material-code-braces: RowFilterConfigurationTypeDef](./type_defs.md#rowfilterconfigurationtypedef) [:material-code-braces: RowFilterConfigurationOutputTypeDef](./type_defs.md#rowfilterconfigurationoutputtypedef) 
## CreateAssetFilterInputRequestTypeDef

```python
# CreateAssetFilterInputRequestTypeDef definition

class CreateAssetFilterInputRequestTypeDef(TypedDict):
    assetIdentifier: str,
    configuration: AssetFilterConfigurationTypeDef,  # (1)
    domainIdentifier: str,
    name: str,
    clientToken: NotRequired[str],
    description: NotRequired[str],
```

1. See [:material-code-braces: AssetFilterConfigurationTypeDef](./type_defs.md#assetfilterconfigurationtypedef) 
## UpdateAssetFilterInputRequestTypeDef

```python
# UpdateAssetFilterInputRequestTypeDef definition

class UpdateAssetFilterInputRequestTypeDef(TypedDict):
    assetIdentifier: str,
    domainIdentifier: str,
    identifier: str,
    configuration: NotRequired[AssetFilterConfigurationTypeDef],  # (1)
    description: NotRequired[str],
    name: NotRequired[str],
```

1. See [:material-code-braces: AssetFilterConfigurationTypeDef](./type_defs.md#assetfilterconfigurationtypedef) 

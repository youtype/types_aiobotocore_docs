# Type definitions

> [Index](../README.md) > [ServiceCatalog](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [ServiceCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
    type annotations stubs module [types-aiobotocore-servicecatalog](https://pypi.org/project/types-aiobotocore-servicecatalog/).



## AcceptPortfolioShareInputRequestTypeDef

```python
# AcceptPortfolioShareInputRequestTypeDef definition

class AcceptPortfolioShareInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    PortfolioShareType: NotRequired[PortfolioShareTypeType],  # (1)
```

1. See [:material-code-brackets: PortfolioShareTypeType](./literals.md#portfoliosharetypetype) 
## AccessLevelFilterTypeDef

```python
# AccessLevelFilterTypeDef definition

class AccessLevelFilterTypeDef(TypedDict):
    Key: NotRequired[AccessLevelFilterKeyType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: AccessLevelFilterKeyType](./literals.md#accesslevelfilterkeytype) 
## AssociateBudgetWithResourceInputRequestTypeDef

```python
# AssociateBudgetWithResourceInputRequestTypeDef definition

class AssociateBudgetWithResourceInputRequestTypeDef(TypedDict):
    BudgetName: str,
    ResourceId: str,
```

## AssociatePrincipalWithPortfolioInputRequestTypeDef

```python
# AssociatePrincipalWithPortfolioInputRequestTypeDef definition

class AssociatePrincipalWithPortfolioInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    PrincipalARN: str,
    PrincipalType: PrincipalTypeType,  # (1)
    AcceptLanguage: NotRequired[str],
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## AssociateProductWithPortfolioInputRequestTypeDef

```python
# AssociateProductWithPortfolioInputRequestTypeDef definition

class AssociateProductWithPortfolioInputRequestTypeDef(TypedDict):
    ProductId: str,
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    SourcePortfolioId: NotRequired[str],
```

## AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef

```python
# AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef definition

class AssociateServiceActionWithProvisioningArtifactInputRequestTypeDef(TypedDict):
    ProductId: str,
    ProvisioningArtifactId: str,
    ServiceActionId: str,
    AcceptLanguage: NotRequired[str],
    IdempotencyToken: NotRequired[str],
```

## AssociateTagOptionWithResourceInputRequestTypeDef

```python
# AssociateTagOptionWithResourceInputRequestTypeDef definition

class AssociateTagOptionWithResourceInputRequestTypeDef(TypedDict):
    ResourceId: str,
    TagOptionId: str,
```

## ServiceActionAssociationTypeDef

```python
# ServiceActionAssociationTypeDef definition

class ServiceActionAssociationTypeDef(TypedDict):
    ServiceActionId: str,
    ProductId: str,
    ProvisioningArtifactId: str,
```

## FailedServiceActionAssociationTypeDef

```python
# FailedServiceActionAssociationTypeDef definition

class FailedServiceActionAssociationTypeDef(TypedDict):
    ServiceActionId: NotRequired[str],
    ProductId: NotRequired[str],
    ProvisioningArtifactId: NotRequired[str],
    ErrorCode: NotRequired[ServiceActionAssociationErrorCodeType],  # (1)
    ErrorMessage: NotRequired[str],
```

1. See [:material-code-brackets: ServiceActionAssociationErrorCodeType](./literals.md#serviceactionassociationerrorcodetype) 
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

## BudgetDetailTypeDef

```python
# BudgetDetailTypeDef definition

class BudgetDetailTypeDef(TypedDict):
    BudgetName: NotRequired[str],
```

## CloudWatchDashboardTypeDef

```python
# CloudWatchDashboardTypeDef definition

class CloudWatchDashboardTypeDef(TypedDict):
    Name: NotRequired[str],
```

## CodeStarParametersTypeDef

```python
# CodeStarParametersTypeDef definition

class CodeStarParametersTypeDef(TypedDict):
    ConnectionArn: str,
    Repository: str,
    Branch: str,
    ArtifactPath: str,
```

## ConstraintDetailTypeDef

```python
# ConstraintDetailTypeDef definition

class ConstraintDetailTypeDef(TypedDict):
    ConstraintId: NotRequired[str],
    Type: NotRequired[str],
    Description: NotRequired[str],
    Owner: NotRequired[str],
    ProductId: NotRequired[str],
    PortfolioId: NotRequired[str],
```

## ConstraintSummaryTypeDef

```python
# ConstraintSummaryTypeDef definition

class ConstraintSummaryTypeDef(TypedDict):
    Type: NotRequired[str],
    Description: NotRequired[str],
```

## CopyProductInputRequestTypeDef

```python
# CopyProductInputRequestTypeDef definition

class CopyProductInputRequestTypeDef(TypedDict):
    SourceProductArn: str,
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
    TargetProductId: NotRequired[str],
    TargetProductName: NotRequired[str],
    SourceProvisioningArtifactIdentifiers: NotRequired[Sequence[Mapping[ProvisioningArtifactPropertyNameType, str]]],  # (1)
    CopyOptions: NotRequired[Sequence[CopyOptionType]],  # (2)
```

1. See [:material-code-brackets: ProvisioningArtifactPropertyNameType](./literals.md#provisioningartifactpropertynametype) 
2. See [:material-code-brackets: CopyOptionType](./literals.md#copyoptiontype) 
## CreateConstraintInputRequestTypeDef

```python
# CreateConstraintInputRequestTypeDef definition

class CreateConstraintInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    ProductId: str,
    Parameters: str,
    Type: str,
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
    Description: NotRequired[str],
```

## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## PortfolioDetailTypeDef

```python
# PortfolioDetailTypeDef definition

class PortfolioDetailTypeDef(TypedDict):
    Id: NotRequired[str],
    ARN: NotRequired[str],
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    ProviderName: NotRequired[str],
```

## OrganizationNodeTypeDef

```python
# OrganizationNodeTypeDef definition

class OrganizationNodeTypeDef(TypedDict):
    Type: NotRequired[OrganizationNodeTypeType],  # (1)
    Value: NotRequired[str],
```

1. See [:material-code-brackets: OrganizationNodeTypeType](./literals.md#organizationnodetypetype) 
## ProvisioningArtifactPropertiesTypeDef

```python
# ProvisioningArtifactPropertiesTypeDef definition

class ProvisioningArtifactPropertiesTypeDef(TypedDict):
    Name: NotRequired[str],
    Description: NotRequired[str],
    Info: NotRequired[Mapping[str, str]],
    Type: NotRequired[ProvisioningArtifactTypeType],  # (1)
    DisableTemplateValidation: NotRequired[bool],
```

1. See [:material-code-brackets: ProvisioningArtifactTypeType](./literals.md#provisioningartifacttypetype) 
## ProvisioningArtifactDetailTypeDef

```python
# ProvisioningArtifactDetailTypeDef definition

class ProvisioningArtifactDetailTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Type: NotRequired[ProvisioningArtifactTypeType],  # (1)
    CreatedTime: NotRequired[datetime],
    Active: NotRequired[bool],
    Guidance: NotRequired[ProvisioningArtifactGuidanceType],  # (2)
    SourceRevision: NotRequired[str],
```

1. See [:material-code-brackets: ProvisioningArtifactTypeType](./literals.md#provisioningartifacttypetype) 
2. See [:material-code-brackets: ProvisioningArtifactGuidanceType](./literals.md#provisioningartifactguidancetype) 
## UpdateProvisioningParameterTypeDef

```python
# UpdateProvisioningParameterTypeDef definition

class UpdateProvisioningParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    UsePreviousValue: NotRequired[bool],
```

## CreateServiceActionInputRequestTypeDef

```python
# CreateServiceActionInputRequestTypeDef definition

class CreateServiceActionInputRequestTypeDef(TypedDict):
    Name: str,
    DefinitionType: ServiceActionDefinitionTypeType,  # (1)
    Definition: Mapping[ServiceActionDefinitionKeyType, str],  # (2)
    IdempotencyToken: str,
    Description: NotRequired[str],
    AcceptLanguage: NotRequired[str],
```

1. See [:material-code-brackets: ServiceActionDefinitionTypeType](./literals.md#serviceactiondefinitiontypetype) 
2. See [:material-code-brackets: ServiceActionDefinitionKeyType](./literals.md#serviceactiondefinitionkeytype) 
## CreateTagOptionInputRequestTypeDef

```python
# CreateTagOptionInputRequestTypeDef definition

class CreateTagOptionInputRequestTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## TagOptionDetailTypeDef

```python
# TagOptionDetailTypeDef definition

class TagOptionDetailTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    Active: NotRequired[bool],
    Id: NotRequired[str],
    Owner: NotRequired[str],
```

## DeleteConstraintInputRequestTypeDef

```python
# DeleteConstraintInputRequestTypeDef definition

class DeleteConstraintInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
```

## DeletePortfolioInputRequestTypeDef

```python
# DeletePortfolioInputRequestTypeDef definition

class DeletePortfolioInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
```

## DeleteProductInputRequestTypeDef

```python
# DeleteProductInputRequestTypeDef definition

class DeleteProductInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
```

## DeleteProvisionedProductPlanInputRequestTypeDef

```python
# DeleteProvisionedProductPlanInputRequestTypeDef definition

class DeleteProvisionedProductPlanInputRequestTypeDef(TypedDict):
    PlanId: str,
    AcceptLanguage: NotRequired[str],
    IgnoreErrors: NotRequired[bool],
```

## DeleteProvisioningArtifactInputRequestTypeDef

```python
# DeleteProvisioningArtifactInputRequestTypeDef definition

class DeleteProvisioningArtifactInputRequestTypeDef(TypedDict):
    ProductId: str,
    ProvisioningArtifactId: str,
    AcceptLanguage: NotRequired[str],
```

## DeleteServiceActionInputRequestTypeDef

```python
# DeleteServiceActionInputRequestTypeDef definition

class DeleteServiceActionInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
    IdempotencyToken: NotRequired[str],
```

## DeleteTagOptionInputRequestTypeDef

```python
# DeleteTagOptionInputRequestTypeDef definition

class DeleteTagOptionInputRequestTypeDef(TypedDict):
    Id: str,
```

## DescribeConstraintInputRequestTypeDef

```python
# DescribeConstraintInputRequestTypeDef definition

class DescribeConstraintInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
```

## DescribeCopyProductStatusInputRequestTypeDef

```python
# DescribeCopyProductStatusInputRequestTypeDef definition

class DescribeCopyProductStatusInputRequestTypeDef(TypedDict):
    CopyProductToken: str,
    AcceptLanguage: NotRequired[str],
```

## DescribePortfolioInputRequestTypeDef

```python
# DescribePortfolioInputRequestTypeDef definition

class DescribePortfolioInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
```

## DescribePortfolioShareStatusInputRequestTypeDef

```python
# DescribePortfolioShareStatusInputRequestTypeDef definition

class DescribePortfolioShareStatusInputRequestTypeDef(TypedDict):
    PortfolioShareToken: str,
```

## DescribePortfolioSharesInputRequestTypeDef

```python
# DescribePortfolioSharesInputRequestTypeDef definition

class DescribePortfolioSharesInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    Type: DescribePortfolioShareTypeType,  # (1)
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-brackets: DescribePortfolioShareTypeType](./literals.md#describeportfoliosharetypetype) 
## PortfolioShareDetailTypeDef

```python
# PortfolioShareDetailTypeDef definition

class PortfolioShareDetailTypeDef(TypedDict):
    PrincipalId: NotRequired[str],
    Type: NotRequired[DescribePortfolioShareTypeType],  # (1)
    Accepted: NotRequired[bool],
    ShareTagOptions: NotRequired[bool],
    SharePrincipals: NotRequired[bool],
```

1. See [:material-code-brackets: DescribePortfolioShareTypeType](./literals.md#describeportfoliosharetypetype) 
## DescribeProductAsAdminInputRequestTypeDef

```python
# DescribeProductAsAdminInputRequestTypeDef definition

class DescribeProductAsAdminInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    SourcePortfolioId: NotRequired[str],
```

## ProvisioningArtifactSummaryTypeDef

```python
# ProvisioningArtifactSummaryTypeDef definition

class ProvisioningArtifactSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    ProvisioningArtifactMetadata: NotRequired[Dict[str, str]],
```

## DescribeProductInputRequestTypeDef

```python
# DescribeProductInputRequestTypeDef definition

class DescribeProductInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
```

## LaunchPathTypeDef

```python
# LaunchPathTypeDef definition

class LaunchPathTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
```

## ProductViewSummaryTypeDef

```python
# ProductViewSummaryTypeDef definition

class ProductViewSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    ProductId: NotRequired[str],
    Name: NotRequired[str],
    Owner: NotRequired[str],
    ShortDescription: NotRequired[str],
    Type: NotRequired[ProductTypeType],  # (1)
    Distributor: NotRequired[str],
    HasDefaultPath: NotRequired[bool],
    SupportEmail: NotRequired[str],
    SupportDescription: NotRequired[str],
    SupportUrl: NotRequired[str],
```

1. See [:material-code-brackets: ProductTypeType](./literals.md#producttypetype) 
## ProvisioningArtifactTypeDef

```python
# ProvisioningArtifactTypeDef definition

class ProvisioningArtifactTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    Guidance: NotRequired[ProvisioningArtifactGuidanceType],  # (1)
```

1. See [:material-code-brackets: ProvisioningArtifactGuidanceType](./literals.md#provisioningartifactguidancetype) 
## DescribeProductViewInputRequestTypeDef

```python
# DescribeProductViewInputRequestTypeDef definition

class DescribeProductViewInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
```

## DescribeProvisionedProductInputRequestTypeDef

```python
# DescribeProvisionedProductInputRequestTypeDef definition

class DescribeProvisionedProductInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
```

## ProvisionedProductDetailTypeDef

```python
# ProvisionedProductDetailTypeDef definition

class ProvisionedProductDetailTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Type: NotRequired[str],
    Id: NotRequired[str],
    Status: NotRequired[ProvisionedProductStatusType],  # (1)
    StatusMessage: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    IdempotencyToken: NotRequired[str],
    LastRecordId: NotRequired[str],
    LastProvisioningRecordId: NotRequired[str],
    LastSuccessfulProvisioningRecordId: NotRequired[str],
    ProductId: NotRequired[str],
    ProvisioningArtifactId: NotRequired[str],
    LaunchRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: ProvisionedProductStatusType](./literals.md#provisionedproductstatustype) 
## DescribeProvisionedProductPlanInputRequestTypeDef

```python
# DescribeProvisionedProductPlanInputRequestTypeDef definition

class DescribeProvisionedProductPlanInputRequestTypeDef(TypedDict):
    PlanId: str,
    AcceptLanguage: NotRequired[str],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

## DescribeProvisioningArtifactInputRequestTypeDef

```python
# DescribeProvisioningArtifactInputRequestTypeDef definition

class DescribeProvisioningArtifactInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    ProvisioningArtifactId: NotRequired[str],
    ProductId: NotRequired[str],
    ProvisioningArtifactName: NotRequired[str],
    ProductName: NotRequired[str],
    Verbose: NotRequired[bool],
    IncludeProvisioningArtifactParameters: NotRequired[bool],
```

## DescribeProvisioningParametersInputRequestTypeDef

```python
# DescribeProvisioningParametersInputRequestTypeDef definition

class DescribeProvisioningParametersInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    ProductId: NotRequired[str],
    ProductName: NotRequired[str],
    ProvisioningArtifactId: NotRequired[str],
    ProvisioningArtifactName: NotRequired[str],
    PathId: NotRequired[str],
    PathName: NotRequired[str],
```

## ProvisioningArtifactOutputTypeDef

```python
# ProvisioningArtifactOutputTypeDef definition

class ProvisioningArtifactOutputTypeDef(TypedDict):
    Key: NotRequired[str],
    Description: NotRequired[str],
```

## ProvisioningArtifactPreferencesTypeDef

```python
# ProvisioningArtifactPreferencesTypeDef definition

class ProvisioningArtifactPreferencesTypeDef(TypedDict):
    StackSetAccounts: NotRequired[List[str]],
    StackSetRegions: NotRequired[List[str]],
```

## TagOptionSummaryTypeDef

```python
# TagOptionSummaryTypeDef definition

class TagOptionSummaryTypeDef(TypedDict):
    Key: NotRequired[str],
    Values: NotRequired[List[str]],
```

## UsageInstructionTypeDef

```python
# UsageInstructionTypeDef definition

class UsageInstructionTypeDef(TypedDict):
    Type: NotRequired[str],
    Value: NotRequired[str],
```

## DescribeRecordInputRequestTypeDef

```python
# DescribeRecordInputRequestTypeDef definition

class DescribeRecordInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## RecordOutputTypeDef

```python
# RecordOutputTypeDef definition

class RecordOutputTypeDef(TypedDict):
    OutputKey: NotRequired[str],
    OutputValue: NotRequired[str],
    Description: NotRequired[str],
```

## DescribeServiceActionExecutionParametersInputRequestTypeDef

```python
# DescribeServiceActionExecutionParametersInputRequestTypeDef definition

class DescribeServiceActionExecutionParametersInputRequestTypeDef(TypedDict):
    ProvisionedProductId: str,
    ServiceActionId: str,
    AcceptLanguage: NotRequired[str],
```

## ExecutionParameterTypeDef

```python
# ExecutionParameterTypeDef definition

class ExecutionParameterTypeDef(TypedDict):
    Name: NotRequired[str],
    Type: NotRequired[str],
    DefaultValues: NotRequired[List[str]],
```

## DescribeServiceActionInputRequestTypeDef

```python
# DescribeServiceActionInputRequestTypeDef definition

class DescribeServiceActionInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
```

## DescribeTagOptionInputRequestTypeDef

```python
# DescribeTagOptionInputRequestTypeDef definition

class DescribeTagOptionInputRequestTypeDef(TypedDict):
    Id: str,
```

## DisassociateBudgetFromResourceInputRequestTypeDef

```python
# DisassociateBudgetFromResourceInputRequestTypeDef definition

class DisassociateBudgetFromResourceInputRequestTypeDef(TypedDict):
    BudgetName: str,
    ResourceId: str,
```

## DisassociatePrincipalFromPortfolioInputRequestTypeDef

```python
# DisassociatePrincipalFromPortfolioInputRequestTypeDef definition

class DisassociatePrincipalFromPortfolioInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    PrincipalARN: str,
    AcceptLanguage: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## DisassociateProductFromPortfolioInputRequestTypeDef

```python
# DisassociateProductFromPortfolioInputRequestTypeDef definition

class DisassociateProductFromPortfolioInputRequestTypeDef(TypedDict):
    ProductId: str,
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
```

## DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef

```python
# DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef definition

class DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef(TypedDict):
    ProductId: str,
    ProvisioningArtifactId: str,
    ServiceActionId: str,
    AcceptLanguage: NotRequired[str],
    IdempotencyToken: NotRequired[str],
```

## DisassociateTagOptionFromResourceInputRequestTypeDef

```python
# DisassociateTagOptionFromResourceInputRequestTypeDef definition

class DisassociateTagOptionFromResourceInputRequestTypeDef(TypedDict):
    ResourceId: str,
    TagOptionId: str,
```

## UniqueTagResourceIdentifierTypeDef

```python
# UniqueTagResourceIdentifierTypeDef definition

class UniqueTagResourceIdentifierTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ExecuteProvisionedProductPlanInputRequestTypeDef

```python
# ExecuteProvisionedProductPlanInputRequestTypeDef definition

class ExecuteProvisionedProductPlanInputRequestTypeDef(TypedDict):
    PlanId: str,
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
```

## ExecuteProvisionedProductServiceActionInputRequestTypeDef

```python
# ExecuteProvisionedProductServiceActionInputRequestTypeDef definition

class ExecuteProvisionedProductServiceActionInputRequestTypeDef(TypedDict):
    ProvisionedProductId: str,
    ServiceActionId: str,
    ExecuteToken: str,
    AcceptLanguage: NotRequired[str],
    Parameters: NotRequired[Mapping[str, Sequence[str]]],
```

## GetProvisionedProductOutputsInputRequestTypeDef

```python
# GetProvisionedProductOutputsInputRequestTypeDef definition

class GetProvisionedProductOutputsInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    ProvisionedProductId: NotRequired[str],
    ProvisionedProductName: NotRequired[str],
    OutputKeys: NotRequired[Sequence[str]],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

## ImportAsProvisionedProductInputRequestTypeDef

```python
# ImportAsProvisionedProductInputRequestTypeDef definition

class ImportAsProvisionedProductInputRequestTypeDef(TypedDict):
    ProductId: str,
    ProvisioningArtifactId: str,
    ProvisionedProductName: str,
    PhysicalId: str,
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
```

## LastSyncTypeDef

```python
# LastSyncTypeDef definition

class LastSyncTypeDef(TypedDict):
    LastSyncTime: NotRequired[datetime],
    LastSyncStatus: NotRequired[LastSyncStatusType],  # (1)
    LastSyncStatusMessage: NotRequired[str],
    LastSuccessfulSyncTime: NotRequired[datetime],
    LastSuccessfulSyncProvisioningArtifactId: NotRequired[str],
```

1. See [:material-code-brackets: LastSyncStatusType](./literals.md#lastsyncstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAcceptedPortfolioSharesInputRequestTypeDef

```python
# ListAcceptedPortfolioSharesInputRequestTypeDef definition

class ListAcceptedPortfolioSharesInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
    PortfolioShareType: NotRequired[PortfolioShareTypeType],  # (1)
```

1. See [:material-code-brackets: PortfolioShareTypeType](./literals.md#portfoliosharetypetype) 
## ListBudgetsForResourceInputRequestTypeDef

```python
# ListBudgetsForResourceInputRequestTypeDef definition

class ListBudgetsForResourceInputRequestTypeDef(TypedDict):
    ResourceId: str,
    AcceptLanguage: NotRequired[str],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

## ListConstraintsForPortfolioInputRequestTypeDef

```python
# ListConstraintsForPortfolioInputRequestTypeDef definition

class ListConstraintsForPortfolioInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    ProductId: NotRequired[str],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

## ListLaunchPathsInputRequestTypeDef

```python
# ListLaunchPathsInputRequestTypeDef definition

class ListLaunchPathsInputRequestTypeDef(TypedDict):
    ProductId: str,
    AcceptLanguage: NotRequired[str],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

## ListOrganizationPortfolioAccessInputRequestTypeDef

```python
# ListOrganizationPortfolioAccessInputRequestTypeDef definition

class ListOrganizationPortfolioAccessInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    OrganizationNodeType: OrganizationNodeTypeType,  # (1)
    AcceptLanguage: NotRequired[str],
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
```

1. See [:material-code-brackets: OrganizationNodeTypeType](./literals.md#organizationnodetypetype) 
## ListPortfolioAccessInputRequestTypeDef

```python
# ListPortfolioAccessInputRequestTypeDef definition

class ListPortfolioAccessInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    OrganizationParentId: NotRequired[str],
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListPortfoliosForProductInputRequestTypeDef

```python
# ListPortfoliosForProductInputRequestTypeDef definition

class ListPortfoliosForProductInputRequestTypeDef(TypedDict):
    ProductId: str,
    AcceptLanguage: NotRequired[str],
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListPortfoliosInputRequestTypeDef

```python
# ListPortfoliosInputRequestTypeDef definition

class ListPortfoliosInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## ListPrincipalsForPortfolioInputRequestTypeDef

```python
# ListPrincipalsForPortfolioInputRequestTypeDef definition

class ListPrincipalsForPortfolioInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

## PrincipalTypeDef

```python
# PrincipalTypeDef definition

class PrincipalTypeDef(TypedDict):
    PrincipalARN: NotRequired[str],
    PrincipalType: NotRequired[PrincipalTypeType],  # (1)
```

1. See [:material-code-brackets: PrincipalTypeType](./literals.md#principaltypetype) 
## ProvisionedProductPlanSummaryTypeDef

```python
# ProvisionedProductPlanSummaryTypeDef definition

class ProvisionedProductPlanSummaryTypeDef(TypedDict):
    PlanName: NotRequired[str],
    PlanId: NotRequired[str],
    ProvisionProductId: NotRequired[str],
    ProvisionProductName: NotRequired[str],
    PlanType: NotRequired[ProvisionedProductPlanTypeType],  # (1)
    ProvisioningArtifactId: NotRequired[str],
```

1. See [:material-code-brackets: ProvisionedProductPlanTypeType](./literals.md#provisionedproductplantypetype) 
## ListProvisioningArtifactsForServiceActionInputRequestTypeDef

```python
# ListProvisioningArtifactsForServiceActionInputRequestTypeDef definition

class ListProvisioningArtifactsForServiceActionInputRequestTypeDef(TypedDict):
    ServiceActionId: str,
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
    AcceptLanguage: NotRequired[str],
```

## ListProvisioningArtifactsInputRequestTypeDef

```python
# ListProvisioningArtifactsInputRequestTypeDef definition

class ListProvisioningArtifactsInputRequestTypeDef(TypedDict):
    ProductId: str,
    AcceptLanguage: NotRequired[str],
```

## ListRecordHistorySearchFilterTypeDef

```python
# ListRecordHistorySearchFilterTypeDef definition

class ListRecordHistorySearchFilterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ListResourcesForTagOptionInputRequestTypeDef

```python
# ListResourcesForTagOptionInputRequestTypeDef definition

class ListResourcesForTagOptionInputRequestTypeDef(TypedDict):
    TagOptionId: str,
    ResourceType: NotRequired[str],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

## ResourceDetailTypeDef

```python
# ResourceDetailTypeDef definition

class ResourceDetailTypeDef(TypedDict):
    Id: NotRequired[str],
    ARN: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    CreatedTime: NotRequired[datetime],
```

## ListServiceActionsForProvisioningArtifactInputRequestTypeDef

```python
# ListServiceActionsForProvisioningArtifactInputRequestTypeDef definition

class ListServiceActionsForProvisioningArtifactInputRequestTypeDef(TypedDict):
    ProductId: str,
    ProvisioningArtifactId: str,
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
    AcceptLanguage: NotRequired[str],
```

## ServiceActionSummaryTypeDef

```python
# ServiceActionSummaryTypeDef definition

class ServiceActionSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    DefinitionType: NotRequired[ServiceActionDefinitionTypeType],  # (1)
```

1. See [:material-code-brackets: ServiceActionDefinitionTypeType](./literals.md#serviceactiondefinitiontypetype) 
## ListServiceActionsInputRequestTypeDef

```python
# ListServiceActionsInputRequestTypeDef definition

class ListServiceActionsInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

## ListStackInstancesForProvisionedProductInputRequestTypeDef

```python
# ListStackInstancesForProvisionedProductInputRequestTypeDef definition

class ListStackInstancesForProvisionedProductInputRequestTypeDef(TypedDict):
    ProvisionedProductId: str,
    AcceptLanguage: NotRequired[str],
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
```

## StackInstanceTypeDef

```python
# StackInstanceTypeDef definition

class StackInstanceTypeDef(TypedDict):
    Account: NotRequired[str],
    Region: NotRequired[str],
    StackInstanceStatus: NotRequired[StackInstanceStatusType],  # (1)
```

1. See [:material-code-brackets: StackInstanceStatusType](./literals.md#stackinstancestatustype) 
## ListTagOptionsFiltersTypeDef

```python
# ListTagOptionsFiltersTypeDef definition

class ListTagOptionsFiltersTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
    Active: NotRequired[bool],
```

## NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef

```python
# NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef definition

class NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef(TypedDict):
    WorkflowToken: str,
    RecordId: str,
    Status: EngineWorkflowStatusType,  # (1)
    IdempotencyToken: str,
    FailureReason: NotRequired[str],
```

1. See [:material-code-brackets: EngineWorkflowStatusType](./literals.md#engineworkflowstatustype) 
## ParameterConstraintsTypeDef

```python
# ParameterConstraintsTypeDef definition

class ParameterConstraintsTypeDef(TypedDict):
    AllowedValues: NotRequired[List[str]],
    AllowedPattern: NotRequired[str],
    ConstraintDescription: NotRequired[str],
    MaxLength: NotRequired[str],
    MinLength: NotRequired[str],
    MaxValue: NotRequired[str],
    MinValue: NotRequired[str],
```

## ProductViewAggregationValueTypeDef

```python
# ProductViewAggregationValueTypeDef definition

class ProductViewAggregationValueTypeDef(TypedDict):
    Value: NotRequired[str],
    ApproximateCount: NotRequired[int],
```

## ProvisioningParameterTypeDef

```python
# ProvisioningParameterTypeDef definition

class ProvisioningParameterTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## ProvisioningPreferencesTypeDef

```python
# ProvisioningPreferencesTypeDef definition

class ProvisioningPreferencesTypeDef(TypedDict):
    StackSetAccounts: NotRequired[Sequence[str]],
    StackSetRegions: NotRequired[Sequence[str]],
    StackSetFailureToleranceCount: NotRequired[int],
    StackSetFailureTolerancePercentage: NotRequired[int],
    StackSetMaxConcurrencyCount: NotRequired[int],
    StackSetMaxConcurrencyPercentage: NotRequired[int],
```

## RecordErrorTypeDef

```python
# RecordErrorTypeDef definition

class RecordErrorTypeDef(TypedDict):
    Code: NotRequired[str],
    Description: NotRequired[str],
```

## RecordTagTypeDef

```python
# RecordTagTypeDef definition

class RecordTagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## RejectPortfolioShareInputRequestTypeDef

```python
# RejectPortfolioShareInputRequestTypeDef definition

class RejectPortfolioShareInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    PortfolioShareType: NotRequired[PortfolioShareTypeType],  # (1)
```

1. See [:material-code-brackets: PortfolioShareTypeType](./literals.md#portfoliosharetypetype) 
## ResourceTargetDefinitionTypeDef

```python
# ResourceTargetDefinitionTypeDef definition

class ResourceTargetDefinitionTypeDef(TypedDict):
    Attribute: NotRequired[ResourceAttributeType],  # (1)
    Name: NotRequired[str],
    RequiresRecreation: NotRequired[RequiresRecreationType],  # (2)
```

1. See [:material-code-brackets: ResourceAttributeType](./literals.md#resourceattributetype) 
2. See [:material-code-brackets: RequiresRecreationType](./literals.md#requiresrecreationtype) 
## SearchProductsAsAdminInputRequestTypeDef

```python
# SearchProductsAsAdminInputRequestTypeDef definition

class SearchProductsAsAdminInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    PortfolioId: NotRequired[str],
    Filters: NotRequired[Mapping[ProductViewFilterByType, Sequence[str]]],  # (1)
    SortBy: NotRequired[ProductViewSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PageToken: NotRequired[str],
    PageSize: NotRequired[int],
    ProductSource: NotRequired[ProductSourceType],  # (4)
```

1. See [:material-code-brackets: ProductViewFilterByType](./literals.md#productviewfilterbytype) 
2. See [:material-code-brackets: ProductViewSortByType](./literals.md#productviewsortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-brackets: ProductSourceType](./literals.md#productsourcetype) 
## SearchProductsInputRequestTypeDef

```python
# SearchProductsInputRequestTypeDef definition

class SearchProductsInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    Filters: NotRequired[Mapping[ProductViewFilterByType, Sequence[str]]],  # (1)
    PageSize: NotRequired[int],
    SortBy: NotRequired[ProductViewSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    PageToken: NotRequired[str],
```

1. See [:material-code-brackets: ProductViewFilterByType](./literals.md#productviewfilterbytype) 
2. See [:material-code-brackets: ProductViewSortByType](./literals.md#productviewsortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## ShareErrorTypeDef

```python
# ShareErrorTypeDef definition

class ShareErrorTypeDef(TypedDict):
    Accounts: NotRequired[List[str]],
    Message: NotRequired[str],
    Error: NotRequired[str],
```

## TerminateProvisionedProductInputRequestTypeDef

```python
# TerminateProvisionedProductInputRequestTypeDef definition

class TerminateProvisionedProductInputRequestTypeDef(TypedDict):
    TerminateToken: str,
    ProvisionedProductName: NotRequired[str],
    ProvisionedProductId: NotRequired[str],
    IgnoreErrors: NotRequired[bool],
    AcceptLanguage: NotRequired[str],
    RetainPhysicalResources: NotRequired[bool],
```

## UpdateConstraintInputRequestTypeDef

```python
# UpdateConstraintInputRequestTypeDef definition

class UpdateConstraintInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
    Description: NotRequired[str],
    Parameters: NotRequired[str],
```

## UpdateProvisioningPreferencesTypeDef

```python
# UpdateProvisioningPreferencesTypeDef definition

class UpdateProvisioningPreferencesTypeDef(TypedDict):
    StackSetAccounts: NotRequired[Sequence[str]],
    StackSetRegions: NotRequired[Sequence[str]],
    StackSetFailureToleranceCount: NotRequired[int],
    StackSetFailureTolerancePercentage: NotRequired[int],
    StackSetMaxConcurrencyCount: NotRequired[int],
    StackSetMaxConcurrencyPercentage: NotRequired[int],
    StackSetOperationType: NotRequired[StackSetOperationTypeType],  # (1)
```

1. See [:material-code-brackets: StackSetOperationTypeType](./literals.md#stacksetoperationtypetype) 
## UpdateProvisionedProductPropertiesInputRequestTypeDef

```python
# UpdateProvisionedProductPropertiesInputRequestTypeDef definition

class UpdateProvisionedProductPropertiesInputRequestTypeDef(TypedDict):
    ProvisionedProductId: str,
    ProvisionedProductProperties: Mapping[PropertyKeyType, str],  # (1)
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
```

1. See [:material-code-brackets: PropertyKeyType](./literals.md#propertykeytype) 
## UpdateProvisioningArtifactInputRequestTypeDef

```python
# UpdateProvisioningArtifactInputRequestTypeDef definition

class UpdateProvisioningArtifactInputRequestTypeDef(TypedDict):
    ProductId: str,
    ProvisioningArtifactId: str,
    AcceptLanguage: NotRequired[str],
    Name: NotRequired[str],
    Description: NotRequired[str],
    Active: NotRequired[bool],
    Guidance: NotRequired[ProvisioningArtifactGuidanceType],  # (1)
```

1. See [:material-code-brackets: ProvisioningArtifactGuidanceType](./literals.md#provisioningartifactguidancetype) 
## UpdateServiceActionInputRequestTypeDef

```python
# UpdateServiceActionInputRequestTypeDef definition

class UpdateServiceActionInputRequestTypeDef(TypedDict):
    Id: str,
    Name: NotRequired[str],
    Definition: NotRequired[Mapping[ServiceActionDefinitionKeyType, str]],  # (1)
    Description: NotRequired[str],
    AcceptLanguage: NotRequired[str],
```

1. See [:material-code-brackets: ServiceActionDefinitionKeyType](./literals.md#serviceactiondefinitionkeytype) 
## UpdateTagOptionInputRequestTypeDef

```python
# UpdateTagOptionInputRequestTypeDef definition

class UpdateTagOptionInputRequestTypeDef(TypedDict):
    Id: str,
    Value: NotRequired[str],
    Active: NotRequired[bool],
```

## ListProvisionedProductPlansInputRequestTypeDef

```python
# ListProvisionedProductPlansInputRequestTypeDef definition

class ListProvisionedProductPlansInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    ProvisionProductId: NotRequired[str],
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
    AccessLevelFilter: NotRequired[AccessLevelFilterTypeDef],  # (1)
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
## ScanProvisionedProductsInputRequestTypeDef

```python
# ScanProvisionedProductsInputRequestTypeDef definition

class ScanProvisionedProductsInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    AccessLevelFilter: NotRequired[AccessLevelFilterTypeDef],  # (1)
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
## SearchProvisionedProductsInputRequestTypeDef

```python
# SearchProvisionedProductsInputRequestTypeDef definition

class SearchProvisionedProductsInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    AccessLevelFilter: NotRequired[AccessLevelFilterTypeDef],  # (1)
    Filters: NotRequired[Mapping[ProvisionedProductViewFilterByType, Sequence[str]]],  # (2)
    SortBy: NotRequired[str],
    SortOrder: NotRequired[SortOrderType],  # (3)
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
2. See [:material-code-brackets: ProvisionedProductViewFilterByType](./literals.md#provisionedproductviewfilterbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
## BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef

```python
# BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef definition

class BatchAssociateServiceActionWithProvisioningArtifactInputRequestTypeDef(TypedDict):
    ServiceActionAssociations: Sequence[ServiceActionAssociationTypeDef],  # (1)
    AcceptLanguage: NotRequired[str],
```

1. See [:material-code-braces: ServiceActionAssociationTypeDef](./type_defs.md#serviceactionassociationtypedef) 
## BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef

```python
# BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef definition

class BatchDisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef(TypedDict):
    ServiceActionAssociations: Sequence[ServiceActionAssociationTypeDef],  # (1)
    AcceptLanguage: NotRequired[str],
```

1. See [:material-code-braces: ServiceActionAssociationTypeDef](./type_defs.md#serviceactionassociationtypedef) 
## BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef

```python
# BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef definition

class BatchAssociateServiceActionWithProvisioningArtifactOutputTypeDef(TypedDict):
    FailedServiceActionAssociations: List[FailedServiceActionAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedServiceActionAssociationTypeDef](./type_defs.md#failedserviceactionassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef

```python
# BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef definition

class BatchDisassociateServiceActionFromProvisioningArtifactOutputTypeDef(TypedDict):
    FailedServiceActionAssociations: List[FailedServiceActionAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: FailedServiceActionAssociationTypeDef](./type_defs.md#failedserviceactionassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CopyProductOutputTypeDef

```python
# CopyProductOutputTypeDef definition

class CopyProductOutputTypeDef(TypedDict):
    CopyProductToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePortfolioShareOutputTypeDef

```python
# CreatePortfolioShareOutputTypeDef definition

class CreatePortfolioShareOutputTypeDef(TypedDict):
    PortfolioShareToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProvisionedProductPlanOutputTypeDef

```python
# CreateProvisionedProductPlanOutputTypeDef definition

class CreateProvisionedProductPlanOutputTypeDef(TypedDict):
    PlanName: str,
    PlanId: str,
    ProvisionProductId: str,
    ProvisionedProductName: str,
    ProvisioningArtifactId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePortfolioShareOutputTypeDef

```python
# DeletePortfolioShareOutputTypeDef definition

class DeletePortfolioShareOutputTypeDef(TypedDict):
    PortfolioShareToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCopyProductStatusOutputTypeDef

```python
# DescribeCopyProductStatusOutputTypeDef definition

class DescribeCopyProductStatusOutputTypeDef(TypedDict):
    CopyProductStatus: CopyProductStatusType,  # (1)
    TargetProductId: str,
    StatusDetail: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: CopyProductStatusType](./literals.md#copyproductstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetAWSOrganizationsAccessStatusOutputTypeDef

```python
# GetAWSOrganizationsAccessStatusOutputTypeDef definition

class GetAWSOrganizationsAccessStatusOutputTypeDef(TypedDict):
    AccessStatus: AccessStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: AccessStatusType](./literals.md#accessstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPortfolioAccessOutputTypeDef

```python
# ListPortfolioAccessOutputTypeDef definition

class ListPortfolioAccessOutputTypeDef(TypedDict):
    AccountIds: List[str],
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePortfolioShareOutputTypeDef

```python
# UpdatePortfolioShareOutputTypeDef definition

class UpdatePortfolioShareOutputTypeDef(TypedDict):
    PortfolioShareToken: str,
    Status: ShareStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProvisionedProductPropertiesOutputTypeDef

```python
# UpdateProvisionedProductPropertiesOutputTypeDef definition

class UpdateProvisionedProductPropertiesOutputTypeDef(TypedDict):
    ProvisionedProductId: str,
    ProvisionedProductProperties: Dict[PropertyKeyType, str],  # (1)
    RecordId: str,
    Status: RecordStatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: PropertyKeyType](./literals.md#propertykeytype) 
2. See [:material-code-brackets: RecordStatusType](./literals.md#recordstatustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBudgetsForResourceOutputTypeDef

```python
# ListBudgetsForResourceOutputTypeDef definition

class ListBudgetsForResourceOutputTypeDef(TypedDict):
    Budgets: List[BudgetDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BudgetDetailTypeDef](./type_defs.md#budgetdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SourceConnectionParametersTypeDef

```python
# SourceConnectionParametersTypeDef definition

class SourceConnectionParametersTypeDef(TypedDict):
    CodeStar: NotRequired[CodeStarParametersTypeDef],  # (1)
```

1. See [:material-code-braces: CodeStarParametersTypeDef](./type_defs.md#codestarparameterstypedef) 
## CreateConstraintOutputTypeDef

```python
# CreateConstraintOutputTypeDef definition

class CreateConstraintOutputTypeDef(TypedDict):
    ConstraintDetail: ConstraintDetailTypeDef,  # (1)
    ConstraintParameters: str,
    Status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConstraintDetailTypeDef](./type_defs.md#constraintdetailtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeConstraintOutputTypeDef

```python
# DescribeConstraintOutputTypeDef definition

class DescribeConstraintOutputTypeDef(TypedDict):
    ConstraintDetail: ConstraintDetailTypeDef,  # (1)
    ConstraintParameters: str,
    Status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConstraintDetailTypeDef](./type_defs.md#constraintdetailtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListConstraintsForPortfolioOutputTypeDef

```python
# ListConstraintsForPortfolioOutputTypeDef definition

class ListConstraintsForPortfolioOutputTypeDef(TypedDict):
    ConstraintDetails: List[ConstraintDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConstraintDetailTypeDef](./type_defs.md#constraintdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateConstraintOutputTypeDef

```python
# UpdateConstraintOutputTypeDef definition

class UpdateConstraintOutputTypeDef(TypedDict):
    ConstraintDetail: ConstraintDetailTypeDef,  # (1)
    ConstraintParameters: str,
    Status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConstraintDetailTypeDef](./type_defs.md#constraintdetailtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePortfolioInputRequestTypeDef

```python
# CreatePortfolioInputRequestTypeDef definition

class CreatePortfolioInputRequestTypeDef(TypedDict):
    DisplayName: str,
    ProviderName: str,
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## LaunchPathSummaryTypeDef

```python
# LaunchPathSummaryTypeDef definition

class LaunchPathSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    ConstraintSummaries: NotRequired[List[ConstraintSummaryTypeDef]],  # (1)
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    Name: NotRequired[str],
```

1. See [:material-code-braces: ConstraintSummaryTypeDef](./type_defs.md#constraintsummarytypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ProvisionedProductAttributeTypeDef

```python
# ProvisionedProductAttributeTypeDef definition

class ProvisionedProductAttributeTypeDef(TypedDict):
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Type: NotRequired[str],
    Id: NotRequired[str],
    Status: NotRequired[ProvisionedProductStatusType],  # (1)
    StatusMessage: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    IdempotencyToken: NotRequired[str],
    LastRecordId: NotRequired[str],
    LastProvisioningRecordId: NotRequired[str],
    LastSuccessfulProvisioningRecordId: NotRequired[str],
    Tags: NotRequired[List[TagTypeDef]],  # (2)
    PhysicalId: NotRequired[str],
    ProductId: NotRequired[str],
    ProductName: NotRequired[str],
    ProvisioningArtifactId: NotRequired[str],
    ProvisioningArtifactName: NotRequired[str],
    UserArn: NotRequired[str],
    UserArnSession: NotRequired[str],
```

1. See [:material-code-brackets: ProvisionedProductStatusType](./literals.md#provisionedproductstatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## UpdatePortfolioInputRequestTypeDef

```python
# UpdatePortfolioInputRequestTypeDef definition

class UpdatePortfolioInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
    DisplayName: NotRequired[str],
    Description: NotRequired[str],
    ProviderName: NotRequired[str],
    AddTags: NotRequired[Sequence[TagTypeDef]],  # (1)
    RemoveTags: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreatePortfolioOutputTypeDef

```python
# CreatePortfolioOutputTypeDef definition

class CreatePortfolioOutputTypeDef(TypedDict):
    PortfolioDetail: PortfolioDetailTypeDef,  # (1)
    Tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PortfolioDetailTypeDef](./type_defs.md#portfoliodetailtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAcceptedPortfolioSharesOutputTypeDef

```python
# ListAcceptedPortfolioSharesOutputTypeDef definition

class ListAcceptedPortfolioSharesOutputTypeDef(TypedDict):
    PortfolioDetails: List[PortfolioDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortfolioDetailTypeDef](./type_defs.md#portfoliodetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPortfoliosForProductOutputTypeDef

```python
# ListPortfoliosForProductOutputTypeDef definition

class ListPortfoliosForProductOutputTypeDef(TypedDict):
    PortfolioDetails: List[PortfolioDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortfolioDetailTypeDef](./type_defs.md#portfoliodetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPortfoliosOutputTypeDef

```python
# ListPortfoliosOutputTypeDef definition

class ListPortfoliosOutputTypeDef(TypedDict):
    PortfolioDetails: List[PortfolioDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortfolioDetailTypeDef](./type_defs.md#portfoliodetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePortfolioOutputTypeDef

```python
# UpdatePortfolioOutputTypeDef definition

class UpdatePortfolioOutputTypeDef(TypedDict):
    PortfolioDetail: PortfolioDetailTypeDef,  # (1)
    Tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PortfolioDetailTypeDef](./type_defs.md#portfoliodetailtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePortfolioShareInputRequestTypeDef

```python
# CreatePortfolioShareInputRequestTypeDef definition

class CreatePortfolioShareInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    AccountId: NotRequired[str],
    OrganizationNode: NotRequired[OrganizationNodeTypeDef],  # (1)
    ShareTagOptions: NotRequired[bool],
    SharePrincipals: NotRequired[bool],
```

1. See [:material-code-braces: OrganizationNodeTypeDef](./type_defs.md#organizationnodetypedef) 
## DeletePortfolioShareInputRequestTypeDef

```python
# DeletePortfolioShareInputRequestTypeDef definition

class DeletePortfolioShareInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    AccountId: NotRequired[str],
    OrganizationNode: NotRequired[OrganizationNodeTypeDef],  # (1)
```

1. See [:material-code-braces: OrganizationNodeTypeDef](./type_defs.md#organizationnodetypedef) 
## ListOrganizationPortfolioAccessOutputTypeDef

```python
# ListOrganizationPortfolioAccessOutputTypeDef definition

class ListOrganizationPortfolioAccessOutputTypeDef(TypedDict):
    OrganizationNodes: List[OrganizationNodeTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationNodeTypeDef](./type_defs.md#organizationnodetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdatePortfolioShareInputRequestTypeDef

```python
# UpdatePortfolioShareInputRequestTypeDef definition

class UpdatePortfolioShareInputRequestTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    AccountId: NotRequired[str],
    OrganizationNode: NotRequired[OrganizationNodeTypeDef],  # (1)
    ShareTagOptions: NotRequired[bool],
    SharePrincipals: NotRequired[bool],
```

1. See [:material-code-braces: OrganizationNodeTypeDef](./type_defs.md#organizationnodetypedef) 
## CreateProvisioningArtifactInputRequestTypeDef

```python
# CreateProvisioningArtifactInputRequestTypeDef definition

class CreateProvisioningArtifactInputRequestTypeDef(TypedDict):
    ProductId: str,
    Parameters: ProvisioningArtifactPropertiesTypeDef,  # (1)
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
```

1. See [:material-code-braces: ProvisioningArtifactPropertiesTypeDef](./type_defs.md#provisioningartifactpropertiestypedef) 
## CreateProvisioningArtifactOutputTypeDef

```python
# CreateProvisioningArtifactOutputTypeDef definition

class CreateProvisioningArtifactOutputTypeDef(TypedDict):
    ProvisioningArtifactDetail: ProvisioningArtifactDetailTypeDef,  # (1)
    Info: Dict[str, str],
    Status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProvisioningArtifactDetailTypeDef](./type_defs.md#provisioningartifactdetailtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProvisioningArtifactsOutputTypeDef

```python
# ListProvisioningArtifactsOutputTypeDef definition

class ListProvisioningArtifactsOutputTypeDef(TypedDict):
    ProvisioningArtifactDetails: List[ProvisioningArtifactDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisioningArtifactDetailTypeDef](./type_defs.md#provisioningartifactdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProvisioningArtifactOutputTypeDef

```python
# UpdateProvisioningArtifactOutputTypeDef definition

class UpdateProvisioningArtifactOutputTypeDef(TypedDict):
    ProvisioningArtifactDetail: ProvisioningArtifactDetailTypeDef,  # (1)
    Info: Dict[str, str],
    Status: StatusType,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProvisioningArtifactDetailTypeDef](./type_defs.md#provisioningartifactdetailtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProvisionedProductPlanInputRequestTypeDef

```python
# CreateProvisionedProductPlanInputRequestTypeDef definition

class CreateProvisionedProductPlanInputRequestTypeDef(TypedDict):
    PlanName: str,
    PlanType: ProvisionedProductPlanTypeType,  # (1)
    ProductId: str,
    ProvisionedProductName: str,
    ProvisioningArtifactId: str,
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
    NotificationArns: NotRequired[Sequence[str]],
    PathId: NotRequired[str],
    ProvisioningParameters: NotRequired[Sequence[UpdateProvisioningParameterTypeDef]],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: ProvisionedProductPlanTypeType](./literals.md#provisionedproductplantypetype) 
2. See [:material-code-braces: UpdateProvisioningParameterTypeDef](./type_defs.md#updateprovisioningparametertypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ProvisionedProductPlanDetailsTypeDef

```python
# ProvisionedProductPlanDetailsTypeDef definition

class ProvisionedProductPlanDetailsTypeDef(TypedDict):
    CreatedTime: NotRequired[datetime],
    PathId: NotRequired[str],
    ProductId: NotRequired[str],
    PlanName: NotRequired[str],
    PlanId: NotRequired[str],
    ProvisionProductId: NotRequired[str],
    ProvisionProductName: NotRequired[str],
    PlanType: NotRequired[ProvisionedProductPlanTypeType],  # (1)
    ProvisioningArtifactId: NotRequired[str],
    Status: NotRequired[ProvisionedProductPlanStatusType],  # (2)
    UpdatedTime: NotRequired[datetime],
    NotificationArns: NotRequired[List[str]],
    ProvisioningParameters: NotRequired[List[UpdateProvisioningParameterTypeDef]],  # (3)
    Tags: NotRequired[List[TagTypeDef]],  # (4)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ProvisionedProductPlanTypeType](./literals.md#provisionedproductplantypetype) 
2. See [:material-code-brackets: ProvisionedProductPlanStatusType](./literals.md#provisionedproductplanstatustype) 
3. See [:material-code-braces: UpdateProvisioningParameterTypeDef](./type_defs.md#updateprovisioningparametertypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTagOptionOutputTypeDef

```python
# CreateTagOptionOutputTypeDef definition

class CreateTagOptionOutputTypeDef(TypedDict):
    TagOptionDetail: TagOptionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagOptionDetailTypeDef](./type_defs.md#tagoptiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePortfolioOutputTypeDef

```python
# DescribePortfolioOutputTypeDef definition

class DescribePortfolioOutputTypeDef(TypedDict):
    PortfolioDetail: PortfolioDetailTypeDef,  # (1)
    Tags: List[TagTypeDef],  # (2)
    TagOptions: List[TagOptionDetailTypeDef],  # (3)
    Budgets: List[BudgetDetailTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: PortfolioDetailTypeDef](./type_defs.md#portfoliodetailtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: TagOptionDetailTypeDef](./type_defs.md#tagoptiondetailtypedef) 
4. See [:material-code-braces: BudgetDetailTypeDef](./type_defs.md#budgetdetailtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTagOptionOutputTypeDef

```python
# DescribeTagOptionOutputTypeDef definition

class DescribeTagOptionOutputTypeDef(TypedDict):
    TagOptionDetail: TagOptionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagOptionDetailTypeDef](./type_defs.md#tagoptiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagOptionsOutputTypeDef

```python
# ListTagOptionsOutputTypeDef definition

class ListTagOptionsOutputTypeDef(TypedDict):
    TagOptionDetails: List[TagOptionDetailTypeDef],  # (1)
    PageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagOptionDetailTypeDef](./type_defs.md#tagoptiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTagOptionOutputTypeDef

```python
# UpdateTagOptionOutputTypeDef definition

class UpdateTagOptionOutputTypeDef(TypedDict):
    TagOptionDetail: TagOptionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagOptionDetailTypeDef](./type_defs.md#tagoptiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribePortfolioSharesOutputTypeDef

```python
# DescribePortfolioSharesOutputTypeDef definition

class DescribePortfolioSharesOutputTypeDef(TypedDict):
    NextPageToken: str,
    PortfolioShareDetails: List[PortfolioShareDetailTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PortfolioShareDetailTypeDef](./type_defs.md#portfoliosharedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProductOutputTypeDef

```python
# DescribeProductOutputTypeDef definition

class DescribeProductOutputTypeDef(TypedDict):
    ProductViewSummary: ProductViewSummaryTypeDef,  # (1)
    ProvisioningArtifacts: List[ProvisioningArtifactTypeDef],  # (2)
    Budgets: List[BudgetDetailTypeDef],  # (3)
    LaunchPaths: List[LaunchPathTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: ProductViewSummaryTypeDef](./type_defs.md#productviewsummarytypedef) 
2. See [:material-code-braces: ProvisioningArtifactTypeDef](./type_defs.md#provisioningartifacttypedef) 
3. See [:material-code-braces: BudgetDetailTypeDef](./type_defs.md#budgetdetailtypedef) 
4. See [:material-code-braces: LaunchPathTypeDef](./type_defs.md#launchpathtypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProductViewOutputTypeDef

```python
# DescribeProductViewOutputTypeDef definition

class DescribeProductViewOutputTypeDef(TypedDict):
    ProductViewSummary: ProductViewSummaryTypeDef,  # (1)
    ProvisioningArtifacts: List[ProvisioningArtifactTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProductViewSummaryTypeDef](./type_defs.md#productviewsummarytypedef) 
2. See [:material-code-braces: ProvisioningArtifactTypeDef](./type_defs.md#provisioningartifacttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisioningArtifactViewTypeDef

```python
# ProvisioningArtifactViewTypeDef definition

class ProvisioningArtifactViewTypeDef(TypedDict):
    ProductViewSummary: NotRequired[ProductViewSummaryTypeDef],  # (1)
    ProvisioningArtifact: NotRequired[ProvisioningArtifactTypeDef],  # (2)
```

1. See [:material-code-braces: ProductViewSummaryTypeDef](./type_defs.md#productviewsummarytypedef) 
2. See [:material-code-braces: ProvisioningArtifactTypeDef](./type_defs.md#provisioningartifacttypedef) 
## DescribeProvisionedProductOutputTypeDef

```python
# DescribeProvisionedProductOutputTypeDef definition

class DescribeProvisionedProductOutputTypeDef(TypedDict):
    ProvisionedProductDetail: ProvisionedProductDetailTypeDef,  # (1)
    CloudWatchDashboards: List[CloudWatchDashboardTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProvisionedProductDetailTypeDef](./type_defs.md#provisionedproductdetailtypedef) 
2. See [:material-code-braces: CloudWatchDashboardTypeDef](./type_defs.md#cloudwatchdashboardtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ScanProvisionedProductsOutputTypeDef

```python
# ScanProvisionedProductsOutputTypeDef definition

class ScanProvisionedProductsOutputTypeDef(TypedDict):
    ProvisionedProducts: List[ProvisionedProductDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedProductDetailTypeDef](./type_defs.md#provisionedproductdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProvisionedProductOutputsOutputTypeDef

```python
# GetProvisionedProductOutputsOutputTypeDef definition

class GetProvisionedProductOutputsOutputTypeDef(TypedDict):
    Outputs: List[RecordOutputTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordOutputTypeDef](./type_defs.md#recordoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef

```python
# NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef definition

class NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef(TypedDict):
    WorkflowToken: str,
    RecordId: str,
    Status: EngineWorkflowStatusType,  # (1)
    IdempotencyToken: str,
    FailureReason: NotRequired[str],
    Outputs: NotRequired[Sequence[RecordOutputTypeDef]],  # (2)
```

1. See [:material-code-brackets: EngineWorkflowStatusType](./literals.md#engineworkflowstatustype) 
2. See [:material-code-braces: RecordOutputTypeDef](./type_defs.md#recordoutputtypedef) 
## DescribeServiceActionExecutionParametersOutputTypeDef

```python
# DescribeServiceActionExecutionParametersOutputTypeDef definition

class DescribeServiceActionExecutionParametersOutputTypeDef(TypedDict):
    ServiceActionParameters: List[ExecutionParameterTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExecutionParameterTypeDef](./type_defs.md#executionparametertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EngineWorkflowResourceIdentifierTypeDef

```python
# EngineWorkflowResourceIdentifierTypeDef definition

class EngineWorkflowResourceIdentifierTypeDef(TypedDict):
    UniqueTag: NotRequired[UniqueTagResourceIdentifierTypeDef],  # (1)
```

1. See [:material-code-braces: UniqueTagResourceIdentifierTypeDef](./type_defs.md#uniquetagresourceidentifiertypedef) 
## ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef

```python
# ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef definition

class ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    PortfolioShareType: NotRequired[PortfolioShareTypeType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PortfolioShareTypeType](./literals.md#portfoliosharetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef

```python
# ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef definition

class ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    ProductId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLaunchPathsInputListLaunchPathsPaginateTypeDef

```python
# ListLaunchPathsInputListLaunchPathsPaginateTypeDef definition

class ListLaunchPathsInputListLaunchPathsPaginateTypeDef(TypedDict):
    ProductId: str,
    AcceptLanguage: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef

```python
# ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef definition

class ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef(TypedDict):
    PortfolioId: str,
    OrganizationNodeType: OrganizationNodeTypeType,  # (1)
    AcceptLanguage: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: OrganizationNodeTypeType](./literals.md#organizationnodetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef

```python
# ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef definition

class ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef(TypedDict):
    ProductId: str,
    AcceptLanguage: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPortfoliosInputListPortfoliosPaginateTypeDef

```python
# ListPortfoliosInputListPortfoliosPaginateTypeDef definition

class ListPortfoliosInputListPortfoliosPaginateTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef

```python
# ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef definition

class ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef(TypedDict):
    PortfolioId: str,
    AcceptLanguage: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef

```python
# ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef definition

class ListProvisionedProductPlansInputListProvisionedProductPlansPaginateTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    ProvisionProductId: NotRequired[str],
    AccessLevelFilter: NotRequired[AccessLevelFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef

```python
# ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef definition

class ListProvisioningArtifactsForServiceActionInputListProvisioningArtifactsForServiceActionPaginateTypeDef(TypedDict):
    ServiceActionId: str,
    AcceptLanguage: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef

```python
# ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef definition

class ListResourcesForTagOptionInputListResourcesForTagOptionPaginateTypeDef(TypedDict):
    TagOptionId: str,
    ResourceType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef

```python
# ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef definition

class ListServiceActionsForProvisioningArtifactInputListServiceActionsForProvisioningArtifactPaginateTypeDef(TypedDict):
    ProductId: str,
    ProvisioningArtifactId: str,
    AcceptLanguage: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListServiceActionsInputListServiceActionsPaginateTypeDef

```python
# ListServiceActionsInputListServiceActionsPaginateTypeDef definition

class ListServiceActionsInputListServiceActionsPaginateTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef

```python
# ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef definition

class ScanProvisionedProductsInputScanProvisionedProductsPaginateTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    AccessLevelFilter: NotRequired[AccessLevelFilterTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef

```python
# SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef definition

class SearchProductsAsAdminInputSearchProductsAsAdminPaginateTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    PortfolioId: NotRequired[str],
    Filters: NotRequired[Mapping[ProductViewFilterByType, Sequence[str]]],  # (1)
    SortBy: NotRequired[ProductViewSortByType],  # (2)
    SortOrder: NotRequired[SortOrderType],  # (3)
    ProductSource: NotRequired[ProductSourceType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: ProductViewFilterByType](./literals.md#productviewfilterbytype) 
2. See [:material-code-brackets: ProductViewSortByType](./literals.md#productviewsortbytype) 
3. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
4. See [:material-code-brackets: ProductSourceType](./literals.md#productsourcetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrincipalsForPortfolioOutputTypeDef

```python
# ListPrincipalsForPortfolioOutputTypeDef definition

class ListPrincipalsForPortfolioOutputTypeDef(TypedDict):
    Principals: List[PrincipalTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProvisionedProductPlansOutputTypeDef

```python
# ListProvisionedProductPlansOutputTypeDef definition

class ListProvisionedProductPlansOutputTypeDef(TypedDict):
    ProvisionedProductPlans: List[ProvisionedProductPlanSummaryTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedProductPlanSummaryTypeDef](./type_defs.md#provisionedproductplansummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecordHistoryInputListRecordHistoryPaginateTypeDef

```python
# ListRecordHistoryInputListRecordHistoryPaginateTypeDef definition

class ListRecordHistoryInputListRecordHistoryPaginateTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    AccessLevelFilter: NotRequired[AccessLevelFilterTypeDef],  # (1)
    SearchFilter: NotRequired[ListRecordHistorySearchFilterTypeDef],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
2. See [:material-code-braces: ListRecordHistorySearchFilterTypeDef](./type_defs.md#listrecordhistorysearchfiltertypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecordHistoryInputRequestTypeDef

```python
# ListRecordHistoryInputRequestTypeDef definition

class ListRecordHistoryInputRequestTypeDef(TypedDict):
    AcceptLanguage: NotRequired[str],
    AccessLevelFilter: NotRequired[AccessLevelFilterTypeDef],  # (1)
    SearchFilter: NotRequired[ListRecordHistorySearchFilterTypeDef],  # (2)
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

1. See [:material-code-braces: AccessLevelFilterTypeDef](./type_defs.md#accesslevelfiltertypedef) 
2. See [:material-code-braces: ListRecordHistorySearchFilterTypeDef](./type_defs.md#listrecordhistorysearchfiltertypedef) 
## ListResourcesForTagOptionOutputTypeDef

```python
# ListResourcesForTagOptionOutputTypeDef definition

class ListResourcesForTagOptionOutputTypeDef(TypedDict):
    ResourceDetails: List[ResourceDetailTypeDef],  # (1)
    PageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceDetailTypeDef](./type_defs.md#resourcedetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceActionsForProvisioningArtifactOutputTypeDef

```python
# ListServiceActionsForProvisioningArtifactOutputTypeDef definition

class ListServiceActionsForProvisioningArtifactOutputTypeDef(TypedDict):
    ServiceActionSummaries: List[ServiceActionSummaryTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceActionSummaryTypeDef](./type_defs.md#serviceactionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListServiceActionsOutputTypeDef

```python
# ListServiceActionsOutputTypeDef definition

class ListServiceActionsOutputTypeDef(TypedDict):
    ServiceActionSummaries: List[ServiceActionSummaryTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceActionSummaryTypeDef](./type_defs.md#serviceactionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceActionDetailTypeDef

```python
# ServiceActionDetailTypeDef definition

class ServiceActionDetailTypeDef(TypedDict):
    ServiceActionSummary: NotRequired[ServiceActionSummaryTypeDef],  # (1)
    Definition: NotRequired[Dict[ServiceActionDefinitionKeyType, str]],  # (2)
```

1. See [:material-code-braces: ServiceActionSummaryTypeDef](./type_defs.md#serviceactionsummarytypedef) 
2. See [:material-code-brackets: ServiceActionDefinitionKeyType](./literals.md#serviceactiondefinitionkeytype) 
## ListStackInstancesForProvisionedProductOutputTypeDef

```python
# ListStackInstancesForProvisionedProductOutputTypeDef definition

class ListStackInstancesForProvisionedProductOutputTypeDef(TypedDict):
    StackInstances: List[StackInstanceTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: StackInstanceTypeDef](./type_defs.md#stackinstancetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagOptionsInputListTagOptionsPaginateTypeDef

```python
# ListTagOptionsInputListTagOptionsPaginateTypeDef definition

class ListTagOptionsInputListTagOptionsPaginateTypeDef(TypedDict):
    Filters: NotRequired[ListTagOptionsFiltersTypeDef],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: ListTagOptionsFiltersTypeDef](./type_defs.md#listtagoptionsfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagOptionsInputRequestTypeDef

```python
# ListTagOptionsInputRequestTypeDef definition

class ListTagOptionsInputRequestTypeDef(TypedDict):
    Filters: NotRequired[ListTagOptionsFiltersTypeDef],  # (1)
    PageSize: NotRequired[int],
    PageToken: NotRequired[str],
```

1. See [:material-code-braces: ListTagOptionsFiltersTypeDef](./type_defs.md#listtagoptionsfilterstypedef) 
## ProvisioningArtifactParameterTypeDef

```python
# ProvisioningArtifactParameterTypeDef definition

class ProvisioningArtifactParameterTypeDef(TypedDict):
    ParameterKey: NotRequired[str],
    DefaultValue: NotRequired[str],
    ParameterType: NotRequired[str],
    IsNoEcho: NotRequired[bool],
    Description: NotRequired[str],
    ParameterConstraints: NotRequired[ParameterConstraintsTypeDef],  # (1)
```

1. See [:material-code-braces: ParameterConstraintsTypeDef](./type_defs.md#parameterconstraintstypedef) 
## SearchProductsOutputTypeDef

```python
# SearchProductsOutputTypeDef definition

class SearchProductsOutputTypeDef(TypedDict):
    ProductViewSummaries: List[ProductViewSummaryTypeDef],  # (1)
    ProductViewAggregations: Dict[str, List[ProductViewAggregationValueTypeDef]],  # (2)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProductViewSummaryTypeDef](./type_defs.md#productviewsummarytypedef) 
2. See [:material-code-braces: ProductViewAggregationValueTypeDef](./type_defs.md#productviewaggregationvaluetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisionProductInputRequestTypeDef

```python
# ProvisionProductInputRequestTypeDef definition

class ProvisionProductInputRequestTypeDef(TypedDict):
    ProvisionedProductName: str,
    ProvisionToken: str,
    AcceptLanguage: NotRequired[str],
    ProductId: NotRequired[str],
    ProductName: NotRequired[str],
    ProvisioningArtifactId: NotRequired[str],
    ProvisioningArtifactName: NotRequired[str],
    PathId: NotRequired[str],
    PathName: NotRequired[str],
    ProvisioningParameters: NotRequired[Sequence[ProvisioningParameterTypeDef]],  # (1)
    ProvisioningPreferences: NotRequired[ProvisioningPreferencesTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
    NotificationArns: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: ProvisioningParameterTypeDef](./type_defs.md#provisioningparametertypedef) 
2. See [:material-code-braces: ProvisioningPreferencesTypeDef](./type_defs.md#provisioningpreferencestypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## RecordDetailTypeDef

```python
# RecordDetailTypeDef definition

class RecordDetailTypeDef(TypedDict):
    RecordId: NotRequired[str],
    ProvisionedProductName: NotRequired[str],
    Status: NotRequired[RecordStatusType],  # (1)
    CreatedTime: NotRequired[datetime],
    UpdatedTime: NotRequired[datetime],
    ProvisionedProductType: NotRequired[str],
    RecordType: NotRequired[str],
    ProvisionedProductId: NotRequired[str],
    ProductId: NotRequired[str],
    ProvisioningArtifactId: NotRequired[str],
    PathId: NotRequired[str],
    RecordErrors: NotRequired[List[RecordErrorTypeDef]],  # (2)
    RecordTags: NotRequired[List[RecordTagTypeDef]],  # (3)
    LaunchRoleArn: NotRequired[str],
```

1. See [:material-code-brackets: RecordStatusType](./literals.md#recordstatustype) 
2. See [:material-code-braces: RecordErrorTypeDef](./type_defs.md#recorderrortypedef) 
3. See [:material-code-braces: RecordTagTypeDef](./type_defs.md#recordtagtypedef) 
## ResourceChangeDetailTypeDef

```python
# ResourceChangeDetailTypeDef definition

class ResourceChangeDetailTypeDef(TypedDict):
    Target: NotRequired[ResourceTargetDefinitionTypeDef],  # (1)
    Evaluation: NotRequired[EvaluationTypeType],  # (2)
    CausingEntity: NotRequired[str],
```

1. See [:material-code-braces: ResourceTargetDefinitionTypeDef](./type_defs.md#resourcetargetdefinitiontypedef) 
2. See [:material-code-brackets: EvaluationTypeType](./literals.md#evaluationtypetype) 
## ShareDetailsTypeDef

```python
# ShareDetailsTypeDef definition

class ShareDetailsTypeDef(TypedDict):
    SuccessfulShares: NotRequired[List[str]],
    ShareErrors: NotRequired[List[ShareErrorTypeDef]],  # (1)
```

1. See [:material-code-braces: ShareErrorTypeDef](./type_defs.md#shareerrortypedef) 
## UpdateProvisionedProductInputRequestTypeDef

```python
# UpdateProvisionedProductInputRequestTypeDef definition

class UpdateProvisionedProductInputRequestTypeDef(TypedDict):
    UpdateToken: str,
    AcceptLanguage: NotRequired[str],
    ProvisionedProductName: NotRequired[str],
    ProvisionedProductId: NotRequired[str],
    ProductId: NotRequired[str],
    ProductName: NotRequired[str],
    ProvisioningArtifactId: NotRequired[str],
    ProvisioningArtifactName: NotRequired[str],
    PathId: NotRequired[str],
    PathName: NotRequired[str],
    ProvisioningParameters: NotRequired[Sequence[UpdateProvisioningParameterTypeDef]],  # (1)
    ProvisioningPreferences: NotRequired[UpdateProvisioningPreferencesTypeDef],  # (2)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (3)
```

1. See [:material-code-braces: UpdateProvisioningParameterTypeDef](./type_defs.md#updateprovisioningparametertypedef) 
2. See [:material-code-braces: UpdateProvisioningPreferencesTypeDef](./type_defs.md#updateprovisioningpreferencestypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## SourceConnectionDetailTypeDef

```python
# SourceConnectionDetailTypeDef definition

class SourceConnectionDetailTypeDef(TypedDict):
    Type: NotRequired[SourceTypeType],  # (1)
    ConnectionParameters: NotRequired[SourceConnectionParametersTypeDef],  # (2)
    LastSync: NotRequired[LastSyncTypeDef],  # (3)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: SourceConnectionParametersTypeDef](./type_defs.md#sourceconnectionparameterstypedef) 
3. See [:material-code-braces: LastSyncTypeDef](./type_defs.md#lastsynctypedef) 
## SourceConnectionTypeDef

```python
# SourceConnectionTypeDef definition

class SourceConnectionTypeDef(TypedDict):
    ConnectionParameters: SourceConnectionParametersTypeDef,  # (2)
    Type: NotRequired[SourceTypeType],  # (1)
```

1. See [:material-code-brackets: SourceTypeType](./literals.md#sourcetypetype) 
2. See [:material-code-braces: SourceConnectionParametersTypeDef](./type_defs.md#sourceconnectionparameterstypedef) 
## ListLaunchPathsOutputTypeDef

```python
# ListLaunchPathsOutputTypeDef definition

class ListLaunchPathsOutputTypeDef(TypedDict):
    LaunchPathSummaries: List[LaunchPathSummaryTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: LaunchPathSummaryTypeDef](./type_defs.md#launchpathsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchProvisionedProductsOutputTypeDef

```python
# SearchProvisionedProductsOutputTypeDef definition

class SearchProvisionedProductsOutputTypeDef(TypedDict):
    ProvisionedProducts: List[ProvisionedProductAttributeTypeDef],  # (1)
    TotalResultsCount: int,
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisionedProductAttributeTypeDef](./type_defs.md#provisionedproductattributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProvisioningArtifactsForServiceActionOutputTypeDef

```python
# ListProvisioningArtifactsForServiceActionOutputTypeDef definition

class ListProvisioningArtifactsForServiceActionOutputTypeDef(TypedDict):
    ProvisioningArtifactViews: List[ProvisioningArtifactViewTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProvisioningArtifactViewTypeDef](./type_defs.md#provisioningartifactviewtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef

```python
# NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef definition

class NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef(TypedDict):
    WorkflowToken: str,
    RecordId: str,
    Status: EngineWorkflowStatusType,  # (1)
    IdempotencyToken: str,
    FailureReason: NotRequired[str],
    ResourceIdentifier: NotRequired[EngineWorkflowResourceIdentifierTypeDef],  # (2)
    Outputs: NotRequired[Sequence[RecordOutputTypeDef]],  # (3)
```

1. See [:material-code-brackets: EngineWorkflowStatusType](./literals.md#engineworkflowstatustype) 
2. See [:material-code-braces: EngineWorkflowResourceIdentifierTypeDef](./type_defs.md#engineworkflowresourceidentifiertypedef) 
3. See [:material-code-braces: RecordOutputTypeDef](./type_defs.md#recordoutputtypedef) 
## CreateServiceActionOutputTypeDef

```python
# CreateServiceActionOutputTypeDef definition

class CreateServiceActionOutputTypeDef(TypedDict):
    ServiceActionDetail: ServiceActionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceActionDetailTypeDef](./type_defs.md#serviceactiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeServiceActionOutputTypeDef

```python
# DescribeServiceActionOutputTypeDef definition

class DescribeServiceActionOutputTypeDef(TypedDict):
    ServiceActionDetail: ServiceActionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceActionDetailTypeDef](./type_defs.md#serviceactiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateServiceActionOutputTypeDef

```python
# UpdateServiceActionOutputTypeDef definition

class UpdateServiceActionOutputTypeDef(TypedDict):
    ServiceActionDetail: ServiceActionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceActionDetailTypeDef](./type_defs.md#serviceactiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProvisioningArtifactOutputTypeDef

```python
# DescribeProvisioningArtifactOutputTypeDef definition

class DescribeProvisioningArtifactOutputTypeDef(TypedDict):
    ProvisioningArtifactDetail: ProvisioningArtifactDetailTypeDef,  # (1)
    Info: Dict[str, str],
    Status: StatusType,  # (2)
    ProvisioningArtifactParameters: List[ProvisioningArtifactParameterTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ProvisioningArtifactDetailTypeDef](./type_defs.md#provisioningartifactdetailtypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: ProvisioningArtifactParameterTypeDef](./type_defs.md#provisioningartifactparametertypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProvisioningParametersOutputTypeDef

```python
# DescribeProvisioningParametersOutputTypeDef definition

class DescribeProvisioningParametersOutputTypeDef(TypedDict):
    ProvisioningArtifactParameters: List[ProvisioningArtifactParameterTypeDef],  # (1)
    ConstraintSummaries: List[ConstraintSummaryTypeDef],  # (2)
    UsageInstructions: List[UsageInstructionTypeDef],  # (3)
    TagOptions: List[TagOptionSummaryTypeDef],  # (4)
    ProvisioningArtifactPreferences: ProvisioningArtifactPreferencesTypeDef,  # (5)
    ProvisioningArtifactOutputs: List[ProvisioningArtifactOutputTypeDef],  # (6)
    ProvisioningArtifactOutputKeys: List[ProvisioningArtifactOutputTypeDef],  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (8)
```

1. See [:material-code-braces: ProvisioningArtifactParameterTypeDef](./type_defs.md#provisioningartifactparametertypedef) 
2. See [:material-code-braces: ConstraintSummaryTypeDef](./type_defs.md#constraintsummarytypedef) 
3. See [:material-code-braces: UsageInstructionTypeDef](./type_defs.md#usageinstructiontypedef) 
4. See [:material-code-braces: TagOptionSummaryTypeDef](./type_defs.md#tagoptionsummarytypedef) 
5. See [:material-code-braces: ProvisioningArtifactPreferencesTypeDef](./type_defs.md#provisioningartifactpreferencestypedef) 
6. See [:material-code-braces: ProvisioningArtifactOutputTypeDef](./type_defs.md#provisioningartifactoutputtypedef) 
7. See [:material-code-braces: ProvisioningArtifactOutputTypeDef](./type_defs.md#provisioningartifactoutputtypedef) 
8. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRecordOutputTypeDef

```python
# DescribeRecordOutputTypeDef definition

class DescribeRecordOutputTypeDef(TypedDict):
    RecordDetail: RecordDetailTypeDef,  # (1)
    RecordOutputs: List[RecordOutputTypeDef],  # (2)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: RecordDetailTypeDef](./type_defs.md#recorddetailtypedef) 
2. See [:material-code-braces: RecordOutputTypeDef](./type_defs.md#recordoutputtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteProvisionedProductPlanOutputTypeDef

```python
# ExecuteProvisionedProductPlanOutputTypeDef definition

class ExecuteProvisionedProductPlanOutputTypeDef(TypedDict):
    RecordDetail: RecordDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordDetailTypeDef](./type_defs.md#recorddetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteProvisionedProductServiceActionOutputTypeDef

```python
# ExecuteProvisionedProductServiceActionOutputTypeDef definition

class ExecuteProvisionedProductServiceActionOutputTypeDef(TypedDict):
    RecordDetail: RecordDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordDetailTypeDef](./type_defs.md#recorddetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ImportAsProvisionedProductOutputTypeDef

```python
# ImportAsProvisionedProductOutputTypeDef definition

class ImportAsProvisionedProductOutputTypeDef(TypedDict):
    RecordDetail: RecordDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordDetailTypeDef](./type_defs.md#recorddetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecordHistoryOutputTypeDef

```python
# ListRecordHistoryOutputTypeDef definition

class ListRecordHistoryOutputTypeDef(TypedDict):
    RecordDetails: List[RecordDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordDetailTypeDef](./type_defs.md#recorddetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisionProductOutputTypeDef

```python
# ProvisionProductOutputTypeDef definition

class ProvisionProductOutputTypeDef(TypedDict):
    RecordDetail: RecordDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordDetailTypeDef](./type_defs.md#recorddetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TerminateProvisionedProductOutputTypeDef

```python
# TerminateProvisionedProductOutputTypeDef definition

class TerminateProvisionedProductOutputTypeDef(TypedDict):
    RecordDetail: RecordDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordDetailTypeDef](./type_defs.md#recorddetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProvisionedProductOutputTypeDef

```python
# UpdateProvisionedProductOutputTypeDef definition

class UpdateProvisionedProductOutputTypeDef(TypedDict):
    RecordDetail: RecordDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecordDetailTypeDef](./type_defs.md#recorddetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceChangeTypeDef

```python
# ResourceChangeTypeDef definition

class ResourceChangeTypeDef(TypedDict):
    Action: NotRequired[ChangeActionType],  # (1)
    LogicalResourceId: NotRequired[str],
    PhysicalResourceId: NotRequired[str],
    ResourceType: NotRequired[str],
    Replacement: NotRequired[ReplacementType],  # (2)
    Scope: NotRequired[List[ResourceAttributeType]],  # (3)
    Details: NotRequired[List[ResourceChangeDetailTypeDef]],  # (4)
```

1. See [:material-code-brackets: ChangeActionType](./literals.md#changeactiontype) 
2. See [:material-code-brackets: ReplacementType](./literals.md#replacementtype) 
3. See [:material-code-brackets: ResourceAttributeType](./literals.md#resourceattributetype) 
4. See [:material-code-braces: ResourceChangeDetailTypeDef](./type_defs.md#resourcechangedetailtypedef) 
## DescribePortfolioShareStatusOutputTypeDef

```python
# DescribePortfolioShareStatusOutputTypeDef definition

class DescribePortfolioShareStatusOutputTypeDef(TypedDict):
    PortfolioShareToken: str,
    PortfolioId: str,
    OrganizationNodeValue: str,
    Status: ShareStatusType,  # (1)
    ShareDetails: ShareDetailsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-braces: ShareDetailsTypeDef](./type_defs.md#sharedetailstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProductViewDetailTypeDef

```python
# ProductViewDetailTypeDef definition

class ProductViewDetailTypeDef(TypedDict):
    ProductViewSummary: NotRequired[ProductViewSummaryTypeDef],  # (1)
    Status: NotRequired[StatusType],  # (2)
    ProductARN: NotRequired[str],
    CreatedTime: NotRequired[datetime],
    SourceConnection: NotRequired[SourceConnectionDetailTypeDef],  # (3)
```

1. See [:material-code-braces: ProductViewSummaryTypeDef](./type_defs.md#productviewsummarytypedef) 
2. See [:material-code-brackets: StatusType](./literals.md#statustype) 
3. See [:material-code-braces: SourceConnectionDetailTypeDef](./type_defs.md#sourceconnectiondetailtypedef) 
## CreateProductInputRequestTypeDef

```python
# CreateProductInputRequestTypeDef definition

class CreateProductInputRequestTypeDef(TypedDict):
    Name: str,
    Owner: str,
    ProductType: ProductTypeType,  # (1)
    IdempotencyToken: str,
    AcceptLanguage: NotRequired[str],
    Description: NotRequired[str],
    Distributor: NotRequired[str],
    SupportDescription: NotRequired[str],
    SupportEmail: NotRequired[str],
    SupportUrl: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
    ProvisioningArtifactParameters: NotRequired[ProvisioningArtifactPropertiesTypeDef],  # (3)
    SourceConnection: NotRequired[SourceConnectionTypeDef],  # (4)
```

1. See [:material-code-brackets: ProductTypeType](./literals.md#producttypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ProvisioningArtifactPropertiesTypeDef](./type_defs.md#provisioningartifactpropertiestypedef) 
4. See [:material-code-braces: SourceConnectionTypeDef](./type_defs.md#sourceconnectiontypedef) 
## UpdateProductInputRequestTypeDef

```python
# UpdateProductInputRequestTypeDef definition

class UpdateProductInputRequestTypeDef(TypedDict):
    Id: str,
    AcceptLanguage: NotRequired[str],
    Name: NotRequired[str],
    Owner: NotRequired[str],
    Description: NotRequired[str],
    Distributor: NotRequired[str],
    SupportDescription: NotRequired[str],
    SupportEmail: NotRequired[str],
    SupportUrl: NotRequired[str],
    AddTags: NotRequired[Sequence[TagTypeDef]],  # (1)
    RemoveTags: NotRequired[Sequence[str]],
    SourceConnection: NotRequired[SourceConnectionTypeDef],  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: SourceConnectionTypeDef](./type_defs.md#sourceconnectiontypedef) 
## DescribeProvisionedProductPlanOutputTypeDef

```python
# DescribeProvisionedProductPlanOutputTypeDef definition

class DescribeProvisionedProductPlanOutputTypeDef(TypedDict):
    ProvisionedProductPlanDetails: ProvisionedProductPlanDetailsTypeDef,  # (1)
    ResourceChanges: List[ResourceChangeTypeDef],  # (2)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProvisionedProductPlanDetailsTypeDef](./type_defs.md#provisionedproductplandetailstypedef) 
2. See [:material-code-braces: ResourceChangeTypeDef](./type_defs.md#resourcechangetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProductOutputTypeDef

```python
# CreateProductOutputTypeDef definition

class CreateProductOutputTypeDef(TypedDict):
    ProductViewDetail: ProductViewDetailTypeDef,  # (1)
    ProvisioningArtifactDetail: ProvisioningArtifactDetailTypeDef,  # (2)
    Tags: List[TagTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: ProductViewDetailTypeDef](./type_defs.md#productviewdetailtypedef) 
2. See [:material-code-braces: ProvisioningArtifactDetailTypeDef](./type_defs.md#provisioningartifactdetailtypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeProductAsAdminOutputTypeDef

```python
# DescribeProductAsAdminOutputTypeDef definition

class DescribeProductAsAdminOutputTypeDef(TypedDict):
    ProductViewDetail: ProductViewDetailTypeDef,  # (1)
    ProvisioningArtifactSummaries: List[ProvisioningArtifactSummaryTypeDef],  # (2)
    Tags: List[TagTypeDef],  # (3)
    TagOptions: List[TagOptionDetailTypeDef],  # (4)
    Budgets: List[BudgetDetailTypeDef],  # (5)
    ResponseMetadata: ResponseMetadataTypeDef,  # (6)
```

1. See [:material-code-braces: ProductViewDetailTypeDef](./type_defs.md#productviewdetailtypedef) 
2. See [:material-code-braces: ProvisioningArtifactSummaryTypeDef](./type_defs.md#provisioningartifactsummarytypedef) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: TagOptionDetailTypeDef](./type_defs.md#tagoptiondetailtypedef) 
5. See [:material-code-braces: BudgetDetailTypeDef](./type_defs.md#budgetdetailtypedef) 
6. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SearchProductsAsAdminOutputTypeDef

```python
# SearchProductsAsAdminOutputTypeDef definition

class SearchProductsAsAdminOutputTypeDef(TypedDict):
    ProductViewDetails: List[ProductViewDetailTypeDef],  # (1)
    NextPageToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProductViewDetailTypeDef](./type_defs.md#productviewdetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProductOutputTypeDef

```python
# UpdateProductOutputTypeDef definition

class UpdateProductOutputTypeDef(TypedDict):
    ProductViewDetail: ProductViewDetailTypeDef,  # (1)
    Tags: List[TagTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ProductViewDetailTypeDef](./type_defs.md#productviewdetailtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

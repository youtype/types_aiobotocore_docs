# Type definitions

> [Index](../README.md) > [TrustedAdvisorPublicAPI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TrustedAdvisorPublicAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#trustedadvisorpublicapi)
    type annotations stubs module [types-aiobotocore-trustedadvisor](https://pypi.org/project/types-aiobotocore-trustedadvisor/).

## TimestampTypeDef

```python
# TimestampTypeDef Union usage example

from types_aiobotocore_trustedadvisor.type_defs import TimestampTypeDef


def get_value() -> TimestampTypeDef:
    return ...


# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccountRecommendationLifecycleSummaryTypeDef

```python
# AccountRecommendationLifecycleSummaryTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import AccountRecommendationLifecycleSummaryTypeDef


def get_value() -> AccountRecommendationLifecycleSummaryTypeDef:
    return {
        "accountId": ...,
    }


# AccountRecommendationLifecycleSummaryTypeDef definition

class AccountRecommendationLifecycleSummaryTypeDef(TypedDict):
    accountId: NotRequired[str],
    accountRecommendationArn: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    lifecycleStage: NotRequired[RecommendationLifecycleStageType],  # (1)
    updateReason: NotRequired[str],
    updateReasonCode: NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],  # (2)
    updatedOnBehalfOf: NotRequired[str],
    updatedOnBehalfOfJobTitle: NotRequired[str],
```

1. See [:material-code-brackets: RecommendationLifecycleStageType](./literals.md#recommendationlifecyclestagetype) 
2. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
## RecommendationResourceExclusionTypeDef

```python
# RecommendationResourceExclusionTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import RecommendationResourceExclusionTypeDef


def get_value() -> RecommendationResourceExclusionTypeDef:
    return {
        "arn": ...,
    }


# RecommendationResourceExclusionTypeDef definition

class RecommendationResourceExclusionTypeDef(TypedDict):
    arn: str,
    isExcluded: bool,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ResponseMetadataTypeDef


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

## UpdateRecommendationResourceExclusionErrorTypeDef

```python
# UpdateRecommendationResourceExclusionErrorTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import UpdateRecommendationResourceExclusionErrorTypeDef


def get_value() -> UpdateRecommendationResourceExclusionErrorTypeDef:
    return {
        "arn": ...,
    }


# UpdateRecommendationResourceExclusionErrorTypeDef definition

class UpdateRecommendationResourceExclusionErrorTypeDef(TypedDict):
    arn: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## CheckSummaryTypeDef

```python
# CheckSummaryTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import CheckSummaryTypeDef


def get_value() -> CheckSummaryTypeDef:
    return {
        "arn": ...,
    }


# CheckSummaryTypeDef definition

class CheckSummaryTypeDef(TypedDict):
    arn: str,
    awsServices: List[str],
    description: str,
    id: str,
    metadata: Dict[str, str],
    name: str,
    pillars: List[RecommendationPillarType],  # (1)
    source: RecommendationSourceType,  # (2)
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
## GetOrganizationRecommendationRequestTypeDef

```python
# GetOrganizationRecommendationRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import GetOrganizationRecommendationRequestTypeDef


def get_value() -> GetOrganizationRecommendationRequestTypeDef:
    return {
        "organizationRecommendationIdentifier": ...,
    }


# GetOrganizationRecommendationRequestTypeDef definition

class GetOrganizationRecommendationRequestTypeDef(TypedDict):
    organizationRecommendationIdentifier: str,
```

## GetRecommendationRequestTypeDef

```python
# GetRecommendationRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import GetRecommendationRequestTypeDef


def get_value() -> GetRecommendationRequestTypeDef:
    return {
        "recommendationIdentifier": ...,
    }


# GetRecommendationRequestTypeDef definition

class GetRecommendationRequestTypeDef(TypedDict):
    recommendationIdentifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import PaginatorConfigTypeDef


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

## ListChecksRequestTypeDef

```python
# ListChecksRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListChecksRequestTypeDef


def get_value() -> ListChecksRequestTypeDef:
    return {
        "awsService": ...,
    }


# ListChecksRequestTypeDef definition

class ListChecksRequestTypeDef(TypedDict):
    awsService: NotRequired[str],
    language: NotRequired[RecommendationLanguageType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    pillar: NotRequired[RecommendationPillarType],  # (2)
    source: NotRequired[RecommendationSourceType],  # (3)
```

1. See [:material-code-brackets: RecommendationLanguageType](./literals.md#recommendationlanguagetype) 
2. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
3. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
## ListOrganizationRecommendationAccountsRequestTypeDef

```python
# ListOrganizationRecommendationAccountsRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationAccountsRequestTypeDef


def get_value() -> ListOrganizationRecommendationAccountsRequestTypeDef:
    return {
        "organizationRecommendationIdentifier": ...,
    }


# ListOrganizationRecommendationAccountsRequestTypeDef definition

class ListOrganizationRecommendationAccountsRequestTypeDef(TypedDict):
    organizationRecommendationIdentifier: str,
    affectedAccountId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListOrganizationRecommendationResourcesRequestTypeDef

```python
# ListOrganizationRecommendationResourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationResourcesRequestTypeDef


def get_value() -> ListOrganizationRecommendationResourcesRequestTypeDef:
    return {
        "organizationRecommendationIdentifier": ...,
    }


# ListOrganizationRecommendationResourcesRequestTypeDef definition

class ListOrganizationRecommendationResourcesRequestTypeDef(TypedDict):
    organizationRecommendationIdentifier: str,
    affectedAccountId: NotRequired[str],
    exclusionStatus: NotRequired[ExclusionStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    regionCode: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (2)
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## OrganizationRecommendationResourceSummaryTypeDef

```python
# OrganizationRecommendationResourceSummaryTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import OrganizationRecommendationResourceSummaryTypeDef


def get_value() -> OrganizationRecommendationResourceSummaryTypeDef:
    return {
        "accountId": ...,
    }


# OrganizationRecommendationResourceSummaryTypeDef definition

class OrganizationRecommendationResourceSummaryTypeDef(TypedDict):
    arn: str,
    awsResourceId: str,
    id: str,
    lastUpdatedAt: datetime,
    metadata: Dict[str, str],
    recommendationArn: str,
    regionCode: str,
    status: ResourceStatusType,  # (2)
    accountId: NotRequired[str],
    exclusionStatus: NotRequired[ExclusionStatusType],  # (1)
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## ListRecommendationResourcesRequestTypeDef

```python
# ListRecommendationResourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListRecommendationResourcesRequestTypeDef


def get_value() -> ListRecommendationResourcesRequestTypeDef:
    return {
        "recommendationIdentifier": ...,
    }


# ListRecommendationResourcesRequestTypeDef definition

class ListRecommendationResourcesRequestTypeDef(TypedDict):
    recommendationIdentifier: str,
    exclusionStatus: NotRequired[ExclusionStatusType],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    regionCode: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (2)
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## RecommendationResourceSummaryTypeDef

```python
# RecommendationResourceSummaryTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import RecommendationResourceSummaryTypeDef


def get_value() -> RecommendationResourceSummaryTypeDef:
    return {
        "arn": ...,
    }


# RecommendationResourceSummaryTypeDef definition

class RecommendationResourceSummaryTypeDef(TypedDict):
    arn: str,
    awsResourceId: str,
    id: str,
    lastUpdatedAt: datetime,
    metadata: Dict[str, str],
    recommendationArn: str,
    regionCode: str,
    status: ResourceStatusType,  # (2)
    exclusionStatus: NotRequired[ExclusionStatusType],  # (1)
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
## RecommendationResourcesAggregatesTypeDef

```python
# RecommendationResourcesAggregatesTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import RecommendationResourcesAggregatesTypeDef


def get_value() -> RecommendationResourcesAggregatesTypeDef:
    return {
        "errorCount": ...,
    }


# RecommendationResourcesAggregatesTypeDef definition

class RecommendationResourcesAggregatesTypeDef(TypedDict):
    errorCount: int,
    okCount: int,
    warningCount: int,
```

## RecommendationCostOptimizingAggregatesTypeDef

```python
# RecommendationCostOptimizingAggregatesTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import RecommendationCostOptimizingAggregatesTypeDef


def get_value() -> RecommendationCostOptimizingAggregatesTypeDef:
    return {
        "estimatedMonthlySavings": ...,
    }


# RecommendationCostOptimizingAggregatesTypeDef definition

class RecommendationCostOptimizingAggregatesTypeDef(TypedDict):
    estimatedMonthlySavings: float,
    estimatedPercentMonthlySavings: float,
```

## UpdateOrganizationRecommendationLifecycleRequestTypeDef

```python
# UpdateOrganizationRecommendationLifecycleRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import UpdateOrganizationRecommendationLifecycleRequestTypeDef


def get_value() -> UpdateOrganizationRecommendationLifecycleRequestTypeDef:
    return {
        "lifecycleStage": ...,
    }


# UpdateOrganizationRecommendationLifecycleRequestTypeDef definition

class UpdateOrganizationRecommendationLifecycleRequestTypeDef(TypedDict):
    lifecycleStage: UpdateRecommendationLifecycleStageType,  # (1)
    organizationRecommendationIdentifier: str,
    updateReason: NotRequired[str],
    updateReasonCode: NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],  # (2)
```

1. See [:material-code-brackets: UpdateRecommendationLifecycleStageType](./literals.md#updaterecommendationlifecyclestagetype) 
2. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
## UpdateRecommendationLifecycleRequestTypeDef

```python
# UpdateRecommendationLifecycleRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import UpdateRecommendationLifecycleRequestTypeDef


def get_value() -> UpdateRecommendationLifecycleRequestTypeDef:
    return {
        "lifecycleStage": ...,
    }


# UpdateRecommendationLifecycleRequestTypeDef definition

class UpdateRecommendationLifecycleRequestTypeDef(TypedDict):
    lifecycleStage: UpdateRecommendationLifecycleStageType,  # (1)
    recommendationIdentifier: str,
    updateReason: NotRequired[str],
    updateReasonCode: NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],  # (2)
```

1. See [:material-code-brackets: UpdateRecommendationLifecycleStageType](./literals.md#updaterecommendationlifecyclestagetype) 
2. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
## BatchUpdateRecommendationResourceExclusionRequestTypeDef

```python
# BatchUpdateRecommendationResourceExclusionRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import BatchUpdateRecommendationResourceExclusionRequestTypeDef


def get_value() -> BatchUpdateRecommendationResourceExclusionRequestTypeDef:
    return {
        "recommendationResourceExclusions": ...,
    }


# BatchUpdateRecommendationResourceExclusionRequestTypeDef definition

class BatchUpdateRecommendationResourceExclusionRequestTypeDef(TypedDict):
    recommendationResourceExclusions: Sequence[RecommendationResourceExclusionTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationResourceExclusionTypeDef](./type_defs.md#recommendationresourceexclusiontypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationRecommendationAccountsResponseTypeDef

```python
# ListOrganizationRecommendationAccountsResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationAccountsResponseTypeDef


def get_value() -> ListOrganizationRecommendationAccountsResponseTypeDef:
    return {
        "accountRecommendationLifecycleSummaries": ...,
    }


# ListOrganizationRecommendationAccountsResponseTypeDef definition

class ListOrganizationRecommendationAccountsResponseTypeDef(TypedDict):
    accountRecommendationLifecycleSummaries: List[AccountRecommendationLifecycleSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: AccountRecommendationLifecycleSummaryTypeDef](./type_defs.md#accountrecommendationlifecyclesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchUpdateRecommendationResourceExclusionResponseTypeDef

```python
# BatchUpdateRecommendationResourceExclusionResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import BatchUpdateRecommendationResourceExclusionResponseTypeDef


def get_value() -> BatchUpdateRecommendationResourceExclusionResponseTypeDef:
    return {
        "batchUpdateRecommendationResourceExclusionErrors": ...,
    }


# BatchUpdateRecommendationResourceExclusionResponseTypeDef definition

class BatchUpdateRecommendationResourceExclusionResponseTypeDef(TypedDict):
    batchUpdateRecommendationResourceExclusionErrors: List[UpdateRecommendationResourceExclusionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateRecommendationResourceExclusionErrorTypeDef](./type_defs.md#updaterecommendationresourceexclusionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChecksResponseTypeDef

```python
# ListChecksResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListChecksResponseTypeDef


def get_value() -> ListChecksResponseTypeDef:
    return {
        "checkSummaries": ...,
    }


# ListChecksResponseTypeDef definition

class ListChecksResponseTypeDef(TypedDict):
    checkSummaries: List[CheckSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: CheckSummaryTypeDef](./type_defs.md#checksummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChecksRequestPaginateTypeDef

```python
# ListChecksRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListChecksRequestPaginateTypeDef


def get_value() -> ListChecksRequestPaginateTypeDef:
    return {
        "awsService": ...,
    }


# ListChecksRequestPaginateTypeDef definition

class ListChecksRequestPaginateTypeDef(TypedDict):
    awsService: NotRequired[str],
    language: NotRequired[RecommendationLanguageType],  # (1)
    pillar: NotRequired[RecommendationPillarType],  # (2)
    source: NotRequired[RecommendationSourceType],  # (3)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: RecommendationLanguageType](./literals.md#recommendationlanguagetype) 
2. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
3. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationRecommendationAccountsRequestPaginateTypeDef

```python
# ListOrganizationRecommendationAccountsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationAccountsRequestPaginateTypeDef


def get_value() -> ListOrganizationRecommendationAccountsRequestPaginateTypeDef:
    return {
        "organizationRecommendationIdentifier": ...,
    }


# ListOrganizationRecommendationAccountsRequestPaginateTypeDef definition

class ListOrganizationRecommendationAccountsRequestPaginateTypeDef(TypedDict):
    organizationRecommendationIdentifier: str,
    affectedAccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationRecommendationResourcesRequestPaginateTypeDef

```python
# ListOrganizationRecommendationResourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationResourcesRequestPaginateTypeDef


def get_value() -> ListOrganizationRecommendationResourcesRequestPaginateTypeDef:
    return {
        "organizationRecommendationIdentifier": ...,
    }


# ListOrganizationRecommendationResourcesRequestPaginateTypeDef definition

class ListOrganizationRecommendationResourcesRequestPaginateTypeDef(TypedDict):
    organizationRecommendationIdentifier: str,
    affectedAccountId: NotRequired[str],
    exclusionStatus: NotRequired[ExclusionStatusType],  # (1)
    regionCode: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationResourcesRequestPaginateTypeDef

```python
# ListRecommendationResourcesRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListRecommendationResourcesRequestPaginateTypeDef


def get_value() -> ListRecommendationResourcesRequestPaginateTypeDef:
    return {
        "recommendationIdentifier": ...,
    }


# ListRecommendationResourcesRequestPaginateTypeDef definition

class ListRecommendationResourcesRequestPaginateTypeDef(TypedDict):
    recommendationIdentifier: str,
    exclusionStatus: NotRequired[ExclusionStatusType],  # (1)
    regionCode: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ExclusionStatusType](./literals.md#exclusionstatustype) 
2. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationRecommendationResourcesResponseTypeDef

```python
# ListOrganizationRecommendationResourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationResourcesResponseTypeDef


def get_value() -> ListOrganizationRecommendationResourcesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListOrganizationRecommendationResourcesResponseTypeDef definition

class ListOrganizationRecommendationResourcesResponseTypeDef(TypedDict):
    organizationRecommendationResourceSummaries: List[OrganizationRecommendationResourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationRecommendationResourceSummaryTypeDef](./type_defs.md#organizationrecommendationresourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationRecommendationsRequestPaginateTypeDef

```python
# ListOrganizationRecommendationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationsRequestPaginateTypeDef


def get_value() -> ListOrganizationRecommendationsRequestPaginateTypeDef:
    return {
        "afterLastUpdatedAt": ...,
    }


# ListOrganizationRecommendationsRequestPaginateTypeDef definition

class ListOrganizationRecommendationsRequestPaginateTypeDef(TypedDict):
    afterLastUpdatedAt: NotRequired[TimestampTypeDef],
    awsService: NotRequired[str],
    beforeLastUpdatedAt: NotRequired[TimestampTypeDef],
    checkIdentifier: NotRequired[str],
    pillar: NotRequired[RecommendationPillarType],  # (1)
    source: NotRequired[RecommendationSourceType],  # (2)
    status: NotRequired[RecommendationStatusType],  # (3)
    type: NotRequired[RecommendationTypeType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationRecommendationsRequestTypeDef

```python
# ListOrganizationRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationsRequestTypeDef


def get_value() -> ListOrganizationRecommendationsRequestTypeDef:
    return {
        "afterLastUpdatedAt": ...,
    }


# ListOrganizationRecommendationsRequestTypeDef definition

class ListOrganizationRecommendationsRequestTypeDef(TypedDict):
    afterLastUpdatedAt: NotRequired[TimestampTypeDef],
    awsService: NotRequired[str],
    beforeLastUpdatedAt: NotRequired[TimestampTypeDef],
    checkIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    pillar: NotRequired[RecommendationPillarType],  # (1)
    source: NotRequired[RecommendationSourceType],  # (2)
    status: NotRequired[RecommendationStatusType],  # (3)
    type: NotRequired[RecommendationTypeType],  # (4)
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
## ListRecommendationsRequestPaginateTypeDef

```python
# ListRecommendationsRequestPaginateTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListRecommendationsRequestPaginateTypeDef


def get_value() -> ListRecommendationsRequestPaginateTypeDef:
    return {
        "afterLastUpdatedAt": ...,
    }


# ListRecommendationsRequestPaginateTypeDef definition

class ListRecommendationsRequestPaginateTypeDef(TypedDict):
    afterLastUpdatedAt: NotRequired[TimestampTypeDef],
    awsService: NotRequired[str],
    beforeLastUpdatedAt: NotRequired[TimestampTypeDef],
    checkIdentifier: NotRequired[str],
    pillar: NotRequired[RecommendationPillarType],  # (1)
    source: NotRequired[RecommendationSourceType],  # (2)
    status: NotRequired[RecommendationStatusType],  # (3)
    type: NotRequired[RecommendationTypeType],  # (4)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecommendationsRequestTypeDef

```python
# ListRecommendationsRequestTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListRecommendationsRequestTypeDef


def get_value() -> ListRecommendationsRequestTypeDef:
    return {
        "afterLastUpdatedAt": ...,
    }


# ListRecommendationsRequestTypeDef definition

class ListRecommendationsRequestTypeDef(TypedDict):
    afterLastUpdatedAt: NotRequired[TimestampTypeDef],
    awsService: NotRequired[str],
    beforeLastUpdatedAt: NotRequired[TimestampTypeDef],
    checkIdentifier: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
    pillar: NotRequired[RecommendationPillarType],  # (1)
    source: NotRequired[RecommendationSourceType],  # (2)
    status: NotRequired[RecommendationStatusType],  # (3)
    type: NotRequired[RecommendationTypeType],  # (4)
```

1. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
2. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
3. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
4. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
## ListRecommendationResourcesResponseTypeDef

```python
# ListRecommendationResourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListRecommendationResourcesResponseTypeDef


def get_value() -> ListRecommendationResourcesResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListRecommendationResourcesResponseTypeDef definition

class ListRecommendationResourcesResponseTypeDef(TypedDict):
    recommendationResourceSummaries: List[RecommendationResourceSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationResourceSummaryTypeDef](./type_defs.md#recommendationresourcesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RecommendationPillarSpecificAggregatesTypeDef

```python
# RecommendationPillarSpecificAggregatesTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import RecommendationPillarSpecificAggregatesTypeDef


def get_value() -> RecommendationPillarSpecificAggregatesTypeDef:
    return {
        "costOptimizing": ...,
    }


# RecommendationPillarSpecificAggregatesTypeDef definition

class RecommendationPillarSpecificAggregatesTypeDef(TypedDict):
    costOptimizing: NotRequired[RecommendationCostOptimizingAggregatesTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationCostOptimizingAggregatesTypeDef](./type_defs.md#recommendationcostoptimizingaggregatestypedef) 
## OrganizationRecommendationSummaryTypeDef

```python
# OrganizationRecommendationSummaryTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import OrganizationRecommendationSummaryTypeDef


def get_value() -> OrganizationRecommendationSummaryTypeDef:
    return {
        "arn": ...,
    }


# OrganizationRecommendationSummaryTypeDef definition

class OrganizationRecommendationSummaryTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    pillars: List[RecommendationPillarType],  # (3)
    resourcesAggregates: RecommendationResourcesAggregatesTypeDef,  # (4)
    source: RecommendationSourceType,  # (5)
    status: RecommendationStatusType,  # (6)
    type: RecommendationTypeType,  # (7)
    awsServices: NotRequired[List[str]],
    checkArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    lifecycleStage: NotRequired[RecommendationLifecycleStageType],  # (1)
    pillarSpecificAggregates: NotRequired[RecommendationPillarSpecificAggregatesTypeDef],  # (2)
```

1. See [:material-code-brackets: RecommendationLifecycleStageType](./literals.md#recommendationlifecyclestagetype) 
2. See [:material-code-braces: RecommendationPillarSpecificAggregatesTypeDef](./type_defs.md#recommendationpillarspecificaggregatestypedef) 
3. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
4. See [:material-code-braces: RecommendationResourcesAggregatesTypeDef](./type_defs.md#recommendationresourcesaggregatestypedef) 
5. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
6. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
7. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
## OrganizationRecommendationTypeDef

```python
# OrganizationRecommendationTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import OrganizationRecommendationTypeDef


def get_value() -> OrganizationRecommendationTypeDef:
    return {
        "arn": ...,
    }


# OrganizationRecommendationTypeDef definition

class OrganizationRecommendationTypeDef(TypedDict):
    arn: str,
    description: str,
    id: str,
    name: str,
    pillars: List[RecommendationPillarType],  # (3)
    resourcesAggregates: RecommendationResourcesAggregatesTypeDef,  # (4)
    source: RecommendationSourceType,  # (5)
    status: RecommendationStatusType,  # (6)
    type: RecommendationTypeType,  # (7)
    awsServices: NotRequired[List[str]],
    checkArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    lifecycleStage: NotRequired[RecommendationLifecycleStageType],  # (1)
    pillarSpecificAggregates: NotRequired[RecommendationPillarSpecificAggregatesTypeDef],  # (2)
    resolvedAt: NotRequired[datetime],
    updateReason: NotRequired[str],
    updateReasonCode: NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],  # (8)
    updatedOnBehalfOf: NotRequired[str],
    updatedOnBehalfOfJobTitle: NotRequired[str],
```

1. See [:material-code-brackets: RecommendationLifecycleStageType](./literals.md#recommendationlifecyclestagetype) 
2. See [:material-code-braces: RecommendationPillarSpecificAggregatesTypeDef](./type_defs.md#recommendationpillarspecificaggregatestypedef) 
3. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
4. See [:material-code-braces: RecommendationResourcesAggregatesTypeDef](./type_defs.md#recommendationresourcesaggregatestypedef) 
5. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
6. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
7. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
8. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
## RecommendationSummaryTypeDef

```python
# RecommendationSummaryTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import RecommendationSummaryTypeDef


def get_value() -> RecommendationSummaryTypeDef:
    return {
        "arn": ...,
    }


# RecommendationSummaryTypeDef definition

class RecommendationSummaryTypeDef(TypedDict):
    arn: str,
    id: str,
    name: str,
    pillars: List[RecommendationPillarType],  # (3)
    resourcesAggregates: RecommendationResourcesAggregatesTypeDef,  # (4)
    source: RecommendationSourceType,  # (5)
    status: RecommendationStatusType,  # (6)
    type: RecommendationTypeType,  # (7)
    awsServices: NotRequired[List[str]],
    checkArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    lastUpdatedAt: NotRequired[datetime],
    lifecycleStage: NotRequired[RecommendationLifecycleStageType],  # (1)
    pillarSpecificAggregates: NotRequired[RecommendationPillarSpecificAggregatesTypeDef],  # (2)
```

1. See [:material-code-brackets: RecommendationLifecycleStageType](./literals.md#recommendationlifecyclestagetype) 
2. See [:material-code-braces: RecommendationPillarSpecificAggregatesTypeDef](./type_defs.md#recommendationpillarspecificaggregatestypedef) 
3. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
4. See [:material-code-braces: RecommendationResourcesAggregatesTypeDef](./type_defs.md#recommendationresourcesaggregatestypedef) 
5. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
6. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
7. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
## RecommendationTypeDef

```python
# RecommendationTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import RecommendationTypeDef


def get_value() -> RecommendationTypeDef:
    return {
        "arn": ...,
    }


# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    arn: str,
    description: str,
    id: str,
    name: str,
    pillars: List[RecommendationPillarType],  # (3)
    resourcesAggregates: RecommendationResourcesAggregatesTypeDef,  # (4)
    source: RecommendationSourceType,  # (5)
    status: RecommendationStatusType,  # (6)
    type: RecommendationTypeType,  # (7)
    awsServices: NotRequired[List[str]],
    checkArn: NotRequired[str],
    createdAt: NotRequired[datetime],
    createdBy: NotRequired[str],
    lastUpdatedAt: NotRequired[datetime],
    lifecycleStage: NotRequired[RecommendationLifecycleStageType],  # (1)
    pillarSpecificAggregates: NotRequired[RecommendationPillarSpecificAggregatesTypeDef],  # (2)
    resolvedAt: NotRequired[datetime],
    updateReason: NotRequired[str],
    updateReasonCode: NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],  # (8)
    updatedOnBehalfOf: NotRequired[str],
    updatedOnBehalfOfJobTitle: NotRequired[str],
```

1. See [:material-code-brackets: RecommendationLifecycleStageType](./literals.md#recommendationlifecyclestagetype) 
2. See [:material-code-braces: RecommendationPillarSpecificAggregatesTypeDef](./type_defs.md#recommendationpillarspecificaggregatestypedef) 
3. See [:material-code-brackets: RecommendationPillarType](./literals.md#recommendationpillartype) 
4. See [:material-code-braces: RecommendationResourcesAggregatesTypeDef](./type_defs.md#recommendationresourcesaggregatestypedef) 
5. See [:material-code-brackets: RecommendationSourceType](./literals.md#recommendationsourcetype) 
6. See [:material-code-brackets: RecommendationStatusType](./literals.md#recommendationstatustype) 
7. See [:material-code-brackets: RecommendationTypeType](./literals.md#recommendationtypetype) 
8. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
## ListOrganizationRecommendationsResponseTypeDef

```python
# ListOrganizationRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListOrganizationRecommendationsResponseTypeDef


def get_value() -> ListOrganizationRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListOrganizationRecommendationsResponseTypeDef definition

class ListOrganizationRecommendationsResponseTypeDef(TypedDict):
    organizationRecommendationSummaries: List[OrganizationRecommendationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: OrganizationRecommendationSummaryTypeDef](./type_defs.md#organizationrecommendationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetOrganizationRecommendationResponseTypeDef

```python
# GetOrganizationRecommendationResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import GetOrganizationRecommendationResponseTypeDef


def get_value() -> GetOrganizationRecommendationResponseTypeDef:
    return {
        "organizationRecommendation": ...,
    }


# GetOrganizationRecommendationResponseTypeDef definition

class GetOrganizationRecommendationResponseTypeDef(TypedDict):
    organizationRecommendation: OrganizationRecommendationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationRecommendationTypeDef](./type_defs.md#organizationrecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecommendationsResponseTypeDef

```python
# ListRecommendationsResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import ListRecommendationsResponseTypeDef


def get_value() -> ListRecommendationsResponseTypeDef:
    return {
        "nextToken": ...,
    }


# ListRecommendationsResponseTypeDef definition

class ListRecommendationsResponseTypeDef(TypedDict):
    recommendationSummaries: List[RecommendationSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationSummaryTypeDef](./type_defs.md#recommendationsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecommendationResponseTypeDef

```python
# GetRecommendationResponseTypeDef TypedDict usage example

from types_aiobotocore_trustedadvisor.type_defs import GetRecommendationResponseTypeDef


def get_value() -> GetRecommendationResponseTypeDef:
    return {
        "recommendation": ...,
    }


# GetRecommendationResponseTypeDef definition

class GetRecommendationResponseTypeDef(TypedDict):
    recommendation: RecommendationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

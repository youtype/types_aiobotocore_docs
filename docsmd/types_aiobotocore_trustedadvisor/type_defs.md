# Type definitions

> [Index](../README.md) > [TrustedAdvisorPublicAPI](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [TrustedAdvisorPublicAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/trustedadvisor.html#trustedadvisorpublicapi)
    type annotations stubs module [types-aiobotocore-trustedadvisor](https://pypi.org/project/types-aiobotocore-trustedadvisor/).

## TimestampTypeDef

```python
# TimestampTypeDef definition

TimestampTypeDef = Union[
    datetime,
    str,
]
```




## AccountRecommendationLifecycleSummaryTypeDef

```python
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
# RecommendationResourceExclusionTypeDef definition

class RecommendationResourceExclusionTypeDef(TypedDict):
    arn: str,
    isExcluded: bool,
```

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

## UpdateRecommendationResourceExclusionErrorTypeDef

```python
# UpdateRecommendationResourceExclusionErrorTypeDef definition

class UpdateRecommendationResourceExclusionErrorTypeDef(TypedDict):
    arn: NotRequired[str],
    errorCode: NotRequired[str],
    errorMessage: NotRequired[str],
```

## CheckSummaryTypeDef

```python
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
## GetOrganizationRecommendationRequestRequestTypeDef

```python
# GetOrganizationRecommendationRequestRequestTypeDef definition

class GetOrganizationRecommendationRequestRequestTypeDef(TypedDict):
    organizationRecommendationIdentifier: str,
```

## GetRecommendationRequestRequestTypeDef

```python
# GetRecommendationRequestRequestTypeDef definition

class GetRecommendationRequestRequestTypeDef(TypedDict):
    recommendationIdentifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListChecksRequestRequestTypeDef

```python
# ListChecksRequestRequestTypeDef definition

class ListChecksRequestRequestTypeDef(TypedDict):
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
## ListOrganizationRecommendationAccountsRequestRequestTypeDef

```python
# ListOrganizationRecommendationAccountsRequestRequestTypeDef definition

class ListOrganizationRecommendationAccountsRequestRequestTypeDef(TypedDict):
    organizationRecommendationIdentifier: str,
    affectedAccountId: NotRequired[str],
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListOrganizationRecommendationResourcesRequestRequestTypeDef

```python
# ListOrganizationRecommendationResourcesRequestRequestTypeDef definition

class ListOrganizationRecommendationResourcesRequestRequestTypeDef(TypedDict):
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
## ListRecommendationResourcesRequestRequestTypeDef

```python
# ListRecommendationResourcesRequestRequestTypeDef definition

class ListRecommendationResourcesRequestRequestTypeDef(TypedDict):
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
# RecommendationResourcesAggregatesTypeDef definition

class RecommendationResourcesAggregatesTypeDef(TypedDict):
    errorCount: int,
    okCount: int,
    warningCount: int,
```

## RecommendationCostOptimizingAggregatesTypeDef

```python
# RecommendationCostOptimizingAggregatesTypeDef definition

class RecommendationCostOptimizingAggregatesTypeDef(TypedDict):
    estimatedMonthlySavings: float,
    estimatedPercentMonthlySavings: float,
```

## UpdateOrganizationRecommendationLifecycleRequestRequestTypeDef

```python
# UpdateOrganizationRecommendationLifecycleRequestRequestTypeDef definition

class UpdateOrganizationRecommendationLifecycleRequestRequestTypeDef(TypedDict):
    lifecycleStage: UpdateRecommendationLifecycleStageType,  # (1)
    organizationRecommendationIdentifier: str,
    updateReason: NotRequired[str],
    updateReasonCode: NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],  # (2)
```

1. See [:material-code-brackets: UpdateRecommendationLifecycleStageType](./literals.md#updaterecommendationlifecyclestagetype) 
2. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
## UpdateRecommendationLifecycleRequestRequestTypeDef

```python
# UpdateRecommendationLifecycleRequestRequestTypeDef definition

class UpdateRecommendationLifecycleRequestRequestTypeDef(TypedDict):
    lifecycleStage: UpdateRecommendationLifecycleStageType,  # (1)
    recommendationIdentifier: str,
    updateReason: NotRequired[str],
    updateReasonCode: NotRequired[UpdateRecommendationLifecycleStageReasonCodeType],  # (2)
```

1. See [:material-code-brackets: UpdateRecommendationLifecycleStageType](./literals.md#updaterecommendationlifecyclestagetype) 
2. See [:material-code-brackets: UpdateRecommendationLifecycleStageReasonCodeType](./literals.md#updaterecommendationlifecyclestagereasoncodetype) 
## BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef

```python
# BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef definition

class BatchUpdateRecommendationResourceExclusionRequestRequestTypeDef(TypedDict):
    recommendationResourceExclusions: Sequence[RecommendationResourceExclusionTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationResourceExclusionTypeDef](./type_defs.md#recommendationresourceexclusiontypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListOrganizationRecommendationAccountsResponseTypeDef

```python
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
# BatchUpdateRecommendationResourceExclusionResponseTypeDef definition

class BatchUpdateRecommendationResourceExclusionResponseTypeDef(TypedDict):
    batchUpdateRecommendationResourceExclusionErrors: List[UpdateRecommendationResourceExclusionErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: UpdateRecommendationResourceExclusionErrorTypeDef](./type_defs.md#updaterecommendationresourceexclusionerrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListChecksResponseTypeDef

```python
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
# ListOrganizationRecommendationAccountsRequestPaginateTypeDef definition

class ListOrganizationRecommendationAccountsRequestPaginateTypeDef(TypedDict):
    organizationRecommendationIdentifier: str,
    affectedAccountId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOrganizationRecommendationResourcesRequestPaginateTypeDef

```python
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
## ListOrganizationRecommendationsRequestRequestTypeDef

```python
# ListOrganizationRecommendationsRequestRequestTypeDef definition

class ListOrganizationRecommendationsRequestRequestTypeDef(TypedDict):
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
## ListRecommendationsRequestRequestTypeDef

```python
# ListRecommendationsRequestRequestTypeDef definition

class ListRecommendationsRequestRequestTypeDef(TypedDict):
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
# RecommendationPillarSpecificAggregatesTypeDef definition

class RecommendationPillarSpecificAggregatesTypeDef(TypedDict):
    costOptimizing: NotRequired[RecommendationCostOptimizingAggregatesTypeDef],  # (1)
```

1. See [:material-code-braces: RecommendationCostOptimizingAggregatesTypeDef](./type_defs.md#recommendationcostoptimizingaggregatestypedef) 
## OrganizationRecommendationSummaryTypeDef

```python
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
# GetOrganizationRecommendationResponseTypeDef definition

class GetOrganizationRecommendationResponseTypeDef(TypedDict):
    organizationRecommendation: OrganizationRecommendationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: OrganizationRecommendationTypeDef](./type_defs.md#organizationrecommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecommendationsResponseTypeDef

```python
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
# GetRecommendationResponseTypeDef definition

class GetRecommendationResponseTypeDef(TypedDict):
    recommendation: RecommendationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

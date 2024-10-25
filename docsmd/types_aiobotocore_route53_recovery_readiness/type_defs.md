# Type definitions

> [Index](../README.md) > [Route53RecoveryReadiness](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Route53RecoveryReadiness](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-readiness.html#Route53RecoveryReadiness)
    type annotations stubs module [types-aiobotocore-route53-recovery-readiness](https://pypi.org/project/types-aiobotocore-route53-recovery-readiness/).

## ResourceUnionTypeDef

```python
# ResourceUnionTypeDef definition

ResourceUnionTypeDef = Union[
    ResourceTypeDef,  # (1)
    ResourceOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 



## CellOutputTypeDef

```python
# CellOutputTypeDef definition

class CellOutputTypeDef(TypedDict):
    CellArn: str,
    CellName: str,
    Cells: List[str],
    ParentReadinessScopes: List[str],
    Tags: NotRequired[Dict[str, str]],
```

## CreateCellRequestRequestTypeDef

```python
# CreateCellRequestRequestTypeDef definition

class CreateCellRequestRequestTypeDef(TypedDict):
    CellName: str,
    Cells: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
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

## CreateCrossAccountAuthorizationRequestRequestTypeDef

```python
# CreateCrossAccountAuthorizationRequestRequestTypeDef definition

class CreateCrossAccountAuthorizationRequestRequestTypeDef(TypedDict):
    CrossAccountAuthorization: str,
```

## CreateReadinessCheckRequestRequestTypeDef

```python
# CreateReadinessCheckRequestRequestTypeDef definition

class CreateReadinessCheckRequestRequestTypeDef(TypedDict):
    ReadinessCheckName: str,
    ResourceSetName: str,
    Tags: NotRequired[Mapping[str, str]],
```

## CreateRecoveryGroupRequestRequestTypeDef

```python
# CreateRecoveryGroupRequestRequestTypeDef definition

class CreateRecoveryGroupRequestRequestTypeDef(TypedDict):
    RecoveryGroupName: str,
    Cells: NotRequired[Sequence[str]],
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteCellRequestRequestTypeDef

```python
# DeleteCellRequestRequestTypeDef definition

class DeleteCellRequestRequestTypeDef(TypedDict):
    CellName: str,
```

## DeleteCrossAccountAuthorizationRequestRequestTypeDef

```python
# DeleteCrossAccountAuthorizationRequestRequestTypeDef definition

class DeleteCrossAccountAuthorizationRequestRequestTypeDef(TypedDict):
    CrossAccountAuthorization: str,
```

## DeleteReadinessCheckRequestRequestTypeDef

```python
# DeleteReadinessCheckRequestRequestTypeDef definition

class DeleteReadinessCheckRequestRequestTypeDef(TypedDict):
    ReadinessCheckName: str,
```

## DeleteRecoveryGroupRequestRequestTypeDef

```python
# DeleteRecoveryGroupRequestRequestTypeDef definition

class DeleteRecoveryGroupRequestRequestTypeDef(TypedDict):
    RecoveryGroupName: str,
```

## DeleteResourceSetRequestRequestTypeDef

```python
# DeleteResourceSetRequestRequestTypeDef definition

class DeleteResourceSetRequestRequestTypeDef(TypedDict):
    ResourceSetName: str,
```

## GetArchitectureRecommendationsRequestRequestTypeDef

```python
# GetArchitectureRecommendationsRequestRequestTypeDef definition

class GetArchitectureRecommendationsRequestRequestTypeDef(TypedDict):
    RecoveryGroupName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## RecommendationTypeDef

```python
# RecommendationTypeDef definition

class RecommendationTypeDef(TypedDict):
    RecommendationText: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetCellReadinessSummaryRequestRequestTypeDef

```python
# GetCellReadinessSummaryRequestRequestTypeDef definition

class GetCellReadinessSummaryRequestRequestTypeDef(TypedDict):
    CellName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ReadinessCheckSummaryTypeDef

```python
# ReadinessCheckSummaryTypeDef definition

class ReadinessCheckSummaryTypeDef(TypedDict):
    Readiness: NotRequired[ReadinessType],  # (1)
    ReadinessCheckName: NotRequired[str],
```

1. See [:material-code-brackets: ReadinessType](./literals.md#readinesstype) 
## GetCellRequestRequestTypeDef

```python
# GetCellRequestRequestTypeDef definition

class GetCellRequestRequestTypeDef(TypedDict):
    CellName: str,
```

## GetReadinessCheckRequestRequestTypeDef

```python
# GetReadinessCheckRequestRequestTypeDef definition

class GetReadinessCheckRequestRequestTypeDef(TypedDict):
    ReadinessCheckName: str,
```

## GetReadinessCheckResourceStatusRequestRequestTypeDef

```python
# GetReadinessCheckResourceStatusRequestRequestTypeDef definition

class GetReadinessCheckResourceStatusRequestRequestTypeDef(TypedDict):
    ReadinessCheckName: str,
    ResourceIdentifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetReadinessCheckStatusRequestRequestTypeDef

```python
# GetReadinessCheckStatusRequestRequestTypeDef definition

class GetReadinessCheckStatusRequestRequestTypeDef(TypedDict):
    ReadinessCheckName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## MessageTypeDef

```python
# MessageTypeDef definition

class MessageTypeDef(TypedDict):
    MessageText: NotRequired[str],
```

## ResourceResultTypeDef

```python
# ResourceResultTypeDef definition

class ResourceResultTypeDef(TypedDict):
    LastCheckedTimestamp: datetime,
    Readiness: ReadinessType,  # (1)
    ComponentId: NotRequired[str],
    ResourceArn: NotRequired[str],
```

1. See [:material-code-brackets: ReadinessType](./literals.md#readinesstype) 
## GetRecoveryGroupReadinessSummaryRequestRequestTypeDef

```python
# GetRecoveryGroupReadinessSummaryRequestRequestTypeDef definition

class GetRecoveryGroupReadinessSummaryRequestRequestTypeDef(TypedDict):
    RecoveryGroupName: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## GetRecoveryGroupRequestRequestTypeDef

```python
# GetRecoveryGroupRequestRequestTypeDef definition

class GetRecoveryGroupRequestRequestTypeDef(TypedDict):
    RecoveryGroupName: str,
```

## GetResourceSetRequestRequestTypeDef

```python
# GetResourceSetRequestRequestTypeDef definition

class GetResourceSetRequestRequestTypeDef(TypedDict):
    ResourceSetName: str,
```

## ListCellsRequestRequestTypeDef

```python
# ListCellsRequestRequestTypeDef definition

class ListCellsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListCrossAccountAuthorizationsRequestRequestTypeDef

```python
# ListCrossAccountAuthorizationsRequestRequestTypeDef definition

class ListCrossAccountAuthorizationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListReadinessChecksRequestRequestTypeDef

```python
# ListReadinessChecksRequestRequestTypeDef definition

class ListReadinessChecksRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ReadinessCheckOutputTypeDef

```python
# ReadinessCheckOutputTypeDef definition

class ReadinessCheckOutputTypeDef(TypedDict):
    ReadinessCheckArn: str,
    ResourceSet: str,
    ReadinessCheckName: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
```

## ListRecoveryGroupsRequestRequestTypeDef

```python
# ListRecoveryGroupsRequestRequestTypeDef definition

class ListRecoveryGroupsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## RecoveryGroupOutputTypeDef

```python
# RecoveryGroupOutputTypeDef definition

class RecoveryGroupOutputTypeDef(TypedDict):
    Cells: List[str],
    RecoveryGroupArn: str,
    RecoveryGroupName: str,
    Tags: NotRequired[Dict[str, str]],
```

## ListResourceSetsRequestRequestTypeDef

```python
# ListResourceSetsRequestRequestTypeDef definition

class ListResourceSetsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListRulesOutputTypeDef

```python
# ListRulesOutputTypeDef definition

class ListRulesOutputTypeDef(TypedDict):
    ResourceType: str,
    RuleDescription: str,
    RuleId: str,
```

## ListRulesRequestRequestTypeDef

```python
# ListRulesRequestRequestTypeDef definition

class ListRulesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ResourceType: NotRequired[str],
```

## ListTagsForResourcesRequestRequestTypeDef

```python
# ListTagsForResourcesRequestRequestTypeDef definition

class ListTagsForResourcesRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## NLBResourceTypeDef

```python
# NLBResourceTypeDef definition

class NLBResourceTypeDef(TypedDict):
    Arn: NotRequired[str],
```

## R53ResourceRecordTypeDef

```python
# R53ResourceRecordTypeDef definition

class R53ResourceRecordTypeDef(TypedDict):
    DomainName: NotRequired[str],
    RecordSetId: NotRequired[str],
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateCellRequestRequestTypeDef

```python
# UpdateCellRequestRequestTypeDef definition

class UpdateCellRequestRequestTypeDef(TypedDict):
    CellName: str,
    Cells: Sequence[str],
```

## UpdateReadinessCheckRequestRequestTypeDef

```python
# UpdateReadinessCheckRequestRequestTypeDef definition

class UpdateReadinessCheckRequestRequestTypeDef(TypedDict):
    ReadinessCheckName: str,
    ResourceSetName: str,
```

## UpdateRecoveryGroupRequestRequestTypeDef

```python
# UpdateRecoveryGroupRequestRequestTypeDef definition

class UpdateRecoveryGroupRequestRequestTypeDef(TypedDict):
    Cells: Sequence[str],
    RecoveryGroupName: str,
```

## CreateCellResponseTypeDef

```python
# CreateCellResponseTypeDef definition

class CreateCellResponseTypeDef(TypedDict):
    CellArn: str,
    CellName: str,
    Cells: List[str],
    ParentReadinessScopes: List[str],
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCrossAccountAuthorizationResponseTypeDef

```python
# CreateCrossAccountAuthorizationResponseTypeDef definition

class CreateCrossAccountAuthorizationResponseTypeDef(TypedDict):
    CrossAccountAuthorization: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReadinessCheckResponseTypeDef

```python
# CreateReadinessCheckResponseTypeDef definition

class CreateReadinessCheckResponseTypeDef(TypedDict):
    ReadinessCheckArn: str,
    ReadinessCheckName: str,
    ResourceSet: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateRecoveryGroupResponseTypeDef

```python
# CreateRecoveryGroupResponseTypeDef definition

class CreateRecoveryGroupResponseTypeDef(TypedDict):
    Cells: List[str],
    RecoveryGroupArn: str,
    RecoveryGroupName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCellResponseTypeDef

```python
# GetCellResponseTypeDef definition

class GetCellResponseTypeDef(TypedDict):
    CellArn: str,
    CellName: str,
    Cells: List[str],
    ParentReadinessScopes: List[str],
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetReadinessCheckResponseTypeDef

```python
# GetReadinessCheckResponseTypeDef definition

class GetReadinessCheckResponseTypeDef(TypedDict):
    ReadinessCheckArn: str,
    ReadinessCheckName: str,
    ResourceSet: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecoveryGroupResponseTypeDef

```python
# GetRecoveryGroupResponseTypeDef definition

class GetRecoveryGroupResponseTypeDef(TypedDict):
    Cells: List[str],
    RecoveryGroupArn: str,
    RecoveryGroupName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCellsResponseTypeDef

```python
# ListCellsResponseTypeDef definition

class ListCellsResponseTypeDef(TypedDict):
    Cells: List[CellOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CellOutputTypeDef](./type_defs.md#celloutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListCrossAccountAuthorizationsResponseTypeDef

```python
# ListCrossAccountAuthorizationsResponseTypeDef definition

class ListCrossAccountAuthorizationsResponseTypeDef(TypedDict):
    CrossAccountAuthorizations: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourcesResponseTypeDef

```python
# ListTagsForResourcesResponseTypeDef definition

class ListTagsForResourcesResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCellResponseTypeDef

```python
# UpdateCellResponseTypeDef definition

class UpdateCellResponseTypeDef(TypedDict):
    CellArn: str,
    CellName: str,
    Cells: List[str],
    ParentReadinessScopes: List[str],
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReadinessCheckResponseTypeDef

```python
# UpdateReadinessCheckResponseTypeDef definition

class UpdateReadinessCheckResponseTypeDef(TypedDict):
    ReadinessCheckArn: str,
    ReadinessCheckName: str,
    ResourceSet: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateRecoveryGroupResponseTypeDef

```python
# UpdateRecoveryGroupResponseTypeDef definition

class UpdateRecoveryGroupResponseTypeDef(TypedDict):
    Cells: List[str],
    RecoveryGroupArn: str,
    RecoveryGroupName: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetArchitectureRecommendationsResponseTypeDef

```python
# GetArchitectureRecommendationsResponseTypeDef definition

class GetArchitectureRecommendationsResponseTypeDef(TypedDict):
    LastAuditTimestamp: datetime,
    Recommendations: List[RecommendationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecommendationTypeDef](./type_defs.md#recommendationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef

```python
# GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef definition

class GetCellReadinessSummaryRequestGetCellReadinessSummaryPaginateTypeDef(TypedDict):
    CellName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef

```python
# GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef definition

class GetReadinessCheckResourceStatusRequestGetReadinessCheckResourceStatusPaginateTypeDef(TypedDict):
    ReadinessCheckName: str,
    ResourceIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef

```python
# GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef definition

class GetReadinessCheckStatusRequestGetReadinessCheckStatusPaginateTypeDef(TypedDict):
    ReadinessCheckName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef

```python
# GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef definition

class GetRecoveryGroupReadinessSummaryRequestGetRecoveryGroupReadinessSummaryPaginateTypeDef(TypedDict):
    RecoveryGroupName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCellsRequestListCellsPaginateTypeDef

```python
# ListCellsRequestListCellsPaginateTypeDef definition

class ListCellsRequestListCellsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef

```python
# ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef definition

class ListCrossAccountAuthorizationsRequestListCrossAccountAuthorizationsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListReadinessChecksRequestListReadinessChecksPaginateTypeDef

```python
# ListReadinessChecksRequestListReadinessChecksPaginateTypeDef definition

class ListReadinessChecksRequestListReadinessChecksPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef

```python
# ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef definition

class ListRecoveryGroupsRequestListRecoveryGroupsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourceSetsRequestListResourceSetsPaginateTypeDef

```python
# ListResourceSetsRequestListResourceSetsPaginateTypeDef definition

class ListResourceSetsRequestListResourceSetsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListRulesRequestListRulesPaginateTypeDef

```python
# ListRulesRequestListRulesPaginateTypeDef definition

class ListRulesRequestListRulesPaginateTypeDef(TypedDict):
    ResourceType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetCellReadinessSummaryResponseTypeDef

```python
# GetCellReadinessSummaryResponseTypeDef definition

class GetCellReadinessSummaryResponseTypeDef(TypedDict):
    Readiness: ReadinessType,  # (1)
    ReadinessChecks: List[ReadinessCheckSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ReadinessType](./literals.md#readinesstype) 
2. See [:material-code-braces: ReadinessCheckSummaryTypeDef](./type_defs.md#readinesschecksummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetRecoveryGroupReadinessSummaryResponseTypeDef

```python
# GetRecoveryGroupReadinessSummaryResponseTypeDef definition

class GetRecoveryGroupReadinessSummaryResponseTypeDef(TypedDict):
    Readiness: ReadinessType,  # (1)
    ReadinessChecks: List[ReadinessCheckSummaryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ReadinessType](./literals.md#readinesstype) 
2. See [:material-code-braces: ReadinessCheckSummaryTypeDef](./type_defs.md#readinesschecksummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RuleResultTypeDef

```python
# RuleResultTypeDef definition

class RuleResultTypeDef(TypedDict):
    LastCheckedTimestamp: datetime,
    Messages: List[MessageTypeDef],  # (1)
    Readiness: ReadinessType,  # (2)
    RuleId: str,
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-brackets: ReadinessType](./literals.md#readinesstype) 
## GetReadinessCheckStatusResponseTypeDef

```python
# GetReadinessCheckStatusResponseTypeDef definition

class GetReadinessCheckStatusResponseTypeDef(TypedDict):
    Messages: List[MessageTypeDef],  # (1)
    Readiness: ReadinessType,  # (2)
    Resources: List[ResourceResultTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: MessageTypeDef](./type_defs.md#messagetypedef) 
2. See [:material-code-brackets: ReadinessType](./literals.md#readinesstype) 
3. See [:material-code-braces: ResourceResultTypeDef](./type_defs.md#resourceresulttypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReadinessChecksResponseTypeDef

```python
# ListReadinessChecksResponseTypeDef definition

class ListReadinessChecksResponseTypeDef(TypedDict):
    ReadinessChecks: List[ReadinessCheckOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ReadinessCheckOutputTypeDef](./type_defs.md#readinesscheckoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRecoveryGroupsResponseTypeDef

```python
# ListRecoveryGroupsResponseTypeDef definition

class ListRecoveryGroupsResponseTypeDef(TypedDict):
    RecoveryGroups: List[RecoveryGroupOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RecoveryGroupOutputTypeDef](./type_defs.md#recoverygroupoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListRulesResponseTypeDef

```python
# ListRulesResponseTypeDef definition

class ListRulesResponseTypeDef(TypedDict):
    Rules: List[ListRulesOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ListRulesOutputTypeDef](./type_defs.md#listrulesoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TargetResourceTypeDef

```python
# TargetResourceTypeDef definition

class TargetResourceTypeDef(TypedDict):
    NLBResource: NotRequired[NLBResourceTypeDef],  # (1)
    R53Resource: NotRequired[R53ResourceRecordTypeDef],  # (2)
```

1. See [:material-code-braces: NLBResourceTypeDef](./type_defs.md#nlbresourcetypedef) 
2. See [:material-code-braces: R53ResourceRecordTypeDef](./type_defs.md#r53resourcerecordtypedef) 
## GetReadinessCheckResourceStatusResponseTypeDef

```python
# GetReadinessCheckResourceStatusResponseTypeDef definition

class GetReadinessCheckResourceStatusResponseTypeDef(TypedDict):
    Readiness: ReadinessType,  # (1)
    Rules: List[RuleResultTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
    NextToken: NotRequired[str],
```

1. See [:material-code-brackets: ReadinessType](./literals.md#readinesstype) 
2. See [:material-code-braces: RuleResultTypeDef](./type_defs.md#ruleresulttypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DNSTargetResourceTypeDef

```python
# DNSTargetResourceTypeDef definition

class DNSTargetResourceTypeDef(TypedDict):
    DomainName: NotRequired[str],
    HostedZoneArn: NotRequired[str],
    RecordSetId: NotRequired[str],
    RecordType: NotRequired[str],
    TargetResource: NotRequired[TargetResourceTypeDef],  # (1)
```

1. See [:material-code-braces: TargetResourceTypeDef](./type_defs.md#targetresourcetypedef) 
## ResourceOutputTypeDef

```python
# ResourceOutputTypeDef definition

class ResourceOutputTypeDef(TypedDict):
    ComponentId: NotRequired[str],
    DnsTargetResource: NotRequired[DNSTargetResourceTypeDef],  # (1)
    ReadinessScopes: NotRequired[List[str]],
    ResourceArn: NotRequired[str],
```

1. See [:material-code-braces: DNSTargetResourceTypeDef](./type_defs.md#dnstargetresourcetypedef) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    ComponentId: NotRequired[str],
    DnsTargetResource: NotRequired[DNSTargetResourceTypeDef],  # (1)
    ReadinessScopes: NotRequired[Sequence[str]],
    ResourceArn: NotRequired[str],
```

1. See [:material-code-braces: DNSTargetResourceTypeDef](./type_defs.md#dnstargetresourcetypedef) 
## CreateResourceSetResponseTypeDef

```python
# CreateResourceSetResponseTypeDef definition

class CreateResourceSetResponseTypeDef(TypedDict):
    ResourceSetArn: str,
    ResourceSetName: str,
    ResourceSetType: str,
    Resources: List[ResourceOutputTypeDef],  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceSetResponseTypeDef

```python
# GetResourceSetResponseTypeDef definition

class GetResourceSetResponseTypeDef(TypedDict):
    ResourceSetArn: str,
    ResourceSetName: str,
    ResourceSetType: str,
    Resources: List[ResourceOutputTypeDef],  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceSetOutputTypeDef

```python
# ResourceSetOutputTypeDef definition

class ResourceSetOutputTypeDef(TypedDict):
    ResourceSetArn: str,
    ResourceSetName: str,
    ResourceSetType: str,
    Resources: List[ResourceOutputTypeDef],  # (1)
    Tags: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
## UpdateResourceSetResponseTypeDef

```python
# UpdateResourceSetResponseTypeDef definition

class UpdateResourceSetResponseTypeDef(TypedDict):
    ResourceSetArn: str,
    ResourceSetName: str,
    ResourceSetType: str,
    Resources: List[ResourceOutputTypeDef],  # (1)
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResourceSetRequestRequestTypeDef

```python
# UpdateResourceSetRequestRequestTypeDef definition

class UpdateResourceSetRequestRequestTypeDef(TypedDict):
    ResourceSetName: str,
    ResourceSetType: str,
    Resources: Sequence[ResourceTypeDef],  # (1)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
## ListResourceSetsResponseTypeDef

```python
# ListResourceSetsResponseTypeDef definition

class ListResourceSetsResponseTypeDef(TypedDict):
    ResourceSets: List[ResourceSetOutputTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResourceSetOutputTypeDef](./type_defs.md#resourcesetoutputtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceSetRequestRequestTypeDef

```python
# CreateResourceSetRequestRequestTypeDef definition

class CreateResourceSetRequestRequestTypeDef(TypedDict):
    ResourceSetName: str,
    ResourceSetType: str,
    Resources: Sequence[ResourceUnionTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) [:material-code-braces: ResourceOutputTypeDef](./type_defs.md#resourceoutputtypedef) 

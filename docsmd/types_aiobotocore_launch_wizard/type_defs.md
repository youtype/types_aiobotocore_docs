# Type definitions

> [Index](../README.md) > [LaunchWizard](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#LaunchWizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).



## CreateDeploymentInputRequestTypeDef

```python
# CreateDeploymentInputRequestTypeDef definition

class CreateDeploymentInputRequestTypeDef(TypedDict):
    deploymentPatternName: str,
    name: str,
    specifications: Mapping[str, str],
    workloadName: str,
    dryRun: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
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

## DeleteDeploymentInputRequestTypeDef

```python
# DeleteDeploymentInputRequestTypeDef definition

class DeleteDeploymentInputRequestTypeDef(TypedDict):
    deploymentId: str,
```

## DeploymentConditionalFieldTypeDef

```python
# DeploymentConditionalFieldTypeDef definition

class DeploymentConditionalFieldTypeDef(TypedDict):
    comparator: NotRequired[str],
    name: NotRequired[str],
    value: NotRequired[str],
```

## DeploymentDataSummaryTypeDef

```python
# DeploymentDataSummaryTypeDef definition

class DeploymentDataSummaryTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    id: NotRequired[str],
    name: NotRequired[str],
    patternName: NotRequired[str],
    status: NotRequired[DeploymentStatusType],  # (1)
    workloadName: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## DeploymentDataTypeDef

```python
# DeploymentDataTypeDef definition

class DeploymentDataTypeDef(TypedDict):
    createdAt: NotRequired[datetime],
    deletedAt: NotRequired[datetime],
    deploymentArn: NotRequired[str],
    id: NotRequired[str],
    name: NotRequired[str],
    patternName: NotRequired[str],
    resourceGroup: NotRequired[str],
    specifications: NotRequired[Dict[str, str]],
    status: NotRequired[DeploymentStatusType],  # (1)
    tags: NotRequired[Dict[str, str]],
    workloadName: NotRequired[str],
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
## DeploymentEventDataSummaryTypeDef

```python
# DeploymentEventDataSummaryTypeDef definition

class DeploymentEventDataSummaryTypeDef(TypedDict):
    description: NotRequired[str],
    name: NotRequired[str],
    status: NotRequired[EventStatusType],  # (1)
    statusReason: NotRequired[str],
    timestamp: NotRequired[datetime],
```

1. See [:material-code-brackets: EventStatusType](./literals.md#eventstatustype) 
## DeploymentFilterTypeDef

```python
# DeploymentFilterTypeDef definition

class DeploymentFilterTypeDef(TypedDict):
    name: NotRequired[DeploymentFilterKeyType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DeploymentFilterKeyType](./literals.md#deploymentfilterkeytype) 
## GetDeploymentInputRequestTypeDef

```python
# GetDeploymentInputRequestTypeDef definition

class GetDeploymentInputRequestTypeDef(TypedDict):
    deploymentId: str,
```

## GetWorkloadDeploymentPatternInputRequestTypeDef

```python
# GetWorkloadDeploymentPatternInputRequestTypeDef definition

class GetWorkloadDeploymentPatternInputRequestTypeDef(TypedDict):
    deploymentPatternName: str,
    workloadName: str,
```

## GetWorkloadInputRequestTypeDef

```python
# GetWorkloadInputRequestTypeDef definition

class GetWorkloadInputRequestTypeDef(TypedDict):
    workloadName: str,
```

## WorkloadDataTypeDef

```python
# WorkloadDataTypeDef definition

class WorkloadDataTypeDef(TypedDict):
    description: NotRequired[str],
    displayName: NotRequired[str],
    documentationUrl: NotRequired[str],
    iconUrl: NotRequired[str],
    status: NotRequired[WorkloadStatusType],  # (1)
    statusMessage: NotRequired[str],
    workloadName: NotRequired[str],
```

1. See [:material-code-brackets: WorkloadStatusType](./literals.md#workloadstatustype) 
## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDeploymentEventsInputRequestTypeDef

```python
# ListDeploymentEventsInputRequestTypeDef definition

class ListDeploymentEventsInputRequestTypeDef(TypedDict):
    deploymentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
```

## ListWorkloadDeploymentPatternsInputRequestTypeDef

```python
# ListWorkloadDeploymentPatternsInputRequestTypeDef definition

class ListWorkloadDeploymentPatternsInputRequestTypeDef(TypedDict):
    workloadName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WorkloadDeploymentPatternDataSummaryTypeDef

```python
# WorkloadDeploymentPatternDataSummaryTypeDef definition

class WorkloadDeploymentPatternDataSummaryTypeDef(TypedDict):
    deploymentPatternName: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    status: NotRequired[WorkloadDeploymentPatternStatusType],  # (1)
    statusMessage: NotRequired[str],
    workloadName: NotRequired[str],
    workloadVersionName: NotRequired[str],
```

1. See [:material-code-brackets: WorkloadDeploymentPatternStatusType](./literals.md#workloaddeploymentpatternstatustype) 
## ListWorkloadsInputRequestTypeDef

```python
# ListWorkloadsInputRequestTypeDef definition

class ListWorkloadsInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WorkloadDataSummaryTypeDef

```python
# WorkloadDataSummaryTypeDef definition

class WorkloadDataSummaryTypeDef(TypedDict):
    displayName: NotRequired[str],
    workloadName: NotRequired[str],
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## CreateDeploymentOutputTypeDef

```python
# CreateDeploymentOutputTypeDef definition

class CreateDeploymentOutputTypeDef(TypedDict):
    deploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDeploymentOutputTypeDef

```python
# DeleteDeploymentOutputTypeDef definition

class DeleteDeploymentOutputTypeDef(TypedDict):
    status: DeploymentStatusType,  # (1)
    statusReason: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DeploymentStatusType](./literals.md#deploymentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentSpecificationsFieldTypeDef

```python
# DeploymentSpecificationsFieldTypeDef definition

class DeploymentSpecificationsFieldTypeDef(TypedDict):
    allowedValues: NotRequired[List[str]],
    conditionals: NotRequired[List[DeploymentConditionalFieldTypeDef]],  # (1)
    description: NotRequired[str],
    name: NotRequired[str],
    required: NotRequired[str],
```

1. See [:material-code-braces: DeploymentConditionalFieldTypeDef](./type_defs.md#deploymentconditionalfieldtypedef) 
## ListDeploymentsOutputTypeDef

```python
# ListDeploymentsOutputTypeDef definition

class ListDeploymentsOutputTypeDef(TypedDict):
    deployments: List[DeploymentDataSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentDataSummaryTypeDef](./type_defs.md#deploymentdatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDeploymentOutputTypeDef

```python
# GetDeploymentOutputTypeDef definition

class GetDeploymentOutputTypeDef(TypedDict):
    deployment: DeploymentDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentDataTypeDef](./type_defs.md#deploymentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentEventsOutputTypeDef

```python
# ListDeploymentEventsOutputTypeDef definition

class ListDeploymentEventsOutputTypeDef(TypedDict):
    deploymentEvents: List[DeploymentEventDataSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentEventDataSummaryTypeDef](./type_defs.md#deploymenteventdatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentsInputRequestTypeDef

```python
# ListDeploymentsInputRequestTypeDef definition

class ListDeploymentsInputRequestTypeDef(TypedDict):
    filters: NotRequired[Sequence[DeploymentFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef) 
## GetWorkloadOutputTypeDef

```python
# GetWorkloadOutputTypeDef definition

class GetWorkloadOutputTypeDef(TypedDict):
    workload: WorkloadDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadDataTypeDef](./type_defs.md#workloaddatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentEventsInputListDeploymentEventsPaginateTypeDef

```python
# ListDeploymentEventsInputListDeploymentEventsPaginateTypeDef definition

class ListDeploymentEventsInputListDeploymentEventsPaginateTypeDef(TypedDict):
    deploymentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentsInputListDeploymentsPaginateTypeDef

```python
# ListDeploymentsInputListDeploymentsPaginateTypeDef definition

class ListDeploymentsInputListDeploymentsPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[DeploymentFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkloadDeploymentPatternsInputListWorkloadDeploymentPatternsPaginateTypeDef

```python
# ListWorkloadDeploymentPatternsInputListWorkloadDeploymentPatternsPaginateTypeDef definition

class ListWorkloadDeploymentPatternsInputListWorkloadDeploymentPatternsPaginateTypeDef(TypedDict):
    workloadName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkloadsInputListWorkloadsPaginateTypeDef

```python
# ListWorkloadsInputListWorkloadsPaginateTypeDef definition

class ListWorkloadsInputListWorkloadsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkloadDeploymentPatternsOutputTypeDef

```python
# ListWorkloadDeploymentPatternsOutputTypeDef definition

class ListWorkloadDeploymentPatternsOutputTypeDef(TypedDict):
    workloadDeploymentPatterns: List[WorkloadDeploymentPatternDataSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkloadDeploymentPatternDataSummaryTypeDef](./type_defs.md#workloaddeploymentpatterndatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkloadsOutputTypeDef

```python
# ListWorkloadsOutputTypeDef definition

class ListWorkloadsOutputTypeDef(TypedDict):
    workloads: List[WorkloadDataSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: WorkloadDataSummaryTypeDef](./type_defs.md#workloaddatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## WorkloadDeploymentPatternDataTypeDef

```python
# WorkloadDeploymentPatternDataTypeDef definition

class WorkloadDeploymentPatternDataTypeDef(TypedDict):
    deploymentPatternName: NotRequired[str],
    description: NotRequired[str],
    displayName: NotRequired[str],
    specifications: NotRequired[List[DeploymentSpecificationsFieldTypeDef]],  # (1)
    status: NotRequired[WorkloadDeploymentPatternStatusType],  # (2)
    statusMessage: NotRequired[str],
    workloadName: NotRequired[str],
    workloadVersionName: NotRequired[str],
```

1. See [:material-code-braces: DeploymentSpecificationsFieldTypeDef](./type_defs.md#deploymentspecificationsfieldtypedef) 
2. See [:material-code-brackets: WorkloadDeploymentPatternStatusType](./literals.md#workloaddeploymentpatternstatustype) 
## GetWorkloadDeploymentPatternOutputTypeDef

```python
# GetWorkloadDeploymentPatternOutputTypeDef definition

class GetWorkloadDeploymentPatternOutputTypeDef(TypedDict):
    workloadDeploymentPattern: WorkloadDeploymentPatternDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadDeploymentPatternDataTypeDef](./type_defs.md#workloaddeploymentpatterndatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

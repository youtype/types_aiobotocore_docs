# Type definitions

> [Index](../README.md) > [LaunchWizard](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [LaunchWizard](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/launch-wizard.html#launchwizard)
    type annotations stubs module [types-aiobotocore-launch-wizard](https://pypi.org/project/types-aiobotocore-launch-wizard/).



## CreateDeploymentInputTypeDef

```python
# CreateDeploymentInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import CreateDeploymentInputTypeDef


def get_value() -> CreateDeploymentInputTypeDef:
    return {
        "deploymentPatternName": ...,
    }


# CreateDeploymentInputTypeDef definition

class CreateDeploymentInputTypeDef(TypedDict):
    deploymentPatternName: str,
    name: str,
    specifications: Mapping[str, str],
    workloadName: str,
    dryRun: NotRequired[bool],
    tags: NotRequired[Mapping[str, str]],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ResponseMetadataTypeDef


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

## DeleteDeploymentInputTypeDef

```python
# DeleteDeploymentInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import DeleteDeploymentInputTypeDef


def get_value() -> DeleteDeploymentInputTypeDef:
    return {
        "deploymentId": ...,
    }


# DeleteDeploymentInputTypeDef definition

class DeleteDeploymentInputTypeDef(TypedDict):
    deploymentId: str,
```

## DeploymentConditionalFieldTypeDef

```python
# DeploymentConditionalFieldTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import DeploymentConditionalFieldTypeDef


def get_value() -> DeploymentConditionalFieldTypeDef:
    return {
        "comparator": ...,
    }


# DeploymentConditionalFieldTypeDef definition

class DeploymentConditionalFieldTypeDef(TypedDict):
    comparator: NotRequired[str],
    name: NotRequired[str],
    value: NotRequired[str],
```

## DeploymentDataSummaryTypeDef

```python
# DeploymentDataSummaryTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import DeploymentDataSummaryTypeDef


def get_value() -> DeploymentDataSummaryTypeDef:
    return {
        "createdAt": ...,
    }


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
# DeploymentDataTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import DeploymentDataTypeDef


def get_value() -> DeploymentDataTypeDef:
    return {
        "createdAt": ...,
    }


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
# DeploymentEventDataSummaryTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import DeploymentEventDataSummaryTypeDef


def get_value() -> DeploymentEventDataSummaryTypeDef:
    return {
        "description": ...,
    }


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
# DeploymentFilterTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import DeploymentFilterTypeDef


def get_value() -> DeploymentFilterTypeDef:
    return {
        "name": ...,
    }


# DeploymentFilterTypeDef definition

class DeploymentFilterTypeDef(TypedDict):
    name: NotRequired[DeploymentFilterKeyType],  # (1)
    values: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: DeploymentFilterKeyType](./literals.md#deploymentfilterkeytype) 
## GetDeploymentInputTypeDef

```python
# GetDeploymentInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import GetDeploymentInputTypeDef


def get_value() -> GetDeploymentInputTypeDef:
    return {
        "deploymentId": ...,
    }


# GetDeploymentInputTypeDef definition

class GetDeploymentInputTypeDef(TypedDict):
    deploymentId: str,
```

## GetWorkloadDeploymentPatternInputTypeDef

```python
# GetWorkloadDeploymentPatternInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import GetWorkloadDeploymentPatternInputTypeDef


def get_value() -> GetWorkloadDeploymentPatternInputTypeDef:
    return {
        "deploymentPatternName": ...,
    }


# GetWorkloadDeploymentPatternInputTypeDef definition

class GetWorkloadDeploymentPatternInputTypeDef(TypedDict):
    deploymentPatternName: str,
    workloadName: str,
```

## GetWorkloadInputTypeDef

```python
# GetWorkloadInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import GetWorkloadInputTypeDef


def get_value() -> GetWorkloadInputTypeDef:
    return {
        "workloadName": ...,
    }


# GetWorkloadInputTypeDef definition

class GetWorkloadInputTypeDef(TypedDict):
    workloadName: str,
```

## WorkloadDataTypeDef

```python
# WorkloadDataTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import WorkloadDataTypeDef


def get_value() -> WorkloadDataTypeDef:
    return {
        "description": ...,
    }


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
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import PaginatorConfigTypeDef


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

## ListDeploymentEventsInputTypeDef

```python
# ListDeploymentEventsInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListDeploymentEventsInputTypeDef


def get_value() -> ListDeploymentEventsInputTypeDef:
    return {
        "deploymentId": ...,
    }


# ListDeploymentEventsInputTypeDef definition

class ListDeploymentEventsInputTypeDef(TypedDict):
    deploymentId: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```

## ListWorkloadDeploymentPatternsInputTypeDef

```python
# ListWorkloadDeploymentPatternsInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListWorkloadDeploymentPatternsInputTypeDef


def get_value() -> ListWorkloadDeploymentPatternsInputTypeDef:
    return {
        "workloadName": ...,
    }


# ListWorkloadDeploymentPatternsInputTypeDef definition

class ListWorkloadDeploymentPatternsInputTypeDef(TypedDict):
    workloadName: str,
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WorkloadDeploymentPatternDataSummaryTypeDef

```python
# WorkloadDeploymentPatternDataSummaryTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import WorkloadDeploymentPatternDataSummaryTypeDef


def get_value() -> WorkloadDeploymentPatternDataSummaryTypeDef:
    return {
        "deploymentPatternName": ...,
    }


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
## ListWorkloadsInputTypeDef

```python
# ListWorkloadsInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListWorkloadsInputTypeDef


def get_value() -> ListWorkloadsInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListWorkloadsInputTypeDef definition

class ListWorkloadsInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## WorkloadDataSummaryTypeDef

```python
# WorkloadDataSummaryTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import WorkloadDataSummaryTypeDef


def get_value() -> WorkloadDataSummaryTypeDef:
    return {
        "displayName": ...,
    }


# WorkloadDataSummaryTypeDef definition

class WorkloadDataSummaryTypeDef(TypedDict):
    displayName: NotRequired[str],
    workloadName: NotRequired[str],
```

## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## CreateDeploymentOutputTypeDef

```python
# CreateDeploymentOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import CreateDeploymentOutputTypeDef


def get_value() -> CreateDeploymentOutputTypeDef:
    return {
        "deploymentId": ...,
    }


# CreateDeploymentOutputTypeDef definition

class CreateDeploymentOutputTypeDef(TypedDict):
    deploymentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteDeploymentOutputTypeDef

```python
# DeleteDeploymentOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import DeleteDeploymentOutputTypeDef


def get_value() -> DeleteDeploymentOutputTypeDef:
    return {
        "status": ...,
    }


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
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeploymentSpecificationsFieldTypeDef

```python
# DeploymentSpecificationsFieldTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import DeploymentSpecificationsFieldTypeDef


def get_value() -> DeploymentSpecificationsFieldTypeDef:
    return {
        "allowedValues": ...,
    }


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
# ListDeploymentsOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListDeploymentsOutputTypeDef


def get_value() -> ListDeploymentsOutputTypeDef:
    return {
        "deployments": ...,
    }


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
# GetDeploymentOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import GetDeploymentOutputTypeDef


def get_value() -> GetDeploymentOutputTypeDef:
    return {
        "deployment": ...,
    }


# GetDeploymentOutputTypeDef definition

class GetDeploymentOutputTypeDef(TypedDict):
    deployment: DeploymentDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DeploymentDataTypeDef](./type_defs.md#deploymentdatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentEventsOutputTypeDef

```python
# ListDeploymentEventsOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListDeploymentEventsOutputTypeDef


def get_value() -> ListDeploymentEventsOutputTypeDef:
    return {
        "deploymentEvents": ...,
    }


# ListDeploymentEventsOutputTypeDef definition

class ListDeploymentEventsOutputTypeDef(TypedDict):
    deploymentEvents: List[DeploymentEventDataSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentEventDataSummaryTypeDef](./type_defs.md#deploymenteventdatasummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentsInputTypeDef

```python
# ListDeploymentsInputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListDeploymentsInputTypeDef


def get_value() -> ListDeploymentsInputTypeDef:
    return {
        "filters": ...,
    }


# ListDeploymentsInputTypeDef definition

class ListDeploymentsInputTypeDef(TypedDict):
    filters: NotRequired[Sequence[DeploymentFilterTypeDef]],  # (1)
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef) 
## GetWorkloadOutputTypeDef

```python
# GetWorkloadOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import GetWorkloadOutputTypeDef


def get_value() -> GetWorkloadOutputTypeDef:
    return {
        "workload": ...,
    }


# GetWorkloadOutputTypeDef definition

class GetWorkloadOutputTypeDef(TypedDict):
    workload: WorkloadDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadDataTypeDef](./type_defs.md#workloaddatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDeploymentEventsInputPaginateTypeDef

```python
# ListDeploymentEventsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListDeploymentEventsInputPaginateTypeDef


def get_value() -> ListDeploymentEventsInputPaginateTypeDef:
    return {
        "deploymentId": ...,
    }


# ListDeploymentEventsInputPaginateTypeDef definition

class ListDeploymentEventsInputPaginateTypeDef(TypedDict):
    deploymentId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDeploymentsInputPaginateTypeDef

```python
# ListDeploymentsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListDeploymentsInputPaginateTypeDef


def get_value() -> ListDeploymentsInputPaginateTypeDef:
    return {
        "filters": ...,
    }


# ListDeploymentsInputPaginateTypeDef definition

class ListDeploymentsInputPaginateTypeDef(TypedDict):
    filters: NotRequired[Sequence[DeploymentFilterTypeDef]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-braces: DeploymentFilterTypeDef](./type_defs.md#deploymentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkloadDeploymentPatternsInputPaginateTypeDef

```python
# ListWorkloadDeploymentPatternsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListWorkloadDeploymentPatternsInputPaginateTypeDef


def get_value() -> ListWorkloadDeploymentPatternsInputPaginateTypeDef:
    return {
        "workloadName": ...,
    }


# ListWorkloadDeploymentPatternsInputPaginateTypeDef definition

class ListWorkloadDeploymentPatternsInputPaginateTypeDef(TypedDict):
    workloadName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkloadsInputPaginateTypeDef

```python
# ListWorkloadsInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListWorkloadsInputPaginateTypeDef


def get_value() -> ListWorkloadsInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListWorkloadsInputPaginateTypeDef definition

class ListWorkloadsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListWorkloadDeploymentPatternsOutputTypeDef

```python
# ListWorkloadDeploymentPatternsOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListWorkloadDeploymentPatternsOutputTypeDef


def get_value() -> ListWorkloadDeploymentPatternsOutputTypeDef:
    return {
        "nextToken": ...,
    }


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
# ListWorkloadsOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import ListWorkloadsOutputTypeDef


def get_value() -> ListWorkloadsOutputTypeDef:
    return {
        "nextToken": ...,
    }


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
# WorkloadDeploymentPatternDataTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import WorkloadDeploymentPatternDataTypeDef


def get_value() -> WorkloadDeploymentPatternDataTypeDef:
    return {
        "deploymentPatternName": ...,
    }


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
# GetWorkloadDeploymentPatternOutputTypeDef TypedDict usage example

from types_aiobotocore_launch_wizard.type_defs import GetWorkloadDeploymentPatternOutputTypeDef


def get_value() -> GetWorkloadDeploymentPatternOutputTypeDef:
    return {
        "workloadDeploymentPattern": ...,
    }


# GetWorkloadDeploymentPatternOutputTypeDef definition

class GetWorkloadDeploymentPatternOutputTypeDef(TypedDict):
    workloadDeploymentPattern: WorkloadDeploymentPatternDataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkloadDeploymentPatternDataTypeDef](./type_defs.md#workloaddeploymentpatterndatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

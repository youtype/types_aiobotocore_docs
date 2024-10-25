# Type definitions

> [Index](../README.md) > [IoTJobsDataPlane](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [IoTJobsDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
    type annotations stubs module [types-aiobotocore-iot-jobs-data](https://pypi.org/project/types-aiobotocore-iot-jobs-data/).



## DescribeJobExecutionRequestRequestTypeDef

```python
# DescribeJobExecutionRequestRequestTypeDef definition

class DescribeJobExecutionRequestRequestTypeDef(TypedDict):
    jobId: str,
    thingName: str,
    includeJobDocument: NotRequired[bool],
    executionNumber: NotRequired[int],
```

## JobExecutionTypeDef

```python
# JobExecutionTypeDef definition

class JobExecutionTypeDef(TypedDict):
    jobId: NotRequired[str],
    thingName: NotRequired[str],
    status: NotRequired[JobExecutionStatusType],  # (1)
    statusDetails: NotRequired[Dict[str, str]],
    queuedAt: NotRequired[int],
    startedAt: NotRequired[int],
    lastUpdatedAt: NotRequired[int],
    approximateSecondsBeforeTimedOut: NotRequired[int],
    versionNumber: NotRequired[int],
    executionNumber: NotRequired[int],
    jobDocument: NotRequired[str],
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
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

## GetPendingJobExecutionsRequestRequestTypeDef

```python
# GetPendingJobExecutionsRequestRequestTypeDef definition

class GetPendingJobExecutionsRequestRequestTypeDef(TypedDict):
    thingName: str,
```

## JobExecutionSummaryTypeDef

```python
# JobExecutionSummaryTypeDef definition

class JobExecutionSummaryTypeDef(TypedDict):
    jobId: NotRequired[str],
    queuedAt: NotRequired[int],
    startedAt: NotRequired[int],
    lastUpdatedAt: NotRequired[int],
    versionNumber: NotRequired[int],
    executionNumber: NotRequired[int],
```

## JobExecutionStateTypeDef

```python
# JobExecutionStateTypeDef definition

class JobExecutionStateTypeDef(TypedDict):
    status: NotRequired[JobExecutionStatusType],  # (1)
    statusDetails: NotRequired[Dict[str, str]],
    versionNumber: NotRequired[int],
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
## StartNextPendingJobExecutionRequestRequestTypeDef

```python
# StartNextPendingJobExecutionRequestRequestTypeDef definition

class StartNextPendingJobExecutionRequestRequestTypeDef(TypedDict):
    thingName: str,
    statusDetails: NotRequired[Mapping[str, str]],
    stepTimeoutInMinutes: NotRequired[int],
```

## UpdateJobExecutionRequestRequestTypeDef

```python
# UpdateJobExecutionRequestRequestTypeDef definition

class UpdateJobExecutionRequestRequestTypeDef(TypedDict):
    jobId: str,
    thingName: str,
    status: JobExecutionStatusType,  # (1)
    statusDetails: NotRequired[Mapping[str, str]],
    stepTimeoutInMinutes: NotRequired[int],
    expectedVersion: NotRequired[int],
    includeJobExecutionState: NotRequired[bool],
    includeJobDocument: NotRequired[bool],
    executionNumber: NotRequired[int],
```

1. See [:material-code-brackets: JobExecutionStatusType](./literals.md#jobexecutionstatustype) 
## DescribeJobExecutionResponseTypeDef

```python
# DescribeJobExecutionResponseTypeDef definition

class DescribeJobExecutionResponseTypeDef(TypedDict):
    execution: JobExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobExecutionTypeDef](./type_defs.md#jobexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartNextPendingJobExecutionResponseTypeDef

```python
# StartNextPendingJobExecutionResponseTypeDef definition

class StartNextPendingJobExecutionResponseTypeDef(TypedDict):
    execution: JobExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobExecutionTypeDef](./type_defs.md#jobexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPendingJobExecutionsResponseTypeDef

```python
# GetPendingJobExecutionsResponseTypeDef definition

class GetPendingJobExecutionsResponseTypeDef(TypedDict):
    inProgressJobs: List[JobExecutionSummaryTypeDef],  # (1)
    queuedJobs: List[JobExecutionSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: JobExecutionSummaryTypeDef](./type_defs.md#jobexecutionsummarytypedef) 
2. See [:material-code-braces: JobExecutionSummaryTypeDef](./type_defs.md#jobexecutionsummarytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateJobExecutionResponseTypeDef

```python
# UpdateJobExecutionResponseTypeDef definition

class UpdateJobExecutionResponseTypeDef(TypedDict):
    executionState: JobExecutionStateTypeDef,  # (1)
    jobDocument: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: JobExecutionStateTypeDef](./type_defs.md#jobexecutionstatetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

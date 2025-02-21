# Type definitions

> [Index](../README.md) > [SimSpaceWeaver](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SimSpaceWeaver](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/simspaceweaver.html#simspaceweaver)
    type annotations stubs module [types-aiobotocore-simspaceweaver](https://pypi.org/project/types-aiobotocore-simspaceweaver/).

## LaunchOverridesUnionTypeDef

```python
# LaunchOverridesUnionTypeDef Union usage example

from types_aiobotocore_simspaceweaver.type_defs import LaunchOverridesUnionTypeDef


def get_value() -> LaunchOverridesUnionTypeDef:
    return ...


# LaunchOverridesUnionTypeDef definition

LaunchOverridesUnionTypeDef = Union[
    LaunchOverridesTypeDef,  # (1)
    LaunchOverridesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: LaunchOverridesTypeDef](./type_defs.md#launchoverridestypedef) 
2. See [:material-code-braces: LaunchOverridesOutputTypeDef](./type_defs.md#launchoverridesoutputtypedef) 



## CloudWatchLogsLogGroupTypeDef

```python
# CloudWatchLogsLogGroupTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import CloudWatchLogsLogGroupTypeDef


def get_value() -> CloudWatchLogsLogGroupTypeDef:
    return {
        "LogGroupArn": ...,
    }


# CloudWatchLogsLogGroupTypeDef definition

class CloudWatchLogsLogGroupTypeDef(TypedDict):
    LogGroupArn: NotRequired[str],
```

## S3DestinationTypeDef

```python
# S3DestinationTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import S3DestinationTypeDef


def get_value() -> S3DestinationTypeDef:
    return {
        "BucketName": ...,
    }


# S3DestinationTypeDef definition

class S3DestinationTypeDef(TypedDict):
    BucketName: str,
    ObjectKeyPrefix: NotRequired[str],
```

## DeleteAppInputTypeDef

```python
# DeleteAppInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import DeleteAppInputTypeDef


def get_value() -> DeleteAppInputTypeDef:
    return {
        "App": ...,
    }


# DeleteAppInputTypeDef definition

class DeleteAppInputTypeDef(TypedDict):
    App: str,
    Domain: str,
    Simulation: str,
```

## DeleteSimulationInputTypeDef

```python
# DeleteSimulationInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import DeleteSimulationInputTypeDef


def get_value() -> DeleteSimulationInputTypeDef:
    return {
        "Simulation": ...,
    }


# DeleteSimulationInputTypeDef definition

class DeleteSimulationInputTypeDef(TypedDict):
    Simulation: str,
```

## DescribeAppInputTypeDef

```python
# DescribeAppInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import DescribeAppInputTypeDef


def get_value() -> DescribeAppInputTypeDef:
    return {
        "App": ...,
    }


# DescribeAppInputTypeDef definition

class DescribeAppInputTypeDef(TypedDict):
    App: str,
    Domain: str,
    Simulation: str,
```

## LaunchOverridesOutputTypeDef

```python
# LaunchOverridesOutputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import LaunchOverridesOutputTypeDef


def get_value() -> LaunchOverridesOutputTypeDef:
    return {
        "LaunchCommands": ...,
    }


# LaunchOverridesOutputTypeDef definition

class LaunchOverridesOutputTypeDef(TypedDict):
    LaunchCommands: NotRequired[List[str]],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import ResponseMetadataTypeDef


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

## DescribeSimulationInputTypeDef

```python
# DescribeSimulationInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import DescribeSimulationInputTypeDef


def get_value() -> DescribeSimulationInputTypeDef:
    return {
        "Simulation": ...,
    }


# DescribeSimulationInputTypeDef definition

class DescribeSimulationInputTypeDef(TypedDict):
    Simulation: str,
```

## S3LocationTypeDef

```python
# S3LocationTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import S3LocationTypeDef


def get_value() -> S3LocationTypeDef:
    return {
        "BucketName": ...,
    }


# S3LocationTypeDef definition

class S3LocationTypeDef(TypedDict):
    BucketName: str,
    ObjectKey: str,
```

## DomainTypeDef

```python
# DomainTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import DomainTypeDef


def get_value() -> DomainTypeDef:
    return {
        "Lifecycle": ...,
    }


# DomainTypeDef definition

class DomainTypeDef(TypedDict):
    Lifecycle: NotRequired[LifecycleManagementStrategyType],  # (1)
    Name: NotRequired[str],
```

1. See [:material-code-brackets: LifecycleManagementStrategyType](./literals.md#lifecyclemanagementstrategytype) 
## LaunchOverridesTypeDef

```python
# LaunchOverridesTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import LaunchOverridesTypeDef


def get_value() -> LaunchOverridesTypeDef:
    return {
        "LaunchCommands": ...,
    }


# LaunchOverridesTypeDef definition

class LaunchOverridesTypeDef(TypedDict):
    LaunchCommands: NotRequired[Sequence[str]],
```

## ListAppsInputTypeDef

```python
# ListAppsInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import ListAppsInputTypeDef


def get_value() -> ListAppsInputTypeDef:
    return {
        "Simulation": ...,
    }


# ListAppsInputTypeDef definition

class ListAppsInputTypeDef(TypedDict):
    Simulation: str,
    Domain: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SimulationAppMetadataTypeDef

```python
# SimulationAppMetadataTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import SimulationAppMetadataTypeDef


def get_value() -> SimulationAppMetadataTypeDef:
    return {
        "Domain": ...,
    }


# SimulationAppMetadataTypeDef definition

class SimulationAppMetadataTypeDef(TypedDict):
    Domain: NotRequired[str],
    Name: NotRequired[str],
    Simulation: NotRequired[str],
    Status: NotRequired[SimulationAppStatusType],  # (1)
    TargetStatus: NotRequired[SimulationAppTargetStatusType],  # (2)
```

1. See [:material-code-brackets: SimulationAppStatusType](./literals.md#simulationappstatustype) 
2. See [:material-code-brackets: SimulationAppTargetStatusType](./literals.md#simulationapptargetstatustype) 
## ListSimulationsInputTypeDef

```python
# ListSimulationsInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import ListSimulationsInputTypeDef


def get_value() -> ListSimulationsInputTypeDef:
    return {
        "MaxResults": ...,
    }


# ListSimulationsInputTypeDef definition

class ListSimulationsInputTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## SimulationMetadataTypeDef

```python
# SimulationMetadataTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import SimulationMetadataTypeDef


def get_value() -> SimulationMetadataTypeDef:
    return {
        "Arn": ...,
    }


# SimulationMetadataTypeDef definition

class SimulationMetadataTypeDef(TypedDict):
    Arn: NotRequired[str],
    CreationTime: NotRequired[datetime],
    Name: NotRequired[str],
    Status: NotRequired[SimulationStatusType],  # (1)
    TargetStatus: NotRequired[SimulationTargetStatusType],  # (2)
```

1. See [:material-code-brackets: SimulationStatusType](./literals.md#simulationstatustype) 
2. See [:material-code-brackets: SimulationTargetStatusType](./literals.md#simulationtargetstatustype) 
## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    ResourceArn: str,
```

## SimulationClockTypeDef

```python
# SimulationClockTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import SimulationClockTypeDef


def get_value() -> SimulationClockTypeDef:
    return {
        "Status": ...,
    }


# SimulationClockTypeDef definition

class SimulationClockTypeDef(TypedDict):
    Status: NotRequired[ClockStatusType],  # (1)
    TargetStatus: NotRequired[ClockTargetStatusType],  # (2)
```

1. See [:material-code-brackets: ClockStatusType](./literals.md#clockstatustype) 
2. See [:material-code-brackets: ClockTargetStatusType](./literals.md#clocktargetstatustype) 
## SimulationAppPortMappingTypeDef

```python
# SimulationAppPortMappingTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import SimulationAppPortMappingTypeDef


def get_value() -> SimulationAppPortMappingTypeDef:
    return {
        "Actual": ...,
    }


# SimulationAppPortMappingTypeDef definition

class SimulationAppPortMappingTypeDef(TypedDict):
    Actual: NotRequired[int],
    Declared: NotRequired[int],
```

## StartClockInputTypeDef

```python
# StartClockInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import StartClockInputTypeDef


def get_value() -> StartClockInputTypeDef:
    return {
        "Simulation": ...,
    }


# StartClockInputTypeDef definition

class StartClockInputTypeDef(TypedDict):
    Simulation: str,
```

## StopAppInputTypeDef

```python
# StopAppInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import StopAppInputTypeDef


def get_value() -> StopAppInputTypeDef:
    return {
        "App": ...,
    }


# StopAppInputTypeDef definition

class StopAppInputTypeDef(TypedDict):
    App: str,
    Domain: str,
    Simulation: str,
```

## StopClockInputTypeDef

```python
# StopClockInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import StopClockInputTypeDef


def get_value() -> StopClockInputTypeDef:
    return {
        "Simulation": ...,
    }


# StopClockInputTypeDef definition

class StopClockInputTypeDef(TypedDict):
    Simulation: str,
```

## StopSimulationInputTypeDef

```python
# StopSimulationInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import StopSimulationInputTypeDef


def get_value() -> StopSimulationInputTypeDef:
    return {
        "Simulation": ...,
    }


# StopSimulationInputTypeDef definition

class StopSimulationInputTypeDef(TypedDict):
    Simulation: str,
```

## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import TagResourceInputTypeDef


def get_value() -> TagResourceInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceInputTypeDef definition

class TagResourceInputTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceInputTypeDef

```python
# UntagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## LogDestinationTypeDef

```python
# LogDestinationTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import LogDestinationTypeDef


def get_value() -> LogDestinationTypeDef:
    return {
        "CloudWatchLogsLogGroup": ...,
    }


# LogDestinationTypeDef definition

class LogDestinationTypeDef(TypedDict):
    CloudWatchLogsLogGroup: NotRequired[CloudWatchLogsLogGroupTypeDef],  # (1)
```

1. See [:material-code-braces: CloudWatchLogsLogGroupTypeDef](./type_defs.md#cloudwatchlogsloggrouptypedef) 
## CreateSnapshotInputTypeDef

```python
# CreateSnapshotInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import CreateSnapshotInputTypeDef


def get_value() -> CreateSnapshotInputTypeDef:
    return {
        "Destination": ...,
    }


# CreateSnapshotInputTypeDef definition

class CreateSnapshotInputTypeDef(TypedDict):
    Destination: S3DestinationTypeDef,  # (1)
    Simulation: str,
```

1. See [:material-code-braces: S3DestinationTypeDef](./type_defs.md#s3destinationtypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartAppOutputTypeDef

```python
# StartAppOutputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import StartAppOutputTypeDef


def get_value() -> StartAppOutputTypeDef:
    return {
        "Domain": ...,
    }


# StartAppOutputTypeDef definition

class StartAppOutputTypeDef(TypedDict):
    Domain: str,
    Name: str,
    Simulation: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSimulationOutputTypeDef

```python
# StartSimulationOutputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import StartSimulationOutputTypeDef


def get_value() -> StartSimulationOutputTypeDef:
    return {
        "Arn": ...,
    }


# StartSimulationOutputTypeDef definition

class StartSimulationOutputTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    ExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StartSimulationInputTypeDef

```python
# StartSimulationInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import StartSimulationInputTypeDef


def get_value() -> StartSimulationInputTypeDef:
    return {
        "Name": ...,
    }


# StartSimulationInputTypeDef definition

class StartSimulationInputTypeDef(TypedDict):
    Name: str,
    RoleArn: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    MaximumDuration: NotRequired[str],
    SchemaS3Location: NotRequired[S3LocationTypeDef],  # (1)
    SnapshotS3Location: NotRequired[S3LocationTypeDef],  # (1)
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
2. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
## ListAppsOutputTypeDef

```python
# ListAppsOutputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import ListAppsOutputTypeDef


def get_value() -> ListAppsOutputTypeDef:
    return {
        "Apps": ...,
    }


# ListAppsOutputTypeDef definition

class ListAppsOutputTypeDef(TypedDict):
    Apps: List[SimulationAppMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SimulationAppMetadataTypeDef](./type_defs.md#simulationappmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSimulationsOutputTypeDef

```python
# ListSimulationsOutputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import ListSimulationsOutputTypeDef


def get_value() -> ListSimulationsOutputTypeDef:
    return {
        "NextToken": ...,
    }


# ListSimulationsOutputTypeDef definition

class ListSimulationsOutputTypeDef(TypedDict):
    Simulations: List[SimulationMetadataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SimulationMetadataTypeDef](./type_defs.md#simulationmetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LiveSimulationStateTypeDef

```python
# LiveSimulationStateTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import LiveSimulationStateTypeDef


def get_value() -> LiveSimulationStateTypeDef:
    return {
        "Clocks": ...,
    }


# LiveSimulationStateTypeDef definition

class LiveSimulationStateTypeDef(TypedDict):
    Clocks: NotRequired[List[SimulationClockTypeDef]],  # (1)
    Domains: NotRequired[List[DomainTypeDef]],  # (2)
```

1. See [:material-code-braces: SimulationClockTypeDef](./type_defs.md#simulationclocktypedef) 
2. See [:material-code-braces: DomainTypeDef](./type_defs.md#domaintypedef) 
## SimulationAppEndpointInfoTypeDef

```python
# SimulationAppEndpointInfoTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import SimulationAppEndpointInfoTypeDef


def get_value() -> SimulationAppEndpointInfoTypeDef:
    return {
        "Address": ...,
    }


# SimulationAppEndpointInfoTypeDef definition

class SimulationAppEndpointInfoTypeDef(TypedDict):
    Address: NotRequired[str],
    IngressPortMappings: NotRequired[List[SimulationAppPortMappingTypeDef]],  # (1)
```

1. See [:material-code-braces: SimulationAppPortMappingTypeDef](./type_defs.md#simulationappportmappingtypedef) 
## LoggingConfigurationTypeDef

```python
# LoggingConfigurationTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import LoggingConfigurationTypeDef


def get_value() -> LoggingConfigurationTypeDef:
    return {
        "Destinations": ...,
    }


# LoggingConfigurationTypeDef definition

class LoggingConfigurationTypeDef(TypedDict):
    Destinations: NotRequired[List[LogDestinationTypeDef]],  # (1)
```

1. See [:material-code-braces: LogDestinationTypeDef](./type_defs.md#logdestinationtypedef) 
## StartAppInputTypeDef

```python
# StartAppInputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import StartAppInputTypeDef


def get_value() -> StartAppInputTypeDef:
    return {
        "Domain": ...,
    }


# StartAppInputTypeDef definition

class StartAppInputTypeDef(TypedDict):
    Domain: str,
    Name: str,
    Simulation: str,
    ClientToken: NotRequired[str],
    Description: NotRequired[str],
    LaunchOverrides: NotRequired[LaunchOverridesUnionTypeDef],  # (1)
```

1. See [:material-code-braces: LaunchOverridesTypeDef](./type_defs.md#launchoverridestypedef) [:material-code-braces: LaunchOverridesOutputTypeDef](./type_defs.md#launchoverridesoutputtypedef) 
## DescribeAppOutputTypeDef

```python
# DescribeAppOutputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import DescribeAppOutputTypeDef


def get_value() -> DescribeAppOutputTypeDef:
    return {
        "Description": ...,
    }


# DescribeAppOutputTypeDef definition

class DescribeAppOutputTypeDef(TypedDict):
    Description: str,
    Domain: str,
    EndpointInfo: SimulationAppEndpointInfoTypeDef,  # (1)
    LaunchOverrides: LaunchOverridesOutputTypeDef,  # (2)
    Name: str,
    Simulation: str,
    Status: SimulationAppStatusType,  # (3)
    TargetStatus: SimulationAppTargetStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SimulationAppEndpointInfoTypeDef](./type_defs.md#simulationappendpointinfotypedef) 
2. See [:material-code-braces: LaunchOverridesOutputTypeDef](./type_defs.md#launchoverridesoutputtypedef) 
3. See [:material-code-brackets: SimulationAppStatusType](./literals.md#simulationappstatustype) 
4. See [:material-code-brackets: SimulationAppTargetStatusType](./literals.md#simulationapptargetstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeSimulationOutputTypeDef

```python
# DescribeSimulationOutputTypeDef TypedDict usage example

from types_aiobotocore_simspaceweaver.type_defs import DescribeSimulationOutputTypeDef


def get_value() -> DescribeSimulationOutputTypeDef:
    return {
        "Arn": ...,
    }


# DescribeSimulationOutputTypeDef definition

class DescribeSimulationOutputTypeDef(TypedDict):
    Arn: str,
    CreationTime: datetime,
    Description: str,
    ExecutionId: str,
    LiveSimulationState: LiveSimulationStateTypeDef,  # (1)
    LoggingConfiguration: LoggingConfigurationTypeDef,  # (2)
    MaximumDuration: str,
    Name: str,
    RoleArn: str,
    SchemaError: str,
    SchemaS3Location: S3LocationTypeDef,  # (3)
    SnapshotS3Location: S3LocationTypeDef,  # (3)
    StartError: str,
    Status: SimulationStatusType,  # (5)
    TargetStatus: SimulationTargetStatusType,  # (6)
    ResponseMetadata: ResponseMetadataTypeDef,  # (7)
```

1. See [:material-code-braces: LiveSimulationStateTypeDef](./type_defs.md#livesimulationstatetypedef) 
2. See [:material-code-braces: LoggingConfigurationTypeDef](./type_defs.md#loggingconfigurationtypedef) 
3. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
4. See [:material-code-braces: S3LocationTypeDef](./type_defs.md#s3locationtypedef) 
5. See [:material-code-brackets: SimulationStatusType](./literals.md#simulationstatustype) 
6. See [:material-code-brackets: SimulationTargetStatusType](./literals.md#simulationtargetstatustype) 
7. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

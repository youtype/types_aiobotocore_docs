# Type definitions

> [Index](../README.md) > [Synthetics](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Synthetics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/synthetics.html#synthetics)
    type annotations stubs module [types-aiobotocore-synthetics](https://pypi.org/project/types-aiobotocore-synthetics/).

## BlobTypeDef

```python
# BlobTypeDef Union usage example

from types_aiobotocore_synthetics.type_defs import BlobTypeDef


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


## BaseScreenshotUnionTypeDef

```python
# BaseScreenshotUnionTypeDef Union usage example

from types_aiobotocore_synthetics.type_defs import BaseScreenshotUnionTypeDef


def get_value() -> BaseScreenshotUnionTypeDef:
    return ...


# BaseScreenshotUnionTypeDef definition

BaseScreenshotUnionTypeDef = Union[
    BaseScreenshotTypeDef,  # (1)
    BaseScreenshotOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: BaseScreenshotTypeDef](./type_defs.md#basescreenshottypedef) 
2. See [:material-code-braces: BaseScreenshotOutputTypeDef](./type_defs.md#basescreenshotoutputtypedef) 



## S3EncryptionConfigTypeDef

```python
# S3EncryptionConfigTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import S3EncryptionConfigTypeDef


def get_value() -> S3EncryptionConfigTypeDef:
    return {
        "EncryptionMode": ...,
    }


# S3EncryptionConfigTypeDef definition

class S3EncryptionConfigTypeDef(TypedDict):
    EncryptionMode: NotRequired[EncryptionModeType],  # (1)
    KmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionModeType](./literals.md#encryptionmodetype) 
## AssociateResourceRequestTypeDef

```python
# AssociateResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import AssociateResourceRequestTypeDef


def get_value() -> AssociateResourceRequestTypeDef:
    return {
        "GroupIdentifier": ...,
    }


# AssociateResourceRequestTypeDef definition

class AssociateResourceRequestTypeDef(TypedDict):
    GroupIdentifier: str,
    ResourceArn: str,
```

## BaseScreenshotOutputTypeDef

```python
# BaseScreenshotOutputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import BaseScreenshotOutputTypeDef


def get_value() -> BaseScreenshotOutputTypeDef:
    return {
        "ScreenshotName": ...,
    }


# BaseScreenshotOutputTypeDef definition

class BaseScreenshotOutputTypeDef(TypedDict):
    ScreenshotName: str,
    IgnoreCoordinates: NotRequired[List[str]],
```

## BaseScreenshotTypeDef

```python
# BaseScreenshotTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import BaseScreenshotTypeDef


def get_value() -> BaseScreenshotTypeDef:
    return {
        "ScreenshotName": ...,
    }


# BaseScreenshotTypeDef definition

class BaseScreenshotTypeDef(TypedDict):
    ScreenshotName: str,
    IgnoreCoordinates: NotRequired[Sequence[str]],
```

## CanaryCodeOutputTypeDef

```python
# CanaryCodeOutputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryCodeOutputTypeDef


def get_value() -> CanaryCodeOutputTypeDef:
    return {
        "SourceLocationArn": ...,
    }


# CanaryCodeOutputTypeDef definition

class CanaryCodeOutputTypeDef(TypedDict):
    SourceLocationArn: NotRequired[str],
    Handler: NotRequired[str],
```

## CanaryRunConfigInputTypeDef

```python
# CanaryRunConfigInputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryRunConfigInputTypeDef


def get_value() -> CanaryRunConfigInputTypeDef:
    return {
        "TimeoutInSeconds": ...,
    }


# CanaryRunConfigInputTypeDef definition

class CanaryRunConfigInputTypeDef(TypedDict):
    TimeoutInSeconds: NotRequired[int],
    MemoryInMB: NotRequired[int],
    ActiveTracing: NotRequired[bool],
    EnvironmentVariables: NotRequired[Mapping[str, str]],
```

## CanaryRunConfigOutputTypeDef

```python
# CanaryRunConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryRunConfigOutputTypeDef


def get_value() -> CanaryRunConfigOutputTypeDef:
    return {
        "TimeoutInSeconds": ...,
    }


# CanaryRunConfigOutputTypeDef definition

class CanaryRunConfigOutputTypeDef(TypedDict):
    TimeoutInSeconds: NotRequired[int],
    MemoryInMB: NotRequired[int],
    ActiveTracing: NotRequired[bool],
```

## CanaryRunStatusTypeDef

```python
# CanaryRunStatusTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryRunStatusTypeDef


def get_value() -> CanaryRunStatusTypeDef:
    return {
        "State": ...,
    }


# CanaryRunStatusTypeDef definition

class CanaryRunStatusTypeDef(TypedDict):
    State: NotRequired[CanaryRunStateType],  # (1)
    StateReason: NotRequired[str],
    StateReasonCode: NotRequired[CanaryRunStateReasonCodeType],  # (2)
```

1. See [:material-code-brackets: CanaryRunStateType](./literals.md#canaryrunstatetype) 
2. See [:material-code-brackets: CanaryRunStateReasonCodeType](./literals.md#canaryrunstatereasoncodetype) 
## CanaryRunTimelineTypeDef

```python
# CanaryRunTimelineTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryRunTimelineTypeDef


def get_value() -> CanaryRunTimelineTypeDef:
    return {
        "Started": ...,
    }


# CanaryRunTimelineTypeDef definition

class CanaryRunTimelineTypeDef(TypedDict):
    Started: NotRequired[datetime],
    Completed: NotRequired[datetime],
```

## CanaryScheduleInputTypeDef

```python
# CanaryScheduleInputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryScheduleInputTypeDef


def get_value() -> CanaryScheduleInputTypeDef:
    return {
        "Expression": ...,
    }


# CanaryScheduleInputTypeDef definition

class CanaryScheduleInputTypeDef(TypedDict):
    Expression: str,
    DurationInSeconds: NotRequired[int],
```

## CanaryScheduleOutputTypeDef

```python
# CanaryScheduleOutputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryScheduleOutputTypeDef


def get_value() -> CanaryScheduleOutputTypeDef:
    return {
        "Expression": ...,
    }


# CanaryScheduleOutputTypeDef definition

class CanaryScheduleOutputTypeDef(TypedDict):
    Expression: NotRequired[str],
    DurationInSeconds: NotRequired[int],
```

## CanaryStatusTypeDef

```python
# CanaryStatusTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryStatusTypeDef


def get_value() -> CanaryStatusTypeDef:
    return {
        "State": ...,
    }


# CanaryStatusTypeDef definition

class CanaryStatusTypeDef(TypedDict):
    State: NotRequired[CanaryStateType],  # (1)
    StateReason: NotRequired[str],
    StateReasonCode: NotRequired[CanaryStateReasonCodeType],  # (2)
```

1. See [:material-code-brackets: CanaryStateType](./literals.md#canarystatetype) 
2. See [:material-code-brackets: CanaryStateReasonCodeType](./literals.md#canarystatereasoncodetype) 
## CanaryTimelineTypeDef

```python
# CanaryTimelineTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryTimelineTypeDef


def get_value() -> CanaryTimelineTypeDef:
    return {
        "Created": ...,
    }


# CanaryTimelineTypeDef definition

class CanaryTimelineTypeDef(TypedDict):
    Created: NotRequired[datetime],
    LastModified: NotRequired[datetime],
    LastStarted: NotRequired[datetime],
    LastStopped: NotRequired[datetime],
```

## VpcConfigOutputTypeDef

```python
# VpcConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import VpcConfigOutputTypeDef


def get_value() -> VpcConfigOutputTypeDef:
    return {
        "VpcId": ...,
    }


# VpcConfigOutputTypeDef definition

class VpcConfigOutputTypeDef(TypedDict):
    VpcId: NotRequired[str],
    SubnetIds: NotRequired[List[str]],
    SecurityGroupIds: NotRequired[List[str]],
    Ipv6AllowedForDualStack: NotRequired[bool],
```

## VpcConfigInputTypeDef

```python
# VpcConfigInputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import VpcConfigInputTypeDef


def get_value() -> VpcConfigInputTypeDef:
    return {
        "SubnetIds": ...,
    }


# VpcConfigInputTypeDef definition

class VpcConfigInputTypeDef(TypedDict):
    SubnetIds: NotRequired[Sequence[str]],
    SecurityGroupIds: NotRequired[Sequence[str]],
    Ipv6AllowedForDualStack: NotRequired[bool],
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ResponseMetadataTypeDef


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

## CreateGroupRequestTypeDef

```python
# CreateGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CreateGroupRequestTypeDef


def get_value() -> CreateGroupRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateGroupRequestTypeDef definition

class CreateGroupRequestTypeDef(TypedDict):
    Name: str,
    Tags: NotRequired[Mapping[str, str]],
```

## GroupTypeDef

```python
# GroupTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import GroupTypeDef


def get_value() -> GroupTypeDef:
    return {
        "Id": ...,
    }


# GroupTypeDef definition

class GroupTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Arn: NotRequired[str],
    Tags: NotRequired[Dict[str, str]],
    CreatedTime: NotRequired[datetime],
    LastModifiedTime: NotRequired[datetime],
```

## DeleteCanaryRequestTypeDef

```python
# DeleteCanaryRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DeleteCanaryRequestTypeDef


def get_value() -> DeleteCanaryRequestTypeDef:
    return {
        "Name": ...,
    }


# DeleteCanaryRequestTypeDef definition

class DeleteCanaryRequestTypeDef(TypedDict):
    Name: str,
    DeleteLambda: NotRequired[bool],
```

## DeleteGroupRequestTypeDef

```python
# DeleteGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DeleteGroupRequestTypeDef


def get_value() -> DeleteGroupRequestTypeDef:
    return {
        "GroupIdentifier": ...,
    }


# DeleteGroupRequestTypeDef definition

class DeleteGroupRequestTypeDef(TypedDict):
    GroupIdentifier: str,
```

## DescribeCanariesLastRunRequestTypeDef

```python
# DescribeCanariesLastRunRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DescribeCanariesLastRunRequestTypeDef


def get_value() -> DescribeCanariesLastRunRequestTypeDef:
    return {
        "NextToken": ...,
    }


# DescribeCanariesLastRunRequestTypeDef definition

class DescribeCanariesLastRunRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Names: NotRequired[Sequence[str]],
```

## DescribeCanariesRequestTypeDef

```python
# DescribeCanariesRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DescribeCanariesRequestTypeDef


def get_value() -> DescribeCanariesRequestTypeDef:
    return {
        "NextToken": ...,
    }


# DescribeCanariesRequestTypeDef definition

class DescribeCanariesRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    Names: NotRequired[Sequence[str]],
```

## DescribeRuntimeVersionsRequestTypeDef

```python
# DescribeRuntimeVersionsRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DescribeRuntimeVersionsRequestTypeDef


def get_value() -> DescribeRuntimeVersionsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# DescribeRuntimeVersionsRequestTypeDef definition

class DescribeRuntimeVersionsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## RuntimeVersionTypeDef

```python
# RuntimeVersionTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import RuntimeVersionTypeDef


def get_value() -> RuntimeVersionTypeDef:
    return {
        "VersionName": ...,
    }


# RuntimeVersionTypeDef definition

class RuntimeVersionTypeDef(TypedDict):
    VersionName: NotRequired[str],
    Description: NotRequired[str],
    ReleaseDate: NotRequired[datetime],
    DeprecationDate: NotRequired[datetime],
```

## DisassociateResourceRequestTypeDef

```python
# DisassociateResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DisassociateResourceRequestTypeDef


def get_value() -> DisassociateResourceRequestTypeDef:
    return {
        "GroupIdentifier": ...,
    }


# DisassociateResourceRequestTypeDef definition

class DisassociateResourceRequestTypeDef(TypedDict):
    GroupIdentifier: str,
    ResourceArn: str,
```

## GetCanaryRequestTypeDef

```python
# GetCanaryRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import GetCanaryRequestTypeDef


def get_value() -> GetCanaryRequestTypeDef:
    return {
        "Name": ...,
    }


# GetCanaryRequestTypeDef definition

class GetCanaryRequestTypeDef(TypedDict):
    Name: str,
```

## GetCanaryRunsRequestTypeDef

```python
# GetCanaryRunsRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import GetCanaryRunsRequestTypeDef


def get_value() -> GetCanaryRunsRequestTypeDef:
    return {
        "Name": ...,
    }


# GetCanaryRunsRequestTypeDef definition

class GetCanaryRunsRequestTypeDef(TypedDict):
    Name: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetGroupRequestTypeDef

```python
# GetGroupRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import GetGroupRequestTypeDef


def get_value() -> GetGroupRequestTypeDef:
    return {
        "GroupIdentifier": ...,
    }


# GetGroupRequestTypeDef definition

class GetGroupRequestTypeDef(TypedDict):
    GroupIdentifier: str,
```

## GroupSummaryTypeDef

```python
# GroupSummaryTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import GroupSummaryTypeDef


def get_value() -> GroupSummaryTypeDef:
    return {
        "Id": ...,
    }


# GroupSummaryTypeDef definition

class GroupSummaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Arn: NotRequired[str],
```

## ListAssociatedGroupsRequestTypeDef

```python
# ListAssociatedGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ListAssociatedGroupsRequestTypeDef


def get_value() -> ListAssociatedGroupsRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListAssociatedGroupsRequestTypeDef definition

class ListAssociatedGroupsRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListGroupResourcesRequestTypeDef

```python
# ListGroupResourcesRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ListGroupResourcesRequestTypeDef


def get_value() -> ListGroupResourcesRequestTypeDef:
    return {
        "GroupIdentifier": ...,
    }


# ListGroupResourcesRequestTypeDef definition

class ListGroupResourcesRequestTypeDef(TypedDict):
    GroupIdentifier: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListGroupsRequestTypeDef

```python
# ListGroupsRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ListGroupsRequestTypeDef


def get_value() -> ListGroupsRequestTypeDef:
    return {
        "NextToken": ...,
    }


# ListGroupsRequestTypeDef definition

class ListGroupsRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## StartCanaryRequestTypeDef

```python
# StartCanaryRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import StartCanaryRequestTypeDef


def get_value() -> StartCanaryRequestTypeDef:
    return {
        "Name": ...,
    }


# StartCanaryRequestTypeDef definition

class StartCanaryRequestTypeDef(TypedDict):
    Name: str,
```

## StopCanaryRequestTypeDef

```python
# StopCanaryRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import StopCanaryRequestTypeDef


def get_value() -> StopCanaryRequestTypeDef:
    return {
        "Name": ...,
    }


# StopCanaryRequestTypeDef definition

class StopCanaryRequestTypeDef(TypedDict):
    Name: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "ResourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## ArtifactConfigInputTypeDef

```python
# ArtifactConfigInputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ArtifactConfigInputTypeDef


def get_value() -> ArtifactConfigInputTypeDef:
    return {
        "S3Encryption": ...,
    }


# ArtifactConfigInputTypeDef definition

class ArtifactConfigInputTypeDef(TypedDict):
    S3Encryption: NotRequired[S3EncryptionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: S3EncryptionConfigTypeDef](./type_defs.md#s3encryptionconfigtypedef) 
## ArtifactConfigOutputTypeDef

```python
# ArtifactConfigOutputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ArtifactConfigOutputTypeDef


def get_value() -> ArtifactConfigOutputTypeDef:
    return {
        "S3Encryption": ...,
    }


# ArtifactConfigOutputTypeDef definition

class ArtifactConfigOutputTypeDef(TypedDict):
    S3Encryption: NotRequired[S3EncryptionConfigTypeDef],  # (1)
```

1. See [:material-code-braces: S3EncryptionConfigTypeDef](./type_defs.md#s3encryptionconfigtypedef) 
## VisualReferenceOutputTypeDef

```python
# VisualReferenceOutputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import VisualReferenceOutputTypeDef


def get_value() -> VisualReferenceOutputTypeDef:
    return {
        "BaseScreenshots": ...,
    }


# VisualReferenceOutputTypeDef definition

class VisualReferenceOutputTypeDef(TypedDict):
    BaseScreenshots: NotRequired[List[BaseScreenshotOutputTypeDef]],  # (1)
    BaseCanaryRunId: NotRequired[str],
```

1. See [:material-code-braces: BaseScreenshotOutputTypeDef](./type_defs.md#basescreenshotoutputtypedef) 
## CanaryCodeInputTypeDef

```python
# CanaryCodeInputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryCodeInputTypeDef


def get_value() -> CanaryCodeInputTypeDef:
    return {
        "S3Bucket": ...,
    }


# CanaryCodeInputTypeDef definition

class CanaryCodeInputTypeDef(TypedDict):
    Handler: str,
    S3Bucket: NotRequired[str],
    S3Key: NotRequired[str],
    S3Version: NotRequired[str],
    ZipFile: NotRequired[BlobTypeDef],
```

## CanaryRunTypeDef

```python
# CanaryRunTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryRunTypeDef


def get_value() -> CanaryRunTypeDef:
    return {
        "Id": ...,
    }


# CanaryRunTypeDef definition

class CanaryRunTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Status: NotRequired[CanaryRunStatusTypeDef],  # (1)
    Timeline: NotRequired[CanaryRunTimelineTypeDef],  # (2)
    ArtifactS3Location: NotRequired[str],
```

1. See [:material-code-braces: CanaryRunStatusTypeDef](./type_defs.md#canaryrunstatustypedef) 
2. See [:material-code-braces: CanaryRunTimelineTypeDef](./type_defs.md#canaryruntimelinetypedef) 
## ListGroupResourcesResponseTypeDef

```python
# ListGroupResourcesResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ListGroupResourcesResponseTypeDef


def get_value() -> ListGroupResourcesResponseTypeDef:
    return {
        "Resources": ...,
    }


# ListGroupResourcesResponseTypeDef definition

class ListGroupResourcesResponseTypeDef(TypedDict):
    Resources: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "Tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGroupResponseTypeDef

```python
# CreateGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CreateGroupResponseTypeDef


def get_value() -> CreateGroupResponseTypeDef:
    return {
        "Group": ...,
    }


# CreateGroupResponseTypeDef definition

class CreateGroupResponseTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetGroupResponseTypeDef

```python
# GetGroupResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import GetGroupResponseTypeDef


def get_value() -> GetGroupResponseTypeDef:
    return {
        "Group": ...,
    }


# GetGroupResponseTypeDef definition

class GetGroupResponseTypeDef(TypedDict):
    Group: GroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GroupTypeDef](./type_defs.md#grouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeRuntimeVersionsResponseTypeDef

```python
# DescribeRuntimeVersionsResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DescribeRuntimeVersionsResponseTypeDef


def get_value() -> DescribeRuntimeVersionsResponseTypeDef:
    return {
        "RuntimeVersions": ...,
    }


# DescribeRuntimeVersionsResponseTypeDef definition

class DescribeRuntimeVersionsResponseTypeDef(TypedDict):
    RuntimeVersions: List[RuntimeVersionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: RuntimeVersionTypeDef](./type_defs.md#runtimeversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAssociatedGroupsResponseTypeDef

```python
# ListAssociatedGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ListAssociatedGroupsResponseTypeDef


def get_value() -> ListAssociatedGroupsResponseTypeDef:
    return {
        "Groups": ...,
    }


# ListAssociatedGroupsResponseTypeDef definition

class ListAssociatedGroupsResponseTypeDef(TypedDict):
    Groups: List[GroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGroupsResponseTypeDef

```python
# ListGroupsResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import ListGroupsResponseTypeDef


def get_value() -> ListGroupsResponseTypeDef:
    return {
        "Groups": ...,
    }


# ListGroupsResponseTypeDef definition

class ListGroupsResponseTypeDef(TypedDict):
    Groups: List[GroupSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CanaryTypeDef

```python
# CanaryTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryTypeDef


def get_value() -> CanaryTypeDef:
    return {
        "Id": ...,
    }


# CanaryTypeDef definition

class CanaryTypeDef(TypedDict):
    Id: NotRequired[str],
    Name: NotRequired[str],
    Code: NotRequired[CanaryCodeOutputTypeDef],  # (1)
    ExecutionRoleArn: NotRequired[str],
    Schedule: NotRequired[CanaryScheduleOutputTypeDef],  # (2)
    RunConfig: NotRequired[CanaryRunConfigOutputTypeDef],  # (3)
    SuccessRetentionPeriodInDays: NotRequired[int],
    FailureRetentionPeriodInDays: NotRequired[int],
    Status: NotRequired[CanaryStatusTypeDef],  # (4)
    Timeline: NotRequired[CanaryTimelineTypeDef],  # (5)
    ArtifactS3Location: NotRequired[str],
    EngineArn: NotRequired[str],
    RuntimeVersion: NotRequired[str],
    VpcConfig: NotRequired[VpcConfigOutputTypeDef],  # (6)
    VisualReference: NotRequired[VisualReferenceOutputTypeDef],  # (7)
    ProvisionedResourceCleanup: NotRequired[ProvisionedResourceCleanupSettingType],  # (8)
    Tags: NotRequired[Dict[str, str]],
    ArtifactConfig: NotRequired[ArtifactConfigOutputTypeDef],  # (9)
```

1. See [:material-code-braces: CanaryCodeOutputTypeDef](./type_defs.md#canarycodeoutputtypedef) 
2. See [:material-code-braces: CanaryScheduleOutputTypeDef](./type_defs.md#canaryscheduleoutputtypedef) 
3. See [:material-code-braces: CanaryRunConfigOutputTypeDef](./type_defs.md#canaryrunconfigoutputtypedef) 
4. See [:material-code-braces: CanaryStatusTypeDef](./type_defs.md#canarystatustypedef) 
5. See [:material-code-braces: CanaryTimelineTypeDef](./type_defs.md#canarytimelinetypedef) 
6. See [:material-code-braces: VpcConfigOutputTypeDef](./type_defs.md#vpcconfigoutputtypedef) 
7. See [:material-code-braces: VisualReferenceOutputTypeDef](./type_defs.md#visualreferenceoutputtypedef) 
8. See [:material-code-brackets: ProvisionedResourceCleanupSettingType](./literals.md#provisionedresourcecleanupsettingtype) 
9. See [:material-code-braces: ArtifactConfigOutputTypeDef](./type_defs.md#artifactconfigoutputtypedef) 
## VisualReferenceInputTypeDef

```python
# VisualReferenceInputTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import VisualReferenceInputTypeDef


def get_value() -> VisualReferenceInputTypeDef:
    return {
        "BaseScreenshots": ...,
    }


# VisualReferenceInputTypeDef definition

class VisualReferenceInputTypeDef(TypedDict):
    BaseCanaryRunId: str,
    BaseScreenshots: NotRequired[Sequence[BaseScreenshotUnionTypeDef]],  # (1)
```

1. See [:material-code-braces: BaseScreenshotTypeDef](./type_defs.md#basescreenshottypedef) [:material-code-braces: BaseScreenshotOutputTypeDef](./type_defs.md#basescreenshotoutputtypedef) 
## CreateCanaryRequestTypeDef

```python
# CreateCanaryRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CreateCanaryRequestTypeDef


def get_value() -> CreateCanaryRequestTypeDef:
    return {
        "Name": ...,
    }


# CreateCanaryRequestTypeDef definition

class CreateCanaryRequestTypeDef(TypedDict):
    Name: str,
    Code: CanaryCodeInputTypeDef,  # (1)
    ArtifactS3Location: str,
    ExecutionRoleArn: str,
    Schedule: CanaryScheduleInputTypeDef,  # (2)
    RuntimeVersion: str,
    RunConfig: NotRequired[CanaryRunConfigInputTypeDef],  # (3)
    SuccessRetentionPeriodInDays: NotRequired[int],
    FailureRetentionPeriodInDays: NotRequired[int],
    VpcConfig: NotRequired[VpcConfigInputTypeDef],  # (4)
    ResourcesToReplicateTags: NotRequired[Sequence[ResourceToTagType]],  # (5)
    ProvisionedResourceCleanup: NotRequired[ProvisionedResourceCleanupSettingType],  # (6)
    Tags: NotRequired[Mapping[str, str]],
    ArtifactConfig: NotRequired[ArtifactConfigInputTypeDef],  # (7)
```

1. See [:material-code-braces: CanaryCodeInputTypeDef](./type_defs.md#canarycodeinputtypedef) 
2. See [:material-code-braces: CanaryScheduleInputTypeDef](./type_defs.md#canaryscheduleinputtypedef) 
3. See [:material-code-braces: CanaryRunConfigInputTypeDef](./type_defs.md#canaryrunconfiginputtypedef) 
4. See [:material-code-braces: VpcConfigInputTypeDef](./type_defs.md#vpcconfiginputtypedef) 
5. See [:material-code-brackets: ResourceToTagType](./literals.md#resourcetotagtype) 
6. See [:material-code-brackets: ProvisionedResourceCleanupSettingType](./literals.md#provisionedresourcecleanupsettingtype) 
7. See [:material-code-braces: ArtifactConfigInputTypeDef](./type_defs.md#artifactconfiginputtypedef) 
## CanaryLastRunTypeDef

```python
# CanaryLastRunTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CanaryLastRunTypeDef


def get_value() -> CanaryLastRunTypeDef:
    return {
        "CanaryName": ...,
    }


# CanaryLastRunTypeDef definition

class CanaryLastRunTypeDef(TypedDict):
    CanaryName: NotRequired[str],
    LastRun: NotRequired[CanaryRunTypeDef],  # (1)
```

1. See [:material-code-braces: CanaryRunTypeDef](./type_defs.md#canaryruntypedef) 
## GetCanaryRunsResponseTypeDef

```python
# GetCanaryRunsResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import GetCanaryRunsResponseTypeDef


def get_value() -> GetCanaryRunsResponseTypeDef:
    return {
        "CanaryRuns": ...,
    }


# GetCanaryRunsResponseTypeDef definition

class GetCanaryRunsResponseTypeDef(TypedDict):
    CanaryRuns: List[CanaryRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CanaryRunTypeDef](./type_defs.md#canaryruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateCanaryResponseTypeDef

```python
# CreateCanaryResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import CreateCanaryResponseTypeDef


def get_value() -> CreateCanaryResponseTypeDef:
    return {
        "Canary": ...,
    }


# CreateCanaryResponseTypeDef definition

class CreateCanaryResponseTypeDef(TypedDict):
    Canary: CanaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CanaryTypeDef](./type_defs.md#canarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeCanariesResponseTypeDef

```python
# DescribeCanariesResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DescribeCanariesResponseTypeDef


def get_value() -> DescribeCanariesResponseTypeDef:
    return {
        "Canaries": ...,
    }


# DescribeCanariesResponseTypeDef definition

class DescribeCanariesResponseTypeDef(TypedDict):
    Canaries: List[CanaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CanaryTypeDef](./type_defs.md#canarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetCanaryResponseTypeDef

```python
# GetCanaryResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import GetCanaryResponseTypeDef


def get_value() -> GetCanaryResponseTypeDef:
    return {
        "Canary": ...,
    }


# GetCanaryResponseTypeDef definition

class GetCanaryResponseTypeDef(TypedDict):
    Canary: CanaryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: CanaryTypeDef](./type_defs.md#canarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateCanaryRequestTypeDef

```python
# UpdateCanaryRequestTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import UpdateCanaryRequestTypeDef


def get_value() -> UpdateCanaryRequestTypeDef:
    return {
        "Name": ...,
    }


# UpdateCanaryRequestTypeDef definition

class UpdateCanaryRequestTypeDef(TypedDict):
    Name: str,
    Code: NotRequired[CanaryCodeInputTypeDef],  # (1)
    ExecutionRoleArn: NotRequired[str],
    RuntimeVersion: NotRequired[str],
    Schedule: NotRequired[CanaryScheduleInputTypeDef],  # (2)
    RunConfig: NotRequired[CanaryRunConfigInputTypeDef],  # (3)
    SuccessRetentionPeriodInDays: NotRequired[int],
    FailureRetentionPeriodInDays: NotRequired[int],
    VpcConfig: NotRequired[VpcConfigInputTypeDef],  # (4)
    VisualReference: NotRequired[VisualReferenceInputTypeDef],  # (5)
    ArtifactS3Location: NotRequired[str],
    ArtifactConfig: NotRequired[ArtifactConfigInputTypeDef],  # (6)
    ProvisionedResourceCleanup: NotRequired[ProvisionedResourceCleanupSettingType],  # (7)
```

1. See [:material-code-braces: CanaryCodeInputTypeDef](./type_defs.md#canarycodeinputtypedef) 
2. See [:material-code-braces: CanaryScheduleInputTypeDef](./type_defs.md#canaryscheduleinputtypedef) 
3. See [:material-code-braces: CanaryRunConfigInputTypeDef](./type_defs.md#canaryrunconfiginputtypedef) 
4. See [:material-code-braces: VpcConfigInputTypeDef](./type_defs.md#vpcconfiginputtypedef) 
5. See [:material-code-braces: VisualReferenceInputTypeDef](./type_defs.md#visualreferenceinputtypedef) 
6. See [:material-code-braces: ArtifactConfigInputTypeDef](./type_defs.md#artifactconfiginputtypedef) 
7. See [:material-code-brackets: ProvisionedResourceCleanupSettingType](./literals.md#provisionedresourcecleanupsettingtype) 
## DescribeCanariesLastRunResponseTypeDef

```python
# DescribeCanariesLastRunResponseTypeDef TypedDict usage example

from types_aiobotocore_synthetics.type_defs import DescribeCanariesLastRunResponseTypeDef


def get_value() -> DescribeCanariesLastRunResponseTypeDef:
    return {
        "CanariesLastRun": ...,
    }


# DescribeCanariesLastRunResponseTypeDef definition

class DescribeCanariesLastRunResponseTypeDef(TypedDict):
    CanariesLastRun: List[CanaryLastRunTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: CanaryLastRunTypeDef](./type_defs.md#canarylastruntypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

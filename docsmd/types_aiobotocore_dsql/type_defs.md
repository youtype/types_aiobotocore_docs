# Type definitions

> [Index](../README.md) > [AuroraDSQL](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [AuroraDSQL](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dsql.html#auroradsql)
    type annotations stubs module [types-aiobotocore-dsql](https://pypi.org/project/types-aiobotocore-dsql/).

## MultiRegionPropertiesUnionTypeDef

```python
# MultiRegionPropertiesUnionTypeDef Union usage example

from types_aiobotocore_dsql.type_defs import MultiRegionPropertiesUnionTypeDef


def get_value() -> MultiRegionPropertiesUnionTypeDef:
    return ...


# MultiRegionPropertiesUnionTypeDef definition

MultiRegionPropertiesUnionTypeDef = Union[
    MultiRegionPropertiesTypeDef,  # (1)
    MultiRegionPropertiesOutputTypeDef,  # (2)
]
```

1. See [:material-code-braces: MultiRegionPropertiesTypeDef](./type_defs.md#multiregionpropertiestypedef)
2. See [:material-code-braces: MultiRegionPropertiesOutputTypeDef](./type_defs.md#multiregionpropertiesoutputtypedef)



## ClusterSummaryTypeDef

```python
# ClusterSummaryTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ClusterSummaryTypeDef


def get_value() -> ClusterSummaryTypeDef:
    return {
        "identifier": ...,
    }


# ClusterSummaryTypeDef definition

class ClusterSummaryTypeDef(TypedDict):
    identifier: str,
    arn: str,
```


## EncryptionDetailsTypeDef

```python
# EncryptionDetailsTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import EncryptionDetailsTypeDef


def get_value() -> EncryptionDetailsTypeDef:
    return {
        "encryptionType": ...,
    }


# EncryptionDetailsTypeDef definition

class EncryptionDetailsTypeDef(TypedDict):
    encryptionType: EncryptionTypeType,  # (1)
    encryptionStatus: EncryptionStatusType,  # (2)
    kmsKeyArn: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionTypeType](./literals.md#encryptiontypetype)
2. See [:material-code-brackets: EncryptionStatusType](./literals.md#encryptionstatustype)

## MultiRegionPropertiesOutputTypeDef

```python
# MultiRegionPropertiesOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import MultiRegionPropertiesOutputTypeDef


def get_value() -> MultiRegionPropertiesOutputTypeDef:
    return {
        "witnessRegion": ...,
    }


# MultiRegionPropertiesOutputTypeDef definition

class MultiRegionPropertiesOutputTypeDef(TypedDict):
    witnessRegion: NotRequired[str],
    clusters: NotRequired[list[str]],
```


## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ResponseMetadataTypeDef


def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
    }


# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```


## DeleteClusterInputTypeDef

```python
# DeleteClusterInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import DeleteClusterInputTypeDef


def get_value() -> DeleteClusterInputTypeDef:
    return {
        "identifier": ...,
    }


# DeleteClusterInputTypeDef definition

class DeleteClusterInputTypeDef(TypedDict):
    identifier: str,
    clientToken: NotRequired[str],
```


## DeleteClusterPolicyInputTypeDef

```python
# DeleteClusterPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import DeleteClusterPolicyInputTypeDef


def get_value() -> DeleteClusterPolicyInputTypeDef:
    return {
        "identifier": ...,
    }


# DeleteClusterPolicyInputTypeDef definition

class DeleteClusterPolicyInputTypeDef(TypedDict):
    identifier: str,
    expectedPolicyVersion: NotRequired[str],
    clientToken: NotRequired[str],
```


## GetClusterInputTypeDef

```python
# GetClusterInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterInputTypeDef


def get_value() -> GetClusterInputTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterInputTypeDef definition

class GetClusterInputTypeDef(TypedDict):
    identifier: str,
```


## WaiterConfigTypeDef

```python
# WaiterConfigTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import WaiterConfigTypeDef


def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }


# WaiterConfigTypeDef definition

class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```


## GetClusterPolicyInputTypeDef

```python
# GetClusterPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterPolicyInputTypeDef


def get_value() -> GetClusterPolicyInputTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterPolicyInputTypeDef definition

class GetClusterPolicyInputTypeDef(TypedDict):
    identifier: str,
```


## GetVpcEndpointServiceNameInputTypeDef

```python
# GetVpcEndpointServiceNameInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetVpcEndpointServiceNameInputTypeDef


def get_value() -> GetVpcEndpointServiceNameInputTypeDef:
    return {
        "identifier": ...,
    }


# GetVpcEndpointServiceNameInputTypeDef definition

class GetVpcEndpointServiceNameInputTypeDef(TypedDict):
    identifier: str,
```


## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import PaginatorConfigTypeDef


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


## ListClustersInputTypeDef

```python
# ListClustersInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListClustersInputTypeDef


def get_value() -> ListClustersInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListClustersInputTypeDef definition

class ListClustersInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```


## ListTagsForResourceInputTypeDef

```python
# ListTagsForResourceInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListTagsForResourceInputTypeDef


def get_value() -> ListTagsForResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceInputTypeDef definition

class ListTagsForResourceInputTypeDef(TypedDict):
    resourceArn: str,
```


## MultiRegionPropertiesTypeDef

```python
# MultiRegionPropertiesTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import MultiRegionPropertiesTypeDef


def get_value() -> MultiRegionPropertiesTypeDef:
    return {
        "witnessRegion": ...,
    }


# MultiRegionPropertiesTypeDef definition

class MultiRegionPropertiesTypeDef(TypedDict):
    witnessRegion: NotRequired[str],
    clusters: NotRequired[Sequence[str]],
```


## PutClusterPolicyInputTypeDef

```python
# PutClusterPolicyInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import PutClusterPolicyInputTypeDef


def get_value() -> PutClusterPolicyInputTypeDef:
    return {
        "identifier": ...,
    }


# PutClusterPolicyInputTypeDef definition

class PutClusterPolicyInputTypeDef(TypedDict):
    identifier: str,
    policy: str,
    bypassPolicyLockoutSafetyCheck: NotRequired[bool],
    expectedPolicyVersion: NotRequired[str],
    clientToken: NotRequired[str],
```


## TagResourceInputTypeDef

```python
# TagResourceInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import TagResourceInputTypeDef


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

from types_aiobotocore_dsql.type_defs import UntagResourceInputTypeDef


def get_value() -> UntagResourceInputTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceInputTypeDef definition

class UntagResourceInputTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```


## CreateClusterOutputTypeDef

```python
# CreateClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import CreateClusterOutputTypeDef


def get_value() -> CreateClusterOutputTypeDef:
    return {
        "identifier": ...,
    }


# CreateClusterOutputTypeDef definition

class CreateClusterOutputTypeDef(TypedDict):
    identifier: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    creationTime: datetime.datetime,
    multiRegionProperties: MultiRegionPropertiesOutputTypeDef,  # (2)
    encryptionDetails: EncryptionDetailsTypeDef,  # (3)
    deletionProtectionEnabled: bool,
    endpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype)
2. See [:material-code-braces: MultiRegionPropertiesOutputTypeDef](./type_defs.md#multiregionpropertiesoutputtypedef)
3. See [:material-code-braces: EncryptionDetailsTypeDef](./type_defs.md#encryptiondetailstypedef)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteClusterOutputTypeDef

```python
# DeleteClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import DeleteClusterOutputTypeDef


def get_value() -> DeleteClusterOutputTypeDef:
    return {
        "identifier": ...,
    }


# DeleteClusterOutputTypeDef definition

class DeleteClusterOutputTypeDef(TypedDict):
    identifier: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    creationTime: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## DeleteClusterPolicyOutputTypeDef

```python
# DeleteClusterPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import DeleteClusterPolicyOutputTypeDef


def get_value() -> DeleteClusterPolicyOutputTypeDef:
    return {
        "policyVersion": ...,
    }


# DeleteClusterPolicyOutputTypeDef definition

class DeleteClusterPolicyOutputTypeDef(TypedDict):
    policyVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetClusterOutputTypeDef

```python
# GetClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterOutputTypeDef


def get_value() -> GetClusterOutputTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterOutputTypeDef definition

class GetClusterOutputTypeDef(TypedDict):
    identifier: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    creationTime: datetime.datetime,
    deletionProtectionEnabled: bool,
    multiRegionProperties: MultiRegionPropertiesOutputTypeDef,  # (2)
    tags: dict[str, str],
    encryptionDetails: EncryptionDetailsTypeDef,  # (3)
    endpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype)
2. See [:material-code-braces: MultiRegionPropertiesOutputTypeDef](./type_defs.md#multiregionpropertiesoutputtypedef)
3. See [:material-code-braces: EncryptionDetailsTypeDef](./type_defs.md#encryptiondetailstypedef)
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetClusterPolicyOutputTypeDef

```python
# GetClusterPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterPolicyOutputTypeDef


def get_value() -> GetClusterPolicyOutputTypeDef:
    return {
        "policy": ...,
    }


# GetClusterPolicyOutputTypeDef definition

class GetClusterPolicyOutputTypeDef(TypedDict):
    policy: str,
    policyVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetVpcEndpointServiceNameOutputTypeDef

```python
# GetVpcEndpointServiceNameOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetVpcEndpointServiceNameOutputTypeDef


def get_value() -> GetVpcEndpointServiceNameOutputTypeDef:
    return {
        "serviceName": ...,
    }


# GetVpcEndpointServiceNameOutputTypeDef definition

class GetVpcEndpointServiceNameOutputTypeDef(TypedDict):
    serviceName: str,
    clusterVpcEndpoint: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListClustersOutputTypeDef

```python
# ListClustersOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListClustersOutputTypeDef


def get_value() -> ListClustersOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListClustersOutputTypeDef definition

class ListClustersOutputTypeDef(TypedDict):
    clusters: list[ClusterSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See `list[ClusterSummaryTypeDef]`
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListTagsForResourceOutputTypeDef


def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    tags: dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## PutClusterPolicyOutputTypeDef

```python
# PutClusterPolicyOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import PutClusterPolicyOutputTypeDef


def get_value() -> PutClusterPolicyOutputTypeDef:
    return {
        "policyVersion": ...,
    }


# PutClusterPolicyOutputTypeDef definition

class PutClusterPolicyOutputTypeDef(TypedDict):
    policyVersion: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## UpdateClusterOutputTypeDef

```python
# UpdateClusterOutputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import UpdateClusterOutputTypeDef


def get_value() -> UpdateClusterOutputTypeDef:
    return {
        "identifier": ...,
    }


# UpdateClusterOutputTypeDef definition

class UpdateClusterOutputTypeDef(TypedDict):
    identifier: str,
    arn: str,
    status: ClusterStatusType,  # (1)
    creationTime: datetime.datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ClusterStatusType](./literals.md#clusterstatustype)
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

## GetClusterInputWaitExtraTypeDef

```python
# GetClusterInputWaitExtraTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterInputWaitExtraTypeDef


def get_value() -> GetClusterInputWaitExtraTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterInputWaitExtraTypeDef definition

class GetClusterInputWaitExtraTypeDef(TypedDict):
    identifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## GetClusterInputWaitTypeDef

```python
# GetClusterInputWaitTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import GetClusterInputWaitTypeDef


def get_value() -> GetClusterInputWaitTypeDef:
    return {
        "identifier": ...,
    }


# GetClusterInputWaitTypeDef definition

class GetClusterInputWaitTypeDef(TypedDict):
    identifier: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

## ListClustersInputPaginateTypeDef

```python
# ListClustersInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import ListClustersInputPaginateTypeDef


def get_value() -> ListClustersInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListClustersInputPaginateTypeDef definition

class ListClustersInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

## CreateClusterInputTypeDef

```python
# CreateClusterInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import CreateClusterInputTypeDef


def get_value() -> CreateClusterInputTypeDef:
    return {
        "deletionProtectionEnabled": ...,
    }


# CreateClusterInputTypeDef definition

class CreateClusterInputTypeDef(TypedDict):
    deletionProtectionEnabled: NotRequired[bool],
    kmsEncryptionKey: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    clientToken: NotRequired[str],
    multiRegionProperties: NotRequired[MultiRegionPropertiesUnionTypeDef],  # (1)
    policy: NotRequired[str],
    bypassPolicyLockoutSafetyCheck: NotRequired[bool],
```

1. See [:material-code-braces: MultiRegionPropertiesUnionTypeDef](#multiregionpropertiesuniontypedef)

## UpdateClusterInputTypeDef

```python
# UpdateClusterInputTypeDef TypedDict usage example

from types_aiobotocore_dsql.type_defs import UpdateClusterInputTypeDef


def get_value() -> UpdateClusterInputTypeDef:
    return {
        "identifier": ...,
    }


# UpdateClusterInputTypeDef definition

class UpdateClusterInputTypeDef(TypedDict):
    identifier: str,
    deletionProtectionEnabled: NotRequired[bool],
    kmsEncryptionKey: NotRequired[str],
    clientToken: NotRequired[str],
    multiRegionProperties: NotRequired[MultiRegionPropertiesUnionTypeDef],  # (1)
```

1. See [:material-code-braces: MultiRegionPropertiesUnionTypeDef](#multiregionpropertiesuniontypedef)


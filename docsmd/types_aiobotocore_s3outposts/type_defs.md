# Type definitions

> [Index](../README.md) > [S3Outposts](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [S3Outposts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3outposts.html#s3outposts)
    type annotations stubs module [types-aiobotocore-s3outposts](https://pypi.org/project/types-aiobotocore-s3outposts/).



## CreateEndpointRequestRequestTypeDef

```python
# CreateEndpointRequestRequestTypeDef definition

class CreateEndpointRequestRequestTypeDef(TypedDict):
    OutpostId: str,
    SubnetId: str,
    SecurityGroupId: str,
    AccessType: NotRequired[EndpointAccessTypeType],  # (1)
    CustomerOwnedIpv4Pool: NotRequired[str],
```

1. See [:material-code-brackets: EndpointAccessTypeType](./literals.md#endpointaccesstypetype) 
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

## DeleteEndpointRequestRequestTypeDef

```python
# DeleteEndpointRequestRequestTypeDef definition

class DeleteEndpointRequestRequestTypeDef(TypedDict):
    EndpointId: str,
    OutpostId: str,
```

## FailedReasonTypeDef

```python
# FailedReasonTypeDef definition

class FailedReasonTypeDef(TypedDict):
    ErrorCode: NotRequired[str],
    Message: NotRequired[str],
```

## NetworkInterfaceTypeDef

```python
# NetworkInterfaceTypeDef definition

class NetworkInterfaceTypeDef(TypedDict):
    NetworkInterfaceId: NotRequired[str],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEndpointsRequestRequestTypeDef

```python
# ListEndpointsRequestRequestTypeDef definition

class ListEndpointsRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListOutpostsWithS3RequestRequestTypeDef

```python
# ListOutpostsWithS3RequestRequestTypeDef definition

class ListOutpostsWithS3RequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## OutpostTypeDef

```python
# OutpostTypeDef definition

class OutpostTypeDef(TypedDict):
    OutpostArn: NotRequired[str],
    S3OutpostArn: NotRequired[str],
    OutpostId: NotRequired[str],
    OwnerId: NotRequired[str],
    CapacityInBytes: NotRequired[int],
```

## ListSharedEndpointsRequestRequestTypeDef

```python
# ListSharedEndpointsRequestRequestTypeDef definition

class ListSharedEndpointsRequestRequestTypeDef(TypedDict):
    OutpostId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## CreateEndpointResultTypeDef

```python
# CreateEndpointResultTypeDef definition

class CreateEndpointResultTypeDef(TypedDict):
    EndpointArn: str,
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
## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    EndpointArn: NotRequired[str],
    OutpostsId: NotRequired[str],
    CidrBlock: NotRequired[str],
    Status: NotRequired[EndpointStatusType],  # (1)
    CreationTime: NotRequired[datetime],
    NetworkInterfaces: NotRequired[List[NetworkInterfaceTypeDef]],  # (2)
    VpcId: NotRequired[str],
    SubnetId: NotRequired[str],
    SecurityGroupId: NotRequired[str],
    AccessType: NotRequired[EndpointAccessTypeType],  # (3)
    CustomerOwnedIpv4Pool: NotRequired[str],
    FailedReason: NotRequired[FailedReasonTypeDef],  # (4)
```

1. See [:material-code-brackets: EndpointStatusType](./literals.md#endpointstatustype) 
2. See [:material-code-braces: NetworkInterfaceTypeDef](./type_defs.md#networkinterfacetypedef) 
3. See [:material-code-brackets: EndpointAccessTypeType](./literals.md#endpointaccesstypetype) 
4. See [:material-code-braces: FailedReasonTypeDef](./type_defs.md#failedreasontypedef) 
## ListEndpointsRequestPaginateTypeDef

```python
# ListEndpointsRequestPaginateTypeDef definition

class ListEndpointsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOutpostsWithS3RequestPaginateTypeDef

```python
# ListOutpostsWithS3RequestPaginateTypeDef definition

class ListOutpostsWithS3RequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSharedEndpointsRequestPaginateTypeDef

```python
# ListSharedEndpointsRequestPaginateTypeDef definition

class ListSharedEndpointsRequestPaginateTypeDef(TypedDict):
    OutpostId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOutpostsWithS3ResultTypeDef

```python
# ListOutpostsWithS3ResultTypeDef definition

class ListOutpostsWithS3ResultTypeDef(TypedDict):
    Outposts: List[OutpostTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: OutpostTypeDef](./type_defs.md#outposttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEndpointsResultTypeDef

```python
# ListEndpointsResultTypeDef definition

class ListEndpointsResultTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSharedEndpointsResultTypeDef

```python
# ListSharedEndpointsResultTypeDef definition

class ListSharedEndpointsResultTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

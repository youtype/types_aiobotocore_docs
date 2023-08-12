# Type definitions

> [Index](../README.md) > [CloudWatchObservabilityAccessManager](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudWatchObservabilityAccessManager](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
    type annotations stubs module [types-aiobotocore-oam](https://pypi.org/project/types-aiobotocore-oam/).



## CreateLinkInputRequestTypeDef

```python
# CreateLinkInputRequestTypeDef definition

class CreateLinkInputRequestTypeDef(TypedDict):
    LabelTemplate: str,
    ResourceTypes: Sequence[ResourceTypeType],  # (1)
    SinkIdentifier: str,
    Tags: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## CreateSinkInputRequestTypeDef

```python
# CreateSinkInputRequestTypeDef definition

class CreateSinkInputRequestTypeDef(TypedDict):
    Name: str,
    Tags: NotRequired[Mapping[str, str]],
```

## DeleteLinkInputRequestTypeDef

```python
# DeleteLinkInputRequestTypeDef definition

class DeleteLinkInputRequestTypeDef(TypedDict):
    Identifier: str,
```

## DeleteSinkInputRequestTypeDef

```python
# DeleteSinkInputRequestTypeDef definition

class DeleteSinkInputRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetLinkInputRequestTypeDef

```python
# GetLinkInputRequestTypeDef definition

class GetLinkInputRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetSinkInputRequestTypeDef

```python
# GetSinkInputRequestTypeDef definition

class GetSinkInputRequestTypeDef(TypedDict):
    Identifier: str,
```

## GetSinkPolicyInputRequestTypeDef

```python
# GetSinkPolicyInputRequestTypeDef definition

class GetSinkPolicyInputRequestTypeDef(TypedDict):
    SinkIdentifier: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListAttachedLinksInputRequestTypeDef

```python
# ListAttachedLinksInputRequestTypeDef definition

class ListAttachedLinksInputRequestTypeDef(TypedDict):
    SinkIdentifier: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListAttachedLinksItemTypeDef

```python
# ListAttachedLinksItemTypeDef definition

class ListAttachedLinksItemTypeDef(TypedDict):
    Label: NotRequired[str],
    LinkArn: NotRequired[str],
    ResourceTypes: NotRequired[List[str]],
```

## ListLinksInputRequestTypeDef

```python
# ListLinksInputRequestTypeDef definition

class ListLinksInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListLinksItemTypeDef

```python
# ListLinksItemTypeDef definition

class ListLinksItemTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Label: NotRequired[str],
    ResourceTypes: NotRequired[List[str]],
    SinkArn: NotRequired[str],
```

## ListSinksInputRequestTypeDef

```python
# ListSinksInputRequestTypeDef definition

class ListSinksInputRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListSinksItemTypeDef

```python
# ListSinksItemTypeDef definition

class ListSinksItemTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
```

## ListTagsForResourceInputRequestTypeDef

```python
# ListTagsForResourceInputRequestTypeDef definition

class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## PutSinkPolicyInputRequestTypeDef

```python
# PutSinkPolicyInputRequestTypeDef definition

class PutSinkPolicyInputRequestTypeDef(TypedDict):
    SinkIdentifier: str,
    Policy: str,
```

## TagResourceInputRequestTypeDef

```python
# TagResourceInputRequestTypeDef definition

class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceInputRequestTypeDef

```python
# UntagResourceInputRequestTypeDef definition

class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateLinkInputRequestTypeDef

```python
# UpdateLinkInputRequestTypeDef definition

class UpdateLinkInputRequestTypeDef(TypedDict):
    Identifier: str,
    ResourceTypes: Sequence[ResourceTypeType],  # (1)
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
## CreateLinkOutputTypeDef

```python
# CreateLinkOutputTypeDef definition

class CreateLinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Label: str,
    LabelTemplate: str,
    ResourceTypes: List[str],
    SinkArn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSinkOutputTypeDef

```python
# CreateSinkOutputTypeDef definition

class CreateSinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetLinkOutputTypeDef

```python
# GetLinkOutputTypeDef definition

class GetLinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Label: str,
    LabelTemplate: str,
    ResourceTypes: List[str],
    SinkArn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSinkOutputTypeDef

```python
# GetSinkOutputTypeDef definition

class GetSinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Name: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSinkPolicyOutputTypeDef

```python
# GetSinkPolicyOutputTypeDef definition

class GetSinkPolicyOutputTypeDef(TypedDict):
    SinkArn: str,
    SinkId: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceOutputTypeDef

```python
# ListTagsForResourceOutputTypeDef definition

class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutSinkPolicyOutputTypeDef

```python
# PutSinkPolicyOutputTypeDef definition

class PutSinkPolicyOutputTypeDef(TypedDict):
    SinkArn: str,
    SinkId: str,
    Policy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateLinkOutputTypeDef

```python
# UpdateLinkOutputTypeDef definition

class UpdateLinkOutputTypeDef(TypedDict):
    Arn: str,
    Id: str,
    Label: str,
    LabelTemplate: str,
    ResourceTypes: List[str],
    SinkArn: str,
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListAttachedLinksInputListAttachedLinksPaginateTypeDef

```python
# ListAttachedLinksInputListAttachedLinksPaginateTypeDef definition

class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(TypedDict):
    SinkIdentifier: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListLinksInputListLinksPaginateTypeDef

```python
# ListLinksInputListLinksPaginateTypeDef definition

class ListLinksInputListLinksPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSinksInputListSinksPaginateTypeDef

```python
# ListSinksInputListSinksPaginateTypeDef definition

class ListSinksInputListSinksPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListAttachedLinksOutputTypeDef

```python
# ListAttachedLinksOutputTypeDef definition

class ListAttachedLinksOutputTypeDef(TypedDict):
    Items: List[ListAttachedLinksItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListAttachedLinksItemTypeDef](./type_defs.md#listattachedlinksitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListLinksOutputTypeDef

```python
# ListLinksOutputTypeDef definition

class ListLinksOutputTypeDef(TypedDict):
    Items: List[ListLinksItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListLinksItemTypeDef](./type_defs.md#listlinksitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSinksOutputTypeDef

```python
# ListSinksOutputTypeDef definition

class ListSinksOutputTypeDef(TypedDict):
    Items: List[ListSinksItemTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ListSinksItemTypeDef](./type_defs.md#listsinksitemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

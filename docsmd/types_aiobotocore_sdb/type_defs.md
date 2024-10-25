# Type definitions

> [Index](../README.md) > [SimpleDB](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SimpleDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
    type annotations stubs module [types-aiobotocore-sdb](https://pypi.org/project/types-aiobotocore-sdb/).



## AttributeTypeDef

```python
# AttributeTypeDef definition

class AttributeTypeDef(TypedDict):
    Name: str,
    Value: str,
    AlternateNameEncoding: NotRequired[str],
    AlternateValueEncoding: NotRequired[str],
```

## CreateDomainRequestRequestTypeDef

```python
# CreateDomainRequestRequestTypeDef definition

class CreateDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## UpdateConditionTypeDef

```python
# UpdateConditionTypeDef definition

class UpdateConditionTypeDef(TypedDict):
    Name: NotRequired[str],
    Value: NotRequired[str],
    Exists: NotRequired[bool],
```

## DeleteDomainRequestRequestTypeDef

```python
# DeleteDomainRequestRequestTypeDef definition

class DeleteDomainRequestRequestTypeDef(TypedDict):
    DomainName: str,
```

## DomainMetadataRequestRequestTypeDef

```python
# DomainMetadataRequestRequestTypeDef definition

class DomainMetadataRequestRequestTypeDef(TypedDict):
    DomainName: str,
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

## GetAttributesRequestRequestTypeDef

```python
# GetAttributesRequestRequestTypeDef definition

class GetAttributesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ItemName: str,
    AttributeNames: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListDomainsRequestRequestTypeDef

```python
# ListDomainsRequestRequestTypeDef definition

class ListDomainsRequestRequestTypeDef(TypedDict):
    MaxNumberOfDomains: NotRequired[int],
    NextToken: NotRequired[str],
```

## ReplaceableAttributeTypeDef

```python
# ReplaceableAttributeTypeDef definition

class ReplaceableAttributeTypeDef(TypedDict):
    Name: str,
    Value: str,
    Replace: NotRequired[bool],
```

## SelectRequestRequestTypeDef

```python
# SelectRequestRequestTypeDef definition

class SelectRequestRequestTypeDef(TypedDict):
    SelectExpression: str,
    NextToken: NotRequired[str],
    ConsistentRead: NotRequired[bool],
```

## DeletableItemTypeDef

```python
# DeletableItemTypeDef definition

class DeletableItemTypeDef(TypedDict):
    Name: str,
    Attributes: NotRequired[Sequence[AttributeTypeDef]],  # (1)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## ItemTypeDef

```python
# ItemTypeDef definition

class ItemTypeDef(TypedDict):
    Name: str,
    Attributes: List[AttributeTypeDef],  # (1)
    AlternateNameEncoding: NotRequired[str],
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
## DeleteAttributesRequestRequestTypeDef

```python
# DeleteAttributesRequestRequestTypeDef definition

class DeleteAttributesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ItemName: str,
    Attributes: NotRequired[Sequence[AttributeTypeDef]],  # (1)
    Expected: NotRequired[UpdateConditionTypeDef],  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: UpdateConditionTypeDef](./type_defs.md#updateconditiontypedef) 
## DomainMetadataResultTypeDef

```python
# DomainMetadataResultTypeDef definition

class DomainMetadataResultTypeDef(TypedDict):
    ItemCount: int,
    ItemNamesSizeBytes: int,
    AttributeNameCount: int,
    AttributeNamesSizeBytes: int,
    AttributeValueCount: int,
    AttributeValuesSizeBytes: int,
    Timestamp: int,
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
## GetAttributesResultTypeDef

```python
# GetAttributesResultTypeDef definition

class GetAttributesResultTypeDef(TypedDict):
    Attributes: List[AttributeTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AttributeTypeDef](./type_defs.md#attributetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainsResultTypeDef

```python
# ListDomainsResultTypeDef definition

class ListDomainsResultTypeDef(TypedDict):
    DomainNames: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDomainsRequestListDomainsPaginateTypeDef

```python
# ListDomainsRequestListDomainsPaginateTypeDef definition

class ListDomainsRequestListDomainsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## SelectRequestSelectPaginateTypeDef

```python
# SelectRequestSelectPaginateTypeDef definition

class SelectRequestSelectPaginateTypeDef(TypedDict):
    SelectExpression: str,
    ConsistentRead: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## PutAttributesRequestRequestTypeDef

```python
# PutAttributesRequestRequestTypeDef definition

class PutAttributesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    ItemName: str,
    Attributes: Sequence[ReplaceableAttributeTypeDef],  # (1)
    Expected: NotRequired[UpdateConditionTypeDef],  # (2)
```

1. See [:material-code-braces: ReplaceableAttributeTypeDef](./type_defs.md#replaceableattributetypedef) 
2. See [:material-code-braces: UpdateConditionTypeDef](./type_defs.md#updateconditiontypedef) 
## ReplaceableItemTypeDef

```python
# ReplaceableItemTypeDef definition

class ReplaceableItemTypeDef(TypedDict):
    Name: str,
    Attributes: Sequence[ReplaceableAttributeTypeDef],  # (1)
```

1. See [:material-code-braces: ReplaceableAttributeTypeDef](./type_defs.md#replaceableattributetypedef) 
## BatchDeleteAttributesRequestRequestTypeDef

```python
# BatchDeleteAttributesRequestRequestTypeDef definition

class BatchDeleteAttributesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Items: Sequence[DeletableItemTypeDef],  # (1)
```

1. See [:material-code-braces: DeletableItemTypeDef](./type_defs.md#deletableitemtypedef) 
## SelectResultTypeDef

```python
# SelectResultTypeDef definition

class SelectResultTypeDef(TypedDict):
    Items: List[ItemTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ItemTypeDef](./type_defs.md#itemtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchPutAttributesRequestRequestTypeDef

```python
# BatchPutAttributesRequestRequestTypeDef definition

class BatchPutAttributesRequestRequestTypeDef(TypedDict):
    DomainName: str,
    Items: Sequence[ReplaceableItemTypeDef],  # (1)
```

1. See [:material-code-braces: ReplaceableItemTypeDef](./type_defs.md#replaceableitemtypedef) 

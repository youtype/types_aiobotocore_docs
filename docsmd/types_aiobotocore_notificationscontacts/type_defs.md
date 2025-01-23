# Type definitions

> [Index](../README.md) > [UserNotificationsContacts](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [UserNotificationsContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/notificationscontacts.html#usernotificationscontacts)
    type annotations stubs module [types-aiobotocore-notificationscontacts](https://pypi.org/project/types-aiobotocore-notificationscontacts/).



## ActivateEmailContactRequestRequestTypeDef

```python
# ActivateEmailContactRequestRequestTypeDef definition

class ActivateEmailContactRequestRequestTypeDef(TypedDict):
    arn: str,
    code: str,
```

## CreateEmailContactRequestRequestTypeDef

```python
# CreateEmailContactRequestRequestTypeDef definition

class CreateEmailContactRequestRequestTypeDef(TypedDict):
    name: str,
    emailAddress: str,
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

## DeleteEmailContactRequestRequestTypeDef

```python
# DeleteEmailContactRequestRequestTypeDef definition

class DeleteEmailContactRequestRequestTypeDef(TypedDict):
    arn: str,
```

## EmailContactTypeDef

```python
# EmailContactTypeDef definition

class EmailContactTypeDef(TypedDict):
    arn: str,
    name: str,
    address: str,
    status: EmailContactStatusType,  # (1)
    creationTime: datetime,
    updateTime: datetime,
```

1. See [:material-code-brackets: EmailContactStatusType](./literals.md#emailcontactstatustype) 
## GetEmailContactRequestRequestTypeDef

```python
# GetEmailContactRequestRequestTypeDef definition

class GetEmailContactRequestRequestTypeDef(TypedDict):
    arn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEmailContactsRequestRequestTypeDef

```python
# ListEmailContactsRequestRequestTypeDef definition

class ListEmailContactsRequestRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    arn: str,
```

## SendActivationCodeRequestRequestTypeDef

```python
# SendActivationCodeRequestRequestTypeDef definition

class SendActivationCodeRequestRequestTypeDef(TypedDict):
    arn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    arn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    arn: str,
    tagKeys: Sequence[str],
```

## CreateEmailContactResponseTypeDef

```python
# CreateEmailContactResponseTypeDef definition

class CreateEmailContactResponseTypeDef(TypedDict):
    arn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEmailContactResponseTypeDef

```python
# GetEmailContactResponseTypeDef definition

class GetEmailContactResponseTypeDef(TypedDict):
    emailContact: EmailContactTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EmailContactTypeDef](./type_defs.md#emailcontacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEmailContactsResponseTypeDef

```python
# ListEmailContactsResponseTypeDef definition

class ListEmailContactsResponseTypeDef(TypedDict):
    emailContacts: List[EmailContactTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EmailContactTypeDef](./type_defs.md#emailcontacttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEmailContactsRequestPaginateTypeDef

```python
# ListEmailContactsRequestPaginateTypeDef definition

class ListEmailContactsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 

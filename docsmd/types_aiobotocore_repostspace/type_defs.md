# Type definitions

> [Index](../README.md) > [RePostPrivate](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#repostprivate)
    type annotations stubs module [types-aiobotocore-repostspace](https://pypi.org/project/types-aiobotocore-repostspace/).



## BatchAddRoleInputTypeDef

```python
# BatchAddRoleInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import BatchAddRoleInputTypeDef


def get_value() -> BatchAddRoleInputTypeDef:
    return {
        "accessorIds": ...,
    }


# BatchAddRoleInputTypeDef definition

class BatchAddRoleInputTypeDef(TypedDict):
    accessorIds: Sequence[str],
    role: RoleType,  # (1)
    spaceId: str,
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
## BatchErrorTypeDef

```python
# BatchErrorTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import BatchErrorTypeDef


def get_value() -> BatchErrorTypeDef:
    return {
        "accessorId": ...,
    }


# BatchErrorTypeDef definition

class BatchErrorTypeDef(TypedDict):
    accessorId: str,
    error: int,
    message: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import ResponseMetadataTypeDef


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

## BatchRemoveRoleInputTypeDef

```python
# BatchRemoveRoleInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import BatchRemoveRoleInputTypeDef


def get_value() -> BatchRemoveRoleInputTypeDef:
    return {
        "accessorIds": ...,
    }


# BatchRemoveRoleInputTypeDef definition

class BatchRemoveRoleInputTypeDef(TypedDict):
    accessorIds: Sequence[str],
    role: RoleType,  # (1)
    spaceId: str,
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
## CreateSpaceInputTypeDef

```python
# CreateSpaceInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import CreateSpaceInputTypeDef


def get_value() -> CreateSpaceInputTypeDef:
    return {
        "name": ...,
    }


# CreateSpaceInputTypeDef definition

class CreateSpaceInputTypeDef(TypedDict):
    name: str,
    subdomain: str,
    tier: TierLevelType,  # (1)
    description: NotRequired[str],
    roleArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    userKMSKey: NotRequired[str],
```

1. See [:material-code-brackets: TierLevelType](./literals.md#tierleveltype) 
## DeleteSpaceInputTypeDef

```python
# DeleteSpaceInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import DeleteSpaceInputTypeDef


def get_value() -> DeleteSpaceInputTypeDef:
    return {
        "spaceId": ...,
    }


# DeleteSpaceInputTypeDef definition

class DeleteSpaceInputTypeDef(TypedDict):
    spaceId: str,
```

## DeregisterAdminInputTypeDef

```python
# DeregisterAdminInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import DeregisterAdminInputTypeDef


def get_value() -> DeregisterAdminInputTypeDef:
    return {
        "adminId": ...,
    }


# DeregisterAdminInputTypeDef definition

class DeregisterAdminInputTypeDef(TypedDict):
    adminId: str,
    spaceId: str,
```

## GetSpaceInputTypeDef

```python
# GetSpaceInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import GetSpaceInputTypeDef


def get_value() -> GetSpaceInputTypeDef:
    return {
        "spaceId": ...,
    }


# GetSpaceInputTypeDef definition

class GetSpaceInputTypeDef(TypedDict):
    spaceId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import PaginatorConfigTypeDef


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

## ListSpacesInputTypeDef

```python
# ListSpacesInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import ListSpacesInputTypeDef


def get_value() -> ListSpacesInputTypeDef:
    return {
        "maxResults": ...,
    }


# ListSpacesInputTypeDef definition

class ListSpacesInputTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SpaceDataTypeDef

```python
# SpaceDataTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import SpaceDataTypeDef


def get_value() -> SpaceDataTypeDef:
    return {
        "arn": ...,
    }


# SpaceDataTypeDef definition

class SpaceDataTypeDef(TypedDict):
    arn: str,
    configurationStatus: ConfigurationStatusType,  # (1)
    createDateTime: datetime,
    name: str,
    randomDomain: str,
    spaceId: str,
    status: str,
    storageLimit: int,
    tier: TierLevelType,  # (2)
    vanityDomain: str,
    vanityDomainStatus: VanityDomainStatusType,  # (3)
    contentSize: NotRequired[int],
    deleteDateTime: NotRequired[datetime],
    description: NotRequired[str],
    userCount: NotRequired[int],
    userKMSKey: NotRequired[str],
```

1. See [:material-code-brackets: ConfigurationStatusType](./literals.md#configurationstatustype) 
2. See [:material-code-brackets: TierLevelType](./literals.md#tierleveltype) 
3. See [:material-code-brackets: VanityDomainStatusType](./literals.md#vanitydomainstatustype) 
## ListTagsForResourceRequestTypeDef

```python
# ListTagsForResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import ListTagsForResourceRequestTypeDef


def get_value() -> ListTagsForResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# ListTagsForResourceRequestTypeDef definition

class ListTagsForResourceRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RegisterAdminInputTypeDef

```python
# RegisterAdminInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import RegisterAdminInputTypeDef


def get_value() -> RegisterAdminInputTypeDef:
    return {
        "adminId": ...,
    }


# RegisterAdminInputTypeDef definition

class RegisterAdminInputTypeDef(TypedDict):
    adminId: str,
    spaceId: str,
```

## SendInvitesInputTypeDef

```python
# SendInvitesInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import SendInvitesInputTypeDef


def get_value() -> SendInvitesInputTypeDef:
    return {
        "accessorIds": ...,
    }


# SendInvitesInputTypeDef definition

class SendInvitesInputTypeDef(TypedDict):
    accessorIds: Sequence[str],
    body: str,
    spaceId: str,
    title: str,
```

## TagResourceRequestTypeDef

```python
# TagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import TagResourceRequestTypeDef


def get_value() -> TagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# TagResourceRequestTypeDef definition

class TagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestTypeDef

```python
# UntagResourceRequestTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import UntagResourceRequestTypeDef


def get_value() -> UntagResourceRequestTypeDef:
    return {
        "resourceArn": ...,
    }


# UntagResourceRequestTypeDef definition

class UntagResourceRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateSpaceInputTypeDef

```python
# UpdateSpaceInputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import UpdateSpaceInputTypeDef


def get_value() -> UpdateSpaceInputTypeDef:
    return {
        "spaceId": ...,
    }


# UpdateSpaceInputTypeDef definition

class UpdateSpaceInputTypeDef(TypedDict):
    spaceId: str,
    description: NotRequired[str],
    roleArn: NotRequired[str],
    tier: NotRequired[TierLevelType],  # (1)
```

1. See [:material-code-brackets: TierLevelType](./literals.md#tierleveltype) 
## BatchAddRoleOutputTypeDef

```python
# BatchAddRoleOutputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import BatchAddRoleOutputTypeDef


def get_value() -> BatchAddRoleOutputTypeDef:
    return {
        "addedAccessorIds": ...,
    }


# BatchAddRoleOutputTypeDef definition

class BatchAddRoleOutputTypeDef(TypedDict):
    addedAccessorIds: List[str],
    errors: List[BatchErrorTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchErrorTypeDef](./type_defs.md#batcherrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchRemoveRoleOutputTypeDef

```python
# BatchRemoveRoleOutputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import BatchRemoveRoleOutputTypeDef


def get_value() -> BatchRemoveRoleOutputTypeDef:
    return {
        "errors": ...,
    }


# BatchRemoveRoleOutputTypeDef definition

class BatchRemoveRoleOutputTypeDef(TypedDict):
    errors: List[BatchErrorTypeDef],  # (1)
    removedAccessorIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BatchErrorTypeDef](./type_defs.md#batcherrortypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateSpaceOutputTypeDef

```python
# CreateSpaceOutputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import CreateSpaceOutputTypeDef


def get_value() -> CreateSpaceOutputTypeDef:
    return {
        "spaceId": ...,
    }


# CreateSpaceOutputTypeDef definition

class CreateSpaceOutputTypeDef(TypedDict):
    spaceId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import EmptyResponseMetadataTypeDef


def get_value() -> EmptyResponseMetadataTypeDef:
    return {
        "ResponseMetadata": ...,
    }


# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSpaceOutputTypeDef

```python
# GetSpaceOutputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import GetSpaceOutputTypeDef


def get_value() -> GetSpaceOutputTypeDef:
    return {
        "arn": ...,
    }


# GetSpaceOutputTypeDef definition

class GetSpaceOutputTypeDef(TypedDict):
    arn: str,
    clientId: str,
    configurationStatus: ConfigurationStatusType,  # (1)
    contentSize: int,
    createDateTime: datetime,
    customerRoleArn: str,
    deleteDateTime: datetime,
    description: str,
    groupAdmins: List[str],
    name: str,
    randomDomain: str,
    roles: Dict[str, List[RoleType]],  # (2)
    spaceId: str,
    status: str,
    storageLimit: int,
    tier: TierLevelType,  # (3)
    userAdmins: List[str],
    userCount: int,
    userKMSKey: str,
    vanityDomain: str,
    vanityDomainStatus: VanityDomainStatusType,  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-brackets: ConfigurationStatusType](./literals.md#configurationstatustype) 
2. See [:material-code-brackets: RoleType](./literals.md#roletype) 
3. See [:material-code-brackets: TierLevelType](./literals.md#tierleveltype) 
4. See [:material-code-brackets: VanityDomainStatusType](./literals.md#vanitydomainstatustype) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import ListTagsForResourceResponseTypeDef


def get_value() -> ListTagsForResourceResponseTypeDef:
    return {
        "tags": ...,
    }


# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSpacesInputPaginateTypeDef

```python
# ListSpacesInputPaginateTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import ListSpacesInputPaginateTypeDef


def get_value() -> ListSpacesInputPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }


# ListSpacesInputPaginateTypeDef definition

class ListSpacesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSpacesOutputTypeDef

```python
# ListSpacesOutputTypeDef TypedDict usage example

from types_aiobotocore_repostspace.type_defs import ListSpacesOutputTypeDef


def get_value() -> ListSpacesOutputTypeDef:
    return {
        "nextToken": ...,
    }


# ListSpacesOutputTypeDef definition

class ListSpacesOutputTypeDef(TypedDict):
    spaces: List[SpaceDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SpaceDataTypeDef](./type_defs.md#spacedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

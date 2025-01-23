# Type definitions

> [Index](../README.md) > [RePostPrivate](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RePostPrivate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/repostspace.html#repostprivate)
    type annotations stubs module [types-aiobotocore-repostspace](https://pypi.org/project/types-aiobotocore-repostspace/).



## BatchAddRoleInputRequestTypeDef

```python
# BatchAddRoleInputRequestTypeDef definition

class BatchAddRoleInputRequestTypeDef(TypedDict):
    accessorIds: Sequence[str],
    role: RoleType,  # (1)
    spaceId: str,
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
## BatchErrorTypeDef

```python
# BatchErrorTypeDef definition

class BatchErrorTypeDef(TypedDict):
    accessorId: str,
    error: int,
    message: str,
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

## BatchRemoveRoleInputRequestTypeDef

```python
# BatchRemoveRoleInputRequestTypeDef definition

class BatchRemoveRoleInputRequestTypeDef(TypedDict):
    accessorIds: Sequence[str],
    role: RoleType,  # (1)
    spaceId: str,
```

1. See [:material-code-brackets: RoleType](./literals.md#roletype) 
## CreateSpaceInputRequestTypeDef

```python
# CreateSpaceInputRequestTypeDef definition

class CreateSpaceInputRequestTypeDef(TypedDict):
    name: str,
    subdomain: str,
    tier: TierLevelType,  # (1)
    description: NotRequired[str],
    roleArn: NotRequired[str],
    tags: NotRequired[Mapping[str, str]],
    userKMSKey: NotRequired[str],
```

1. See [:material-code-brackets: TierLevelType](./literals.md#tierleveltype) 
## DeleteSpaceInputRequestTypeDef

```python
# DeleteSpaceInputRequestTypeDef definition

class DeleteSpaceInputRequestTypeDef(TypedDict):
    spaceId: str,
```

## DeregisterAdminInputRequestTypeDef

```python
# DeregisterAdminInputRequestTypeDef definition

class DeregisterAdminInputRequestTypeDef(TypedDict):
    adminId: str,
    spaceId: str,
```

## GetSpaceInputRequestTypeDef

```python
# GetSpaceInputRequestTypeDef definition

class GetSpaceInputRequestTypeDef(TypedDict):
    spaceId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListSpacesInputRequestTypeDef

```python
# ListSpacesInputRequestTypeDef definition

class ListSpacesInputRequestTypeDef(TypedDict):
    maxResults: NotRequired[int],
    nextToken: NotRequired[str],
```

## SpaceDataTypeDef

```python
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
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
```

## RegisterAdminInputRequestTypeDef

```python
# RegisterAdminInputRequestTypeDef definition

class RegisterAdminInputRequestTypeDef(TypedDict):
    adminId: str,
    spaceId: str,
```

## SendInvitesInputRequestTypeDef

```python
# SendInvitesInputRequestTypeDef definition

class SendInvitesInputRequestTypeDef(TypedDict):
    accessorIds: Sequence[str],
    body: str,
    spaceId: str,
    title: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    resourceArn: str,
    tagKeys: Sequence[str],
```

## UpdateSpaceInputRequestTypeDef

```python
# UpdateSpaceInputRequestTypeDef definition

class UpdateSpaceInputRequestTypeDef(TypedDict):
    spaceId: str,
    description: NotRequired[str],
    roleArn: NotRequired[str],
    tier: NotRequired[TierLevelType],  # (1)
```

1. See [:material-code-brackets: TierLevelType](./literals.md#tierleveltype) 
## BatchAddRoleOutputTypeDef

```python
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
# CreateSpaceOutputTypeDef definition

class CreateSpaceOutputTypeDef(TypedDict):
    spaceId: str,
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
## GetSpaceOutputTypeDef

```python
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
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSpacesInputPaginateTypeDef

```python
# ListSpacesInputPaginateTypeDef definition

class ListSpacesInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSpacesOutputTypeDef

```python
# ListSpacesOutputTypeDef definition

class ListSpacesOutputTypeDef(TypedDict):
    spaces: List[SpaceDataTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: SpaceDataTypeDef](./type_defs.md#spacedatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

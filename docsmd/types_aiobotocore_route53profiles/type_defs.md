# Type definitions

> [Index](../README.md) > [Route53Profiles](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Route53Profiles](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53profiles.html#Route53Profiles)
    type annotations stubs module [types-aiobotocore-route53profiles](https://pypi.org/project/types-aiobotocore-route53profiles/).



## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## ProfileAssociationTypeDef

```python
# ProfileAssociationTypeDef definition

class ProfileAssociationTypeDef(TypedDict):
    CreationTime: NotRequired[datetime],
    Id: NotRequired[str],
    ModificationTime: NotRequired[datetime],
    Name: NotRequired[str],
    OwnerId: NotRequired[str],
    ProfileId: NotRequired[str],
    ResourceId: NotRequired[str],
    Status: NotRequired[ProfileStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ProfileStatusType](./literals.md#profilestatustype) 
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

## AssociateResourceToProfileRequestRequestTypeDef

```python
# AssociateResourceToProfileRequestRequestTypeDef definition

class AssociateResourceToProfileRequestRequestTypeDef(TypedDict):
    Name: str,
    ProfileId: str,
    ResourceArn: str,
    ResourceProperties: NotRequired[str],
```

## ProfileResourceAssociationTypeDef

```python
# ProfileResourceAssociationTypeDef definition

class ProfileResourceAssociationTypeDef(TypedDict):
    CreationTime: NotRequired[datetime],
    Id: NotRequired[str],
    ModificationTime: NotRequired[datetime],
    Name: NotRequired[str],
    OwnerId: NotRequired[str],
    ProfileId: NotRequired[str],
    ResourceArn: NotRequired[str],
    ResourceProperties: NotRequired[str],
    ResourceType: NotRequired[str],
    Status: NotRequired[ProfileStatusType],  # (1)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ProfileStatusType](./literals.md#profilestatustype) 
## ProfileTypeDef

```python
# ProfileTypeDef definition

class ProfileTypeDef(TypedDict):
    Arn: NotRequired[str],
    ClientToken: NotRequired[str],
    CreationTime: NotRequired[datetime],
    Id: NotRequired[str],
    ModificationTime: NotRequired[datetime],
    Name: NotRequired[str],
    OwnerId: NotRequired[str],
    ShareStatus: NotRequired[ShareStatusType],  # (1)
    Status: NotRequired[ProfileStatusType],  # (2)
    StatusMessage: NotRequired[str],
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
2. See [:material-code-brackets: ProfileStatusType](./literals.md#profilestatustype) 
## DeleteProfileRequestRequestTypeDef

```python
# DeleteProfileRequestRequestTypeDef definition

class DeleteProfileRequestRequestTypeDef(TypedDict):
    ProfileId: str,
```

## DisassociateProfileRequestRequestTypeDef

```python
# DisassociateProfileRequestRequestTypeDef definition

class DisassociateProfileRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    ResourceId: str,
```

## DisassociateResourceFromProfileRequestRequestTypeDef

```python
# DisassociateResourceFromProfileRequestRequestTypeDef definition

class DisassociateResourceFromProfileRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    ResourceArn: str,
```

## GetProfileAssociationRequestRequestTypeDef

```python
# GetProfileAssociationRequestRequestTypeDef definition

class GetProfileAssociationRequestRequestTypeDef(TypedDict):
    ProfileAssociationId: str,
```

## GetProfileRequestRequestTypeDef

```python
# GetProfileRequestRequestTypeDef definition

class GetProfileRequestRequestTypeDef(TypedDict):
    ProfileId: str,
```

## GetProfileResourceAssociationRequestRequestTypeDef

```python
# GetProfileResourceAssociationRequestRequestTypeDef definition

class GetProfileResourceAssociationRequestRequestTypeDef(TypedDict):
    ProfileResourceAssociationId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListProfileAssociationsRequestRequestTypeDef

```python
# ListProfileAssociationsRequestRequestTypeDef definition

class ListProfileAssociationsRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ProfileId: NotRequired[str],
    ResourceId: NotRequired[str],
```

## ListProfileResourceAssociationsRequestRequestTypeDef

```python
# ListProfileResourceAssociationsRequestRequestTypeDef definition

class ListProfileResourceAssociationsRequestRequestTypeDef(TypedDict):
    ProfileId: str,
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
    ResourceType: NotRequired[str],
```

## ListProfilesRequestRequestTypeDef

```python
# ListProfilesRequestRequestTypeDef definition

class ListProfilesRequestRequestTypeDef(TypedDict):
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ProfileSummaryTypeDef

```python
# ProfileSummaryTypeDef definition

class ProfileSummaryTypeDef(TypedDict):
    Arn: NotRequired[str],
    Id: NotRequired[str],
    Name: NotRequired[str],
    ShareStatus: NotRequired[ShareStatusType],  # (1)
```

1. See [:material-code-brackets: ShareStatusType](./literals.md#sharestatustype) 
## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Mapping[str, str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateProfileResourceAssociationRequestRequestTypeDef

```python
# UpdateProfileResourceAssociationRequestRequestTypeDef definition

class UpdateProfileResourceAssociationRequestRequestTypeDef(TypedDict):
    ProfileResourceAssociationId: str,
    Name: NotRequired[str],
    ResourceProperties: NotRequired[str],
```

## AssociateProfileRequestRequestTypeDef

```python
# AssociateProfileRequestRequestTypeDef definition

class AssociateProfileRequestRequestTypeDef(TypedDict):
    Name: str,
    ProfileId: str,
    ResourceId: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateProfileRequestRequestTypeDef

```python
# CreateProfileRequestRequestTypeDef definition

class CreateProfileRequestRequestTypeDef(TypedDict):
    ClientToken: str,
    Name: str,
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## AssociateProfileResponseTypeDef

```python
# AssociateProfileResponseTypeDef definition

class AssociateProfileResponseTypeDef(TypedDict):
    ProfileAssociation: ProfileAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileAssociationTypeDef](./type_defs.md#profileassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateProfileResponseTypeDef

```python
# DisassociateProfileResponseTypeDef definition

class DisassociateProfileResponseTypeDef(TypedDict):
    ProfileAssociation: ProfileAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileAssociationTypeDef](./type_defs.md#profileassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileAssociationResponseTypeDef

```python
# GetProfileAssociationResponseTypeDef definition

class GetProfileAssociationResponseTypeDef(TypedDict):
    ProfileAssociation: ProfileAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileAssociationTypeDef](./type_defs.md#profileassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfileAssociationsResponseTypeDef

```python
# ListProfileAssociationsResponseTypeDef definition

class ListProfileAssociationsResponseTypeDef(TypedDict):
    ProfileAssociations: List[ProfileAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProfileAssociationTypeDef](./type_defs.md#profileassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateResourceToProfileResponseTypeDef

```python
# AssociateResourceToProfileResponseTypeDef definition

class AssociateResourceToProfileResponseTypeDef(TypedDict):
    ProfileResourceAssociation: ProfileResourceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileResourceAssociationTypeDef](./type_defs.md#profileresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateResourceFromProfileResponseTypeDef

```python
# DisassociateResourceFromProfileResponseTypeDef definition

class DisassociateResourceFromProfileResponseTypeDef(TypedDict):
    ProfileResourceAssociation: ProfileResourceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileResourceAssociationTypeDef](./type_defs.md#profileresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileResourceAssociationResponseTypeDef

```python
# GetProfileResourceAssociationResponseTypeDef definition

class GetProfileResourceAssociationResponseTypeDef(TypedDict):
    ProfileResourceAssociation: ProfileResourceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileResourceAssociationTypeDef](./type_defs.md#profileresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfileResourceAssociationsResponseTypeDef

```python
# ListProfileResourceAssociationsResponseTypeDef definition

class ListProfileResourceAssociationsResponseTypeDef(TypedDict):
    ProfileResourceAssociations: List[ProfileResourceAssociationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProfileResourceAssociationTypeDef](./type_defs.md#profileresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateProfileResourceAssociationResponseTypeDef

```python
# UpdateProfileResourceAssociationResponseTypeDef definition

class UpdateProfileResourceAssociationResponseTypeDef(TypedDict):
    ProfileResourceAssociation: ProfileResourceAssociationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileResourceAssociationTypeDef](./type_defs.md#profileresourceassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateProfileResponseTypeDef

```python
# CreateProfileResponseTypeDef definition

class CreateProfileResponseTypeDef(TypedDict):
    Profile: ProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileTypeDef](./type_defs.md#profiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteProfileResponseTypeDef

```python
# DeleteProfileResponseTypeDef definition

class DeleteProfileResponseTypeDef(TypedDict):
    Profile: ProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileTypeDef](./type_defs.md#profiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetProfileResponseTypeDef

```python
# GetProfileResponseTypeDef definition

class GetProfileResponseTypeDef(TypedDict):
    Profile: ProfileTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ProfileTypeDef](./type_defs.md#profiletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListProfileAssociationsRequestListProfileAssociationsPaginateTypeDef

```python
# ListProfileAssociationsRequestListProfileAssociationsPaginateTypeDef definition

class ListProfileAssociationsRequestListProfileAssociationsPaginateTypeDef(TypedDict):
    ProfileId: NotRequired[str],
    ResourceId: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProfileResourceAssociationsRequestListProfileResourceAssociationsPaginateTypeDef

```python
# ListProfileResourceAssociationsRequestListProfileResourceAssociationsPaginateTypeDef definition

class ListProfileResourceAssociationsRequestListProfileResourceAssociationsPaginateTypeDef(TypedDict):
    ProfileId: str,
    ResourceType: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProfilesRequestListProfilesPaginateTypeDef

```python
# ListProfilesRequestListProfilesPaginateTypeDef definition

class ListProfilesRequestListProfilesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListProfilesResponseTypeDef

```python
# ListProfilesResponseTypeDef definition

class ListProfilesResponseTypeDef(TypedDict):
    ProfileSummaries: List[ProfileSummaryTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: ProfileSummaryTypeDef](./type_defs.md#profilesummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

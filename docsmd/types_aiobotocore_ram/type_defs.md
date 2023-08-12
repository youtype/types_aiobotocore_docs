# Type definitions

> [Index](../README.md) > [RAM](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [RAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ram.html#RAM)
    type annotations stubs module [types-aiobotocore-ram](https://pypi.org/project/types-aiobotocore-ram/).



## AcceptResourceShareInvitationRequestRequestTypeDef

```python
# AcceptResourceShareInvitationRequestRequestTypeDef definition

class AcceptResourceShareInvitationRequestRequestTypeDef(TypedDict):
    resourceShareInvitationArn: str,
    clientToken: NotRequired[str],
```

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

## AssociateResourceSharePermissionRequestRequestTypeDef

```python
# AssociateResourceSharePermissionRequestRequestTypeDef definition

class AssociateResourceSharePermissionRequestRequestTypeDef(TypedDict):
    resourceShareArn: str,
    permissionArn: str,
    replace: NotRequired[bool],
    clientToken: NotRequired[str],
    permissionVersion: NotRequired[int],
```

## AssociateResourceShareRequestRequestTypeDef

```python
# AssociateResourceShareRequestRequestTypeDef definition

class AssociateResourceShareRequestRequestTypeDef(TypedDict):
    resourceShareArn: str,
    resourceArns: NotRequired[Sequence[str]],
    principals: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
    sources: NotRequired[Sequence[str]],
```

## ResourceShareAssociationTypeDef

```python
# ResourceShareAssociationTypeDef definition

class ResourceShareAssociationTypeDef(TypedDict):
    resourceShareArn: NotRequired[str],
    resourceShareName: NotRequired[str],
    associatedEntity: NotRequired[str],
    associationType: NotRequired[ResourceShareAssociationTypeType],  # (1)
    status: NotRequired[ResourceShareAssociationStatusType],  # (2)
    statusMessage: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
    external: NotRequired[bool],
```

1. See [:material-code-brackets: ResourceShareAssociationTypeType](./literals.md#resourceshareassociationtypetype) 
2. See [:material-code-brackets: ResourceShareAssociationStatusType](./literals.md#resourceshareassociationstatustype) 
## AssociatedPermissionTypeDef

```python
# AssociatedPermissionTypeDef definition

class AssociatedPermissionTypeDef(TypedDict):
    arn: NotRequired[str],
    permissionVersion: NotRequired[str],
    defaultVersion: NotRequired[bool],
    resourceType: NotRequired[str],
    status: NotRequired[str],
    featureSet: NotRequired[PermissionFeatureSetType],  # (1)
    lastUpdatedTime: NotRequired[datetime],
    resourceShareArn: NotRequired[str],
```

1. See [:material-code-brackets: PermissionFeatureSetType](./literals.md#permissionfeaturesettype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    key: NotRequired[str],
    value: NotRequired[str],
```

## CreatePermissionVersionRequestRequestTypeDef

```python
# CreatePermissionVersionRequestRequestTypeDef definition

class CreatePermissionVersionRequestRequestTypeDef(TypedDict):
    permissionArn: str,
    policyTemplate: str,
    clientToken: NotRequired[str],
```

## DeletePermissionRequestRequestTypeDef

```python
# DeletePermissionRequestRequestTypeDef definition

class DeletePermissionRequestRequestTypeDef(TypedDict):
    permissionArn: str,
    clientToken: NotRequired[str],
```

## DeletePermissionVersionRequestRequestTypeDef

```python
# DeletePermissionVersionRequestRequestTypeDef definition

class DeletePermissionVersionRequestRequestTypeDef(TypedDict):
    permissionArn: str,
    permissionVersion: int,
    clientToken: NotRequired[str],
```

## DeleteResourceShareRequestRequestTypeDef

```python
# DeleteResourceShareRequestRequestTypeDef definition

class DeleteResourceShareRequestRequestTypeDef(TypedDict):
    resourceShareArn: str,
    clientToken: NotRequired[str],
```

## DisassociateResourceSharePermissionRequestRequestTypeDef

```python
# DisassociateResourceSharePermissionRequestRequestTypeDef definition

class DisassociateResourceSharePermissionRequestRequestTypeDef(TypedDict):
    resourceShareArn: str,
    permissionArn: str,
    clientToken: NotRequired[str],
```

## DisassociateResourceShareRequestRequestTypeDef

```python
# DisassociateResourceShareRequestRequestTypeDef definition

class DisassociateResourceShareRequestRequestTypeDef(TypedDict):
    resourceShareArn: str,
    resourceArns: NotRequired[Sequence[str]],
    principals: NotRequired[Sequence[str]],
    clientToken: NotRequired[str],
    sources: NotRequired[Sequence[str]],
```

## GetPermissionRequestRequestTypeDef

```python
# GetPermissionRequestRequestTypeDef definition

class GetPermissionRequestRequestTypeDef(TypedDict):
    permissionArn: str,
    permissionVersion: NotRequired[int],
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## GetResourcePoliciesRequestRequestTypeDef

```python
# GetResourcePoliciesRequestRequestTypeDef definition

class GetResourcePoliciesRequestRequestTypeDef(TypedDict):
    resourceArns: Sequence[str],
    principal: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## GetResourceShareAssociationsRequestRequestTypeDef

```python
# GetResourceShareAssociationsRequestRequestTypeDef definition

class GetResourceShareAssociationsRequestRequestTypeDef(TypedDict):
    associationType: ResourceShareAssociationTypeType,  # (1)
    resourceShareArns: NotRequired[Sequence[str]],
    resourceArn: NotRequired[str],
    principal: NotRequired[str],
    associationStatus: NotRequired[ResourceShareAssociationStatusType],  # (2)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceShareAssociationTypeType](./literals.md#resourceshareassociationtypetype) 
2. See [:material-code-brackets: ResourceShareAssociationStatusType](./literals.md#resourceshareassociationstatustype) 
## GetResourceShareInvitationsRequestRequestTypeDef

```python
# GetResourceShareInvitationsRequestRequestTypeDef definition

class GetResourceShareInvitationsRequestRequestTypeDef(TypedDict):
    resourceShareInvitationArns: NotRequired[Sequence[str]],
    resourceShareArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## TagFilterTypeDef

```python
# TagFilterTypeDef definition

class TagFilterTypeDef(TypedDict):
    tagKey: NotRequired[str],
    tagValues: NotRequired[Sequence[str]],
```

## ListPendingInvitationResourcesRequestRequestTypeDef

```python
# ListPendingInvitationResourcesRequestRequestTypeDef definition

class ListPendingInvitationResourcesRequestRequestTypeDef(TypedDict):
    resourceShareInvitationArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    resourceRegionScope: NotRequired[ResourceRegionScopeFilterType],  # (1)
```

1. See [:material-code-brackets: ResourceRegionScopeFilterType](./literals.md#resourceregionscopefiltertype) 
## ResourceTypeDef

```python
# ResourceTypeDef definition

class ResourceTypeDef(TypedDict):
    arn: NotRequired[str],
    type: NotRequired[str],
    resourceShareArn: NotRequired[str],
    resourceGroupArn: NotRequired[str],
    status: NotRequired[ResourceStatusType],  # (1)
    statusMessage: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
    resourceRegionScope: NotRequired[ResourceRegionScopeType],  # (2)
```

1. See [:material-code-brackets: ResourceStatusType](./literals.md#resourcestatustype) 
2. See [:material-code-brackets: ResourceRegionScopeType](./literals.md#resourceregionscopetype) 
## ListPermissionAssociationsRequestRequestTypeDef

```python
# ListPermissionAssociationsRequestRequestTypeDef definition

class ListPermissionAssociationsRequestRequestTypeDef(TypedDict):
    permissionArn: NotRequired[str],
    permissionVersion: NotRequired[int],
    associationStatus: NotRequired[ResourceShareAssociationStatusType],  # (1)
    resourceType: NotRequired[str],
    featureSet: NotRequired[PermissionFeatureSetType],  # (2)
    defaultVersion: NotRequired[bool],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceShareAssociationStatusType](./literals.md#resourceshareassociationstatustype) 
2. See [:material-code-brackets: PermissionFeatureSetType](./literals.md#permissionfeaturesettype) 
## ListPermissionVersionsRequestRequestTypeDef

```python
# ListPermissionVersionsRequestRequestTypeDef definition

class ListPermissionVersionsRequestRequestTypeDef(TypedDict):
    permissionArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListPermissionsRequestRequestTypeDef

```python
# ListPermissionsRequestRequestTypeDef definition

class ListPermissionsRequestRequestTypeDef(TypedDict):
    resourceType: NotRequired[str],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    permissionType: NotRequired[PermissionTypeFilterType],  # (1)
```

1. See [:material-code-brackets: PermissionTypeFilterType](./literals.md#permissiontypefiltertype) 
## ListPrincipalsRequestRequestTypeDef

```python
# ListPrincipalsRequestRequestTypeDef definition

class ListPrincipalsRequestRequestTypeDef(TypedDict):
    resourceOwner: ResourceOwnerType,  # (1)
    resourceArn: NotRequired[str],
    principals: NotRequired[Sequence[str]],
    resourceType: NotRequired[str],
    resourceShareArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
## PrincipalTypeDef

```python
# PrincipalTypeDef definition

class PrincipalTypeDef(TypedDict):
    id: NotRequired[str],
    resourceShareArn: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
    external: NotRequired[bool],
```

## ListReplacePermissionAssociationsWorkRequestRequestTypeDef

```python
# ListReplacePermissionAssociationsWorkRequestRequestTypeDef definition

class ListReplacePermissionAssociationsWorkRequestRequestTypeDef(TypedDict):
    workIds: NotRequired[Sequence[str]],
    status: NotRequired[ReplacePermissionAssociationsWorkStatusType],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: ReplacePermissionAssociationsWorkStatusType](./literals.md#replacepermissionassociationsworkstatustype) 
## ReplacePermissionAssociationsWorkTypeDef

```python
# ReplacePermissionAssociationsWorkTypeDef definition

class ReplacePermissionAssociationsWorkTypeDef(TypedDict):
    id: NotRequired[str],
    fromPermissionArn: NotRequired[str],
    fromPermissionVersion: NotRequired[str],
    toPermissionArn: NotRequired[str],
    toPermissionVersion: NotRequired[str],
    status: NotRequired[ReplacePermissionAssociationsWorkStatusType],  # (1)
    statusMessage: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
```

1. See [:material-code-brackets: ReplacePermissionAssociationsWorkStatusType](./literals.md#replacepermissionassociationsworkstatustype) 
## ListResourceSharePermissionsRequestRequestTypeDef

```python
# ListResourceSharePermissionsRequestRequestTypeDef definition

class ListResourceSharePermissionsRequestRequestTypeDef(TypedDict):
    resourceShareArn: str,
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListResourceTypesRequestRequestTypeDef

```python
# ListResourceTypesRequestRequestTypeDef definition

class ListResourceTypesRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    resourceRegionScope: NotRequired[ResourceRegionScopeFilterType],  # (1)
```

1. See [:material-code-brackets: ResourceRegionScopeFilterType](./literals.md#resourceregionscopefiltertype) 
## ServiceNameAndResourceTypeTypeDef

```python
# ServiceNameAndResourceTypeTypeDef definition

class ServiceNameAndResourceTypeTypeDef(TypedDict):
    resourceType: NotRequired[str],
    serviceName: NotRequired[str],
    resourceRegionScope: NotRequired[ResourceRegionScopeType],  # (1)
```

1. See [:material-code-brackets: ResourceRegionScopeType](./literals.md#resourceregionscopetype) 
## ListResourcesRequestRequestTypeDef

```python
# ListResourcesRequestRequestTypeDef definition

class ListResourcesRequestRequestTypeDef(TypedDict):
    resourceOwner: ResourceOwnerType,  # (1)
    principal: NotRequired[str],
    resourceType: NotRequired[str],
    resourceArns: NotRequired[Sequence[str]],
    resourceShareArns: NotRequired[Sequence[str]],
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    resourceRegionScope: NotRequired[ResourceRegionScopeFilterType],  # (2)
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-brackets: ResourceRegionScopeFilterType](./literals.md#resourceregionscopefiltertype) 
## PromotePermissionCreatedFromPolicyRequestRequestTypeDef

```python
# PromotePermissionCreatedFromPolicyRequestRequestTypeDef definition

class PromotePermissionCreatedFromPolicyRequestRequestTypeDef(TypedDict):
    permissionArn: str,
    name: str,
    clientToken: NotRequired[str],
```

## PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef

```python
# PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef definition

class PromoteResourceShareCreatedFromPolicyRequestRequestTypeDef(TypedDict):
    resourceShareArn: str,
```

## RejectResourceShareInvitationRequestRequestTypeDef

```python
# RejectResourceShareInvitationRequestRequestTypeDef definition

class RejectResourceShareInvitationRequestRequestTypeDef(TypedDict):
    resourceShareInvitationArn: str,
    clientToken: NotRequired[str],
```

## ReplacePermissionAssociationsRequestRequestTypeDef

```python
# ReplacePermissionAssociationsRequestRequestTypeDef definition

class ReplacePermissionAssociationsRequestRequestTypeDef(TypedDict):
    fromPermissionArn: str,
    toPermissionArn: str,
    fromPermissionVersion: NotRequired[int],
    clientToken: NotRequired[str],
```

## SetDefaultPermissionVersionRequestRequestTypeDef

```python
# SetDefaultPermissionVersionRequestRequestTypeDef definition

class SetDefaultPermissionVersionRequestRequestTypeDef(TypedDict):
    permissionArn: str,
    permissionVersion: int,
    clientToken: NotRequired[str],
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    tagKeys: Sequence[str],
    resourceShareArn: NotRequired[str],
    resourceArn: NotRequired[str],
```

## UpdateResourceShareRequestRequestTypeDef

```python
# UpdateResourceShareRequestRequestTypeDef definition

class UpdateResourceShareRequestRequestTypeDef(TypedDict):
    resourceShareArn: str,
    name: NotRequired[str],
    allowExternalPrincipals: NotRequired[bool],
    clientToken: NotRequired[str],
```

## AssociateResourceSharePermissionResponseTypeDef

```python
# AssociateResourceSharePermissionResponseTypeDef definition

class AssociateResourceSharePermissionResponseTypeDef(TypedDict):
    returnValue: bool,
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePermissionResponseTypeDef

```python
# DeletePermissionResponseTypeDef definition

class DeletePermissionResponseTypeDef(TypedDict):
    returnValue: bool,
    clientToken: str,
    permissionStatus: PermissionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PermissionStatusType](./literals.md#permissionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeletePermissionVersionResponseTypeDef

```python
# DeletePermissionVersionResponseTypeDef definition

class DeletePermissionVersionResponseTypeDef(TypedDict):
    returnValue: bool,
    clientToken: str,
    permissionStatus: PermissionStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: PermissionStatusType](./literals.md#permissionstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteResourceShareResponseTypeDef

```python
# DeleteResourceShareResponseTypeDef definition

class DeleteResourceShareResponseTypeDef(TypedDict):
    returnValue: bool,
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateResourceSharePermissionResponseTypeDef

```python
# DisassociateResourceSharePermissionResponseTypeDef definition

class DisassociateResourceSharePermissionResponseTypeDef(TypedDict):
    returnValue: bool,
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EnableSharingWithAwsOrganizationResponseTypeDef

```python
# EnableSharingWithAwsOrganizationResponseTypeDef definition

class EnableSharingWithAwsOrganizationResponseTypeDef(TypedDict):
    returnValue: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourcePoliciesResponseTypeDef

```python
# GetResourcePoliciesResponseTypeDef definition

class GetResourcePoliciesResponseTypeDef(TypedDict):
    policies: List[str],
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromoteResourceShareCreatedFromPolicyResponseTypeDef

```python
# PromoteResourceShareCreatedFromPolicyResponseTypeDef definition

class PromoteResourceShareCreatedFromPolicyResponseTypeDef(TypedDict):
    returnValue: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SetDefaultPermissionVersionResponseTypeDef

```python
# SetDefaultPermissionVersionResponseTypeDef definition

class SetDefaultPermissionVersionResponseTypeDef(TypedDict):
    returnValue: bool,
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AssociateResourceShareResponseTypeDef

```python
# AssociateResourceShareResponseTypeDef definition

class AssociateResourceShareResponseTypeDef(TypedDict):
    resourceShareAssociations: List[ResourceShareAssociationTypeDef],  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareAssociationTypeDef](./type_defs.md#resourceshareassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DisassociateResourceShareResponseTypeDef

```python
# DisassociateResourceShareResponseTypeDef definition

class DisassociateResourceShareResponseTypeDef(TypedDict):
    resourceShareAssociations: List[ResourceShareAssociationTypeDef],  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareAssociationTypeDef](./type_defs.md#resourceshareassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceShareAssociationsResponseTypeDef

```python
# GetResourceShareAssociationsResponseTypeDef definition

class GetResourceShareAssociationsResponseTypeDef(TypedDict):
    resourceShareAssociations: List[ResourceShareAssociationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareAssociationTypeDef](./type_defs.md#resourceshareassociationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ResourceShareInvitationTypeDef

```python
# ResourceShareInvitationTypeDef definition

class ResourceShareInvitationTypeDef(TypedDict):
    resourceShareInvitationArn: NotRequired[str],
    resourceShareName: NotRequired[str],
    resourceShareArn: NotRequired[str],
    senderAccountId: NotRequired[str],
    receiverAccountId: NotRequired[str],
    invitationTimestamp: NotRequired[datetime],
    status: NotRequired[ResourceShareInvitationStatusType],  # (1)
    resourceShareAssociations: NotRequired[List[ResourceShareAssociationTypeDef]],  # (2)
    receiverArn: NotRequired[str],
```

1. See [:material-code-brackets: ResourceShareInvitationStatusType](./literals.md#resourceshareinvitationstatustype) 
2. See [:material-code-braces: ResourceShareAssociationTypeDef](./type_defs.md#resourceshareassociationtypedef) 
## ListPermissionAssociationsResponseTypeDef

```python
# ListPermissionAssociationsResponseTypeDef definition

class ListPermissionAssociationsResponseTypeDef(TypedDict):
    permissions: List[AssociatedPermissionTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: AssociatedPermissionTypeDef](./type_defs.md#associatedpermissiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePermissionRequestRequestTypeDef

```python
# CreatePermissionRequestRequestTypeDef definition

class CreatePermissionRequestRequestTypeDef(TypedDict):
    name: str,
    resourceType: str,
    policyTemplate: str,
    clientToken: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateResourceShareRequestRequestTypeDef

```python
# CreateResourceShareRequestRequestTypeDef definition

class CreateResourceShareRequestRequestTypeDef(TypedDict):
    name: str,
    resourceArns: NotRequired[Sequence[str]],
    principals: NotRequired[Sequence[str]],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    allowExternalPrincipals: NotRequired[bool],
    clientToken: NotRequired[str],
    permissionArns: NotRequired[Sequence[str]],
    sources: NotRequired[Sequence[str]],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResourceSharePermissionDetailTypeDef

```python
# ResourceSharePermissionDetailTypeDef definition

class ResourceSharePermissionDetailTypeDef(TypedDict):
    arn: NotRequired[str],
    version: NotRequired[str],
    defaultVersion: NotRequired[bool],
    name: NotRequired[str],
    resourceType: NotRequired[str],
    permission: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
    isResourceTypeDefault: NotRequired[bool],
    permissionType: NotRequired[PermissionTypeType],  # (1)
    featureSet: NotRequired[PermissionFeatureSetType],  # (2)
    status: NotRequired[PermissionStatusType],  # (3)
    tags: NotRequired[List[TagTypeDef]],  # (4)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-brackets: PermissionFeatureSetType](./literals.md#permissionfeaturesettype) 
3. See [:material-code-brackets: PermissionStatusType](./literals.md#permissionstatustype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResourceSharePermissionSummaryTypeDef

```python
# ResourceSharePermissionSummaryTypeDef definition

class ResourceSharePermissionSummaryTypeDef(TypedDict):
    arn: NotRequired[str],
    version: NotRequired[str],
    defaultVersion: NotRequired[bool],
    name: NotRequired[str],
    resourceType: NotRequired[str],
    status: NotRequired[str],
    creationTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
    isResourceTypeDefault: NotRequired[bool],
    permissionType: NotRequired[PermissionTypeType],  # (1)
    featureSet: NotRequired[PermissionFeatureSetType],  # (2)
    tags: NotRequired[List[TagTypeDef]],  # (3)
```

1. See [:material-code-brackets: PermissionTypeType](./literals.md#permissiontypetype) 
2. See [:material-code-brackets: PermissionFeatureSetType](./literals.md#permissionfeaturesettype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ResourceShareTypeDef

```python
# ResourceShareTypeDef definition

class ResourceShareTypeDef(TypedDict):
    resourceShareArn: NotRequired[str],
    name: NotRequired[str],
    owningAccountId: NotRequired[str],
    allowExternalPrincipals: NotRequired[bool],
    status: NotRequired[ResourceShareStatusType],  # (1)
    statusMessage: NotRequired[str],
    tags: NotRequired[List[TagTypeDef]],  # (2)
    creationTime: NotRequired[datetime],
    lastUpdatedTime: NotRequired[datetime],
    featureSet: NotRequired[ResourceShareFeatureSetType],  # (3)
```

1. See [:material-code-brackets: ResourceShareStatusType](./literals.md#resourcesharestatustype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-brackets: ResourceShareFeatureSetType](./literals.md#resourcesharefeaturesettype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    tags: Sequence[TagTypeDef],  # (1)
    resourceShareArn: NotRequired[str],
    resourceArn: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef

```python
# GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef definition

class GetResourcePoliciesRequestGetResourcePoliciesPaginateTypeDef(TypedDict):
    resourceArns: Sequence[str],
    principal: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef

```python
# GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef definition

class GetResourceShareAssociationsRequestGetResourceShareAssociationsPaginateTypeDef(TypedDict):
    associationType: ResourceShareAssociationTypeType,  # (1)
    resourceShareArns: NotRequired[Sequence[str]],
    resourceArn: NotRequired[str],
    principal: NotRequired[str],
    associationStatus: NotRequired[ResourceShareAssociationStatusType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceShareAssociationTypeType](./literals.md#resourceshareassociationtypetype) 
2. See [:material-code-brackets: ResourceShareAssociationStatusType](./literals.md#resourceshareassociationstatustype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef

```python
# GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef definition

class GetResourceShareInvitationsRequestGetResourceShareInvitationsPaginateTypeDef(TypedDict):
    resourceShareInvitationArns: NotRequired[Sequence[str]],
    resourceShareArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPrincipalsRequestListPrincipalsPaginateTypeDef

```python
# ListPrincipalsRequestListPrincipalsPaginateTypeDef definition

class ListPrincipalsRequestListPrincipalsPaginateTypeDef(TypedDict):
    resourceOwner: ResourceOwnerType,  # (1)
    resourceArn: NotRequired[str],
    principals: NotRequired[Sequence[str]],
    resourceType: NotRequired[str],
    resourceShareArns: NotRequired[Sequence[str]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListResourcesRequestListResourcesPaginateTypeDef

```python
# ListResourcesRequestListResourcesPaginateTypeDef definition

class ListResourcesRequestListResourcesPaginateTypeDef(TypedDict):
    resourceOwner: ResourceOwnerType,  # (1)
    principal: NotRequired[str],
    resourceType: NotRequired[str],
    resourceArns: NotRequired[Sequence[str]],
    resourceShareArns: NotRequired[Sequence[str]],
    resourceRegionScope: NotRequired[ResourceRegionScopeFilterType],  # (2)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (3)
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-brackets: ResourceRegionScopeFilterType](./literals.md#resourceregionscopefiltertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourceSharesRequestGetResourceSharesPaginateTypeDef

```python
# GetResourceSharesRequestGetResourceSharesPaginateTypeDef definition

class GetResourceSharesRequestGetResourceSharesPaginateTypeDef(TypedDict):
    resourceOwner: ResourceOwnerType,  # (1)
    resourceShareArns: NotRequired[Sequence[str]],
    resourceShareStatus: NotRequired[ResourceShareStatusType],  # (2)
    name: NotRequired[str],
    tagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (3)
    permissionArn: NotRequired[str],
    permissionVersion: NotRequired[int],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (4)
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-brackets: ResourceShareStatusType](./literals.md#resourcesharestatustype) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetResourceSharesRequestRequestTypeDef

```python
# GetResourceSharesRequestRequestTypeDef definition

class GetResourceSharesRequestRequestTypeDef(TypedDict):
    resourceOwner: ResourceOwnerType,  # (1)
    resourceShareArns: NotRequired[Sequence[str]],
    resourceShareStatus: NotRequired[ResourceShareStatusType],  # (2)
    name: NotRequired[str],
    tagFilters: NotRequired[Sequence[TagFilterTypeDef]],  # (3)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
    permissionArn: NotRequired[str],
    permissionVersion: NotRequired[int],
```

1. See [:material-code-brackets: ResourceOwnerType](./literals.md#resourceownertype) 
2. See [:material-code-brackets: ResourceShareStatusType](./literals.md#resourcesharestatustype) 
3. See [:material-code-braces: TagFilterTypeDef](./type_defs.md#tagfiltertypedef) 
## ListPendingInvitationResourcesResponseTypeDef

```python
# ListPendingInvitationResourcesResponseTypeDef definition

class ListPendingInvitationResourcesResponseTypeDef(TypedDict):
    resources: List[ResourceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourcesResponseTypeDef

```python
# ListResourcesResponseTypeDef definition

class ListResourcesResponseTypeDef(TypedDict):
    resources: List[ResourceTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceTypeDef](./type_defs.md#resourcetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPrincipalsResponseTypeDef

```python
# ListPrincipalsResponseTypeDef definition

class ListPrincipalsResponseTypeDef(TypedDict):
    principals: List[PrincipalTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PrincipalTypeDef](./type_defs.md#principaltypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListReplacePermissionAssociationsWorkResponseTypeDef

```python
# ListReplacePermissionAssociationsWorkResponseTypeDef definition

class ListReplacePermissionAssociationsWorkResponseTypeDef(TypedDict):
    replacePermissionAssociationsWorks: List[ReplacePermissionAssociationsWorkTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplacePermissionAssociationsWorkTypeDef](./type_defs.md#replacepermissionassociationsworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplacePermissionAssociationsResponseTypeDef

```python
# ReplacePermissionAssociationsResponseTypeDef definition

class ReplacePermissionAssociationsResponseTypeDef(TypedDict):
    replacePermissionAssociationsWork: ReplacePermissionAssociationsWorkTypeDef,  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplacePermissionAssociationsWorkTypeDef](./type_defs.md#replacepermissionassociationsworktypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceTypesResponseTypeDef

```python
# ListResourceTypesResponseTypeDef definition

class ListResourceTypesResponseTypeDef(TypedDict):
    resourceTypes: List[ServiceNameAndResourceTypeTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ServiceNameAndResourceTypeTypeDef](./type_defs.md#servicenameandresourcetypetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## AcceptResourceShareInvitationResponseTypeDef

```python
# AcceptResourceShareInvitationResponseTypeDef definition

class AcceptResourceShareInvitationResponseTypeDef(TypedDict):
    resourceShareInvitation: ResourceShareInvitationTypeDef,  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareInvitationTypeDef](./type_defs.md#resourceshareinvitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceShareInvitationsResponseTypeDef

```python
# GetResourceShareInvitationsResponseTypeDef definition

class GetResourceShareInvitationsResponseTypeDef(TypedDict):
    resourceShareInvitations: List[ResourceShareInvitationTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareInvitationTypeDef](./type_defs.md#resourceshareinvitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RejectResourceShareInvitationResponseTypeDef

```python
# RejectResourceShareInvitationResponseTypeDef definition

class RejectResourceShareInvitationResponseTypeDef(TypedDict):
    resourceShareInvitation: ResourceShareInvitationTypeDef,  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareInvitationTypeDef](./type_defs.md#resourceshareinvitationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePermissionVersionResponseTypeDef

```python
# CreatePermissionVersionResponseTypeDef definition

class CreatePermissionVersionResponseTypeDef(TypedDict):
    permission: ResourceSharePermissionDetailTypeDef,  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSharePermissionDetailTypeDef](./type_defs.md#resourcesharepermissiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPermissionResponseTypeDef

```python
# GetPermissionResponseTypeDef definition

class GetPermissionResponseTypeDef(TypedDict):
    permission: ResourceSharePermissionDetailTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSharePermissionDetailTypeDef](./type_defs.md#resourcesharepermissiondetailtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePermissionResponseTypeDef

```python
# CreatePermissionResponseTypeDef definition

class CreatePermissionResponseTypeDef(TypedDict):
    permission: ResourceSharePermissionSummaryTypeDef,  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSharePermissionSummaryTypeDef](./type_defs.md#resourcesharepermissionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionVersionsResponseTypeDef

```python
# ListPermissionVersionsResponseTypeDef definition

class ListPermissionVersionsResponseTypeDef(TypedDict):
    permissions: List[ResourceSharePermissionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSharePermissionSummaryTypeDef](./type_defs.md#resourcesharepermissionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPermissionsResponseTypeDef

```python
# ListPermissionsResponseTypeDef definition

class ListPermissionsResponseTypeDef(TypedDict):
    permissions: List[ResourceSharePermissionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSharePermissionSummaryTypeDef](./type_defs.md#resourcesharepermissionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListResourceSharePermissionsResponseTypeDef

```python
# ListResourceSharePermissionsResponseTypeDef definition

class ListResourceSharePermissionsResponseTypeDef(TypedDict):
    permissions: List[ResourceSharePermissionSummaryTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSharePermissionSummaryTypeDef](./type_defs.md#resourcesharepermissionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PromotePermissionCreatedFromPolicyResponseTypeDef

```python
# PromotePermissionCreatedFromPolicyResponseTypeDef definition

class PromotePermissionCreatedFromPolicyResponseTypeDef(TypedDict):
    permission: ResourceSharePermissionSummaryTypeDef,  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceSharePermissionSummaryTypeDef](./type_defs.md#resourcesharepermissionsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateResourceShareResponseTypeDef

```python
# CreateResourceShareResponseTypeDef definition

class CreateResourceShareResponseTypeDef(TypedDict):
    resourceShare: ResourceShareTypeDef,  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareTypeDef](./type_defs.md#resourcesharetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetResourceSharesResponseTypeDef

```python
# GetResourceSharesResponseTypeDef definition

class GetResourceSharesResponseTypeDef(TypedDict):
    resourceShares: List[ResourceShareTypeDef],  # (1)
    nextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareTypeDef](./type_defs.md#resourcesharetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateResourceShareResponseTypeDef

```python
# UpdateResourceShareResponseTypeDef definition

class UpdateResourceShareResponseTypeDef(TypedDict):
    resourceShare: ResourceShareTypeDef,  # (1)
    clientToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResourceShareTypeDef](./type_defs.md#resourcesharetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

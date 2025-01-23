# Type definitions

> [Index](../README.md) > [Cloud9](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#cloud9)
    type annotations stubs module [types-aiobotocore-cloud9](https://pypi.org/project/types-aiobotocore-cloud9/).



## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
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

## CreateEnvironmentMembershipRequestRequestTypeDef

```python
# CreateEnvironmentMembershipRequestRequestTypeDef definition

class CreateEnvironmentMembershipRequestRequestTypeDef(TypedDict):
    environmentId: str,
    userArn: str,
    permissions: MemberPermissionsType,  # (1)
```

1. See [:material-code-brackets: MemberPermissionsType](./literals.md#memberpermissionstype) 
## EnvironmentMemberTypeDef

```python
# EnvironmentMemberTypeDef definition

class EnvironmentMemberTypeDef(TypedDict):
    permissions: PermissionsType,  # (1)
    userId: str,
    userArn: str,
    environmentId: str,
    lastAccess: NotRequired[datetime],
```

1. See [:material-code-brackets: PermissionsType](./literals.md#permissionstype) 
## DeleteEnvironmentMembershipRequestRequestTypeDef

```python
# DeleteEnvironmentMembershipRequestRequestTypeDef definition

class DeleteEnvironmentMembershipRequestRequestTypeDef(TypedDict):
    environmentId: str,
    userArn: str,
```

## DeleteEnvironmentRequestRequestTypeDef

```python
# DeleteEnvironmentRequestRequestTypeDef definition

class DeleteEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## DescribeEnvironmentMembershipsRequestRequestTypeDef

```python
# DescribeEnvironmentMembershipsRequestRequestTypeDef definition

class DescribeEnvironmentMembershipsRequestRequestTypeDef(TypedDict):
    userArn: NotRequired[str],
    environmentId: NotRequired[str],
    permissions: NotRequired[Sequence[PermissionsType]],  # (1)
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

1. See [:material-code-brackets: PermissionsType](./literals.md#permissionstype) 
## DescribeEnvironmentStatusRequestRequestTypeDef

```python
# DescribeEnvironmentStatusRequestRequestTypeDef definition

class DescribeEnvironmentStatusRequestRequestTypeDef(TypedDict):
    environmentId: str,
```

## DescribeEnvironmentsRequestRequestTypeDef

```python
# DescribeEnvironmentsRequestRequestTypeDef definition

class DescribeEnvironmentsRequestRequestTypeDef(TypedDict):
    environmentIds: Sequence[str],
```

## EnvironmentLifecycleTypeDef

```python
# EnvironmentLifecycleTypeDef definition

class EnvironmentLifecycleTypeDef(TypedDict):
    status: NotRequired[EnvironmentLifecycleStatusType],  # (1)
    reason: NotRequired[str],
    failureResource: NotRequired[str],
```

1. See [:material-code-brackets: EnvironmentLifecycleStatusType](./literals.md#environmentlifecyclestatustype) 
## ListEnvironmentsRequestRequestTypeDef

```python
# ListEnvironmentsRequestRequestTypeDef definition

class ListEnvironmentsRequestRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
    maxResults: NotRequired[int],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateEnvironmentMembershipRequestRequestTypeDef

```python
# UpdateEnvironmentMembershipRequestRequestTypeDef definition

class UpdateEnvironmentMembershipRequestRequestTypeDef(TypedDict):
    environmentId: str,
    userArn: str,
    permissions: MemberPermissionsType,  # (1)
```

1. See [:material-code-brackets: MemberPermissionsType](./literals.md#memberpermissionstype) 
## UpdateEnvironmentRequestRequestTypeDef

```python
# UpdateEnvironmentRequestRequestTypeDef definition

class UpdateEnvironmentRequestRequestTypeDef(TypedDict):
    environmentId: str,
    name: NotRequired[str],
    description: NotRequired[str],
    managedCredentialsAction: NotRequired[ManagedCredentialsActionType],  # (1)
```

1. See [:material-code-brackets: ManagedCredentialsActionType](./literals.md#managedcredentialsactiontype) 
## CreateEnvironmentEC2RequestRequestTypeDef

```python
# CreateEnvironmentEC2RequestRequestTypeDef definition

class CreateEnvironmentEC2RequestRequestTypeDef(TypedDict):
    name: str,
    instanceType: str,
    imageId: str,
    description: NotRequired[str],
    clientRequestToken: NotRequired[str],
    subnetId: NotRequired[str],
    automaticStopTimeMinutes: NotRequired[int],
    ownerArn: NotRequired[str],
    tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    connectionType: NotRequired[ConnectionTypeType],  # (2)
    dryRun: NotRequired[bool],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateEnvironmentEC2ResultTypeDef

```python
# CreateEnvironmentEC2ResultTypeDef definition

class CreateEnvironmentEC2ResultTypeDef(TypedDict):
    environmentId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEnvironmentStatusResultTypeDef

```python
# DescribeEnvironmentStatusResultTypeDef definition

class DescribeEnvironmentStatusResultTypeDef(TypedDict):
    status: EnvironmentStatusType,  # (1)
    message: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: EnvironmentStatusType](./literals.md#environmentstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEnvironmentsResultTypeDef

```python
# ListEnvironmentsResultTypeDef definition

class ListEnvironmentsResultTypeDef(TypedDict):
    environmentIds: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEnvironmentMembershipResultTypeDef

```python
# CreateEnvironmentMembershipResultTypeDef definition

class CreateEnvironmentMembershipResultTypeDef(TypedDict):
    membership: EnvironmentMemberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentMemberTypeDef](./type_defs.md#environmentmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEnvironmentMembershipsResultTypeDef

```python
# DescribeEnvironmentMembershipsResultTypeDef definition

class DescribeEnvironmentMembershipsResultTypeDef(TypedDict):
    memberships: List[EnvironmentMemberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: EnvironmentMemberTypeDef](./type_defs.md#environmentmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateEnvironmentMembershipResultTypeDef

```python
# UpdateEnvironmentMembershipResultTypeDef definition

class UpdateEnvironmentMembershipResultTypeDef(TypedDict):
    membership: EnvironmentMemberTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentMemberTypeDef](./type_defs.md#environmentmembertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEnvironmentMembershipsRequestPaginateTypeDef

```python
# DescribeEnvironmentMembershipsRequestPaginateTypeDef definition

class DescribeEnvironmentMembershipsRequestPaginateTypeDef(TypedDict):
    userArn: NotRequired[str],
    environmentId: NotRequired[str],
    permissions: NotRequired[Sequence[PermissionsType]],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: PermissionsType](./literals.md#permissionstype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListEnvironmentsRequestPaginateTypeDef

```python
# ListEnvironmentsRequestPaginateTypeDef definition

class ListEnvironmentsRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## EnvironmentTypeDef

```python
# EnvironmentTypeDef definition

class EnvironmentTypeDef(TypedDict):
    type: EnvironmentTypeType,  # (1)
    arn: str,
    ownerArn: str,
    id: NotRequired[str],
    name: NotRequired[str],
    description: NotRequired[str],
    connectionType: NotRequired[ConnectionTypeType],  # (2)
    lifecycle: NotRequired[EnvironmentLifecycleTypeDef],  # (3)
    managedCredentialsStatus: NotRequired[ManagedCredentialsStatusType],  # (4)
```

1. See [:material-code-brackets: EnvironmentTypeType](./literals.md#environmenttypetype) 
2. See [:material-code-brackets: ConnectionTypeType](./literals.md#connectiontypetype) 
3. See [:material-code-braces: EnvironmentLifecycleTypeDef](./type_defs.md#environmentlifecycletypedef) 
4. See [:material-code-brackets: ManagedCredentialsStatusType](./literals.md#managedcredentialsstatustype) 
## DescribeEnvironmentsResultTypeDef

```python
# DescribeEnvironmentsResultTypeDef definition

class DescribeEnvironmentsResultTypeDef(TypedDict):
    environments: List[EnvironmentTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EnvironmentTypeDef](./type_defs.md#environmenttypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

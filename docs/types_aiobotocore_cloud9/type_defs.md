<a id="typed-dictionaries-for-aiobotocore-cloud9-module"></a>

# Typed dictionaries for aiobotocore Cloud9 module

> [Index](../README.md) > [Cloud9](./README.md) > Typed dictionaries

Auto-generated documentation for
[Cloud9](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
type annotations stubs module
[types-aiobotocore-cloud9](https://pypi.org/project/types-aiobotocore-cloud9/).

- [Typed dictionaries for aiobotocore Cloud9 module](#typed-dictionaries-for-aiobotocore-cloud9-module)
  - [CreateEnvironmentEC2RequestRequestTypeDef](#createenvironmentec2requestrequesttypedef)
  - [CreateEnvironmentEC2ResultTypeDef](#createenvironmentec2resulttypedef)
  - [CreateEnvironmentMembershipRequestRequestTypeDef](#createenvironmentmembershiprequestrequesttypedef)
  - [CreateEnvironmentMembershipResultTypeDef](#createenvironmentmembershipresulttypedef)
  - [DeleteEnvironmentMembershipRequestRequestTypeDef](#deleteenvironmentmembershiprequestrequesttypedef)
  - [DeleteEnvironmentRequestRequestTypeDef](#deleteenvironmentrequestrequesttypedef)
  - [DescribeEnvironmentMembershipsRequestRequestTypeDef](#describeenvironmentmembershipsrequestrequesttypedef)
  - [DescribeEnvironmentMembershipsResultTypeDef](#describeenvironmentmembershipsresulttypedef)
  - [DescribeEnvironmentStatusRequestRequestTypeDef](#describeenvironmentstatusrequestrequesttypedef)
  - [DescribeEnvironmentStatusResultTypeDef](#describeenvironmentstatusresulttypedef)
  - [DescribeEnvironmentsRequestRequestTypeDef](#describeenvironmentsrequestrequesttypedef)
  - [DescribeEnvironmentsResultTypeDef](#describeenvironmentsresulttypedef)
  - [EnvironmentLifecycleTypeDef](#environmentlifecycletypedef)
  - [EnvironmentMemberTypeDef](#environmentmembertypedef)
  - [EnvironmentTypeDef](#environmenttypedef)
  - [ListEnvironmentsRequestRequestTypeDef](#listenvironmentsrequestrequesttypedef)
  - [ListEnvironmentsResultTypeDef](#listenvironmentsresulttypedef)
  - [ListTagsForResourceRequestRequestTypeDef](#listtagsforresourcerequestrequesttypedef)
  - [ListTagsForResourceResponseTypeDef](#listtagsforresourceresponsetypedef)
  - [PaginatorConfigTypeDef](#paginatorconfigtypedef)
  - [ResponseMetadataTypeDef](#responsemetadatatypedef)
  - [TagResourceRequestRequestTypeDef](#tagresourcerequestrequesttypedef)
  - [TagTypeDef](#tagtypedef)
  - [UntagResourceRequestRequestTypeDef](#untagresourcerequestrequesttypedef)
  - [UpdateEnvironmentMembershipRequestRequestTypeDef](#updateenvironmentmembershiprequestrequesttypedef)
  - [UpdateEnvironmentMembershipResultTypeDef](#updateenvironmentmembershipresulttypedef)
  - [UpdateEnvironmentRequestRequestTypeDef](#updateenvironmentrequestrequesttypedef)

<a id="createenvironmentec2requestrequesttypedef"></a>

## CreateEnvironmentEC2RequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import CreateEnvironmentEC2RequestRequestTypeDef
```

Required fields:

- `name`: `str`
- `instanceType`: `str`

Optional fields:

- `description`: `str`
- `clientRequestToken`: `str`
- `subnetId`: `str`
- `imageId`: `str`
- `automaticStopTimeMinutes`: `int`
- `ownerArn`: `str`
- `tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `connectionType`: [ConnectionTypeType](./literals.md#connectiontypetype)
- `dryRun`: `bool`

<a id="createenvironmentec2resulttypedef"></a>

## CreateEnvironmentEC2ResultTypeDef

```python
from types_aiobotocore_cloud9.type_defs import CreateEnvironmentEC2ResultTypeDef
```

Required fields:

- `environmentId`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="createenvironmentmembershiprequestrequesttypedef"></a>

## CreateEnvironmentMembershipRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import CreateEnvironmentMembershipRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`
- `userArn`: `str`
- `permissions`: [MemberPermissionsType](./literals.md#memberpermissionstype)

<a id="createenvironmentmembershipresulttypedef"></a>

## CreateEnvironmentMembershipResultTypeDef

```python
from types_aiobotocore_cloud9.type_defs import CreateEnvironmentMembershipResultTypeDef
```

Required fields:

- `membership`:
  [EnvironmentMemberTypeDef](./type_defs.md#environmentmembertypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="deleteenvironmentmembershiprequestrequesttypedef"></a>

## DeleteEnvironmentMembershipRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import DeleteEnvironmentMembershipRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`
- `userArn`: `str`

<a id="deleteenvironmentrequestrequesttypedef"></a>

## DeleteEnvironmentRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import DeleteEnvironmentRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`

<a id="describeenvironmentmembershipsrequestrequesttypedef"></a>

## DescribeEnvironmentMembershipsRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import DescribeEnvironmentMembershipsRequestRequestTypeDef
```

Optional fields:

- `userArn`: `str`
- `environmentId`: `str`
- `permissions`: `Sequence`\[[PermissionsType](./literals.md#permissionstype)\]
- `nextToken`: `str`
- `maxResults`: `int`

<a id="describeenvironmentmembershipsresulttypedef"></a>

## DescribeEnvironmentMembershipsResultTypeDef

```python
from types_aiobotocore_cloud9.type_defs import DescribeEnvironmentMembershipsResultTypeDef
```

Required fields:

- `memberships`:
  `List`\[[EnvironmentMemberTypeDef](./type_defs.md#environmentmembertypedef)\]
- `nextToken`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeenvironmentstatusrequestrequesttypedef"></a>

## DescribeEnvironmentStatusRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import DescribeEnvironmentStatusRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`

<a id="describeenvironmentstatusresulttypedef"></a>

## DescribeEnvironmentStatusResultTypeDef

```python
from types_aiobotocore_cloud9.type_defs import DescribeEnvironmentStatusResultTypeDef
```

Required fields:

- `status`: [EnvironmentStatusType](./literals.md#environmentstatustype)
- `message`: `str`
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="describeenvironmentsrequestrequesttypedef"></a>

## DescribeEnvironmentsRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import DescribeEnvironmentsRequestRequestTypeDef
```

Required fields:

- `environmentIds`: `Sequence`\[`str`\]

<a id="describeenvironmentsresulttypedef"></a>

## DescribeEnvironmentsResultTypeDef

```python
from types_aiobotocore_cloud9.type_defs import DescribeEnvironmentsResultTypeDef
```

Required fields:

- `environments`:
  `List`\[[EnvironmentTypeDef](./type_defs.md#environmenttypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="environmentlifecycletypedef"></a>

## EnvironmentLifecycleTypeDef

```python
from types_aiobotocore_cloud9.type_defs import EnvironmentLifecycleTypeDef
```

Optional fields:

- `status`:
  [EnvironmentLifecycleStatusType](./literals.md#environmentlifecyclestatustype)
- `reason`: `str`
- `failureResource`: `str`

<a id="environmentmembertypedef"></a>

## EnvironmentMemberTypeDef

```python
from types_aiobotocore_cloud9.type_defs import EnvironmentMemberTypeDef
```

Required fields:

- `permissions`: [PermissionsType](./literals.md#permissionstype)
- `userId`: `str`
- `userArn`: `str`
- `environmentId`: `str`

Optional fields:

- `lastAccess`: `datetime`

<a id="environmenttypedef"></a>

## EnvironmentTypeDef

```python
from types_aiobotocore_cloud9.type_defs import EnvironmentTypeDef
```

Required fields:

- `type`: [EnvironmentTypeType](./literals.md#environmenttypetype)
- `arn`: `str`
- `ownerArn`: `str`

Optional fields:

- `id`: `str`
- `name`: `str`
- `description`: `str`
- `connectionType`: [ConnectionTypeType](./literals.md#connectiontypetype)
- `lifecycle`:
  [EnvironmentLifecycleTypeDef](./type_defs.md#environmentlifecycletypedef)
- `managedCredentialsStatus`:
  [ManagedCredentialsStatusType](./literals.md#managedcredentialsstatustype)

<a id="listenvironmentsrequestrequesttypedef"></a>

## ListEnvironmentsRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import ListEnvironmentsRequestRequestTypeDef
```

Optional fields:

- `nextToken`: `str`
- `maxResults`: `int`

<a id="listenvironmentsresulttypedef"></a>

## ListEnvironmentsResultTypeDef

```python
from types_aiobotocore_cloud9.type_defs import ListEnvironmentsResultTypeDef
```

Required fields:

- `nextToken`: `str`
- `environmentIds`: `List`\[`str`\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="listtagsforresourcerequestrequesttypedef"></a>

## ListTagsForResourceRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import ListTagsForResourceRequestRequestTypeDef
```

Required fields:

- `ResourceARN`: `str`

<a id="listtagsforresourceresponsetypedef"></a>

## ListTagsForResourceResponseTypeDef

```python
from types_aiobotocore_cloud9.type_defs import ListTagsForResourceResponseTypeDef
```

Required fields:

- `Tags`: `List`\[[TagTypeDef](./type_defs.md#tagtypedef)\]
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="paginatorconfigtypedef"></a>

## PaginatorConfigTypeDef

```python
from types_aiobotocore_cloud9.type_defs import PaginatorConfigTypeDef
```

Optional fields:

- `MaxItems`: `int`
- `PageSize`: `int`
- `StartingToken`: `str`

<a id="responsemetadatatypedef"></a>

## ResponseMetadataTypeDef

```python
from types_aiobotocore_cloud9.type_defs import ResponseMetadataTypeDef
```

Required fields:

- `RequestId`: `str`
- `HostId`: `str`
- `HTTPStatusCode`: `int`
- `HTTPHeaders`: `Dict`\[`str`, `str`\]
- `RetryAttempts`: `int`

<a id="tagresourcerequestrequesttypedef"></a>

## TagResourceRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import TagResourceRequestRequestTypeDef
```

Required fields:

- `ResourceARN`: `str`
- `Tags`: `Sequence`\[[TagTypeDef](./type_defs.md#tagtypedef)\]

<a id="tagtypedef"></a>

## TagTypeDef

```python
from types_aiobotocore_cloud9.type_defs import TagTypeDef
```

Required fields:

- `Key`: `str`
- `Value`: `str`

<a id="untagresourcerequestrequesttypedef"></a>

## UntagResourceRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import UntagResourceRequestRequestTypeDef
```

Required fields:

- `ResourceARN`: `str`
- `TagKeys`: `Sequence`\[`str`\]

<a id="updateenvironmentmembershiprequestrequesttypedef"></a>

## UpdateEnvironmentMembershipRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import UpdateEnvironmentMembershipRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`
- `userArn`: `str`
- `permissions`: [MemberPermissionsType](./literals.md#memberpermissionstype)

<a id="updateenvironmentmembershipresulttypedef"></a>

## UpdateEnvironmentMembershipResultTypeDef

```python
from types_aiobotocore_cloud9.type_defs import UpdateEnvironmentMembershipResultTypeDef
```

Required fields:

- `membership`:
  [EnvironmentMemberTypeDef](./type_defs.md#environmentmembertypedef)
- `ResponseMetadata`:
  [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)

<a id="updateenvironmentrequestrequesttypedef"></a>

## UpdateEnvironmentRequestRequestTypeDef

```python
from types_aiobotocore_cloud9.type_defs import UpdateEnvironmentRequestRequestTypeDef
```

Required fields:

- `environmentId`: `str`

Optional fields:

- `name`: `str`
- `description`: `str`
- `managedCredentialsAction`:
  [ManagedCredentialsActionType](./literals.md#managedcredentialsactiontype)

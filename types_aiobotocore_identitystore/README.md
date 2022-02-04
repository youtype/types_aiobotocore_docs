<a id="type-annotations-for-aiobotocore-identitystore-module"></a>

# Type annotations for aiobotocore IdentityStore module

> [Index](..) > IdentityStore

Auto-generated documentation for
[IdentityStore](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/identitystore.html#IdentityStore)
type annotations stubs module
[types-aiobotocore-identitystore](https://pypi.org/project/types-aiobotocore-identitystore/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[identitystore]'

# install as a standalone
pip install types-aiobotocore-identitystore
```

- [Type annotations for aiobotocore IdentityStore module](#type-annotations-for-aiobotocore-identitystore-module)
  - [IdentityStoreClient](#identitystoreclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="identitystoreclient"></a>

## IdentityStoreClient

Type annotations for `aiobotocore.create_client("identitystore")` as
[IdentityStoreClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_identitystore.client import IdentityStoreClient
```

<a id="methods"></a>

### Methods

- [can_paginate](./client.md#can_paginate)
- [describe_group](./client.md#describe_group)
- [describe_user](./client.md#describe_user)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [list_groups](./client.md#list_groups)
- [list_users](./client.md#list_users)

<a id="exceptions"></a>

### Exceptions

IdentityStoreClient [exceptions](./client.md#exceptions)

- AccessDeniedException
- ClientError
- InternalServerException
- ResourceNotFoundException
- ThrottlingException
- ValidationException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_identitystore.literals import ServiceName, ...
```

- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_identitystore.type_defs import DescribeGroupRequestRequestTypeDef, ...
```

- [DescribeGroupRequestRequestTypeDef](./type_defs.md#describegrouprequestrequesttypedef)
- [DescribeGroupResponseTypeDef](./type_defs.md#describegroupresponsetypedef)
- [DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef)
- [DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef)
- [FilterTypeDef](./type_defs.md#filtertypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef)
- [ListGroupsResponseTypeDef](./type_defs.md#listgroupsresponsetypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [UserTypeDef](./type_defs.md#usertypedef)

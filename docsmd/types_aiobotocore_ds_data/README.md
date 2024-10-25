# DirectoryServiceData module

> [Index](../README.md) > DirectoryServiceData


!!! note ""

    Auto-generated documentation for [DirectoryServiceData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#DirectoryServiceData)
    type annotations stubs module [types-aiobotocore-ds-data](https://pypi.org/project/types-aiobotocore-ds-data/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `DirectoryServiceData` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ds-data]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ds-data]'


# standalone installation
python -m pip install types-aiobotocore-ds-data
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ds-data
```

## Usage

Code samples can be found in [Examples](./usage.md).

## DirectoryServiceDataClient

Type annotations and code completion for  `#!python session.create_client("ds-data")` as [DirectoryServiceDataClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds-data.html#DirectoryServiceData.Client)

```python
# DirectoryServiceDataClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ds_data.client import DirectoryServiceDataClient


session = get_session()
async with session.create_client("ds-data") as client:
    client: DirectoryServiceDataClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("ds-data").get_paginator("...")`.

```python
# ListGroupMembersPaginator usage example

from types_aiobotocore_ds_data.paginator import ListGroupMembersPaginator

def get_list_group_members_paginator() -> ListGroupMembersPaginator:
    return client.get_paginator("list_group_members"))
```

- [ListGroupMembersPaginator](./paginators.md#listgroupmemberspaginator)
- [ListGroupsPaginator](./paginators.md#listgroupspaginator)
- [ListGroupsForMemberPaginator](./paginators.md#listgroupsformemberpaginator)
- [ListUsersPaginator](./paginators.md#listuserspaginator)
- [SearchGroupsPaginator](./paginators.md#searchgroupspaginator)
- [SearchUsersPaginator](./paginators.md#searchuserspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# GroupScopeType usage example

from types_aiobotocore_ds_data.literals import GroupScopeType

def get_value() -> GroupScopeType:
    return "BuiltinLocal"
```

- [GroupScopeType](./literals.md#groupscopetype)
- [GroupTypeType](./literals.md#grouptypetype)
- [ListGroupMembersPaginatorName](./literals.md#listgroupmemberspaginatorname)
- [ListGroupsForMemberPaginatorName](./literals.md#listgroupsformemberpaginatorname)
- [ListGroupsPaginatorName](./literals.md#listgroupspaginatorname)
- [ListUsersPaginatorName](./literals.md#listuserspaginatorname)
- [MemberTypeType](./literals.md#membertypetype)
- [SearchGroupsPaginatorName](./literals.md#searchgroupspaginatorname)
- [SearchUsersPaginatorName](./literals.md#searchuserspaginatorname)
- [UpdateTypeType](./literals.md#updatetypetype)
- [DirectoryServiceDataServiceName](./literals.md#directoryservicedataservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AddGroupMemberRequestRequestTypeDef](./type_defs.md#addgroupmemberrequestrequesttypedef)
- [AttributeValueOutputTypeDef](./type_defs.md#attributevalueoutputtypedef)
- [AttributeValueTypeDef](./type_defs.md#attributevaluetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeleteGroupRequestRequestTypeDef](./type_defs.md#deletegrouprequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DescribeGroupRequestRequestTypeDef](./type_defs.md#describegrouprequestrequesttypedef)
- [DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef)
- [DisableUserRequestRequestTypeDef](./type_defs.md#disableuserrequestrequesttypedef)
- [GroupSummaryTypeDef](./type_defs.md#groupsummarytypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListGroupMembersRequestRequestTypeDef](./type_defs.md#listgroupmembersrequestrequesttypedef)
- [MemberTypeDef](./type_defs.md#membertypedef)
- [ListGroupsForMemberRequestRequestTypeDef](./type_defs.md#listgroupsformemberrequestrequesttypedef)
- [ListGroupsRequestRequestTypeDef](./type_defs.md#listgroupsrequestrequesttypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [UserSummaryTypeDef](./type_defs.md#usersummarytypedef)
- [RemoveGroupMemberRequestRequestTypeDef](./type_defs.md#removegroupmemberrequestrequesttypedef)
- [SearchGroupsRequestRequestTypeDef](./type_defs.md#searchgroupsrequestrequesttypedef)
- [SearchUsersRequestRequestTypeDef](./type_defs.md#searchusersrequestrequesttypedef)
- [GroupTypeDef](./type_defs.md#grouptypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [AttributeValueUnionTypeDef](./type_defs.md#attributevalueuniontypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [UpdateGroupRequestRequestTypeDef](./type_defs.md#updategrouprequestrequesttypedef)
- [UpdateUserRequestRequestTypeDef](./type_defs.md#updateuserrequestrequesttypedef)
- [CreateGroupResultTypeDef](./type_defs.md#creategroupresulttypedef)
- [CreateUserResultTypeDef](./type_defs.md#createuserresulttypedef)
- [DescribeGroupResultTypeDef](./type_defs.md#describegroupresulttypedef)
- [DescribeUserResultTypeDef](./type_defs.md#describeuserresulttypedef)
- [ListGroupsForMemberResultTypeDef](./type_defs.md#listgroupsformemberresulttypedef)
- [ListGroupsResultTypeDef](./type_defs.md#listgroupsresulttypedef)
- [ListGroupMembersRequestListGroupMembersPaginateTypeDef](./type_defs.md#listgroupmembersrequestlistgroupmemberspaginatetypedef)
- [ListGroupsForMemberRequestListGroupsForMemberPaginateTypeDef](./type_defs.md#listgroupsformemberrequestlistgroupsformemberpaginatetypedef)
- [ListGroupsRequestListGroupsPaginateTypeDef](./type_defs.md#listgroupsrequestlistgroupspaginatetypedef)
- [ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef)
- [SearchGroupsRequestSearchGroupsPaginateTypeDef](./type_defs.md#searchgroupsrequestsearchgroupspaginatetypedef)
- [SearchUsersRequestSearchUsersPaginateTypeDef](./type_defs.md#searchusersrequestsearchuserspaginatetypedef)
- [ListGroupMembersResultTypeDef](./type_defs.md#listgroupmembersresulttypedef)
- [ListUsersResultTypeDef](./type_defs.md#listusersresulttypedef)
- [SearchGroupsResultTypeDef](./type_defs.md#searchgroupsresulttypedef)
- [SearchUsersResultTypeDef](./type_defs.md#searchusersresulttypedef)
- [CreateGroupRequestRequestTypeDef](./type_defs.md#creategrouprequestrequesttypedef)


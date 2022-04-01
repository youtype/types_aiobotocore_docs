# Paginators

> [Index](../README.md) > [SSOAdmin](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SSOAdmin](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin)
    type annotations stubs module [types-aiobotocore-sso-admin](https://pypi.org/project/types-aiobotocore-sso-admin/).

## ListAccountAssignmentCreationStatusPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_account_assignment_creation_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentCreationStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentCreationStatusPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListAccountAssignmentCreationStatusPaginator = client.get_paginator("list_account_assignment_creation_status")
```


### paginate

Type annotations and code completion for `#!python ListAccountAssignmentCreationStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAccountAssignmentCreationStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAccountAssignmentCreationStatusResponseTypeDef](./type_defs.md#listaccountassignmentcreationstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentCreationStatusRequestListAccountAssignmentCreationStatusPaginateTypeDef](./type_defs.md#listaccountassignmentcreationstatusrequestlistaccountassignmentcreationstatuspaginatetypedef) 
## ListAccountAssignmentDeletionStatusPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_account_assignment_deletion_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignmentDeletionStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentDeletionStatusPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListAccountAssignmentDeletionStatusPaginator = client.get_paginator("list_account_assignment_deletion_status")
```


### paginate

Type annotations and code completion for `#!python ListAccountAssignmentDeletionStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAccountAssignmentDeletionStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAccountAssignmentDeletionStatusResponseTypeDef](./type_defs.md#listaccountassignmentdeletionstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentDeletionStatusRequestListAccountAssignmentDeletionStatusPaginateTypeDef](./type_defs.md#listaccountassignmentdeletionstatusrequestlistaccountassignmentdeletionstatuspaginatetypedef) 
## ListAccountAssignmentsPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_account_assignments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountAssignments)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountAssignmentsPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListAccountAssignmentsPaginator = client.get_paginator("list_account_assignments")
```


### paginate

Type annotations and code completion for `#!python ListAccountAssignmentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    AccountId: str,
    PermissionSetArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListAccountAssignmentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListAccountAssignmentsResponseTypeDef](./type_defs.md#listaccountassignmentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "AccountId": ...,
    "PermissionSetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountAssignmentsRequestListAccountAssignmentsPaginateTypeDef](./type_defs.md#listaccountassignmentsrequestlistaccountassignmentspaginatetypedef) 
## ListAccountsForProvisionedPermissionSetPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_accounts_for_provisioned_permission_set")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListAccountsForProvisionedPermissionSet)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListAccountsForProvisionedPermissionSetPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListAccountsForProvisionedPermissionSetPaginator = client.get_paginator("list_accounts_for_provisioned_permission_set")
```


### paginate

Type annotations and code completion for `#!python ListAccountsForProvisionedPermissionSetPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    ProvisioningStatus: ProvisioningStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListAccountsForProvisionedPermissionSetResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListAccountsForProvisionedPermissionSetResponseTypeDef](./type_defs.md#listaccountsforprovisionedpermissionsetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAccountsForProvisionedPermissionSetRequestListAccountsForProvisionedPermissionSetPaginateTypeDef](./type_defs.md#listaccountsforprovisionedpermissionsetrequestlistaccountsforprovisionedpermissionsetpaginatetypedef) 
## ListInstancesPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_instances")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListInstances)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListInstancesPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListInstancesPaginator = client.get_paginator("list_instances")
```


### paginate

Type annotations and code completion for `#!python ListInstancesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListInstancesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListInstancesRequestListInstancesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListInstancesRequestListInstancesPaginateTypeDef](./type_defs.md#listinstancesrequestlistinstancespaginatetypedef) 
## ListManagedPoliciesInPermissionSetPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_managed_policies_in_permission_set")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListManagedPoliciesInPermissionSet)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListManagedPoliciesInPermissionSetPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListManagedPoliciesInPermissionSetPaginator = client.get_paginator("list_managed_policies_in_permission_set")
```


### paginate

Type annotations and code completion for `#!python ListManagedPoliciesInPermissionSetPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    PermissionSetArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListManagedPoliciesInPermissionSetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListManagedPoliciesInPermissionSetResponseTypeDef](./type_defs.md#listmanagedpoliciesinpermissionsetresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "PermissionSetArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef](./type_defs.md#listmanagedpoliciesinpermissionsetrequestlistmanagedpoliciesinpermissionsetpaginatetypedef) 
## ListPermissionSetProvisioningStatusPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_permission_set_provisioning_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetProvisioningStatus)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListPermissionSetProvisioningStatusPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListPermissionSetProvisioningStatusPaginator = client.get_paginator("list_permission_set_provisioning_status")
```


### paginate

Type annotations and code completion for `#!python ListPermissionSetProvisioningStatusPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    Filter: OperationStatusFilterTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPermissionSetProvisioningStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OperationStatusFilterTypeDef](./type_defs.md#operationstatusfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPermissionSetProvisioningStatusResponseTypeDef](./type_defs.md#listpermissionsetprovisioningstatusresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef](./type_defs.md#listpermissionsetprovisioningstatusrequestlistpermissionsetprovisioningstatuspaginatetypedef) 
## ListPermissionSetsPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_permission_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListPermissionSetsPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListPermissionSetsPaginator = client.get_paginator("list_permission_sets")
```


### paginate

Type annotations and code completion for `#!python ListPermissionSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListPermissionSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListPermissionSetsResponseTypeDef](./type_defs.md#listpermissionsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPermissionSetsRequestListPermissionSetsPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetsRequestListPermissionSetsPaginateTypeDef](./type_defs.md#listpermissionsetsrequestlistpermissionsetspaginatetypedef) 
## ListPermissionSetsProvisionedToAccountPaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_permission_sets_provisioned_to_account")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListPermissionSetsProvisionedToAccount)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListPermissionSetsProvisionedToAccountPaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListPermissionSetsProvisionedToAccountPaginator = client.get_paginator("list_permission_sets_provisioned_to_account")
```


### paginate

Type annotations and code completion for `#!python ListPermissionSetsProvisionedToAccountPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    AccountId: str,
    ProvisioningStatus: ProvisioningStatusType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListPermissionSetsProvisionedToAccountResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ProvisioningStatusType](./literals.md#provisioningstatustype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPermissionSetsProvisionedToAccountResponseTypeDef](./type_defs.md#listpermissionsetsprovisionedtoaccountresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "AccountId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef](./type_defs.md#listpermissionsetsprovisionedtoaccountrequestlistpermissionsetsprovisionedtoaccountpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("sso-admin").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Paginator.ListTagsForResource)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sso_admin.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("sso-admin") as client:
    client: SSOAdminClient
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
```


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    InstanceArn: str,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef = {  # (1)
    "InstanceArn": ...,
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestListTagsForResourcePaginateTypeDef](./type_defs.md#listtagsforresourcerequestlisttagsforresourcepaginatetypedef) 

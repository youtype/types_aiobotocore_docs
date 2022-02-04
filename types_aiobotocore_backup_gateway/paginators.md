<a id="paginators-for-aiobotocore-backupgateway-module"></a>

# Paginators for aiobotocore BackupGateway module

> [Index](..) > [BackupGateway](.) > Paginators

Auto-generated documentation for
[BackupGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
type annotations stubs module
[types-aiobotocore-backup-gateway](https://pypi.org/project/types-aiobotocore-backup-gateway/).

- [Paginators for aiobotocore BackupGateway module](#paginators-for-aiobotocore-backupgateway-module)
  - [ListGatewaysPaginator](#listgatewayspaginator)
  - [ListHypervisorsPaginator](#listhypervisorspaginator)
  - [ListVirtualMachinesPaginator](#listvirtualmachinespaginator)

<a id="listgatewayspaginator"></a>

## ListGatewaysPaginator

Type annotations for
`aiobotocore.create_client("backup-gateway").get_paginator("list_gateways")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_backup_gateway.paginator import ListGatewaysPaginator

def get_list_gateways_paginator() -> ListGatewaysPaginator:
    return Session().create_client("backup-gateway").get_paginator("list_gateways")
```

Boto3 documentation:
[BackupGateway.Paginator.ListGateways](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways)

Arguments for `ListGatewaysPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListGatewaysPaginator.paginate` returns
`_PageIterator`\[[ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef)\].

<a id="listhypervisorspaginator"></a>

## ListHypervisorsPaginator

Type annotations for
`aiobotocore.create_client("backup-gateway").get_paginator("list_hypervisors")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_backup_gateway.paginator import ListHypervisorsPaginator

def get_list_hypervisors_paginator() -> ListHypervisorsPaginator:
    return Session().create_client("backup-gateway").get_paginator("list_hypervisors")
```

Boto3 documentation:
[BackupGateway.Paginator.ListHypervisors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors)

Arguments for `ListHypervisorsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListHypervisorsPaginator.paginate` returns
`_PageIterator`\[[ListHypervisorsOutputTypeDef](./type_defs.md#listhypervisorsoutputtypedef)\].

<a id="listvirtualmachinespaginator"></a>

## ListVirtualMachinesPaginator

Type annotations for
`aiobotocore.create_client("backup-gateway").get_paginator("list_virtual_machines")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_backup_gateway.paginator import ListVirtualMachinesPaginator

def get_list_virtual_machines_paginator() -> ListVirtualMachinesPaginator:
    return Session().create_client("backup-gateway").get_paginator("list_virtual_machines")
```

Boto3 documentation:
[BackupGateway.Paginator.ListVirtualMachines](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines)

Arguments for `ListVirtualMachinesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListVirtualMachinesPaginator.paginate` returns
`_PageIterator`\[[ListVirtualMachinesOutputTypeDef](./type_defs.md#listvirtualmachinesoutputtypedef)\].

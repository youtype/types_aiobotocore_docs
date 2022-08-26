# Paginators

> [Index](../README.md) > [BackupGateway](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [BackupGateway](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway)
    type annotations stubs module [types-aiobotocore-backup-gateway](https://pypi.org/project/types-aiobotocore-backup-gateway/).

## ListGatewaysPaginator

Type annotations and code completion for `#!python session.create_client("backup-gateway").get_paginator("list_gateways")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListGateways)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup_gateway.paginator import ListGatewaysPaginator

session = get_session()
async with session.create_client("backup-gateway") as client:  # (1)
    paginator: ListGatewaysPaginator = client.get_paginator("list_gateways")  # (2)
    async for item in paginator.paginate(...):
        item: ListGatewaysOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupGatewayClient](./client.md)
2. paginator: [ListGatewaysPaginator](./paginators.md#listgatewayspaginator)
3. item: [:material-code-braces: ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListGatewaysPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListGatewaysOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListGatewaysOutputTypeDef](./type_defs.md#listgatewaysoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListGatewaysInputListGatewaysPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListGatewaysInputListGatewaysPaginateTypeDef](./type_defs.md#listgatewaysinputlistgatewayspaginatetypedef) 
## ListHypervisorsPaginator

Type annotations and code completion for `#!python session.create_client("backup-gateway").get_paginator("list_hypervisors")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListHypervisors)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup_gateway.paginator import ListHypervisorsPaginator

session = get_session()
async with session.create_client("backup-gateway") as client:  # (1)
    paginator: ListHypervisorsPaginator = client.get_paginator("list_hypervisors")  # (2)
    async for item in paginator.paginate(...):
        item: ListHypervisorsOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupGatewayClient](./client.md)
2. paginator: [ListHypervisorsPaginator](./paginators.md#listhypervisorspaginator)
3. item: [:material-code-braces: ListHypervisorsOutputTypeDef](./type_defs.md#listhypervisorsoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListHypervisorsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListHypervisorsOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListHypervisorsOutputTypeDef](./type_defs.md#listhypervisorsoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListHypervisorsInputListHypervisorsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListHypervisorsInputListHypervisorsPaginateTypeDef](./type_defs.md#listhypervisorsinputlisthypervisorspaginatetypedef) 
## ListVirtualMachinesPaginator

Type annotations and code completion for `#!python session.create_client("backup-gateway").get_paginator("list_virtual_machines")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backup-gateway.html#BackupGateway.Paginator.ListVirtualMachines)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_backup_gateway.paginator import ListVirtualMachinesPaginator

session = get_session()
async with session.create_client("backup-gateway") as client:  # (1)
    paginator: ListVirtualMachinesPaginator = client.get_paginator("list_virtual_machines")  # (2)
    async for item in paginator.paginate(...):
        item: ListVirtualMachinesOutputTypeDef
        print(item)  # (3)
```

1. client: [BackupGatewayClient](./client.md)
2. paginator: [ListVirtualMachinesPaginator](./paginators.md#listvirtualmachinespaginator)
3. item: [:material-code-braces: ListVirtualMachinesOutputTypeDef](./type_defs.md#listvirtualmachinesoutputtypedef) 


### paginate

Type annotations and code completion for `#!python ListVirtualMachinesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVirtualMachinesOutputTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVirtualMachinesOutputTypeDef](./type_defs.md#listvirtualmachinesoutputtypedef) 


```python title="Usage example with kwargs"
kwargs: ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVirtualMachinesInputListVirtualMachinesPaginateTypeDef](./type_defs.md#listvirtualmachinesinputlistvirtualmachinespaginatetypedef) 

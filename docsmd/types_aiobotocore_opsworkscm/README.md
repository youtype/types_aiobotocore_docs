# OpsWorksCM module

> [Index](../README.md) > OpsWorksCM


!!! note ""

    Auto-generated documentation for [OpsWorksCM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#opsworkscm)
    type annotations stubs module [types-aiobotocore-opsworkscm](https://pypi.org/project/types-aiobotocore-opsworkscm/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.21.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `OpsWorksCM` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `OpsWorksCM` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[opsworkscm]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[opsworkscm]'

# standalone installation
python -m pip install types-aiobotocore-opsworkscm
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-opsworkscm
```

## Usage

Code samples can be found in [Examples](./usage.md).

## OpsWorksCMClient

Type annotations and code completion for  `#!python session.create_client("opsworkscm")` as [OpsWorksCMClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Client)

```python
# OpsWorksCMClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_opsworkscm.client import OpsWorksCMClient


session = get_session()
async with session.create_client("opsworkscm") as client:
    client: OpsWorksCMClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("opsworkscm").get_paginator("...")`.

```python
# DescribeBackupsPaginator usage example

from types_aiobotocore_opsworkscm.paginator import DescribeBackupsPaginator

def get_describe_backups_paginator() -> DescribeBackupsPaginator:
    return client.get_paginator("describe_backups"))
```

- [DescribeBackupsPaginator](./paginators.md#describebackupspaginator)
- [DescribeEventsPaginator](./paginators.md#describeeventspaginator)
- [DescribeServersPaginator](./paginators.md#describeserverspaginator)
- [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)




## Waiters

Type annotations and code completion for
[waiters](./waiters.md)
from `#!python session.create_client("opsworkscm").get_waiter("...")`.

```python
# NodeAssociatedWaiter usage example

from types_aiobotocore_opsworkscm.waiter import NodeAssociatedWaiter

def get_node_associated_waiter() -> NodeAssociatedWaiter:
    return Session().client("opsworkscm").get_waiter("node_associated")
```

- [NodeAssociatedWaiter](./waiters.md#nodeassociatedwaiter)






## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# BackupStatusType usage example

from types_aiobotocore_opsworkscm.literals import BackupStatusType

def get_value() -> BackupStatusType:
    return "DELETING"
```

- [BackupStatusType](./literals.md#backupstatustype)
- [BackupTypeType](./literals.md#backuptypetype)
- [DescribeBackupsPaginatorName](./literals.md#describebackupspaginatorname)
- [DescribeEventsPaginatorName](./literals.md#describeeventspaginatorname)
- [DescribeServersPaginatorName](./literals.md#describeserverspaginatorname)
- [ListTagsForResourcePaginatorName](./literals.md#listtagsforresourcepaginatorname)
- [MaintenanceStatusType](./literals.md#maintenancestatustype)
- [NodeAssociatedWaiterName](./literals.md#nodeassociatedwaitername)
- [NodeAssociationStatusType](./literals.md#nodeassociationstatustype)
- [ServerStatusType](./literals.md#serverstatustype)
- [OpsWorksCMServiceName](./literals.md#opsworkscmservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [WaiterName](./literals.md#waitername)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AccountAttributeTypeDef](./type_defs.md#accountattributetypedef)
- [EngineAttributeTypeDef](./type_defs.md#engineattributetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [BackupTypeDef](./type_defs.md#backuptypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteBackupRequestTypeDef](./type_defs.md#deletebackuprequesttypedef)
- [DeleteServerRequestTypeDef](./type_defs.md#deleteserverrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [DescribeBackupsRequestTypeDef](./type_defs.md#describebackupsrequesttypedef)
- [DescribeEventsRequestTypeDef](./type_defs.md#describeeventsrequesttypedef)
- [ServerEventTypeDef](./type_defs.md#servereventtypedef)
- [DescribeNodeAssociationStatusRequestTypeDef](./type_defs.md#describenodeassociationstatusrequesttypedef)
- [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)
- [DescribeServersRequestTypeDef](./type_defs.md#describeserversrequesttypedef)
- [ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef)
- [RestoreServerRequestTypeDef](./type_defs.md#restoreserverrequesttypedef)
- [UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef)
- [UpdateServerEngineAttributesRequestTypeDef](./type_defs.md#updateserverengineattributesrequesttypedef)
- [UpdateServerRequestTypeDef](./type_defs.md#updateserverrequesttypedef)
- [AssociateNodeRequestTypeDef](./type_defs.md#associatenoderequesttypedef)
- [DisassociateNodeRequestTypeDef](./type_defs.md#disassociatenoderequesttypedef)
- [ExportServerEngineAttributeRequestTypeDef](./type_defs.md#exportserverengineattributerequesttypedef)
- [ServerTypeDef](./type_defs.md#servertypedef)
- [StartMaintenanceRequestTypeDef](./type_defs.md#startmaintenancerequesttypedef)
- [AssociateNodeResponseTypeDef](./type_defs.md#associatenoderesponsetypedef)
- [DescribeAccountAttributesResponseTypeDef](./type_defs.md#describeaccountattributesresponsetypedef)
- [DescribeNodeAssociationStatusResponseTypeDef](./type_defs.md#describenodeassociationstatusresponsetypedef)
- [DisassociateNodeResponseTypeDef](./type_defs.md#disassociatenoderesponsetypedef)
- [ExportServerEngineAttributeResponseTypeDef](./type_defs.md#exportserverengineattributeresponsetypedef)
- [CreateBackupResponseTypeDef](./type_defs.md#createbackupresponsetypedef)
- [DescribeBackupsResponseTypeDef](./type_defs.md#describebackupsresponsetypedef)
- [CreateBackupRequestTypeDef](./type_defs.md#createbackuprequesttypedef)
- [CreateServerRequestTypeDef](./type_defs.md#createserverrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef)
- [DescribeBackupsRequestPaginateTypeDef](./type_defs.md#describebackupsrequestpaginatetypedef)
- [DescribeEventsRequestPaginateTypeDef](./type_defs.md#describeeventsrequestpaginatetypedef)
- [DescribeServersRequestPaginateTypeDef](./type_defs.md#describeserversrequestpaginatetypedef)
- [ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef)
- [DescribeEventsResponseTypeDef](./type_defs.md#describeeventsresponsetypedef)
- [DescribeNodeAssociationStatusRequestWaitTypeDef](./type_defs.md#describenodeassociationstatusrequestwaittypedef)
- [CreateServerResponseTypeDef](./type_defs.md#createserverresponsetypedef)
- [DescribeServersResponseTypeDef](./type_defs.md#describeserversresponsetypedef)
- [RestoreServerResponseTypeDef](./type_defs.md#restoreserverresponsetypedef)
- [StartMaintenanceResponseTypeDef](./type_defs.md#startmaintenanceresponsetypedef)
- [UpdateServerEngineAttributesResponseTypeDef](./type_defs.md#updateserverengineattributesresponsetypedef)
- [UpdateServerResponseTypeDef](./type_defs.md#updateserverresponsetypedef)


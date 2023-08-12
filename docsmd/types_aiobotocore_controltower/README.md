# ControlTower module

> [Index](../README.md) > ControlTower


!!! note ""

    Auto-generated documentation for [ControlTower](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
    type annotations stubs module [types-aiobotocore-controltower](https://pypi.org/project/types-aiobotocore-controltower/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ControlTower` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[controltower]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[controltower]'


# standalone installation
python -m pip install types-aiobotocore-controltower
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-controltower
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ControlTowerClient

Type annotations and code completion for  `#!python session.create_client("controltower")` as [ControlTowerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Client)

```python
# ControlTowerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_controltower.client import ControlTowerClient


session = get_session()
async with session.create_client("controltower") as client:
    client: ControlTowerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("controltower").get_paginator("...")`.

```python
# ListEnabledControlsPaginator usage example

from types_aiobotocore_controltower.paginator import ListEnabledControlsPaginator

def get_list_enabled_controls_paginator() -> ListEnabledControlsPaginator:
    return client.get_paginator("list_enabled_controls"))
```

- [ListEnabledControlsPaginator](./paginators.md#listenabledcontrolspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ControlOperationStatusType usage example

from types_aiobotocore_controltower.literals import ControlOperationStatusType

def get_value() -> ControlOperationStatusType:
    return "FAILED"
```

- [ControlOperationStatusType](./literals.md#controloperationstatustype)
- [ControlOperationTypeType](./literals.md#controloperationtypetype)
- [ListEnabledControlsPaginatorName](./literals.md#listenabledcontrolspaginatorname)
- [ControlTowerServiceName](./literals.md#controltowerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [ControlOperationTypeDef](./type_defs.md#controloperationtypedef)
- [DisableControlInputRequestTypeDef](./type_defs.md#disablecontrolinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [EnableControlInputRequestTypeDef](./type_defs.md#enablecontrolinputrequesttypedef)
- [EnabledControlSummaryTypeDef](./type_defs.md#enabledcontrolsummarytypedef)
- [GetControlOperationInputRequestTypeDef](./type_defs.md#getcontroloperationinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEnabledControlsInputRequestTypeDef](./type_defs.md#listenabledcontrolsinputrequesttypedef)
- [DisableControlOutputTypeDef](./type_defs.md#disablecontroloutputtypedef)
- [EnableControlOutputTypeDef](./type_defs.md#enablecontroloutputtypedef)
- [GetControlOperationOutputTypeDef](./type_defs.md#getcontroloperationoutputtypedef)
- [ListEnabledControlsOutputTypeDef](./type_defs.md#listenabledcontrolsoutputtypedef)
- [ListEnabledControlsInputListEnabledControlsPaginateTypeDef](./type_defs.md#listenabledcontrolsinputlistenabledcontrolspaginatetypedef)


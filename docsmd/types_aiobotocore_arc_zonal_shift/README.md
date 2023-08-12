# ARCZonalShift module

> [Index](../README.md) > ARCZonalShift


!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `ARCZonalShift` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[arc-zonal-shift]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[arc-zonal-shift]'


# standalone installation
python -m pip install types-aiobotocore-arc-zonal-shift
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-arc-zonal-shift
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ARCZonalShiftClient

Type annotations and code completion for  `#!python session.create_client("arc-zonal-shift")` as [ARCZonalShiftClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Client)

```python
# ARCZonalShiftClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_arc_zonal_shift.client import ARCZonalShiftClient


session = get_session()
async with session.create_client("arc-zonal-shift") as client:
    client: ARCZonalShiftClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("arc-zonal-shift").get_paginator("...")`.

```python
# ListManagedResourcesPaginator usage example

from types_aiobotocore_arc_zonal_shift.paginator import ListManagedResourcesPaginator

def get_list_managed_resources_paginator() -> ListManagedResourcesPaginator:
    return client.get_paginator("list_managed_resources"))
```

- [ListManagedResourcesPaginator](./paginators.md#listmanagedresourcespaginator)
- [ListZonalShiftsPaginator](./paginators.md#listzonalshiftspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AppliedStatusType usage example

from types_aiobotocore_arc_zonal_shift.literals import AppliedStatusType

def get_value() -> AppliedStatusType:
    return "APPLIED"
```

- [AppliedStatusType](./literals.md#appliedstatustype)
- [ListManagedResourcesPaginatorName](./literals.md#listmanagedresourcespaginatorname)
- [ListZonalShiftsPaginatorName](./literals.md#listzonalshiftspaginatorname)
- [ZonalShiftStatusType](./literals.md#zonalshiftstatustype)
- [ARCZonalShiftServiceName](./literals.md#arczonalshiftservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CancelZonalShiftRequestRequestTypeDef](./type_defs.md#cancelzonalshiftrequestrequesttypedef)
- [GetManagedResourceRequestRequestTypeDef](./type_defs.md#getmanagedresourcerequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ZonalShiftInResourceTypeDef](./type_defs.md#zonalshiftinresourcetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListManagedResourcesRequestRequestTypeDef](./type_defs.md#listmanagedresourcesrequestrequesttypedef)
- [ManagedResourceSummaryTypeDef](./type_defs.md#managedresourcesummarytypedef)
- [ListZonalShiftsRequestRequestTypeDef](./type_defs.md#listzonalshiftsrequestrequesttypedef)
- [ZonalShiftSummaryTypeDef](./type_defs.md#zonalshiftsummarytypedef)
- [StartZonalShiftRequestRequestTypeDef](./type_defs.md#startzonalshiftrequestrequesttypedef)
- [UpdateZonalShiftRequestRequestTypeDef](./type_defs.md#updatezonalshiftrequestrequesttypedef)
- [ZonalShiftTypeDef](./type_defs.md#zonalshifttypedef)
- [GetManagedResourceResponseTypeDef](./type_defs.md#getmanagedresourceresponsetypedef)
- [ListManagedResourcesRequestListManagedResourcesPaginateTypeDef](./type_defs.md#listmanagedresourcesrequestlistmanagedresourcespaginatetypedef)
- [ListZonalShiftsRequestListZonalShiftsPaginateTypeDef](./type_defs.md#listzonalshiftsrequestlistzonalshiftspaginatetypedef)
- [ListManagedResourcesResponseTypeDef](./type_defs.md#listmanagedresourcesresponsetypedef)
- [ListZonalShiftsResponseTypeDef](./type_defs.md#listzonalshiftsresponsetypedef)


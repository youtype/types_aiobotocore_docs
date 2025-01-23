# ARCZonalShift module

> [Index](../README.md) > ARCZonalShift


!!! note ""

    Auto-generated documentation for [ARCZonalShift](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#arczonalshift)
    type annotations stubs module [types-aiobotocore-arc-zonal-shift](https://pypi.org/project/types-aiobotocore-arc-zonal-shift/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `ARCZonalShift` service.
1. Use provided commands to install generated packages.



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
# ListAutoshiftsPaginator usage example

from types_aiobotocore_arc_zonal_shift.paginator import ListAutoshiftsPaginator

def get_list_autoshifts_paginator() -> ListAutoshiftsPaginator:
    return client.get_paginator("list_autoshifts"))
```

- [ListAutoshiftsPaginator](./paginators.md#listautoshiftspaginator)
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
- [AutoshiftAppliedStatusType](./literals.md#autoshiftappliedstatustype)
- [AutoshiftExecutionStatusType](./literals.md#autoshiftexecutionstatustype)
- [AutoshiftObserverNotificationStatusType](./literals.md#autoshiftobservernotificationstatustype)
- [ControlConditionTypeType](./literals.md#controlconditiontypetype)
- [ListAutoshiftsPaginatorName](./literals.md#listautoshiftspaginatorname)
- [ListManagedResourcesPaginatorName](./literals.md#listmanagedresourcespaginatorname)
- [ListZonalShiftsPaginatorName](./literals.md#listzonalshiftspaginatorname)
- [PracticeRunOutcomeType](./literals.md#practicerunoutcometype)
- [ZonalAutoshiftStatusType](./literals.md#zonalautoshiftstatustype)
- [ZonalShiftStatusType](./literals.md#zonalshiftstatustype)
- [ARCZonalShiftServiceName](./literals.md#arczonalshiftservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AutoshiftInResourceTypeDef](./type_defs.md#autoshiftinresourcetypedef)
- [AutoshiftSummaryTypeDef](./type_defs.md#autoshiftsummarytypedef)
- [CancelZonalShiftRequestRequestTypeDef](./type_defs.md#cancelzonalshiftrequestrequesttypedef)
- [ControlConditionTypeDef](./type_defs.md#controlconditiontypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [DeletePracticeRunConfigurationRequestRequestTypeDef](./type_defs.md#deletepracticerunconfigurationrequestrequesttypedef)
- [GetManagedResourceRequestRequestTypeDef](./type_defs.md#getmanagedresourcerequestrequesttypedef)
- [ZonalShiftInResourceTypeDef](./type_defs.md#zonalshiftinresourcetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAutoshiftsRequestRequestTypeDef](./type_defs.md#listautoshiftsrequestrequesttypedef)
- [ListManagedResourcesRequestRequestTypeDef](./type_defs.md#listmanagedresourcesrequestrequesttypedef)
- [ListZonalShiftsRequestRequestTypeDef](./type_defs.md#listzonalshiftsrequestrequesttypedef)
- [ZonalShiftSummaryTypeDef](./type_defs.md#zonalshiftsummarytypedef)
- [StartZonalShiftRequestRequestTypeDef](./type_defs.md#startzonalshiftrequestrequesttypedef)
- [UpdateAutoshiftObserverNotificationStatusRequestRequestTypeDef](./type_defs.md#updateautoshiftobservernotificationstatusrequestrequesttypedef)
- [UpdateZonalAutoshiftConfigurationRequestRequestTypeDef](./type_defs.md#updatezonalautoshiftconfigurationrequestrequesttypedef)
- [UpdateZonalShiftRequestRequestTypeDef](./type_defs.md#updatezonalshiftrequestrequesttypedef)
- [CreatePracticeRunConfigurationRequestRequestTypeDef](./type_defs.md#createpracticerunconfigurationrequestrequesttypedef)
- [PracticeRunConfigurationTypeDef](./type_defs.md#practicerunconfigurationtypedef)
- [UpdatePracticeRunConfigurationRequestRequestTypeDef](./type_defs.md#updatepracticerunconfigurationrequestrequesttypedef)
- [DeletePracticeRunConfigurationResponseTypeDef](./type_defs.md#deletepracticerunconfigurationresponsetypedef)
- [GetAutoshiftObserverNotificationStatusResponseTypeDef](./type_defs.md#getautoshiftobservernotificationstatusresponsetypedef)
- [ListAutoshiftsResponseTypeDef](./type_defs.md#listautoshiftsresponsetypedef)
- [UpdateAutoshiftObserverNotificationStatusResponseTypeDef](./type_defs.md#updateautoshiftobservernotificationstatusresponsetypedef)
- [UpdateZonalAutoshiftConfigurationResponseTypeDef](./type_defs.md#updatezonalautoshiftconfigurationresponsetypedef)
- [ZonalShiftTypeDef](./type_defs.md#zonalshifttypedef)
- [ManagedResourceSummaryTypeDef](./type_defs.md#managedresourcesummarytypedef)
- [ListAutoshiftsRequestPaginateTypeDef](./type_defs.md#listautoshiftsrequestpaginatetypedef)
- [ListManagedResourcesRequestPaginateTypeDef](./type_defs.md#listmanagedresourcesrequestpaginatetypedef)
- [ListZonalShiftsRequestPaginateTypeDef](./type_defs.md#listzonalshiftsrequestpaginatetypedef)
- [ListZonalShiftsResponseTypeDef](./type_defs.md#listzonalshiftsresponsetypedef)
- [CreatePracticeRunConfigurationResponseTypeDef](./type_defs.md#createpracticerunconfigurationresponsetypedef)
- [GetManagedResourceResponseTypeDef](./type_defs.md#getmanagedresourceresponsetypedef)
- [UpdatePracticeRunConfigurationResponseTypeDef](./type_defs.md#updatepracticerunconfigurationresponsetypedef)
- [ListManagedResourcesResponseTypeDef](./type_defs.md#listmanagedresourcesresponsetypedef)


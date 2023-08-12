# IoTRoboRunner module

> [Index](../README.md) > IoTRoboRunner


!!! note ""

    Auto-generated documentation for [IoTRoboRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner)
    type annotations stubs module [types-aiobotocore-iot-roborunner](https://pypi.org/project/types-aiobotocore-iot-roborunner/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `IoTRoboRunner` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[iot-roborunner]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[iot-roborunner]'


# standalone installation
python -m pip install types-aiobotocore-iot-roborunner
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-iot-roborunner
```

## Usage

Code samples can be found in [Examples](./usage.md).

## IoTRoboRunnerClient

Type annotations and code completion for  `#!python session.create_client("iot-roborunner")` as [IoTRoboRunnerClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-roborunner.html#IoTRoboRunner.Client)

```python
# IoTRoboRunnerClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_iot_roborunner.client import IoTRoboRunnerClient


session = get_session()
async with session.create_client("iot-roborunner") as client:
    client: IoTRoboRunnerClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("iot-roborunner").get_paginator("...")`.

```python
# ListDestinationsPaginator usage example

from types_aiobotocore_iot_roborunner.paginator import ListDestinationsPaginator

def get_list_destinations_paginator() -> ListDestinationsPaginator:
    return client.get_paginator("list_destinations"))
```

- [ListDestinationsPaginator](./paginators.md#listdestinationspaginator)
- [ListSitesPaginator](./paginators.md#listsitespaginator)
- [ListWorkerFleetsPaginator](./paginators.md#listworkerfleetspaginator)
- [ListWorkersPaginator](./paginators.md#listworkerspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# DestinationStateType usage example

from types_aiobotocore_iot_roborunner.literals import DestinationStateType

def get_value() -> DestinationStateType:
    return "DECOMMISSIONED"
```

- [DestinationStateType](./literals.md#destinationstatetype)
- [ListDestinationsPaginatorName](./literals.md#listdestinationspaginatorname)
- [ListSitesPaginatorName](./literals.md#listsitespaginatorname)
- [ListWorkerFleetsPaginatorName](./literals.md#listworkerfleetspaginatorname)
- [ListWorkersPaginatorName](./literals.md#listworkerspaginatorname)
- [IoTRoboRunnerServiceName](./literals.md#iotroborunnerservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [CartesianCoordinatesTypeDef](./type_defs.md#cartesiancoordinatestypedef)
- [CreateDestinationRequestRequestTypeDef](./type_defs.md#createdestinationrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateSiteRequestRequestTypeDef](./type_defs.md#createsiterequestrequesttypedef)
- [CreateWorkerFleetRequestRequestTypeDef](./type_defs.md#createworkerfleetrequestrequesttypedef)
- [OrientationTypeDef](./type_defs.md#orientationtypedef)
- [VendorPropertiesTypeDef](./type_defs.md#vendorpropertiestypedef)
- [DeleteDestinationRequestRequestTypeDef](./type_defs.md#deletedestinationrequestrequesttypedef)
- [DeleteSiteRequestRequestTypeDef](./type_defs.md#deletesiterequestrequesttypedef)
- [DeleteWorkerFleetRequestRequestTypeDef](./type_defs.md#deleteworkerfleetrequestrequesttypedef)
- [DeleteWorkerRequestRequestTypeDef](./type_defs.md#deleteworkerrequestrequesttypedef)
- [DestinationTypeDef](./type_defs.md#destinationtypedef)
- [GetDestinationRequestRequestTypeDef](./type_defs.md#getdestinationrequestrequesttypedef)
- [GetSiteRequestRequestTypeDef](./type_defs.md#getsiterequestrequesttypedef)
- [GetWorkerFleetRequestRequestTypeDef](./type_defs.md#getworkerfleetrequestrequesttypedef)
- [GetWorkerRequestRequestTypeDef](./type_defs.md#getworkerrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListDestinationsRequestRequestTypeDef](./type_defs.md#listdestinationsrequestrequesttypedef)
- [ListSitesRequestRequestTypeDef](./type_defs.md#listsitesrequestrequesttypedef)
- [SiteTypeDef](./type_defs.md#sitetypedef)
- [ListWorkerFleetsRequestRequestTypeDef](./type_defs.md#listworkerfleetsrequestrequesttypedef)
- [WorkerFleetTypeDef](./type_defs.md#workerfleettypedef)
- [ListWorkersRequestRequestTypeDef](./type_defs.md#listworkersrequestrequesttypedef)
- [UpdateDestinationRequestRequestTypeDef](./type_defs.md#updatedestinationrequestrequesttypedef)
- [UpdateSiteRequestRequestTypeDef](./type_defs.md#updatesiterequestrequesttypedef)
- [UpdateWorkerFleetRequestRequestTypeDef](./type_defs.md#updateworkerfleetrequestrequesttypedef)
- [PositionCoordinatesTypeDef](./type_defs.md#positioncoordinatestypedef)
- [CreateDestinationResponseTypeDef](./type_defs.md#createdestinationresponsetypedef)
- [CreateSiteResponseTypeDef](./type_defs.md#createsiteresponsetypedef)
- [CreateWorkerFleetResponseTypeDef](./type_defs.md#createworkerfleetresponsetypedef)
- [CreateWorkerResponseTypeDef](./type_defs.md#createworkerresponsetypedef)
- [GetDestinationResponseTypeDef](./type_defs.md#getdestinationresponsetypedef)
- [GetSiteResponseTypeDef](./type_defs.md#getsiteresponsetypedef)
- [GetWorkerFleetResponseTypeDef](./type_defs.md#getworkerfleetresponsetypedef)
- [UpdateDestinationResponseTypeDef](./type_defs.md#updatedestinationresponsetypedef)
- [UpdateSiteResponseTypeDef](./type_defs.md#updatesiteresponsetypedef)
- [UpdateWorkerFleetResponseTypeDef](./type_defs.md#updateworkerfleetresponsetypedef)
- [ListDestinationsResponseTypeDef](./type_defs.md#listdestinationsresponsetypedef)
- [ListDestinationsRequestListDestinationsPaginateTypeDef](./type_defs.md#listdestinationsrequestlistdestinationspaginatetypedef)
- [ListSitesRequestListSitesPaginateTypeDef](./type_defs.md#listsitesrequestlistsitespaginatetypedef)
- [ListWorkerFleetsRequestListWorkerFleetsPaginateTypeDef](./type_defs.md#listworkerfleetsrequestlistworkerfleetspaginatetypedef)
- [ListWorkersRequestListWorkersPaginateTypeDef](./type_defs.md#listworkersrequestlistworkerspaginatetypedef)
- [ListSitesResponseTypeDef](./type_defs.md#listsitesresponsetypedef)
- [ListWorkerFleetsResponseTypeDef](./type_defs.md#listworkerfleetsresponsetypedef)
- [CreateWorkerRequestRequestTypeDef](./type_defs.md#createworkerrequestrequesttypedef)
- [GetWorkerResponseTypeDef](./type_defs.md#getworkerresponsetypedef)
- [UpdateWorkerRequestRequestTypeDef](./type_defs.md#updateworkerrequestrequesttypedef)
- [UpdateWorkerResponseTypeDef](./type_defs.md#updateworkerresponsetypedef)
- [WorkerTypeDef](./type_defs.md#workertypedef)
- [ListWorkersResponseTypeDef](./type_defs.md#listworkersresponsetypedef)


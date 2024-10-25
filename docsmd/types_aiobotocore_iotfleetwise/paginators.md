# Paginators

> [Index](../README.md) > [IoTFleetWise](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTFleetWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise)
    type annotations stubs module [types-aiobotocore-iotfleetwise](https://pypi.org/project/types-aiobotocore-iotfleetwise/).

## GetVehicleStatusPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("get_vehicle_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.GetVehicleStatus)

```python
# GetVehicleStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import GetVehicleStatusPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: GetVehicleStatusPaginator = client.get_paginator("get_vehicle_status")  # (2)
    async for item in paginator.paginate(...):
        item: GetVehicleStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [GetVehicleStatusPaginator](./paginators.md#getvehiclestatuspaginator)
3. item: [:material-code-braces: GetVehicleStatusResponseTypeDef](./type_defs.md#getvehiclestatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetVehicleStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    vehicleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetVehicleStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetVehicleStatusResponseTypeDef](./type_defs.md#getvehiclestatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef = {  # (1)
    "vehicleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetVehicleStatusRequestGetVehicleStatusPaginateTypeDef](./type_defs.md#getvehiclestatusrequestgetvehiclestatuspaginatetypedef) 
## ListCampaignsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_campaigns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListCampaigns)

```python
# ListCampaignsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListCampaignsPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListCampaignsPaginator = client.get_paginator("list_campaigns")  # (2)
    async for item in paginator.paginate(...):
        item: ListCampaignsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
3. item: [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCampaignsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCampaignsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCampaignsRequestListCampaignsPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCampaignsRequestListCampaignsPaginateTypeDef](./type_defs.md#listcampaignsrequestlistcampaignspaginatetypedef) 
## ListDecoderManifestNetworkInterfacesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_decoder_manifest_network_interfaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces)

```python
# ListDecoderManifestNetworkInterfacesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListDecoderManifestNetworkInterfacesPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListDecoderManifestNetworkInterfacesPaginator = client.get_paginator("list_decoder_manifest_network_interfaces")  # (2)
    async for item in paginator.paginate(...):
        item: ListDecoderManifestNetworkInterfacesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListDecoderManifestNetworkInterfacesPaginator](./paginators.md#listdecodermanifestnetworkinterfacespaginator)
3. item: [:material-code-braces: ListDecoderManifestNetworkInterfacesResponseTypeDef](./type_defs.md#listdecodermanifestnetworkinterfacesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDecoderManifestNetworkInterfacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDecoderManifestNetworkInterfacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDecoderManifestNetworkInterfacesResponseTypeDef](./type_defs.md#listdecodermanifestnetworkinterfacesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDecoderManifestNetworkInterfacesRequestListDecoderManifestNetworkInterfacesPaginateTypeDef](./type_defs.md#listdecodermanifestnetworkinterfacesrequestlistdecodermanifestnetworkinterfacespaginatetypedef) 
## ListDecoderManifestSignalsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_decoder_manifest_signals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifestSignals)

```python
# ListDecoderManifestSignalsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListDecoderManifestSignalsPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListDecoderManifestSignalsPaginator = client.get_paginator("list_decoder_manifest_signals")  # (2)
    async for item in paginator.paginate(...):
        item: ListDecoderManifestSignalsResponsePaginatorTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListDecoderManifestSignalsPaginator](./paginators.md#listdecodermanifestsignalspaginator)
3. item: [:material-code-braces: ListDecoderManifestSignalsResponsePaginatorTypeDef](./type_defs.md#listdecodermanifestsignalsresponsepaginatortypedef) 


### paginate

Type annotations and code completion for `#!python ListDecoderManifestSignalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDecoderManifestSignalsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDecoderManifestSignalsResponsePaginatorTypeDef](./type_defs.md#listdecodermanifestsignalsresponsepaginatortypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDecoderManifestSignalsRequestListDecoderManifestSignalsPaginateTypeDef](./type_defs.md#listdecodermanifestsignalsrequestlistdecodermanifestsignalspaginatetypedef) 
## ListDecoderManifestsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_decoder_manifests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListDecoderManifests)

```python
# ListDecoderManifestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListDecoderManifestsPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListDecoderManifestsPaginator = client.get_paginator("list_decoder_manifests")  # (2)
    async for item in paginator.paginate(...):
        item: ListDecoderManifestsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListDecoderManifestsPaginator](./paginators.md#listdecodermanifestspaginator)
3. item: [:material-code-braces: ListDecoderManifestsResponseTypeDef](./type_defs.md#listdecodermanifestsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDecoderManifestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    modelManifestArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDecoderManifestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDecoderManifestsResponseTypeDef](./type_defs.md#listdecodermanifestsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef = {  # (1)
    "modelManifestArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDecoderManifestsRequestListDecoderManifestsPaginateTypeDef](./type_defs.md#listdecodermanifestsrequestlistdecodermanifestspaginatetypedef) 
## ListFleetsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleets)

```python
# ListFleetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListFleetsPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListFleetsPaginator = client.get_paginator("list_fleets")  # (2)
    async for item in paginator.paginate(...):
        item: ListFleetsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListFleetsPaginator](./paginators.md#listfleetspaginator)
3. item: [:material-code-braces: ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFleetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFleetsResponseTypeDef](./type_defs.md#listfleetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFleetsRequestListFleetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetsRequestListFleetsPaginateTypeDef](./type_defs.md#listfleetsrequestlistfleetspaginatetypedef) 
## ListFleetsForVehiclePaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_fleets_for_vehicle")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListFleetsForVehicle)

```python
# ListFleetsForVehiclePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListFleetsForVehiclePaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListFleetsForVehiclePaginator = client.get_paginator("list_fleets_for_vehicle")  # (2)
    async for item in paginator.paginate(...):
        item: ListFleetsForVehicleResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListFleetsForVehiclePaginator](./paginators.md#listfleetsforvehiclepaginator)
3. item: [:material-code-braces: ListFleetsForVehicleResponseTypeDef](./type_defs.md#listfleetsforvehicleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListFleetsForVehiclePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    vehicleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListFleetsForVehicleResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListFleetsForVehicleResponseTypeDef](./type_defs.md#listfleetsforvehicleresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef = {  # (1)
    "vehicleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetsForVehicleRequestListFleetsForVehiclePaginateTypeDef](./type_defs.md#listfleetsforvehiclerequestlistfleetsforvehiclepaginatetypedef) 
## ListModelManifestNodesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_model_manifest_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifestNodes)

```python
# ListModelManifestNodesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListModelManifestNodesPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListModelManifestNodesPaginator = client.get_paginator("list_model_manifest_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ListModelManifestNodesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListModelManifestNodesPaginator](./paginators.md#listmodelmanifestnodespaginator)
3. item: [:material-code-braces: ListModelManifestNodesResponseTypeDef](./type_defs.md#listmodelmanifestnodesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListModelManifestNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListModelManifestNodesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListModelManifestNodesResponseTypeDef](./type_defs.md#listmodelmanifestnodesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListModelManifestNodesRequestListModelManifestNodesPaginateTypeDef](./type_defs.md#listmodelmanifestnodesrequestlistmodelmanifestnodespaginatetypedef) 
## ListModelManifestsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_model_manifests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListModelManifests)

```python
# ListModelManifestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListModelManifestsPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListModelManifestsPaginator = client.get_paginator("list_model_manifests")  # (2)
    async for item in paginator.paginate(...):
        item: ListModelManifestsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListModelManifestsPaginator](./paginators.md#listmodelmanifestspaginator)
3. item: [:material-code-braces: ListModelManifestsResponseTypeDef](./type_defs.md#listmodelmanifestsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListModelManifestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    signalCatalogArn: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListModelManifestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListModelManifestsResponseTypeDef](./type_defs.md#listmodelmanifestsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListModelManifestsRequestListModelManifestsPaginateTypeDef = {  # (1)
    "signalCatalogArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListModelManifestsRequestListModelManifestsPaginateTypeDef](./type_defs.md#listmodelmanifestsrequestlistmodelmanifestspaginatetypedef) 
## ListSignalCatalogNodesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_signal_catalog_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogNodes)

```python
# ListSignalCatalogNodesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListSignalCatalogNodesPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListSignalCatalogNodesPaginator = client.get_paginator("list_signal_catalog_nodes")  # (2)
    async for item in paginator.paginate(...):
        item: ListSignalCatalogNodesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListSignalCatalogNodesPaginator](./paginators.md#listsignalcatalognodespaginator)
3. item: [:material-code-braces: ListSignalCatalogNodesResponseTypeDef](./type_defs.md#listsignalcatalognodesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSignalCatalogNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str,
    signalNodeType: SignalNodeTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListSignalCatalogNodesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SignalNodeTypeType](./literals.md#signalnodetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListSignalCatalogNodesResponseTypeDef](./type_defs.md#listsignalcatalognodesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSignalCatalogNodesRequestListSignalCatalogNodesPaginateTypeDef](./type_defs.md#listsignalcatalognodesrequestlistsignalcatalognodespaginatetypedef) 
## ListSignalCatalogsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_signal_catalogs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListSignalCatalogs)

```python
# ListSignalCatalogsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListSignalCatalogsPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListSignalCatalogsPaginator = client.get_paginator("list_signal_catalogs")  # (2)
    async for item in paginator.paginate(...):
        item: ListSignalCatalogsResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListSignalCatalogsPaginator](./paginators.md#listsignalcatalogspaginator)
3. item: [:material-code-braces: ListSignalCatalogsResponseTypeDef](./type_defs.md#listsignalcatalogsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListSignalCatalogsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListSignalCatalogsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListSignalCatalogsResponseTypeDef](./type_defs.md#listsignalcatalogsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSignalCatalogsRequestListSignalCatalogsPaginateTypeDef](./type_defs.md#listsignalcatalogsrequestlistsignalcatalogspaginatetypedef) 
## ListVehiclesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_vehicles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehicles)

```python
# ListVehiclesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListVehiclesPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListVehiclesPaginator = client.get_paginator("list_vehicles")  # (2)
    async for item in paginator.paginate(...):
        item: ListVehiclesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListVehiclesPaginator](./paginators.md#listvehiclespaginator)
3. item: [:material-code-braces: ListVehiclesResponseTypeDef](./type_defs.md#listvehiclesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVehiclesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    modelManifestArn: str = ...,
    attributeNames: Sequence[str] = ...,
    attributeValues: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVehiclesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVehiclesResponseTypeDef](./type_defs.md#listvehiclesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVehiclesRequestListVehiclesPaginateTypeDef = {  # (1)
    "modelManifestArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVehiclesRequestListVehiclesPaginateTypeDef](./type_defs.md#listvehiclesrequestlistvehiclespaginatetypedef) 
## ListVehiclesInFleetPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_vehicles_in_fleet")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#IoTFleetWise.Paginator.ListVehiclesInFleet)

```python
# ListVehiclesInFleetPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListVehiclesInFleetPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListVehiclesInFleetPaginator = client.get_paginator("list_vehicles_in_fleet")  # (2)
    async for item in paginator.paginate(...):
        item: ListVehiclesInFleetResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListVehiclesInFleetPaginator](./paginators.md#listvehiclesinfleetpaginator)
3. item: [:material-code-braces: ListVehiclesInFleetResponseTypeDef](./type_defs.md#listvehiclesinfleetresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListVehiclesInFleetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    fleetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListVehiclesInFleetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListVehiclesInFleetResponseTypeDef](./type_defs.md#listvehiclesinfleetresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef = {  # (1)
    "fleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVehiclesInFleetRequestListVehiclesInFleetPaginateTypeDef](./type_defs.md#listvehiclesinfleetrequestlistvehiclesinfleetpaginatetypedef) 

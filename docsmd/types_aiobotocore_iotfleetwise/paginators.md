# Paginators

> [Index](../README.md) > [IoTFleetWise](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [IoTFleetWise](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise.html#iotfleetwise)
    type annotations stubs module [types-aiobotocore-iotfleetwise](https://pypi.org/project/types-aiobotocore-iotfleetwise/).

## GetVehicleStatusPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("get_vehicle_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/GetVehicleStatus.html#IoTFleetWise.Paginator.GetVehicleStatus)

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
3. item: `AioPageIterator[GetVehicleStatusResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python GetVehicleStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    vehicleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[GetVehicleStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[GetVehicleStatusResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: GetVehicleStatusRequestPaginateTypeDef = {  # (1)
    "vehicleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetVehicleStatusRequestPaginateTypeDef](./type_defs.md#getvehiclestatusrequestpaginatetypedef)
## ListCampaignsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_campaigns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListCampaigns.html#IoTFleetWise.Paginator.ListCampaigns)

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
3. item: `AioPageIterator[ListCampaignsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListCampaignsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    status: str = ...,
    listResponseScope: ListResponseScopeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListCampaignsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListResponseScopeType](./literals.md#listresponsescopetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListCampaignsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListCampaignsRequestPaginateTypeDef = {  # (1)
    "status": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCampaignsRequestPaginateTypeDef](./type_defs.md#listcampaignsrequestpaginatetypedef)
## ListDecoderManifestNetworkInterfacesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_decoder_manifest_network_interfaces")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListDecoderManifestNetworkInterfaces.html#IoTFleetWise.Paginator.ListDecoderManifestNetworkInterfaces)

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
3. item: `AioPageIterator[ListDecoderManifestNetworkInterfacesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDecoderManifestNetworkInterfacesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDecoderManifestNetworkInterfacesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDecoderManifestNetworkInterfacesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDecoderManifestNetworkInterfacesRequestPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDecoderManifestNetworkInterfacesRequestPaginateTypeDef](./type_defs.md#listdecodermanifestnetworkinterfacesrequestpaginatetypedef)
## ListDecoderManifestSignalsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_decoder_manifest_signals")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListDecoderManifestSignals.html#IoTFleetWise.Paginator.ListDecoderManifestSignals)

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
3. item: `AioPageIterator[ListDecoderManifestSignalsResponsePaginatorTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDecoderManifestSignalsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListDecoderManifestSignalsResponsePaginatorTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListDecoderManifestSignalsResponsePaginatorTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDecoderManifestSignalsRequestPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDecoderManifestSignalsRequestPaginateTypeDef](./type_defs.md#listdecodermanifestsignalsrequestpaginatetypedef)
## ListDecoderManifestsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_decoder_manifests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListDecoderManifests.html#IoTFleetWise.Paginator.ListDecoderManifests)

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
3. item: `AioPageIterator[ListDecoderManifestsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListDecoderManifestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    modelManifestArn: str = ...,
    listResponseScope: ListResponseScopeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListDecoderManifestsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListResponseScopeType](./literals.md#listresponsescopetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListDecoderManifestsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListDecoderManifestsRequestPaginateTypeDef = {  # (1)
    "modelManifestArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDecoderManifestsRequestPaginateTypeDef](./type_defs.md#listdecodermanifestsrequestpaginatetypedef)
## ListFleetsForVehiclePaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_fleets_for_vehicle")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListFleetsForVehicle.html#IoTFleetWise.Paginator.ListFleetsForVehicle)

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
3. item: `AioPageIterator[ListFleetsForVehicleResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFleetsForVehiclePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    vehicleName: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListFleetsForVehicleResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListFleetsForVehicleResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFleetsForVehicleRequestPaginateTypeDef = {  # (1)
    "vehicleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetsForVehicleRequestPaginateTypeDef](./type_defs.md#listfleetsforvehiclerequestpaginatetypedef)
## ListFleetsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_fleets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListFleets.html#IoTFleetWise.Paginator.ListFleets)

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
3. item: `AioPageIterator[ListFleetsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListFleetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    listResponseScope: ListResponseScopeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListFleetsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListResponseScopeType](./literals.md#listresponsescopetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListFleetsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListFleetsRequestPaginateTypeDef = {  # (1)
    "listResponseScope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListFleetsRequestPaginateTypeDef](./type_defs.md#listfleetsrequestpaginatetypedef)
## ListModelManifestNodesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_model_manifest_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListModelManifestNodes.html#IoTFleetWise.Paginator.ListModelManifestNodes)

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
3. item: `AioPageIterator[ListModelManifestNodesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListModelManifestNodesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListModelManifestNodesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListModelManifestNodesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListModelManifestNodesRequestPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListModelManifestNodesRequestPaginateTypeDef](./type_defs.md#listmodelmanifestnodesrequestpaginatetypedef)
## ListModelManifestsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_model_manifests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListModelManifests.html#IoTFleetWise.Paginator.ListModelManifests)

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
3. item: `AioPageIterator[ListModelManifestsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListModelManifestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    signalCatalogArn: str = ...,
    listResponseScope: ListResponseScopeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListModelManifestsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListResponseScopeType](./literals.md#listresponsescopetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListModelManifestsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListModelManifestsRequestPaginateTypeDef = {  # (1)
    "signalCatalogArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListModelManifestsRequestPaginateTypeDef](./type_defs.md#listmodelmanifestsrequestpaginatetypedef)
## ListSignalCatalogNodesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_signal_catalog_nodes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListSignalCatalogNodes.html#IoTFleetWise.Paginator.ListSignalCatalogNodes)

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
3. item: `AioPageIterator[ListSignalCatalogNodesResponseTypeDef]`


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
) -> aiobotocore.paginate.AioPageIterator[ListSignalCatalogNodesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: SignalNodeTypeType](./literals.md#signalnodetypetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListSignalCatalogNodesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSignalCatalogNodesRequestPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSignalCatalogNodesRequestPaginateTypeDef](./type_defs.md#listsignalcatalognodesrequestpaginatetypedef)
## ListSignalCatalogsPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_signal_catalogs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListSignalCatalogs.html#IoTFleetWise.Paginator.ListSignalCatalogs)

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
3. item: `AioPageIterator[ListSignalCatalogsResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListSignalCatalogsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListSignalCatalogsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListSignalCatalogsResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListSignalCatalogsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListSignalCatalogsRequestPaginateTypeDef](./type_defs.md#listsignalcatalogsrequestpaginatetypedef)
## ListStateTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_state_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListStateTemplates.html#IoTFleetWise.Paginator.ListStateTemplates)

```python
# ListStateTemplatesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_iotfleetwise.paginator import ListStateTemplatesPaginator

session = get_session()
async with session.create_client("iotfleetwise") as client:  # (1)
    paginator: ListStateTemplatesPaginator = client.get_paginator("list_state_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListStateTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [IoTFleetWiseClient](./client.md)
2. paginator: [ListStateTemplatesPaginator](./paginators.md#liststatetemplatespaginator)
3. item: `AioPageIterator[ListStateTemplatesResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListStateTemplatesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    listResponseScope: ListResponseScopeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListStateTemplatesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListResponseScopeType](./literals.md#listresponsescopetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListStateTemplatesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListStateTemplatesRequestPaginateTypeDef = {  # (1)
    "listResponseScope": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListStateTemplatesRequestPaginateTypeDef](./type_defs.md#liststatetemplatesrequestpaginatetypedef)
## ListVehiclesInFleetPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_vehicles_in_fleet")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListVehiclesInFleet.html#IoTFleetWise.Paginator.ListVehiclesInFleet)

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
3. item: `AioPageIterator[ListVehiclesInFleetResponseTypeDef]`


### paginate

Type annotations and code completion for `#!python ListVehiclesInFleetPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    fleetId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[ListVehiclesInFleetResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[ListVehiclesInFleetResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListVehiclesInFleetRequestPaginateTypeDef = {  # (1)
    "fleetId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVehiclesInFleetRequestPaginateTypeDef](./type_defs.md#listvehiclesinfleetrequestpaginatetypedef)
## ListVehiclesPaginator

Type annotations and code completion for `#!python session.create_client("iotfleetwise").get_paginator("list_vehicles")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleetwise/paginator/ListVehicles.html#IoTFleetWise.Paginator.ListVehicles)

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
3. item: `AioPageIterator[ListVehiclesResponseTypeDef]`


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
    listResponseScope: ListResponseScopeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListVehiclesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ListResponseScopeType](./literals.md#listresponsescopetype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListVehiclesResponseTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListVehiclesRequestPaginateTypeDef = {  # (1)
    "modelManifestArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListVehiclesRequestPaginateTypeDef](./type_defs.md#listvehiclesrequestpaginatetypedef)

# Paginators

> [Index](../README.md) > [ConnectCampaignServiceV2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ConnectCampaignServiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2.html#connectcampaignservicev2)
    type annotations stubs module [types-aiobotocore-connectcampaignsv2](https://pypi.org/project/types-aiobotocore-connectcampaignsv2/).

## ListCampaignsPaginator

Type annotations and code completion for `#!python session.create_client("connectcampaignsv2").get_paginator("list_campaigns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2/paginator/ListCampaigns.html#ConnectCampaignServiceV2.Paginator.ListCampaigns)

```python
# ListCampaignsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcampaignsv2.paginator import ListCampaignsPaginator

session = get_session()
async with session.create_client("connectcampaignsv2") as client:  # (1)
    paginator: ListCampaignsPaginator = client.get_paginator("list_campaigns")  # (2)
    async for item in paginator.paginate(...):
        item: ListCampaignsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCampaignServiceV2Client](./client.md)
2. paginator: [ListCampaignsPaginator](./paginators.md#listcampaignspaginator)
3. item: [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCampaignsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    filters: CampaignFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListCampaignsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: CampaignFiltersTypeDef](./type_defs.md#campaignfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListCampaignsRequestPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCampaignsRequestPaginateTypeDef](./type_defs.md#listcampaignsrequestpaginatetypedef) 
## ListConnectInstanceIntegrationsPaginator

Type annotations and code completion for `#!python session.create_client("connectcampaignsv2").get_paginator("list_connect_instance_integrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaignsv2/paginator/ListConnectInstanceIntegrations.html#ConnectCampaignServiceV2.Paginator.ListConnectInstanceIntegrations)

```python
# ListConnectInstanceIntegrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_connectcampaignsv2.paginator import ListConnectInstanceIntegrationsPaginator

session = get_session()
async with session.create_client("connectcampaignsv2") as client:  # (1)
    paginator: ListConnectInstanceIntegrationsPaginator = client.get_paginator("list_connect_instance_integrations")  # (2)
    async for item in paginator.paginate(...):
        item: ListConnectInstanceIntegrationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConnectCampaignServiceV2Client](./client.md)
2. paginator: [ListConnectInstanceIntegrationsPaginator](./paginators.md#listconnectinstanceintegrationspaginator)
3. item: [:material-code-braces: ListConnectInstanceIntegrationsResponseTypeDef](./type_defs.md#listconnectinstanceintegrationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConnectInstanceIntegrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    connectInstanceId: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConnectInstanceIntegrationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConnectInstanceIntegrationsResponseTypeDef](./type_defs.md#listconnectinstanceintegrationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConnectInstanceIntegrationsRequestPaginateTypeDef = {  # (1)
    "connectInstanceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConnectInstanceIntegrationsRequestPaginateTypeDef](./type_defs.md#listconnectinstanceintegrationsrequestpaginatetypedef) 

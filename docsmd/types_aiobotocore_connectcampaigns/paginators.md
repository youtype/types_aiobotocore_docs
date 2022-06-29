# Paginators

> [Index](../README.md) > [ConnectCampaignService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ConnectCampaignService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService)
    type annotations stubs module [types-aiobotocore-connectcampaigns](https://pypi.org/project/types-aiobotocore-connectcampaigns/).

## ListCampaignsPaginator

Type annotations and code completion for `#!python session.create_client("connectcampaigns").get_paginator("list_campaigns")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcampaigns.html#ConnectCampaignService.Paginator.ListCampaigns)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_connectcampaigns.paginator import ListCampaignsPaginator

session = get_session()
async with session.create_client("connectcampaigns") as client:
    client: ConnectCampaignServiceClient
    paginator: ListCampaignsPaginator = client.get_paginator("list_campaigns")
```


### paginate

Type annotations and code completion for `#!python ListCampaignsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    filters: CampaignFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListCampaignsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: CampaignFiltersTypeDef](./type_defs.md#campaignfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListCampaignsResponseTypeDef](./type_defs.md#listcampaignsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCampaignsRequestListCampaignsPaginateTypeDef = {  # (1)
    "filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCampaignsRequestListCampaignsPaginateTypeDef](./type_defs.md#listcampaignsrequestlistcampaignspaginatetypedef) 

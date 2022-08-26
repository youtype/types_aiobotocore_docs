# Paginators

> [Index](../README.md) > [PinpointEmail](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PinpointEmail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail)
    type annotations stubs module [types-aiobotocore-pinpoint-email](https://pypi.org/project/types-aiobotocore-pinpoint-email/).

## GetDedicatedIpsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("get_dedicated_ips")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.GetDedicatedIps)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import GetDedicatedIpsPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:  # (1)
    paginator: GetDedicatedIpsPaginator = client.get_paginator("get_dedicated_ips")  # (2)
    async for item in paginator.paginate(...):
        item: GetDedicatedIpsResponseTypeDef
        print(item)  # (3)
```

1. client: [PinpointEmailClient](./client.md)
2. paginator: [GetDedicatedIpsPaginator](./paginators.md#getdedicatedipspaginator)
3. item: [:material-code-braces: GetDedicatedIpsResponseTypeDef](./type_defs.md#getdedicatedipsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetDedicatedIpsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PoolName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[GetDedicatedIpsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDedicatedIpsResponseTypeDef](./type_defs.md#getdedicatedipsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = {  # (1)
    "PoolName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef](./type_defs.md#getdedicatedipsrequestgetdedicatedipspaginatetypedef) 
## ListConfigurationSetsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("list_configuration_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListConfigurationSets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import ListConfigurationSetsPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:  # (1)
    paginator: ListConfigurationSetsPaginator = client.get_paginator("list_configuration_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [PinpointEmailClient](./client.md)
2. paginator: [ListConfigurationSetsPaginator](./paginators.md#listconfigurationsetspaginator)
3. item: [:material-code-braces: ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConfigurationSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef](./type_defs.md#listconfigurationsetsrequestlistconfigurationsetspaginatetypedef) 
## ListDedicatedIpPoolsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("list_dedicated_ip_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDedicatedIpPools)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import ListDedicatedIpPoolsPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:  # (1)
    paginator: ListDedicatedIpPoolsPaginator = client.get_paginator("list_dedicated_ip_pools")  # (2)
    async for item in paginator.paginate(...):
        item: ListDedicatedIpPoolsResponseTypeDef
        print(item)  # (3)
```

1. client: [PinpointEmailClient](./client.md)
2. paginator: [ListDedicatedIpPoolsPaginator](./paginators.md#listdedicatedippoolspaginator)
3. item: [:material-code-braces: ListDedicatedIpPoolsResponseTypeDef](./type_defs.md#listdedicatedippoolsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDedicatedIpPoolsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDedicatedIpPoolsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDedicatedIpPoolsResponseTypeDef](./type_defs.md#listdedicatedippoolsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef](./type_defs.md#listdedicatedippoolsrequestlistdedicatedippoolspaginatetypedef) 
## ListDeliverabilityTestReportsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("list_deliverability_test_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListDeliverabilityTestReports)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import ListDeliverabilityTestReportsPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:  # (1)
    paginator: ListDeliverabilityTestReportsPaginator = client.get_paginator("list_deliverability_test_reports")  # (2)
    async for item in paginator.paginate(...):
        item: ListDeliverabilityTestReportsResponseTypeDef
        print(item)  # (3)
```

1. client: [PinpointEmailClient](./client.md)
2. paginator: [ListDeliverabilityTestReportsPaginator](./paginators.md#listdeliverabilitytestreportspaginator)
3. item: [:material-code-braces: ListDeliverabilityTestReportsResponseTypeDef](./type_defs.md#listdeliverabilitytestreportsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDeliverabilityTestReportsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListDeliverabilityTestReportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeliverabilityTestReportsResponseTypeDef](./type_defs.md#listdeliverabilitytestreportsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef](./type_defs.md#listdeliverabilitytestreportsrequestlistdeliverabilitytestreportspaginatetypedef) 
## ListEmailIdentitiesPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("list_email_identities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Paginator.ListEmailIdentities)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.paginator import ListEmailIdentitiesPaginator

session = get_session()
async with session.create_client("pinpoint-email") as client:  # (1)
    paginator: ListEmailIdentitiesPaginator = client.get_paginator("list_email_identities")  # (2)
    async for item in paginator.paginate(...):
        item: ListEmailIdentitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [PinpointEmailClient](./client.md)
2. paginator: [ListEmailIdentitiesPaginator](./paginators.md#listemailidentitiespaginator)
3. item: [:material-code-braces: ListEmailIdentitiesResponseTypeDef](./type_defs.md#listemailidentitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListEmailIdentitiesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListEmailIdentitiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEmailIdentitiesResponseTypeDef](./type_defs.md#listemailidentitiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef](./type_defs.md#listemailidentitiesrequestlistemailidentitiespaginatetypedef) 

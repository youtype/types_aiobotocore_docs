# Paginators

> [Index](../README.md) > [PinpointEmail](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PinpointEmail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#pinpointemail)
    type annotations stubs module [types-aiobotocore-pinpoint-email](https://pypi.org/project/types-aiobotocore-pinpoint-email/).

## GetDedicatedIpsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("get_dedicated_ips")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email/paginator/GetDedicatedIps.html#PinpointEmail.Paginator.GetDedicatedIps)

```python
# GetDedicatedIpsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PoolName: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetDedicatedIpsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetDedicatedIpsResponseTypeDef](./type_defs.md#getdedicatedipsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetDedicatedIpsRequestPaginateTypeDef = {  # (1)
    "PoolName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetDedicatedIpsRequestPaginateTypeDef](./type_defs.md#getdedicatedipsrequestpaginatetypedef) 
## ListConfigurationSetsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("list_configuration_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email/paginator/ListConfigurationSets.html#PinpointEmail.Paginator.ListConfigurationSets)

```python
# ListConfigurationSetsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListConfigurationSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationSetsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationSetsRequestPaginateTypeDef](./type_defs.md#listconfigurationsetsrequestpaginatetypedef) 
## ListDedicatedIpPoolsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("list_dedicated_ip_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email/paginator/ListDedicatedIpPools.html#PinpointEmail.Paginator.ListDedicatedIpPools)

```python
# ListDedicatedIpPoolsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDedicatedIpPoolsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDedicatedIpPoolsResponseTypeDef](./type_defs.md#listdedicatedippoolsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDedicatedIpPoolsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDedicatedIpPoolsRequestPaginateTypeDef](./type_defs.md#listdedicatedippoolsrequestpaginatetypedef) 
## ListDeliverabilityTestReportsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("list_deliverability_test_reports")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email/paginator/ListDeliverabilityTestReports.html#PinpointEmail.Paginator.ListDeliverabilityTestReports)

```python
# ListDeliverabilityTestReportsPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListDeliverabilityTestReportsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListDeliverabilityTestReportsResponseTypeDef](./type_defs.md#listdeliverabilitytestreportsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDeliverabilityTestReportsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDeliverabilityTestReportsRequestPaginateTypeDef](./type_defs.md#listdeliverabilitytestreportsrequestpaginatetypedef) 
## ListEmailIdentitiesPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-email").get_paginator("list_email_identities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email/paginator/ListEmailIdentities.html#PinpointEmail.Paginator.ListEmailIdentities)

```python
# ListEmailIdentitiesPaginator usage example

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

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListEmailIdentitiesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListEmailIdentitiesResponseTypeDef](./type_defs.md#listemailidentitiesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListEmailIdentitiesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListEmailIdentitiesRequestPaginateTypeDef](./type_defs.md#listemailidentitiesrequestpaginatetypedef) 

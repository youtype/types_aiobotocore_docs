# Examples

> [Index](../README.md) > [PinpointEmail](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [PinpointEmail](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#pinpointemail)
    type annotations stubs module [types-aiobotocore-pinpoint-email](https://pypi.org/project/types-aiobotocore-pinpoint-email/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[pinpoint-email]` package installed.

Write your `PinpointEmail` code as usual,
type checking and code completion should work out of the box.



```python
# PinpointEmailClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pinpoint-email") as client:  # (1)
    result = await client.create_deliverability_test_report()  # (2)
```

1. client: [PinpointEmailClient](./client.md)
2. result: [:material-code-braces: CreateDeliverabilityTestReportResponseTypeDef](./type_defs.md#createdeliverabilitytestreportresponsetypedef) 



```python
# GetDedicatedIpsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("pinpoint-email") as client:  # (1)
    paginator = client.get_paginator("get_dedicated_ips")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [PinpointEmailClient](./client.md)
2. paginator: [GetDedicatedIpsPaginator](./paginators.md#getdedicatedipspaginator)
3. item: [:material-code-braces: GetDedicatedIpsResponseTypeDef](./type_defs.md#getdedicatedipsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[pinpoint-email]`
or a standalone `types_aiobotocore_pinpoint_email` package, you have to explicitly specify
`client: PinpointEmailClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# PinpointEmailClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.client import PinpointEmailClient
from types_aiobotocore_pinpoint_email.type_defs import CreateDeliverabilityTestReportResponseTypeDef
from types_aiobotocore_pinpoint_email.type_defs import CreateDeliverabilityTestReportRequestTypeDef


session = get_session()

async with session.create_client("pinpoint-email") as client:
    client: PinpointEmailClient
    kwargs: CreateDeliverabilityTestReportRequestTypeDef = {...}
    result: CreateDeliverabilityTestReportResponseTypeDef = await client.create_deliverability_test_report(**kwargs)
```



```python
# GetDedicatedIpsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_email.client import PinpointEmailClient
from types_aiobotocore_pinpoint_email.paginator import GetDedicatedIpsPaginator
from types_aiobotocore_pinpoint_email.type_defs import GetDedicatedIpsResponseTypeDef


session = get_session()

async with session.create_client("pinpoint-email") as client:
    client: PinpointEmailClient
    paginator: GetDedicatedIpsPaginator = client.get_paginator("get_dedicated_ips")
    async for item in paginator.paginate(...):
        item: GetDedicatedIpsResponseTypeDef
        print(item)
```



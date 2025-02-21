# Examples

> [Index](../README.md) > [CloudTrailDataService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudTrailDataService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#cloudtraildataservice)
    type annotations stubs module [types-aiobotocore-cloudtrail-data](https://pypi.org/project/types-aiobotocore-cloudtrail-data/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cloudtrail-data]` package installed.

Write your `CloudTrailDataService` code as usual,
type checking and code completion should work out of the box.



```python
# CloudTrailDataServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudtrail-data") as client:  # (1)
    result = await client.put_audit_events()  # (2)
```

1. client: [CloudTrailDataServiceClient](./client.md)
2. result: [:material-code-braces: PutAuditEventsResponseTypeDef](./type_defs.md#putauditeventsresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[cloudtrail-data]`
or a standalone `types_aiobotocore_cloudtrail_data` package, you have to explicitly specify
`client: CloudTrailDataServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudTrailDataServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudtrail_data.client import CloudTrailDataServiceClient
from types_aiobotocore_cloudtrail_data.type_defs import PutAuditEventsResponseTypeDef
from types_aiobotocore_cloudtrail_data.type_defs import PutAuditEventsRequestTypeDef


session = get_session()

async with session.create_client("cloudtrail-data") as client:
    client: CloudTrailDataServiceClient
    kwargs: PutAuditEventsRequestTypeDef = {...}
    result: PutAuditEventsResponseTypeDef = await client.put_audit_events(**kwargs)
```





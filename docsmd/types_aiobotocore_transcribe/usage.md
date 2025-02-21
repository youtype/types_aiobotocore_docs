# Examples

> [Index](../README.md) > [TranscribeService](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [TranscribeService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transcribe.html#transcribeservice)
    type annotations stubs module [types-aiobotocore-transcribe](https://pypi.org/project/types-aiobotocore-transcribe/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[transcribe]` package installed.

Write your `TranscribeService` code as usual,
type checking and code completion should work out of the box.



```python
# TranscribeServiceClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("transcribe") as client:  # (1)
    result = await client.create_call_analytics_category()  # (2)
```

1. client: [TranscribeServiceClient](./client.md)
2. result: [:material-code-braces: CreateCallAnalyticsCategoryResponseTypeDef](./type_defs.md#createcallanalyticscategoryresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[transcribe]`
or a standalone `types_aiobotocore_transcribe` package, you have to explicitly specify
`client: TranscribeServiceClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TranscribeServiceClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_transcribe.client import TranscribeServiceClient
from types_aiobotocore_transcribe.type_defs import CreateCallAnalyticsCategoryResponseTypeDef
from types_aiobotocore_transcribe.type_defs import CreateCallAnalyticsCategoryRequestTypeDef


session = get_session()

async with session.create_client("transcribe") as client:
    client: TranscribeServiceClient
    kwargs: CreateCallAnalyticsCategoryRequestTypeDef = {...}
    result: CreateCallAnalyticsCategoryResponseTypeDef = await client.create_call_analytics_category(**kwargs)
```





# Examples

> [Index](../README.md) > [AppConfigData](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppConfigData](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#appconfigdata)
    type annotations stubs module [types-aiobotocore-appconfigdata](https://pypi.org/project/types-aiobotocore-appconfigdata/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[appconfigdata]` package installed.

Write your `AppConfigData` code as usual,
type checking and code completion should work out of the box.



```python
# AppConfigDataClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("appconfigdata") as client:  # (1)
    result = await client.get_latest_configuration()  # (2)
```

1. client: [AppConfigDataClient](./client.md)
2. result: [:material-code-braces: GetLatestConfigurationResponseTypeDef](./type_defs.md#getlatestconfigurationresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[appconfigdata]`
or a standalone `types_aiobotocore_appconfigdata` package, you have to explicitly specify
`client: AppConfigDataClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AppConfigDataClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_appconfigdata.client import AppConfigDataClient
from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationResponseTypeDef
from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationRequestTypeDef


session = get_session()

async with session.create_client("appconfigdata") as client:
    client: AppConfigDataClient
    kwargs: GetLatestConfigurationRequestTypeDef = {...}
    result: GetLatestConfigurationResponseTypeDef = await client.get_latest_configuration(**kwargs)
```





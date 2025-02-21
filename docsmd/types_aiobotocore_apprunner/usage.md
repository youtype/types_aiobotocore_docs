# Examples

> [Index](../README.md) > [AppRunner](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [AppRunner](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apprunner.html#apprunner)
    type annotations stubs module [types-aiobotocore-apprunner](https://pypi.org/project/types-aiobotocore-apprunner/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[apprunner]` package installed.

Write your `AppRunner` code as usual,
type checking and code completion should work out of the box.



```python
# AppRunnerClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("apprunner") as client:  # (1)
    result = await client.associate_custom_domain()  # (2)
```

1. client: [AppRunnerClient](./client.md)
2. result: [:material-code-braces: AssociateCustomDomainResponseTypeDef](./type_defs.md#associatecustomdomainresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[apprunner]`
or a standalone `types_aiobotocore_apprunner` package, you have to explicitly specify
`client: AppRunnerClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# AppRunnerClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_apprunner.client import AppRunnerClient
from types_aiobotocore_apprunner.type_defs import AssociateCustomDomainResponseTypeDef
from types_aiobotocore_apprunner.type_defs import AssociateCustomDomainRequestTypeDef


session = get_session()

async with session.create_client("apprunner") as client:
    client: AppRunnerClient
    kwargs: AssociateCustomDomainRequestTypeDef = {...}
    result: AssociateCustomDomainResponseTypeDef = await client.associate_custom_domain(**kwargs)
```





# Examples

> [Index](../README.md) > [CloudSearch](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CloudSearch](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearch.html#cloudsearch)
    type annotations stubs module [types-aiobotocore-cloudsearch](https://pypi.org/project/types-aiobotocore-cloudsearch/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[cloudsearch]` package installed.

Write your `CloudSearch` code as usual,
type checking and code completion should work out of the box.



```python
# CloudSearchClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("cloudsearch") as client:  # (1)
    result = await client.build_suggesters()  # (2)
```

1. client: [CloudSearchClient](./client.md)
2. result: [:material-code-braces: BuildSuggestersResponseTypeDef](./type_defs.md#buildsuggestersresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[cloudsearch]`
or a standalone `types_aiobotocore_cloudsearch` package, you have to explicitly specify
`client: CloudSearchClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CloudSearchClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_cloudsearch.client import CloudSearchClient
from types_aiobotocore_cloudsearch.type_defs import BuildSuggestersResponseTypeDef
from types_aiobotocore_cloudsearch.type_defs import BuildSuggestersRequestTypeDef


session = get_session()

async with session.create_client("cloudsearch") as client:
    client: CloudSearchClient
    kwargs: BuildSuggestersRequestTypeDef = {...}
    result: BuildSuggestersResponseTypeDef = await client.build_suggesters(**kwargs)
```





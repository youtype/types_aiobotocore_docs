# Examples

> [Index](../README.md) > [Kendra](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Kendra](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra.html#kendra)
    type annotations stubs module [types-aiobotocore-kendra](https://pypi.org/project/types-aiobotocore-kendra/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[kendra]` package installed.

Write your `Kendra` code as usual,
type checking and code completion should work out of the box.



```python
# KendraClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("kendra") as client:  # (1)
    result = await client.associate_entities_to_experience()  # (2)
```

1. client: [KendraClient](./client.md)
2. result: [:material-code-braces: AssociateEntitiesToExperienceResponseTypeDef](./type_defs.md#associateentitiestoexperienceresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[kendra]`
or a standalone `types_aiobotocore_kendra` package, you have to explicitly specify
`client: KendraClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# KendraClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_kendra.client import KendraClient
from types_aiobotocore_kendra.type_defs import AssociateEntitiesToExperienceResponseTypeDef
from types_aiobotocore_kendra.type_defs import AssociateEntitiesToExperienceRequestTypeDef


session = get_session()

async with session.create_client("kendra") as client:
    client: KendraClient
    kwargs: AssociateEntitiesToExperienceRequestTypeDef = {...}
    result: AssociateEntitiesToExperienceResponseTypeDef = await client.associate_entities_to_experience(**kwargs)
```





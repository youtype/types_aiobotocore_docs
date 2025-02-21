# Examples

> [Index](../README.md) > [OpenSearchIngestion](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [OpenSearchIngestion](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#opensearchingestion)
    type annotations stubs module [types-aiobotocore-osis](https://pypi.org/project/types-aiobotocore-osis/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[osis]` package installed.

Write your `OpenSearchIngestion` code as usual,
type checking and code completion should work out of the box.



```python
# OpenSearchIngestionClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("osis") as client:  # (1)
    result = await client.create_pipeline()  # (2)
```

1. client: [OpenSearchIngestionClient](./client.md)
2. result: [:material-code-braces: CreatePipelineResponseTypeDef](./type_defs.md#createpipelineresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[osis]`
or a standalone `types_aiobotocore_osis` package, you have to explicitly specify
`client: OpenSearchIngestionClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# OpenSearchIngestionClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_osis.client import OpenSearchIngestionClient
from types_aiobotocore_osis.type_defs import CreatePipelineResponseTypeDef
from types_aiobotocore_osis.type_defs import CreatePipelineRequestTypeDef


session = get_session()

async with session.create_client("osis") as client:
    client: OpenSearchIngestionClient
    kwargs: CreatePipelineRequestTypeDef = {...}
    result: CreatePipelineResponseTypeDef = await client.create_pipeline(**kwargs)
```





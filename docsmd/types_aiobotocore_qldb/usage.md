# Examples

> [Index](../README.md) > [QLDB](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [QLDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb.html#qldb)
    type annotations stubs module [types-aiobotocore-qldb](https://pypi.org/project/types-aiobotocore-qldb/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[qldb]` package installed.

Write your `QLDB` code as usual,
type checking and code completion should work out of the box.



```python
# QLDBClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("qldb") as client:  # (1)
    result = await client.cancel_journal_kinesis_stream()  # (2)
```

1. client: [QLDBClient](./client.md)
2. result: [:material-code-braces: CancelJournalKinesisStreamResponseTypeDef](./type_defs.md#canceljournalkinesisstreamresponsetypedef) 






### Explicit type annotations

With `types-aiobotocore-lite[qldb]`
or a standalone `types_aiobotocore_qldb` package, you have to explicitly specify
`client: QLDBClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# QLDBClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_qldb.client import QLDBClient
from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamResponseTypeDef
from types_aiobotocore_qldb.type_defs import CancelJournalKinesisStreamRequestTypeDef


session = get_session()

async with session.create_client("qldb") as client:
    client: QLDBClient
    kwargs: CancelJournalKinesisStreamRequestTypeDef = {...}
    result: CancelJournalKinesisStreamResponseTypeDef = await client.cancel_journal_kinesis_stream(**kwargs)
```





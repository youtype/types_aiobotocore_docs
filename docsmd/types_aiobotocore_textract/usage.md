# Examples

> [Index](../README.md) > [Textract](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Textract](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/textract.html#textract)
    type annotations stubs module [types-aiobotocore-textract](https://pypi.org/project/types-aiobotocore-textract/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[textract]` package installed.

Write your `Textract` code as usual,
type checking and code completion should work out of the box.



```python
# TextractClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("textract") as client:  # (1)
    result = await client.analyze_document()  # (2)
```

1. client: [TextractClient](./client.md)
2. result: [:material-code-braces: AnalyzeDocumentResponseTypeDef](./type_defs.md#analyzedocumentresponsetypedef) 



```python
# ListAdapterVersionsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("textract") as client:  # (1)
    paginator = client.get_paginator("list_adapter_versions")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [TextractClient](./client.md)
2. paginator: [ListAdapterVersionsPaginator](./paginators.md#listadapterversionspaginator)
3. item: [:material-code-braces: ListAdapterVersionsResponseTypeDef](./type_defs.md#listadapterversionsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[textract]`
or a standalone `types_aiobotocore_textract` package, you have to explicitly specify
`client: TextractClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# TextractClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_textract.client import TextractClient
from types_aiobotocore_textract.type_defs import AnalyzeDocumentResponseTypeDef
from types_aiobotocore_textract.type_defs import AnalyzeDocumentRequestTypeDef


session = get_session()

async with session.create_client("textract") as client:
    client: TextractClient
    kwargs: AnalyzeDocumentRequestTypeDef = {...}
    result: AnalyzeDocumentResponseTypeDef = await client.analyze_document(**kwargs)
```



```python
# ListAdapterVersionsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_textract.client import TextractClient
from types_aiobotocore_textract.paginator import ListAdapterVersionsPaginator
from types_aiobotocore_textract.type_defs import ListAdapterVersionsResponseTypeDef


session = get_session()

async with session.create_client("textract") as client:
    client: TextractClient
    paginator: ListAdapterVersionsPaginator = client.get_paginator("list_adapter_versions")
    async for item in paginator.paginate(...):
        item: ListAdapterVersionsResponseTypeDef
        print(item)
```



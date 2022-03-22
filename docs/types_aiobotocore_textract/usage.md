<a id="examples-for-aiobotocore-textract-module"></a>

# Examples for aiobotocore Textract module

> [Index](../README.md) > [Textract](./README.md) > Examples

- [Examples for aiobotocore Textract module](#examples-for-aiobotocore-textract-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[textract]` package installed.

Write your `Textract` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type TextractClient
# and provides type checking and code completion
async with session.create_client("textract") as client:
    
    # result has type AnalyzeDocumentResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.analyze_document()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[textract]` or a standalone
`types_aiobotocore_textract` package, you have to explicitly specify
`client: TextractClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_textract.client import TextractClient
from types_aiobotocore_textract.type_defs import AnalyzeDocumentResponseTypeDef






session = get_session()

async with session.create_client("textract") as client:
    client: TextractClient

    
    result: AnalyzeDocumentResponseTypeDef = client.analyze_document()
    

    

    
```

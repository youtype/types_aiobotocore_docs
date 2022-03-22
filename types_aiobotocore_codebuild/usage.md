<a id="examples-for-aiobotocore-codebuild-module"></a>

# Examples for aiobotocore CodeBuild module

> [Index](../README.md) > [CodeBuild](./README.md) > Examples

- [Examples for aiobotocore CodeBuild module](#examples-for-aiobotocore-codebuild-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codebuild]` package installed.

Write your `CodeBuild` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodeBuildClient
# and provides type checking and code completion
async with session.create_client("codebuild") as client:
    
    # result has type BatchDeleteBuildsOutputTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.batch_delete_builds()
    

    
    # paginator has type DescribeCodeCoveragesPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_code_coverages")
    async for item in paginator.paginate(...):
        # item has type DescribeCodeCoveragesOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codebuild]` or a standalone
`types_aiobotocore_codebuild` package, you have to explicitly specify
`client: CodeBuildClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codebuild.client import CodeBuildClient
from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsOutputTypeDef
from types_aiobotocore_codebuild.paginator import DescribeCodeCoveragesPaginator

from types_aiobotocore_codebuild.literals import PaginatorName



session = get_session()

async with session.create_client("codebuild") as client:
    client: CodeBuildClient

    
    result: BatchDeleteBuildsOutputTypeDef = client.batch_delete_builds()
    

    
    paginator_name: PaginatorName = "describe_code_coverages"
    paginator: DescribeCodeCoveragesPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribeCodeCoveragesOutputTypeDef
        print(item)
    

    
```

# Examples

> [Index](../README.md) > [CodeBuild](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [CodeBuild](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codebuild.html#codebuild)
    type annotations stubs module [types-aiobotocore-codebuild](https://pypi.org/project/types-aiobotocore-codebuild/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[codebuild]` package installed.

Write your `CodeBuild` code as usual,
type checking and code completion should work out of the box.



```python
# CodeBuildClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codebuild") as client:  # (1)
    result = await client.batch_delete_builds()  # (2)
```

1. client: [CodeBuildClient](./client.md)
2. result: [:material-code-braces: BatchDeleteBuildsOutputTypeDef](./type_defs.md#batchdeletebuildsoutputtypedef) 



```python
# DescribeCodeCoveragesPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("codebuild") as client:  # (1)
    paginator = client.get_paginator("describe_code_coverages")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [CodeBuildClient](./client.md)
2. paginator: [DescribeCodeCoveragesPaginator](./paginators.md#describecodecoveragespaginator)
3. item: [:material-code-braces: DescribeCodeCoveragesOutputTypeDef](./type_defs.md#describecodecoveragesoutputtypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[codebuild]`
or a standalone `types_aiobotocore_codebuild` package, you have to explicitly specify
`client: CodeBuildClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# CodeBuildClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codebuild.client import CodeBuildClient
from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsOutputTypeDef
from types_aiobotocore_codebuild.type_defs import BatchDeleteBuildsInputTypeDef


session = get_session()

async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    kwargs: BatchDeleteBuildsInputTypeDef = {...}
    result: BatchDeleteBuildsOutputTypeDef = await client.batch_delete_builds(**kwargs)
```



```python
# DescribeCodeCoveragesPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_codebuild.client import CodeBuildClient
from types_aiobotocore_codebuild.paginator import DescribeCodeCoveragesPaginator
from types_aiobotocore_codebuild.type_defs import DescribeCodeCoveragesOutputTypeDef


session = get_session()

async with session.create_client("codebuild") as client:
    client: CodeBuildClient
    paginator: DescribeCodeCoveragesPaginator = client.get_paginator("describe_code_coverages")
    async for item in paginator.paginate(...):
        item: DescribeCodeCoveragesOutputTypeDef
        print(item)
```



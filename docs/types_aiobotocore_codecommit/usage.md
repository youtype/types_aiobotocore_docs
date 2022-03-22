<a id="examples-for-aiobotocore-codecommit-module"></a>

# Examples for aiobotocore CodeCommit module

> [Index](../README.md) > [CodeCommit](./README.md) > Examples

- [Examples for aiobotocore CodeCommit module](#examples-for-aiobotocore-codecommit-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[codecommit]` package installed.

Write your `CodeCommit` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type CodeCommitClient
# and provides type checking and code completion
async with session.create_client("codecommit") as client:
    
    # result has type None
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_approval_rule_template_with_repository()
    

    
    # paginator has type DescribePullRequestEventsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("describe_pull_request_events")
    async for item in paginator.paginate(...):
        # item has type DescribePullRequestEventsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[codecommit]` or a standalone
`types_aiobotocore_codecommit` package, you have to explicitly specify
`client: CodeCommitClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_codecommit.client import CodeCommitClient
from types_aiobotocore_codecommit.type_defs import None
from types_aiobotocore_codecommit.paginator import DescribePullRequestEventsPaginator

from types_aiobotocore_codecommit.literals import PaginatorName



session = get_session()

async with session.create_client("codecommit") as client:
    client: CodeCommitClient

    
    result: None = client.associate_approval_rule_template_with_repository()
    

    
    paginator_name: PaginatorName = "describe_pull_request_events"
    paginator: DescribePullRequestEventsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: DescribePullRequestEventsOutputTypeDef
        print(item)
    

    
```

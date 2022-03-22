<a id="examples-for-aiobotocore-inspector-module"></a>

# Examples for aiobotocore Inspector module

> [Index](../README.md) > [Inspector](./README.md) > Examples

- [Examples for aiobotocore Inspector module](#examples-for-aiobotocore-inspector-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[inspector]` package installed.

Write your `Inspector` code as usual, type checking and code completion should
work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type InspectorClient
# and provides type checking and code completion
async with session.create_client("inspector") as client:
    
    # result has type AddAttributesToFindingsResponseTypeDef
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.add_attributes_to_findings()
    

    
    # paginator has type ListAssessmentRunAgentsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_assessment_run_agents")
    async for item in paginator.paginate(...):
        # item has type ListAssessmentRunAgentsResponseTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[inspector]` or a standalone
`types_aiobotocore_inspector` package, you have to explicitly specify
`client: InspectorClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_inspector.client import InspectorClient
from types_aiobotocore_inspector.type_defs import AddAttributesToFindingsResponseTypeDef
from types_aiobotocore_inspector.paginator import ListAssessmentRunAgentsPaginator

from types_aiobotocore_inspector.literals import PaginatorName



session = get_session()

async with session.create_client("inspector") as client:
    client: InspectorClient

    
    result: AddAttributesToFindingsResponseTypeDef = client.add_attributes_to_findings()
    

    
    paginator_name: PaginatorName = "list_assessment_run_agents"
    paginator: ListAssessmentRunAgentsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListAssessmentRunAgentsResponseTypeDef
        print(item)
    

    
```

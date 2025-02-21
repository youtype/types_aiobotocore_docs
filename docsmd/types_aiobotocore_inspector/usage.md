# Examples

> [Index](../README.md) > [Inspector](./README.md) > Examples

!!! note ""

    Auto-generated documentation for [Inspector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector.html#inspector)
    type annotations stubs module [types-aiobotocore-inspector](https://pypi.org/project/types-aiobotocore-inspector/).

## Client

### Implicit type annotations

Can be used with `types-aiobotocore[inspector]` package installed.

Write your `Inspector` code as usual,
type checking and code completion should work out of the box.



```python
# InspectorClient usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("inspector") as client:  # (1)
    result = await client.add_attributes_to_findings()  # (2)
```

1. client: [InspectorClient](./client.md)
2. result: [:material-code-braces: AddAttributesToFindingsResponseTypeDef](./type_defs.md#addattributestofindingsresponsetypedef) 



```python
# ListAssessmentRunAgentsPaginator usage example

from aiobotocore.session import get_session


session = get_session()

async with session.create_client("inspector") as client:  # (1)
    paginator = client.get_paginator("list_assessment_run_agents")  # (2)
    async for item in paginator.paginate(...):
        print(item)  # (3)
```

1. client: [InspectorClient](./client.md)
2. paginator: [ListAssessmentRunAgentsPaginator](./paginators.md#listassessmentrunagentspaginator)
3. item: [:material-code-braces: ListAssessmentRunAgentsResponseTypeDef](./type_defs.md#listassessmentrunagentsresponsetypedef) 




### Explicit type annotations

With `types-aiobotocore-lite[inspector]`
or a standalone `types_aiobotocore_inspector` package, you have to explicitly specify
`client: InspectorClient` type annotation.

All other type annotations are optional, as types should be discovered automatically.
However, these type annotations can be helpful in your functions and methods.


```python
# InspectorClient usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_inspector.client import InspectorClient
from types_aiobotocore_inspector.type_defs import AddAttributesToFindingsResponseTypeDef
from types_aiobotocore_inspector.type_defs import AddAttributesToFindingsRequestTypeDef


session = get_session()

async with session.create_client("inspector") as client:
    client: InspectorClient
    kwargs: AddAttributesToFindingsRequestTypeDef = {...}
    result: AddAttributesToFindingsResponseTypeDef = await client.add_attributes_to_findings(**kwargs)
```



```python
# ListAssessmentRunAgentsPaginator usage example with type annotations

from aiobotocore.session import get_session

from types_aiobotocore_inspector.client import InspectorClient
from types_aiobotocore_inspector.paginator import ListAssessmentRunAgentsPaginator
from types_aiobotocore_inspector.type_defs import ListAssessmentRunAgentsResponseTypeDef


session = get_session()

async with session.create_client("inspector") as client:
    client: InspectorClient
    paginator: ListAssessmentRunAgentsPaginator = client.get_paginator("list_assessment_run_agents")
    async for item in paginator.paginate(...):
        item: ListAssessmentRunAgentsResponseTypeDef
        print(item)
```



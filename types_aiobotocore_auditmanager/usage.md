<a id="examples-for-aiobotocore-auditmanager-module"></a>

# Examples for aiobotocore AuditManager module

> [Index](../README.md) > [AuditManager](./README.md) > Examples

- [Examples for aiobotocore AuditManager module](#examples-for-aiobotocore-auditmanager-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[auditmanager]` package installed.

Write your `AuditManager` code as usual, type checking and code completion
should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type AuditManagerClient
# and provides type checking and code completion
async with session.create_client("auditmanager") as client:
    
    # result has type Dict[str, Any]
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.associate_assessment_report_evidence_folder()
    

    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[auditmanager]` or a standalone
`types_aiobotocore_auditmanager` package, you have to explicitly specify
`client: AuditManagerClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_auditmanager.client import AuditManagerClient
from types_aiobotocore_auditmanager.type_defs import Dict[str, Any]






session = get_session()

async with session.create_client("auditmanager") as client:
    client: AuditManagerClient

    
    result: Dict[str, Any] = client.associate_assessment_report_evidence_folder()
    

    

    
```

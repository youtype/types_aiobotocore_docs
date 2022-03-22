<a id="waiters-for-aiobotocore-schemas-module"></a>

# Waiters for aiobotocore Schemas module

> [Index](../README.md) > [Schemas](./README.md) > Waiters

Auto-generated documentation for
[Schemas](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
type annotations stubs module
[types-aiobotocore-schemas](https://pypi.org/project/types-aiobotocore-schemas/).

- [Waiters for aiobotocore Schemas module](#waiters-for-aiobotocore-schemas-module)
  - [CodeBindingExistsWaiter](#codebindingexistswaiter)

<a id="codebindingexistswaiter"></a>

## CodeBindingExistsWaiter

Type annotations for
`session.create_client("schemas").get_waiter("code_binding_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_schemas.waiter import CodeBindingExistsWaiter

def get_code_binding_exists_waiter() -> CodeBindingExistsWaiter:
    return Session().client("schemas").get_waiter("code_binding_exists")
```

Boto3 documentation:
[Schemas.Waiter.code_binding_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Waiter.CodeBindingExists)

Arguments for `CodeBindingExistsWaiter.wait` method:

- `Language`: `str` *(required)*
- `RegistryName`: `str` *(required)*
- `SchemaName`: `str` *(required)*
- `SchemaVersion`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

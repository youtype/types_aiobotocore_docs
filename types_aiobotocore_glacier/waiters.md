<a id="waiters-for-aiobotocore-glacier-module"></a>

# Waiters for aiobotocore Glacier module

> [Index](..) > [Glacier](.) > Waiters

Auto-generated documentation for
[Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
type annotations stubs module
[types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

- [Waiters for aiobotocore Glacier module](#waiters-for-aiobotocore-glacier-module)
  - [VaultExistsWaiter](#vaultexistswaiter)
  - [VaultNotExistsWaiter](#vaultnotexistswaiter)

<a id="vaultexistswaiter"></a>

## VaultExistsWaiter

Type annotations for
`aiobotocore.create_client("glacier").get_waiter("vault_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_glacier.waiter import VaultExistsWaiter

def get_vault_exists_waiter() -> VaultExistsWaiter:
    return Session().create_client("glacier").get_waiter("vault_exists")
```

Boto3 documentation:
[Glacier.Waiter.vault_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Waiter.VaultExists)

Arguments for `VaultExistsWaiter.wait` method:

- `accountId`: `str` *(required)*
- `vaultName`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="vaultnotexistswaiter"></a>

## VaultNotExistsWaiter

Type annotations for
`aiobotocore.create_client("glacier").get_waiter("vault_not_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_glacier.waiter import VaultNotExistsWaiter

def get_vault_not_exists_waiter() -> VaultNotExistsWaiter:
    return Session().create_client("glacier").get_waiter("vault_not_exists")
```

Boto3 documentation:
[Glacier.Waiter.vault_not_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Waiter.VaultNotExists)

Arguments for `VaultNotExistsWaiter.wait` method:

- `accountId`: `str` *(required)*
- `vaultName`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

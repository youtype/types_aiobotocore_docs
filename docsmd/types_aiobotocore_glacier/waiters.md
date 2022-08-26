# Waiters

> [Index](../README.md) > [Glacier](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [Glacier](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier)
    type annotations stubs module [types-aiobotocore-glacier](https://pypi.org/project/types-aiobotocore-glacier/).

## VaultExistsWaiter

Type annotations and code completion for `#!python session.create_client("glacier").get_waiter("vault_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Waiter.VaultExists)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_glacier.waiter import VaultExistsWaiter

session = get_session()
async with session.create_client("glacier") as client:  # (1)
    waiter: VaultExistsWaiter = client.get_waiter("vault_exists")  # (2)
    await waiter.wait()
```

1. client: [GlacierClient](./client.md)
2. waiter: [VaultExistsWaiter](./waiters.md#vaultexistswaiter)


### wait

Type annotations and code completion for `#!python VaultExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    accountId: str,
    vaultName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVaultInputVaultExistsWaitTypeDef = {  # (1)
    "accountId": ...,
    "vaultName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVaultInputVaultExistsWaitTypeDef](./type_defs.md#describevaultinputvaultexistswaittypedef) 
## VaultNotExistsWaiter

Type annotations and code completion for `#!python session.create_client("glacier").get_waiter("vault_not_exists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Waiter.VaultNotExists)

```python title="Usage example"
from aiobotocore.session import Session

from types_aiobotocore_glacier.waiter import VaultNotExistsWaiter

session = get_session()
async with session.create_client("glacier") as client:  # (1)
    waiter: VaultNotExistsWaiter = client.get_waiter("vault_not_exists")  # (2)
    await waiter.wait()
```

1. client: [GlacierClient](./client.md)
2. waiter: [VaultNotExistsWaiter](./waiters.md#vaultnotexistswaiter)


### wait

Type annotations and code completion for `#!python VaultNotExistsWaiter.wait` method.

```python title="Method definition"
await def wait(
    self,
    *,
    accountId: str,
    vaultName: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: DescribeVaultInputVaultNotExistsWaitTypeDef = {  # (1)
    "accountId": ...,
    "vaultName": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: DescribeVaultInputVaultNotExistsWaitTypeDef](./type_defs.md#describevaultinputvaultnotexistswaittypedef) 

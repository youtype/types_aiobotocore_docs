<a id="waiters-for-aiobotocore-iam-module"></a>

# Waiters for aiobotocore IAM module

> [Index](..) > [IAM](.) > Waiters

Auto-generated documentation for
[IAM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM)
type annotations stubs module
[types-aiobotocore-iam](https://pypi.org/project/types-aiobotocore-iam/).

- [Waiters for aiobotocore IAM module](#waiters-for-aiobotocore-iam-module)
  - [InstanceProfileExistsWaiter](#instanceprofileexistswaiter)
  - [PolicyExistsWaiter](#policyexistswaiter)
  - [RoleExistsWaiter](#roleexistswaiter)
  - [UserExistsWaiter](#userexistswaiter)

<a id="instanceprofileexistswaiter"></a>

## InstanceProfileExistsWaiter

Type annotations for
`session.create_client("iam").get_waiter("instance_profile_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_iam.waiter import InstanceProfileExistsWaiter

def get_instance_profile_exists_waiter() -> InstanceProfileExistsWaiter:
    return Session().client("iam").get_waiter("instance_profile_exists")
```

Boto3 documentation:
[IAM.Waiter.instance_profile_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Waiter.InstanceProfileExists)

Arguments for `InstanceProfileExistsWaiter.wait` method:

- `InstanceProfileName`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="policyexistswaiter"></a>

## PolicyExistsWaiter

Type annotations for
`session.create_client("iam").get_waiter("policy_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_iam.waiter import PolicyExistsWaiter

def get_policy_exists_waiter() -> PolicyExistsWaiter:
    return Session().client("iam").get_waiter("policy_exists")
```

Boto3 documentation:
[IAM.Waiter.policy_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Waiter.PolicyExists)

Arguments for `PolicyExistsWaiter.wait` method:

- `PolicyArn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="roleexistswaiter"></a>

## RoleExistsWaiter

Type annotations for `session.create_client("iam").get_waiter("role_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_iam.waiter import RoleExistsWaiter

def get_role_exists_waiter() -> RoleExistsWaiter:
    return Session().client("iam").get_waiter("role_exists")
```

Boto3 documentation:
[IAM.Waiter.role_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Waiter.RoleExists)

Arguments for `RoleExistsWaiter.wait` method:

- `RoleName`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

<a id="userexistswaiter"></a>

## UserExistsWaiter

Type annotations for `session.create_client("iam").get_waiter("user_exists")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_iam.waiter import UserExistsWaiter

def get_user_exists_waiter() -> UserExistsWaiter:
    return Session().client("iam").get_waiter("user_exists")
```

Boto3 documentation:
[IAM.Waiter.user_exists](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iam.html#IAM.Waiter.UserExists)

Arguments for `UserExistsWaiter.wait` method:

- `UserName`: `str`
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

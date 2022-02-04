<a id="waiters-for-aiobotocore-codedeploy-module"></a>

# Waiters for aiobotocore CodeDeploy module

> [Index](..) > [CodeDeploy](.) > Waiters

Auto-generated documentation for
[CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy)
type annotations stubs module
[types-aiobotocore-codedeploy](https://pypi.org/project/types-aiobotocore-codedeploy/).

- [Waiters for aiobotocore CodeDeploy module](#waiters-for-aiobotocore-codedeploy-module)
  - [DeploymentSuccessfulWaiter](#deploymentsuccessfulwaiter)

<a id="deploymentsuccessfulwaiter"></a>

## DeploymentSuccessfulWaiter

Type annotations for
`aiobotocore.create_client("codedeploy").get_waiter("deployment_successful")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_codedeploy.waiter import DeploymentSuccessfulWaiter

def get_deployment_successful_waiter() -> DeploymentSuccessfulWaiter:
    return Session().create_client("codedeploy").get_waiter("deployment_successful")
```

Boto3 documentation:
[CodeDeploy.Waiter.deployment_successful](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#CodeDeploy.Waiter.DeploymentSuccessful)

Arguments for `DeploymentSuccessfulWaiter.wait` method:

- `deploymentId`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

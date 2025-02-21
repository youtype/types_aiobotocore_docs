# Waiters

> [Index](../README.md) > [CodeDeploy](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [CodeDeploy](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy.html#codedeploy)
    type annotations stubs module [types-aiobotocore-codedeploy](https://pypi.org/project/types-aiobotocore-codedeploy/).

## DeploymentSuccessfulWaiter

Type annotations and code completion for `#!python session.create_client("codedeploy").get_waiter("deployment_successful")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codedeploy/waiter/DeploymentSuccessful.html#CodeDeploy.Waiter.DeploymentSuccessful)

```python
# DeploymentSuccessfulWaiter usage example

from aiobotocore.session import Session

from types_aiobotocore_codedeploy.waiter import DeploymentSuccessfulWaiter

session = get_session()
async with session.create_client("codedeploy") as client:  # (1)
    waiter: DeploymentSuccessfulWaiter = client.get_waiter("deployment_successful")  # (2)
    await waiter.wait()
```

1. client: [CodeDeployClient](./client.md)
2. waiter: [DeploymentSuccessfulWaiter](./waiters.md#deploymentsuccessfulwaiter)


### wait

Type annotations and code completion for `#!python DeploymentSuccessfulWaiter.wait` method.

```python
# wait method definition

await def wait(
    self,
    *,
    deploymentId: str,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python
# wait method usage example with argument unpacking

kwargs: GetDeploymentInputWaitTypeDef = {  # (1)
    "deploymentId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetDeploymentInputWaitTypeDef](./type_defs.md#getdeploymentinputwaittypedef) 

<a id="waiters-for-aiobotocore-cloudcontrolapi-module"></a>

# Waiters for aiobotocore CloudControlApi module

> [Index](..) > [CloudControlApi](.) > Waiters

Auto-generated documentation for
[CloudControlApi](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
type annotations stubs module
[types-aiobotocore-cloudcontrol](https://pypi.org/project/types-aiobotocore-cloudcontrol/).

- [Waiters for aiobotocore CloudControlApi module](#waiters-for-aiobotocore-cloudcontrolapi-module)
  - [ResourceRequestSuccessWaiter](#resourcerequestsuccesswaiter)

<a id="resourcerequestsuccesswaiter"></a>

## ResourceRequestSuccessWaiter

Type annotations for
`session.create_client("cloudcontrol").get_waiter("resource_request_success")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_cloudcontrol.waiter import ResourceRequestSuccessWaiter

def get_resource_request_success_waiter() -> ResourceRequestSuccessWaiter:
    return Session().client("cloudcontrol").get_waiter("resource_request_success")
```

Boto3 documentation:
[CloudControlApi.Waiter.resource_request_success](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Waiter.ResourceRequestSuccess)

Arguments for `ResourceRequestSuccessWaiter.wait` method:

- `RequestToken`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

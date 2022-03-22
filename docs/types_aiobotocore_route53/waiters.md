<a id="waiters-for-aiobotocore-route53-module"></a>

# Waiters for aiobotocore Route53 module

> [Index](../README.md) > [Route53](./README.md) > Waiters

Auto-generated documentation for
[Route53](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
type annotations stubs module
[types-aiobotocore-route53](https://pypi.org/project/types-aiobotocore-route53/).

- [Waiters for aiobotocore Route53 module](#waiters-for-aiobotocore-route53-module)
  - [ResourceRecordSetsChangedWaiter](#resourcerecordsetschangedwaiter)

<a id="resourcerecordsetschangedwaiter"></a>

## ResourceRecordSetsChangedWaiter

Type annotations for
`session.create_client("route53").get_waiter("resource_record_sets_changed")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_route53.waiter import ResourceRecordSetsChangedWaiter

def get_resource_record_sets_changed_waiter() -> ResourceRecordSetsChangedWaiter:
    return Session().client("route53").get_waiter("resource_record_sets_changed")
```

Boto3 documentation:
[Route53.Waiter.resource_record_sets_changed](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Waiter.ResourceRecordSetsChanged)

Arguments for `ResourceRecordSetsChangedWaiter.wait` method:

- `Id`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

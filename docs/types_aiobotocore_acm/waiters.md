<a id="waiters-for-aiobotocore-acm-module"></a>

# Waiters for aiobotocore ACM module

> [Index](../README.md) > [ACM](./README.md) > Waiters

Auto-generated documentation for
[ACM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM)
type annotations stubs module
[types-aiobotocore-acm](https://pypi.org/project/types-aiobotocore-acm/).

- [Waiters for aiobotocore ACM module](#waiters-for-aiobotocore-acm-module)
  - [CertificateValidatedWaiter](#certificatevalidatedwaiter)

<a id="certificatevalidatedwaiter"></a>

## CertificateValidatedWaiter

Type annotations for
`session.create_client("acm").get_waiter("certificate_validated")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_acm.waiter import CertificateValidatedWaiter

def get_certificate_validated_waiter() -> CertificateValidatedWaiter:
    return Session().client("acm").get_waiter("certificate_validated")
```

Boto3 documentation:
[ACM.Waiter.certificate_validated](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm.html#ACM.Waiter.CertificateValidated)

Arguments for `CertificateValidatedWaiter.wait` method:

- `CertificateArn`: `str` *(required)*
- `WaiterConfig`: [WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef)

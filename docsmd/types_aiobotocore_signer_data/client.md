# SignerDataPlaneClient

> [Index](../README.md) > [SignerDataPlane](./README.md) > SignerDataPlaneClient

!!! note ""

    Auto-generated documentation for [SignerDataPlane](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer-data.html#signerdataplane)
    type annotations stubs module [types-aiobotocore-signer-data](https://pypi.org/project/types-aiobotocore-signer-data/).

## SignerDataPlaneClient

Type annotations and code completion for `#!python session.create_client("signer-data")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer-data.html#SignerDataPlane.Client)

```python
# SignerDataPlaneClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_signer_data.client import SignerDataPlaneClient

session = get_session()
async with session.create_client("signer-data") as client:
    client: SignerDataPlaneClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("signer-data").exceptions` structure.

```python
# SignerDataPlaneClient.exceptions usage example

async with session.create_client("signer-data") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServiceErrorException,
        client.TooManyRequestsException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# SignerDataPlaneClient usage type checking example

from types_aiobotocore_signer_data.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("signer-data").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer-data/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("signer-data").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer-data/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### get\_revocation\_status

Retrieves the revocation status for a signed artifact by checking if the
signing profile, job, or certificate has been revoked.

Type annotations and code completion for `#!python session.create_client("signer-data").get_revocation_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer-data/client/get_revocation_status.html)

```python
# get_revocation_status method definition

await def get_revocation_status(
    self,
    *,
    signatureTimestamp: TimestampTypeDef,
    platformId: str,
    profileVersionArn: str,
    jobArn: str,
    certificateHashes: Sequence[str],
) -> GetRevocationStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRevocationStatusResponseTypeDef](./type_defs.md#getrevocationstatusresponsetypedef)


```python
# get_revocation_status method usage example with argument unpacking

kwargs: GetRevocationStatusRequestTypeDef = {  # (1)
    "signatureTimestamp": ...,
    "platformId": ...,
    "profileVersionArn": ...,
    "jobArn": ...,
    "certificateHashes": ...,
}

parent.get_revocation_status(**kwargs)
```

1. See [:material-code-braces: GetRevocationStatusRequestTypeDef](./type_defs.md#getrevocationstatusrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("signer-data").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer-data.html#SignerDataPlane.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("signer-data").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/signer-data.html#SignerDataPlane.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: type[BaseException] | None,
    exc_val: BaseException | None,
    exc_tb: types.TracebackType | None,
) -> None:
    ...
```






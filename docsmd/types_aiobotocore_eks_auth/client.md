# EKSAuthClient

> [Index](../README.md) > [EKSAuth](./README.md) > EKSAuthClient

!!! note ""

    Auto-generated documentation for [EKSAuth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth)
    type annotations stubs module [types-aiobotocore-eks-auth](https://pypi.org/project/types-aiobotocore-eks-auth/).

## EKSAuthClient

Type annotations and code completion for `#!python session.create_client("eks-auth")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client)

```python
# EKSAuthClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_eks_auth.client import EKSAuthClient

session = get_session()
async with session.create_client("eks-auth") as client:
    client: EKSAuthClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("eks-auth").exceptions` structure.

```python
# EKSAuthClient.exceptions usage example

async with session.create_client("eks-auth") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ExpiredTokenException,
        client.InternalServerException,
        client.InvalidParameterException,
        client.InvalidRequestException,
        client.InvalidTokenException,
        client.ResourceNotFoundException,
        client.ServiceUnavailableException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# EKSAuthClient usage type checking example

from types_aiobotocore_eks_auth.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### assume\_role\_for\_pod\_identity

The Amazon EKS Auth API and the `AssumeRoleForPodIdentity` action are only used
by the EKS Pod Identity
Agent.

Type annotations and code completion for `#!python session.create_client("eks-auth").assume_role_for_pod_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client.assume_role_for_pod_identity)

```python
# assume_role_for_pod_identity method definition

await def assume_role_for_pod_identity(
    self,
    *,
    clusterName: str,
    token: str,
) -> AssumeRoleForPodIdentityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssumeRoleForPodIdentityResponseTypeDef](./type_defs.md#assumeroleforpodidentityresponsetypedef) 


```python
# assume_role_for_pod_identity method usage example with argument unpacking

kwargs: AssumeRoleForPodIdentityRequestRequestTypeDef = {  # (1)
    "clusterName": ...,
    "token": ...,
}

parent.assume_role_for_pod_identity(**kwargs)
```

1. See [:material-code-braces: AssumeRoleForPodIdentityRequestRequestTypeDef](./type_defs.md#assumeroleforpodidentityrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("eks-auth").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("eks-auth").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("eks-auth").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client.generate_presigned_url)

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


### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("eks-auth").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "EKSAuthClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("eks-auth").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```






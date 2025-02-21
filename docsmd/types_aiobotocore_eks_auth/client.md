# EKSAuthClient

> [Index](../README.md) > [EKSAuth](./README.md) > EKSAuthClient

!!! note ""

    Auto-generated documentation for [EKSAuth](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#eksauth)
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


### can\_paginate



Type annotations and code completion for `#!python session.create_client("eks-auth").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("eks-auth").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth/client/generate_presigned_url.html)

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


### assume\_role\_for\_pod\_identity

The Amazon EKS Auth API and the <code>AssumeRoleForPodIdentity</code> action
are only used by the EKS Pod Identity Agent.

Type annotations and code completion for `#!python session.create_client("eks-auth").assume_role_for_pod_identity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth/client/assume_role_for_pod_identity.html)

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

kwargs: AssumeRoleForPodIdentityRequestTypeDef = {  # (1)
    "clusterName": ...,
    "token": ...,
}

parent.assume_role_for_pod_identity(**kwargs)
```

1. See [:material-code-braces: AssumeRoleForPodIdentityRequestTypeDef](./type_defs.md#assumeroleforpodidentityrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("eks-auth").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("eks-auth").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/eks-auth.html#EKSAuth.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```






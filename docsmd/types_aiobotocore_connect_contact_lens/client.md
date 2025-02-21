# ConnectContactLensClient

> [Index](../README.md) > [ConnectContactLens](./README.md) > ConnectContactLensClient

!!! note ""

    Auto-generated documentation for [ConnectContactLens](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#connectcontactlens)
    type annotations stubs module [types-aiobotocore-connect-contact-lens](https://pypi.org/project/types-aiobotocore-connect-contact-lens/).

## ConnectContactLensClient

Type annotations and code completion for `#!python session.create_client("connect-contact-lens")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client)

```python
# ConnectContactLensClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_connect_contact_lens.client import ConnectContactLensClient

session = get_session()
async with session.create_client("connect-contact-lens") as client:
    client: ConnectContactLensClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("connect-contact-lens").exceptions` structure.

```python
# ConnectContactLensClient.exceptions usage example

async with session.create_client("connect-contact-lens") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServiceException,
        client.InvalidRequestException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# ConnectContactLensClient usage type checking example

from types_aiobotocore_connect_contact_lens.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("connect-contact-lens").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("connect-contact-lens").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens/client/generate_presigned_url.html)

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


### list\_realtime\_contact\_analysis\_segments

Provides a list of analysis segments for a real-time analysis session.

Type annotations and code completion for `#!python session.create_client("connect-contact-lens").list_realtime_contact_analysis_segments` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens/client/list_realtime_contact_analysis_segments.html)

```python
# list_realtime_contact_analysis_segments method definition

await def list_realtime_contact_analysis_segments(
    self,
    *,
    InstanceId: str,
    ContactId: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRealtimeContactAnalysisSegmentsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRealtimeContactAnalysisSegmentsResponseTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsresponsetypedef) 


```python
# list_realtime_contact_analysis_segments method usage example with argument unpacking

kwargs: ListRealtimeContactAnalysisSegmentsRequestTypeDef = {  # (1)
    "InstanceId": ...,
    "ContactId": ...,
}

parent.list_realtime_contact_analysis_segments(**kwargs)
```

1. See [:material-code-braces: ListRealtimeContactAnalysisSegmentsRequestTypeDef](./type_defs.md#listrealtimecontactanalysissegmentsrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("connect-contact-lens").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("connect-contact-lens").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect-contact-lens.html#ConnectContactLens.Client)

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






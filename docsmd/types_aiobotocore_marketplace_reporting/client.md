# MarketplaceReportingServiceClient

> [Index](../README.md) > [MarketplaceReportingService](./README.md) > MarketplaceReportingServiceClient

!!! note ""

    Auto-generated documentation for [MarketplaceReportingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#marketplacereportingservice)
    type annotations stubs module [types-aiobotocore-marketplace-reporting](https://pypi.org/project/types-aiobotocore-marketplace-reporting/).

## MarketplaceReportingServiceClient

Type annotations and code completion for `#!python session.create_client("marketplace-reporting")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#MarketplaceReportingService.Client)

```python
# MarketplaceReportingServiceClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_marketplace_reporting.client import MarketplaceReportingServiceClient

session = get_session()
async with session.create_client("marketplace-reporting") as client:
    client: MarketplaceReportingServiceClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("marketplace-reporting").exceptions` structure.

```python
# MarketplaceReportingServiceClient.exceptions usage example

async with session.create_client("marketplace-reporting") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
        client.ClientError,
        client.InternalServerException,
        client.UnauthorizedException,
    ) as e:
        print(e)
```

```python
# MarketplaceReportingServiceClient usage type checking example

from types_aiobotocore_marketplace_reporting.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("marketplace-reporting").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("marketplace-reporting").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting/client/generate_presigned_url.html)

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


### get\_buyer\_dashboard

Generates an embedding URL for an Amazon QuickSight dashboard for an anonymous
user.

Type annotations and code completion for `#!python session.create_client("marketplace-reporting").get_buyer_dashboard` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting/client/get_buyer_dashboard.html)

```python
# get_buyer_dashboard method definition

await def get_buyer_dashboard(
    self,
    *,
    dashboardIdentifier: str,
    embeddingDomains: Sequence[str],
) -> GetBuyerDashboardOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetBuyerDashboardOutputTypeDef](./type_defs.md#getbuyerdashboardoutputtypedef) 


```python
# get_buyer_dashboard method usage example with argument unpacking

kwargs: GetBuyerDashboardInputTypeDef = {  # (1)
    "dashboardIdentifier": ...,
    "embeddingDomains": ...,
}

parent.get_buyer_dashboard(**kwargs)
```

1. See [:material-code-braces: GetBuyerDashboardInputTypeDef](./type_defs.md#getbuyerdashboardinputtypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("marketplace-reporting").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#MarketplaceReportingService.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("marketplace-reporting").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-reporting.html#MarketplaceReportingService.Client)

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






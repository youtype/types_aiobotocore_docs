# LicenseManagerLinuxSubscriptionsClient

> [Index](../README.md) > [LicenseManagerLinuxSubscriptions](./README.md) > LicenseManagerLinuxSubscriptionsClient

!!! note ""

    Auto-generated documentation for [LicenseManagerLinuxSubscriptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions)
    type annotations stubs module [types-aiobotocore-license-manager-linux-subscriptions](https://pypi.org/project/types-aiobotocore-license-manager-linux-subscriptions/).

## LicenseManagerLinuxSubscriptionsClient

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client)

```python
LicenseManagerLinuxSubscriptionsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_license_manager_linux_subscriptions.client import LicenseManagerLinuxSubscriptionsClient

session = get_session()
async with session.create_client("license-manager-linux-subscriptions") as client:
    client: LicenseManagerLinuxSubscriptionsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("license-manager-linux-subscriptions").exceptions` structure.

```python
LicenseManagerLinuxSubscriptionsClient.exceptions usage example

async with session.create_client("license-manager-linux-subscriptions") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.InternalServerException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
LicenseManagerLinuxSubscriptionsClient usage type checking example

from types_aiobotocore_license_manager_linux_subscriptions.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.generate_presigned_url)

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


### get\_service\_settings

Lists the Linux subscriptions service settings.

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").get_service_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.get_service_settings)

```python
# get_service_settings method definition

await def get_service_settings(
    self,
) -> GetServiceSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetServiceSettingsResponseTypeDef](./type_defs.md#getservicesettingsresponsetypedef) 

### list\_linux\_subscription\_instances

Lists the running Amazon EC2 instances that were discovered with commercial
Linux subscriptions.

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").list_linux_subscription_instances` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.list_linux_subscription_instances)

```python
# list_linux_subscription_instances method definition

await def list_linux_subscription_instances(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLinuxSubscriptionInstancesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListLinuxSubscriptionInstancesResponseTypeDef](./type_defs.md#listlinuxsubscriptioninstancesresponsetypedef) 


```python
# list_linux_subscription_instances method usage example with argument unpacking

kwargs: ListLinuxSubscriptionInstancesRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_linux_subscription_instances(**kwargs)
```

1. See [:material-code-braces: ListLinuxSubscriptionInstancesRequestRequestTypeDef](./type_defs.md#listlinuxsubscriptioninstancesrequestrequesttypedef) 

### list\_linux\_subscriptions

Lists the Linux subscriptions that have been discovered.

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").list_linux_subscriptions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.list_linux_subscriptions)

```python
# list_linux_subscriptions method definition

await def list_linux_subscriptions(
    self,
    *,
    Filters: Sequence[FilterTypeDef] = ...,  # (1)
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListLinuxSubscriptionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FilterTypeDef](./type_defs.md#filtertypedef) 
2. See [:material-code-braces: ListLinuxSubscriptionsResponseTypeDef](./type_defs.md#listlinuxsubscriptionsresponsetypedef) 


```python
# list_linux_subscriptions method usage example with argument unpacking

kwargs: ListLinuxSubscriptionsRequestRequestTypeDef = {  # (1)
    "Filters": ...,
}

parent.list_linux_subscriptions(**kwargs)
```

1. See [:material-code-braces: ListLinuxSubscriptionsRequestRequestTypeDef](./type_defs.md#listlinuxsubscriptionsrequestrequesttypedef) 

### update\_service\_settings

Updates the service settings for Linux subscriptions.

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").update_service_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.update_service_settings)

```python
# update_service_settings method definition

await def update_service_settings(
    self,
    *,
    LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,  # (1)
    LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsTypeDef,  # (2)
    AllowUpdate: bool = ...,
) -> UpdateServiceSettingsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LinuxSubscriptionsDiscoveryType](./literals.md#linuxsubscriptionsdiscoverytype) 
2. See [:material-code-braces: LinuxSubscriptionsDiscoverySettingsTypeDef](./type_defs.md#linuxsubscriptionsdiscoverysettingstypedef) 
3. See [:material-code-braces: UpdateServiceSettingsResponseTypeDef](./type_defs.md#updateservicesettingsresponsetypedef) 


```python
# update_service_settings method usage example with argument unpacking

kwargs: UpdateServiceSettingsRequestRequestTypeDef = {  # (1)
    "LinuxSubscriptionsDiscovery": ...,
    "LinuxSubscriptionsDiscoverySettings": ...,
}

parent.update_service_settings(**kwargs)
```

1. See [:material-code-braces: UpdateServiceSettingsRequestRequestTypeDef](./type_defs.md#updateservicesettingsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> LicenseManagerLinuxSubscriptionsClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.__aexit__)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("license-manager-linux-subscriptions").get_paginator` method with overloads.

- `client.get_paginator("list_linux_subscription_instances")` -> [ListLinuxSubscriptionInstancesPaginator](./paginators.md#listlinuxsubscriptioninstancespaginator)
- `client.get_paginator("list_linux_subscriptions")` -> [ListLinuxSubscriptionsPaginator](./paginators.md#listlinuxsubscriptionspaginator)




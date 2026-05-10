# BillingandCostManagementRecommendedActionsClient

> [Index](../README.md) > [BillingandCostManagementRecommendedActions](./README.md) > BillingandCostManagementRecommendedActionsClient

!!! note ""

    Auto-generated documentation for [BillingandCostManagementRecommendedActions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions.html#billingandcostmanagementrecommendedactions)
    type annotations stubs module [types-aiobotocore-bcm-recommended-actions](https://pypi.org/project/types-aiobotocore-bcm-recommended-actions/).

## BillingandCostManagementRecommendedActionsClient

Type annotations and code completion for `#!python session.create_client("bcm-recommended-actions")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions.html#BillingandCostManagementRecommendedActions.Client)

```python
# BillingandCostManagementRecommendedActionsClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_bcm_recommended_actions.client import BillingandCostManagementRecommendedActionsClient

session = get_session()
async with session.create_client("bcm-recommended-actions") as client:
    client: BillingandCostManagementRecommendedActionsClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("bcm-recommended-actions").exceptions` structure.

```python
# BillingandCostManagementRecommendedActionsClient.exceptions usage example

async with session.create_client("bcm-recommended-actions") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# BillingandCostManagementRecommendedActionsClient usage type checking example

from types_aiobotocore_bcm_recommended_actions.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("bcm-recommended-actions").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("bcm-recommended-actions").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions/client/generate_presigned_url.html)

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


### list\_recommended\_actions

Returns a list of recommended actions that match the filter criteria.

Type annotations and code completion for `#!python session.create_client("bcm-recommended-actions").list_recommended_actions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions/client/list_recommended_actions.html)

```python
# list_recommended_actions method definition

await def list_recommended_actions(
    self,
    *,
    filter: RequestFilterTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListRecommendedActionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RequestFilterTypeDef](./type_defs.md#requestfiltertypedef)
2. See [:material-code-braces: ListRecommendedActionsResponseTypeDef](./type_defs.md#listrecommendedactionsresponsetypedef)


```python
# list_recommended_actions method usage example with argument unpacking

kwargs: ListRecommendedActionsRequestTypeDef = {  # (1)
    "filter": ...,
}

parent.list_recommended_actions(**kwargs)
```

1. See [:material-code-braces: ListRecommendedActionsRequestTypeDef](./type_defs.md#listrecommendedactionsrequesttypedef)

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("bcm-recommended-actions").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions.html#BillingandCostManagementRecommendedActions.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("bcm-recommended-actions").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/bcm-recommended-actions.html#BillingandCostManagementRecommendedActions.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("bcm-recommended-actions").get_paginator` method with overloads.

- `client.get_paginator("list_recommended_actions")` -> [ListRecommendedActionsPaginator](./paginators.md#listrecommendedactionspaginator)




# ControlCatalogClient

> [Index](../README.md) > [ControlCatalog](./README.md) > ControlCatalogClient

!!! note ""

    Auto-generated documentation for [ControlCatalog](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#controlcatalog)
    type annotations stubs module [types-aiobotocore-controlcatalog](https://pypi.org/project/types-aiobotocore-controlcatalog/).

## ControlCatalogClient

Type annotations and code completion for `#!python session.create_client("controlcatalog")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#ControlCatalog.Client)

```python
# ControlCatalogClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_controlcatalog.client import ControlCatalogClient

session = get_session()
async with session.create_client("controlcatalog") as client:
    client: ControlCatalogClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("controlcatalog").exceptions` structure.

```python
# ControlCatalogClient.exceptions usage example

async with session.create_client("controlcatalog") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# ControlCatalogClient usage type checking example

from types_aiobotocore_controlcatalog.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("controlcatalog").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("controlcatalog").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/client/generate_presigned_url.html)

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


### get\_control

Returns details about a specific control, most notably a list of Amazon Web
Services Regions where this control is supported.

Type annotations and code completion for `#!python session.create_client("controlcatalog").get_control` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/client/get_control.html)

```python
# get_control method definition

await def get_control(
    self,
    *,
    ControlArn: str,
) -> GetControlResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetControlResponseTypeDef](./type_defs.md#getcontrolresponsetypedef) 


```python
# get_control method usage example with argument unpacking

kwargs: GetControlRequestTypeDef = {  # (1)
    "ControlArn": ...,
}

parent.get_control(**kwargs)
```

1. See [:material-code-braces: GetControlRequestTypeDef](./type_defs.md#getcontrolrequesttypedef) 

### list\_common\_controls

Returns a paginated list of common controls from the Amazon Web Services
Control Catalog.

Type annotations and code completion for `#!python session.create_client("controlcatalog").list_common_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/client/list_common_controls.html)

```python
# list_common_controls method definition

await def list_common_controls(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    CommonControlFilter: CommonControlFilterTypeDef = ...,  # (1)
) -> ListCommonControlsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CommonControlFilterTypeDef](./type_defs.md#commoncontrolfiltertypedef) 
2. See [:material-code-braces: ListCommonControlsResponseTypeDef](./type_defs.md#listcommoncontrolsresponsetypedef) 


```python
# list_common_controls method usage example with argument unpacking

kwargs: ListCommonControlsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_common_controls(**kwargs)
```

1. See [:material-code-braces: ListCommonControlsRequestTypeDef](./type_defs.md#listcommoncontrolsrequesttypedef) 

### list\_controls

Returns a paginated list of all available controls in the Amazon Web Services
Control Catalog library.

Type annotations and code completion for `#!python session.create_client("controlcatalog").list_controls` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/client/list_controls.html)

```python
# list_controls method definition

await def list_controls(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListControlsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListControlsResponseTypeDef](./type_defs.md#listcontrolsresponsetypedef) 


```python
# list_controls method usage example with argument unpacking

kwargs: ListControlsRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_controls(**kwargs)
```

1. See [:material-code-braces: ListControlsRequestTypeDef](./type_defs.md#listcontrolsrequesttypedef) 

### list\_domains

Returns a paginated list of domains from the Amazon Web Services Control
Catalog.

Type annotations and code completion for `#!python session.create_client("controlcatalog").list_domains` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/client/list_domains.html)

```python
# list_domains method definition

await def list_domains(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListDomainsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDomainsResponseTypeDef](./type_defs.md#listdomainsresponsetypedef) 


```python
# list_domains method usage example with argument unpacking

kwargs: ListDomainsRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_domains(**kwargs)
```

1. See [:material-code-braces: ListDomainsRequestTypeDef](./type_defs.md#listdomainsrequesttypedef) 

### list\_objectives

Returns a paginated list of objectives from the Amazon Web Services Control
Catalog.

Type annotations and code completion for `#!python session.create_client("controlcatalog").list_objectives` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog/client/list_objectives.html)

```python
# list_objectives method definition

await def list_objectives(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    ObjectiveFilter: ObjectiveFilterTypeDef = ...,  # (1)
) -> ListObjectivesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ObjectiveFilterTypeDef](./type_defs.md#objectivefiltertypedef) 
2. See [:material-code-braces: ListObjectivesResponseTypeDef](./type_defs.md#listobjectivesresponsetypedef) 


```python
# list_objectives method usage example with argument unpacking

kwargs: ListObjectivesRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_objectives(**kwargs)
```

1. See [:material-code-braces: ListObjectivesRequestTypeDef](./type_defs.md#listobjectivesrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("controlcatalog").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#ControlCatalog.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("controlcatalog").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controlcatalog.html#ControlCatalog.Client)

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




### get_paginator

Type annotations and code completion for `#!python session.create_client("controlcatalog").get_paginator` method with overloads.

- `client.get_paginator("list_common_controls")` -> [ListCommonControlsPaginator](./paginators.md#listcommoncontrolspaginator)
- `client.get_paginator("list_controls")` -> [ListControlsPaginator](./paginators.md#listcontrolspaginator)
- `client.get_paginator("list_domains")` -> [ListDomainsPaginator](./paginators.md#listdomainspaginator)
- `client.get_paginator("list_objectives")` -> [ListObjectivesPaginator](./paginators.md#listobjectivespaginator)




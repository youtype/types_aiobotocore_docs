# InspectorscanClient

> [Index](../README.md) > [Inspectorscan](./README.md) > InspectorscanClient

!!! note ""

    Auto-generated documentation for [Inspectorscan](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#inspectorscan)
    type annotations stubs module [types-aiobotocore-inspector-scan](https://pypi.org/project/types-aiobotocore-inspector-scan/).

## InspectorscanClient

Type annotations and code completion for `#!python session.create_client("inspector-scan")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# InspectorscanClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_inspector_scan.client import InspectorscanClient

session = get_session()
async with session.create_client("inspector-scan") as client:
    client: InspectorscanClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("inspector-scan").exceptions` structure.

```python
# InspectorscanClient.exceptions usage example

async with session.create_client("inspector-scan") as client:
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
# InspectorscanClient usage type checking example

from types_aiobotocore_inspector_scan.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("inspector-scan").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("inspector-scan").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan/client/generate_presigned_url.html)

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


### close



Type annotations and code completion for `#!python session.create_client("inspector-scan").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan/client/close.html)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### scan\_sbom

Scans a provided CycloneDX 1.5 SBOM and reports on any vulnerabilities
discovered in that SBOM.

Type annotations and code completion for `#!python session.create_client("inspector-scan").scan_sbom` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan/client/scan_sbom.html)

```python
# scan_sbom method definition

await def scan_sbom(
    self,
    *,
    sbom: Mapping[str, Any],
    outputFormat: OutputFormatType = ...,  # (1)
) -> ScanSbomResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: OutputFormatType](./literals.md#outputformattype) 
2. See [:material-code-braces: ScanSbomResponseTypeDef](./type_defs.md#scansbomresponsetypedef) 


```python
# scan_sbom method usage example with argument unpacking

kwargs: ScanSbomRequestRequestTypeDef = {  # (1)
    "sbom": ...,
}

parent.scan_sbom(**kwargs)
```

1. See [:material-code-braces: ScanSbomRequestRequestTypeDef](./type_defs.md#scansbomrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("inspector-scan").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "InspectorscanClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("inspector-scan").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector-scan.html#Inspectorscan.Client)

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






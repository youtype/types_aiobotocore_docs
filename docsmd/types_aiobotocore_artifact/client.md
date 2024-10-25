# ArtifactClient

> [Index](../README.md) > [Artifact](./README.md) > ArtifactClient

!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact)
    type annotations stubs module [types-aiobotocore-artifact](https://pypi.org/project/types-aiobotocore-artifact/).

## ArtifactClient

Type annotations and code completion for `#!python session.create_client("artifact")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client)

```python
# ArtifactClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_artifact.client import ArtifactClient

session = get_session()
async with session.create_client("artifact") as client:
    client: ArtifactClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("artifact").exceptions` structure.

```python
# ArtifactClient.exceptions usage example

async with session.create_client("artifact") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
# ArtifactClient usage type checking example

from types_aiobotocore_artifact.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("artifact").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.can_paginate)

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

Type annotations and code completion for `#!python session.create_client("artifact").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("artifact").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.generate_presigned_url)

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


### get\_account\_settings

Get the account settings for Artifact.

Type annotations and code completion for `#!python session.create_client("artifact").get_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.get_account_settings)

```python
# get_account_settings method definition

await def get_account_settings(
    self,
) -> GetAccountSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAccountSettingsResponseTypeDef](./type_defs.md#getaccountsettingsresponsetypedef) 

### get\_report

Get the content for a single report.

Type annotations and code completion for `#!python session.create_client("artifact").get_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.get_report)

```python
# get_report method definition

await def get_report(
    self,
    *,
    reportId: str,
    termToken: str,
    reportVersion: int = ...,
) -> GetReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReportResponseTypeDef](./type_defs.md#getreportresponsetypedef) 


```python
# get_report method usage example with argument unpacking

kwargs: GetReportRequestRequestTypeDef = {  # (1)
    "reportId": ...,
    "termToken": ...,
}

parent.get_report(**kwargs)
```

1. See [:material-code-braces: GetReportRequestRequestTypeDef](./type_defs.md#getreportrequestrequesttypedef) 

### get\_report\_metadata

Get the metadata for a single report.

Type annotations and code completion for `#!python session.create_client("artifact").get_report_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.get_report_metadata)

```python
# get_report_metadata method definition

await def get_report_metadata(
    self,
    *,
    reportId: str,
    reportVersion: int = ...,
) -> GetReportMetadataResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetReportMetadataResponseTypeDef](./type_defs.md#getreportmetadataresponsetypedef) 


```python
# get_report_metadata method usage example with argument unpacking

kwargs: GetReportMetadataRequestRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.get_report_metadata(**kwargs)
```

1. See [:material-code-braces: GetReportMetadataRequestRequestTypeDef](./type_defs.md#getreportmetadatarequestrequesttypedef) 

### get\_term\_for\_report

Get the Term content associated with a single report.

Type annotations and code completion for `#!python session.create_client("artifact").get_term_for_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.get_term_for_report)

```python
# get_term_for_report method definition

await def get_term_for_report(
    self,
    *,
    reportId: str,
    reportVersion: int = ...,
) -> GetTermForReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetTermForReportResponseTypeDef](./type_defs.md#gettermforreportresponsetypedef) 


```python
# get_term_for_report method usage example with argument unpacking

kwargs: GetTermForReportRequestRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.get_term_for_report(**kwargs)
```

1. See [:material-code-braces: GetTermForReportRequestRequestTypeDef](./type_defs.md#gettermforreportrequestrequesttypedef) 

### list\_reports

List available reports.

Type annotations and code completion for `#!python session.create_client("artifact").list_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.list_reports)

```python
# list_reports method definition

await def list_reports(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListReportsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListReportsResponseTypeDef](./type_defs.md#listreportsresponsetypedef) 


```python
# list_reports method usage example with argument unpacking

kwargs: ListReportsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_reports(**kwargs)
```

1. See [:material-code-braces: ListReportsRequestRequestTypeDef](./type_defs.md#listreportsrequestrequesttypedef) 

### put\_account\_settings

Put the account settings for Artifact.

Type annotations and code completion for `#!python session.create_client("artifact").put_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.put_account_settings)

```python
# put_account_settings method definition

await def put_account_settings(
    self,
    *,
    notificationSubscriptionStatus: NotificationSubscriptionStatusType = ...,  # (1)
) -> PutAccountSettingsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: NotificationSubscriptionStatusType](./literals.md#notificationsubscriptionstatustype) 
2. See [:material-code-braces: PutAccountSettingsResponseTypeDef](./type_defs.md#putaccountsettingsresponsetypedef) 


```python
# put_account_settings method usage example with argument unpacking

kwargs: PutAccountSettingsRequestRequestTypeDef = {  # (1)
    "notificationSubscriptionStatus": ...,
}

parent.put_account_settings(**kwargs)
```

1. See [:material-code-braces: PutAccountSettingsRequestRequestTypeDef](./type_defs.md#putaccountsettingsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("artifact").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> "ArtifactClient":
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("artifact").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("artifact").get_paginator` method with overloads.

- `client.get_paginator("list_reports")` -> [ListReportsPaginator](./paginators.md#listreportspaginator)




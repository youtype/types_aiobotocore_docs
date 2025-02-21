# ArtifactClient

> [Index](../README.md) > [Artifact](./README.md) > ArtifactClient

!!! note ""

    Auto-generated documentation for [Artifact](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#artifact)
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



Type annotations and code completion for `#!python session.create_client("artifact").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("artifact").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/generate_presigned_url.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/get_account_settings.html)

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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/get_report.html)

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

kwargs: GetReportRequestTypeDef = {  # (1)
    "reportId": ...,
    "termToken": ...,
}

parent.get_report(**kwargs)
```

1. See [:material-code-braces: GetReportRequestTypeDef](./type_defs.md#getreportrequesttypedef) 

### get\_report\_metadata

Get the metadata for a single report.

Type annotations and code completion for `#!python session.create_client("artifact").get_report_metadata` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/get_report_metadata.html)

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

kwargs: GetReportMetadataRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.get_report_metadata(**kwargs)
```

1. See [:material-code-braces: GetReportMetadataRequestTypeDef](./type_defs.md#getreportmetadatarequesttypedef) 

### get\_term\_for\_report

Get the Term content associated with a single report.

Type annotations and code completion for `#!python session.create_client("artifact").get_term_for_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/get_term_for_report.html)

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

kwargs: GetTermForReportRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.get_term_for_report(**kwargs)
```

1. See [:material-code-braces: GetTermForReportRequestTypeDef](./type_defs.md#gettermforreportrequesttypedef) 

### list\_customer\_agreements

List active customer-agreements applicable to calling identity.

Type annotations and code completion for `#!python session.create_client("artifact").list_customer_agreements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/list_customer_agreements.html)

```python
# list_customer_agreements method definition

await def list_customer_agreements(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListCustomerAgreementsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListCustomerAgreementsResponseTypeDef](./type_defs.md#listcustomeragreementsresponsetypedef) 


```python
# list_customer_agreements method usage example with argument unpacking

kwargs: ListCustomerAgreementsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_customer_agreements(**kwargs)
```

1. See [:material-code-braces: ListCustomerAgreementsRequestTypeDef](./type_defs.md#listcustomeragreementsrequesttypedef) 

### list\_reports

List available reports.

Type annotations and code completion for `#!python session.create_client("artifact").list_reports` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/list_reports.html)

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

kwargs: ListReportsRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_reports(**kwargs)
```

1. See [:material-code-braces: ListReportsRequestTypeDef](./type_defs.md#listreportsrequesttypedef) 

### put\_account\_settings

Put the account settings for Artifact.

Type annotations and code completion for `#!python session.create_client("artifact").put_account_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact/client/put_account_settings.html)

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

kwargs: PutAccountSettingsRequestTypeDef = {  # (1)
    "notificationSubscriptionStatus": ...,
}

parent.put_account_settings(**kwargs)
```

1. See [:material-code-braces: PutAccountSettingsRequestTypeDef](./type_defs.md#putaccountsettingsrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("artifact").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("artifact").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/artifact.html#Artifact.Client)

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

Type annotations and code completion for `#!python session.create_client("artifact").get_paginator` method with overloads.

- `client.get_paginator("list_customer_agreements")` -> [ListCustomerAgreementsPaginator](./paginators.md#listcustomeragreementspaginator)
- `client.get_paginator("list_reports")` -> [ListReportsPaginator](./paginators.md#listreportspaginator)




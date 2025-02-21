# SupportClient

> [Index](../README.md) > [Support](./README.md) > SupportClient

!!! note ""

    Auto-generated documentation for [Support](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#support)
    type annotations stubs module [types-aiobotocore-support](https://pypi.org/project/types-aiobotocore-support/).

## SupportClient

Type annotations and code completion for `#!python session.create_client("support")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client)

```python
# SupportClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_support.client import SupportClient

session = get_session()
async with session.create_client("support") as client:
    client: SupportClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("support").exceptions` structure.

```python
# SupportClient.exceptions usage example

async with session.create_client("support") as client:
    try:
        do_something(client)
    except (
            client.AttachmentIdNotFound,
        client.AttachmentLimitExceeded,
        client.AttachmentSetExpired,
        client.AttachmentSetIdNotFound,
        client.AttachmentSetSizeLimitExceeded,
        client.CaseCreationLimitExceeded,
        client.CaseIdNotFound,
        client.ClientError,
        client.DescribeAttachmentLimitExceeded,
        client.InternalServerError,
        client.ThrottlingException,
    ) as e:
        print(e)
```

```python
# SupportClient usage type checking example

from types_aiobotocore_support.client import Exceptions

def handle_error(exc: Exceptions.AttachmentIdNotFound) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("support").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("support").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/generate_presigned_url.html)

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


### add\_attachments\_to\_set

Adds one or more attachments to an attachment set.

Type annotations and code completion for `#!python session.create_client("support").add_attachments_to_set` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/add_attachments_to_set.html)

```python
# add_attachments_to_set method definition

await def add_attachments_to_set(
    self,
    *,
    attachments: Sequence[AttachmentUnionTypeDef],  # (1)
    attachmentSetId: str = ...,
) -> AddAttachmentsToSetResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AttachmentTypeDef](./type_defs.md#attachmenttypedef) [:material-code-braces: AttachmentOutputTypeDef](./type_defs.md#attachmentoutputtypedef) 
2. See [:material-code-braces: AddAttachmentsToSetResponseTypeDef](./type_defs.md#addattachmentstosetresponsetypedef) 


```python
# add_attachments_to_set method usage example with argument unpacking

kwargs: AddAttachmentsToSetRequestTypeDef = {  # (1)
    "attachments": ...,
}

parent.add_attachments_to_set(**kwargs)
```

1. See [:material-code-braces: AddAttachmentsToSetRequestTypeDef](./type_defs.md#addattachmentstosetrequesttypedef) 

### add\_communication\_to\_case

Adds additional customer communication to an Amazon Web Services Support case.

Type annotations and code completion for `#!python session.create_client("support").add_communication_to_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/add_communication_to_case.html)

```python
# add_communication_to_case method definition

await def add_communication_to_case(
    self,
    *,
    communicationBody: str,
    caseId: str = ...,
    ccEmailAddresses: Sequence[str] = ...,
    attachmentSetId: str = ...,
) -> AddCommunicationToCaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AddCommunicationToCaseResponseTypeDef](./type_defs.md#addcommunicationtocaseresponsetypedef) 


```python
# add_communication_to_case method usage example with argument unpacking

kwargs: AddCommunicationToCaseRequestTypeDef = {  # (1)
    "communicationBody": ...,
}

parent.add_communication_to_case(**kwargs)
```

1. See [:material-code-braces: AddCommunicationToCaseRequestTypeDef](./type_defs.md#addcommunicationtocaserequesttypedef) 

### create\_case

Creates a case in the Amazon Web Services Support Center.

Type annotations and code completion for `#!python session.create_client("support").create_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/create_case.html)

```python
# create_case method definition

await def create_case(
    self,
    *,
    subject: str,
    communicationBody: str,
    serviceCode: str = ...,
    severityCode: str = ...,
    categoryCode: str = ...,
    ccEmailAddresses: Sequence[str] = ...,
    language: str = ...,
    issueType: str = ...,
    attachmentSetId: str = ...,
) -> CreateCaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CreateCaseResponseTypeDef](./type_defs.md#createcaseresponsetypedef) 


```python
# create_case method usage example with argument unpacking

kwargs: CreateCaseRequestTypeDef = {  # (1)
    "subject": ...,
    "communicationBody": ...,
}

parent.create_case(**kwargs)
```

1. See [:material-code-braces: CreateCaseRequestTypeDef](./type_defs.md#createcaserequesttypedef) 

### describe\_attachment

Returns the attachment that has the specified ID.

Type annotations and code completion for `#!python session.create_client("support").describe_attachment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_attachment.html)

```python
# describe_attachment method definition

await def describe_attachment(
    self,
    *,
    attachmentId: str,
) -> DescribeAttachmentResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeAttachmentResponseTypeDef](./type_defs.md#describeattachmentresponsetypedef) 


```python
# describe_attachment method usage example with argument unpacking

kwargs: DescribeAttachmentRequestTypeDef = {  # (1)
    "attachmentId": ...,
}

parent.describe_attachment(**kwargs)
```

1. See [:material-code-braces: DescribeAttachmentRequestTypeDef](./type_defs.md#describeattachmentrequesttypedef) 

### describe\_cases

Returns a list of cases that you specify by passing one or more case IDs.

Type annotations and code completion for `#!python session.create_client("support").describe_cases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_cases.html)

```python
# describe_cases method definition

await def describe_cases(
    self,
    *,
    caseIdList: Sequence[str] = ...,
    displayId: str = ...,
    afterTime: str = ...,
    beforeTime: str = ...,
    includeResolvedCases: bool = ...,
    nextToken: str = ...,
    maxResults: int = ...,
    language: str = ...,
    includeCommunications: bool = ...,
) -> DescribeCasesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCasesResponseTypeDef](./type_defs.md#describecasesresponsetypedef) 


```python
# describe_cases method usage example with argument unpacking

kwargs: DescribeCasesRequestTypeDef = {  # (1)
    "caseIdList": ...,
}

parent.describe_cases(**kwargs)
```

1. See [:material-code-braces: DescribeCasesRequestTypeDef](./type_defs.md#describecasesrequesttypedef) 

### describe\_communications

Returns communications and attachments for one or more support cases.

Type annotations and code completion for `#!python session.create_client("support").describe_communications` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_communications.html)

```python
# describe_communications method definition

await def describe_communications(
    self,
    *,
    caseId: str,
    beforeTime: str = ...,
    afterTime: str = ...,
    nextToken: str = ...,
    maxResults: int = ...,
) -> DescribeCommunicationsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCommunicationsResponseTypeDef](./type_defs.md#describecommunicationsresponsetypedef) 


```python
# describe_communications method usage example with argument unpacking

kwargs: DescribeCommunicationsRequestTypeDef = {  # (1)
    "caseId": ...,
}

parent.describe_communications(**kwargs)
```

1. See [:material-code-braces: DescribeCommunicationsRequestTypeDef](./type_defs.md#describecommunicationsrequesttypedef) 

### describe\_create\_case\_options

Returns a list of CreateCaseOption types along with the corresponding supported
hours and language availability.

Type annotations and code completion for `#!python session.create_client("support").describe_create_case_options` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_create_case_options.html)

```python
# describe_create_case_options method definition

await def describe_create_case_options(
    self,
    *,
    issueType: str,
    serviceCode: str,
    language: str,
    categoryCode: str,
) -> DescribeCreateCaseOptionsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeCreateCaseOptionsResponseTypeDef](./type_defs.md#describecreatecaseoptionsresponsetypedef) 


```python
# describe_create_case_options method usage example with argument unpacking

kwargs: DescribeCreateCaseOptionsRequestTypeDef = {  # (1)
    "issueType": ...,
    "serviceCode": ...,
    "language": ...,
    "categoryCode": ...,
}

parent.describe_create_case_options(**kwargs)
```

1. See [:material-code-braces: DescribeCreateCaseOptionsRequestTypeDef](./type_defs.md#describecreatecaseoptionsrequesttypedef) 

### describe\_services

Returns the current list of Amazon Web Services services and a list of service
categories for each service.

Type annotations and code completion for `#!python session.create_client("support").describe_services` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_services.html)

```python
# describe_services method definition

await def describe_services(
    self,
    *,
    serviceCodeList: Sequence[str] = ...,
    language: str = ...,
) -> DescribeServicesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef) 


```python
# describe_services method usage example with argument unpacking

kwargs: DescribeServicesRequestTypeDef = {  # (1)
    "serviceCodeList": ...,
}

parent.describe_services(**kwargs)
```

1. See [:material-code-braces: DescribeServicesRequestTypeDef](./type_defs.md#describeservicesrequesttypedef) 

### describe\_severity\_levels

Returns the list of severity levels that you can assign to a support case.

Type annotations and code completion for `#!python session.create_client("support").describe_severity_levels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_severity_levels.html)

```python
# describe_severity_levels method definition

await def describe_severity_levels(
    self,
    *,
    language: str = ...,
) -> DescribeSeverityLevelsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSeverityLevelsResponseTypeDef](./type_defs.md#describeseveritylevelsresponsetypedef) 


```python
# describe_severity_levels method usage example with argument unpacking

kwargs: DescribeSeverityLevelsRequestTypeDef = {  # (1)
    "language": ...,
}

parent.describe_severity_levels(**kwargs)
```

1. See [:material-code-braces: DescribeSeverityLevelsRequestTypeDef](./type_defs.md#describeseveritylevelsrequesttypedef) 

### describe\_supported\_languages

Returns a list of supported languages for a specified
<code>categoryCode</code>, <code>issueType</code> and <code>serviceCode</code>.

Type annotations and code completion for `#!python session.create_client("support").describe_supported_languages` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_supported_languages.html)

```python
# describe_supported_languages method definition

await def describe_supported_languages(
    self,
    *,
    issueType: str,
    serviceCode: str,
    categoryCode: str,
) -> DescribeSupportedLanguagesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSupportedLanguagesResponseTypeDef](./type_defs.md#describesupportedlanguagesresponsetypedef) 


```python
# describe_supported_languages method usage example with argument unpacking

kwargs: DescribeSupportedLanguagesRequestTypeDef = {  # (1)
    "issueType": ...,
    "serviceCode": ...,
    "categoryCode": ...,
}

parent.describe_supported_languages(**kwargs)
```

1. See [:material-code-braces: DescribeSupportedLanguagesRequestTypeDef](./type_defs.md#describesupportedlanguagesrequesttypedef) 

### describe\_trusted\_advisor\_check\_refresh\_statuses

Returns the refresh status of the Trusted Advisor checks that have the
specified check IDs.

Type annotations and code completion for `#!python session.create_client("support").describe_trusted_advisor_check_refresh_statuses` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_trusted_advisor_check_refresh_statuses.html)

```python
# describe_trusted_advisor_check_refresh_statuses method definition

await def describe_trusted_advisor_check_refresh_statuses(
    self,
    *,
    checkIds: Sequence[str],
) -> DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef](./type_defs.md#describetrustedadvisorcheckrefreshstatusesresponsetypedef) 


```python
# describe_trusted_advisor_check_refresh_statuses method usage example with argument unpacking

kwargs: DescribeTrustedAdvisorCheckRefreshStatusesRequestTypeDef = {  # (1)
    "checkIds": ...,
}

parent.describe_trusted_advisor_check_refresh_statuses(**kwargs)
```

1. See [:material-code-braces: DescribeTrustedAdvisorCheckRefreshStatusesRequestTypeDef](./type_defs.md#describetrustedadvisorcheckrefreshstatusesrequesttypedef) 

### describe\_trusted\_advisor\_check\_result

Returns the results of the Trusted Advisor check that has the specified check
ID.

Type annotations and code completion for `#!python session.create_client("support").describe_trusted_advisor_check_result` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_trusted_advisor_check_result.html)

```python
# describe_trusted_advisor_check_result method definition

await def describe_trusted_advisor_check_result(
    self,
    *,
    checkId: str,
    language: str = ...,
) -> DescribeTrustedAdvisorCheckResultResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrustedAdvisorCheckResultResponseTypeDef](./type_defs.md#describetrustedadvisorcheckresultresponsetypedef) 


```python
# describe_trusted_advisor_check_result method usage example with argument unpacking

kwargs: DescribeTrustedAdvisorCheckResultRequestTypeDef = {  # (1)
    "checkId": ...,
}

parent.describe_trusted_advisor_check_result(**kwargs)
```

1. See [:material-code-braces: DescribeTrustedAdvisorCheckResultRequestTypeDef](./type_defs.md#describetrustedadvisorcheckresultrequesttypedef) 

### describe\_trusted\_advisor\_check\_summaries

Returns the results for the Trusted Advisor check summaries for the check IDs
that you specified.

Type annotations and code completion for `#!python session.create_client("support").describe_trusted_advisor_check_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_trusted_advisor_check_summaries.html)

```python
# describe_trusted_advisor_check_summaries method definition

await def describe_trusted_advisor_check_summaries(
    self,
    *,
    checkIds: Sequence[str],
) -> DescribeTrustedAdvisorCheckSummariesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrustedAdvisorCheckSummariesResponseTypeDef](./type_defs.md#describetrustedadvisorchecksummariesresponsetypedef) 


```python
# describe_trusted_advisor_check_summaries method usage example with argument unpacking

kwargs: DescribeTrustedAdvisorCheckSummariesRequestTypeDef = {  # (1)
    "checkIds": ...,
}

parent.describe_trusted_advisor_check_summaries(**kwargs)
```

1. See [:material-code-braces: DescribeTrustedAdvisorCheckSummariesRequestTypeDef](./type_defs.md#describetrustedadvisorchecksummariesrequesttypedef) 

### describe\_trusted\_advisor\_checks

Returns information about all available Trusted Advisor checks, including the
name, ID, category, description, and metadata.

Type annotations and code completion for `#!python session.create_client("support").describe_trusted_advisor_checks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/describe_trusted_advisor_checks.html)

```python
# describe_trusted_advisor_checks method definition

await def describe_trusted_advisor_checks(
    self,
    *,
    language: str,
) -> DescribeTrustedAdvisorChecksResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTrustedAdvisorChecksResponseTypeDef](./type_defs.md#describetrustedadvisorchecksresponsetypedef) 


```python
# describe_trusted_advisor_checks method usage example with argument unpacking

kwargs: DescribeTrustedAdvisorChecksRequestTypeDef = {  # (1)
    "language": ...,
}

parent.describe_trusted_advisor_checks(**kwargs)
```

1. See [:material-code-braces: DescribeTrustedAdvisorChecksRequestTypeDef](./type_defs.md#describetrustedadvisorchecksrequesttypedef) 

### refresh\_trusted\_advisor\_check

Refreshes the Trusted Advisor check that you specify using the check ID.

Type annotations and code completion for `#!python session.create_client("support").refresh_trusted_advisor_check` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/refresh_trusted_advisor_check.html)

```python
# refresh_trusted_advisor_check method definition

await def refresh_trusted_advisor_check(
    self,
    *,
    checkId: str,
) -> RefreshTrustedAdvisorCheckResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: RefreshTrustedAdvisorCheckResponseTypeDef](./type_defs.md#refreshtrustedadvisorcheckresponsetypedef) 


```python
# refresh_trusted_advisor_check method usage example with argument unpacking

kwargs: RefreshTrustedAdvisorCheckRequestTypeDef = {  # (1)
    "checkId": ...,
}

parent.refresh_trusted_advisor_check(**kwargs)
```

1. See [:material-code-braces: RefreshTrustedAdvisorCheckRequestTypeDef](./type_defs.md#refreshtrustedadvisorcheckrequesttypedef) 

### resolve\_case

Resolves a support case.

Type annotations and code completion for `#!python session.create_client("support").resolve_case` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support/client/resolve_case.html)

```python
# resolve_case method definition

await def resolve_case(
    self,
    *,
    caseId: str = ...,
) -> ResolveCaseResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ResolveCaseResponseTypeDef](./type_defs.md#resolvecaseresponsetypedef) 


```python
# resolve_case method usage example with argument unpacking

kwargs: ResolveCaseRequestTypeDef = {  # (1)
    "caseId": ...,
}

parent.resolve_case(**kwargs)
```

1. See [:material-code-braces: ResolveCaseRequestTypeDef](./type_defs.md#resolvecaserequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("support").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("support").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client)

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

Type annotations and code completion for `#!python session.create_client("support").get_paginator` method with overloads.

- `client.get_paginator("describe_cases")` -> [DescribeCasesPaginator](./paginators.md#describecasespaginator)
- `client.get_paginator("describe_communications")` -> [DescribeCommunicationsPaginator](./paginators.md#describecommunicationspaginator)




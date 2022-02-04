<a id="supportclient-for-aiobotocore-support-module"></a>

# SupportClient for aiobotocore Support module

> [Index](..) > [Support](.) > SupportClient

Auto-generated documentation for
[Support](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support)
type annotations stubs module
[types-aiobotocore-support](https://pypi.org/project/types-aiobotocore-support/).

- [SupportClient for aiobotocore Support module](#supportclient-for-aiobotocore-support-module)
  - [SupportClient](#supportclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [add_attachments_to_set](#add_attachments_to_set)
    - [add_communication_to_case](#add_communication_to_case)
    - [can_paginate](#can_paginate)
    - [create_case](#create_case)
    - [describe_attachment](#describe_attachment)
    - [describe_cases](#describe_cases)
    - [describe_communications](#describe_communications)
    - [describe_services](#describe_services)
    - [describe_severity_levels](#describe_severity_levels)
    - [describe_trusted_advisor_check_refresh_statuses](#describe_trusted_advisor_check_refresh_statuses)
    - [describe_trusted_advisor_check_result](#describe_trusted_advisor_check_result)
    - [describe_trusted_advisor_check_summaries](#describe_trusted_advisor_check_summaries)
    - [describe_trusted_advisor_checks](#describe_trusted_advisor_checks)
    - [generate_presigned_url](#generate_presigned_url)
    - [refresh_trusted_advisor_check](#refresh_trusted_advisor_check)
    - [resolve_case](#resolve_case)
    - [get_paginator](#get_paginator)

<a id="supportclient"></a>

## SupportClient

Type annotations for `aiobotocore.create_client("support")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_support.client import SupportClient

def get_support_client() -> SupportClient:
    return Session().client("support")
```

Boto3 documentation:
[Support.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_support.client import Exceptions

def handle_error(exc: Exceptions.AttachmentIdNotFound) -> None:
    ...
```

Exceptions:

- `Exceptions.AttachmentIdNotFound`
- `Exceptions.AttachmentLimitExceeded`
- `Exceptions.AttachmentSetExpired`
- `Exceptions.AttachmentSetIdNotFound`
- `Exceptions.AttachmentSetSizeLimitExceeded`
- `Exceptions.CaseCreationLimitExceeded`
- `Exceptions.CaseIdNotFound`
- `Exceptions.ClientError`
- `Exceptions.DescribeAttachmentLimitExceeded`
- `Exceptions.InternalServerError`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

SupportClient exceptions.

Type annotations for `aiobotocore.create_client("support").exceptions` method.

Boto3 documentation:
[Support.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="add_attachments_to_set"></a>

### add_attachments_to_set

Adds one or more attachments to an attachment set.

Type annotations for
`aiobotocore.create_client("support").add_attachments_to_set` method.

Boto3 documentation:
[Support.Client.add_attachments_to_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_attachments_to_set)

Asynchronous method. Use `await add_attachments_to_set(...)` for a synchronous
call.

Arguments mapping described in
[AddAttachmentsToSetRequestRequestTypeDef](./type_defs.md#addattachmentstosetrequestrequesttypedef).

Keyword-only arguments:

- `attachments`:
  `Sequence`\[[AttachmentTypeDef](./type_defs.md#attachmenttypedef)\]
  *(required)*
- `attachmentSetId`: `str`

Returns a `Coroutine` for
[AddAttachmentsToSetResponseTypeDef](./type_defs.md#addattachmentstosetresponsetypedef).

<a id="add_communication_to_case"></a>

### add_communication_to_case

Adds additional customer communication to an Amazon Web Services Support case.

Type annotations for
`aiobotocore.create_client("support").add_communication_to_case` method.

Boto3 documentation:
[Support.Client.add_communication_to_case](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.add_communication_to_case)

Asynchronous method. Use `await add_communication_to_case(...)` for a
synchronous call.

Arguments mapping described in
[AddCommunicationToCaseRequestRequestTypeDef](./type_defs.md#addcommunicationtocaserequestrequesttypedef).

Keyword-only arguments:

- `communicationBody`: `str` *(required)*
- `caseId`: `str`
- `ccEmailAddresses`: `Sequence`\[`str`\]
- `attachmentSetId`: `str`

Returns a `Coroutine` for
[AddCommunicationToCaseResponseTypeDef](./type_defs.md#addcommunicationtocaseresponsetypedef).

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("support").can_paginate`
method.

Boto3 documentation:
[Support.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_case"></a>

### create_case

Creates a case in the Amazon Web Services Support Center.

Type annotations for `aiobotocore.create_client("support").create_case` method.

Boto3 documentation:
[Support.Client.create_case](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.create_case)

Asynchronous method. Use `await create_case(...)` for a synchronous call.

Arguments mapping described in
[CreateCaseRequestRequestTypeDef](./type_defs.md#createcaserequestrequesttypedef).

Keyword-only arguments:

- `subject`: `str` *(required)*
- `communicationBody`: `str` *(required)*
- `serviceCode`: `str`
- `severityCode`: `str`
- `categoryCode`: `str`
- `ccEmailAddresses`: `Sequence`\[`str`\]
- `language`: `str`
- `issueType`: `str`
- `attachmentSetId`: `str`

Returns a `Coroutine` for
[CreateCaseResponseTypeDef](./type_defs.md#createcaseresponsetypedef).

<a id="describe_attachment"></a>

### describe_attachment

Returns the attachment that has the specified ID.

Type annotations for `aiobotocore.create_client("support").describe_attachment`
method.

Boto3 documentation:
[Support.Client.describe_attachment](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_attachment)

Asynchronous method. Use `await describe_attachment(...)` for a synchronous
call.

Arguments mapping described in
[DescribeAttachmentRequestRequestTypeDef](./type_defs.md#describeattachmentrequestrequesttypedef).

Keyword-only arguments:

- `attachmentId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeAttachmentResponseTypeDef](./type_defs.md#describeattachmentresponsetypedef).

<a id="describe_cases"></a>

### describe_cases

Returns a list of cases that you specify by passing one or more case IDs.

Type annotations for `aiobotocore.create_client("support").describe_cases`
method.

Boto3 documentation:
[Support.Client.describe_cases](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_cases)

Asynchronous method. Use `await describe_cases(...)` for a synchronous call.

Arguments mapping described in
[DescribeCasesRequestRequestTypeDef](./type_defs.md#describecasesrequestrequesttypedef).

Keyword-only arguments:

- `caseIdList`: `Sequence`\[`str`\]
- `displayId`: `str`
- `afterTime`: `str`
- `beforeTime`: `str`
- `includeResolvedCases`: `bool`
- `nextToken`: `str`
- `maxResults`: `int`
- `language`: `str`
- `includeCommunications`: `bool`

Returns a `Coroutine` for
[DescribeCasesResponseTypeDef](./type_defs.md#describecasesresponsetypedef).

<a id="describe_communications"></a>

### describe_communications

Returns communications and attachments for one or more support cases.

Type annotations for
`aiobotocore.create_client("support").describe_communications` method.

Boto3 documentation:
[Support.Client.describe_communications](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_communications)

Asynchronous method. Use `await describe_communications(...)` for a synchronous
call.

Arguments mapping described in
[DescribeCommunicationsRequestRequestTypeDef](./type_defs.md#describecommunicationsrequestrequesttypedef).

Keyword-only arguments:

- `caseId`: `str` *(required)*
- `beforeTime`: `str`
- `afterTime`: `str`
- `nextToken`: `str`
- `maxResults`: `int`

Returns a `Coroutine` for
[DescribeCommunicationsResponseTypeDef](./type_defs.md#describecommunicationsresponsetypedef).

<a id="describe_services"></a>

### describe_services

Returns the current list of Amazon Web Services services and a list of service
categories for each service.

Type annotations for `aiobotocore.create_client("support").describe_services`
method.

Boto3 documentation:
[Support.Client.describe_services](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_services)

Asynchronous method. Use `await describe_services(...)` for a synchronous call.

Arguments mapping described in
[DescribeServicesRequestRequestTypeDef](./type_defs.md#describeservicesrequestrequesttypedef).

Keyword-only arguments:

- `serviceCodeList`: `Sequence`\[`str`\]
- `language`: `str`

Returns a `Coroutine` for
[DescribeServicesResponseTypeDef](./type_defs.md#describeservicesresponsetypedef).

<a id="describe_severity_levels"></a>

### describe_severity_levels

Returns the list of severity levels that you can assign to a support case.

Type annotations for
`aiobotocore.create_client("support").describe_severity_levels` method.

Boto3 documentation:
[Support.Client.describe_severity_levels](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_severity_levels)

Asynchronous method. Use `await describe_severity_levels(...)` for a
synchronous call.

Arguments mapping described in
[DescribeSeverityLevelsRequestRequestTypeDef](./type_defs.md#describeseveritylevelsrequestrequesttypedef).

Keyword-only arguments:

- `language`: `str`

Returns a `Coroutine` for
[DescribeSeverityLevelsResponseTypeDef](./type_defs.md#describeseveritylevelsresponsetypedef).

<a id="describe_trusted_advisor_check_refresh_statuses"></a>

### describe_trusted_advisor_check_refresh_statuses

Returns the refresh status of the Trusted Advisor checks that have the
specified check IDs.

Type annotations for
`aiobotocore.create_client("support").describe_trusted_advisor_check_refresh_statuses`
method.

Boto3 documentation:
[Support.Client.describe_trusted_advisor_check_refresh_statuses](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_trusted_advisor_check_refresh_statuses)

Asynchronous method. Use
`await describe_trusted_advisor_check_refresh_statuses(...)` for a synchronous
call.

Arguments mapping described in
[DescribeTrustedAdvisorCheckRefreshStatusesRequestRequestTypeDef](./type_defs.md#describetrustedadvisorcheckrefreshstatusesrequestrequesttypedef).

Keyword-only arguments:

- `checkIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DescribeTrustedAdvisorCheckRefreshStatusesResponseTypeDef](./type_defs.md#describetrustedadvisorcheckrefreshstatusesresponsetypedef).

<a id="describe_trusted_advisor_check_result"></a>

### describe_trusted_advisor_check_result

Returns the results of the Trusted Advisor check that has the specified check
ID.

Type annotations for
`aiobotocore.create_client("support").describe_trusted_advisor_check_result`
method.

Boto3 documentation:
[Support.Client.describe_trusted_advisor_check_result](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_trusted_advisor_check_result)

Asynchronous method. Use `await describe_trusted_advisor_check_result(...)` for
a synchronous call.

Arguments mapping described in
[DescribeTrustedAdvisorCheckResultRequestRequestTypeDef](./type_defs.md#describetrustedadvisorcheckresultrequestrequesttypedef).

Keyword-only arguments:

- `checkId`: `str` *(required)*
- `language`: `str`

Returns a `Coroutine` for
[DescribeTrustedAdvisorCheckResultResponseTypeDef](./type_defs.md#describetrustedadvisorcheckresultresponsetypedef).

<a id="describe_trusted_advisor_check_summaries"></a>

### describe_trusted_advisor_check_summaries

Returns the results for the Trusted Advisor check summaries for the check IDs
that you specified.

Type annotations for
`aiobotocore.create_client("support").describe_trusted_advisor_check_summaries`
method.

Boto3 documentation:
[Support.Client.describe_trusted_advisor_check_summaries](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_trusted_advisor_check_summaries)

Asynchronous method. Use `await describe_trusted_advisor_check_summaries(...)`
for a synchronous call.

Arguments mapping described in
[DescribeTrustedAdvisorCheckSummariesRequestRequestTypeDef](./type_defs.md#describetrustedadvisorchecksummariesrequestrequesttypedef).

Keyword-only arguments:

- `checkIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DescribeTrustedAdvisorCheckSummariesResponseTypeDef](./type_defs.md#describetrustedadvisorchecksummariesresponsetypedef).

<a id="describe_trusted_advisor_checks"></a>

### describe_trusted_advisor_checks

Returns information about all available Trusted Advisor checks, including the
name, ID, category, description, and metadata.

Type annotations for
`aiobotocore.create_client("support").describe_trusted_advisor_checks` method.

Boto3 documentation:
[Support.Client.describe_trusted_advisor_checks](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.describe_trusted_advisor_checks)

Asynchronous method. Use `await describe_trusted_advisor_checks(...)` for a
synchronous call.

Arguments mapping described in
[DescribeTrustedAdvisorChecksRequestRequestTypeDef](./type_defs.md#describetrustedadvisorchecksrequestrequesttypedef).

Keyword-only arguments:

- `language`: `str` *(required)*

Returns a `Coroutine` for
[DescribeTrustedAdvisorChecksResponseTypeDef](./type_defs.md#describetrustedadvisorchecksresponsetypedef).

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("support").generate_presigned_url` method.

Boto3 documentation:
[Support.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="refresh_trusted_advisor_check"></a>

### refresh_trusted_advisor_check

Refreshes the Trusted Advisor check that you specify using the check ID.

Type annotations for
`aiobotocore.create_client("support").refresh_trusted_advisor_check` method.

Boto3 documentation:
[Support.Client.refresh_trusted_advisor_check](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.refresh_trusted_advisor_check)

Asynchronous method. Use `await refresh_trusted_advisor_check(...)` for a
synchronous call.

Arguments mapping described in
[RefreshTrustedAdvisorCheckRequestRequestTypeDef](./type_defs.md#refreshtrustedadvisorcheckrequestrequesttypedef).

Keyword-only arguments:

- `checkId`: `str` *(required)*

Returns a `Coroutine` for
[RefreshTrustedAdvisorCheckResponseTypeDef](./type_defs.md#refreshtrustedadvisorcheckresponsetypedef).

<a id="resolve_case"></a>

### resolve_case

Resolves a support case.

Type annotations for `aiobotocore.create_client("support").resolve_case`
method.

Boto3 documentation:
[Support.Client.resolve_case](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support.html#Support.Client.resolve_case)

Asynchronous method. Use `await resolve_case(...)` for a synchronous call.

Arguments mapping described in
[ResolveCaseRequestRequestTypeDef](./type_defs.md#resolvecaserequestrequesttypedef).

Keyword-only arguments:

- `caseId`: `str`

Returns a `Coroutine` for
[ResolveCaseResponseTypeDef](./type_defs.md#resolvecaseresponsetypedef).

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("support").get_paginator`
method with overloads.

- `client.get_paginator("describe_cases")` ->
  [DescribeCasesPaginator](./paginators.md#describecasespaginator)
- `client.get_paginator("describe_communications")` ->
  [DescribeCommunicationsPaginator](./paginators.md#describecommunicationspaginator)

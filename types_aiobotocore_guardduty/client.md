<a id="guarddutyclient-for-aiobotocore-guardduty-module"></a>

# GuardDutyClient for aiobotocore GuardDuty module

> [Index](..) > [GuardDuty](.) > GuardDutyClient

Auto-generated documentation for
[GuardDuty](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
type annotations stubs module
[types-aiobotocore-guardduty](https://pypi.org/project/types-aiobotocore-guardduty/).

- [GuardDutyClient for aiobotocore GuardDuty module](#guarddutyclient-for-aiobotocore-guardduty-module)
  - [GuardDutyClient](#guarddutyclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [accept_invitation](#accept_invitation)
    - [archive_findings](#archive_findings)
    - [can_paginate](#can_paginate)
    - [create_detector](#create_detector)
    - [create_filter](#create_filter)
    - [create_ip_set](#create_ip_set)
    - [create_members](#create_members)
    - [create_publishing_destination](#create_publishing_destination)
    - [create_sample_findings](#create_sample_findings)
    - [create_threat_intel_set](#create_threat_intel_set)
    - [decline_invitations](#decline_invitations)
    - [delete_detector](#delete_detector)
    - [delete_filter](#delete_filter)
    - [delete_invitations](#delete_invitations)
    - [delete_ip_set](#delete_ip_set)
    - [delete_members](#delete_members)
    - [delete_publishing_destination](#delete_publishing_destination)
    - [delete_threat_intel_set](#delete_threat_intel_set)
    - [describe_organization_configuration](#describe_organization_configuration)
    - [describe_publishing_destination](#describe_publishing_destination)
    - [disable_organization_admin_account](#disable_organization_admin_account)
    - [disassociate_from_master_account](#disassociate_from_master_account)
    - [disassociate_members](#disassociate_members)
    - [enable_organization_admin_account](#enable_organization_admin_account)
    - [generate_presigned_url](#generate_presigned_url)
    - [get_detector](#get_detector)
    - [get_filter](#get_filter)
    - [get_findings](#get_findings)
    - [get_findings_statistics](#get_findings_statistics)
    - [get_invitations_count](#get_invitations_count)
    - [get_ip_set](#get_ip_set)
    - [get_master_account](#get_master_account)
    - [get_member_detectors](#get_member_detectors)
    - [get_members](#get_members)
    - [get_threat_intel_set](#get_threat_intel_set)
    - [get_usage_statistics](#get_usage_statistics)
    - [invite_members](#invite_members)
    - [list_detectors](#list_detectors)
    - [list_filters](#list_filters)
    - [list_findings](#list_findings)
    - [list_invitations](#list_invitations)
    - [list_ip_sets](#list_ip_sets)
    - [list_members](#list_members)
    - [list_organization_admin_accounts](#list_organization_admin_accounts)
    - [list_publishing_destinations](#list_publishing_destinations)
    - [list_tags_for_resource](#list_tags_for_resource)
    - [list_threat_intel_sets](#list_threat_intel_sets)
    - [start_monitoring_members](#start_monitoring_members)
    - [stop_monitoring_members](#stop_monitoring_members)
    - [tag_resource](#tag_resource)
    - [unarchive_findings](#unarchive_findings)
    - [untag_resource](#untag_resource)
    - [update_detector](#update_detector)
    - [update_filter](#update_filter)
    - [update_findings_feedback](#update_findings_feedback)
    - [update_ip_set](#update_ip_set)
    - [update_member_detectors](#update_member_detectors)
    - [update_organization_configuration](#update_organization_configuration)
    - [update_publishing_destination](#update_publishing_destination)
    - [update_threat_intel_set](#update_threat_intel_set)
    - [get_paginator](#get_paginator)

<a id="guarddutyclient"></a>

## GuardDutyClient

Type annotations for `aiobotocore.create_client("guardduty")`

Can be used directly:

```python
from aiobotocore.session import Session
from types_aiobotocore_guardduty.client import GuardDutyClient

def get_guardduty_client() -> GuardDutyClient:
    return Session().client("guardduty")
```

Boto3 documentation:
[GuardDuty.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_guardduty.client import Exceptions

def handle_error(exc: Exceptions.BadRequestException) -> None:
    ...
```

Exceptions:

- `Exceptions.BadRequestException`
- `Exceptions.ClientError`
- `Exceptions.InternalServerErrorException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

GuardDutyClient exceptions.

Type annotations for `aiobotocore.create_client("guardduty").exceptions`
method.

Boto3 documentation:
[GuardDuty.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="accept_invitation"></a>

### accept_invitation

Accepts the invitation to be monitored by a GuardDuty administrator account.

Type annotations for `aiobotocore.create_client("guardduty").accept_invitation`
method.

Boto3 documentation:
[GuardDuty.Client.accept_invitation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.accept_invitation)

Asynchronous method. Use `await accept_invitation(...)` for a synchronous call.

Arguments mapping described in
[AcceptInvitationRequestRequestTypeDef](./type_defs.md#acceptinvitationrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `MasterId`: `str` *(required)*
- `InvitationId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="archive_findings"></a>

### archive_findings

Archives GuardDuty findings that are specified by the list of finding IDs.

Type annotations for `aiobotocore.create_client("guardduty").archive_findings`
method.

Boto3 documentation:
[GuardDuty.Client.archive_findings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.archive_findings)

Asynchronous method. Use `await archive_findings(...)` for a synchronous call.

Arguments mapping described in
[ArchiveFindingsRequestRequestTypeDef](./type_defs.md#archivefindingsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FindingIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="can_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `aiobotocore.create_client("guardduty").can_paginate`
method.

Boto3 documentation:
[GuardDuty.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.can_paginate)

Asynchronous method. Use `await can_paginate(...)` for a synchronous call.

Arguments:

- `operation_name`: `str` *(required)*

Returns a `Coroutine` for `bool`.

<a id="create_detector"></a>

### create_detector

Creates a single Amazon GuardDuty detector.

Type annotations for `aiobotocore.create_client("guardduty").create_detector`
method.

Boto3 documentation:
[GuardDuty.Client.create_detector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_detector)

Asynchronous method. Use `await create_detector(...)` for a synchronous call.

Arguments mapping described in
[CreateDetectorRequestRequestTypeDef](./type_defs.md#createdetectorrequestrequesttypedef).

Keyword-only arguments:

- `Enable`: `bool` *(required)*
- `ClientToken`: `str`
- `FindingPublishingFrequency`:
  [FindingPublishingFrequencyType](./literals.md#findingpublishingfrequencytype)
- `DataSources`:
  [DataSourceConfigurationsTypeDef](./type_defs.md#datasourceconfigurationstypedef)
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateDetectorResponseTypeDef](./type_defs.md#createdetectorresponsetypedef).

<a id="create_filter"></a>

### create_filter

Creates a filter using the specified finding criteria.

Type annotations for `aiobotocore.create_client("guardduty").create_filter`
method.

Boto3 documentation:
[GuardDuty.Client.create_filter](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_filter)

Asynchronous method. Use `await create_filter(...)` for a synchronous call.

Arguments mapping described in
[CreateFilterRequestRequestTypeDef](./type_defs.md#createfilterrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `Name`: `str` *(required)*
- `FindingCriteria`:
  [FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef) *(required)*
- `Description`: `str`
- `Action`: [FilterActionType](./literals.md#filteractiontype)
- `Rank`: `int`
- `ClientToken`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateFilterResponseTypeDef](./type_defs.md#createfilterresponsetypedef).

<a id="create_ip_set"></a>

### create_ip_set

Creates a new IPSet, which is called a trusted IP list in the console user
interface.

Type annotations for `aiobotocore.create_client("guardduty").create_ip_set`
method.

Boto3 documentation:
[GuardDuty.Client.create_ip_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_ip_set)

Asynchronous method. Use `await create_ip_set(...)` for a synchronous call.

Arguments mapping described in
[CreateIPSetRequestRequestTypeDef](./type_defs.md#createipsetrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `Name`: `str` *(required)*
- `Format`: [IpSetFormatType](./literals.md#ipsetformattype) *(required)*
- `Location`: `str` *(required)*
- `Activate`: `bool` *(required)*
- `ClientToken`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateIPSetResponseTypeDef](./type_defs.md#createipsetresponsetypedef).

<a id="create_members"></a>

### create_members

.

Type annotations for `aiobotocore.create_client("guardduty").create_members`
method.

Boto3 documentation:
[GuardDuty.Client.create_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_members)

Asynchronous method. Use `await create_members(...)` for a synchronous call.

Arguments mapping described in
[CreateMembersRequestRequestTypeDef](./type_defs.md#createmembersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountDetails`:
  `Sequence`\[[AccountDetailTypeDef](./type_defs.md#accountdetailtypedef)\]
  *(required)*

Returns a `Coroutine` for
[CreateMembersResponseTypeDef](./type_defs.md#createmembersresponsetypedef).

<a id="create_publishing_destination"></a>

### create_publishing_destination

Creates a publishing destination to export findings to.

Type annotations for
`aiobotocore.create_client("guardduty").create_publishing_destination` method.

Boto3 documentation:
[GuardDuty.Client.create_publishing_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_publishing_destination)

Asynchronous method. Use `await create_publishing_destination(...)` for a
synchronous call.

Arguments mapping described in
[CreatePublishingDestinationRequestRequestTypeDef](./type_defs.md#createpublishingdestinationrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `DestinationType`: `Literal['S3']` (see
  [DestinationTypeType](./literals.md#destinationtypetype)) *(required)*
- `DestinationProperties`:
  [DestinationPropertiesTypeDef](./type_defs.md#destinationpropertiestypedef)
  *(required)*
- `ClientToken`: `str`

Returns a `Coroutine` for
[CreatePublishingDestinationResponseTypeDef](./type_defs.md#createpublishingdestinationresponsetypedef).

<a id="create_sample_findings"></a>

### create_sample_findings

Generates example findings of types specified by the list of finding types.

Type annotations for
`aiobotocore.create_client("guardduty").create_sample_findings` method.

Boto3 documentation:
[GuardDuty.Client.create_sample_findings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_sample_findings)

Asynchronous method. Use `await create_sample_findings(...)` for a synchronous
call.

Arguments mapping described in
[CreateSampleFindingsRequestRequestTypeDef](./type_defs.md#createsamplefindingsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FindingTypes`: `Sequence`\[`str`\]

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="create_threat_intel_set"></a>

### create_threat_intel_set

Creates a new ThreatIntelSet.

Type annotations for
`aiobotocore.create_client("guardduty").create_threat_intel_set` method.

Boto3 documentation:
[GuardDuty.Client.create_threat_intel_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.create_threat_intel_set)

Asynchronous method. Use `await create_threat_intel_set(...)` for a synchronous
call.

Arguments mapping described in
[CreateThreatIntelSetRequestRequestTypeDef](./type_defs.md#createthreatintelsetrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `Name`: `str` *(required)*
- `Format`: [ThreatIntelSetFormatType](./literals.md#threatintelsetformattype)
  *(required)*
- `Location`: `str` *(required)*
- `Activate`: `bool` *(required)*
- `ClientToken`: `str`
- `Tags`: `Mapping`\[`str`, `str`\]

Returns a `Coroutine` for
[CreateThreatIntelSetResponseTypeDef](./type_defs.md#createthreatintelsetresponsetypedef).

<a id="decline_invitations"></a>

### decline_invitations

Declines invitations sent to the current member account by AWS accounts
specified by their account IDs.

Type annotations for
`aiobotocore.create_client("guardduty").decline_invitations` method.

Boto3 documentation:
[GuardDuty.Client.decline_invitations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.decline_invitations)

Asynchronous method. Use `await decline_invitations(...)` for a synchronous
call.

Arguments mapping described in
[DeclineInvitationsRequestRequestTypeDef](./type_defs.md#declineinvitationsrequestrequesttypedef).

Keyword-only arguments:

- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DeclineInvitationsResponseTypeDef](./type_defs.md#declineinvitationsresponsetypedef).

<a id="delete_detector"></a>

### delete_detector

Deletes an Amazon GuardDuty detector that is specified by the detector ID.

Type annotations for `aiobotocore.create_client("guardduty").delete_detector`
method.

Boto3 documentation:
[GuardDuty.Client.delete_detector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_detector)

Asynchronous method. Use `await delete_detector(...)` for a synchronous call.

Arguments mapping described in
[DeleteDetectorRequestRequestTypeDef](./type_defs.md#deletedetectorrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_filter"></a>

### delete_filter

Deletes the filter specified by the filter name.

Type annotations for `aiobotocore.create_client("guardduty").delete_filter`
method.

Boto3 documentation:
[GuardDuty.Client.delete_filter](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_filter)

Asynchronous method. Use `await delete_filter(...)` for a synchronous call.

Arguments mapping described in
[DeleteFilterRequestRequestTypeDef](./type_defs.md#deletefilterrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FilterName`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_invitations"></a>

### delete_invitations

Deletes invitations sent to the current member account by AWS accounts
specified by their account IDs.

Type annotations for
`aiobotocore.create_client("guardduty").delete_invitations` method.

Boto3 documentation:
[GuardDuty.Client.delete_invitations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_invitations)

Asynchronous method. Use `await delete_invitations(...)` for a synchronous
call.

Arguments mapping described in
[DeleteInvitationsRequestRequestTypeDef](./type_defs.md#deleteinvitationsrequestrequesttypedef).

Keyword-only arguments:

- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DeleteInvitationsResponseTypeDef](./type_defs.md#deleteinvitationsresponsetypedef).

<a id="delete_ip_set"></a>

### delete_ip_set

Deletes the IPSet specified by the `ipSetId`.

Type annotations for `aiobotocore.create_client("guardduty").delete_ip_set`
method.

Boto3 documentation:
[GuardDuty.Client.delete_ip_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_ip_set)

Asynchronous method. Use `await delete_ip_set(...)` for a synchronous call.

Arguments mapping described in
[DeleteIPSetRequestRequestTypeDef](./type_defs.md#deleteipsetrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `IpSetId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_members"></a>

### delete_members

Deletes GuardDuty member accounts (to the current GuardDuty administrator
account) specified by the account IDs.

Type annotations for `aiobotocore.create_client("guardduty").delete_members`
method.

Boto3 documentation:
[GuardDuty.Client.delete_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_members)

Asynchronous method. Use `await delete_members(...)` for a synchronous call.

Arguments mapping described in
[DeleteMembersRequestRequestTypeDef](./type_defs.md#deletemembersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DeleteMembersResponseTypeDef](./type_defs.md#deletemembersresponsetypedef).

<a id="delete_publishing_destination"></a>

### delete_publishing_destination

Deletes the publishing definition with the specified `destinationId` .

Type annotations for
`aiobotocore.create_client("guardduty").delete_publishing_destination` method.

Boto3 documentation:
[GuardDuty.Client.delete_publishing_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_publishing_destination)

Asynchronous method. Use `await delete_publishing_destination(...)` for a
synchronous call.

Arguments mapping described in
[DeletePublishingDestinationRequestRequestTypeDef](./type_defs.md#deletepublishingdestinationrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `DestinationId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="delete_threat_intel_set"></a>

### delete_threat_intel_set

Deletes the ThreatIntelSet specified by the ThreatIntelSet ID.

Type annotations for
`aiobotocore.create_client("guardduty").delete_threat_intel_set` method.

Boto3 documentation:
[GuardDuty.Client.delete_threat_intel_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.delete_threat_intel_set)

Asynchronous method. Use `await delete_threat_intel_set(...)` for a synchronous
call.

Arguments mapping described in
[DeleteThreatIntelSetRequestRequestTypeDef](./type_defs.md#deletethreatintelsetrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `ThreatIntelSetId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="describe_organization_configuration"></a>

### describe_organization_configuration

Returns information about the account selected as the delegated administrator
for GuardDuty.

Type annotations for
`aiobotocore.create_client("guardduty").describe_organization_configuration`
method.

Boto3 documentation:
[GuardDuty.Client.describe_organization_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.describe_organization_configuration)

Asynchronous method. Use `await describe_organization_configuration(...)` for a
synchronous call.

Arguments mapping described in
[DescribeOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#describeorganizationconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*

Returns a `Coroutine` for
[DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef).

<a id="describe_publishing_destination"></a>

### describe_publishing_destination

Returns information about the publishing destination specified by the provided
`destinationId` .

Type annotations for
`aiobotocore.create_client("guardduty").describe_publishing_destination`
method.

Boto3 documentation:
[GuardDuty.Client.describe_publishing_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.describe_publishing_destination)

Asynchronous method. Use `await describe_publishing_destination(...)` for a
synchronous call.

Arguments mapping described in
[DescribePublishingDestinationRequestRequestTypeDef](./type_defs.md#describepublishingdestinationrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `DestinationId`: `str` *(required)*

Returns a `Coroutine` for
[DescribePublishingDestinationResponseTypeDef](./type_defs.md#describepublishingdestinationresponsetypedef).

<a id="disable_organization_admin_account"></a>

### disable_organization_admin_account

Disables an AWS account within the Organization as the GuardDuty delegated
administrator.

Type annotations for
`aiobotocore.create_client("guardduty").disable_organization_admin_account`
method.

Boto3 documentation:
[GuardDuty.Client.disable_organization_admin_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.disable_organization_admin_account)

Asynchronous method. Use `await disable_organization_admin_account(...)` for a
synchronous call.

Arguments mapping described in
[DisableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#disableorganizationadminaccountrequestrequesttypedef).

Keyword-only arguments:

- `AdminAccountId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate_from_master_account"></a>

### disassociate_from_master_account

Disassociates the current GuardDuty member account from its administrator
account.

Type annotations for
`aiobotocore.create_client("guardduty").disassociate_from_master_account`
method.

Boto3 documentation:
[GuardDuty.Client.disassociate_from_master_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.disassociate_from_master_account)

Asynchronous method. Use `await disassociate_from_master_account(...)` for a
synchronous call.

Arguments mapping described in
[DisassociateFromMasterAccountRequestRequestTypeDef](./type_defs.md#disassociatefrommasteraccountrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="disassociate_members"></a>

### disassociate_members

Disassociates GuardDuty member accounts (to the current GuardDuty administrator
account) specified by the account IDs.

Type annotations for
`aiobotocore.create_client("guardduty").disassociate_members` method.

Boto3 documentation:
[GuardDuty.Client.disassociate_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.disassociate_members)

Asynchronous method. Use `await disassociate_members(...)` for a synchronous
call.

Arguments mapping described in
[DisassociateMembersRequestRequestTypeDef](./type_defs.md#disassociatemembersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[DisassociateMembersResponseTypeDef](./type_defs.md#disassociatemembersresponsetypedef).

<a id="enable_organization_admin_account"></a>

### enable_organization_admin_account

Enables an AWS account within the organization as the GuardDuty delegated
administrator.

Type annotations for
`aiobotocore.create_client("guardduty").enable_organization_admin_account`
method.

Boto3 documentation:
[GuardDuty.Client.enable_organization_admin_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.enable_organization_admin_account)

Asynchronous method. Use `await enable_organization_admin_account(...)` for a
synchronous call.

Arguments mapping described in
[EnableOrganizationAdminAccountRequestRequestTypeDef](./type_defs.md#enableorganizationadminaccountrequestrequesttypedef).

Keyword-only arguments:

- `AdminAccountId`: `str` *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="generate_presigned_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`aiobotocore.create_client("guardduty").generate_presigned_url` method.

Boto3 documentation:
[GuardDuty.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="get_detector"></a>

### get_detector

Retrieves an Amazon GuardDuty detector specified by the detectorId.

Type annotations for `aiobotocore.create_client("guardduty").get_detector`
method.

Boto3 documentation:
[GuardDuty.Client.get_detector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_detector)

Asynchronous method. Use `await get_detector(...)` for a synchronous call.

Arguments mapping described in
[GetDetectorRequestRequestTypeDef](./type_defs.md#getdetectorrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*

Returns a `Coroutine` for
[GetDetectorResponseTypeDef](./type_defs.md#getdetectorresponsetypedef).

<a id="get_filter"></a>

### get_filter

Returns the details of the filter specified by the filter name.

Type annotations for `aiobotocore.create_client("guardduty").get_filter`
method.

Boto3 documentation:
[GuardDuty.Client.get_filter](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_filter)

Asynchronous method. Use `await get_filter(...)` for a synchronous call.

Arguments mapping described in
[GetFilterRequestRequestTypeDef](./type_defs.md#getfilterrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FilterName`: `str` *(required)*

Returns a `Coroutine` for
[GetFilterResponseTypeDef](./type_defs.md#getfilterresponsetypedef).

<a id="get_findings"></a>

### get_findings

Describes Amazon GuardDuty findings specified by finding IDs.

Type annotations for `aiobotocore.create_client("guardduty").get_findings`
method.

Boto3 documentation:
[GuardDuty.Client.get_findings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings)

Asynchronous method. Use `await get_findings(...)` for a synchronous call.

Arguments mapping described in
[GetFindingsRequestRequestTypeDef](./type_defs.md#getfindingsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FindingIds`: `Sequence`\[`str`\] *(required)*
- `SortCriteria`: [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)

Returns a `Coroutine` for
[GetFindingsResponseTypeDef](./type_defs.md#getfindingsresponsetypedef).

<a id="get_findings_statistics"></a>

### get_findings_statistics

Lists Amazon GuardDuty findings statistics for the specified detector ID.

Type annotations for
`aiobotocore.create_client("guardduty").get_findings_statistics` method.

Boto3 documentation:
[GuardDuty.Client.get_findings_statistics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)

Asynchronous method. Use `await get_findings_statistics(...)` for a synchronous
call.

Arguments mapping described in
[GetFindingsStatisticsRequestRequestTypeDef](./type_defs.md#getfindingsstatisticsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FindingStatisticTypes`: `Sequence`\[`Literal['COUNT_BY_SEVERITY']` (see
  [FindingStatisticTypeType](./literals.md#findingstatistictypetype))\]
  *(required)*
- `FindingCriteria`:
  [FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef)

Returns a `Coroutine` for
[GetFindingsStatisticsResponseTypeDef](./type_defs.md#getfindingsstatisticsresponsetypedef).

<a id="get_invitations_count"></a>

### get_invitations_count

Returns the count of all GuardDuty membership invitations that were sent to the
current member account except the currently accepted invitation.

Type annotations for
`aiobotocore.create_client("guardduty").get_invitations_count` method.

Boto3 documentation:
[GuardDuty.Client.get_invitations_count](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_invitations_count)

Asynchronous method. Use `await get_invitations_count(...)` for a synchronous
call.

Returns a `Coroutine` for
[GetInvitationsCountResponseTypeDef](./type_defs.md#getinvitationscountresponsetypedef).

<a id="get_ip_set"></a>

### get_ip_set

Retrieves the IPSet specified by the `ipSetId` .

Type annotations for `aiobotocore.create_client("guardduty").get_ip_set`
method.

Boto3 documentation:
[GuardDuty.Client.get_ip_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_ip_set)

Asynchronous method. Use `await get_ip_set(...)` for a synchronous call.

Arguments mapping described in
[GetIPSetRequestRequestTypeDef](./type_defs.md#getipsetrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `IpSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetIPSetResponseTypeDef](./type_defs.md#getipsetresponsetypedef).

<a id="get_master_account"></a>

### get_master_account

Provides the details for the GuardDuty administrator account associated with
the current GuardDuty member account.

Type annotations for
`aiobotocore.create_client("guardduty").get_master_account` method.

Boto3 documentation:
[GuardDuty.Client.get_master_account](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_master_account)

Asynchronous method. Use `await get_master_account(...)` for a synchronous
call.

Arguments mapping described in
[GetMasterAccountRequestRequestTypeDef](./type_defs.md#getmasteraccountrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*

Returns a `Coroutine` for
[GetMasterAccountResponseTypeDef](./type_defs.md#getmasteraccountresponsetypedef).

<a id="get_member_detectors"></a>

### get_member_detectors

Describes which data sources are enabled for the member account's detector.

Type annotations for
`aiobotocore.create_client("guardduty").get_member_detectors` method.

Boto3 documentation:
[GuardDuty.Client.get_member_detectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_member_detectors)

Asynchronous method. Use `await get_member_detectors(...)` for a synchronous
call.

Arguments mapping described in
[GetMemberDetectorsRequestRequestTypeDef](./type_defs.md#getmemberdetectorsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[GetMemberDetectorsResponseTypeDef](./type_defs.md#getmemberdetectorsresponsetypedef).

<a id="get_members"></a>

### get_members

Retrieves GuardDuty member accounts (of the current GuardDuty administrator
account) specified by the account IDs.

Type annotations for `aiobotocore.create_client("guardduty").get_members`
method.

Boto3 documentation:
[GuardDuty.Client.get_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_members)

Asynchronous method. Use `await get_members(...)` for a synchronous call.

Arguments mapping described in
[GetMembersRequestRequestTypeDef](./type_defs.md#getmembersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[GetMembersResponseTypeDef](./type_defs.md#getmembersresponsetypedef).

<a id="get_threat_intel_set"></a>

### get_threat_intel_set

Retrieves the ThreatIntelSet that is specified by the ThreatIntelSet ID.

Type annotations for
`aiobotocore.create_client("guardduty").get_threat_intel_set` method.

Boto3 documentation:
[GuardDuty.Client.get_threat_intel_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_threat_intel_set)

Asynchronous method. Use `await get_threat_intel_set(...)` for a synchronous
call.

Arguments mapping described in
[GetThreatIntelSetRequestRequestTypeDef](./type_defs.md#getthreatintelsetrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `ThreatIntelSetId`: `str` *(required)*

Returns a `Coroutine` for
[GetThreatIntelSetResponseTypeDef](./type_defs.md#getthreatintelsetresponsetypedef).

<a id="get_usage_statistics"></a>

### get_usage_statistics

Lists Amazon GuardDuty usage statistics over the last 30 days for the specified
detector ID.

Type annotations for
`aiobotocore.create_client("guardduty").get_usage_statistics` method.

Boto3 documentation:
[GuardDuty.Client.get_usage_statistics](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_usage_statistics)

Asynchronous method. Use `await get_usage_statistics(...)` for a synchronous
call.

Arguments mapping described in
[GetUsageStatisticsRequestRequestTypeDef](./type_defs.md#getusagestatisticsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `UsageStatisticType`:
  [UsageStatisticTypeType](./literals.md#usagestatistictypetype) *(required)*
- `UsageCriteria`: [UsageCriteriaTypeDef](./type_defs.md#usagecriteriatypedef)
  *(required)*
- `Unit`: `str`
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[GetUsageStatisticsResponseTypeDef](./type_defs.md#getusagestatisticsresponsetypedef).

<a id="invite_members"></a>

### invite_members

Invites other AWS accounts (created as members of the current AWS account by
CreateMembers) to enable GuardDuty, and allow the current AWS account to view
and manage these accounts' findings on their behalf as the GuardDuty
administrator account.

Type annotations for `aiobotocore.create_client("guardduty").invite_members`
method.

Boto3 documentation:
[GuardDuty.Client.invite_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.invite_members)

Asynchronous method. Use `await invite_members(...)` for a synchronous call.

Arguments mapping described in
[InviteMembersRequestRequestTypeDef](./type_defs.md#invitemembersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*
- `DisableEmailNotification`: `bool`
- `Message`: `str`

Returns a `Coroutine` for
[InviteMembersResponseTypeDef](./type_defs.md#invitemembersresponsetypedef).

<a id="list_detectors"></a>

### list_detectors

Lists detectorIds of all the existing Amazon GuardDuty detector resources.

Type annotations for `aiobotocore.create_client("guardduty").list_detectors`
method.

Boto3 documentation:
[GuardDuty.Client.list_detectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_detectors)

Asynchronous method. Use `await list_detectors(...)` for a synchronous call.

Arguments mapping described in
[ListDetectorsRequestRequestTypeDef](./type_defs.md#listdetectorsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListDetectorsResponseTypeDef](./type_defs.md#listdetectorsresponsetypedef).

<a id="list_filters"></a>

### list_filters

Returns a paginated list of the current filters.

Type annotations for `aiobotocore.create_client("guardduty").list_filters`
method.

Boto3 documentation:
[GuardDuty.Client.list_filters](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_filters)

Asynchronous method. Use `await list_filters(...)` for a synchronous call.

Arguments mapping described in
[ListFiltersRequestRequestTypeDef](./type_defs.md#listfiltersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef).

<a id="list_findings"></a>

### list_findings

Lists Amazon GuardDuty findings for the specified detector ID.

Type annotations for `aiobotocore.create_client("guardduty").list_findings`
method.

Boto3 documentation:
[GuardDuty.Client.list_findings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_findings)

Asynchronous method. Use `await list_findings(...)` for a synchronous call.

Arguments mapping described in
[ListFindingsRequestRequestTypeDef](./type_defs.md#listfindingsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FindingCriteria`:
  [FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef)
- `SortCriteria`: [SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef)
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef).

<a id="list_invitations"></a>

### list_invitations

Lists all GuardDuty membership invitations that were sent to the current AWS
account.

Type annotations for `aiobotocore.create_client("guardduty").list_invitations`
method.

Boto3 documentation:
[GuardDuty.Client.list_invitations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_invitations)

Asynchronous method. Use `await list_invitations(...)` for a synchronous call.

Arguments mapping described in
[ListInvitationsRequestRequestTypeDef](./type_defs.md#listinvitationsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListInvitationsResponseTypeDef](./type_defs.md#listinvitationsresponsetypedef).

<a id="list_ip_sets"></a>

### list_ip_sets

Lists the IPSets of the GuardDuty service specified by the detector ID.

Type annotations for `aiobotocore.create_client("guardduty").list_ip_sets`
method.

Boto3 documentation:
[GuardDuty.Client.list_ip_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_ip_sets)

Asynchronous method. Use `await list_ip_sets(...)` for a synchronous call.

Arguments mapping described in
[ListIPSetsRequestRequestTypeDef](./type_defs.md#listipsetsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListIPSetsResponseTypeDef](./type_defs.md#listipsetsresponsetypedef).

<a id="list_members"></a>

### list_members

Lists details about all member accounts for the current GuardDuty administrator
account.

Type annotations for `aiobotocore.create_client("guardduty").list_members`
method.

Boto3 documentation:
[GuardDuty.Client.list_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_members)

Asynchronous method. Use `await list_members(...)` for a synchronous call.

Arguments mapping described in
[ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`
- `OnlyAssociated`: `str`

Returns a `Coroutine` for
[ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef).

<a id="list_organization_admin_accounts"></a>

### list_organization_admin_accounts

Lists the accounts configured as GuardDuty delegated administrators.

Type annotations for
`aiobotocore.create_client("guardduty").list_organization_admin_accounts`
method.

Boto3 documentation:
[GuardDuty.Client.list_organization_admin_accounts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_organization_admin_accounts)

Asynchronous method. Use `await list_organization_admin_accounts(...)` for a
synchronous call.

Arguments mapping described in
[ListOrganizationAdminAccountsRequestRequestTypeDef](./type_defs.md#listorganizationadminaccountsrequestrequesttypedef).

Keyword-only arguments:

- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListOrganizationAdminAccountsResponseTypeDef](./type_defs.md#listorganizationadminaccountsresponsetypedef).

<a id="list_publishing_destinations"></a>

### list_publishing_destinations

Returns a list of publishing destinations associated with the specified
`dectectorId` .

Type annotations for
`aiobotocore.create_client("guardduty").list_publishing_destinations` method.

Boto3 documentation:
[GuardDuty.Client.list_publishing_destinations](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_publishing_destinations)

Asynchronous method. Use `await list_publishing_destinations(...)` for a
synchronous call.

Arguments mapping described in
[ListPublishingDestinationsRequestRequestTypeDef](./type_defs.md#listpublishingdestinationsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListPublishingDestinationsResponseTypeDef](./type_defs.md#listpublishingdestinationsresponsetypedef).

<a id="list_tags_for_resource"></a>

### list_tags_for_resource

Lists tags for a resource.

Type annotations for
`aiobotocore.create_client("guardduty").list_tags_for_resource` method.

Boto3 documentation:
[GuardDuty.Client.list_tags_for_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_tags_for_resource)

Asynchronous method. Use `await list_tags_for_resource(...)` for a synchronous
call.

Arguments mapping described in
[ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*

Returns a `Coroutine` for
[ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef).

<a id="list_threat_intel_sets"></a>

### list_threat_intel_sets

Lists the ThreatIntelSets of the GuardDuty service specified by the detector
ID.

Type annotations for
`aiobotocore.create_client("guardduty").list_threat_intel_sets` method.

Boto3 documentation:
[GuardDuty.Client.list_threat_intel_sets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_threat_intel_sets)

Asynchronous method. Use `await list_threat_intel_sets(...)` for a synchronous
call.

Arguments mapping described in
[ListThreatIntelSetsRequestRequestTypeDef](./type_defs.md#listthreatintelsetsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `MaxResults`: `int`
- `NextToken`: `str`

Returns a `Coroutine` for
[ListThreatIntelSetsResponseTypeDef](./type_defs.md#listthreatintelsetsresponsetypedef).

<a id="start_monitoring_members"></a>

### start_monitoring_members

Turns on GuardDuty monitoring of the specified member accounts.

Type annotations for
`aiobotocore.create_client("guardduty").start_monitoring_members` method.

Boto3 documentation:
[GuardDuty.Client.start_monitoring_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.start_monitoring_members)

Asynchronous method. Use `await start_monitoring_members(...)` for a
synchronous call.

Arguments mapping described in
[StartMonitoringMembersRequestRequestTypeDef](./type_defs.md#startmonitoringmembersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[StartMonitoringMembersResponseTypeDef](./type_defs.md#startmonitoringmembersresponsetypedef).

<a id="stop_monitoring_members"></a>

### stop_monitoring_members

Stops GuardDuty monitoring for the specified member accounts.

Type annotations for
`aiobotocore.create_client("guardduty").stop_monitoring_members` method.

Boto3 documentation:
[GuardDuty.Client.stop_monitoring_members](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.stop_monitoring_members)

Asynchronous method. Use `await stop_monitoring_members(...)` for a synchronous
call.

Arguments mapping described in
[StopMonitoringMembersRequestRequestTypeDef](./type_defs.md#stopmonitoringmembersrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for
[StopMonitoringMembersResponseTypeDef](./type_defs.md#stopmonitoringmembersresponsetypedef).

<a id="tag_resource"></a>

### tag_resource

Adds tags to a resource.

Type annotations for `aiobotocore.create_client("guardduty").tag_resource`
method.

Boto3 documentation:
[GuardDuty.Client.tag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.tag_resource)

Asynchronous method. Use `await tag_resource(...)` for a synchronous call.

Arguments mapping described in
[TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `Tags`: `Mapping`\[`str`, `str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="unarchive_findings"></a>

### unarchive_findings

Unarchives GuardDuty findings specified by the `findingIds` .

Type annotations for
`aiobotocore.create_client("guardduty").unarchive_findings` method.

Boto3 documentation:
[GuardDuty.Client.unarchive_findings](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.unarchive_findings)

Asynchronous method. Use `await unarchive_findings(...)` for a synchronous
call.

Arguments mapping described in
[UnarchiveFindingsRequestRequestTypeDef](./type_defs.md#unarchivefindingsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FindingIds`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="untag_resource"></a>

### untag_resource

Removes tags from a resource.

Type annotations for `aiobotocore.create_client("guardduty").untag_resource`
method.

Boto3 documentation:
[GuardDuty.Client.untag_resource](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.untag_resource)

Asynchronous method. Use `await untag_resource(...)` for a synchronous call.

Arguments mapping described in
[UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef).

Keyword-only arguments:

- `ResourceArn`: `str` *(required)*
- `TagKeys`: `Sequence`\[`str`\] *(required)*

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_detector"></a>

### update_detector

Updates the Amazon GuardDuty detector specified by the detectorId.

Type annotations for `aiobotocore.create_client("guardduty").update_detector`
method.

Boto3 documentation:
[GuardDuty.Client.update_detector](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_detector)

Asynchronous method. Use `await update_detector(...)` for a synchronous call.

Arguments mapping described in
[UpdateDetectorRequestRequestTypeDef](./type_defs.md#updatedetectorrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `Enable`: `bool`
- `FindingPublishingFrequency`:
  [FindingPublishingFrequencyType](./literals.md#findingpublishingfrequencytype)
- `DataSources`:
  [DataSourceConfigurationsTypeDef](./type_defs.md#datasourceconfigurationstypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_filter"></a>

### update_filter

Updates the filter specified by the filter name.

Type annotations for `aiobotocore.create_client("guardduty").update_filter`
method.

Boto3 documentation:
[GuardDuty.Client.update_filter](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)

Asynchronous method. Use `await update_filter(...)` for a synchronous call.

Arguments mapping described in
[UpdateFilterRequestRequestTypeDef](./type_defs.md#updatefilterrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FilterName`: `str` *(required)*
- `Description`: `str`
- `Action`: [FilterActionType](./literals.md#filteractiontype)
- `Rank`: `int`
- `FindingCriteria`:
  [FindingCriteriaTypeDef](./type_defs.md#findingcriteriatypedef)

Returns a `Coroutine` for
[UpdateFilterResponseTypeDef](./type_defs.md#updatefilterresponsetypedef).

<a id="update_findings_feedback"></a>

### update_findings_feedback

Marks the specified GuardDuty findings as useful or not useful.

Type annotations for
`aiobotocore.create_client("guardduty").update_findings_feedback` method.

Boto3 documentation:
[GuardDuty.Client.update_findings_feedback](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_findings_feedback)

Asynchronous method. Use `await update_findings_feedback(...)` for a
synchronous call.

Arguments mapping described in
[UpdateFindingsFeedbackRequestRequestTypeDef](./type_defs.md#updatefindingsfeedbackrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `FindingIds`: `Sequence`\[`str`\] *(required)*
- `Feedback`: [FeedbackType](./literals.md#feedbacktype) *(required)*
- `Comments`: `str`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_ip_set"></a>

### update_ip_set

Updates the IPSet specified by the IPSet ID.

Type annotations for `aiobotocore.create_client("guardduty").update_ip_set`
method.

Boto3 documentation:
[GuardDuty.Client.update_ip_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_ip_set)

Asynchronous method. Use `await update_ip_set(...)` for a synchronous call.

Arguments mapping described in
[UpdateIPSetRequestRequestTypeDef](./type_defs.md#updateipsetrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `IpSetId`: `str` *(required)*
- `Name`: `str`
- `Location`: `str`
- `Activate`: `bool`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_member_detectors"></a>

### update_member_detectors

Contains information on member accounts to be updated.

Type annotations for
`aiobotocore.create_client("guardduty").update_member_detectors` method.

Boto3 documentation:
[GuardDuty.Client.update_member_detectors](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_member_detectors)

Asynchronous method. Use `await update_member_detectors(...)` for a synchronous
call.

Arguments mapping described in
[UpdateMemberDetectorsRequestRequestTypeDef](./type_defs.md#updatememberdetectorsrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AccountIds`: `Sequence`\[`str`\] *(required)*
- `DataSources`:
  [DataSourceConfigurationsTypeDef](./type_defs.md#datasourceconfigurationstypedef)

Returns a `Coroutine` for
[UpdateMemberDetectorsResponseTypeDef](./type_defs.md#updatememberdetectorsresponsetypedef).

<a id="update_organization_configuration"></a>

### update_organization_configuration

Updates the delegated administrator account with the values provided.

Type annotations for
`aiobotocore.create_client("guardduty").update_organization_configuration`
method.

Boto3 documentation:
[GuardDuty.Client.update_organization_configuration](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_organization_configuration)

Asynchronous method. Use `await update_organization_configuration(...)` for a
synchronous call.

Arguments mapping described in
[UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `AutoEnable`: `bool` *(required)*
- `DataSources`:
  [OrganizationDataSourceConfigurationsTypeDef](./type_defs.md#organizationdatasourceconfigurationstypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_publishing_destination"></a>

### update_publishing_destination

Updates information about the publishing destination specified by the
`destinationId` .

Type annotations for
`aiobotocore.create_client("guardduty").update_publishing_destination` method.

Boto3 documentation:
[GuardDuty.Client.update_publishing_destination](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_publishing_destination)

Asynchronous method. Use `await update_publishing_destination(...)` for a
synchronous call.

Arguments mapping described in
[UpdatePublishingDestinationRequestRequestTypeDef](./type_defs.md#updatepublishingdestinationrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `DestinationId`: `str` *(required)*
- `DestinationProperties`:
  [DestinationPropertiesTypeDef](./type_defs.md#destinationpropertiestypedef)

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="update_threat_intel_set"></a>

### update_threat_intel_set

Updates the ThreatIntelSet specified by the ThreatIntelSet ID.

Type annotations for
`aiobotocore.create_client("guardduty").update_threat_intel_set` method.

Boto3 documentation:
[GuardDuty.Client.update_threat_intel_set](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_threat_intel_set)

Asynchronous method. Use `await update_threat_intel_set(...)` for a synchronous
call.

Arguments mapping described in
[UpdateThreatIntelSetRequestRequestTypeDef](./type_defs.md#updatethreatintelsetrequestrequesttypedef).

Keyword-only arguments:

- `DetectorId`: `str` *(required)*
- `ThreatIntelSetId`: `str` *(required)*
- `Name`: `str`
- `Location`: `str`
- `Activate`: `bool`

Returns a `Coroutine` for `Dict`\[`str`, `Any`\].

<a id="get_paginator"></a>

### get_paginator

Type annotations for `aiobotocore.create_client("guardduty").get_paginator`
method with overloads.

- `client.get_paginator("list_detectors")` ->
  [ListDetectorsPaginator](./paginators.md#listdetectorspaginator)
- `client.get_paginator("list_filters")` ->
  [ListFiltersPaginator](./paginators.md#listfilterspaginator)
- `client.get_paginator("list_findings")` ->
  [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- `client.get_paginator("list_ip_sets")` ->
  [ListIPSetsPaginator](./paginators.md#listipsetspaginator)
- `client.get_paginator("list_invitations")` ->
  [ListInvitationsPaginator](./paginators.md#listinvitationspaginator)
- `client.get_paginator("list_members")` ->
  [ListMembersPaginator](./paginators.md#listmemberspaginator)
- `client.get_paginator("list_organization_admin_accounts")` ->
  [ListOrganizationAdminAccountsPaginator](./paginators.md#listorganizationadminaccountspaginator)
- `client.get_paginator("list_threat_intel_sets")` ->
  [ListThreatIntelSetsPaginator](./paginators.md#listthreatintelsetspaginator)

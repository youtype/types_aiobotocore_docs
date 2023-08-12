# Inspector2Client

> [Index](../README.md) > [Inspector2](./README.md) > Inspector2Client

!!! note ""

    Auto-generated documentation for [Inspector2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
    type annotations stubs module [types-aiobotocore-inspector2](https://pypi.org/project/types-aiobotocore-inspector2/).

## Inspector2Client

Type annotations and code completion for `#!python session.create_client("inspector2")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client)

```python
Inspector2Client usage example

from aiobotocore.session import get_session
from types_aiobotocore_inspector2.client import Inspector2Client

session = get_session()
async with session.create_client("inspector2") as client:
    client: Inspector2Client
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("inspector2").exceptions` structure.

```python
Inspector2Client.exceptions usage example

async with session.create_client("inspector2") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.BadRequestException,
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
Inspector2Client usage type checking example

from types_aiobotocore_inspector2.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### associate\_member

Associates an Amazon Web Services account with an Amazon Inspector delegated
administrator.

Type annotations and code completion for `#!python session.create_client("inspector2").associate_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.associate_member)

```python
# associate_member method definition

await def associate_member(
    self,
    *,
    accountId: str,
) -> AssociateMemberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: AssociateMemberResponseTypeDef](./type_defs.md#associatememberresponsetypedef) 


```python
# associate_member method usage example with argument unpacking

kwargs: AssociateMemberRequestRequestTypeDef = {  # (1)
    "accountId": ...,
}

parent.associate_member(**kwargs)
```

1. See [:material-code-braces: AssociateMemberRequestRequestTypeDef](./type_defs.md#associatememberrequestrequesttypedef) 

### batch\_get\_account\_status

Retrieves the Amazon Inspector status of multiple Amazon Web Services accounts
within your environment.

Type annotations and code completion for `#!python session.create_client("inspector2").batch_get_account_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_account_status)

```python
# batch_get_account_status method definition

await def batch_get_account_status(
    self,
    *,
    accountIds: Sequence[str] = ...,
) -> BatchGetAccountStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetAccountStatusResponseTypeDef](./type_defs.md#batchgetaccountstatusresponsetypedef) 


```python
# batch_get_account_status method usage example with argument unpacking

kwargs: BatchGetAccountStatusRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.batch_get_account_status(**kwargs)
```

1. See [:material-code-braces: BatchGetAccountStatusRequestRequestTypeDef](./type_defs.md#batchgetaccountstatusrequestrequesttypedef) 

### batch\_get\_code\_snippet

Retrieves code snippets from findings that Amazon Inspector detected code
vulnerabilities in.

Type annotations and code completion for `#!python session.create_client("inspector2").batch_get_code_snippet` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_code_snippet)

```python
# batch_get_code_snippet method definition

await def batch_get_code_snippet(
    self,
    *,
    findingArns: Sequence[str],
) -> BatchGetCodeSnippetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetCodeSnippetResponseTypeDef](./type_defs.md#batchgetcodesnippetresponsetypedef) 


```python
# batch_get_code_snippet method usage example with argument unpacking

kwargs: BatchGetCodeSnippetRequestRequestTypeDef = {  # (1)
    "findingArns": ...,
}

parent.batch_get_code_snippet(**kwargs)
```

1. See [:material-code-braces: BatchGetCodeSnippetRequestRequestTypeDef](./type_defs.md#batchgetcodesnippetrequestrequesttypedef) 

### batch\_get\_finding\_details

Gets vulnerability details for findings.

Type annotations and code completion for `#!python session.create_client("inspector2").batch_get_finding_details` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_finding_details)

```python
# batch_get_finding_details method definition

await def batch_get_finding_details(
    self,
    *,
    findingArns: Sequence[str],
) -> BatchGetFindingDetailsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetFindingDetailsResponseTypeDef](./type_defs.md#batchgetfindingdetailsresponsetypedef) 


```python
# batch_get_finding_details method usage example with argument unpacking

kwargs: BatchGetFindingDetailsRequestRequestTypeDef = {  # (1)
    "findingArns": ...,
}

parent.batch_get_finding_details(**kwargs)
```

1. See [:material-code-braces: BatchGetFindingDetailsRequestRequestTypeDef](./type_defs.md#batchgetfindingdetailsrequestrequesttypedef) 

### batch\_get\_free\_trial\_info

Gets free trial status for multiple Amazon Web Services accounts.

Type annotations and code completion for `#!python session.create_client("inspector2").batch_get_free_trial_info` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_free_trial_info)

```python
# batch_get_free_trial_info method definition

await def batch_get_free_trial_info(
    self,
    *,
    accountIds: Sequence[str],
) -> BatchGetFreeTrialInfoResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetFreeTrialInfoResponseTypeDef](./type_defs.md#batchgetfreetrialinforesponsetypedef) 


```python
# batch_get_free_trial_info method usage example with argument unpacking

kwargs: BatchGetFreeTrialInfoRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.batch_get_free_trial_info(**kwargs)
```

1. See [:material-code-braces: BatchGetFreeTrialInfoRequestRequestTypeDef](./type_defs.md#batchgetfreetrialinforequestrequesttypedef) 

### batch\_get\_member\_ec2\_deep\_inspection\_status

Retrieves Amazon Inspector deep inspection activation status of multiple member
accounts within your organization.

Type annotations and code completion for `#!python session.create_client("inspector2").batch_get_member_ec2_deep_inspection_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_get_member_ec2_deep_inspection_status)

```python
# batch_get_member_ec2_deep_inspection_status method definition

await def batch_get_member_ec2_deep_inspection_status(
    self,
    *,
    accountIds: Sequence[str] = ...,
) -> BatchGetMemberEc2DeepInspectionStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchGetMemberEc2DeepInspectionStatusResponseTypeDef](./type_defs.md#batchgetmemberec2deepinspectionstatusresponsetypedef) 


```python
# batch_get_member_ec2_deep_inspection_status method usage example with argument unpacking

kwargs: BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.batch_get_member_ec2_deep_inspection_status(**kwargs)
```

1. See [:material-code-braces: BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef](./type_defs.md#batchgetmemberec2deepinspectionstatusrequestrequesttypedef) 

### batch\_update\_member\_ec2\_deep\_inspection\_status

Activates or deactivates Amazon Inspector deep inspection for the provided
member accounts in your organization.

Type annotations and code completion for `#!python session.create_client("inspector2").batch_update_member_ec2_deep_inspection_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.batch_update_member_ec2_deep_inspection_status)

```python
# batch_update_member_ec2_deep_inspection_status method definition

await def batch_update_member_ec2_deep_inspection_status(
    self,
    *,
    accountIds: Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],  # (1)
) -> BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: MemberAccountEc2DeepInspectionStatusTypeDef](./type_defs.md#memberaccountec2deepinspectionstatustypedef) 
2. See [:material-code-braces: BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef](./type_defs.md#batchupdatememberec2deepinspectionstatusresponsetypedef) 


```python
# batch_update_member_ec2_deep_inspection_status method usage example with argument unpacking

kwargs: BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.batch_update_member_ec2_deep_inspection_status(**kwargs)
```

1. See [:material-code-braces: BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef](./type_defs.md#batchupdatememberec2deepinspectionstatusrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("inspector2").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### cancel\_findings\_report

Cancels the given findings report.

Type annotations and code completion for `#!python session.create_client("inspector2").cancel_findings_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_findings_report)

```python
# cancel_findings_report method definition

await def cancel_findings_report(
    self,
    *,
    reportId: str,
) -> CancelFindingsReportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelFindingsReportResponseTypeDef](./type_defs.md#cancelfindingsreportresponsetypedef) 


```python
# cancel_findings_report method usage example with argument unpacking

kwargs: CancelFindingsReportRequestRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.cancel_findings_report(**kwargs)
```

1. See [:material-code-braces: CancelFindingsReportRequestRequestTypeDef](./type_defs.md#cancelfindingsreportrequestrequesttypedef) 

### cancel\_sbom\_export

Cancels a software bill of materials (SBOM) report.

Type annotations and code completion for `#!python session.create_client("inspector2").cancel_sbom_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.cancel_sbom_export)

```python
# cancel_sbom_export method definition

await def cancel_sbom_export(
    self,
    *,
    reportId: str,
) -> CancelSbomExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: CancelSbomExportResponseTypeDef](./type_defs.md#cancelsbomexportresponsetypedef) 


```python
# cancel_sbom_export method usage example with argument unpacking

kwargs: CancelSbomExportRequestRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.cancel_sbom_export(**kwargs)
```

1. See [:material-code-braces: CancelSbomExportRequestRequestTypeDef](./type_defs.md#cancelsbomexportrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("inspector2").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### create\_filter

Creates a filter resource using specified filter criteria.

Type annotations and code completion for `#!python session.create_client("inspector2").create_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_filter)

```python
# create_filter method definition

await def create_filter(
    self,
    *,
    action: FilterActionType,  # (1)
    filterCriteria: FilterCriteriaTypeDef,  # (2)
    name: str,
    description: str = ...,
    reason: str = ...,
    tags: Mapping[str, str] = ...,
) -> CreateFilterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
3. See [:material-code-braces: CreateFilterResponseTypeDef](./type_defs.md#createfilterresponsetypedef) 


```python
# create_filter method usage example with argument unpacking

kwargs: CreateFilterRequestRequestTypeDef = {  # (1)
    "action": ...,
    "filterCriteria": ...,
    "name": ...,
}

parent.create_filter(**kwargs)
```

1. See [:material-code-braces: CreateFilterRequestRequestTypeDef](./type_defs.md#createfilterrequestrequesttypedef) 

### create\_findings\_report

Creates a finding report.

Type annotations and code completion for `#!python session.create_client("inspector2").create_findings_report` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)

```python
# create_findings_report method definition

await def create_findings_report(
    self,
    *,
    reportFormat: ReportFormatType,  # (1)
    s3Destination: DestinationTypeDef,  # (2)
    filterCriteria: FilterCriteriaTypeDef = ...,  # (3)
) -> CreateFindingsReportResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: ReportFormatType](./literals.md#reportformattype) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
4. See [:material-code-braces: CreateFindingsReportResponseTypeDef](./type_defs.md#createfindingsreportresponsetypedef) 


```python
# create_findings_report method usage example with argument unpacking

kwargs: CreateFindingsReportRequestRequestTypeDef = {  # (1)
    "reportFormat": ...,
    "s3Destination": ...,
}

parent.create_findings_report(**kwargs)
```

1. See [:material-code-braces: CreateFindingsReportRequestRequestTypeDef](./type_defs.md#createfindingsreportrequestrequesttypedef) 

### create\_sbom\_export

Creates a software bill of materials (SBOM) report.

Type annotations and code completion for `#!python session.create_client("inspector2").create_sbom_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)

```python
# create_sbom_export method definition

await def create_sbom_export(
    self,
    *,
    reportFormat: SbomReportFormatType,  # (1)
    s3Destination: DestinationTypeDef,  # (2)
    resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...,  # (3)
) -> CreateSbomExportResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: SbomReportFormatType](./literals.md#sbomreportformattype) 
2. See [:material-code-braces: DestinationTypeDef](./type_defs.md#destinationtypedef) 
3. See [:material-code-braces: ResourceFilterCriteriaTypeDef](./type_defs.md#resourcefiltercriteriatypedef) 
4. See [:material-code-braces: CreateSbomExportResponseTypeDef](./type_defs.md#createsbomexportresponsetypedef) 


```python
# create_sbom_export method usage example with argument unpacking

kwargs: CreateSbomExportRequestRequestTypeDef = {  # (1)
    "reportFormat": ...,
    "s3Destination": ...,
}

parent.create_sbom_export(**kwargs)
```

1. See [:material-code-braces: CreateSbomExportRequestRequestTypeDef](./type_defs.md#createsbomexportrequestrequesttypedef) 

### delete\_filter

Deletes a filter resource.

Type annotations and code completion for `#!python session.create_client("inspector2").delete_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.delete_filter)

```python
# delete_filter method definition

await def delete_filter(
    self,
    *,
    arn: str,
) -> DeleteFilterResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DeleteFilterResponseTypeDef](./type_defs.md#deletefilterresponsetypedef) 


```python
# delete_filter method usage example with argument unpacking

kwargs: DeleteFilterRequestRequestTypeDef = {  # (1)
    "arn": ...,
}

parent.delete_filter(**kwargs)
```

1. See [:material-code-braces: DeleteFilterRequestRequestTypeDef](./type_defs.md#deletefilterrequestrequesttypedef) 

### describe\_organization\_configuration

Describe Amazon Inspector configuration settings for an Amazon Web Services
organization.

Type annotations and code completion for `#!python session.create_client("inspector2").describe_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.describe_organization_configuration)

```python
# describe_organization_configuration method definition

await def describe_organization_configuration(
    self,
) -> DescribeOrganizationConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeOrganizationConfigurationResponseTypeDef](./type_defs.md#describeorganizationconfigurationresponsetypedef) 

### disable

Disables Amazon Inspector scans for one or more Amazon Web Services accounts.

Type annotations and code completion for `#!python session.create_client("inspector2").disable` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable)

```python
# disable method definition

await def disable(
    self,
    *,
    accountIds: Sequence[str] = ...,
    resourceTypes: Sequence[ResourceScanTypeType] = ...,  # (1)
) -> DisableResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceScanTypeType](./literals.md#resourcescantypetype) 
2. See [:material-code-braces: DisableResponseTypeDef](./type_defs.md#disableresponsetypedef) 


```python
# disable method usage example with argument unpacking

kwargs: DisableRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.disable(**kwargs)
```

1. See [:material-code-braces: DisableRequestRequestTypeDef](./type_defs.md#disablerequestrequesttypedef) 

### disable\_delegated\_admin\_account

Disables the Amazon Inspector delegated administrator for your organization.

Type annotations and code completion for `#!python session.create_client("inspector2").disable_delegated_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disable_delegated_admin_account)

```python
# disable_delegated_admin_account method definition

await def disable_delegated_admin_account(
    self,
    *,
    delegatedAdminAccountId: str,
) -> DisableDelegatedAdminAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisableDelegatedAdminAccountResponseTypeDef](./type_defs.md#disabledelegatedadminaccountresponsetypedef) 


```python
# disable_delegated_admin_account method usage example with argument unpacking

kwargs: DisableDelegatedAdminAccountRequestRequestTypeDef = {  # (1)
    "delegatedAdminAccountId": ...,
}

parent.disable_delegated_admin_account(**kwargs)
```

1. See [:material-code-braces: DisableDelegatedAdminAccountRequestRequestTypeDef](./type_defs.md#disabledelegatedadminaccountrequestrequesttypedef) 

### disassociate\_member

Disassociates a member account from an Amazon Inspector delegated administrator.

Type annotations and code completion for `#!python session.create_client("inspector2").disassociate_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.disassociate_member)

```python
# disassociate_member method definition

await def disassociate_member(
    self,
    *,
    accountId: str,
) -> DisassociateMemberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DisassociateMemberResponseTypeDef](./type_defs.md#disassociatememberresponsetypedef) 


```python
# disassociate_member method usage example with argument unpacking

kwargs: DisassociateMemberRequestRequestTypeDef = {  # (1)
    "accountId": ...,
}

parent.disassociate_member(**kwargs)
```

1. See [:material-code-braces: DisassociateMemberRequestRequestTypeDef](./type_defs.md#disassociatememberrequestrequesttypedef) 

### enable

Enables Amazon Inspector scans for one or more Amazon Web Services accounts.

Type annotations and code completion for `#!python session.create_client("inspector2").enable` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable)

```python
# enable method definition

await def enable(
    self,
    *,
    resourceTypes: Sequence[ResourceScanTypeType],  # (1)
    accountIds: Sequence[str] = ...,
    clientToken: str = ...,
) -> EnableResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceScanTypeType](./literals.md#resourcescantypetype) 
2. See [:material-code-braces: EnableResponseTypeDef](./type_defs.md#enableresponsetypedef) 


```python
# enable method usage example with argument unpacking

kwargs: EnableRequestRequestTypeDef = {  # (1)
    "resourceTypes": ...,
}

parent.enable(**kwargs)
```

1. See [:material-code-braces: EnableRequestRequestTypeDef](./type_defs.md#enablerequestrequesttypedef) 

### enable\_delegated\_admin\_account

Enables the Amazon Inspector delegated administrator for your Organizations
organization.

Type annotations and code completion for `#!python session.create_client("inspector2").enable_delegated_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.enable_delegated_admin_account)

```python
# enable_delegated_admin_account method definition

await def enable_delegated_admin_account(
    self,
    *,
    delegatedAdminAccountId: str,
    clientToken: str = ...,
) -> EnableDelegatedAdminAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EnableDelegatedAdminAccountResponseTypeDef](./type_defs.md#enabledelegatedadminaccountresponsetypedef) 


```python
# enable_delegated_admin_account method usage example with argument unpacking

kwargs: EnableDelegatedAdminAccountRequestRequestTypeDef = {  # (1)
    "delegatedAdminAccountId": ...,
}

parent.enable_delegated_admin_account(**kwargs)
```

1. See [:material-code-braces: EnableDelegatedAdminAccountRequestRequestTypeDef](./type_defs.md#enabledelegatedadminaccountrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("inspector2").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.generate_presigned_url)

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


### get\_configuration

Retrieves setting configurations for Inspector scans.

Type annotations and code completion for `#!python session.create_client("inspector2").get_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_configuration)

```python
# get_configuration method definition

await def get_configuration(
    self,
) -> GetConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetConfigurationResponseTypeDef](./type_defs.md#getconfigurationresponsetypedef) 

### get\_delegated\_admin\_account

Retrieves information about the Amazon Inspector delegated administrator for
your organization.

Type annotations and code completion for `#!python session.create_client("inspector2").get_delegated_admin_account` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_delegated_admin_account)

```python
# get_delegated_admin_account method definition

await def get_delegated_admin_account(
    self,
) -> GetDelegatedAdminAccountResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetDelegatedAdminAccountResponseTypeDef](./type_defs.md#getdelegatedadminaccountresponsetypedef) 

### get\_ec2\_deep\_inspection\_configuration

Retrieves the activation status of Amazon Inspector deep inspection and custom
paths associated with your account.

Type annotations and code completion for `#!python session.create_client("inspector2").get_ec2_deep_inspection_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_ec2_deep_inspection_configuration)

```python
# get_ec2_deep_inspection_configuration method definition

await def get_ec2_deep_inspection_configuration(
    self,
) -> GetEc2DeepInspectionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEc2DeepInspectionConfigurationResponseTypeDef](./type_defs.md#getec2deepinspectionconfigurationresponsetypedef) 

### get\_encryption\_key

Gets an encryption key.

Type annotations and code completion for `#!python session.create_client("inspector2").get_encryption_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_encryption_key)

```python
# get_encryption_key method definition

await def get_encryption_key(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
) -> GetEncryptionKeyResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 
3. See [:material-code-braces: GetEncryptionKeyResponseTypeDef](./type_defs.md#getencryptionkeyresponsetypedef) 


```python
# get_encryption_key method usage example with argument unpacking

kwargs: GetEncryptionKeyRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
    "scanType": ...,
}

parent.get_encryption_key(**kwargs)
```

1. See [:material-code-braces: GetEncryptionKeyRequestRequestTypeDef](./type_defs.md#getencryptionkeyrequestrequesttypedef) 

### get\_findings\_report\_status

Gets the status of a findings report.

Type annotations and code completion for `#!python session.create_client("inspector2").get_findings_report_status` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_findings_report_status)

```python
# get_findings_report_status method definition

await def get_findings_report_status(
    self,
    *,
    reportId: str = ...,
) -> GetFindingsReportStatusResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetFindingsReportStatusResponseTypeDef](./type_defs.md#getfindingsreportstatusresponsetypedef) 


```python
# get_findings_report_status method usage example with argument unpacking

kwargs: GetFindingsReportStatusRequestRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.get_findings_report_status(**kwargs)
```

1. See [:material-code-braces: GetFindingsReportStatusRequestRequestTypeDef](./type_defs.md#getfindingsreportstatusrequestrequesttypedef) 

### get\_member

Gets member information for your organization.

Type annotations and code completion for `#!python session.create_client("inspector2").get_member` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_member)

```python
# get_member method definition

await def get_member(
    self,
    *,
    accountId: str,
) -> GetMemberResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetMemberResponseTypeDef](./type_defs.md#getmemberresponsetypedef) 


```python
# get_member method usage example with argument unpacking

kwargs: GetMemberRequestRequestTypeDef = {  # (1)
    "accountId": ...,
}

parent.get_member(**kwargs)
```

1. See [:material-code-braces: GetMemberRequestRequestTypeDef](./type_defs.md#getmemberrequestrequesttypedef) 

### get\_sbom\_export

Gets details of a software bill of materials (SBOM) report.

Type annotations and code completion for `#!python session.create_client("inspector2").get_sbom_export` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.get_sbom_export)

```python
# get_sbom_export method definition

await def get_sbom_export(
    self,
    *,
    reportId: str,
) -> GetSbomExportResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSbomExportResponseTypeDef](./type_defs.md#getsbomexportresponsetypedef) 


```python
# get_sbom_export method usage example with argument unpacking

kwargs: GetSbomExportRequestRequestTypeDef = {  # (1)
    "reportId": ...,
}

parent.get_sbom_export(**kwargs)
```

1. See [:material-code-braces: GetSbomExportRequestRequestTypeDef](./type_defs.md#getsbomexportrequestrequesttypedef) 

### list\_account\_permissions

Lists the permissions an account has to configure Amazon Inspector.

Type annotations and code completion for `#!python session.create_client("inspector2").list_account_permissions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_account_permissions)

```python
# list_account_permissions method definition

await def list_account_permissions(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    service: ServiceType = ...,  # (1)
) -> ListAccountPermissionsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ServiceType](./literals.md#servicetype) 
2. See [:material-code-braces: ListAccountPermissionsResponseTypeDef](./type_defs.md#listaccountpermissionsresponsetypedef) 


```python
# list_account_permissions method usage example with argument unpacking

kwargs: ListAccountPermissionsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_account_permissions(**kwargs)
```

1. See [:material-code-braces: ListAccountPermissionsRequestRequestTypeDef](./type_defs.md#listaccountpermissionsrequestrequesttypedef) 

### list\_coverage

Lists coverage details for you environment.

Type annotations and code completion for `#!python session.create_client("inspector2").list_coverage` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage)

```python
# list_coverage method definition

await def list_coverage(
    self,
    *,
    filterCriteria: CoverageFilterCriteriaTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListCoverageResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-braces: ListCoverageResponseTypeDef](./type_defs.md#listcoverageresponsetypedef) 


```python
# list_coverage method usage example with argument unpacking

kwargs: ListCoverageRequestRequestTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.list_coverage(**kwargs)
```

1. See [:material-code-braces: ListCoverageRequestRequestTypeDef](./type_defs.md#listcoveragerequestrequesttypedef) 

### list\_coverage\_statistics

Lists Amazon Inspector coverage statistics for your environment.

Type annotations and code completion for `#!python session.create_client("inspector2").list_coverage_statistics` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_coverage_statistics)

```python
# list_coverage_statistics method definition

await def list_coverage_statistics(
    self,
    *,
    filterCriteria: CoverageFilterCriteriaTypeDef = ...,  # (1)
    groupBy: GroupKeyType = ...,  # (2)
    nextToken: str = ...,
) -> ListCoverageStatisticsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: CoverageFilterCriteriaTypeDef](./type_defs.md#coveragefiltercriteriatypedef) 
2. See [:material-code-brackets: GroupKeyType](./literals.md#groupkeytype) 
3. See [:material-code-braces: ListCoverageStatisticsResponseTypeDef](./type_defs.md#listcoveragestatisticsresponsetypedef) 


```python
# list_coverage_statistics method usage example with argument unpacking

kwargs: ListCoverageStatisticsRequestRequestTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.list_coverage_statistics(**kwargs)
```

1. See [:material-code-braces: ListCoverageStatisticsRequestRequestTypeDef](./type_defs.md#listcoveragestatisticsrequestrequesttypedef) 

### list\_delegated\_admin\_accounts

Lists information about the Amazon Inspector delegated administrator of your
organization.

Type annotations and code completion for `#!python session.create_client("inspector2").list_delegated_admin_accounts` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_delegated_admin_accounts)

```python
# list_delegated_admin_accounts method definition

await def list_delegated_admin_accounts(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListDelegatedAdminAccountsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDelegatedAdminAccountsResponseTypeDef](./type_defs.md#listdelegatedadminaccountsresponsetypedef) 


```python
# list_delegated_admin_accounts method usage example with argument unpacking

kwargs: ListDelegatedAdminAccountsRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_delegated_admin_accounts(**kwargs)
```

1. See [:material-code-braces: ListDelegatedAdminAccountsRequestRequestTypeDef](./type_defs.md#listdelegatedadminaccountsrequestrequesttypedef) 

### list\_filters

Lists the filters associated with your account.

Type annotations and code completion for `#!python session.create_client("inspector2").list_filters` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_filters)

```python
# list_filters method definition

await def list_filters(
    self,
    *,
    action: FilterActionType = ...,  # (1)
    arns: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFiltersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: ListFiltersResponseTypeDef](./type_defs.md#listfiltersresponsetypedef) 


```python
# list_filters method usage example with argument unpacking

kwargs: ListFiltersRequestRequestTypeDef = {  # (1)
    "action": ...,
}

parent.list_filters(**kwargs)
```

1. See [:material-code-braces: ListFiltersRequestRequestTypeDef](./type_defs.md#listfiltersrequestrequesttypedef) 

### list\_finding\_aggregations

Lists aggregated finding data for your environment based on specific criteria.

Type annotations and code completion for `#!python session.create_client("inspector2").list_finding_aggregations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)

```python
# list_finding_aggregations method definition

await def list_finding_aggregations(
    self,
    *,
    aggregationType: AggregationTypeType,  # (1)
    accountIds: Sequence[StringFilterTypeDef] = ...,  # (2)
    aggregationRequest: AggregationRequestTypeDef = ...,  # (3)
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListFindingAggregationsResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-brackets: AggregationTypeType](./literals.md#aggregationtypetype) 
2. See [:material-code-braces: StringFilterTypeDef](./type_defs.md#stringfiltertypedef) 
3. See [:material-code-braces: AggregationRequestTypeDef](./type_defs.md#aggregationrequesttypedef) 
4. See [:material-code-braces: ListFindingAggregationsResponseTypeDef](./type_defs.md#listfindingaggregationsresponsetypedef) 


```python
# list_finding_aggregations method usage example with argument unpacking

kwargs: ListFindingAggregationsRequestRequestTypeDef = {  # (1)
    "aggregationType": ...,
}

parent.list_finding_aggregations(**kwargs)
```

1. See [:material-code-braces: ListFindingAggregationsRequestRequestTypeDef](./type_defs.md#listfindingaggregationsrequestrequesttypedef) 

### list\_findings

Lists findings for your environment.

Type annotations and code completion for `#!python session.create_client("inspector2").list_findings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_findings)

```python
# list_findings method definition

await def list_findings(
    self,
    *,
    filterCriteria: FilterCriteriaTypeDef = ...,  # (1)
    maxResults: int = ...,
    nextToken: str = ...,
    sortCriteria: SortCriteriaTypeDef = ...,  # (2)
) -> ListFindingsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
2. See [:material-code-braces: SortCriteriaTypeDef](./type_defs.md#sortcriteriatypedef) 
3. See [:material-code-braces: ListFindingsResponseTypeDef](./type_defs.md#listfindingsresponsetypedef) 


```python
# list_findings method usage example with argument unpacking

kwargs: ListFindingsRequestRequestTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.list_findings(**kwargs)
```

1. See [:material-code-braces: ListFindingsRequestRequestTypeDef](./type_defs.md#listfindingsrequestrequesttypedef) 

### list\_members

List members associated with the Amazon Inspector delegated administrator for
your organization.

Type annotations and code completion for `#!python session.create_client("inspector2").list_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_members)

```python
# list_members method definition

await def list_members(
    self,
    *,
    maxResults: int = ...,
    nextToken: str = ...,
    onlyAssociated: bool = ...,
) -> ListMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListMembersResponseTypeDef](./type_defs.md#listmembersresponsetypedef) 


```python
# list_members method usage example with argument unpacking

kwargs: ListMembersRequestRequestTypeDef = {  # (1)
    "maxResults": ...,
}

parent.list_members(**kwargs)
```

1. See [:material-code-braces: ListMembersRequestRequestTypeDef](./type_defs.md#listmembersrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags attached to a given resource.

Type annotations and code completion for `#!python session.create_client("inspector2").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    resourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_usage\_totals

Lists the Amazon Inspector usage totals over the last 30 days.

Type annotations and code completion for `#!python session.create_client("inspector2").list_usage_totals` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_usage_totals)

```python
# list_usage_totals method definition

await def list_usage_totals(
    self,
    *,
    accountIds: Sequence[str] = ...,
    maxResults: int = ...,
    nextToken: str = ...,
) -> ListUsageTotalsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListUsageTotalsResponseTypeDef](./type_defs.md#listusagetotalsresponsetypedef) 


```python
# list_usage_totals method usage example with argument unpacking

kwargs: ListUsageTotalsRequestRequestTypeDef = {  # (1)
    "accountIds": ...,
}

parent.list_usage_totals(**kwargs)
```

1. See [:material-code-braces: ListUsageTotalsRequestRequestTypeDef](./type_defs.md#listusagetotalsrequestrequesttypedef) 

### reset\_encryption\_key

Resets an encryption key.

Type annotations and code completion for `#!python session.create_client("inspector2").reset_encryption_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.reset_encryption_key)

```python
# reset_encryption_key method definition

await def reset_encryption_key(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 


```python
# reset_encryption_key method usage example with argument unpacking

kwargs: ResetEncryptionKeyRequestRequestTypeDef = {  # (1)
    "resourceType": ...,
    "scanType": ...,
}

parent.reset_encryption_key(**kwargs)
```

1. See [:material-code-braces: ResetEncryptionKeyRequestRequestTypeDef](./type_defs.md#resetencryptionkeyrequestrequesttypedef) 

### search\_vulnerabilities

Lists Amazon Inspector coverage details for a specific vulnerability.

Type annotations and code completion for `#!python session.create_client("inspector2").search_vulnerabilities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.search_vulnerabilities)

```python
# search_vulnerabilities method definition

await def search_vulnerabilities(
    self,
    *,
    filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,  # (1)
    nextToken: str = ...,
) -> SearchVulnerabilitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SearchVulnerabilitiesFilterCriteriaTypeDef](./type_defs.md#searchvulnerabilitiesfiltercriteriatypedef) 
2. See [:material-code-braces: SearchVulnerabilitiesResponseTypeDef](./type_defs.md#searchvulnerabilitiesresponsetypedef) 


```python
# search_vulnerabilities method usage example with argument unpacking

kwargs: SearchVulnerabilitiesRequestRequestTypeDef = {  # (1)
    "filterCriteria": ...,
}

parent.search_vulnerabilities(**kwargs)
```

1. See [:material-code-braces: SearchVulnerabilitiesRequestRequestTypeDef](./type_defs.md#searchvulnerabilitiesrequestrequesttypedef) 

### tag\_resource

Adds tags to a resource.

Type annotations and code completion for `#!python session.create_client("inspector2").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    resourceArn: str,
    tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes tags from a resource.

Type annotations and code completion for `#!python session.create_client("inspector2").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    resourceArn: str,
    tagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "resourceArn": ...,
    "tagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_configuration

Updates setting configurations for your Amazon Inspector account.

Type annotations and code completion for `#!python session.create_client("inspector2").update_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_configuration)

```python
# update_configuration method definition

await def update_configuration(
    self,
    *,
    ecrConfiguration: EcrConfigurationTypeDef,  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: EcrConfigurationTypeDef](./type_defs.md#ecrconfigurationtypedef) 


```python
# update_configuration method usage example with argument unpacking

kwargs: UpdateConfigurationRequestRequestTypeDef = {  # (1)
    "ecrConfiguration": ...,
}

parent.update_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateConfigurationRequestRequestTypeDef](./type_defs.md#updateconfigurationrequestrequesttypedef) 

### update\_ec2\_deep\_inspection\_configuration

Activates, deactivates Amazon Inspector deep inspection, or updates custom paths
for your account.

Type annotations and code completion for `#!python session.create_client("inspector2").update_ec2_deep_inspection_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_ec2_deep_inspection_configuration)

```python
# update_ec2_deep_inspection_configuration method definition

await def update_ec2_deep_inspection_configuration(
    self,
    *,
    activateDeepInspection: bool = ...,
    packagePaths: Sequence[str] = ...,
) -> UpdateEc2DeepInspectionConfigurationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEc2DeepInspectionConfigurationResponseTypeDef](./type_defs.md#updateec2deepinspectionconfigurationresponsetypedef) 


```python
# update_ec2_deep_inspection_configuration method usage example with argument unpacking

kwargs: UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef = {  # (1)
    "activateDeepInspection": ...,
}

parent.update_ec2_deep_inspection_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef](./type_defs.md#updateec2deepinspectionconfigurationrequestrequesttypedef) 

### update\_encryption\_key

Updates an encryption key.

Type annotations and code completion for `#!python session.create_client("inspector2").update_encryption_key` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_encryption_key)

```python
# update_encryption_key method definition

await def update_encryption_key(
    self,
    *,
    kmsKeyId: str,
    resourceType: ResourceTypeType,  # (1)
    scanType: ScanTypeType,  # (2)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ScanTypeType](./literals.md#scantypetype) 


```python
# update_encryption_key method usage example with argument unpacking

kwargs: UpdateEncryptionKeyRequestRequestTypeDef = {  # (1)
    "kmsKeyId": ...,
    "resourceType": ...,
    "scanType": ...,
}

parent.update_encryption_key(**kwargs)
```

1. See [:material-code-braces: UpdateEncryptionKeyRequestRequestTypeDef](./type_defs.md#updateencryptionkeyrequestrequesttypedef) 

### update\_filter

Specifies the action that is to be applied to the findings that match the
filter.

Type annotations and code completion for `#!python session.create_client("inspector2").update_filter` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_filter)

```python
# update_filter method definition

await def update_filter(
    self,
    *,
    filterArn: str,
    action: FilterActionType = ...,  # (1)
    description: str = ...,
    filterCriteria: FilterCriteriaTypeDef = ...,  # (2)
    name: str = ...,
    reason: str = ...,
) -> UpdateFilterResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: FilterActionType](./literals.md#filteractiontype) 
2. See [:material-code-braces: FilterCriteriaTypeDef](./type_defs.md#filtercriteriatypedef) 
3. See [:material-code-braces: UpdateFilterResponseTypeDef](./type_defs.md#updatefilterresponsetypedef) 


```python
# update_filter method usage example with argument unpacking

kwargs: UpdateFilterRequestRequestTypeDef = {  # (1)
    "filterArn": ...,
}

parent.update_filter(**kwargs)
```

1. See [:material-code-braces: UpdateFilterRequestRequestTypeDef](./type_defs.md#updatefilterrequestrequesttypedef) 

### update\_org\_ec2\_deep\_inspection\_configuration

Updates the Amazon Inspector deep inspection custom paths for your organization.

Type annotations and code completion for `#!python session.create_client("inspector2").update_org_ec2_deep_inspection_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_org_ec2_deep_inspection_configuration)

```python
# update_org_ec2_deep_inspection_configuration method definition

await def update_org_ec2_deep_inspection_configuration(
    self,
    *,
    orgPackagePaths: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# update_org_ec2_deep_inspection_configuration method usage example with argument unpacking

kwargs: UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef = {  # (1)
    "orgPackagePaths": ...,
}

parent.update_org_ec2_deep_inspection_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef](./type_defs.md#updateorgec2deepinspectionconfigurationrequestrequesttypedef) 

### update\_organization\_configuration

Updates the configurations for your Amazon Inspector organization.

Type annotations and code completion for `#!python session.create_client("inspector2").update_organization_configuration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.update_organization_configuration)

```python
# update_organization_configuration method definition

await def update_organization_configuration(
    self,
    *,
    autoEnable: AutoEnableTypeDef,  # (1)
) -> UpdateOrganizationConfigurationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AutoEnableTypeDef](./type_defs.md#autoenabletypedef) 
2. See [:material-code-braces: UpdateOrganizationConfigurationResponseTypeDef](./type_defs.md#updateorganizationconfigurationresponsetypedef) 


```python
# update_organization_configuration method usage example with argument unpacking

kwargs: UpdateOrganizationConfigurationRequestRequestTypeDef = {  # (1)
    "autoEnable": ...,
}

parent.update_organization_configuration(**kwargs)
```

1. See [:material-code-braces: UpdateOrganizationConfigurationRequestRequestTypeDef](./type_defs.md#updateorganizationconfigurationrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("inspector2").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Inspector2Client:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("inspector2").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("inspector2").get_paginator` method with overloads.

- `client.get_paginator("list_account_permissions")` -> [ListAccountPermissionsPaginator](./paginators.md#listaccountpermissionspaginator)
- `client.get_paginator("list_coverage")` -> [ListCoveragePaginator](./paginators.md#listcoveragepaginator)
- `client.get_paginator("list_coverage_statistics")` -> [ListCoverageStatisticsPaginator](./paginators.md#listcoveragestatisticspaginator)
- `client.get_paginator("list_delegated_admin_accounts")` -> [ListDelegatedAdminAccountsPaginator](./paginators.md#listdelegatedadminaccountspaginator)
- `client.get_paginator("list_filters")` -> [ListFiltersPaginator](./paginators.md#listfilterspaginator)
- `client.get_paginator("list_finding_aggregations")` -> [ListFindingAggregationsPaginator](./paginators.md#listfindingaggregationspaginator)
- `client.get_paginator("list_findings")` -> [ListFindingsPaginator](./paginators.md#listfindingspaginator)
- `client.get_paginator("list_members")` -> [ListMembersPaginator](./paginators.md#listmemberspaginator)
- `client.get_paginator("list_usage_totals")` -> [ListUsageTotalsPaginator](./paginators.md#listusagetotalspaginator)
- `client.get_paginator("search_vulnerabilities")` -> [SearchVulnerabilitiesPaginator](./paginators.md#searchvulnerabilitiespaginator)




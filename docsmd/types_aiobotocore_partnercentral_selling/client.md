# PartnerCentralSellingAPIClient

> [Index](../README.md) > [PartnerCentralSellingAPI](./README.md) > PartnerCentralSellingAPIClient

!!! note ""

    Auto-generated documentation for [PartnerCentralSellingAPI](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#partnercentralsellingapi)
    type annotations stubs module [types-aiobotocore-partnercentral-selling](https://pypi.org/project/types-aiobotocore-partnercentral-selling/).

## PartnerCentralSellingAPIClient

Type annotations and code completion for `#!python session.create_client("partnercentral-selling")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# PartnerCentralSellingAPIClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_partnercentral_selling.client import PartnerCentralSellingAPIClient

session = get_session()
async with session.create_client("partnercentral-selling") as client:
    client: PartnerCentralSellingAPIClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("partnercentral-selling").exceptions` structure.

```python
# PartnerCentralSellingAPIClient.exceptions usage example

async with session.create_client("partnercentral-selling") as client:
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
# PartnerCentralSellingAPIClient usage type checking example

from types_aiobotocore_partnercentral_selling.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("partnercentral-selling").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("partnercentral-selling").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/generate_presigned_url.html)

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


### accept\_engagement\_invitation

Use the <code>AcceptEngagementInvitation</code> action to accept an engagement
invitation shared by AWS.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").accept_engagement_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/accept_engagement_invitation.html)

```python
# accept_engagement_invitation method definition

await def accept_engagement_invitation(
    self,
    *,
    Catalog: str,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# accept_engagement_invitation method usage example with argument unpacking

kwargs: AcceptEngagementInvitationRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.accept_engagement_invitation(**kwargs)
```

1. See [:material-code-braces: AcceptEngagementInvitationRequestTypeDef](./type_defs.md#acceptengagementinvitationrequesttypedef) 

### assign\_opportunity

Enables you to reassign an existing <code>Opportunity</code> to another user
within your Partner Central account.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").assign_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/assign_opportunity.html)

```python
# assign_opportunity method definition

await def assign_opportunity(
    self,
    *,
    Assignee: AssigneeContactTypeDef,  # (1)
    Catalog: str,
    Identifier: str,
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: AssigneeContactTypeDef](./type_defs.md#assigneecontacttypedef) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# assign_opportunity method usage example with argument unpacking

kwargs: AssignOpportunityRequestTypeDef = {  # (1)
    "Assignee": ...,
    "Catalog": ...,
    "Identifier": ...,
}

parent.assign_opportunity(**kwargs)
```

1. See [:material-code-braces: AssignOpportunityRequestTypeDef](./type_defs.md#assignopportunityrequesttypedef) 

### associate\_opportunity

Enables you to create a formal association between an <code>Opportunity</code>
and various related entities, enriching the context and details of the
opportunity for better collaboration and decision making.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").associate_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/associate_opportunity.html)

```python
# associate_opportunity method definition

await def associate_opportunity(
    self,
    *,
    Catalog: str,
    OpportunityIdentifier: str,
    RelatedEntityIdentifier: str,
    RelatedEntityType: RelatedEntityTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RelatedEntityTypeType](./literals.md#relatedentitytypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# associate_opportunity method usage example with argument unpacking

kwargs: AssociateOpportunityRequestTypeDef = {  # (1)
    "Catalog": ...,
    "OpportunityIdentifier": ...,
    "RelatedEntityIdentifier": ...,
    "RelatedEntityType": ...,
}

parent.associate_opportunity(**kwargs)
```

1. See [:material-code-braces: AssociateOpportunityRequestTypeDef](./type_defs.md#associateopportunityrequesttypedef) 

### create\_engagement

The <code>CreateEngagement</code> action allows you to create an
<code>Engagement</code>, which serves as a collaborative space between
different parties such as AWS Partners and AWS Sellers.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").create_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/create_engagement.html)

```python
# create_engagement method definition

await def create_engagement(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    Description: str,
    Title: str,
    Contexts: Sequence[EngagementContextDetailsTypeDef] = ...,  # (1)
) -> CreateEngagementResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EngagementContextDetailsTypeDef](./type_defs.md#engagementcontextdetailstypedef) 
2. See [:material-code-braces: CreateEngagementResponseTypeDef](./type_defs.md#createengagementresponsetypedef) 


```python
# create_engagement method usage example with argument unpacking

kwargs: CreateEngagementRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "Description": ...,
    "Title": ...,
}

parent.create_engagement(**kwargs)
```

1. See [:material-code-braces: CreateEngagementRequestTypeDef](./type_defs.md#createengagementrequesttypedef) 

### create\_engagement\_invitation

This action creates an invitation from a sender to a single receiver to join an
engagement.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").create_engagement_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/create_engagement_invitation.html)

```python
# create_engagement_invitation method definition

await def create_engagement_invitation(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    Invitation: InvitationTypeDef,  # (1)
) -> CreateEngagementInvitationResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: InvitationTypeDef](./type_defs.md#invitationtypedef) 
2. See [:material-code-braces: CreateEngagementInvitationResponseTypeDef](./type_defs.md#createengagementinvitationresponsetypedef) 


```python
# create_engagement_invitation method usage example with argument unpacking

kwargs: CreateEngagementInvitationRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "EngagementIdentifier": ...,
    "Invitation": ...,
}

parent.create_engagement_invitation(**kwargs)
```

1. See [:material-code-braces: CreateEngagementInvitationRequestTypeDef](./type_defs.md#createengagementinvitationrequesttypedef) 

### create\_opportunity

Creates an <code>Opportunity</code> record in Partner Central.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").create_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/create_opportunity.html)

```python
# create_opportunity method definition

await def create_opportunity(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    Customer: CustomerUnionTypeDef = ...,  # (1)
    LifeCycle: LifeCycleUnionTypeDef = ...,  # (2)
    Marketing: MarketingUnionTypeDef = ...,  # (3)
    NationalSecurity: NationalSecurityType = ...,  # (4)
    OpportunityTeam: Sequence[ContactTypeDef] = ...,  # (5)
    OpportunityType: OpportunityTypeType = ...,  # (6)
    Origin: OpportunityOriginType = ...,  # (7)
    PartnerOpportunityIdentifier: str = ...,
    PrimaryNeedsFromAws: Sequence[PrimaryNeedFromAwsType] = ...,  # (8)
    Project: ProjectUnionTypeDef = ...,  # (9)
    SoftwareRevenue: SoftwareRevenueTypeDef = ...,  # (10)
) -> CreateOpportunityResponseTypeDef:  # (11)
    ...
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) [:material-code-braces: CustomerOutputTypeDef](./type_defs.md#customeroutputtypedef) 
2. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) [:material-code-braces: LifeCycleOutputTypeDef](./type_defs.md#lifecycleoutputtypedef) 
3. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) [:material-code-braces: MarketingOutputTypeDef](./type_defs.md#marketingoutputtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-braces: ContactTypeDef](./type_defs.md#contacttypedef) 
6. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
7. See [:material-code-brackets: OpportunityOriginType](./literals.md#opportunityorigintype) 
8. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
9. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) [:material-code-braces: ProjectOutputTypeDef](./type_defs.md#projectoutputtypedef) 
10. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
11. See [:material-code-braces: CreateOpportunityResponseTypeDef](./type_defs.md#createopportunityresponsetypedef) 


```python
# create_opportunity method usage example with argument unpacking

kwargs: CreateOpportunityRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
}

parent.create_opportunity(**kwargs)
```

1. See [:material-code-braces: CreateOpportunityRequestTypeDef](./type_defs.md#createopportunityrequesttypedef) 

### create\_resource\_snapshot

This action allows you to create an immutable snapshot of a specific resource,
such as an opportunity, within the context of an engagement.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").create_resource_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/create_resource_snapshot.html)

```python
# create_resource_snapshot method definition

await def create_resource_snapshot(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
) -> CreateResourceSnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: CreateResourceSnapshotResponseTypeDef](./type_defs.md#createresourcesnapshotresponsetypedef) 


```python
# create_resource_snapshot method usage example with argument unpacking

kwargs: CreateResourceSnapshotRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "EngagementIdentifier": ...,
    "ResourceIdentifier": ...,
    "ResourceSnapshotTemplateIdentifier": ...,
    "ResourceType": ...,
}

parent.create_resource_snapshot(**kwargs)
```

1. See [:material-code-braces: CreateResourceSnapshotRequestTypeDef](./type_defs.md#createresourcesnapshotrequesttypedef) 

### create\_resource\_snapshot\_job

Use this action to create a job to generate a snapshot of the specified
resource within an engagement.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").create_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/create_resource_snapshot_job.html)

```python
# create_resource_snapshot_job method definition

await def create_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> CreateResourceSnapshotJobResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: CreateResourceSnapshotJobResponseTypeDef](./type_defs.md#createresourcesnapshotjobresponsetypedef) 


```python
# create_resource_snapshot_job method usage example with argument unpacking

kwargs: CreateResourceSnapshotJobRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "EngagementIdentifier": ...,
    "ResourceIdentifier": ...,
    "ResourceSnapshotTemplateIdentifier": ...,
    "ResourceType": ...,
}

parent.create_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: CreateResourceSnapshotJobRequestTypeDef](./type_defs.md#createresourcesnapshotjobrequesttypedef) 

### delete\_resource\_snapshot\_job

Use this action to deletes a previously created resource snapshot job.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").delete_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/delete_resource_snapshot_job.html)

```python
# delete_resource_snapshot_job method definition

await def delete_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# delete_resource_snapshot_job method usage example with argument unpacking

kwargs: DeleteResourceSnapshotJobRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ResourceSnapshotJobIdentifier": ...,
}

parent.delete_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: DeleteResourceSnapshotJobRequestTypeDef](./type_defs.md#deleteresourcesnapshotjobrequesttypedef) 

### disassociate\_opportunity

Allows you to remove an existing association between an
<code>Opportunity</code> and related entities, such as a Partner Solution,
Amazon Web Services product, or an Amazon Web Services Marketplace offer.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").disassociate_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/disassociate_opportunity.html)

```python
# disassociate_opportunity method definition

await def disassociate_opportunity(
    self,
    *,
    Catalog: str,
    OpportunityIdentifier: str,
    RelatedEntityIdentifier: str,
    RelatedEntityType: RelatedEntityTypeType,  # (1)
) -> EmptyResponseMetadataTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: RelatedEntityTypeType](./literals.md#relatedentitytypetype) 
2. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# disassociate_opportunity method usage example with argument unpacking

kwargs: DisassociateOpportunityRequestTypeDef = {  # (1)
    "Catalog": ...,
    "OpportunityIdentifier": ...,
    "RelatedEntityIdentifier": ...,
    "RelatedEntityType": ...,
}

parent.disassociate_opportunity(**kwargs)
```

1. See [:material-code-braces: DisassociateOpportunityRequestTypeDef](./type_defs.md#disassociateopportunityrequesttypedef) 

### get\_aws\_opportunity\_summary

Retrieves a summary of an AWS Opportunity.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_aws_opportunity_summary` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/get_aws_opportunity_summary.html)

```python
# get_aws_opportunity_summary method definition

await def get_aws_opportunity_summary(
    self,
    *,
    Catalog: str,
    RelatedOpportunityIdentifier: str,
) -> GetAwsOpportunitySummaryResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetAwsOpportunitySummaryResponseTypeDef](./type_defs.md#getawsopportunitysummaryresponsetypedef) 


```python
# get_aws_opportunity_summary method usage example with argument unpacking

kwargs: GetAwsOpportunitySummaryRequestTypeDef = {  # (1)
    "Catalog": ...,
    "RelatedOpportunityIdentifier": ...,
}

parent.get_aws_opportunity_summary(**kwargs)
```

1. See [:material-code-braces: GetAwsOpportunitySummaryRequestTypeDef](./type_defs.md#getawsopportunitysummaryrequesttypedef) 

### get\_engagement

Use this action to retrieve the engagement record for a given
<code>EngagementIdentifier</code>.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_engagement` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/get_engagement.html)

```python
# get_engagement method definition

await def get_engagement(
    self,
    *,
    Catalog: str,
    Identifier: str,
) -> GetEngagementResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEngagementResponseTypeDef](./type_defs.md#getengagementresponsetypedef) 


```python
# get_engagement method usage example with argument unpacking

kwargs: GetEngagementRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.get_engagement(**kwargs)
```

1. See [:material-code-braces: GetEngagementRequestTypeDef](./type_defs.md#getengagementrequesttypedef) 

### get\_engagement\_invitation

Retrieves the details of an engagement invitation shared by AWS with a partner.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_engagement_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/get_engagement_invitation.html)

```python
# get_engagement_invitation method definition

await def get_engagement_invitation(
    self,
    *,
    Catalog: str,
    Identifier: str,
) -> GetEngagementInvitationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEngagementInvitationResponseTypeDef](./type_defs.md#getengagementinvitationresponsetypedef) 


```python
# get_engagement_invitation method usage example with argument unpacking

kwargs: GetEngagementInvitationRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.get_engagement_invitation(**kwargs)
```

1. See [:material-code-braces: GetEngagementInvitationRequestTypeDef](./type_defs.md#getengagementinvitationrequesttypedef) 

### get\_opportunity

Fetches the <code>Opportunity</code> record from Partner Central by a given
<code>Identifier</code>.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/get_opportunity.html)

```python
# get_opportunity method definition

await def get_opportunity(
    self,
    *,
    Catalog: str,
    Identifier: str,
) -> GetOpportunityResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetOpportunityResponseTypeDef](./type_defs.md#getopportunityresponsetypedef) 


```python
# get_opportunity method usage example with argument unpacking

kwargs: GetOpportunityRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.get_opportunity(**kwargs)
```

1. See [:material-code-braces: GetOpportunityRequestTypeDef](./type_defs.md#getopportunityrequesttypedef) 

### get\_resource\_snapshot

Use this action to retrieve a specific snapshot record.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_resource_snapshot` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/get_resource_snapshot.html)

```python
# get_resource_snapshot method definition

await def get_resource_snapshot(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: str,
    ResourceIdentifier: str,
    ResourceSnapshotTemplateIdentifier: str,
    ResourceType: ResourceTypeType,  # (1)
    Revision: int = ...,
) -> GetResourceSnapshotResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: GetResourceSnapshotResponseTypeDef](./type_defs.md#getresourcesnapshotresponsetypedef) 


```python
# get_resource_snapshot method usage example with argument unpacking

kwargs: GetResourceSnapshotRequestTypeDef = {  # (1)
    "Catalog": ...,
    "EngagementIdentifier": ...,
    "ResourceIdentifier": ...,
    "ResourceSnapshotTemplateIdentifier": ...,
    "ResourceType": ...,
}

parent.get_resource_snapshot(**kwargs)
```

1. See [:material-code-braces: GetResourceSnapshotRequestTypeDef](./type_defs.md#getresourcesnapshotrequesttypedef) 

### get\_resource\_snapshot\_job

Use this action to retrieves information about a specific resource snapshot job.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/get_resource_snapshot_job.html)

```python
# get_resource_snapshot_job method definition

await def get_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
) -> GetResourceSnapshotJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetResourceSnapshotJobResponseTypeDef](./type_defs.md#getresourcesnapshotjobresponsetypedef) 


```python
# get_resource_snapshot_job method usage example with argument unpacking

kwargs: GetResourceSnapshotJobRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ResourceSnapshotJobIdentifier": ...,
}

parent.get_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: GetResourceSnapshotJobRequestTypeDef](./type_defs.md#getresourcesnapshotjobrequesttypedef) 

### get\_selling\_system\_settings

Retrieves the currently set system settings, which include the IAM Role used
for resource snapshot jobs.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_selling_system_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/get_selling_system_settings.html)

```python
# get_selling_system_settings method definition

await def get_selling_system_settings(
    self,
    *,
    Catalog: str,
) -> GetSellingSystemSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetSellingSystemSettingsResponseTypeDef](./type_defs.md#getsellingsystemsettingsresponsetypedef) 


```python
# get_selling_system_settings method usage example with argument unpacking

kwargs: GetSellingSystemSettingsRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.get_selling_system_settings(**kwargs)
```

1. See [:material-code-braces: GetSellingSystemSettingsRequestTypeDef](./type_defs.md#getsellingsystemsettingsrequesttypedef) 

### list\_engagement\_by\_accepting\_invitation\_tasks

Lists all in-progress, completed, or failed
StartEngagementByAcceptingInvitationTask tasks that were initiated by the
caller's account.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_engagement_by_accepting_invitation_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_engagement_by_accepting_invitation_tasks.html)

```python
# list_engagement_by_accepting_invitation_tasks method definition

await def list_engagement_by_accepting_invitation_tasks(
    self,
    *,
    Catalog: str,
    EngagementInvitationIdentifier: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    OpportunityIdentifier: Sequence[str] = ...,
    Sort: ListTasksSortBaseTypeDef = ...,  # (1)
    TaskIdentifier: Sequence[str] = ...,
    TaskStatus: Sequence[TaskStatusType] = ...,  # (2)
) -> ListEngagementByAcceptingInvitationTasksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: ListEngagementByAcceptingInvitationTasksResponseTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksresponsetypedef) 


```python
# list_engagement_by_accepting_invitation_tasks method usage example with argument unpacking

kwargs: ListEngagementByAcceptingInvitationTasksRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_engagement_by_accepting_invitation_tasks(**kwargs)
```

1. See [:material-code-braces: ListEngagementByAcceptingInvitationTasksRequestTypeDef](./type_defs.md#listengagementbyacceptinginvitationtasksrequesttypedef) 

### list\_engagement\_from\_opportunity\_tasks

Lists all in-progress, completed, or failed
<code>EngagementFromOpportunity</code> tasks that were initiated by the
caller's account.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_engagement_from_opportunity_tasks` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_engagement_from_opportunity_tasks.html)

```python
# list_engagement_from_opportunity_tasks method definition

await def list_engagement_from_opportunity_tasks(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    OpportunityIdentifier: Sequence[str] = ...,
    Sort: ListTasksSortBaseTypeDef = ...,  # (1)
    TaskIdentifier: Sequence[str] = ...,
    TaskStatus: Sequence[TaskStatusType] = ...,  # (2)
) -> ListEngagementFromOpportunityTasksResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: ListTasksSortBaseTypeDef](./type_defs.md#listtaskssortbasetypedef) 
2. See [:material-code-brackets: TaskStatusType](./literals.md#taskstatustype) 
3. See [:material-code-braces: ListEngagementFromOpportunityTasksResponseTypeDef](./type_defs.md#listengagementfromopportunitytasksresponsetypedef) 


```python
# list_engagement_from_opportunity_tasks method usage example with argument unpacking

kwargs: ListEngagementFromOpportunityTasksRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_engagement_from_opportunity_tasks(**kwargs)
```

1. See [:material-code-braces: ListEngagementFromOpportunityTasksRequestTypeDef](./type_defs.md#listengagementfromopportunitytasksrequesttypedef) 

### list\_engagement\_invitations

Retrieves a list of engagement invitations sent to the partner.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_engagement_invitations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_engagement_invitations.html)

```python
# list_engagement_invitations method definition

await def list_engagement_invitations(
    self,
    *,
    Catalog: str,
    ParticipantType: ParticipantTypeType,  # (1)
    EngagementIdentifier: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    PayloadType: Sequence[EngagementInvitationPayloadTypeType] = ...,  # (2)
    SenderAwsAccountId: Sequence[str] = ...,
    Sort: OpportunityEngagementInvitationSortTypeDef = ...,  # (3)
    Status: Sequence[InvitationStatusType] = ...,  # (4)
) -> ListEngagementInvitationsResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-brackets: ParticipantTypeType](./literals.md#participanttypetype) 
2. See [:material-code-brackets: EngagementInvitationPayloadTypeType](./literals.md#engagementinvitationpayloadtypetype) 
3. See [:material-code-braces: OpportunityEngagementInvitationSortTypeDef](./type_defs.md#opportunityengagementinvitationsorttypedef) 
4. See [:material-code-brackets: InvitationStatusType](./literals.md#invitationstatustype) 
5. See [:material-code-braces: ListEngagementInvitationsResponseTypeDef](./type_defs.md#listengagementinvitationsresponsetypedef) 


```python
# list_engagement_invitations method usage example with argument unpacking

kwargs: ListEngagementInvitationsRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ParticipantType": ...,
}

parent.list_engagement_invitations(**kwargs)
```

1. See [:material-code-braces: ListEngagementInvitationsRequestTypeDef](./type_defs.md#listengagementinvitationsrequesttypedef) 

### list\_engagement\_members

Retrieves the details of member partners in an Engagement.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_engagement_members` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_engagement_members.html)

```python
# list_engagement_members method definition

await def list_engagement_members(
    self,
    *,
    Catalog: str,
    Identifier: str,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListEngagementMembersResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEngagementMembersResponseTypeDef](./type_defs.md#listengagementmembersresponsetypedef) 


```python
# list_engagement_members method usage example with argument unpacking

kwargs: ListEngagementMembersRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.list_engagement_members(**kwargs)
```

1. See [:material-code-braces: ListEngagementMembersRequestTypeDef](./type_defs.md#listengagementmembersrequesttypedef) 

### list\_engagement\_resource\_associations

Lists the associations between resources and engagements where the caller is a
member and has at least one snapshot in the engagement.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_engagement_resource_associations` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_engagement_resource_associations.html)

```python
# list_engagement_resource_associations method definition

await def list_engagement_resource_associations(
    self,
    *,
    Catalog: str,
    CreatedBy: str = ...,
    EngagementIdentifier: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ResourceIdentifier: str = ...,
    ResourceType: ResourceTypeType = ...,  # (1)
) -> ListEngagementResourceAssociationsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListEngagementResourceAssociationsResponseTypeDef](./type_defs.md#listengagementresourceassociationsresponsetypedef) 


```python
# list_engagement_resource_associations method usage example with argument unpacking

kwargs: ListEngagementResourceAssociationsRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_engagement_resource_associations(**kwargs)
```

1. See [:material-code-braces: ListEngagementResourceAssociationsRequestTypeDef](./type_defs.md#listengagementresourceassociationsrequesttypedef) 

### list\_engagements

This action allows users to retrieve a list of Engagement records from Partner
Central.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_engagements` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_engagements.html)

```python
# list_engagements method definition

await def list_engagements(
    self,
    *,
    Catalog: str,
    CreatedBy: Sequence[str] = ...,
    EngagementIdentifier: Sequence[str] = ...,
    ExcludeCreatedBy: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: EngagementSortTypeDef = ...,  # (1)
) -> ListEngagementsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EngagementSortTypeDef](./type_defs.md#engagementsorttypedef) 
2. See [:material-code-braces: ListEngagementsResponseTypeDef](./type_defs.md#listengagementsresponsetypedef) 


```python
# list_engagements method usage example with argument unpacking

kwargs: ListEngagementsRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_engagements(**kwargs)
```

1. See [:material-code-braces: ListEngagementsRequestTypeDef](./type_defs.md#listengagementsrequesttypedef) 

### list\_opportunities

This request accepts a list of filters that retrieve opportunity subsets as
well as sort options.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_opportunities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_opportunities.html)

```python
# list_opportunities method definition

await def list_opportunities(
    self,
    *,
    Catalog: str,
    CustomerCompanyName: Sequence[str] = ...,
    Identifier: Sequence[str] = ...,
    LastModifiedDate: LastModifiedDateTypeDef = ...,  # (1)
    LifeCycleReviewStatus: Sequence[ReviewStatusType] = ...,  # (2)
    LifeCycleStage: Sequence[StageType] = ...,  # (3)
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: OpportunitySortTypeDef = ...,  # (4)
) -> ListOpportunitiesResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: LastModifiedDateTypeDef](./type_defs.md#lastmodifieddatetypedef) 
2. See [:material-code-brackets: ReviewStatusType](./literals.md#reviewstatustype) 
3. See [:material-code-brackets: StageType](./literals.md#stagetype) 
4. See [:material-code-braces: OpportunitySortTypeDef](./type_defs.md#opportunitysorttypedef) 
5. See [:material-code-braces: ListOpportunitiesResponseTypeDef](./type_defs.md#listopportunitiesresponsetypedef) 


```python
# list_opportunities method usage example with argument unpacking

kwargs: ListOpportunitiesRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_opportunities(**kwargs)
```

1. See [:material-code-braces: ListOpportunitiesRequestTypeDef](./type_defs.md#listopportunitiesrequesttypedef) 

### list\_resource\_snapshot\_jobs

Lists resource snapshot jobs owned by the customer.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_resource_snapshot_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_resource_snapshot_jobs.html)

```python
# list_resource_snapshot_jobs method definition

await def list_resource_snapshot_jobs(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: SortObjectTypeDef = ...,  # (1)
    Status: ResourceSnapshotJobStatusType = ...,  # (2)
) -> ListResourceSnapshotJobsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SortObjectTypeDef](./type_defs.md#sortobjecttypedef) 
2. See [:material-code-brackets: ResourceSnapshotJobStatusType](./literals.md#resourcesnapshotjobstatustype) 
3. See [:material-code-braces: ListResourceSnapshotJobsResponseTypeDef](./type_defs.md#listresourcesnapshotjobsresponsetypedef) 


```python
# list_resource_snapshot_jobs method usage example with argument unpacking

kwargs: ListResourceSnapshotJobsRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_resource_snapshot_jobs(**kwargs)
```

1. See [:material-code-braces: ListResourceSnapshotJobsRequestTypeDef](./type_defs.md#listresourcesnapshotjobsrequesttypedef) 

### list\_resource\_snapshots

Retrieves a list of resource view snapshots based on specified criteria.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_resource_snapshots` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_resource_snapshots.html)

```python
# list_resource_snapshots method definition

await def list_resource_snapshots(
    self,
    *,
    Catalog: str,
    EngagementIdentifier: str,
    CreatedBy: str = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    ResourceIdentifier: str = ...,
    ResourceSnapshotTemplateIdentifier: str = ...,
    ResourceType: ResourceTypeType = ...,  # (1)
) -> ListResourceSnapshotsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ListResourceSnapshotsResponseTypeDef](./type_defs.md#listresourcesnapshotsresponsetypedef) 


```python
# list_resource_snapshots method usage example with argument unpacking

kwargs: ListResourceSnapshotsRequestTypeDef = {  # (1)
    "Catalog": ...,
    "EngagementIdentifier": ...,
}

parent.list_resource_snapshots(**kwargs)
```

1. See [:material-code-braces: ListResourceSnapshotsRequestTypeDef](./type_defs.md#listresourcesnapshotsrequesttypedef) 

### list\_solutions

Retrieves a list of Partner Solutions that the partner registered on Partner
Central.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_solutions` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_solutions.html)

```python
# list_solutions method definition

await def list_solutions(
    self,
    *,
    Catalog: str,
    Category: Sequence[str] = ...,
    Identifier: Sequence[str] = ...,
    MaxResults: int = ...,
    NextToken: str = ...,
    Sort: SolutionSortTypeDef = ...,  # (1)
    Status: Sequence[SolutionStatusType] = ...,  # (2)
) -> ListSolutionsResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: SolutionSortTypeDef](./type_defs.md#solutionsorttypedef) 
2. See [:material-code-brackets: SolutionStatusType](./literals.md#solutionstatustype) 
3. See [:material-code-braces: ListSolutionsResponseTypeDef](./type_defs.md#listsolutionsresponsetypedef) 


```python
# list_solutions method usage example with argument unpacking

kwargs: ListSolutionsRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.list_solutions(**kwargs)
```

1. See [:material-code-braces: ListSolutionsRequestTypeDef](./type_defs.md#listsolutionsrequesttypedef) 

### list\_tags\_for\_resource

Returns a list of tags for a resource.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/list_tags_for_resource.html)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestTypeDef](./type_defs.md#listtagsforresourcerequesttypedef) 

### put\_selling\_system\_settings

Updates the currently set system settings, which include the IAM Role used for
resource snapshot jobs.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").put_selling_system_settings` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/put_selling_system_settings.html)

```python
# put_selling_system_settings method definition

await def put_selling_system_settings(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobRoleIdentifier: str = ...,
) -> PutSellingSystemSettingsResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutSellingSystemSettingsResponseTypeDef](./type_defs.md#putsellingsystemsettingsresponsetypedef) 


```python
# put_selling_system_settings method usage example with argument unpacking

kwargs: PutSellingSystemSettingsRequestTypeDef = {  # (1)
    "Catalog": ...,
}

parent.put_selling_system_settings(**kwargs)
```

1. See [:material-code-braces: PutSellingSystemSettingsRequestTypeDef](./type_defs.md#putsellingsystemsettingsrequesttypedef) 

### reject\_engagement\_invitation

This action rejects an <code>EngagementInvitation</code> that AWS shared.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").reject_engagement_invitation` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/reject_engagement_invitation.html)

```python
# reject_engagement_invitation method definition

await def reject_engagement_invitation(
    self,
    *,
    Catalog: str,
    Identifier: str,
    RejectionReason: str = ...,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# reject_engagement_invitation method usage example with argument unpacking

kwargs: RejectEngagementInvitationRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
}

parent.reject_engagement_invitation(**kwargs)
```

1. See [:material-code-braces: RejectEngagementInvitationRequestTypeDef](./type_defs.md#rejectengagementinvitationrequesttypedef) 

### start\_engagement\_by\_accepting\_invitation\_task

This action starts the engagement by accepting an
<code>EngagementInvitation</code>.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").start_engagement_by_accepting_invitation_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/start_engagement_by_accepting_invitation_task.html)

```python
# start_engagement_by_accepting_invitation_task method definition

await def start_engagement_by_accepting_invitation_task(
    self,
    *,
    Catalog: str,
    ClientToken: str,
    Identifier: str,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> StartEngagementByAcceptingInvitationTaskResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: StartEngagementByAcceptingInvitationTaskResponseTypeDef](./type_defs.md#startengagementbyacceptinginvitationtaskresponsetypedef) 


```python
# start_engagement_by_accepting_invitation_task method usage example with argument unpacking

kwargs: StartEngagementByAcceptingInvitationTaskRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ClientToken": ...,
    "Identifier": ...,
}

parent.start_engagement_by_accepting_invitation_task(**kwargs)
```

1. See [:material-code-braces: StartEngagementByAcceptingInvitationTaskRequestTypeDef](./type_defs.md#startengagementbyacceptinginvitationtaskrequesttypedef) 

### start\_engagement\_from\_opportunity\_task

This action initiates the engagement process from an existing opportunity by
accepting the engagement invitation and creating a corresponding opportunity in
the partner's system.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").start_engagement_from_opportunity_task` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/start_engagement_from_opportunity_task.html)

```python
# start_engagement_from_opportunity_task method definition

await def start_engagement_from_opportunity_task(
    self,
    *,
    AwsSubmission: AwsSubmissionTypeDef,  # (1)
    Catalog: str,
    ClientToken: str,
    Identifier: str,
    Tags: Sequence[TagTypeDef] = ...,  # (2)
) -> StartEngagementFromOpportunityTaskResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: AwsSubmissionTypeDef](./type_defs.md#awssubmissiontypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
3. See [:material-code-braces: StartEngagementFromOpportunityTaskResponseTypeDef](./type_defs.md#startengagementfromopportunitytaskresponsetypedef) 


```python
# start_engagement_from_opportunity_task method usage example with argument unpacking

kwargs: StartEngagementFromOpportunityTaskRequestTypeDef = {  # (1)
    "AwsSubmission": ...,
    "Catalog": ...,
    "ClientToken": ...,
    "Identifier": ...,
}

parent.start_engagement_from_opportunity_task(**kwargs)
```

1. See [:material-code-braces: StartEngagementFromOpportunityTaskRequestTypeDef](./type_defs.md#startengagementfromopportunitytaskrequesttypedef) 

### start\_resource\_snapshot\_job

Starts a resource snapshot job that has been previously created.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").start_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/start_resource_snapshot_job.html)

```python
# start_resource_snapshot_job method definition

await def start_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# start_resource_snapshot_job method usage example with argument unpacking

kwargs: StartResourceSnapshotJobRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ResourceSnapshotJobIdentifier": ...,
}

parent.start_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: StartResourceSnapshotJobRequestTypeDef](./type_defs.md#startresourcesnapshotjobrequesttypedef) 

### stop\_resource\_snapshot\_job

Stops a resource snapshot job.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").stop_resource_snapshot_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/stop_resource_snapshot_job.html)

```python
# stop_resource_snapshot_job method definition

await def stop_resource_snapshot_job(
    self,
    *,
    Catalog: str,
    ResourceSnapshotJobIdentifier: str,
) -> EmptyResponseMetadataTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# stop_resource_snapshot_job method usage example with argument unpacking

kwargs: StopResourceSnapshotJobRequestTypeDef = {  # (1)
    "Catalog": ...,
    "ResourceSnapshotJobIdentifier": ...,
}

parent.stop_resource_snapshot_job(**kwargs)
```

1. See [:material-code-braces: StopResourceSnapshotJobRequestTypeDef](./type_defs.md#stopresourcesnapshotjobrequesttypedef) 

### submit\_opportunity

Use this action to submit an Opportunity that was previously created by partner
for AWS review.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").submit_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/submit_opportunity.html)

```python
# submit_opportunity method definition

await def submit_opportunity(
    self,
    *,
    Catalog: str,
    Identifier: str,
    InvolvementType: SalesInvolvementTypeType,  # (1)
    Visibility: VisibilityType = ...,  # (2)
) -> EmptyResponseMetadataTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SalesInvolvementTypeType](./literals.md#salesinvolvementtypetype) 
2. See [:material-code-brackets: VisibilityType](./literals.md#visibilitytype) 
3. See [:material-code-braces: EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef) 


```python
# submit_opportunity method usage example with argument unpacking

kwargs: SubmitOpportunityRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
    "InvolvementType": ...,
}

parent.submit_opportunity(**kwargs)
```

1. See [:material-code-braces: SubmitOpportunityRequestTypeDef](./type_defs.md#submitopportunityrequesttypedef) 

### tag\_resource

Assigns one or more tags (key-value pairs) to the specified resource.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/tag_resource.html)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestTypeDef](./type_defs.md#tagresourcerequesttypedef) 

### untag\_resource

Removes a tag or tags from a resource.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/untag_resource.html)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestTypeDef](./type_defs.md#untagresourcerequesttypedef) 

### update\_opportunity

Updates the <code>Opportunity</code> record identified by a given
<code>Identifier</code>.

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").update_opportunity` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling/client/update_opportunity.html)

```python
# update_opportunity method definition

await def update_opportunity(
    self,
    *,
    Catalog: str,
    Identifier: str,
    LastModifiedDate: TimestampTypeDef,
    Customer: CustomerUnionTypeDef = ...,  # (1)
    LifeCycle: LifeCycleUnionTypeDef = ...,  # (2)
    Marketing: MarketingUnionTypeDef = ...,  # (3)
    NationalSecurity: NationalSecurityType = ...,  # (4)
    OpportunityType: OpportunityTypeType = ...,  # (5)
    PartnerOpportunityIdentifier: str = ...,
    PrimaryNeedsFromAws: Sequence[PrimaryNeedFromAwsType] = ...,  # (6)
    Project: ProjectUnionTypeDef = ...,  # (7)
    SoftwareRevenue: SoftwareRevenueTypeDef = ...,  # (8)
) -> UpdateOpportunityResponseTypeDef:  # (9)
    ...
```

1. See [:material-code-braces: CustomerTypeDef](./type_defs.md#customertypedef) [:material-code-braces: CustomerOutputTypeDef](./type_defs.md#customeroutputtypedef) 
2. See [:material-code-braces: LifeCycleTypeDef](./type_defs.md#lifecycletypedef) [:material-code-braces: LifeCycleOutputTypeDef](./type_defs.md#lifecycleoutputtypedef) 
3. See [:material-code-braces: MarketingTypeDef](./type_defs.md#marketingtypedef) [:material-code-braces: MarketingOutputTypeDef](./type_defs.md#marketingoutputtypedef) 
4. See [:material-code-brackets: NationalSecurityType](./literals.md#nationalsecuritytype) 
5. See [:material-code-brackets: OpportunityTypeType](./literals.md#opportunitytypetype) 
6. See [:material-code-brackets: PrimaryNeedFromAwsType](./literals.md#primaryneedfromawstype) 
7. See [:material-code-braces: ProjectTypeDef](./type_defs.md#projecttypedef) [:material-code-braces: ProjectOutputTypeDef](./type_defs.md#projectoutputtypedef) 
8. See [:material-code-braces: SoftwareRevenueTypeDef](./type_defs.md#softwarerevenuetypedef) 
9. See [:material-code-braces: UpdateOpportunityResponseTypeDef](./type_defs.md#updateopportunityresponsetypedef) 


```python
# update_opportunity method usage example with argument unpacking

kwargs: UpdateOpportunityRequestTypeDef = {  # (1)
    "Catalog": ...,
    "Identifier": ...,
    "LastModifiedDate": ...,
}

parent.update_opportunity(**kwargs)
```

1. See [:material-code-braces: UpdateOpportunityRequestTypeDef](./type_defs.md#updateopportunityrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("partnercentral-selling").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("partnercentral-selling").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/partnercentral-selling.html#PartnerCentralSellingAPI.Client)

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

Type annotations and code completion for `#!python session.create_client("partnercentral-selling").get_paginator` method with overloads.

- `client.get_paginator("list_engagement_by_accepting_invitation_tasks")` -> [ListEngagementByAcceptingInvitationTasksPaginator](./paginators.md#listengagementbyacceptinginvitationtaskspaginator)
- `client.get_paginator("list_engagement_from_opportunity_tasks")` -> [ListEngagementFromOpportunityTasksPaginator](./paginators.md#listengagementfromopportunitytaskspaginator)
- `client.get_paginator("list_engagement_invitations")` -> [ListEngagementInvitationsPaginator](./paginators.md#listengagementinvitationspaginator)
- `client.get_paginator("list_engagement_members")` -> [ListEngagementMembersPaginator](./paginators.md#listengagementmemberspaginator)
- `client.get_paginator("list_engagement_resource_associations")` -> [ListEngagementResourceAssociationsPaginator](./paginators.md#listengagementresourceassociationspaginator)
- `client.get_paginator("list_engagements")` -> [ListEngagementsPaginator](./paginators.md#listengagementspaginator)
- `client.get_paginator("list_opportunities")` -> [ListOpportunitiesPaginator](./paginators.md#listopportunitiespaginator)
- `client.get_paginator("list_resource_snapshot_jobs")` -> [ListResourceSnapshotJobsPaginator](./paginators.md#listresourcesnapshotjobspaginator)
- `client.get_paginator("list_resource_snapshots")` -> [ListResourceSnapshotsPaginator](./paginators.md#listresourcesnapshotspaginator)
- `client.get_paginator("list_solutions")` -> [ListSolutionsPaginator](./paginators.md#listsolutionspaginator)




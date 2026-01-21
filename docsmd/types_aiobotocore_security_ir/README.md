# SecurityIncidentResponse module

> [Index](../README.md) > SecurityIncidentResponse


!!! note ""

    Auto-generated documentation for [SecurityIncidentResponse](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#securityincidentresponse)
    type annotations stubs module [types-aiobotocore-security-ir](https://pypi.org/project/types-aiobotocore-security-ir/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy-boto3-builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==3.1.1' mypy-boto3-builder`
1. Select `aiobotocore` AWS SDK.
1. Add `SecurityIncidentResponse` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `SecurityIncidentResponse` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[security-ir]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[security-ir]'

# standalone installation
python -m pip install types-aiobotocore-security-ir
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-security-ir
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SecurityIncidentResponseClient

Type annotations and code completion for  `#!python session.create_client("security-ir")` as [SecurityIncidentResponseClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#SecurityIncidentResponse.Client)

```python
# SecurityIncidentResponseClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_security_ir.client import SecurityIncidentResponseClient


session = get_session()
async with session.create_client("security-ir") as client:
    client: SecurityIncidentResponseClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("security-ir").get_paginator("...")`.

```python
# ListCaseEditsPaginator usage example

from types_aiobotocore_security_ir.paginator import ListCaseEditsPaginator

def get_list_case_edits_paginator() -> ListCaseEditsPaginator:
    return client.get_paginator("list_case_edits"))
```

- [ListCaseEditsPaginator](./paginators.md#listcaseeditspaginator)
- [ListCasesPaginator](./paginators.md#listcasespaginator)
- [ListCommentsPaginator](./paginators.md#listcommentspaginator)
- [ListInvestigationsPaginator](./paginators.md#listinvestigationspaginator)
- [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# ActionTypeType usage example

from types_aiobotocore_security_ir.literals import ActionTypeType

def get_value() -> ActionTypeType:
    return "Evidence"
```

- [ActionTypeType](./literals.md#actiontypetype)
- [AwsRegionType](./literals.md#awsregiontype)
- [CaseAttachmentStatusType](./literals.md#caseattachmentstatustype)
- [CaseStatusType](./literals.md#casestatustype)
- [ClosureCodeType](./literals.md#closurecodetype)
- [CommunicationTypeType](./literals.md#communicationtypetype)
- [CustomerTypeType](./literals.md#customertypetype)
- [EngagementTypeType](./literals.md#engagementtypetype)
- [ExecutionStatusType](./literals.md#executionstatustype)
- [ListCaseEditsPaginatorName](./literals.md#listcaseeditspaginatorname)
- [ListCasesPaginatorName](./literals.md#listcasespaginatorname)
- [ListCommentsPaginatorName](./literals.md#listcommentspaginatorname)
- [ListInvestigationsPaginatorName](./literals.md#listinvestigationspaginatorname)
- [ListMembershipsPaginatorName](./literals.md#listmembershipspaginatorname)
- [MembershipAccountRelationshipStatusType](./literals.md#membershipaccountrelationshipstatustype)
- [MembershipAccountRelationshipTypeType](./literals.md#membershipaccountrelationshiptypetype)
- [MembershipStatusType](./literals.md#membershipstatustype)
- [OptInFeatureNameType](./literals.md#optinfeaturenametype)
- [PendingActionType](./literals.md#pendingactiontype)
- [ResolverTypeType](./literals.md#resolvertypetype)
- [SelfManagedCaseStatusType](./literals.md#selfmanagedcasestatustype)
- [UsefulnessRatingType](./literals.md#usefulnessratingtype)
- [SecurityIncidentResponseServiceName](./literals.md#securityincidentresponseservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchGetMemberAccountDetailsRequestTypeDef](./type_defs.md#batchgetmemberaccountdetailsrequesttypedef)
- [GetMembershipAccountDetailErrorTypeDef](./type_defs.md#getmembershipaccountdetailerrortypedef)
- [GetMembershipAccountDetailItemTypeDef](./type_defs.md#getmembershipaccountdetailitemtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelMembershipRequestTypeDef](./type_defs.md#cancelmembershiprequesttypedef)
- [CaseAttachmentAttributesTypeDef](./type_defs.md#caseattachmentattributestypedef)
- [CaseEditItemTypeDef](./type_defs.md#caseedititemtypedef)
- [CaseMetadataEntryTypeDef](./type_defs.md#casemetadataentrytypedef)
- [CloseCaseRequestTypeDef](./type_defs.md#closecaserequesttypedef)
- [CreateCaseCommentRequestTypeDef](./type_defs.md#createcasecommentrequesttypedef)
- [ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef)
- [ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [WatcherTypeDef](./type_defs.md#watchertypedef)
- [OptInFeatureTypeDef](./type_defs.md#optinfeaturetypedef)
- [GetCaseAttachmentDownloadUrlRequestTypeDef](./type_defs.md#getcaseattachmentdownloadurlrequesttypedef)
- [GetCaseAttachmentUploadUrlRequestTypeDef](./type_defs.md#getcaseattachmentuploadurlrequesttypedef)
- [GetCaseRequestTypeDef](./type_defs.md#getcaserequesttypedef)
- [GetMembershipRequestTypeDef](./type_defs.md#getmembershiprequesttypedef)
- [IncidentResponderOutputTypeDef](./type_defs.md#incidentresponderoutputtypedef)
- [MembershipAccountsConfigurationsTypeDef](./type_defs.md#membershipaccountsconfigurationstypedef)
- [IncidentResponderTypeDef](./type_defs.md#incidentrespondertypedef)
- [InvestigationFeedbackTypeDef](./type_defs.md#investigationfeedbacktypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCaseEditsRequestTypeDef](./type_defs.md#listcaseeditsrequesttypedef)
- [ListCasesItemTypeDef](./type_defs.md#listcasesitemtypedef)
- [ListCasesRequestTypeDef](./type_defs.md#listcasesrequesttypedef)
- [ListCommentsItemTypeDef](./type_defs.md#listcommentsitemtypedef)
- [ListCommentsRequestTypeDef](./type_defs.md#listcommentsrequesttypedef)
- [ListInvestigationsRequestTypeDef](./type_defs.md#listinvestigationsrequesttypedef)
- [ListMembershipItemTypeDef](./type_defs.md#listmembershipitemtypedef)
- [ListMembershipsRequestTypeDef](./type_defs.md#listmembershipsrequesttypedef)
- [ListTagsForResourceInputTypeDef](./type_defs.md#listtagsforresourceinputtypedef)
- [MembershipAccountsConfigurationsUpdateTypeDef](./type_defs.md#membershipaccountsconfigurationsupdatetypedef)
- [SendFeedbackRequestTypeDef](./type_defs.md#sendfeedbackrequesttypedef)
- [TagResourceInputTypeDef](./type_defs.md#tagresourceinputtypedef)
- [UntagResourceInputTypeDef](./type_defs.md#untagresourceinputtypedef)
- [UpdateCaseCommentRequestTypeDef](./type_defs.md#updatecasecommentrequesttypedef)
- [UpdateCaseStatusRequestTypeDef](./type_defs.md#updatecasestatusrequesttypedef)
- [UpdateResolverTypeRequestTypeDef](./type_defs.md#updateresolvertyperequesttypedef)
- [BatchGetMemberAccountDetailsResponseTypeDef](./type_defs.md#batchgetmemberaccountdetailsresponsetypedef)
- [CancelMembershipResponseTypeDef](./type_defs.md#cancelmembershipresponsetypedef)
- [CloseCaseResponseTypeDef](./type_defs.md#closecaseresponsetypedef)
- [CreateCaseCommentResponseTypeDef](./type_defs.md#createcasecommentresponsetypedef)
- [CreateCaseResponseTypeDef](./type_defs.md#createcaseresponsetypedef)
- [CreateMembershipResponseTypeDef](./type_defs.md#createmembershipresponsetypedef)
- [GetCaseAttachmentDownloadUrlResponseTypeDef](./type_defs.md#getcaseattachmentdownloadurlresponsetypedef)
- [GetCaseAttachmentUploadUrlResponseTypeDef](./type_defs.md#getcaseattachmentuploadurlresponsetypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [UpdateCaseCommentResponseTypeDef](./type_defs.md#updatecasecommentresponsetypedef)
- [UpdateCaseStatusResponseTypeDef](./type_defs.md#updatecasestatusresponsetypedef)
- [UpdateResolverTypeResponseTypeDef](./type_defs.md#updateresolvertyperesponsetypedef)
- [ListCaseEditsResponseTypeDef](./type_defs.md#listcaseeditsresponsetypedef)
- [CreateCaseRequestTypeDef](./type_defs.md#createcaserequesttypedef)
- [GetCaseResponseTypeDef](./type_defs.md#getcaseresponsetypedef)
- [UpdateCaseRequestTypeDef](./type_defs.md#updatecaserequesttypedef)
- [GetMembershipResponseTypeDef](./type_defs.md#getmembershipresponsetypedef)
- [IncidentResponderUnionTypeDef](./type_defs.md#incidentresponderuniontypedef)
- [InvestigationActionTypeDef](./type_defs.md#investigationactiontypedef)
- [ListCaseEditsRequestPaginateTypeDef](./type_defs.md#listcaseeditsrequestpaginatetypedef)
- [ListCasesRequestPaginateTypeDef](./type_defs.md#listcasesrequestpaginatetypedef)
- [ListCommentsRequestPaginateTypeDef](./type_defs.md#listcommentsrequestpaginatetypedef)
- [ListInvestigationsRequestPaginateTypeDef](./type_defs.md#listinvestigationsrequestpaginatetypedef)
- [ListMembershipsRequestPaginateTypeDef](./type_defs.md#listmembershipsrequestpaginatetypedef)
- [ListCasesResponseTypeDef](./type_defs.md#listcasesresponsetypedef)
- [ListCommentsResponseTypeDef](./type_defs.md#listcommentsresponsetypedef)
- [ListMembershipsResponseTypeDef](./type_defs.md#listmembershipsresponsetypedef)
- [CreateMembershipRequestTypeDef](./type_defs.md#createmembershiprequesttypedef)
- [UpdateMembershipRequestTypeDef](./type_defs.md#updatemembershiprequesttypedef)
- [ListInvestigationsResponseTypeDef](./type_defs.md#listinvestigationsresponsetypedef)


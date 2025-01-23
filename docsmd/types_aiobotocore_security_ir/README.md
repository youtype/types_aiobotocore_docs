# SecurityIncidentResponse module

> [Index](../README.md) > SecurityIncidentResponse


!!! note ""

    Auto-generated documentation for [SecurityIncidentResponse](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/security-ir.html#securityincidentresponse)
    type annotations stubs module [types-aiobotocore-security-ir](https://pypi.org/project/types-aiobotocore-security-ir/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
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
- [ListMembershipsPaginator](./paginators.md#listmembershipspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AwsRegionType usage example

from types_aiobotocore_security_ir.literals import AwsRegionType

def get_value() -> AwsRegionType:
    return "af-south-1"
```

- [AwsRegionType](./literals.md#awsregiontype)
- [CaseAttachmentStatusType](./literals.md#caseattachmentstatustype)
- [CaseStatusType](./literals.md#casestatustype)
- [ClosureCodeType](./literals.md#closurecodetype)
- [CustomerTypeType](./literals.md#customertypetype)
- [EngagementTypeType](./literals.md#engagementtypetype)
- [ListCaseEditsPaginatorName](./literals.md#listcaseeditspaginatorname)
- [ListCasesPaginatorName](./literals.md#listcasespaginatorname)
- [ListCommentsPaginatorName](./literals.md#listcommentspaginatorname)
- [ListMembershipsPaginatorName](./literals.md#listmembershipspaginatorname)
- [MembershipAccountRelationshipStatusType](./literals.md#membershipaccountrelationshipstatustype)
- [MembershipAccountRelationshipTypeType](./literals.md#membershipaccountrelationshiptypetype)
- [MembershipStatusType](./literals.md#membershipstatustype)
- [OptInFeatureNameType](./literals.md#optinfeaturenametype)
- [PendingActionType](./literals.md#pendingactiontype)
- [ResolverTypeType](./literals.md#resolvertypetype)
- [SelfManagedCaseStatusType](./literals.md#selfmanagedcasestatustype)
- [SecurityIncidentResponseServiceName](./literals.md#securityincidentresponseservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [BatchGetMemberAccountDetailsRequestRequestTypeDef](./type_defs.md#batchgetmemberaccountdetailsrequestrequesttypedef)
- [GetMembershipAccountDetailErrorTypeDef](./type_defs.md#getmembershipaccountdetailerrortypedef)
- [GetMembershipAccountDetailItemTypeDef](./type_defs.md#getmembershipaccountdetailitemtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CancelMembershipRequestRequestTypeDef](./type_defs.md#cancelmembershiprequestrequesttypedef)
- [CaseAttachmentAttributesTypeDef](./type_defs.md#caseattachmentattributestypedef)
- [CaseEditItemTypeDef](./type_defs.md#caseedititemtypedef)
- [CloseCaseRequestRequestTypeDef](./type_defs.md#closecaserequestrequesttypedef)
- [CreateCaseCommentRequestRequestTypeDef](./type_defs.md#createcasecommentrequestrequesttypedef)
- [ImpactedAwsRegionTypeDef](./type_defs.md#impactedawsregiontypedef)
- [ThreatActorIpTypeDef](./type_defs.md#threatactoriptypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [WatcherTypeDef](./type_defs.md#watchertypedef)
- [IncidentResponderTypeDef](./type_defs.md#incidentrespondertypedef)
- [OptInFeatureTypeDef](./type_defs.md#optinfeaturetypedef)
- [GetCaseAttachmentDownloadUrlRequestRequestTypeDef](./type_defs.md#getcaseattachmentdownloadurlrequestrequesttypedef)
- [GetCaseAttachmentUploadUrlRequestRequestTypeDef](./type_defs.md#getcaseattachmentuploadurlrequestrequesttypedef)
- [GetCaseRequestRequestTypeDef](./type_defs.md#getcaserequestrequesttypedef)
- [GetMembershipRequestRequestTypeDef](./type_defs.md#getmembershiprequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListCaseEditsRequestRequestTypeDef](./type_defs.md#listcaseeditsrequestrequesttypedef)
- [ListCasesItemTypeDef](./type_defs.md#listcasesitemtypedef)
- [ListCasesRequestRequestTypeDef](./type_defs.md#listcasesrequestrequesttypedef)
- [ListCommentsItemTypeDef](./type_defs.md#listcommentsitemtypedef)
- [ListCommentsRequestRequestTypeDef](./type_defs.md#listcommentsrequestrequesttypedef)
- [ListMembershipItemTypeDef](./type_defs.md#listmembershipitemtypedef)
- [ListMembershipsRequestRequestTypeDef](./type_defs.md#listmembershipsrequestrequesttypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateCaseCommentRequestRequestTypeDef](./type_defs.md#updatecasecommentrequestrequesttypedef)
- [UpdateCaseStatusRequestRequestTypeDef](./type_defs.md#updatecasestatusrequestrequesttypedef)
- [UpdateResolverTypeRequestRequestTypeDef](./type_defs.md#updateresolvertyperequestrequesttypedef)
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
- [CreateCaseRequestRequestTypeDef](./type_defs.md#createcaserequestrequesttypedef)
- [GetCaseResponseTypeDef](./type_defs.md#getcaseresponsetypedef)
- [UpdateCaseRequestRequestTypeDef](./type_defs.md#updatecaserequestrequesttypedef)
- [CreateMembershipRequestRequestTypeDef](./type_defs.md#createmembershiprequestrequesttypedef)
- [GetMembershipResponseTypeDef](./type_defs.md#getmembershipresponsetypedef)
- [UpdateMembershipRequestRequestTypeDef](./type_defs.md#updatemembershiprequestrequesttypedef)
- [ListCaseEditsRequestPaginateTypeDef](./type_defs.md#listcaseeditsrequestpaginatetypedef)
- [ListCasesRequestPaginateTypeDef](./type_defs.md#listcasesrequestpaginatetypedef)
- [ListCommentsRequestPaginateTypeDef](./type_defs.md#listcommentsrequestpaginatetypedef)
- [ListMembershipsRequestPaginateTypeDef](./type_defs.md#listmembershipsrequestpaginatetypedef)
- [ListCasesResponseTypeDef](./type_defs.md#listcasesresponsetypedef)
- [ListCommentsResponseTypeDef](./type_defs.md#listcommentsresponsetypedef)
- [ListMembershipsResponseTypeDef](./type_defs.md#listmembershipsresponsetypedef)


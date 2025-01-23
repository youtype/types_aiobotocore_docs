# MTurk module

> [Index](../README.md) > MTurk


!!! note ""

    Auto-generated documentation for [MTurk](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#mturk)
    type annotations stubs module [types-aiobotocore-mturk](https://pypi.org/project/types-aiobotocore-mturk/).

## How to install

### Generate locally (recommended)

You can generate type annotations for `aiobotocore` package locally with `mypy_boto3_builder`.
Use [uv](https://docs.astral.sh/uv/getting-started/installation/) for build isolation.

1. Run mypy-boto3-builder in your package root directory: `uvx --with 'aiobotocore==2.19.0' mypy_boto3_builder`
1. Select `aiobotocore` AWS SDK.
1. Add `MTurk` service.
1. Use provided commands to install generated packages.



### From PyPI with pip

Install `types-aiobotocore` for `MTurk` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[mturk]'

# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[mturk]'

# standalone installation
python -m pip install types-aiobotocore-mturk
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-mturk
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MTurkClient

Type annotations and code completion for  `#!python session.create_client("mturk")` as [MTurkClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mturk.html#MTurk.Client)

```python
# MTurkClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_mturk.client import MTurkClient


session = get_session()
async with session.create_client("mturk") as client:
    client: MTurkClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("mturk").get_paginator("...")`.

```python
# ListAssignmentsForHITPaginator usage example

from types_aiobotocore_mturk.paginator import ListAssignmentsForHITPaginator

def get_list_assignments_for_hit_paginator() -> ListAssignmentsForHITPaginator:
    return client.get_paginator("list_assignments_for_hit"))
```

- [ListAssignmentsForHITPaginator](./paginators.md#listassignmentsforhitpaginator)
- [ListBonusPaymentsPaginator](./paginators.md#listbonuspaymentspaginator)
- [ListHITsForQualificationTypePaginator](./paginators.md#listhitsforqualificationtypepaginator)
- [ListHITsPaginator](./paginators.md#listhitspaginator)
- [ListQualificationRequestsPaginator](./paginators.md#listqualificationrequestspaginator)
- [ListQualificationTypesPaginator](./paginators.md#listqualificationtypespaginator)
- [ListReviewableHITsPaginator](./paginators.md#listreviewablehitspaginator)
- [ListWorkerBlocksPaginator](./paginators.md#listworkerblockspaginator)
- [ListWorkersWithQualificationTypePaginator](./paginators.md#listworkerswithqualificationtypepaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AssignmentStatusType usage example

from types_aiobotocore_mturk.literals import AssignmentStatusType

def get_value() -> AssignmentStatusType:
    return "Approved"
```

- [AssignmentStatusType](./literals.md#assignmentstatustype)
- [ComparatorType](./literals.md#comparatortype)
- [EventTypeType](./literals.md#eventtypetype)
- [HITAccessActionsType](./literals.md#hitaccessactionstype)
- [HITReviewStatusType](./literals.md#hitreviewstatustype)
- [HITStatusType](./literals.md#hitstatustype)
- [ListAssignmentsForHITPaginatorName](./literals.md#listassignmentsforhitpaginatorname)
- [ListBonusPaymentsPaginatorName](./literals.md#listbonuspaymentspaginatorname)
- [ListHITsForQualificationTypePaginatorName](./literals.md#listhitsforqualificationtypepaginatorname)
- [ListHITsPaginatorName](./literals.md#listhitspaginatorname)
- [ListQualificationRequestsPaginatorName](./literals.md#listqualificationrequestspaginatorname)
- [ListQualificationTypesPaginatorName](./literals.md#listqualificationtypespaginatorname)
- [ListReviewableHITsPaginatorName](./literals.md#listreviewablehitspaginatorname)
- [ListWorkerBlocksPaginatorName](./literals.md#listworkerblockspaginatorname)
- [ListWorkersWithQualificationTypePaginatorName](./literals.md#listworkerswithqualificationtypepaginatorname)
- [NotificationTransportType](./literals.md#notificationtransporttype)
- [NotifyWorkersFailureCodeType](./literals.md#notifyworkersfailurecodetype)
- [QualificationStatusType](./literals.md#qualificationstatustype)
- [QualificationTypeStatusType](./literals.md#qualificationtypestatustype)
- [ReviewActionStatusType](./literals.md#reviewactionstatustype)
- [ReviewPolicyLevelType](./literals.md#reviewpolicyleveltype)
- [ReviewableHITStatusType](./literals.md#reviewablehitstatustype)
- [MTurkServiceName](./literals.md#mturkservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptQualificationRequestRequestRequestTypeDef](./type_defs.md#acceptqualificationrequestrequestrequesttypedef)
- [ApproveAssignmentRequestRequestTypeDef](./type_defs.md#approveassignmentrequestrequesttypedef)
- [AssignmentTypeDef](./type_defs.md#assignmenttypedef)
- [AssociateQualificationWithWorkerRequestRequestTypeDef](./type_defs.md#associatequalificationwithworkerrequestrequesttypedef)
- [BonusPaymentTypeDef](./type_defs.md#bonuspaymenttypedef)
- [CreateAdditionalAssignmentsForHITRequestRequestTypeDef](./type_defs.md#createadditionalassignmentsforhitrequestrequesttypedef)
- [HITLayoutParameterTypeDef](./type_defs.md#hitlayoutparametertypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [CreateQualificationTypeRequestRequestTypeDef](./type_defs.md#createqualificationtyperequestrequesttypedef)
- [QualificationTypeTypeDef](./type_defs.md#qualificationtypetypedef)
- [CreateWorkerBlockRequestRequestTypeDef](./type_defs.md#createworkerblockrequestrequesttypedef)
- [DeleteHITRequestRequestTypeDef](./type_defs.md#deletehitrequestrequesttypedef)
- [DeleteQualificationTypeRequestRequestTypeDef](./type_defs.md#deletequalificationtyperequestrequesttypedef)
- [DeleteWorkerBlockRequestRequestTypeDef](./type_defs.md#deleteworkerblockrequestrequesttypedef)
- [DisassociateQualificationFromWorkerRequestRequestTypeDef](./type_defs.md#disassociatequalificationfromworkerrequestrequesttypedef)
- [GetAssignmentRequestRequestTypeDef](./type_defs.md#getassignmentrequestrequesttypedef)
- [GetFileUploadURLRequestRequestTypeDef](./type_defs.md#getfileuploadurlrequestrequesttypedef)
- [GetHITRequestRequestTypeDef](./type_defs.md#gethitrequestrequesttypedef)
- [GetQualificationScoreRequestRequestTypeDef](./type_defs.md#getqualificationscorerequestrequesttypedef)
- [GetQualificationTypeRequestRequestTypeDef](./type_defs.md#getqualificationtyperequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListAssignmentsForHITRequestRequestTypeDef](./type_defs.md#listassignmentsforhitrequestrequesttypedef)
- [ListBonusPaymentsRequestRequestTypeDef](./type_defs.md#listbonuspaymentsrequestrequesttypedef)
- [ListHITsForQualificationTypeRequestRequestTypeDef](./type_defs.md#listhitsforqualificationtyperequestrequesttypedef)
- [ListHITsRequestRequestTypeDef](./type_defs.md#listhitsrequestrequesttypedef)
- [ListQualificationRequestsRequestRequestTypeDef](./type_defs.md#listqualificationrequestsrequestrequesttypedef)
- [QualificationRequestTypeDef](./type_defs.md#qualificationrequesttypedef)
- [ListQualificationTypesRequestRequestTypeDef](./type_defs.md#listqualificationtypesrequestrequesttypedef)
- [ListReviewPolicyResultsForHITRequestRequestTypeDef](./type_defs.md#listreviewpolicyresultsforhitrequestrequesttypedef)
- [ListReviewableHITsRequestRequestTypeDef](./type_defs.md#listreviewablehitsrequestrequesttypedef)
- [ListWorkerBlocksRequestRequestTypeDef](./type_defs.md#listworkerblocksrequestrequesttypedef)
- [WorkerBlockTypeDef](./type_defs.md#workerblocktypedef)
- [ListWorkersWithQualificationTypeRequestRequestTypeDef](./type_defs.md#listworkerswithqualificationtyperequestrequesttypedef)
- [LocaleTypeDef](./type_defs.md#localetypedef)
- [NotificationSpecificationTypeDef](./type_defs.md#notificationspecificationtypedef)
- [NotifyWorkersFailureStatusTypeDef](./type_defs.md#notifyworkersfailurestatustypedef)
- [NotifyWorkersRequestRequestTypeDef](./type_defs.md#notifyworkersrequestrequesttypedef)
- [ParameterMapEntryOutputTypeDef](./type_defs.md#parametermapentryoutputtypedef)
- [ParameterMapEntryTypeDef](./type_defs.md#parametermapentrytypedef)
- [RejectAssignmentRequestRequestTypeDef](./type_defs.md#rejectassignmentrequestrequesttypedef)
- [RejectQualificationRequestRequestRequestTypeDef](./type_defs.md#rejectqualificationrequestrequestrequesttypedef)
- [ReviewActionDetailTypeDef](./type_defs.md#reviewactiondetailtypedef)
- [ReviewResultDetailTypeDef](./type_defs.md#reviewresultdetailtypedef)
- [SendBonusRequestRequestTypeDef](./type_defs.md#sendbonusrequestrequesttypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [UpdateHITReviewStatusRequestRequestTypeDef](./type_defs.md#updatehitreviewstatusrequestrequesttypedef)
- [UpdateHITTypeOfHITRequestRequestTypeDef](./type_defs.md#updatehittypeofhitrequestrequesttypedef)
- [UpdateQualificationTypeRequestRequestTypeDef](./type_defs.md#updatequalificationtyperequestrequesttypedef)
- [CreateHITTypeResponseTypeDef](./type_defs.md#createhittyperesponsetypedef)
- [GetAccountBalanceResponseTypeDef](./type_defs.md#getaccountbalanceresponsetypedef)
- [GetFileUploadURLResponseTypeDef](./type_defs.md#getfileuploadurlresponsetypedef)
- [ListAssignmentsForHITResponseTypeDef](./type_defs.md#listassignmentsforhitresponsetypedef)
- [ListBonusPaymentsResponseTypeDef](./type_defs.md#listbonuspaymentsresponsetypedef)
- [CreateQualificationTypeResponseTypeDef](./type_defs.md#createqualificationtyperesponsetypedef)
- [GetQualificationTypeResponseTypeDef](./type_defs.md#getqualificationtyperesponsetypedef)
- [ListQualificationTypesResponseTypeDef](./type_defs.md#listqualificationtypesresponsetypedef)
- [UpdateQualificationTypeResponseTypeDef](./type_defs.md#updatequalificationtyperesponsetypedef)
- [ListAssignmentsForHITRequestPaginateTypeDef](./type_defs.md#listassignmentsforhitrequestpaginatetypedef)
- [ListBonusPaymentsRequestPaginateTypeDef](./type_defs.md#listbonuspaymentsrequestpaginatetypedef)
- [ListHITsForQualificationTypeRequestPaginateTypeDef](./type_defs.md#listhitsforqualificationtyperequestpaginatetypedef)
- [ListHITsRequestPaginateTypeDef](./type_defs.md#listhitsrequestpaginatetypedef)
- [ListQualificationRequestsRequestPaginateTypeDef](./type_defs.md#listqualificationrequestsrequestpaginatetypedef)
- [ListQualificationTypesRequestPaginateTypeDef](./type_defs.md#listqualificationtypesrequestpaginatetypedef)
- [ListReviewableHITsRequestPaginateTypeDef](./type_defs.md#listreviewablehitsrequestpaginatetypedef)
- [ListWorkerBlocksRequestPaginateTypeDef](./type_defs.md#listworkerblocksrequestpaginatetypedef)
- [ListWorkersWithQualificationTypeRequestPaginateTypeDef](./type_defs.md#listworkerswithqualificationtyperequestpaginatetypedef)
- [ListQualificationRequestsResponseTypeDef](./type_defs.md#listqualificationrequestsresponsetypedef)
- [ListWorkerBlocksResponseTypeDef](./type_defs.md#listworkerblocksresponsetypedef)
- [QualificationRequirementOutputTypeDef](./type_defs.md#qualificationrequirementoutputtypedef)
- [QualificationRequirementTypeDef](./type_defs.md#qualificationrequirementtypedef)
- [QualificationTypeDef](./type_defs.md#qualificationtypedef)
- [SendTestEventNotificationRequestRequestTypeDef](./type_defs.md#sendtesteventnotificationrequestrequesttypedef)
- [UpdateNotificationSettingsRequestRequestTypeDef](./type_defs.md#updatenotificationsettingsrequestrequesttypedef)
- [NotifyWorkersResponseTypeDef](./type_defs.md#notifyworkersresponsetypedef)
- [PolicyParameterOutputTypeDef](./type_defs.md#policyparameteroutputtypedef)
- [ParameterMapEntryUnionTypeDef](./type_defs.md#parametermapentryuniontypedef)
- [ReviewReportTypeDef](./type_defs.md#reviewreporttypedef)
- [UpdateExpirationForHITRequestRequestTypeDef](./type_defs.md#updateexpirationforhitrequestrequesttypedef)
- [HITTypeDef](./type_defs.md#hittypedef)
- [CreateHITTypeRequestRequestTypeDef](./type_defs.md#createhittyperequestrequesttypedef)
- [QualificationRequirementUnionTypeDef](./type_defs.md#qualificationrequirementuniontypedef)
- [GetQualificationScoreResponseTypeDef](./type_defs.md#getqualificationscoreresponsetypedef)
- [ListWorkersWithQualificationTypeResponseTypeDef](./type_defs.md#listworkerswithqualificationtyperesponsetypedef)
- [ReviewPolicyOutputTypeDef](./type_defs.md#reviewpolicyoutputtypedef)
- [PolicyParameterTypeDef](./type_defs.md#policyparametertypedef)
- [CreateHITResponseTypeDef](./type_defs.md#createhitresponsetypedef)
- [CreateHITWithHITTypeResponseTypeDef](./type_defs.md#createhitwithhittyperesponsetypedef)
- [GetAssignmentResponseTypeDef](./type_defs.md#getassignmentresponsetypedef)
- [GetHITResponseTypeDef](./type_defs.md#gethitresponsetypedef)
- [ListHITsForQualificationTypeResponseTypeDef](./type_defs.md#listhitsforqualificationtyperesponsetypedef)
- [ListHITsResponseTypeDef](./type_defs.md#listhitsresponsetypedef)
- [ListReviewableHITsResponseTypeDef](./type_defs.md#listreviewablehitsresponsetypedef)
- [ListReviewPolicyResultsForHITResponseTypeDef](./type_defs.md#listreviewpolicyresultsforhitresponsetypedef)
- [PolicyParameterUnionTypeDef](./type_defs.md#policyparameteruniontypedef)
- [ReviewPolicyTypeDef](./type_defs.md#reviewpolicytypedef)
- [CreateHITRequestRequestTypeDef](./type_defs.md#createhitrequestrequesttypedef)
- [CreateHITWithHITTypeRequestRequestTypeDef](./type_defs.md#createhitwithhittyperequestrequesttypedef)


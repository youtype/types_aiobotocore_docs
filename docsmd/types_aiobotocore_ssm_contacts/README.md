# SSMContacts module

> [Index](../README.md) > SSMContacts


!!! note ""

    Auto-generated documentation for [SSMContacts](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts)
    type annotations stubs module [types-aiobotocore-ssm-contacts](https://pypi.org/project/types-aiobotocore-ssm-contacts/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `SSMContacts` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[ssm-contacts]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[ssm-contacts]'


# standalone installation
python -m pip install types-aiobotocore-ssm-contacts
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-ssm-contacts
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SSMContactsClient

Type annotations and code completion for  `#!python session.create_client("ssm-contacts")` as [SSMContactsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm-contacts.html#SSMContacts.Client)

```python
# SSMContactsClient usage example

from aiobotocore.session import get_session

from types_aiobotocore_ssm_contacts.client import SSMContactsClient


session = get_session()
async with session.create_client("ssm-contacts") as client:
    client: SSMContactsClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("ssm-contacts").get_paginator("...")`.

```python
# ListContactChannelsPaginator usage example

from types_aiobotocore_ssm_contacts.paginator import ListContactChannelsPaginator

def get_list_contact_channels_paginator() -> ListContactChannelsPaginator:
    return client.get_paginator("list_contact_channels"))
```

- [ListContactChannelsPaginator](./paginators.md#listcontactchannelspaginator)
- [ListContactsPaginator](./paginators.md#listcontactspaginator)
- [ListEngagementsPaginator](./paginators.md#listengagementspaginator)
- [ListPageReceiptsPaginator](./paginators.md#listpagereceiptspaginator)
- [ListPageResolutionsPaginator](./paginators.md#listpageresolutionspaginator)
- [ListPagesByContactPaginator](./paginators.md#listpagesbycontactpaginator)
- [ListPagesByEngagementPaginator](./paginators.md#listpagesbyengagementpaginator)
- [ListPreviewRotationShiftsPaginator](./paginators.md#listpreviewrotationshiftspaginator)
- [ListRotationOverridesPaginator](./paginators.md#listrotationoverridespaginator)
- [ListRotationShiftsPaginator](./paginators.md#listrotationshiftspaginator)
- [ListRotationsPaginator](./paginators.md#listrotationspaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python
# AcceptCodeValidationType usage example

from types_aiobotocore_ssm_contacts.literals import AcceptCodeValidationType

def get_value() -> AcceptCodeValidationType:
    return "ENFORCE"
```

- [AcceptCodeValidationType](./literals.md#acceptcodevalidationtype)
- [AcceptTypeType](./literals.md#accepttypetype)
- [ActivationStatusType](./literals.md#activationstatustype)
- [ChannelTypeType](./literals.md#channeltypetype)
- [ContactTypeType](./literals.md#contacttypetype)
- [DayOfWeekType](./literals.md#dayofweektype)
- [ListContactChannelsPaginatorName](./literals.md#listcontactchannelspaginatorname)
- [ListContactsPaginatorName](./literals.md#listcontactspaginatorname)
- [ListEngagementsPaginatorName](./literals.md#listengagementspaginatorname)
- [ListPageReceiptsPaginatorName](./literals.md#listpagereceiptspaginatorname)
- [ListPageResolutionsPaginatorName](./literals.md#listpageresolutionspaginatorname)
- [ListPagesByContactPaginatorName](./literals.md#listpagesbycontactpaginatorname)
- [ListPagesByEngagementPaginatorName](./literals.md#listpagesbyengagementpaginatorname)
- [ListPreviewRotationShiftsPaginatorName](./literals.md#listpreviewrotationshiftspaginatorname)
- [ListRotationOverridesPaginatorName](./literals.md#listrotationoverridespaginatorname)
- [ListRotationShiftsPaginatorName](./literals.md#listrotationshiftspaginatorname)
- [ListRotationsPaginatorName](./literals.md#listrotationspaginatorname)
- [ReceiptTypeType](./literals.md#receipttypetype)
- [ShiftTypeType](./literals.md#shifttypetype)
- [SSMContactsServiceName](./literals.md#ssmcontactsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Type definitions

Type annotations for [type definitions](./type_defs.md) used in methods and schema.

- [AcceptPageRequestRequestTypeDef](./type_defs.md#acceptpagerequestrequesttypedef)
- [ActivateContactChannelRequestRequestTypeDef](./type_defs.md#activatecontactchannelrequestrequesttypedef)
- [ChannelTargetInfoTypeDef](./type_defs.md#channeltargetinfotypedef)
- [ContactChannelAddressTypeDef](./type_defs.md#contactchanneladdresstypedef)
- [ContactTargetInfoTypeDef](./type_defs.md#contacttargetinfotypedef)
- [ContactTypeDef](./type_defs.md#contacttypedef)
- [HandOffTimeTypeDef](./type_defs.md#handofftimetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [TimestampTypeDef](./type_defs.md#timestamptypedef)
- [DeactivateContactChannelRequestRequestTypeDef](./type_defs.md#deactivatecontactchannelrequestrequesttypedef)
- [DeleteContactChannelRequestRequestTypeDef](./type_defs.md#deletecontactchannelrequestrequesttypedef)
- [DeleteContactRequestRequestTypeDef](./type_defs.md#deletecontactrequestrequesttypedef)
- [DeleteRotationOverrideRequestRequestTypeDef](./type_defs.md#deleterotationoverriderequestrequesttypedef)
- [DeleteRotationRequestRequestTypeDef](./type_defs.md#deleterotationrequestrequesttypedef)
- [DescribeEngagementRequestRequestTypeDef](./type_defs.md#describeengagementrequestrequesttypedef)
- [DescribePageRequestRequestTypeDef](./type_defs.md#describepagerequestrequesttypedef)
- [EngagementTypeDef](./type_defs.md#engagementtypedef)
- [GetContactChannelRequestRequestTypeDef](./type_defs.md#getcontactchannelrequestrequesttypedef)
- [GetContactPolicyRequestRequestTypeDef](./type_defs.md#getcontactpolicyrequestrequesttypedef)
- [GetContactRequestRequestTypeDef](./type_defs.md#getcontactrequestrequesttypedef)
- [GetRotationOverrideRequestRequestTypeDef](./type_defs.md#getrotationoverriderequestrequesttypedef)
- [GetRotationRequestRequestTypeDef](./type_defs.md#getrotationrequestrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListContactChannelsRequestRequestTypeDef](./type_defs.md#listcontactchannelsrequestrequesttypedef)
- [ListContactsRequestRequestTypeDef](./type_defs.md#listcontactsrequestrequesttypedef)
- [ListPageReceiptsRequestRequestTypeDef](./type_defs.md#listpagereceiptsrequestrequesttypedef)
- [ReceiptTypeDef](./type_defs.md#receipttypedef)
- [ListPageResolutionsRequestRequestTypeDef](./type_defs.md#listpageresolutionsrequestrequesttypedef)
- [ResolutionContactTypeDef](./type_defs.md#resolutioncontacttypedef)
- [ListPagesByContactRequestRequestTypeDef](./type_defs.md#listpagesbycontactrequestrequesttypedef)
- [PageTypeDef](./type_defs.md#pagetypedef)
- [ListPagesByEngagementRequestRequestTypeDef](./type_defs.md#listpagesbyengagementrequestrequesttypedef)
- [RotationOverrideTypeDef](./type_defs.md#rotationoverridetypedef)
- [ListRotationsRequestRequestTypeDef](./type_defs.md#listrotationsrequestrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [PutContactPolicyRequestRequestTypeDef](./type_defs.md#putcontactpolicyrequestrequesttypedef)
- [ShiftDetailsTypeDef](./type_defs.md#shiftdetailstypedef)
- [SendActivationCodeRequestRequestTypeDef](./type_defs.md#sendactivationcoderequestrequesttypedef)
- [StartEngagementRequestRequestTypeDef](./type_defs.md#startengagementrequestrequesttypedef)
- [StopEngagementRequestRequestTypeDef](./type_defs.md#stopengagementrequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [ContactChannelTypeDef](./type_defs.md#contactchanneltypedef)
- [CreateContactChannelRequestRequestTypeDef](./type_defs.md#createcontactchannelrequestrequesttypedef)
- [UpdateContactChannelRequestRequestTypeDef](./type_defs.md#updatecontactchannelrequestrequesttypedef)
- [TargetTypeDef](./type_defs.md#targettypedef)
- [CoverageTimeTypeDef](./type_defs.md#coveragetimetypedef)
- [MonthlySettingTypeDef](./type_defs.md#monthlysettingtypedef)
- [WeeklySettingTypeDef](./type_defs.md#weeklysettingtypedef)
- [CreateContactChannelResultTypeDef](./type_defs.md#createcontactchannelresulttypedef)
- [CreateContactResultTypeDef](./type_defs.md#createcontactresulttypedef)
- [CreateRotationOverrideResultTypeDef](./type_defs.md#createrotationoverrideresulttypedef)
- [CreateRotationResultTypeDef](./type_defs.md#createrotationresulttypedef)
- [DescribeEngagementResultTypeDef](./type_defs.md#describeengagementresulttypedef)
- [DescribePageResultTypeDef](./type_defs.md#describepageresulttypedef)
- [GetContactChannelResultTypeDef](./type_defs.md#getcontactchannelresulttypedef)
- [GetContactPolicyResultTypeDef](./type_defs.md#getcontactpolicyresulttypedef)
- [GetRotationOverrideResultTypeDef](./type_defs.md#getrotationoverrideresulttypedef)
- [ListContactsResultTypeDef](./type_defs.md#listcontactsresulttypedef)
- [StartEngagementResultTypeDef](./type_defs.md#startengagementresulttypedef)
- [ListTagsForResourceResultTypeDef](./type_defs.md#listtagsforresourceresulttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [CreateRotationOverrideRequestRequestTypeDef](./type_defs.md#createrotationoverriderequestrequesttypedef)
- [ListRotationOverridesRequestRequestTypeDef](./type_defs.md#listrotationoverridesrequestrequesttypedef)
- [ListRotationShiftsRequestRequestTypeDef](./type_defs.md#listrotationshiftsrequestrequesttypedef)
- [PreviewOverrideTypeDef](./type_defs.md#previewoverridetypedef)
- [TimeRangeTypeDef](./type_defs.md#timerangetypedef)
- [ListEngagementsResultTypeDef](./type_defs.md#listengagementsresulttypedef)
- [ListContactChannelsRequestListContactChannelsPaginateTypeDef](./type_defs.md#listcontactchannelsrequestlistcontactchannelspaginatetypedef)
- [ListContactsRequestListContactsPaginateTypeDef](./type_defs.md#listcontactsrequestlistcontactspaginatetypedef)
- [ListPageReceiptsRequestListPageReceiptsPaginateTypeDef](./type_defs.md#listpagereceiptsrequestlistpagereceiptspaginatetypedef)
- [ListPageResolutionsRequestListPageResolutionsPaginateTypeDef](./type_defs.md#listpageresolutionsrequestlistpageresolutionspaginatetypedef)
- [ListPagesByContactRequestListPagesByContactPaginateTypeDef](./type_defs.md#listpagesbycontactrequestlistpagesbycontactpaginatetypedef)
- [ListPagesByEngagementRequestListPagesByEngagementPaginateTypeDef](./type_defs.md#listpagesbyengagementrequestlistpagesbyengagementpaginatetypedef)
- [ListRotationOverridesRequestListRotationOverridesPaginateTypeDef](./type_defs.md#listrotationoverridesrequestlistrotationoverridespaginatetypedef)
- [ListRotationShiftsRequestListRotationShiftsPaginateTypeDef](./type_defs.md#listrotationshiftsrequestlistrotationshiftspaginatetypedef)
- [ListRotationsRequestListRotationsPaginateTypeDef](./type_defs.md#listrotationsrequestlistrotationspaginatetypedef)
- [ListPageReceiptsResultTypeDef](./type_defs.md#listpagereceiptsresulttypedef)
- [ListPageResolutionsResultTypeDef](./type_defs.md#listpageresolutionsresulttypedef)
- [ListPagesByContactResultTypeDef](./type_defs.md#listpagesbycontactresulttypedef)
- [ListPagesByEngagementResultTypeDef](./type_defs.md#listpagesbyengagementresulttypedef)
- [ListRotationOverridesResultTypeDef](./type_defs.md#listrotationoverridesresulttypedef)
- [RotationShiftTypeDef](./type_defs.md#rotationshifttypedef)
- [ListContactChannelsResultTypeDef](./type_defs.md#listcontactchannelsresulttypedef)
- [StageOutputTypeDef](./type_defs.md#stageoutputtypedef)
- [StageTypeDef](./type_defs.md#stagetypedef)
- [RecurrenceSettingsOutputTypeDef](./type_defs.md#recurrencesettingsoutputtypedef)
- [RecurrenceSettingsTypeDef](./type_defs.md#recurrencesettingstypedef)
- [ListEngagementsRequestListEngagementsPaginateTypeDef](./type_defs.md#listengagementsrequestlistengagementspaginatetypedef)
- [ListEngagementsRequestRequestTypeDef](./type_defs.md#listengagementsrequestrequesttypedef)
- [ListPreviewRotationShiftsResultTypeDef](./type_defs.md#listpreviewrotationshiftsresulttypedef)
- [ListRotationShiftsResultTypeDef](./type_defs.md#listrotationshiftsresulttypedef)
- [PlanOutputTypeDef](./type_defs.md#planoutputtypedef)
- [StageUnionTypeDef](./type_defs.md#stageuniontypedef)
- [GetRotationResultTypeDef](./type_defs.md#getrotationresulttypedef)
- [RotationTypeDef](./type_defs.md#rotationtypedef)
- [CreateRotationRequestRequestTypeDef](./type_defs.md#createrotationrequestrequesttypedef)
- [ListPreviewRotationShiftsRequestListPreviewRotationShiftsPaginateTypeDef](./type_defs.md#listpreviewrotationshiftsrequestlistpreviewrotationshiftspaginatetypedef)
- [ListPreviewRotationShiftsRequestRequestTypeDef](./type_defs.md#listpreviewrotationshiftsrequestrequesttypedef)
- [UpdateRotationRequestRequestTypeDef](./type_defs.md#updaterotationrequestrequesttypedef)
- [GetContactResultTypeDef](./type_defs.md#getcontactresulttypedef)
- [PlanTypeDef](./type_defs.md#plantypedef)
- [ListRotationsResultTypeDef](./type_defs.md#listrotationsresulttypedef)
- [CreateContactRequestRequestTypeDef](./type_defs.md#createcontactrequestrequesttypedef)
- [UpdateContactRequestRequestTypeDef](./type_defs.md#updatecontactrequestrequesttypedef)


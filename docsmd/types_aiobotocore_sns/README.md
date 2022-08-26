# SNS module

> [Index](../README.md) > SNS


!!! note ""

    Auto-generated documentation for [SNS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS)
    type annotations stubs module [types-aiobotocore-sns](https://pypi.org/project/types-aiobotocore-sns/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `SNS` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[sns]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[sns]'


# standalone installation
python -m pip install types-aiobotocore-sns
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-sns
```

## Usage

Code samples can be found in [Examples](./usage.md).

## SNSClient

Type annotations and code completion for  `#!python session.create_client("sns")` as [SNSClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_sns.client import SNSClient


session = get_session()
async with session.create_client("sns") as client:
    client: SNSClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("sns").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_sns.paginator import ListEndpointsByPlatformApplicationPaginator

def get_list_endpoints_by_platform_application_paginator() -> ListEndpointsByPlatformApplicationPaginator:
    return client.get_paginator("list_endpoints_by_platform_application"))
```

- [ListEndpointsByPlatformApplicationPaginator](./paginators.md#listendpointsbyplatformapplicationpaginator)
- [ListOriginationNumbersPaginator](./paginators.md#listoriginationnumberspaginator)
- [ListPhoneNumbersOptedOutPaginator](./paginators.md#listphonenumbersoptedoutpaginator)
- [ListPlatformApplicationsPaginator](./paginators.md#listplatformapplicationspaginator)
- [ListSMSSandboxPhoneNumbersPaginator](./paginators.md#listsmssandboxphonenumberspaginator)
- [ListSubscriptionsPaginator](./paginators.md#listsubscriptionspaginator)
- [ListSubscriptionsByTopicPaginator](./paginators.md#listsubscriptionsbytopicpaginator)
- [ListTopicsPaginator](./paginators.md#listtopicspaginator)






## SNSServiceResource

Type annotations and code completion for `#!python session.resource("sns")` as
[SNSServiceResource](./service_resource.md#snsserviceresource)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#SNS.ServiceResource)

```python title="Usage example"
from types_aiobotocore_sns.service_resource import SNSServiceResource
```


### Collections

Type annotations and code completion for collections
from `#!python session.resource("sns").*`.

```python title="Usage example"
from types_aiobotocore_sns.service_resource import ServiceResourcePlatformApplicationsCollection

def get_collection() -> ServiceResourcePlatformApplicationsCollection:
    return resource.platform_applications
```

- [ServiceResourcePlatformApplicationsCollection](./service_resource.md#snsserviceresourceplatform_applications)
- [ServiceResourceSubscriptionsCollection](./service_resource.md#snsserviceresourcesubscriptions)
- [ServiceResourceTopicsCollection](./service_resource.md#snsserviceresourcetopics)




### Resources

Type annotations and code completion for additional resources
from `#!python session.resource("sns").*`.

```python title="Usage example"
from types_aiobotocore_sns.service_resource import PlatformApplication

def get_resource() -> PlatformApplication:
    return resource.PlatformApplication(...)
```

- [PlatformApplication](./service_resource.md#platformapplication)
- [PlatformEndpoint](./service_resource.md#platformendpoint)
- [Subscription](./service_resource.md#subscription)
- [Topic](./service_resource.md#topic)





## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sns.literals import LanguageCodeStringType

def get_value() -> LanguageCodeStringType:
    return "de-DE"
```

- [LanguageCodeStringType](./literals.md#languagecodestringtype)
- [ListEndpointsByPlatformApplicationPaginatorName](./literals.md#listendpointsbyplatformapplicationpaginatorname)
- [ListOriginationNumbersPaginatorName](./literals.md#listoriginationnumberspaginatorname)
- [ListPhoneNumbersOptedOutPaginatorName](./literals.md#listphonenumbersoptedoutpaginatorname)
- [ListPlatformApplicationsPaginatorName](./literals.md#listplatformapplicationspaginatorname)
- [ListSMSSandboxPhoneNumbersPaginatorName](./literals.md#listsmssandboxphonenumberspaginatorname)
- [ListSubscriptionsByTopicPaginatorName](./literals.md#listsubscriptionsbytopicpaginatorname)
- [ListSubscriptionsPaginatorName](./literals.md#listsubscriptionspaginatorname)
- [ListTopicsPaginatorName](./literals.md#listtopicspaginatorname)
- [NumberCapabilityType](./literals.md#numbercapabilitytype)
- [RouteTypeType](./literals.md#routetypetype)
- [SMSSandboxPhoneNumberVerificationStatusType](./literals.md#smssandboxphonenumberverificationstatustype)
- [SNSServiceName](./literals.md#snsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_sns.type_defs import AddPermissionInputRequestTypeDef

def get_value() -> AddPermissionInputRequestTypeDef:
    return {
        "TopicArn": ...,
        "Label": ...,
        "AWSAccountId": ...,
        "ActionName": ...,
    }
```

- [AddPermissionInputRequestTypeDef](./type_defs.md#addpermissioninputrequesttypedef)
- [AddPermissionInputTopicAddPermissionTypeDef](./type_defs.md#addpermissioninputtopicaddpermissiontypedef)
- [BatchResultErrorEntryTypeDef](./type_defs.md#batchresulterrorentrytypedef)
- [CheckIfPhoneNumberIsOptedOutInputRequestTypeDef](./type_defs.md#checkifphonenumberisoptedoutinputrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ConfirmSubscriptionInputRequestTypeDef](./type_defs.md#confirmsubscriptioninputrequesttypedef)
- [ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef](./type_defs.md#confirmsubscriptioninputtopicconfirmsubscriptiontypedef)
- [CreatePlatformApplicationInputRequestTypeDef](./type_defs.md#createplatformapplicationinputrequesttypedef)
- [CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef](./type_defs.md#createplatformapplicationinputserviceresourcecreateplatformapplicationtypedef)
- [CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef](./type_defs.md#createplatformendpointinputplatformapplicationcreateplatformendpointtypedef)
- [CreatePlatformEndpointInputRequestTypeDef](./type_defs.md#createplatformendpointinputrequesttypedef)
- [CreateSMSSandboxPhoneNumberInputRequestTypeDef](./type_defs.md#createsmssandboxphonenumberinputrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [DeleteEndpointInputRequestTypeDef](./type_defs.md#deleteendpointinputrequesttypedef)
- [DeletePlatformApplicationInputRequestTypeDef](./type_defs.md#deleteplatformapplicationinputrequesttypedef)
- [DeleteSMSSandboxPhoneNumberInputRequestTypeDef](./type_defs.md#deletesmssandboxphonenumberinputrequesttypedef)
- [DeleteTopicInputRequestTypeDef](./type_defs.md#deletetopicinputrequesttypedef)
- [EndpointTypeDef](./type_defs.md#endpointtypedef)
- [GetEndpointAttributesInputRequestTypeDef](./type_defs.md#getendpointattributesinputrequesttypedef)
- [GetPlatformApplicationAttributesInputRequestTypeDef](./type_defs.md#getplatformapplicationattributesinputrequesttypedef)
- [GetSMSAttributesInputRequestTypeDef](./type_defs.md#getsmsattributesinputrequesttypedef)
- [GetSubscriptionAttributesInputRequestTypeDef](./type_defs.md#getsubscriptionattributesinputrequesttypedef)
- [GetTopicAttributesInputRequestTypeDef](./type_defs.md#gettopicattributesinputrequesttypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListEndpointsByPlatformApplicationInputRequestTypeDef](./type_defs.md#listendpointsbyplatformapplicationinputrequesttypedef)
- [ListOriginationNumbersRequestRequestTypeDef](./type_defs.md#listoriginationnumbersrequestrequesttypedef)
- [PhoneNumberInformationTypeDef](./type_defs.md#phonenumberinformationtypedef)
- [ListPhoneNumbersOptedOutInputRequestTypeDef](./type_defs.md#listphonenumbersoptedoutinputrequesttypedef)
- [ListPlatformApplicationsInputRequestTypeDef](./type_defs.md#listplatformapplicationsinputrequesttypedef)
- [PlatformApplicationTypeDef](./type_defs.md#platformapplicationtypedef)
- [ListSMSSandboxPhoneNumbersInputRequestTypeDef](./type_defs.md#listsmssandboxphonenumbersinputrequesttypedef)
- [SMSSandboxPhoneNumberTypeDef](./type_defs.md#smssandboxphonenumbertypedef)
- [ListSubscriptionsByTopicInputRequestTypeDef](./type_defs.md#listsubscriptionsbytopicinputrequesttypedef)
- [SubscriptionTypeDef](./type_defs.md#subscriptiontypedef)
- [ListSubscriptionsInputRequestTypeDef](./type_defs.md#listsubscriptionsinputrequesttypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTopicsInputRequestTypeDef](./type_defs.md#listtopicsinputrequesttypedef)
- [TopicTypeDef](./type_defs.md#topictypedef)
- [MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef)
- [OptInPhoneNumberInputRequestTypeDef](./type_defs.md#optinphonenumberinputrequesttypedef)
- [PublishBatchResultEntryTypeDef](./type_defs.md#publishbatchresultentrytypedef)
- [RemovePermissionInputRequestTypeDef](./type_defs.md#removepermissioninputrequesttypedef)
- [RemovePermissionInputTopicRemovePermissionTypeDef](./type_defs.md#removepermissioninputtopicremovepermissiontypedef)
- [ServiceResourcePlatformApplicationRequestTypeDef](./type_defs.md#serviceresourceplatformapplicationrequesttypedef)
- [ServiceResourcePlatformEndpointRequestTypeDef](./type_defs.md#serviceresourceplatformendpointrequesttypedef)
- [ServiceResourceSubscriptionRequestTypeDef](./type_defs.md#serviceresourcesubscriptionrequesttypedef)
- [ServiceResourceTopicRequestTypeDef](./type_defs.md#serviceresourcetopicrequesttypedef)
- [SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef](./type_defs.md#setendpointattributesinputplatformendpointsetattributestypedef)
- [SetEndpointAttributesInputRequestTypeDef](./type_defs.md#setendpointattributesinputrequesttypedef)
- [SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef](./type_defs.md#setplatformapplicationattributesinputplatformapplicationsetattributestypedef)
- [SetPlatformApplicationAttributesInputRequestTypeDef](./type_defs.md#setplatformapplicationattributesinputrequesttypedef)
- [SetSMSAttributesInputRequestTypeDef](./type_defs.md#setsmsattributesinputrequesttypedef)
- [SetSubscriptionAttributesInputRequestTypeDef](./type_defs.md#setsubscriptionattributesinputrequesttypedef)
- [SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef](./type_defs.md#setsubscriptionattributesinputsubscriptionsetattributestypedef)
- [SetTopicAttributesInputRequestTypeDef](./type_defs.md#settopicattributesinputrequesttypedef)
- [SetTopicAttributesInputTopicSetAttributesTypeDef](./type_defs.md#settopicattributesinputtopicsetattributestypedef)
- [SubscribeInputRequestTypeDef](./type_defs.md#subscribeinputrequesttypedef)
- [SubscribeInputTopicSubscribeTypeDef](./type_defs.md#subscribeinputtopicsubscribetypedef)
- [UnsubscribeInputRequestTypeDef](./type_defs.md#unsubscribeinputrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [VerifySMSSandboxPhoneNumberInputRequestTypeDef](./type_defs.md#verifysmssandboxphonenumberinputrequesttypedef)
- [CheckIfPhoneNumberIsOptedOutResponseTypeDef](./type_defs.md#checkifphonenumberisoptedoutresponsetypedef)
- [ConfirmSubscriptionResponseTypeDef](./type_defs.md#confirmsubscriptionresponsetypedef)
- [CreateEndpointResponseTypeDef](./type_defs.md#createendpointresponsetypedef)
- [CreatePlatformApplicationResponseTypeDef](./type_defs.md#createplatformapplicationresponsetypedef)
- [CreateTopicResponseTypeDef](./type_defs.md#createtopicresponsetypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [GetEndpointAttributesResponseTypeDef](./type_defs.md#getendpointattributesresponsetypedef)
- [GetPlatformApplicationAttributesResponseTypeDef](./type_defs.md#getplatformapplicationattributesresponsetypedef)
- [GetSMSAttributesResponseTypeDef](./type_defs.md#getsmsattributesresponsetypedef)
- [GetSMSSandboxAccountStatusResultTypeDef](./type_defs.md#getsmssandboxaccountstatusresulttypedef)
- [GetSubscriptionAttributesResponseTypeDef](./type_defs.md#getsubscriptionattributesresponsetypedef)
- [GetTopicAttributesResponseTypeDef](./type_defs.md#gettopicattributesresponsetypedef)
- [ListPhoneNumbersOptedOutResponseTypeDef](./type_defs.md#listphonenumbersoptedoutresponsetypedef)
- [PublishResponseTypeDef](./type_defs.md#publishresponsetypedef)
- [SubscribeResponseTypeDef](./type_defs.md#subscriberesponsetypedef)
- [CreateTopicInputRequestTypeDef](./type_defs.md#createtopicinputrequesttypedef)
- [CreateTopicInputServiceResourceCreateTopicTypeDef](./type_defs.md#createtopicinputserviceresourcecreatetopictypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ListEndpointsByPlatformApplicationResponseTypeDef](./type_defs.md#listendpointsbyplatformapplicationresponsetypedef)
- [ListEndpointsByPlatformApplicationInputListEndpointsByPlatformApplicationPaginateTypeDef](./type_defs.md#listendpointsbyplatformapplicationinputlistendpointsbyplatformapplicationpaginatetypedef)
- [ListOriginationNumbersRequestListOriginationNumbersPaginateTypeDef](./type_defs.md#listoriginationnumbersrequestlistoriginationnumberspaginatetypedef)
- [ListPhoneNumbersOptedOutInputListPhoneNumbersOptedOutPaginateTypeDef](./type_defs.md#listphonenumbersoptedoutinputlistphonenumbersoptedoutpaginatetypedef)
- [ListPlatformApplicationsInputListPlatformApplicationsPaginateTypeDef](./type_defs.md#listplatformapplicationsinputlistplatformapplicationspaginatetypedef)
- [ListSMSSandboxPhoneNumbersInputListSMSSandboxPhoneNumbersPaginateTypeDef](./type_defs.md#listsmssandboxphonenumbersinputlistsmssandboxphonenumberspaginatetypedef)
- [ListSubscriptionsByTopicInputListSubscriptionsByTopicPaginateTypeDef](./type_defs.md#listsubscriptionsbytopicinputlistsubscriptionsbytopicpaginatetypedef)
- [ListSubscriptionsInputListSubscriptionsPaginateTypeDef](./type_defs.md#listsubscriptionsinputlistsubscriptionspaginatetypedef)
- [ListTopicsInputListTopicsPaginateTypeDef](./type_defs.md#listtopicsinputlisttopicspaginatetypedef)
- [ListOriginationNumbersResultTypeDef](./type_defs.md#listoriginationnumbersresulttypedef)
- [ListPlatformApplicationsResponseTypeDef](./type_defs.md#listplatformapplicationsresponsetypedef)
- [ListSMSSandboxPhoneNumbersResultTypeDef](./type_defs.md#listsmssandboxphonenumbersresulttypedef)
- [ListSubscriptionsByTopicResponseTypeDef](./type_defs.md#listsubscriptionsbytopicresponsetypedef)
- [ListSubscriptionsResponseTypeDef](./type_defs.md#listsubscriptionsresponsetypedef)
- [ListTopicsResponseTypeDef](./type_defs.md#listtopicsresponsetypedef)
- [PublishBatchRequestEntryTypeDef](./type_defs.md#publishbatchrequestentrytypedef)
- [PublishInputPlatformEndpointPublishTypeDef](./type_defs.md#publishinputplatformendpointpublishtypedef)
- [PublishInputRequestTypeDef](./type_defs.md#publishinputrequesttypedef)
- [PublishInputTopicPublishTypeDef](./type_defs.md#publishinputtopicpublishtypedef)
- [PublishBatchResponseTypeDef](./type_defs.md#publishbatchresponsetypedef)
- [PublishBatchInputRequestTypeDef](./type_defs.md#publishbatchinputrequesttypedef)


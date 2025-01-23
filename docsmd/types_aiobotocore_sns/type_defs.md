# Type definitions

> [Index](../README.md) > [SNS](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [SNS](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sns.html#sns)
    type annotations stubs module [types-aiobotocore-sns](https://pypi.org/project/types-aiobotocore-sns/).

## BlobTypeDef

```python
# BlobTypeDef definition

BlobTypeDef = Union[
    str,
    bytes,
    IO[Any],
    StreamingBody,
]
```




## AddPermissionInputRequestTypeDef

```python
# AddPermissionInputRequestTypeDef definition

class AddPermissionInputRequestTypeDef(TypedDict):
    TopicArn: str,
    Label: str,
    AWSAccountId: Sequence[str],
    ActionName: Sequence[str],
```

## AddPermissionInputTopicAddPermissionTypeDef

```python
# AddPermissionInputTopicAddPermissionTypeDef definition

class AddPermissionInputTopicAddPermissionTypeDef(TypedDict):
    Label: str,
    AWSAccountId: Sequence[str],
    ActionName: Sequence[str],
```

## BatchResultErrorEntryTypeDef

```python
# BatchResultErrorEntryTypeDef definition

class BatchResultErrorEntryTypeDef(TypedDict):
    Id: str,
    Code: str,
    SenderFault: bool,
    Message: NotRequired[str],
```

## CheckIfPhoneNumberIsOptedOutInputRequestTypeDef

```python
# CheckIfPhoneNumberIsOptedOutInputRequestTypeDef definition

class CheckIfPhoneNumberIsOptedOutInputRequestTypeDef(TypedDict):
    phoneNumber: str,
```

## ResponseMetadataTypeDef

```python
# ResponseMetadataTypeDef definition

class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
    HostId: NotRequired[str],
```

## ConfirmSubscriptionInputRequestTypeDef

```python
# ConfirmSubscriptionInputRequestTypeDef definition

class ConfirmSubscriptionInputRequestTypeDef(TypedDict):
    TopicArn: str,
    Token: str,
    AuthenticateOnUnsubscribe: NotRequired[str],
```

## ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef

```python
# ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef definition

class ConfirmSubscriptionInputTopicConfirmSubscriptionTypeDef(TypedDict):
    Token: str,
    AuthenticateOnUnsubscribe: NotRequired[str],
```

## CreatePlatformApplicationInputRequestTypeDef

```python
# CreatePlatformApplicationInputRequestTypeDef definition

class CreatePlatformApplicationInputRequestTypeDef(TypedDict):
    Name: str,
    Platform: str,
    Attributes: Mapping[str, str],
```

## CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef

```python
# CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef definition

class CreatePlatformApplicationInputServiceResourceCreatePlatformApplicationTypeDef(TypedDict):
    Name: str,
    Platform: str,
    Attributes: Mapping[str, str],
```

## CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef

```python
# CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef definition

class CreatePlatformEndpointInputPlatformApplicationCreatePlatformEndpointTypeDef(TypedDict):
    Token: str,
    CustomUserData: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
```

## CreatePlatformEndpointInputRequestTypeDef

```python
# CreatePlatformEndpointInputRequestTypeDef definition

class CreatePlatformEndpointInputRequestTypeDef(TypedDict):
    PlatformApplicationArn: str,
    Token: str,
    CustomUserData: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
```

## CreateSMSSandboxPhoneNumberInputRequestTypeDef

```python
# CreateSMSSandboxPhoneNumberInputRequestTypeDef definition

class CreateSMSSandboxPhoneNumberInputRequestTypeDef(TypedDict):
    PhoneNumber: str,
    LanguageCode: NotRequired[LanguageCodeStringType],  # (1)
```

1. See [:material-code-brackets: LanguageCodeStringType](./literals.md#languagecodestringtype) 
## TagTypeDef

```python
# TagTypeDef definition

class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## DeleteEndpointInputRequestTypeDef

```python
# DeleteEndpointInputRequestTypeDef definition

class DeleteEndpointInputRequestTypeDef(TypedDict):
    EndpointArn: str,
```

## DeletePlatformApplicationInputRequestTypeDef

```python
# DeletePlatformApplicationInputRequestTypeDef definition

class DeletePlatformApplicationInputRequestTypeDef(TypedDict):
    PlatformApplicationArn: str,
```

## DeleteSMSSandboxPhoneNumberInputRequestTypeDef

```python
# DeleteSMSSandboxPhoneNumberInputRequestTypeDef definition

class DeleteSMSSandboxPhoneNumberInputRequestTypeDef(TypedDict):
    PhoneNumber: str,
```

## DeleteTopicInputRequestTypeDef

```python
# DeleteTopicInputRequestTypeDef definition

class DeleteTopicInputRequestTypeDef(TypedDict):
    TopicArn: str,
```

## EndpointTypeDef

```python
# EndpointTypeDef definition

class EndpointTypeDef(TypedDict):
    EndpointArn: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
```

## GetDataProtectionPolicyInputRequestTypeDef

```python
# GetDataProtectionPolicyInputRequestTypeDef definition

class GetDataProtectionPolicyInputRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## GetEndpointAttributesInputRequestTypeDef

```python
# GetEndpointAttributesInputRequestTypeDef definition

class GetEndpointAttributesInputRequestTypeDef(TypedDict):
    EndpointArn: str,
```

## GetPlatformApplicationAttributesInputRequestTypeDef

```python
# GetPlatformApplicationAttributesInputRequestTypeDef definition

class GetPlatformApplicationAttributesInputRequestTypeDef(TypedDict):
    PlatformApplicationArn: str,
```

## GetSMSAttributesInputRequestTypeDef

```python
# GetSMSAttributesInputRequestTypeDef definition

class GetSMSAttributesInputRequestTypeDef(TypedDict):
    attributes: NotRequired[Sequence[str]],
```

## GetSubscriptionAttributesInputRequestTypeDef

```python
# GetSubscriptionAttributesInputRequestTypeDef definition

class GetSubscriptionAttributesInputRequestTypeDef(TypedDict):
    SubscriptionArn: str,
```

## GetTopicAttributesInputRequestTypeDef

```python
# GetTopicAttributesInputRequestTypeDef definition

class GetTopicAttributesInputRequestTypeDef(TypedDict):
    TopicArn: str,
```

## PaginatorConfigTypeDef

```python
# PaginatorConfigTypeDef definition

class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ListEndpointsByPlatformApplicationInputRequestTypeDef

```python
# ListEndpointsByPlatformApplicationInputRequestTypeDef definition

class ListEndpointsByPlatformApplicationInputRequestTypeDef(TypedDict):
    PlatformApplicationArn: str,
    NextToken: NotRequired[str],
```

## ListOriginationNumbersRequestRequestTypeDef

```python
# ListOriginationNumbersRequestRequestTypeDef definition

class ListOriginationNumbersRequestRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## PhoneNumberInformationTypeDef

```python
# PhoneNumberInformationTypeDef definition

class PhoneNumberInformationTypeDef(TypedDict):
    CreatedAt: NotRequired[datetime],
    PhoneNumber: NotRequired[str],
    Status: NotRequired[str],
    Iso2CountryCode: NotRequired[str],
    RouteType: NotRequired[RouteTypeType],  # (1)
    NumberCapabilities: NotRequired[List[NumberCapabilityType]],  # (2)
```

1. See [:material-code-brackets: RouteTypeType](./literals.md#routetypetype) 
2. See [:material-code-brackets: NumberCapabilityType](./literals.md#numbercapabilitytype) 
## ListPhoneNumbersOptedOutInputRequestTypeDef

```python
# ListPhoneNumbersOptedOutInputRequestTypeDef definition

class ListPhoneNumbersOptedOutInputRequestTypeDef(TypedDict):
    nextToken: NotRequired[str],
```

## ListPlatformApplicationsInputRequestTypeDef

```python
# ListPlatformApplicationsInputRequestTypeDef definition

class ListPlatformApplicationsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## PlatformApplicationTypeDef

```python
# PlatformApplicationTypeDef definition

class PlatformApplicationTypeDef(TypedDict):
    PlatformApplicationArn: NotRequired[str],
    Attributes: NotRequired[Dict[str, str]],
```

## ListSMSSandboxPhoneNumbersInputRequestTypeDef

```python
# ListSMSSandboxPhoneNumbersInputRequestTypeDef definition

class ListSMSSandboxPhoneNumbersInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## SMSSandboxPhoneNumberTypeDef

```python
# SMSSandboxPhoneNumberTypeDef definition

class SMSSandboxPhoneNumberTypeDef(TypedDict):
    PhoneNumber: NotRequired[str],
    Status: NotRequired[SMSSandboxPhoneNumberVerificationStatusType],  # (1)
```

1. See [:material-code-brackets: SMSSandboxPhoneNumberVerificationStatusType](./literals.md#smssandboxphonenumberverificationstatustype) 
## ListSubscriptionsByTopicInputRequestTypeDef

```python
# ListSubscriptionsByTopicInputRequestTypeDef definition

class ListSubscriptionsByTopicInputRequestTypeDef(TypedDict):
    TopicArn: str,
    NextToken: NotRequired[str],
```

## SubscriptionTypeDef

```python
# SubscriptionTypeDef definition

class SubscriptionTypeDef(TypedDict):
    SubscriptionArn: NotRequired[str],
    Owner: NotRequired[str],
    Protocol: NotRequired[str],
    Endpoint: NotRequired[str],
    TopicArn: NotRequired[str],
```

## ListSubscriptionsInputRequestTypeDef

```python
# ListSubscriptionsInputRequestTypeDef definition

class ListSubscriptionsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## ListTagsForResourceRequestRequestTypeDef

```python
# ListTagsForResourceRequestRequestTypeDef definition

class ListTagsForResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
```

## ListTopicsInputRequestTypeDef

```python
# ListTopicsInputRequestTypeDef definition

class ListTopicsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
```

## TopicTypeDef

```python
# TopicTypeDef definition

class TopicTypeDef(TypedDict):
    TopicArn: NotRequired[str],
```

## OptInPhoneNumberInputRequestTypeDef

```python
# OptInPhoneNumberInputRequestTypeDef definition

class OptInPhoneNumberInputRequestTypeDef(TypedDict):
    phoneNumber: str,
```

## PublishBatchResultEntryTypeDef

```python
# PublishBatchResultEntryTypeDef definition

class PublishBatchResultEntryTypeDef(TypedDict):
    Id: NotRequired[str],
    MessageId: NotRequired[str],
    SequenceNumber: NotRequired[str],
```

## PutDataProtectionPolicyInputRequestTypeDef

```python
# PutDataProtectionPolicyInputRequestTypeDef definition

class PutDataProtectionPolicyInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    DataProtectionPolicy: str,
```

## RemovePermissionInputRequestTypeDef

```python
# RemovePermissionInputRequestTypeDef definition

class RemovePermissionInputRequestTypeDef(TypedDict):
    TopicArn: str,
    Label: str,
```

## RemovePermissionInputTopicRemovePermissionTypeDef

```python
# RemovePermissionInputTopicRemovePermissionTypeDef definition

class RemovePermissionInputTopicRemovePermissionTypeDef(TypedDict):
    Label: str,
```

## SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef

```python
# SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef definition

class SetEndpointAttributesInputPlatformEndpointSetAttributesTypeDef(TypedDict):
    Attributes: Mapping[str, str],
```

## SetEndpointAttributesInputRequestTypeDef

```python
# SetEndpointAttributesInputRequestTypeDef definition

class SetEndpointAttributesInputRequestTypeDef(TypedDict):
    EndpointArn: str,
    Attributes: Mapping[str, str],
```

## SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef

```python
# SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef definition

class SetPlatformApplicationAttributesInputPlatformApplicationSetAttributesTypeDef(TypedDict):
    Attributes: Mapping[str, str],
```

## SetPlatformApplicationAttributesInputRequestTypeDef

```python
# SetPlatformApplicationAttributesInputRequestTypeDef definition

class SetPlatformApplicationAttributesInputRequestTypeDef(TypedDict):
    PlatformApplicationArn: str,
    Attributes: Mapping[str, str],
```

## SetSMSAttributesInputRequestTypeDef

```python
# SetSMSAttributesInputRequestTypeDef definition

class SetSMSAttributesInputRequestTypeDef(TypedDict):
    attributes: Mapping[str, str],
```

## SetSubscriptionAttributesInputRequestTypeDef

```python
# SetSubscriptionAttributesInputRequestTypeDef definition

class SetSubscriptionAttributesInputRequestTypeDef(TypedDict):
    SubscriptionArn: str,
    AttributeName: str,
    AttributeValue: NotRequired[str],
```

## SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef

```python
# SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef definition

class SetSubscriptionAttributesInputSubscriptionSetAttributesTypeDef(TypedDict):
    AttributeName: str,
    AttributeValue: NotRequired[str],
```

## SetTopicAttributesInputRequestTypeDef

```python
# SetTopicAttributesInputRequestTypeDef definition

class SetTopicAttributesInputRequestTypeDef(TypedDict):
    TopicArn: str,
    AttributeName: str,
    AttributeValue: NotRequired[str],
```

## SetTopicAttributesInputTopicSetAttributesTypeDef

```python
# SetTopicAttributesInputTopicSetAttributesTypeDef definition

class SetTopicAttributesInputTopicSetAttributesTypeDef(TypedDict):
    AttributeName: str,
    AttributeValue: NotRequired[str],
```

## SubscribeInputRequestTypeDef

```python
# SubscribeInputRequestTypeDef definition

class SubscribeInputRequestTypeDef(TypedDict):
    TopicArn: str,
    Protocol: str,
    Endpoint: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    ReturnSubscriptionArn: NotRequired[bool],
```

## SubscribeInputTopicSubscribeTypeDef

```python
# SubscribeInputTopicSubscribeTypeDef definition

class SubscribeInputTopicSubscribeTypeDef(TypedDict):
    Protocol: str,
    Endpoint: NotRequired[str],
    Attributes: NotRequired[Mapping[str, str]],
    ReturnSubscriptionArn: NotRequired[bool],
```

## UnsubscribeInputRequestTypeDef

```python
# UnsubscribeInputRequestTypeDef definition

class UnsubscribeInputRequestTypeDef(TypedDict):
    SubscriptionArn: str,
```

## UntagResourceRequestRequestTypeDef

```python
# UntagResourceRequestRequestTypeDef definition

class UntagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## VerifySMSSandboxPhoneNumberInputRequestTypeDef

```python
# VerifySMSSandboxPhoneNumberInputRequestTypeDef definition

class VerifySMSSandboxPhoneNumberInputRequestTypeDef(TypedDict):
    PhoneNumber: str,
    OneTimePassword: str,
```

## MessageAttributeValueTypeDef

```python
# MessageAttributeValueTypeDef definition

class MessageAttributeValueTypeDef(TypedDict):
    DataType: str,
    StringValue: NotRequired[str],
    BinaryValue: NotRequired[BlobTypeDef],
```

## CheckIfPhoneNumberIsOptedOutResponseTypeDef

```python
# CheckIfPhoneNumberIsOptedOutResponseTypeDef definition

class CheckIfPhoneNumberIsOptedOutResponseTypeDef(TypedDict):
    isOptedOut: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ConfirmSubscriptionResponseTypeDef

```python
# ConfirmSubscriptionResponseTypeDef definition

class ConfirmSubscriptionResponseTypeDef(TypedDict):
    SubscriptionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateEndpointResponseTypeDef

```python
# CreateEndpointResponseTypeDef definition

class CreateEndpointResponseTypeDef(TypedDict):
    EndpointArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePlatformApplicationResponseTypeDef

```python
# CreatePlatformApplicationResponseTypeDef definition

class CreatePlatformApplicationResponseTypeDef(TypedDict):
    PlatformApplicationArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTopicResponseTypeDef

```python
# CreateTopicResponseTypeDef definition

class CreateTopicResponseTypeDef(TypedDict):
    TopicArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EmptyResponseMetadataTypeDef

```python
# EmptyResponseMetadataTypeDef definition

class EmptyResponseMetadataTypeDef(TypedDict):
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDataProtectionPolicyResponseTypeDef

```python
# GetDataProtectionPolicyResponseTypeDef definition

class GetDataProtectionPolicyResponseTypeDef(TypedDict):
    DataProtectionPolicy: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetEndpointAttributesResponseTypeDef

```python
# GetEndpointAttributesResponseTypeDef definition

class GetEndpointAttributesResponseTypeDef(TypedDict):
    Attributes: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPlatformApplicationAttributesResponseTypeDef

```python
# GetPlatformApplicationAttributesResponseTypeDef definition

class GetPlatformApplicationAttributesResponseTypeDef(TypedDict):
    Attributes: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSMSAttributesResponseTypeDef

```python
# GetSMSAttributesResponseTypeDef definition

class GetSMSAttributesResponseTypeDef(TypedDict):
    attributes: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSMSSandboxAccountStatusResultTypeDef

```python
# GetSMSSandboxAccountStatusResultTypeDef definition

class GetSMSSandboxAccountStatusResultTypeDef(TypedDict):
    IsInSandbox: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetSubscriptionAttributesResponseTypeDef

```python
# GetSubscriptionAttributesResponseTypeDef definition

class GetSubscriptionAttributesResponseTypeDef(TypedDict):
    Attributes: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTopicAttributesResponseTypeDef

```python
# GetTopicAttributesResponseTypeDef definition

class GetTopicAttributesResponseTypeDef(TypedDict):
    Attributes: Dict[str, str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPhoneNumbersOptedOutResponseTypeDef

```python
# ListPhoneNumbersOptedOutResponseTypeDef definition

class ListPhoneNumbersOptedOutResponseTypeDef(TypedDict):
    phoneNumbers: List[str],
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
    nextToken: NotRequired[str],
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishResponseTypeDef

```python
# PublishResponseTypeDef definition

class PublishResponseTypeDef(TypedDict):
    MessageId: str,
    SequenceNumber: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SubscribeResponseTypeDef

```python
# SubscribeResponseTypeDef definition

class SubscribeResponseTypeDef(TypedDict):
    SubscriptionArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateTopicInputRequestTypeDef

```python
# CreateTopicInputRequestTypeDef definition

class CreateTopicInputRequestTypeDef(TypedDict):
    Name: str,
    Attributes: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DataProtectionPolicy: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateTopicInputServiceResourceCreateTopicTypeDef

```python
# CreateTopicInputServiceResourceCreateTopicTypeDef definition

class CreateTopicInputServiceResourceCreateTopicTypeDef(TypedDict):
    Name: str,
    Attributes: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (1)
    DataProtectionPolicy: NotRequired[str],
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListTagsForResourceResponseTypeDef

```python
# ListTagsForResourceResponseTypeDef definition

class ListTagsForResourceResponseTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TagResourceRequestRequestTypeDef

```python
# TagResourceRequestRequestTypeDef definition

class TagResourceRequestRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## ListEndpointsByPlatformApplicationResponseTypeDef

```python
# ListEndpointsByPlatformApplicationResponseTypeDef definition

class ListEndpointsByPlatformApplicationResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEndpointsByPlatformApplicationInputPaginateTypeDef

```python
# ListEndpointsByPlatformApplicationInputPaginateTypeDef definition

class ListEndpointsByPlatformApplicationInputPaginateTypeDef(TypedDict):
    PlatformApplicationArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOriginationNumbersRequestPaginateTypeDef

```python
# ListOriginationNumbersRequestPaginateTypeDef definition

class ListOriginationNumbersRequestPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPhoneNumbersOptedOutInputPaginateTypeDef

```python
# ListPhoneNumbersOptedOutInputPaginateTypeDef definition

class ListPhoneNumbersOptedOutInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListPlatformApplicationsInputPaginateTypeDef

```python
# ListPlatformApplicationsInputPaginateTypeDef definition

class ListPlatformApplicationsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSMSSandboxPhoneNumbersInputPaginateTypeDef

```python
# ListSMSSandboxPhoneNumbersInputPaginateTypeDef definition

class ListSMSSandboxPhoneNumbersInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionsByTopicInputPaginateTypeDef

```python
# ListSubscriptionsByTopicInputPaginateTypeDef definition

class ListSubscriptionsByTopicInputPaginateTypeDef(TypedDict):
    TopicArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListSubscriptionsInputPaginateTypeDef

```python
# ListSubscriptionsInputPaginateTypeDef definition

class ListSubscriptionsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTopicsInputPaginateTypeDef

```python
# ListTopicsInputPaginateTypeDef definition

class ListTopicsInputPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListOriginationNumbersResultTypeDef

```python
# ListOriginationNumbersResultTypeDef definition

class ListOriginationNumbersResultTypeDef(TypedDict):
    PhoneNumbers: List[PhoneNumberInformationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PhoneNumberInformationTypeDef](./type_defs.md#phonenumberinformationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPlatformApplicationsResponseTypeDef

```python
# ListPlatformApplicationsResponseTypeDef definition

class ListPlatformApplicationsResponseTypeDef(TypedDict):
    PlatformApplications: List[PlatformApplicationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: PlatformApplicationTypeDef](./type_defs.md#platformapplicationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSMSSandboxPhoneNumbersResultTypeDef

```python
# ListSMSSandboxPhoneNumbersResultTypeDef definition

class ListSMSSandboxPhoneNumbersResultTypeDef(TypedDict):
    PhoneNumbers: List[SMSSandboxPhoneNumberTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SMSSandboxPhoneNumberTypeDef](./type_defs.md#smssandboxphonenumbertypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscriptionsByTopicResponseTypeDef

```python
# ListSubscriptionsByTopicResponseTypeDef definition

class ListSubscriptionsByTopicResponseTypeDef(TypedDict):
    Subscriptions: List[SubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListSubscriptionsResponseTypeDef

```python
# ListSubscriptionsResponseTypeDef definition

class ListSubscriptionsResponseTypeDef(TypedDict):
    Subscriptions: List[SubscriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: SubscriptionTypeDef](./type_defs.md#subscriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTopicsResponseTypeDef

```python
# ListTopicsResponseTypeDef definition

class ListTopicsResponseTypeDef(TypedDict):
    Topics: List[TopicTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
    NextToken: NotRequired[str],
```

1. See [:material-code-braces: TopicTypeDef](./type_defs.md#topictypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishBatchResponseTypeDef

```python
# PublishBatchResponseTypeDef definition

class PublishBatchResponseTypeDef(TypedDict):
    Successful: List[PublishBatchResultEntryTypeDef],  # (1)
    Failed: List[BatchResultErrorEntryTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: PublishBatchResultEntryTypeDef](./type_defs.md#publishbatchresultentrytypedef) 
2. See [:material-code-braces: BatchResultErrorEntryTypeDef](./type_defs.md#batchresulterrorentrytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PublishBatchRequestEntryTypeDef

```python
# PublishBatchRequestEntryTypeDef definition

class PublishBatchRequestEntryTypeDef(TypedDict):
    Id: str,
    Message: str,
    Subject: NotRequired[str],
    MessageStructure: NotRequired[str],
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueTypeDef]],  # (1)
    MessageDeduplicationId: NotRequired[str],
    MessageGroupId: NotRequired[str],
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
## PublishInputPlatformEndpointPublishTypeDef

```python
# PublishInputPlatformEndpointPublishTypeDef definition

class PublishInputPlatformEndpointPublishTypeDef(TypedDict):
    Message: str,
    TopicArn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    Subject: NotRequired[str],
    MessageStructure: NotRequired[str],
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueTypeDef]],  # (1)
    MessageDeduplicationId: NotRequired[str],
    MessageGroupId: NotRequired[str],
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
## PublishInputRequestTypeDef

```python
# PublishInputRequestTypeDef definition

class PublishInputRequestTypeDef(TypedDict):
    Message: str,
    TopicArn: NotRequired[str],
    TargetArn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    Subject: NotRequired[str],
    MessageStructure: NotRequired[str],
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueTypeDef]],  # (1)
    MessageDeduplicationId: NotRequired[str],
    MessageGroupId: NotRequired[str],
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
## PublishInputTopicPublishTypeDef

```python
# PublishInputTopicPublishTypeDef definition

class PublishInputTopicPublishTypeDef(TypedDict):
    Message: str,
    TargetArn: NotRequired[str],
    PhoneNumber: NotRequired[str],
    Subject: NotRequired[str],
    MessageStructure: NotRequired[str],
    MessageAttributes: NotRequired[Mapping[str, MessageAttributeValueTypeDef]],  # (1)
    MessageDeduplicationId: NotRequired[str],
    MessageGroupId: NotRequired[str],
```

1. See [:material-code-braces: MessageAttributeValueTypeDef](./type_defs.md#messageattributevaluetypedef) 
## PublishBatchInputRequestTypeDef

```python
# PublishBatchInputRequestTypeDef definition

class PublishBatchInputRequestTypeDef(TypedDict):
    TopicArn: str,
    PublishBatchRequestEntries: Sequence[PublishBatchRequestEntryTypeDef],  # (1)
```

1. See [:material-code-braces: PublishBatchRequestEntryTypeDef](./type_defs.md#publishbatchrequestentrytypedef) 

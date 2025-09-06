# Paginators

> [Index](../README.md) > [PinpointSMSVoiceV2](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [PinpointSMSVoiceV2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2.html#pinpointsmsvoicev2)
    type annotations stubs module [types-aiobotocore-pinpoint-sms-voice-v2](https://pypi.org/project/types-aiobotocore-pinpoint-sms-voice-v2/).

## DescribeAccountAttributesPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_account_attributes")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeAccountAttributes.html#PinpointSMSVoiceV2.Paginator.DescribeAccountAttributes)

```python
# DescribeAccountAttributesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeAccountAttributesPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeAccountAttributesPaginator = client.get_paginator("describe_account_attributes")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccountAttributesResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeAccountAttributesPaginator](./paginators.md#describeaccountattributespaginator)
3. item: `AioPageIterator[DescribeAccountAttributesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeAccountAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeAccountAttributesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeAccountAttributesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAccountAttributesRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountAttributesRequestPaginateTypeDef](./type_defs.md#describeaccountattributesrequestpaginatetypedef)
## DescribeAccountLimitsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_account_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeAccountLimits.html#PinpointSMSVoiceV2.Paginator.DescribeAccountLimits)

```python
# DescribeAccountLimitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeAccountLimitsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeAccountLimitsPaginator = client.get_paginator("describe_account_limits")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAccountLimitsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeAccountLimitsPaginator](./paginators.md#describeaccountlimitspaginator)
3. item: `AioPageIterator[DescribeAccountLimitsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeAccountLimitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeAccountLimitsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeAccountLimitsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAccountLimitsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountLimitsRequestPaginateTypeDef](./type_defs.md#describeaccountlimitsrequestpaginatetypedef)
## DescribeConfigurationSetsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_configuration_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeConfigurationSets.html#PinpointSMSVoiceV2.Paginator.DescribeConfigurationSets)

```python
# DescribeConfigurationSetsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeConfigurationSetsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeConfigurationSetsPaginator = client.get_paginator("describe_configuration_sets")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigurationSetsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeConfigurationSetsPaginator](./paginators.md#describeconfigurationsetspaginator)
3. item: `AioPageIterator[DescribeConfigurationSetsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeConfigurationSetsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigurationSetNames: Sequence[str] = ...,
    Filters: Sequence[ConfigurationSetFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeConfigurationSetsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[ConfigurationSetFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeConfigurationSetsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConfigurationSetsRequestPaginateTypeDef = {  # (1)
    "ConfigurationSetNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationSetsRequestPaginateTypeDef](./type_defs.md#describeconfigurationsetsrequestpaginatetypedef)
## DescribeKeywordsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_keywords")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeKeywords.html#PinpointSMSVoiceV2.Paginator.DescribeKeywords)

```python
# DescribeKeywordsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeKeywordsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeKeywordsPaginator = client.get_paginator("describe_keywords")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeKeywordsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeKeywordsPaginator](./paginators.md#describekeywordspaginator)
3. item: `AioPageIterator[DescribeKeywordsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeKeywordsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OriginationIdentity: str,
    Keywords: Sequence[str] = ...,
    Filters: Sequence[KeywordFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeKeywordsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[KeywordFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeKeywordsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeKeywordsRequestPaginateTypeDef = {  # (1)
    "OriginationIdentity": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeKeywordsRequestPaginateTypeDef](./type_defs.md#describekeywordsrequestpaginatetypedef)
## DescribeOptOutListsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_opt_out_lists")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeOptOutLists.html#PinpointSMSVoiceV2.Paginator.DescribeOptOutLists)

```python
# DescribeOptOutListsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeOptOutListsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeOptOutListsPaginator = client.get_paginator("describe_opt_out_lists")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOptOutListsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeOptOutListsPaginator](./paginators.md#describeoptoutlistspaginator)
3. item: `AioPageIterator[DescribeOptOutListsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeOptOutListsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OptOutListNames: Sequence[str] = ...,
    Owner: OwnerType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeOptOutListsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OwnerType](./literals.md#ownertype)
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeOptOutListsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOptOutListsRequestPaginateTypeDef = {  # (1)
    "OptOutListNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOptOutListsRequestPaginateTypeDef](./type_defs.md#describeoptoutlistsrequestpaginatetypedef)
## DescribeOptedOutNumbersPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_opted_out_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeOptedOutNumbers.html#PinpointSMSVoiceV2.Paginator.DescribeOptedOutNumbers)

```python
# DescribeOptedOutNumbersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeOptedOutNumbersPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeOptedOutNumbersPaginator = client.get_paginator("describe_opted_out_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOptedOutNumbersResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeOptedOutNumbersPaginator](./paginators.md#describeoptedoutnumberspaginator)
3. item: `AioPageIterator[DescribeOptedOutNumbersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeOptedOutNumbersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OptOutListName: str,
    OptedOutNumbers: Sequence[str] = ...,
    Filters: Sequence[OptedOutFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeOptedOutNumbersResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[OptedOutFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeOptedOutNumbersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOptedOutNumbersRequestPaginateTypeDef = {  # (1)
    "OptOutListName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOptedOutNumbersRequestPaginateTypeDef](./type_defs.md#describeoptedoutnumbersrequestpaginatetypedef)
## DescribePhoneNumbersPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_phone_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribePhoneNumbers.html#PinpointSMSVoiceV2.Paginator.DescribePhoneNumbers)

```python
# DescribePhoneNumbersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribePhoneNumbersPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribePhoneNumbersPaginator = client.get_paginator("describe_phone_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePhoneNumbersResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribePhoneNumbersPaginator](./paginators.md#describephonenumberspaginator)
3. item: `AioPageIterator[DescribePhoneNumbersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribePhoneNumbersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PhoneNumberIds: Sequence[str] = ...,
    Filters: Sequence[PhoneNumberFilterTypeDef] = ...,  # (1)
    Owner: OwnerType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribePhoneNumbersResultTypeDef]:  # (4)
    ...
```

1. See `Sequence[PhoneNumberFilterTypeDef]`
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribePhoneNumbersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribePhoneNumbersRequestPaginateTypeDef = {  # (1)
    "PhoneNumberIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePhoneNumbersRequestPaginateTypeDef](./type_defs.md#describephonenumbersrequestpaginatetypedef)
## DescribePoolsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_pools")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribePools.html#PinpointSMSVoiceV2.Paginator.DescribePools)

```python
# DescribePoolsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribePoolsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribePoolsPaginator = client.get_paginator("describe_pools")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePoolsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribePoolsPaginator](./paginators.md#describepoolspaginator)
3. item: `AioPageIterator[DescribePoolsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribePoolsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PoolIds: Sequence[str] = ...,
    Filters: Sequence[PoolFilterTypeDef] = ...,  # (1)
    Owner: OwnerType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> aiobotocore.paginate.AioPageIterator[DescribePoolsResultTypeDef]:  # (4)
    ...
```

1. See `Sequence[PoolFilterTypeDef]`
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype)
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
4. See `AioPageIterator[DescribePoolsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribePoolsRequestPaginateTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePoolsRequestPaginateTypeDef](./type_defs.md#describepoolsrequestpaginatetypedef)
## DescribeProtectConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_protect_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeProtectConfigurations.html#PinpointSMSVoiceV2.Paginator.DescribeProtectConfigurations)

```python
# DescribeProtectConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeProtectConfigurationsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeProtectConfigurationsPaginator = client.get_paginator("describe_protect_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeProtectConfigurationsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeProtectConfigurationsPaginator](./paginators.md#describeprotectconfigurationspaginator)
3. item: `AioPageIterator[DescribeProtectConfigurationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeProtectConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProtectConfigurationIds: Sequence[str] = ...,
    Filters: Sequence[ProtectConfigurationFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeProtectConfigurationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[ProtectConfigurationFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeProtectConfigurationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeProtectConfigurationsRequestPaginateTypeDef = {  # (1)
    "ProtectConfigurationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeProtectConfigurationsRequestPaginateTypeDef](./type_defs.md#describeprotectconfigurationsrequestpaginatetypedef)
## DescribeRegistrationAttachmentsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_registration_attachments")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeRegistrationAttachments.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationAttachments)

```python
# DescribeRegistrationAttachmentsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeRegistrationAttachmentsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeRegistrationAttachmentsPaginator = client.get_paginator("describe_registration_attachments")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistrationAttachmentsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeRegistrationAttachmentsPaginator](./paginators.md#describeregistrationattachmentspaginator)
3. item: `AioPageIterator[DescribeRegistrationAttachmentsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRegistrationAttachmentsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistrationAttachmentIds: Sequence[str] = ...,
    Filters: Sequence[RegistrationAttachmentFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeRegistrationAttachmentsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[RegistrationAttachmentFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeRegistrationAttachmentsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationAttachmentsRequestPaginateTypeDef = {  # (1)
    "RegistrationAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationAttachmentsRequestPaginateTypeDef](./type_defs.md#describeregistrationattachmentsrequestpaginatetypedef)
## DescribeRegistrationFieldDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_registration_field_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeRegistrationFieldDefinitions.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldDefinitions)

```python
# DescribeRegistrationFieldDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeRegistrationFieldDefinitionsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeRegistrationFieldDefinitionsPaginator = client.get_paginator("describe_registration_field_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistrationFieldDefinitionsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeRegistrationFieldDefinitionsPaginator](./paginators.md#describeregistrationfielddefinitionspaginator)
3. item: `AioPageIterator[DescribeRegistrationFieldDefinitionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRegistrationFieldDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistrationType: str,
    SectionPath: str = ...,
    FieldPaths: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeRegistrationFieldDefinitionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeRegistrationFieldDefinitionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationFieldDefinitionsRequestPaginateTypeDef = {  # (1)
    "RegistrationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationFieldDefinitionsRequestPaginateTypeDef](./type_defs.md#describeregistrationfielddefinitionsrequestpaginatetypedef)
## DescribeRegistrationFieldValuesPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_registration_field_values")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeRegistrationFieldValues.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationFieldValues)

```python
# DescribeRegistrationFieldValuesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeRegistrationFieldValuesPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeRegistrationFieldValuesPaginator = client.get_paginator("describe_registration_field_values")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistrationFieldValuesResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeRegistrationFieldValuesPaginator](./paginators.md#describeregistrationfieldvaluespaginator)
3. item: `AioPageIterator[DescribeRegistrationFieldValuesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRegistrationFieldValuesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistrationId: str,
    VersionNumber: int = ...,
    SectionPath: str = ...,
    FieldPaths: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeRegistrationFieldValuesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeRegistrationFieldValuesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationFieldValuesRequestPaginateTypeDef = {  # (1)
    "RegistrationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationFieldValuesRequestPaginateTypeDef](./type_defs.md#describeregistrationfieldvaluesrequestpaginatetypedef)
## DescribeRegistrationSectionDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_registration_section_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeRegistrationSectionDefinitions.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationSectionDefinitions)

```python
# DescribeRegistrationSectionDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeRegistrationSectionDefinitionsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeRegistrationSectionDefinitionsPaginator = client.get_paginator("describe_registration_section_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistrationSectionDefinitionsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeRegistrationSectionDefinitionsPaginator](./paginators.md#describeregistrationsectiondefinitionspaginator)
3. item: `AioPageIterator[DescribeRegistrationSectionDefinitionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRegistrationSectionDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistrationType: str,
    SectionPaths: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeRegistrationSectionDefinitionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeRegistrationSectionDefinitionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationSectionDefinitionsRequestPaginateTypeDef = {  # (1)
    "RegistrationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationSectionDefinitionsRequestPaginateTypeDef](./type_defs.md#describeregistrationsectiondefinitionsrequestpaginatetypedef)
## DescribeRegistrationTypeDefinitionsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_registration_type_definitions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeRegistrationTypeDefinitions.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationTypeDefinitions)

```python
# DescribeRegistrationTypeDefinitionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeRegistrationTypeDefinitionsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeRegistrationTypeDefinitionsPaginator = client.get_paginator("describe_registration_type_definitions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistrationTypeDefinitionsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeRegistrationTypeDefinitionsPaginator](./paginators.md#describeregistrationtypedefinitionspaginator)
3. item: `AioPageIterator[DescribeRegistrationTypeDefinitionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRegistrationTypeDefinitionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistrationTypes: Sequence[str] = ...,
    Filters: Sequence[RegistrationTypeFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeRegistrationTypeDefinitionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[RegistrationTypeFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeRegistrationTypeDefinitionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationTypeDefinitionsRequestPaginateTypeDef = {  # (1)
    "RegistrationTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationTypeDefinitionsRequestPaginateTypeDef](./type_defs.md#describeregistrationtypedefinitionsrequestpaginatetypedef)
## DescribeRegistrationVersionsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_registration_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeRegistrationVersions.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrationVersions)

```python
# DescribeRegistrationVersionsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeRegistrationVersionsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeRegistrationVersionsPaginator = client.get_paginator("describe_registration_versions")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistrationVersionsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeRegistrationVersionsPaginator](./paginators.md#describeregistrationversionspaginator)
3. item: `AioPageIterator[DescribeRegistrationVersionsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRegistrationVersionsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistrationId: str,
    VersionNumbers: Sequence[int] = ...,
    Filters: Sequence[RegistrationVersionFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeRegistrationVersionsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[RegistrationVersionFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeRegistrationVersionsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationVersionsRequestPaginateTypeDef = {  # (1)
    "RegistrationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationVersionsRequestPaginateTypeDef](./type_defs.md#describeregistrationversionsrequestpaginatetypedef)
## DescribeRegistrationsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_registrations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeRegistrations.html#PinpointSMSVoiceV2.Paginator.DescribeRegistrations)

```python
# DescribeRegistrationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeRegistrationsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeRegistrationsPaginator = client.get_paginator("describe_registrations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRegistrationsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeRegistrationsPaginator](./paginators.md#describeregistrationspaginator)
3. item: `AioPageIterator[DescribeRegistrationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeRegistrationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistrationIds: Sequence[str] = ...,
    Filters: Sequence[RegistrationFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeRegistrationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[RegistrationFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeRegistrationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationsRequestPaginateTypeDef = {  # (1)
    "RegistrationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationsRequestPaginateTypeDef](./type_defs.md#describeregistrationsrequestpaginatetypedef)
## DescribeSenderIdsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_sender_ids")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeSenderIds.html#PinpointSMSVoiceV2.Paginator.DescribeSenderIds)

```python
# DescribeSenderIdsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeSenderIdsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeSenderIdsPaginator = client.get_paginator("describe_sender_ids")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSenderIdsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeSenderIdsPaginator](./paginators.md#describesenderidspaginator)
3. item: `AioPageIterator[DescribeSenderIdsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSenderIdsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    SenderIds: Sequence[SenderIdAndCountryTypeDef] = ...,  # (1)
    Filters: Sequence[SenderIdFilterTypeDef] = ...,  # (2)
    Owner: OwnerType = ...,  # (3)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (4)
) -> aiobotocore.paginate.AioPageIterator[DescribeSenderIdsResultTypeDef]:  # (5)
    ...
```

1. See `Sequence[SenderIdAndCountryTypeDef]`
2. See `Sequence[SenderIdFilterTypeDef]`
3. See [:material-code-brackets: OwnerType](./literals.md#ownertype)
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
5. See `AioPageIterator[DescribeSenderIdsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSenderIdsRequestPaginateTypeDef = {  # (1)
    "SenderIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSenderIdsRequestPaginateTypeDef](./type_defs.md#describesenderidsrequestpaginatetypedef)
## DescribeSpendLimitsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_spend_limits")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeSpendLimits.html#PinpointSMSVoiceV2.Paginator.DescribeSpendLimits)

```python
# DescribeSpendLimitsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeSpendLimitsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeSpendLimitsPaginator = client.get_paginator("describe_spend_limits")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeSpendLimitsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeSpendLimitsPaginator](./paginators.md#describespendlimitspaginator)
3. item: `AioPageIterator[DescribeSpendLimitsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeSpendLimitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> aiobotocore.paginate.AioPageIterator[DescribeSpendLimitsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
2. See `AioPageIterator[DescribeSpendLimitsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSpendLimitsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpendLimitsRequestPaginateTypeDef](./type_defs.md#describespendlimitsrequestpaginatetypedef)
## DescribeVerifiedDestinationNumbersPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("describe_verified_destination_numbers")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/DescribeVerifiedDestinationNumbers.html#PinpointSMSVoiceV2.Paginator.DescribeVerifiedDestinationNumbers)

```python
# DescribeVerifiedDestinationNumbersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import DescribeVerifiedDestinationNumbersPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: DescribeVerifiedDestinationNumbersPaginator = client.get_paginator("describe_verified_destination_numbers")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeVerifiedDestinationNumbersResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [DescribeVerifiedDestinationNumbersPaginator](./paginators.md#describeverifieddestinationnumberspaginator)
3. item: `AioPageIterator[DescribeVerifiedDestinationNumbersResultTypeDef]`


### paginate

Type annotations and code completion for `#!python DescribeVerifiedDestinationNumbersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    VerifiedDestinationNumberIds: Sequence[str] = ...,
    DestinationPhoneNumbers: Sequence[str] = ...,
    Filters: Sequence[VerifiedDestinationNumberFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[DescribeVerifiedDestinationNumbersResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[VerifiedDestinationNumberFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[DescribeVerifiedDestinationNumbersResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVerifiedDestinationNumbersRequestPaginateTypeDef = {  # (1)
    "VerifiedDestinationNumberIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVerifiedDestinationNumbersRequestPaginateTypeDef](./type_defs.md#describeverifieddestinationnumbersrequestpaginatetypedef)
## ListPoolOriginationIdentitiesPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("list_pool_origination_identities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/ListPoolOriginationIdentities.html#PinpointSMSVoiceV2.Paginator.ListPoolOriginationIdentities)

```python
# ListPoolOriginationIdentitiesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import ListPoolOriginationIdentitiesPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: ListPoolOriginationIdentitiesPaginator = client.get_paginator("list_pool_origination_identities")  # (2)
    async for item in paginator.paginate(...):
        item: ListPoolOriginationIdentitiesResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [ListPoolOriginationIdentitiesPaginator](./paginators.md#listpooloriginationidentitiespaginator)
3. item: `AioPageIterator[ListPoolOriginationIdentitiesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListPoolOriginationIdentitiesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PoolId: str,
    Filters: Sequence[PoolOriginationIdentitiesFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListPoolOriginationIdentitiesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[PoolOriginationIdentitiesFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListPoolOriginationIdentitiesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListPoolOriginationIdentitiesRequestPaginateTypeDef = {  # (1)
    "PoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoolOriginationIdentitiesRequestPaginateTypeDef](./type_defs.md#listpooloriginationidentitiesrequestpaginatetypedef)
## ListProtectConfigurationRuleSetNumberOverridesPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("list_protect_configuration_rule_set_number_overrides")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/ListProtectConfigurationRuleSetNumberOverrides.html#PinpointSMSVoiceV2.Paginator.ListProtectConfigurationRuleSetNumberOverrides)

```python
# ListProtectConfigurationRuleSetNumberOverridesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import ListProtectConfigurationRuleSetNumberOverridesPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: ListProtectConfigurationRuleSetNumberOverridesPaginator = client.get_paginator("list_protect_configuration_rule_set_number_overrides")  # (2)
    async for item in paginator.paginate(...):
        item: ListProtectConfigurationRuleSetNumberOverridesResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [ListProtectConfigurationRuleSetNumberOverridesPaginator](./paginators.md#listprotectconfigurationrulesetnumberoverridespaginator)
3. item: `AioPageIterator[ListProtectConfigurationRuleSetNumberOverridesResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListProtectConfigurationRuleSetNumberOverridesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ProtectConfigurationId: str,
    Filters: Sequence[ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListProtectConfigurationRuleSetNumberOverridesResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListProtectConfigurationRuleSetNumberOverridesResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectConfigurationRuleSetNumberOverridesRequestPaginateTypeDef = {  # (1)
    "ProtectConfigurationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectConfigurationRuleSetNumberOverridesRequestPaginateTypeDef](./type_defs.md#listprotectconfigurationrulesetnumberoverridesrequestpaginatetypedef)
## ListRegistrationAssociationsPaginator

Type annotations and code completion for `#!python session.create_client("pinpoint-sms-voice-v2").get_paginator("list_registration_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-sms-voice-v2/paginator/ListRegistrationAssociations.html#PinpointSMSVoiceV2.Paginator.ListRegistrationAssociations)

```python
# ListRegistrationAssociationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_pinpoint_sms_voice_v2.paginator import ListRegistrationAssociationsPaginator

session = get_session()
async with session.create_client("pinpoint-sms-voice-v2") as client:  # (1)
    paginator: ListRegistrationAssociationsPaginator = client.get_paginator("list_registration_associations")  # (2)
    async for item in paginator.paginate(...):
        item: ListRegistrationAssociationsResultTypeDef
        print(item)  # (3)
```

1. client: [PinpointSMSVoiceV2Client](./client.md)
2. paginator: [ListRegistrationAssociationsPaginator](./paginators.md#listregistrationassociationspaginator)
3. item: `AioPageIterator[ListRegistrationAssociationsResultTypeDef]`


### paginate

Type annotations and code completion for `#!python ListRegistrationAssociationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RegistrationId: str,
    Filters: Sequence[RegistrationAssociationFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> aiobotocore.paginate.AioPageIterator[ListRegistrationAssociationsResultTypeDef]:  # (3)
    ...
```

1. See `Sequence[RegistrationAssociationFilterTypeDef]`
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
3. See `AioPageIterator[ListRegistrationAssociationsResultTypeDef]`


```python
# paginate method usage example with argument unpacking

kwargs: ListRegistrationAssociationsRequestPaginateTypeDef = {  # (1)
    "RegistrationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegistrationAssociationsRequestPaginateTypeDef](./type_defs.md#listregistrationassociationsrequestpaginatetypedef)

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
3. item: [:material-code-braces: DescribeAccountAttributesResultTypeDef](./type_defs.md#describeaccountattributesresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAccountAttributesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAccountAttributesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAccountAttributesResultTypeDef](./type_defs.md#describeaccountattributesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountAttributesRequestDescribeAccountAttributesPaginateTypeDef](./type_defs.md#describeaccountattributesrequestdescribeaccountattributespaginatetypedef) 
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
3. item: [:material-code-braces: DescribeAccountLimitsResultTypeDef](./type_defs.md#describeaccountlimitsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAccountLimitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeAccountLimitsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAccountLimitsResultTypeDef](./type_defs.md#describeaccountlimitsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAccountLimitsRequestDescribeAccountLimitsPaginateTypeDef](./type_defs.md#describeaccountlimitsrequestdescribeaccountlimitspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeConfigurationSetsResultTypeDef](./type_defs.md#describeconfigurationsetsresulttypedef) 


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
) -> AsyncIterator[DescribeConfigurationSetsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ConfigurationSetFilterTypeDef](./type_defs.md#configurationsetfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeConfigurationSetsResultTypeDef](./type_defs.md#describeconfigurationsetsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef = {  # (1)
    "ConfigurationSetNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationSetsRequestDescribeConfigurationSetsPaginateTypeDef](./type_defs.md#describeconfigurationsetsrequestdescribeconfigurationsetspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeKeywordsResultTypeDef](./type_defs.md#describekeywordsresulttypedef) 


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
) -> AsyncIterator[DescribeKeywordsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: KeywordFilterTypeDef](./type_defs.md#keywordfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeKeywordsResultTypeDef](./type_defs.md#describekeywordsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef = {  # (1)
    "OriginationIdentity": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeKeywordsRequestDescribeKeywordsPaginateTypeDef](./type_defs.md#describekeywordsrequestdescribekeywordspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeOptOutListsResultTypeDef](./type_defs.md#describeoptoutlistsresulttypedef) 


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
) -> AsyncIterator[DescribeOptOutListsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeOptOutListsResultTypeDef](./type_defs.md#describeoptoutlistsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef = {  # (1)
    "OptOutListNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOptOutListsRequestDescribeOptOutListsPaginateTypeDef](./type_defs.md#describeoptoutlistsrequestdescribeoptoutlistspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeOptedOutNumbersResultTypeDef](./type_defs.md#describeoptedoutnumbersresulttypedef) 


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
) -> AsyncIterator[DescribeOptedOutNumbersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OptedOutFilterTypeDef](./type_defs.md#optedoutfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeOptedOutNumbersResultTypeDef](./type_defs.md#describeoptedoutnumbersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef = {  # (1)
    "OptOutListName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOptedOutNumbersRequestDescribeOptedOutNumbersPaginateTypeDef](./type_defs.md#describeoptedoutnumbersrequestdescribeoptedoutnumberspaginatetypedef) 
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
3. item: [:material-code-braces: DescribePhoneNumbersResultTypeDef](./type_defs.md#describephonenumbersresulttypedef) 


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
) -> AsyncIterator[DescribePhoneNumbersResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: PhoneNumberFilterTypeDef](./type_defs.md#phonenumberfiltertypedef) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribePhoneNumbersResultTypeDef](./type_defs.md#describephonenumbersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef = {  # (1)
    "PhoneNumberIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePhoneNumbersRequestDescribePhoneNumbersPaginateTypeDef](./type_defs.md#describephonenumbersrequestdescribephonenumberspaginatetypedef) 
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
3. item: [:material-code-braces: DescribePoolsResultTypeDef](./type_defs.md#describepoolsresulttypedef) 


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
) -> AsyncIterator[DescribePoolsResultTypeDef]:  # (4)
    ...
```

1. See [:material-code-braces: PoolFilterTypeDef](./type_defs.md#poolfiltertypedef) 
2. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: DescribePoolsResultTypeDef](./type_defs.md#describepoolsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribePoolsRequestDescribePoolsPaginateTypeDef = {  # (1)
    "PoolIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePoolsRequestDescribePoolsPaginateTypeDef](./type_defs.md#describepoolsrequestdescribepoolspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeProtectConfigurationsResultTypeDef](./type_defs.md#describeprotectconfigurationsresulttypedef) 


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
) -> AsyncIterator[DescribeProtectConfigurationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ProtectConfigurationFilterTypeDef](./type_defs.md#protectconfigurationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeProtectConfigurationsResultTypeDef](./type_defs.md#describeprotectconfigurationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeProtectConfigurationsRequestDescribeProtectConfigurationsPaginateTypeDef = {  # (1)
    "ProtectConfigurationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeProtectConfigurationsRequestDescribeProtectConfigurationsPaginateTypeDef](./type_defs.md#describeprotectconfigurationsrequestdescribeprotectconfigurationspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeRegistrationAttachmentsResultTypeDef](./type_defs.md#describeregistrationattachmentsresulttypedef) 


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
) -> AsyncIterator[DescribeRegistrationAttachmentsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RegistrationAttachmentFilterTypeDef](./type_defs.md#registrationattachmentfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRegistrationAttachmentsResultTypeDef](./type_defs.md#describeregistrationattachmentsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef = {  # (1)
    "RegistrationAttachmentIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationAttachmentsRequestDescribeRegistrationAttachmentsPaginateTypeDef](./type_defs.md#describeregistrationattachmentsrequestdescriberegistrationattachmentspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeRegistrationFieldDefinitionsResultTypeDef](./type_defs.md#describeregistrationfielddefinitionsresulttypedef) 


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
) -> AsyncIterator[DescribeRegistrationFieldDefinitionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRegistrationFieldDefinitionsResultTypeDef](./type_defs.md#describeregistrationfielddefinitionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationFieldDefinitionsRequestDescribeRegistrationFieldDefinitionsPaginateTypeDef = {  # (1)
    "RegistrationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationFieldDefinitionsRequestDescribeRegistrationFieldDefinitionsPaginateTypeDef](./type_defs.md#describeregistrationfielddefinitionsrequestdescriberegistrationfielddefinitionspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeRegistrationFieldValuesResultTypeDef](./type_defs.md#describeregistrationfieldvaluesresulttypedef) 


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
) -> AsyncIterator[DescribeRegistrationFieldValuesResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRegistrationFieldValuesResultTypeDef](./type_defs.md#describeregistrationfieldvaluesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationFieldValuesRequestDescribeRegistrationFieldValuesPaginateTypeDef = {  # (1)
    "RegistrationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationFieldValuesRequestDescribeRegistrationFieldValuesPaginateTypeDef](./type_defs.md#describeregistrationfieldvaluesrequestdescriberegistrationfieldvaluespaginatetypedef) 
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
3. item: [:material-code-braces: DescribeRegistrationSectionDefinitionsResultTypeDef](./type_defs.md#describeregistrationsectiondefinitionsresulttypedef) 


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
) -> AsyncIterator[DescribeRegistrationSectionDefinitionsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRegistrationSectionDefinitionsResultTypeDef](./type_defs.md#describeregistrationsectiondefinitionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationSectionDefinitionsRequestDescribeRegistrationSectionDefinitionsPaginateTypeDef = {  # (1)
    "RegistrationType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationSectionDefinitionsRequestDescribeRegistrationSectionDefinitionsPaginateTypeDef](./type_defs.md#describeregistrationsectiondefinitionsrequestdescriberegistrationsectiondefinitionspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeRegistrationTypeDefinitionsResultTypeDef](./type_defs.md#describeregistrationtypedefinitionsresulttypedef) 


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
) -> AsyncIterator[DescribeRegistrationTypeDefinitionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RegistrationTypeFilterTypeDef](./type_defs.md#registrationtypefiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRegistrationTypeDefinitionsResultTypeDef](./type_defs.md#describeregistrationtypedefinitionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef = {  # (1)
    "RegistrationTypes": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationTypeDefinitionsRequestDescribeRegistrationTypeDefinitionsPaginateTypeDef](./type_defs.md#describeregistrationtypedefinitionsrequestdescriberegistrationtypedefinitionspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeRegistrationVersionsResultTypeDef](./type_defs.md#describeregistrationversionsresulttypedef) 


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
) -> AsyncIterator[DescribeRegistrationVersionsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RegistrationVersionFilterTypeDef](./type_defs.md#registrationversionfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRegistrationVersionsResultTypeDef](./type_defs.md#describeregistrationversionsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationVersionsRequestDescribeRegistrationVersionsPaginateTypeDef = {  # (1)
    "RegistrationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationVersionsRequestDescribeRegistrationVersionsPaginateTypeDef](./type_defs.md#describeregistrationversionsrequestdescriberegistrationversionspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeRegistrationsResultTypeDef](./type_defs.md#describeregistrationsresulttypedef) 


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
) -> AsyncIterator[DescribeRegistrationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RegistrationFilterTypeDef](./type_defs.md#registrationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRegistrationsResultTypeDef](./type_defs.md#describeregistrationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRegistrationsRequestDescribeRegistrationsPaginateTypeDef = {  # (1)
    "RegistrationIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRegistrationsRequestDescribeRegistrationsPaginateTypeDef](./type_defs.md#describeregistrationsrequestdescriberegistrationspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeSenderIdsResultTypeDef](./type_defs.md#describesenderidsresulttypedef) 


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
) -> AsyncIterator[DescribeSenderIdsResultTypeDef]:  # (5)
    ...
```

1. See [:material-code-braces: SenderIdAndCountryTypeDef](./type_defs.md#senderidandcountrytypedef) 
2. See [:material-code-braces: SenderIdFilterTypeDef](./type_defs.md#senderidfiltertypedef) 
3. See [:material-code-brackets: OwnerType](./literals.md#ownertype) 
4. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
5. See [:material-code-braces: DescribeSenderIdsResultTypeDef](./type_defs.md#describesenderidsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef = {  # (1)
    "SenderIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSenderIdsRequestDescribeSenderIdsPaginateTypeDef](./type_defs.md#describesenderidsrequestdescribesenderidspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeSpendLimitsResultTypeDef](./type_defs.md#describespendlimitsresulttypedef) 


### paginate

Type annotations and code completion for `#!python DescribeSpendLimitsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[DescribeSpendLimitsResultTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeSpendLimitsResultTypeDef](./type_defs.md#describespendlimitsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeSpendLimitsRequestDescribeSpendLimitsPaginateTypeDef](./type_defs.md#describespendlimitsrequestdescribespendlimitspaginatetypedef) 
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
3. item: [:material-code-braces: DescribeVerifiedDestinationNumbersResultTypeDef](./type_defs.md#describeverifieddestinationnumbersresulttypedef) 


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
) -> AsyncIterator[DescribeVerifiedDestinationNumbersResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: VerifiedDestinationNumberFilterTypeDef](./type_defs.md#verifieddestinationnumberfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeVerifiedDestinationNumbersResultTypeDef](./type_defs.md#describeverifieddestinationnumbersresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef = {  # (1)
    "VerifiedDestinationNumberIds": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeVerifiedDestinationNumbersRequestDescribeVerifiedDestinationNumbersPaginateTypeDef](./type_defs.md#describeverifieddestinationnumbersrequestdescribeverifieddestinationnumberspaginatetypedef) 
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
3. item: [:material-code-braces: ListPoolOriginationIdentitiesResultTypeDef](./type_defs.md#listpooloriginationidentitiesresulttypedef) 


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
) -> AsyncIterator[ListPoolOriginationIdentitiesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: PoolOriginationIdentitiesFilterTypeDef](./type_defs.md#pooloriginationidentitiesfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListPoolOriginationIdentitiesResultTypeDef](./type_defs.md#listpooloriginationidentitiesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef = {  # (1)
    "PoolId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListPoolOriginationIdentitiesRequestListPoolOriginationIdentitiesPaginateTypeDef](./type_defs.md#listpooloriginationidentitiesrequestlistpooloriginationidentitiespaginatetypedef) 
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
3. item: [:material-code-braces: ListProtectConfigurationRuleSetNumberOverridesResultTypeDef](./type_defs.md#listprotectconfigurationrulesetnumberoverridesresulttypedef) 


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
) -> AsyncIterator[ListProtectConfigurationRuleSetNumberOverridesResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ProtectConfigurationRuleSetNumberOverrideFilterItemTypeDef](./type_defs.md#protectconfigurationrulesetnumberoverridefilteritemtypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListProtectConfigurationRuleSetNumberOverridesResultTypeDef](./type_defs.md#listprotectconfigurationrulesetnumberoverridesresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListProtectConfigurationRuleSetNumberOverridesRequestListProtectConfigurationRuleSetNumberOverridesPaginateTypeDef = {  # (1)
    "ProtectConfigurationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListProtectConfigurationRuleSetNumberOverridesRequestListProtectConfigurationRuleSetNumberOverridesPaginateTypeDef](./type_defs.md#listprotectconfigurationrulesetnumberoverridesrequestlistprotectconfigurationrulesetnumberoverridespaginatetypedef) 
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
3. item: [:material-code-braces: ListRegistrationAssociationsResultTypeDef](./type_defs.md#listregistrationassociationsresulttypedef) 


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
) -> AsyncIterator[ListRegistrationAssociationsResultTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: RegistrationAssociationFilterTypeDef](./type_defs.md#registrationassociationfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListRegistrationAssociationsResultTypeDef](./type_defs.md#listregistrationassociationsresulttypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef = {  # (1)
    "RegistrationId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListRegistrationAssociationsRequestListRegistrationAssociationsPaginateTypeDef](./type_defs.md#listregistrationassociationsrequestlistregistrationassociationspaginatetypedef) 

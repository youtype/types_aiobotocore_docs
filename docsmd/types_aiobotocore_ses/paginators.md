# Paginators

> [Index](../README.md) > [SES](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [SES](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
    type annotations stubs module [types-aiobotocore-ses](https://pypi.org/project/types-aiobotocore-ses/).

## ListConfigurationSetsPaginator

Type annotations and code completion for `#!python session.create_client("ses").get_paginator("list_configuration_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListConfigurationSetsPaginator

session = get_session()
async with session.create_client("ses") as client:  # (1)
    paginator: ListConfigurationSetsPaginator = client.get_paginator("list_configuration_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [SESClient](./client.md)
2. paginator: [ListConfigurationSetsPaginator](./paginators.md#listconfigurationsetspaginator)
3. item: [:material-code-braces: ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListConfigurationSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef](./type_defs.md#listconfigurationsetsrequestlistconfigurationsetspaginatetypedef) 
## ListCustomVerificationEmailTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("ses").get_paginator("list_custom_verification_email_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListCustomVerificationEmailTemplatesPaginator

session = get_session()
async with session.create_client("ses") as client:  # (1)
    paginator: ListCustomVerificationEmailTemplatesPaginator = client.get_paginator("list_custom_verification_email_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListCustomVerificationEmailTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [SESClient](./client.md)
2. paginator: [ListCustomVerificationEmailTemplatesPaginator](./paginators.md#listcustomverificationemailtemplatespaginator)
3. item: [:material-code-braces: ListCustomVerificationEmailTemplatesResponseTypeDef](./type_defs.md#listcustomverificationemailtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListCustomVerificationEmailTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListCustomVerificationEmailTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListCustomVerificationEmailTemplatesResponseTypeDef](./type_defs.md#listcustomverificationemailtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListCustomVerificationEmailTemplatesRequestListCustomVerificationEmailTemplatesPaginateTypeDef](./type_defs.md#listcustomverificationemailtemplatesrequestlistcustomverificationemailtemplatespaginatetypedef) 
## ListIdentitiesPaginator

Type annotations and code completion for `#!python session.create_client("ses").get_paginator("list_identities")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListIdentities)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListIdentitiesPaginator

session = get_session()
async with session.create_client("ses") as client:  # (1)
    paginator: ListIdentitiesPaginator = client.get_paginator("list_identities")  # (2)
    async for item in paginator.paginate(...):
        item: ListIdentitiesResponseTypeDef
        print(item)  # (3)
```

1. client: [SESClient](./client.md)
2. paginator: [ListIdentitiesPaginator](./paginators.md#listidentitiespaginator)
3. item: [:material-code-braces: ListIdentitiesResponseTypeDef](./type_defs.md#listidentitiesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListIdentitiesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    IdentityType: IdentityTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AsyncIterator[ListIdentitiesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: IdentityTypeType](./literals.md#identitytypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListIdentitiesResponseTypeDef](./type_defs.md#listidentitiesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListIdentitiesRequestListIdentitiesPaginateTypeDef = {  # (1)
    "IdentityType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListIdentitiesRequestListIdentitiesPaginateTypeDef](./type_defs.md#listidentitiesrequestlistidentitiespaginatetypedef) 
## ListReceiptRuleSetsPaginator

Type annotations and code completion for `#!python session.create_client("ses").get_paginator("list_receipt_rule_sets")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListReceiptRuleSetsPaginator

session = get_session()
async with session.create_client("ses") as client:  # (1)
    paginator: ListReceiptRuleSetsPaginator = client.get_paginator("list_receipt_rule_sets")  # (2)
    async for item in paginator.paginate(...):
        item: ListReceiptRuleSetsResponseTypeDef
        print(item)  # (3)
```

1. client: [SESClient](./client.md)
2. paginator: [ListReceiptRuleSetsPaginator](./paginators.md#listreceiptrulesetspaginator)
3. item: [:material-code-braces: ListReceiptRuleSetsResponseTypeDef](./type_defs.md#listreceiptrulesetsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListReceiptRuleSetsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListReceiptRuleSetsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListReceiptRuleSetsResponseTypeDef](./type_defs.md#listreceiptrulesetsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListReceiptRuleSetsRequestListReceiptRuleSetsPaginateTypeDef](./type_defs.md#listreceiptrulesetsrequestlistreceiptrulesetspaginatetypedef) 
## ListTemplatesPaginator

Type annotations and code completion for `#!python session.create_client("ses").get_paginator("list_templates")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListTemplatesPaginator

session = get_session()
async with session.create_client("ses") as client:  # (1)
    paginator: ListTemplatesPaginator = client.get_paginator("list_templates")  # (2)
    async for item in paginator.paginate(...):
        item: ListTemplatesResponseTypeDef
        print(item)  # (3)
```

1. client: [SESClient](./client.md)
2. paginator: [ListTemplatesPaginator](./paginators.md#listtemplatespaginator)
3. item: [:material-code-braces: ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTemplatesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AsyncIterator[ListTemplatesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: ListTemplatesRequestListTemplatesPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTemplatesRequestListTemplatesPaginateTypeDef](./type_defs.md#listtemplatesrequestlisttemplatespaginatetypedef) 

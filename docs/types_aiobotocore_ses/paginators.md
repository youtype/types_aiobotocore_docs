<a id="paginators-for-aiobotocore-ses-module"></a>

# Paginators for aiobotocore SES module

> [Index](../README.md) > [SES](./README.md) > Paginators

Auto-generated documentation for
[SES](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES)
type annotations stubs module
[types-aiobotocore-ses](https://pypi.org/project/types-aiobotocore-ses/).

- [Paginators for aiobotocore SES module](#paginators-for-aiobotocore-ses-module)
  - [ListConfigurationSetsPaginator](#listconfigurationsetspaginator)
  - [ListCustomVerificationEmailTemplatesPaginator](#listcustomverificationemailtemplatespaginator)
  - [ListIdentitiesPaginator](#listidentitiespaginator)
  - [ListReceiptRuleSetsPaginator](#listreceiptrulesetspaginator)
  - [ListTemplatesPaginator](#listtemplatespaginator)

<a id="listconfigurationsetspaginator"></a>

## ListConfigurationSetsPaginator

Type annotations for
`session.create_client("ses").get_paginator("list_configuration_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListConfigurationSetsPaginator

session = get_session()
async with session.create_client("ses") as client:
    client: SESClient
    paginator: ListConfigurationSetsPaginator = client.get_paginator("list_configuration_sets")
```

Boto3 documentation:
[SES.Paginator.ListConfigurationSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListConfigurationSets)

Arguments for `ListConfigurationSetsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListConfigurationSetsPaginator.paginate` returns
`AsyncIterator`\[[ListConfigurationSetsResponseTypeDef](./type_defs.md#listconfigurationsetsresponsetypedef)\].

<a id="listcustomverificationemailtemplatespaginator"></a>

## ListCustomVerificationEmailTemplatesPaginator

Type annotations for
`session.create_client("ses").get_paginator("list_custom_verification_email_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListCustomVerificationEmailTemplatesPaginator

session = get_session()
async with session.create_client("ses") as client:
    client: SESClient
    paginator: ListCustomVerificationEmailTemplatesPaginator = client.get_paginator("list_custom_verification_email_templates")
```

Boto3 documentation:
[SES.Paginator.ListCustomVerificationEmailTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListCustomVerificationEmailTemplates)

Arguments for `ListCustomVerificationEmailTemplatesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListCustomVerificationEmailTemplatesPaginator.paginate` returns
`AsyncIterator`\[[ListCustomVerificationEmailTemplatesResponseTypeDef](./type_defs.md#listcustomverificationemailtemplatesresponsetypedef)\].

<a id="listidentitiespaginator"></a>

## ListIdentitiesPaginator

Type annotations for
`session.create_client("ses").get_paginator("list_identities")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListIdentitiesPaginator

session = get_session()
async with session.create_client("ses") as client:
    client: SESClient
    paginator: ListIdentitiesPaginator = client.get_paginator("list_identities")
```

Boto3 documentation:
[SES.Paginator.ListIdentities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListIdentities)

Arguments for `ListIdentitiesPaginator.paginate` method:

- `IdentityType`: [IdentityTypeType](./literals.md#identitytypetype)
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListIdentitiesPaginator.paginate` returns
`AsyncIterator`\[[ListIdentitiesResponseTypeDef](./type_defs.md#listidentitiesresponsetypedef)\].

<a id="listreceiptrulesetspaginator"></a>

## ListReceiptRuleSetsPaginator

Type annotations for
`session.create_client("ses").get_paginator("list_receipt_rule_sets")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListReceiptRuleSetsPaginator

session = get_session()
async with session.create_client("ses") as client:
    client: SESClient
    paginator: ListReceiptRuleSetsPaginator = client.get_paginator("list_receipt_rule_sets")
```

Boto3 documentation:
[SES.Paginator.ListReceiptRuleSets](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListReceiptRuleSets)

Arguments for `ListReceiptRuleSetsPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListReceiptRuleSetsPaginator.paginate` returns
`AsyncIterator`\[[ListReceiptRuleSetsResponseTypeDef](./type_defs.md#listreceiptrulesetsresponsetypedef)\].

<a id="listtemplatespaginator"></a>

## ListTemplatesPaginator

Type annotations for
`session.create_client("ses").get_paginator("list_templates")`.

Can be used directly:

```python
from aiobotocore.session import get_session

from types_aiobotocore_ses.paginator import ListTemplatesPaginator

session = get_session()
async with session.create_client("ses") as client:
    client: SESClient
    paginator: ListTemplatesPaginator = client.get_paginator("list_templates")
```

Boto3 documentation:
[SES.Paginator.ListTemplates](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Paginator.ListTemplates)

Arguments for `ListTemplatesPaginator.paginate` method:

- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListTemplatesPaginator.paginate` returns
`AsyncIterator`\[[ListTemplatesResponseTypeDef](./type_defs.md#listtemplatesresponsetypedef)\].

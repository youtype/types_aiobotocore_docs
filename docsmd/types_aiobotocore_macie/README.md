# Macie module

> [Index](../README.md) > Macie


!!! note ""

    Auto-generated documentation for [Macie](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
    type annotations stubs module [types-aiobotocore-macie](https://pypi.org/project/types-aiobotocore-macie/).

## How to install



### From PyPI with pip

Install `types-aiobotocore` for `Macie` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[macie]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[macie]'


# standalone installation
python -m pip install types-aiobotocore-macie
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-macie
```

## Usage

Code samples can be found in [Examples](./usage.md).

## MacieClient

Type annotations and code completion for  `#!python session.create_client("macie")` as [MacieClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_macie.client import MacieClient


session = get_session()
async with session.create_client("macie") as client:
    client: MacieClient
```


## Paginators

Type annotations and code completion for
[paginators](./paginators.md)
from `#!python session.create_client("macie").get_paginator("...")`.

```python title="Usage example"
from types_aiobotocore_macie.paginator import ListMemberAccountsPaginator

def get_list_member_accounts_paginator() -> ListMemberAccountsPaginator:
    return client.get_paginator("list_member_accounts"))
```

- [ListMemberAccountsPaginator](./paginators.md#listmemberaccountspaginator)
- [ListS3ResourcesPaginator](./paginators.md#lists3resourcespaginator)








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_macie.literals import ListMemberAccountsPaginatorName

def get_value() -> ListMemberAccountsPaginatorName:
    return "list_member_accounts"
```

- [ListMemberAccountsPaginatorName](./literals.md#listmemberaccountspaginatorname)
- [ListS3ResourcesPaginatorName](./literals.md#lists3resourcespaginatorname)
- [S3ContinuousClassificationTypeType](./literals.md#s3continuousclassificationtypetype)
- [S3OneTimeClassificationTypeType](./literals.md#s3onetimeclassificationtypetype)
- [MacieServiceName](./literals.md#macieservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_macie.type_defs import AssociateMemberAccountRequestRequestTypeDef

def get_value() -> AssociateMemberAccountRequestRequestTypeDef:
    return {
        "memberAccountId": ...,
    }
```

- [AssociateMemberAccountRequestRequestTypeDef](./type_defs.md#associatememberaccountrequestrequesttypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ClassificationTypeTypeDef](./type_defs.md#classificationtypetypedef)
- [ClassificationTypeUpdateTypeDef](./type_defs.md#classificationtypeupdatetypedef)
- [DisassociateMemberAccountRequestRequestTypeDef](./type_defs.md#disassociatememberaccountrequestrequesttypedef)
- [S3ResourceTypeDef](./type_defs.md#s3resourcetypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ListMemberAccountsRequestRequestTypeDef](./type_defs.md#listmemberaccountsrequestrequesttypedef)
- [MemberAccountTypeDef](./type_defs.md#memberaccounttypedef)
- [ListS3ResourcesRequestRequestTypeDef](./type_defs.md#lists3resourcesrequestrequesttypedef)
- [EmptyResponseMetadataTypeDef](./type_defs.md#emptyresponsemetadatatypedef)
- [S3ResourceClassificationTypeDef](./type_defs.md#s3resourceclassificationtypedef)
- [S3ResourceClassificationUpdateTypeDef](./type_defs.md#s3resourceclassificationupdatetypedef)
- [DisassociateS3ResourcesRequestRequestTypeDef](./type_defs.md#disassociates3resourcesrequestrequesttypedef)
- [FailedS3ResourceTypeDef](./type_defs.md#faileds3resourcetypedef)
- [ListMemberAccountsRequestListMemberAccountsPaginateTypeDef](./type_defs.md#listmemberaccountsrequestlistmemberaccountspaginatetypedef)
- [ListS3ResourcesRequestListS3ResourcesPaginateTypeDef](./type_defs.md#lists3resourcesrequestlists3resourcespaginatetypedef)
- [ListMemberAccountsResultTypeDef](./type_defs.md#listmemberaccountsresulttypedef)
- [AssociateS3ResourcesRequestRequestTypeDef](./type_defs.md#associates3resourcesrequestrequesttypedef)
- [ListS3ResourcesResultTypeDef](./type_defs.md#lists3resourcesresulttypedef)
- [UpdateS3ResourcesRequestRequestTypeDef](./type_defs.md#updates3resourcesrequestrequesttypedef)
- [AssociateS3ResourcesResultTypeDef](./type_defs.md#associates3resourcesresulttypedef)
- [DisassociateS3ResourcesResultTypeDef](./type_defs.md#disassociates3resourcesresulttypedef)
- [UpdateS3ResourcesResultTypeDef](./type_defs.md#updates3resourcesresulttypedef)


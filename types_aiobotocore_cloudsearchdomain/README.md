<a id="type-annotations-for-aiobotocore-cloudsearchdomain-module"></a>

# Type annotations for aiobotocore CloudSearchDomain module

> [Index](..) > CloudSearchDomain

Auto-generated documentation for
[CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
type annotations stubs module
[types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

```bash
# install with types-aiobotocore
pip install 'types-aiobotocore[cloudsearchdomain]'

# Lite version does not provide session.create_client overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[cloudsearchdomain]'

# standalone installation
pip install types-aiobotocore-cloudsearchdomain
```

- [Type annotations for aiobotocore CloudSearchDomain module](#type-annotations-for-aiobotocore-cloudsearchdomain-module)
  - [CloudSearchDomainClient](#cloudsearchdomainclient)
    - [Methods](#methods)
    - [Exceptions](#exceptions)
  - [Literals](#literals)
  - [Typed dictionaries](#typed-dictionaries)

<a id="cloudsearchdomainclient"></a>

## CloudSearchDomainClient

Type annotations for `session.create_client("cloudsearchdomain")` as
[CloudSearchDomainClient](./client.md)

Can be used directly:

```python
from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient
```

<a id="methods"></a>

### Methods

- [__aenter__](./client.md#__aenter__)
- [__aexit__](./client.md#__aexit__)
- [can_paginate](./client.md#can_paginate)
- [exceptions](./client.md#exceptions)
- [generate_presigned_url](./client.md#generate_presigned_url)
- [search](./client.md#search)
- [suggest](./client.md#suggest)
- [upload_documents](./client.md#upload_documents)

<a id="exceptions"></a>

### Exceptions

CloudSearchDomainClient [exceptions](./client.md#exceptions)

- ClientError
- DocumentServiceException
- SearchException

<a id="literals"></a>

## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

Can be used directly:

```python
from types_aiobotocore_cloudsearchdomain.literals import ContentTypeType, ...
```

- [ContentTypeType](./literals.md#contenttypetype)
- [QueryParserType](./literals.md#queryparsertype)
- [ServiceName](./literals.md#servicename)

<a id="typed-dictionaries"></a>

## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and
schema.

Can be used directly:

```python
from mypy_boto3_cloudsearchdomain.type_defs import BucketInfoTypeDef, ...
```

- [BucketInfoTypeDef](./type_defs.md#bucketinfotypedef)
- [BucketTypeDef](./type_defs.md#buckettypedef)
- [DocumentServiceWarningTypeDef](./type_defs.md#documentservicewarningtypedef)
- [FieldStatsTypeDef](./type_defs.md#fieldstatstypedef)
- [HitTypeDef](./type_defs.md#hittypedef)
- [HitsTypeDef](./type_defs.md#hitstypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [SearchRequestRequestTypeDef](./type_defs.md#searchrequestrequesttypedef)
- [SearchResponseTypeDef](./type_defs.md#searchresponsetypedef)
- [SearchStatusTypeDef](./type_defs.md#searchstatustypedef)
- [SuggestModelTypeDef](./type_defs.md#suggestmodeltypedef)
- [SuggestRequestRequestTypeDef](./type_defs.md#suggestrequestrequesttypedef)
- [SuggestResponseTypeDef](./type_defs.md#suggestresponsetypedef)
- [SuggestStatusTypeDef](./type_defs.md#suggeststatustypedef)
- [SuggestionMatchTypeDef](./type_defs.md#suggestionmatchtypedef)
- [UploadDocumentsRequestRequestTypeDef](./type_defs.md#uploaddocumentsrequestrequesttypedef)
- [UploadDocumentsResponseTypeDef](./type_defs.md#uploaddocumentsresponsetypedef)

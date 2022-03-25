<a id="cloudsearchdomainclient-for-aiobotocore-cloudsearchdomain-module"></a>

# CloudSearchDomainClient for aiobotocore CloudSearchDomain module

> [Index](../README.md) > [CloudSearchDomain](./README.md) >
> CloudSearchDomainClient

Auto-generated documentation for
[CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
type annotations stubs module
[types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

- [CloudSearchDomainClient for aiobotocore CloudSearchDomain module](#cloudsearchdomainclient-for-aiobotocore-cloudsearchdomain-module)
  - [CloudSearchDomainClient](#cloudsearchdomainclient)
  - [Exceptions](#exceptions)
  - [Methods](#methods)
    - [exceptions](#exceptions)
    - [can_paginate](#can_paginate)
    - [generate_presigned_url](#generate_presigned_url)
    - [search](#search)
    - [suggest](#suggest)
    - [upload_documents](#upload_documents)
    - [\_\_aenter\_\_](#__aenter__)
    - [\_\_aexit\_\_](#__aexit__)

<a id="cloudsearchdomainclient"></a>

## CloudSearchDomainClient

Type annotations for `session.create_client("cloudsearchdomain")`

Can be used directly:

```python
from aiobotocore.session import get_session
from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient

session = get_session()
async with session.create_client("cloudsearchdomain") as client:
    client: CloudSearchDomainClient
```

Boto3 documentation:
[CloudSearchDomain.Client](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)

<a id="exceptions"></a>

## Exceptions

`boto3` client exceptions are generated in runtime. This class can be used for
static analysis directly:

```python
from types_aiobotocore_cloudsearchdomain.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```

Exceptions:

- `Exceptions.ClientError`
- `Exceptions.DocumentServiceException`
- `Exceptions.SearchException`

<a id="methods"></a>

## Methods

<a id="exceptions"></a>

### exceptions

CloudSearchDomainClient exceptions.

Type annotations for `session.create_client("cloudsearchdomain").exceptions`
method.

Boto3 documentation:
[CloudSearchDomain.Client.exceptions](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.exceptions)

Returns [Exceptions](#exceptions).

<a id="can\_paginate"></a>

### can_paginate

Check if an operation can be paginated.

Type annotations for `session.create_client("cloudsearchdomain").can_paginate`
method.

Boto3 documentation:
[CloudSearchDomain.Client.can_paginate](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.can_paginate)

Arguments:

- `operation_name`: `str` *(required)*

Returns `bool`.

<a id="generate\_presigned\_url"></a>

### generate_presigned_url

Generate a presigned url given a client, its method, and arguments.

Type annotations for
`session.create_client("cloudsearchdomain").generate_presigned_url` method.

Boto3 documentation:
[CloudSearchDomain.Client.generate_presigned_url](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.generate_presigned_url)

Asynchronous method. Use `await generate_presigned_url(...)` for a synchronous
call.

Arguments:

- `ClientMethod`: `str` *(required)*
- `Params`: `Mapping`\[`str`, `Any`\]
- `ExpiresIn`: `int`
- `HttpMethod`: `str`

Returns a `Coroutine` for `str`.

<a id="search"></a>

### search

Retrieves a list of documents that match the specified search criteria.

Type annotations for `session.create_client("cloudsearchdomain").search`
method.

Boto3 documentation:
[CloudSearchDomain.Client.search](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.search)

Asynchronous method. Use `await search(...)` for a synchronous call.

Arguments mapping described in
[SearchRequestRequestTypeDef](./type_defs.md#searchrequestrequesttypedef).

Keyword-only arguments:

- `query`: `str` *(required)*
- `cursor`: `str`
- `expr`: `str`
- `facet`: `str`
- `filterQuery`: `str`
- `highlight`: `str`
- `partial`: `bool`
- `queryOptions`: `str`
- `queryParser`: [QueryParserType](./literals.md#queryparsertype)
- `returnFields`: `str`
- `size`: `int`
- `sort`: `str`
- `start`: `int`
- `stats`: `str`

Returns a `Coroutine` for
[SearchResponseTypeDef](./type_defs.md#searchresponsetypedef).

<a id="suggest"></a>

### suggest

Retrieves autocomplete suggestions for a partial query string.

Type annotations for `session.create_client("cloudsearchdomain").suggest`
method.

Boto3 documentation:
[CloudSearchDomain.Client.suggest](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.suggest)

Asynchronous method. Use `await suggest(...)` for a synchronous call.

Arguments mapping described in
[SuggestRequestRequestTypeDef](./type_defs.md#suggestrequestrequesttypedef).

Keyword-only arguments:

- `query`: `str` *(required)*
- `suggester`: `str` *(required)*
- `size`: `int`

Returns a `Coroutine` for
[SuggestResponseTypeDef](./type_defs.md#suggestresponsetypedef).

<a id="upload\_documents"></a>

### upload_documents

Posts a batch of documents to a search domain for indexing.

Type annotations for
`session.create_client("cloudsearchdomain").upload_documents` method.

Boto3 documentation:
[CloudSearchDomain.Client.upload_documents](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.upload_documents)

Asynchronous method. Use `await upload_documents(...)` for a synchronous call.

Arguments mapping described in
[UploadDocumentsRequestRequestTypeDef](./type_defs.md#uploaddocumentsrequestrequesttypedef).

Keyword-only arguments:

- `documents`: `Union`\[`bytes`, `IO`\[`bytes`\], `StreamingBody`\]
  *(required)*
- `contentType`: [ContentTypeType](./literals.md#contenttypetype) *(required)*

Returns a `Coroutine` for
[UploadDocumentsResponseTypeDef](./type_defs.md#uploaddocumentsresponsetypedef).

<a id="\_\_aenter\_\_"></a>

### \_\_aenter\_\_

Type annotations for `session.create_client("cloudsearchdomain").__aenter__`
method.

Boto3 documentation:
[CloudSearchDomain.Client.\_\_aenter\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.__aenter__)

Asynchronous method. Use `await __aenter__(...)` for a synchronous call.

Returns a `Coroutine` for [CloudSearchDomainClient](#cloudsearchdomainclient).

<a id="\_\_aexit\_\_"></a>

### \_\_aexit\_\_

Type annotations for `session.create_client("cloudsearchdomain").__aexit__`
method.

Boto3 documentation:
[CloudSearchDomain.Client.\_\_aexit\_\_](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.__aexit__)

Asynchronous method. Use `await __aexit__(...)` for a synchronous call.

Arguments:

- `exc_type`: `Any` *(required)*
- `exc_val`: `Any` *(required)*
- `exc_tb`: `Any` *(required)*

Returns a `Coroutine` for `Any`.
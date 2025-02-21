# CloudSearchDomainClient

> [Index](../README.md) > [CloudSearchDomain](./README.md) > CloudSearchDomainClient

!!! note ""

    Auto-generated documentation for [CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#cloudsearchdomain)
    type annotations stubs module [types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

## CloudSearchDomainClient

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)

```python
# CloudSearchDomainClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient

session = get_session()
async with session.create_client("cloudsearchdomain") as client:
    client: CloudSearchDomainClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cloudsearchdomain").exceptions` structure.

```python
# CloudSearchDomainClient.exceptions usage example

async with session.create_client("cloudsearchdomain") as client:
    try:
        do_something(client)
    except (
            client.ClientError,
        client.DocumentServiceException,
        client.SearchException,
    ) as e:
        print(e)
```

```python
# CloudSearchDomainClient usage type checking example

from types_aiobotocore_cloudsearchdomain.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate



Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain/client/can_paginate.html)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url



Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain/client/generate_presigned_url.html)

```python
# generate_presigned_url method definition

await def generate_presigned_url(
    self,
    ClientMethod: str,
    Params: Mapping[str, Any] = ...,
    ExpiresIn: int = 3600,
    HttpMethod: str = ...,
) -> str:
    ...
```


### search

Retrieves a list of documents that match the specified search criteria.

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").search` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain/client/search.html)

```python
# search method definition

await def search(
    self,
    *,
    query: str,
    cursor: str = ...,
    expr: str = ...,
    facet: str = ...,
    filterQuery: str = ...,
    highlight: str = ...,
    partial: bool = ...,
    queryOptions: str = ...,
    queryParser: QueryParserType = ...,  # (1)
    returnFields: str = ...,
    size: int = ...,
    sort: str = ...,
    start: int = ...,
    stats: str = ...,
) -> SearchResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: QueryParserType](./literals.md#queryparsertype) 
2. See [:material-code-braces: SearchResponseTypeDef](./type_defs.md#searchresponsetypedef) 


```python
# search method usage example with argument unpacking

kwargs: SearchRequestTypeDef = {  # (1)
    "query": ...,
}

parent.search(**kwargs)
```

1. See [:material-code-braces: SearchRequestTypeDef](./type_defs.md#searchrequesttypedef) 

### suggest

Retrieves autocomplete suggestions for a partial query string.

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").suggest` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain/client/suggest.html)

```python
# suggest method definition

await def suggest(
    self,
    *,
    query: str,
    suggester: str,
    size: int = ...,
) -> SuggestResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: SuggestResponseTypeDef](./type_defs.md#suggestresponsetypedef) 


```python
# suggest method usage example with argument unpacking

kwargs: SuggestRequestTypeDef = {  # (1)
    "query": ...,
    "suggester": ...,
}

parent.suggest(**kwargs)
```

1. See [:material-code-braces: SuggestRequestTypeDef](./type_defs.md#suggestrequesttypedef) 

### upload\_documents

Posts a batch of documents to a search domain for indexing.

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").upload_documents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain/client/upload_documents.html)

```python
# upload_documents method definition

await def upload_documents(
    self,
    *,
    documents: BlobTypeDef,
    contentType: ContentTypeType,  # (1)
) -> UploadDocumentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
2. See [:material-code-braces: UploadDocumentsResponseTypeDef](./type_defs.md#uploaddocumentsresponsetypedef) 


```python
# upload_documents method usage example with argument unpacking

kwargs: UploadDocumentsRequestTypeDef = {  # (1)
    "documents": ...,
    "contentType": ...,
}

parent.upload_documents(**kwargs)
```

1. See [:material-code-braces: UploadDocumentsRequestTypeDef](./type_defs.md#uploaddocumentsrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> Self:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Union[Type[BaseException], None],
    exc_val: Union[BaseException, None],
    exc_tb: Union[TracebackType, None],
) -> None:
    ...
```






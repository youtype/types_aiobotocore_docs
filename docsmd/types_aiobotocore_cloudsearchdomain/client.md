# CloudSearchDomainClient

> [Index](../README.md) > [CloudSearchDomain](./README.md) > CloudSearchDomainClient

!!! note ""

    Auto-generated documentation for [CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
    type annotations stubs module [types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

## CloudSearchDomainClient

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client)

```python title="Usage example"
from aiobotocore.session import get_session
from types_aiobotocore_cloudsearchdomain.client import CloudSearchDomainClient

session = get_session()
async with session.create_client("cloudsearchdomain") as client:
    client: CloudSearchDomainClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("cloudsearchdomain").exceptions` structure.

```python title="Usage example"
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

```python title="Type checking example"
from types_aiobotocore_cloudsearchdomain.client import Exceptions

def handle_error(exc: Exceptions.ClientError) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.can_paginate)

```python title="Method definition"
def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.generate_presigned_url)

```python title="Method definition"
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
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.search)

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: SearchRequestRequestTypeDef = {  # (1)
    "query": ...,
}

parent.search(**kwargs)
```

1. See [:material-code-braces: SearchRequestRequestTypeDef](./type_defs.md#searchrequestrequesttypedef) 

### suggest

Retrieves autocomplete suggestions for a partial query string.

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").suggest` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.suggest)

```python title="Method definition"
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


```python title="Usage example with kwargs"
kwargs: SuggestRequestRequestTypeDef = {  # (1)
    "query": ...,
    "suggester": ...,
}

parent.suggest(**kwargs)
```

1. See [:material-code-braces: SuggestRequestRequestTypeDef](./type_defs.md#suggestrequestrequesttypedef) 

### upload\_documents

Posts a batch of documents to a search domain for indexing.

Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").upload_documents` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.upload_documents)

```python title="Method definition"
await def upload_documents(
    self,
    *,
    documents: Union[bytes, IO[bytes], StreamingBody],
    contentType: ContentTypeType,  # (1)
) -> UploadDocumentsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
2. See [:material-code-braces: UploadDocumentsResponseTypeDef](./type_defs.md#uploaddocumentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: UploadDocumentsRequestRequestTypeDef = {  # (1)
    "documents": ...,
    "contentType": ...,
}

parent.upload_documents(**kwargs)
```

1. See [:material-code-braces: UploadDocumentsRequestRequestTypeDef](./type_defs.md#uploaddocumentsrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.__aenter__)

```python title="Method definition"
await def __aenter__(
    self,
) -> CloudSearchDomainClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("cloudsearchdomain").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain.Client.__aexit__)

```python title="Method definition"
await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```






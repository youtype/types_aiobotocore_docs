# Type definitions

> [Index](../README.md) > [CloudSearchDomain](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [CloudSearchDomain](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudsearchdomain.html#CloudSearchDomain)
    type annotations stubs module [types-aiobotocore-cloudsearchdomain](https://pypi.org/project/types-aiobotocore-cloudsearchdomain/).

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




## BucketTypeDef

```python
# BucketTypeDef definition

class BucketTypeDef(TypedDict):
    value: NotRequired[str],
    count: NotRequired[int],
```

## DocumentServiceWarningTypeDef

```python
# DocumentServiceWarningTypeDef definition

class DocumentServiceWarningTypeDef(TypedDict):
    message: NotRequired[str],
```

## FieldStatsTypeDef

```python
# FieldStatsTypeDef definition

class FieldStatsTypeDef(TypedDict):
    min: NotRequired[str],
    max: NotRequired[str],
    count: NotRequired[int],
    missing: NotRequired[int],
    sum: NotRequired[float],
    sumOfSquares: NotRequired[float],
    mean: NotRequired[str],
    stddev: NotRequired[float],
```

## HitTypeDef

```python
# HitTypeDef definition

class HitTypeDef(TypedDict):
    id: NotRequired[str],
    fields: NotRequired[Dict[str, List[str]]],
    exprs: NotRequired[Dict[str, str]],
    highlights: NotRequired[Dict[str, str]],
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

## SearchRequestRequestTypeDef

```python
# SearchRequestRequestTypeDef definition

class SearchRequestRequestTypeDef(TypedDict):
    query: str,
    cursor: NotRequired[str],
    expr: NotRequired[str],
    facet: NotRequired[str],
    filterQuery: NotRequired[str],
    highlight: NotRequired[str],
    partial: NotRequired[bool],
    queryOptions: NotRequired[str],
    queryParser: NotRequired[QueryParserType],  # (1)
    returnFields: NotRequired[str],
    size: NotRequired[int],
    sort: NotRequired[str],
    start: NotRequired[int],
    stats: NotRequired[str],
```

1. See [:material-code-brackets: QueryParserType](./literals.md#queryparsertype) 
## SearchStatusTypeDef

```python
# SearchStatusTypeDef definition

class SearchStatusTypeDef(TypedDict):
    timems: NotRequired[int],
    rid: NotRequired[str],
```

## SuggestionMatchTypeDef

```python
# SuggestionMatchTypeDef definition

class SuggestionMatchTypeDef(TypedDict):
    suggestion: NotRequired[str],
    score: NotRequired[int],
    id: NotRequired[str],
```

## SuggestRequestRequestTypeDef

```python
# SuggestRequestRequestTypeDef definition

class SuggestRequestRequestTypeDef(TypedDict):
    query: str,
    suggester: str,
    size: NotRequired[int],
```

## SuggestStatusTypeDef

```python
# SuggestStatusTypeDef definition

class SuggestStatusTypeDef(TypedDict):
    timems: NotRequired[int],
    rid: NotRequired[str],
```

## UploadDocumentsRequestRequestTypeDef

```python
# UploadDocumentsRequestRequestTypeDef definition

class UploadDocumentsRequestRequestTypeDef(TypedDict):
    documents: BlobTypeDef,
    contentType: ContentTypeType,  # (1)
```

1. See [:material-code-brackets: ContentTypeType](./literals.md#contenttypetype) 
## BucketInfoTypeDef

```python
# BucketInfoTypeDef definition

class BucketInfoTypeDef(TypedDict):
    buckets: NotRequired[List[BucketTypeDef]],  # (1)
```

1. See [:material-code-braces: BucketTypeDef](./type_defs.md#buckettypedef) 
## HitsTypeDef

```python
# HitsTypeDef definition

class HitsTypeDef(TypedDict):
    found: NotRequired[int],
    start: NotRequired[int],
    cursor: NotRequired[str],
    hit: NotRequired[List[HitTypeDef]],  # (1)
```

1. See [:material-code-braces: HitTypeDef](./type_defs.md#hittypedef) 
## UploadDocumentsResponseTypeDef

```python
# UploadDocumentsResponseTypeDef definition

class UploadDocumentsResponseTypeDef(TypedDict):
    status: str,
    adds: int,
    deletes: int,
    warnings: List[DocumentServiceWarningTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DocumentServiceWarningTypeDef](./type_defs.md#documentservicewarningtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SuggestModelTypeDef

```python
# SuggestModelTypeDef definition

class SuggestModelTypeDef(TypedDict):
    query: NotRequired[str],
    found: NotRequired[int],
    suggestions: NotRequired[List[SuggestionMatchTypeDef]],  # (1)
```

1. See [:material-code-braces: SuggestionMatchTypeDef](./type_defs.md#suggestionmatchtypedef) 
## SearchResponseTypeDef

```python
# SearchResponseTypeDef definition

class SearchResponseTypeDef(TypedDict):
    status: SearchStatusTypeDef,  # (1)
    hits: HitsTypeDef,  # (2)
    facets: Dict[str, BucketInfoTypeDef],  # (3)
    stats: Dict[str, FieldStatsTypeDef],  # (4)
    ResponseMetadata: ResponseMetadataTypeDef,  # (5)
```

1. See [:material-code-braces: SearchStatusTypeDef](./type_defs.md#searchstatustypedef) 
2. See [:material-code-braces: HitsTypeDef](./type_defs.md#hitstypedef) 
3. See [:material-code-braces: BucketInfoTypeDef](./type_defs.md#bucketinfotypedef) 
4. See [:material-code-braces: FieldStatsTypeDef](./type_defs.md#fieldstatstypedef) 
5. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SuggestResponseTypeDef

```python
# SuggestResponseTypeDef definition

class SuggestResponseTypeDef(TypedDict):
    status: SuggestStatusTypeDef,  # (1)
    suggest: SuggestModelTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: SuggestStatusTypeDef](./type_defs.md#suggeststatustypedef) 
2. See [:material-code-braces: SuggestModelTypeDef](./type_defs.md#suggestmodeltypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 

# Type definitions

> [Index](../README.md) > [WorkMailMessageFlow](./README.md) > Type definitions

!!! note ""

    Auto-generated documentation for [WorkMailMessageFlow](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#workmailmessageflow)
    type annotations stubs module [types-aiobotocore-workmailmessageflow](https://pypi.org/project/types-aiobotocore-workmailmessageflow/).



## GetRawMessageContentRequestRequestTypeDef

```python
# GetRawMessageContentRequestRequestTypeDef definition

class GetRawMessageContentRequestRequestTypeDef(TypedDict):
    messageId: str,
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

## S3ReferenceTypeDef

```python
# S3ReferenceTypeDef definition

class S3ReferenceTypeDef(TypedDict):
    bucket: str,
    key: str,
    objectVersion: NotRequired[str],
```

## GetRawMessageContentResponseTypeDef

```python
# GetRawMessageContentResponseTypeDef definition

class GetRawMessageContentResponseTypeDef(TypedDict):
    messageContent: StreamingBody,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RawMessageContentTypeDef

```python
# RawMessageContentTypeDef definition

class RawMessageContentTypeDef(TypedDict):
    s3Reference: S3ReferenceTypeDef,  # (1)
```

1. See [:material-code-braces: S3ReferenceTypeDef](./type_defs.md#s3referencetypedef) 
## PutRawMessageContentRequestRequestTypeDef

```python
# PutRawMessageContentRequestRequestTypeDef definition

class PutRawMessageContentRequestRequestTypeDef(TypedDict):
    messageId: str,
    content: RawMessageContentTypeDef,  # (1)
```

1. See [:material-code-braces: RawMessageContentTypeDef](./type_defs.md#rawmessagecontenttypedef) 

# ComprehendClient

> [Index](../README.md) > [Comprehend](./README.md) > ComprehendClient

!!! note ""

    Auto-generated documentation for [Comprehend](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend)
    type annotations stubs module [types-aiobotocore-comprehend](https://pypi.org/project/types-aiobotocore-comprehend/).

## ComprehendClient

Type annotations and code completion for `#!python session.create_client("comprehend")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client)

```python
ComprehendClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_comprehend.client import ComprehendClient

session = get_session()
async with session.create_client("comprehend") as client:
    client: ComprehendClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("comprehend").exceptions` structure.

```python
ComprehendClient.exceptions usage example

async with session.create_client("comprehend") as client:
    try:
        do_something(client)
    except (
            client.BatchSizeLimitExceededException,
        client.ClientError,
        client.ConcurrentModificationException,
        client.InternalServerException,
        client.InvalidFilterException,
        client.InvalidRequestException,
        client.JobNotFoundException,
        client.KmsKeyValidationException,
        client.ResourceInUseException,
        client.ResourceLimitExceededException,
        client.ResourceNotFoundException,
        client.ResourceUnavailableException,
        client.TextSizeLimitExceededException,
        client.TooManyRequestsException,
        client.TooManyTagKeysException,
        client.TooManyTagsException,
        client.UnsupportedLanguageException,
    ) as e:
        print(e)
```

```python
ComprehendClient usage type checking example

from types_aiobotocore_comprehend.client import Exceptions

def handle_error(exc: Exceptions.BatchSizeLimitExceededException) -> None:
    ...
```


## Methods


### batch\_detect\_dominant\_language

Determines the dominant language of the input text for a batch of documents.

Type annotations and code completion for `#!python session.create_client("comprehend").batch_detect_dominant_language` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_dominant_language)

```python
# batch_detect_dominant_language method definition

await def batch_detect_dominant_language(
    self,
    *,
    TextList: Sequence[str],
) -> BatchDetectDominantLanguageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: BatchDetectDominantLanguageResponseTypeDef](./type_defs.md#batchdetectdominantlanguageresponsetypedef) 


```python
# batch_detect_dominant_language method usage example with argument unpacking

kwargs: BatchDetectDominantLanguageRequestRequestTypeDef = {  # (1)
    "TextList": ...,
}

parent.batch_detect_dominant_language(**kwargs)
```

1. See [:material-code-braces: BatchDetectDominantLanguageRequestRequestTypeDef](./type_defs.md#batchdetectdominantlanguagerequestrequesttypedef) 

### batch\_detect\_entities

Inspects the text of a batch of documents for named entities and returns
information about them.

Type annotations and code completion for `#!python session.create_client("comprehend").batch_detect_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_entities)

```python
# batch_detect_entities method definition

await def batch_detect_entities(
    self,
    *,
    TextList: Sequence[str],
    LanguageCode: LanguageCodeType,  # (1)
) -> BatchDetectEntitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: BatchDetectEntitiesResponseTypeDef](./type_defs.md#batchdetectentitiesresponsetypedef) 


```python
# batch_detect_entities method usage example with argument unpacking

kwargs: BatchDetectEntitiesRequestRequestTypeDef = {  # (1)
    "TextList": ...,
    "LanguageCode": ...,
}

parent.batch_detect_entities(**kwargs)
```

1. See [:material-code-braces: BatchDetectEntitiesRequestRequestTypeDef](./type_defs.md#batchdetectentitiesrequestrequesttypedef) 

### batch\_detect\_key\_phrases

Detects the key noun phrases found in a batch of documents.

Type annotations and code completion for `#!python session.create_client("comprehend").batch_detect_key_phrases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_key_phrases)

```python
# batch_detect_key_phrases method definition

await def batch_detect_key_phrases(
    self,
    *,
    TextList: Sequence[str],
    LanguageCode: LanguageCodeType,  # (1)
) -> BatchDetectKeyPhrasesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: BatchDetectKeyPhrasesResponseTypeDef](./type_defs.md#batchdetectkeyphrasesresponsetypedef) 


```python
# batch_detect_key_phrases method usage example with argument unpacking

kwargs: BatchDetectKeyPhrasesRequestRequestTypeDef = {  # (1)
    "TextList": ...,
    "LanguageCode": ...,
}

parent.batch_detect_key_phrases(**kwargs)
```

1. See [:material-code-braces: BatchDetectKeyPhrasesRequestRequestTypeDef](./type_defs.md#batchdetectkeyphrasesrequestrequesttypedef) 

### batch\_detect\_sentiment

Inspects a batch of documents and returns an inference of the prevailing
sentiment, `POSITIVE`, `NEUTRAL`, `MIXED`, or `NEGATIVE`, in each one.

Type annotations and code completion for `#!python session.create_client("comprehend").batch_detect_sentiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_sentiment)

```python
# batch_detect_sentiment method definition

await def batch_detect_sentiment(
    self,
    *,
    TextList: Sequence[str],
    LanguageCode: LanguageCodeType,  # (1)
) -> BatchDetectSentimentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: BatchDetectSentimentResponseTypeDef](./type_defs.md#batchdetectsentimentresponsetypedef) 


```python
# batch_detect_sentiment method usage example with argument unpacking

kwargs: BatchDetectSentimentRequestRequestTypeDef = {  # (1)
    "TextList": ...,
    "LanguageCode": ...,
}

parent.batch_detect_sentiment(**kwargs)
```

1. See [:material-code-braces: BatchDetectSentimentRequestRequestTypeDef](./type_defs.md#batchdetectsentimentrequestrequesttypedef) 

### batch\_detect\_syntax

Inspects the text of a batch of documents for the syntax and part of speech of
the words in the document and returns information about them.

Type annotations and code completion for `#!python session.create_client("comprehend").batch_detect_syntax` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_syntax)

```python
# batch_detect_syntax method definition

await def batch_detect_syntax(
    self,
    *,
    TextList: Sequence[str],
    LanguageCode: SyntaxLanguageCodeType,  # (1)
) -> BatchDetectSyntaxResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyntaxLanguageCodeType](./literals.md#syntaxlanguagecodetype) 
2. See [:material-code-braces: BatchDetectSyntaxResponseTypeDef](./type_defs.md#batchdetectsyntaxresponsetypedef) 


```python
# batch_detect_syntax method usage example with argument unpacking

kwargs: BatchDetectSyntaxRequestRequestTypeDef = {  # (1)
    "TextList": ...,
    "LanguageCode": ...,
}

parent.batch_detect_syntax(**kwargs)
```

1. See [:material-code-braces: BatchDetectSyntaxRequestRequestTypeDef](./type_defs.md#batchdetectsyntaxrequestrequesttypedef) 

### batch\_detect\_targeted\_sentiment

Inspects a batch of documents and returns a sentiment analysis for each entity
identified in the documents.

Type annotations and code completion for `#!python session.create_client("comprehend").batch_detect_targeted_sentiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.batch_detect_targeted_sentiment)

```python
# batch_detect_targeted_sentiment method definition

await def batch_detect_targeted_sentiment(
    self,
    *,
    TextList: Sequence[str],
    LanguageCode: LanguageCodeType,  # (1)
) -> BatchDetectTargetedSentimentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: BatchDetectTargetedSentimentResponseTypeDef](./type_defs.md#batchdetecttargetedsentimentresponsetypedef) 


```python
# batch_detect_targeted_sentiment method usage example with argument unpacking

kwargs: BatchDetectTargetedSentimentRequestRequestTypeDef = {  # (1)
    "TextList": ...,
    "LanguageCode": ...,
}

parent.batch_detect_targeted_sentiment(**kwargs)
```

1. See [:material-code-braces: BatchDetectTargetedSentimentRequestRequestTypeDef](./type_defs.md#batchdetecttargetedsentimentrequestrequesttypedef) 

### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("comprehend").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### classify\_document

Creates a new document classification request to analyze a single document in
real-time, using a previously created and trained custom model and an endpoint.

Type annotations and code completion for `#!python session.create_client("comprehend").classify_document` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.classify_document)

```python
# classify_document method definition

await def classify_document(
    self,
    *,
    EndpointArn: str,
    Text: str = ...,
    Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
    DocumentReaderConfig: DocumentReaderConfigTypeDef = ...,  # (1)
) -> ClassifyDocumentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentReaderConfigTypeDef](./type_defs.md#documentreaderconfigtypedef) 
2. See [:material-code-braces: ClassifyDocumentResponseTypeDef](./type_defs.md#classifydocumentresponsetypedef) 


```python
# classify_document method usage example with argument unpacking

kwargs: ClassifyDocumentRequestRequestTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.classify_document(**kwargs)
```

1. See [:material-code-braces: ClassifyDocumentRequestRequestTypeDef](./type_defs.md#classifydocumentrequestrequesttypedef) 

### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("comprehend").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### contains\_pii\_entities

Analyzes input text for the presence of personally identifiable information
(PII) and returns the labels of identified PII entity types such as name,
address, bank account number, or phone number.

Type annotations and code completion for `#!python session.create_client("comprehend").contains_pii_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.contains_pii_entities)

```python
# contains_pii_entities method definition

await def contains_pii_entities(
    self,
    *,
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
) -> ContainsPiiEntitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: ContainsPiiEntitiesResponseTypeDef](./type_defs.md#containspiientitiesresponsetypedef) 


```python
# contains_pii_entities method usage example with argument unpacking

kwargs: ContainsPiiEntitiesRequestRequestTypeDef = {  # (1)
    "Text": ...,
    "LanguageCode": ...,
}

parent.contains_pii_entities(**kwargs)
```

1. See [:material-code-braces: ContainsPiiEntitiesRequestRequestTypeDef](./type_defs.md#containspiientitiesrequestrequesttypedef) 

### create\_dataset

Creates a dataset to upload training or test data for a model associated with a
flywheel.

Type annotations and code completion for `#!python session.create_client("comprehend").create_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_dataset)

```python
# create_dataset method definition

await def create_dataset(
    self,
    *,
    FlywheelArn: str,
    DatasetName: str,
    InputDataConfig: DatasetInputDataConfigTypeDef,  # (1)
    DatasetType: DatasetTypeType = ...,  # (2)
    Description: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
) -> CreateDatasetResponseTypeDef:  # (4)
    ...
```

1. See [:material-code-braces: DatasetInputDataConfigTypeDef](./type_defs.md#datasetinputdataconfigtypedef) 
2. See [:material-code-brackets: DatasetTypeType](./literals.md#datasettypetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: CreateDatasetResponseTypeDef](./type_defs.md#createdatasetresponsetypedef) 


```python
# create_dataset method usage example with argument unpacking

kwargs: CreateDatasetRequestRequestTypeDef = {  # (1)
    "FlywheelArn": ...,
    "DatasetName": ...,
    "InputDataConfig": ...,
}

parent.create_dataset(**kwargs)
```

1. See [:material-code-braces: CreateDatasetRequestRequestTypeDef](./type_defs.md#createdatasetrequestrequesttypedef) 

### create\_document\_classifier

Creates a new document classifier that you can use to categorize documents.

Type annotations and code completion for `#!python session.create_client("comprehend").create_document_classifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_document_classifier)

```python
# create_document_classifier method definition

await def create_document_classifier(
    self,
    *,
    DocumentClassifierName: str,
    DataAccessRoleArn: str,
    InputDataConfig: DocumentClassifierInputDataConfigTypeDef,  # (1)
    LanguageCode: LanguageCodeType,  # (2)
    VersionName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    OutputDataConfig: DocumentClassifierOutputDataConfigTypeDef = ...,  # (4)
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (5)
    Mode: DocumentClassifierModeType = ...,  # (6)
    ModelKmsKeyId: str = ...,
    ModelPolicy: str = ...,
) -> CreateDocumentClassifierResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: DocumentClassifierInputDataConfigTypeDef](./type_defs.md#documentclassifierinputdataconfigtypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: DocumentClassifierOutputDataConfigTypeDef](./type_defs.md#documentclassifieroutputdataconfigtypedef) 
5. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
6. See [:material-code-brackets: DocumentClassifierModeType](./literals.md#documentclassifiermodetype) 
7. See [:material-code-braces: CreateDocumentClassifierResponseTypeDef](./type_defs.md#createdocumentclassifierresponsetypedef) 


```python
# create_document_classifier method usage example with argument unpacking

kwargs: CreateDocumentClassifierRequestRequestTypeDef = {  # (1)
    "DocumentClassifierName": ...,
    "DataAccessRoleArn": ...,
    "InputDataConfig": ...,
    "LanguageCode": ...,
}

parent.create_document_classifier(**kwargs)
```

1. See [:material-code-braces: CreateDocumentClassifierRequestRequestTypeDef](./type_defs.md#createdocumentclassifierrequestrequesttypedef) 

### create\_endpoint

Creates a model-specific endpoint for synchronous inference for a previously
trained custom model For information about endpoints, see [Managing
endpoints](https://docs.aws.amazon.com/comprehend/latest/dg/manage-
endpoints.html)_.

Type annotations and code completion for `#!python session.create_client("comprehend").create_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_endpoint)

```python
# create_endpoint method definition

await def create_endpoint(
    self,
    *,
    EndpointName: str,
    DesiredInferenceUnits: int,
    ModelArn: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
    DataAccessRoleArn: str = ...,
    FlywheelArn: str = ...,
) -> CreateEndpointResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: CreateEndpointResponseTypeDef](./type_defs.md#createendpointresponsetypedef) 


```python
# create_endpoint method usage example with argument unpacking

kwargs: CreateEndpointRequestRequestTypeDef = {  # (1)
    "EndpointName": ...,
    "DesiredInferenceUnits": ...,
}

parent.create_endpoint(**kwargs)
```

1. See [:material-code-braces: CreateEndpointRequestRequestTypeDef](./type_defs.md#createendpointrequestrequesttypedef) 

### create\_entity\_recognizer

Creates an entity recognizer using submitted files.

Type annotations and code completion for `#!python session.create_client("comprehend").create_entity_recognizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_entity_recognizer)

```python
# create_entity_recognizer method definition

await def create_entity_recognizer(
    self,
    *,
    RecognizerName: str,
    DataAccessRoleArn: str,
    InputDataConfig: EntityRecognizerInputDataConfigTypeDef,  # (1)
    LanguageCode: LanguageCodeType,  # (2)
    VersionName: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (3)
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (4)
    ModelKmsKeyId: str = ...,
    ModelPolicy: str = ...,
) -> CreateEntityRecognizerResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: EntityRecognizerInputDataConfigTypeDef](./type_defs.md#entityrecognizerinputdataconfigtypedef) 
2. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
3. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: CreateEntityRecognizerResponseTypeDef](./type_defs.md#createentityrecognizerresponsetypedef) 


```python
# create_entity_recognizer method usage example with argument unpacking

kwargs: CreateEntityRecognizerRequestRequestTypeDef = {  # (1)
    "RecognizerName": ...,
    "DataAccessRoleArn": ...,
    "InputDataConfig": ...,
    "LanguageCode": ...,
}

parent.create_entity_recognizer(**kwargs)
```

1. See [:material-code-braces: CreateEntityRecognizerRequestRequestTypeDef](./type_defs.md#createentityrecognizerrequestrequesttypedef) 

### create\_flywheel

A flywheel is an Amazon Web Services resource that orchestrates the ongoing
training of a model for custom classification or custom entity recognition.

Type annotations and code completion for `#!python session.create_client("comprehend").create_flywheel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.create_flywheel)

```python
# create_flywheel method definition

await def create_flywheel(
    self,
    *,
    FlywheelName: str,
    DataAccessRoleArn: str,
    DataLakeS3Uri: str,
    ActiveModelArn: str = ...,
    TaskConfig: TaskConfigTypeDef = ...,  # (1)
    ModelType: ModelTypeType = ...,  # (2)
    DataSecurityConfig: DataSecurityConfigTypeDef = ...,  # (3)
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> CreateFlywheelResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: TaskConfigTypeDef](./type_defs.md#taskconfigtypedef) 
2. See [:material-code-brackets: ModelTypeType](./literals.md#modeltypetype) 
3. See [:material-code-braces: DataSecurityConfigTypeDef](./type_defs.md#datasecurityconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: CreateFlywheelResponseTypeDef](./type_defs.md#createflywheelresponsetypedef) 


```python
# create_flywheel method usage example with argument unpacking

kwargs: CreateFlywheelRequestRequestTypeDef = {  # (1)
    "FlywheelName": ...,
    "DataAccessRoleArn": ...,
    "DataLakeS3Uri": ...,
}

parent.create_flywheel(**kwargs)
```

1. See [:material-code-braces: CreateFlywheelRequestRequestTypeDef](./type_defs.md#createflywheelrequestrequesttypedef) 

### delete\_document\_classifier

Deletes a previously created document classifier Only those classifiers that are
in terminated states (IN_ERROR, TRAINED) will be deleted.

Type annotations and code completion for `#!python session.create_client("comprehend").delete_document_classifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_document_classifier)

```python
# delete_document_classifier method definition

await def delete_document_classifier(
    self,
    *,
    DocumentClassifierArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_document_classifier method usage example with argument unpacking

kwargs: DeleteDocumentClassifierRequestRequestTypeDef = {  # (1)
    "DocumentClassifierArn": ...,
}

parent.delete_document_classifier(**kwargs)
```

1. See [:material-code-braces: DeleteDocumentClassifierRequestRequestTypeDef](./type_defs.md#deletedocumentclassifierrequestrequesttypedef) 

### delete\_endpoint

Deletes a model-specific endpoint for a previously-trained custom model.

Type annotations and code completion for `#!python session.create_client("comprehend").delete_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_endpoint)

```python
# delete_endpoint method definition

await def delete_endpoint(
    self,
    *,
    EndpointArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_endpoint method usage example with argument unpacking

kwargs: DeleteEndpointRequestRequestTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.delete_endpoint(**kwargs)
```

1. See [:material-code-braces: DeleteEndpointRequestRequestTypeDef](./type_defs.md#deleteendpointrequestrequesttypedef) 

### delete\_entity\_recognizer

Deletes an entity recognizer.

Type annotations and code completion for `#!python session.create_client("comprehend").delete_entity_recognizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_entity_recognizer)

```python
# delete_entity_recognizer method definition

await def delete_entity_recognizer(
    self,
    *,
    EntityRecognizerArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_entity_recognizer method usage example with argument unpacking

kwargs: DeleteEntityRecognizerRequestRequestTypeDef = {  # (1)
    "EntityRecognizerArn": ...,
}

parent.delete_entity_recognizer(**kwargs)
```

1. See [:material-code-braces: DeleteEntityRecognizerRequestRequestTypeDef](./type_defs.md#deleteentityrecognizerrequestrequesttypedef) 

### delete\_flywheel

Deletes a flywheel.

Type annotations and code completion for `#!python session.create_client("comprehend").delete_flywheel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_flywheel)

```python
# delete_flywheel method definition

await def delete_flywheel(
    self,
    *,
    FlywheelArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_flywheel method usage example with argument unpacking

kwargs: DeleteFlywheelRequestRequestTypeDef = {  # (1)
    "FlywheelArn": ...,
}

parent.delete_flywheel(**kwargs)
```

1. See [:material-code-braces: DeleteFlywheelRequestRequestTypeDef](./type_defs.md#deleteflywheelrequestrequesttypedef) 

### delete\_resource\_policy

Deletes a resource-based policy that is attached to a custom model.

Type annotations and code completion for `#!python session.create_client("comprehend").delete_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.delete_resource_policy)

```python
# delete_resource_policy method definition

await def delete_resource_policy(
    self,
    *,
    ResourceArn: str,
    PolicyRevisionId: str = ...,
) -> Dict[str, Any]:
    ...
```



```python
# delete_resource_policy method usage example with argument unpacking

kwargs: DeleteResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.delete_resource_policy(**kwargs)
```

1. See [:material-code-braces: DeleteResourcePolicyRequestRequestTypeDef](./type_defs.md#deleteresourcepolicyrequestrequesttypedef) 

### describe\_dataset

Returns information about the dataset that you specify.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_dataset` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_dataset)

```python
# describe_dataset method definition

await def describe_dataset(
    self,
    *,
    DatasetArn: str,
) -> DescribeDatasetResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDatasetResponseTypeDef](./type_defs.md#describedatasetresponsetypedef) 


```python
# describe_dataset method usage example with argument unpacking

kwargs: DescribeDatasetRequestRequestTypeDef = {  # (1)
    "DatasetArn": ...,
}

parent.describe_dataset(**kwargs)
```

1. See [:material-code-braces: DescribeDatasetRequestRequestTypeDef](./type_defs.md#describedatasetrequestrequesttypedef) 

### describe\_document\_classification\_job

Gets the properties associated with a document classification job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_document_classification_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_document_classification_job)

```python
# describe_document_classification_job method definition

await def describe_document_classification_job(
    self,
    *,
    JobId: str,
) -> DescribeDocumentClassificationJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDocumentClassificationJobResponseTypeDef](./type_defs.md#describedocumentclassificationjobresponsetypedef) 


```python
# describe_document_classification_job method usage example with argument unpacking

kwargs: DescribeDocumentClassificationJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_document_classification_job(**kwargs)
```

1. See [:material-code-braces: DescribeDocumentClassificationJobRequestRequestTypeDef](./type_defs.md#describedocumentclassificationjobrequestrequesttypedef) 

### describe\_document\_classifier

Gets the properties associated with a document classifier.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_document_classifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_document_classifier)

```python
# describe_document_classifier method definition

await def describe_document_classifier(
    self,
    *,
    DocumentClassifierArn: str,
) -> DescribeDocumentClassifierResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDocumentClassifierResponseTypeDef](./type_defs.md#describedocumentclassifierresponsetypedef) 


```python
# describe_document_classifier method usage example with argument unpacking

kwargs: DescribeDocumentClassifierRequestRequestTypeDef = {  # (1)
    "DocumentClassifierArn": ...,
}

parent.describe_document_classifier(**kwargs)
```

1. See [:material-code-braces: DescribeDocumentClassifierRequestRequestTypeDef](./type_defs.md#describedocumentclassifierrequestrequesttypedef) 

### describe\_dominant\_language\_detection\_job

Gets the properties associated with a dominant language detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_dominant_language_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_dominant_language_detection_job)

```python
# describe_dominant_language_detection_job method definition

await def describe_dominant_language_detection_job(
    self,
    *,
    JobId: str,
) -> DescribeDominantLanguageDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeDominantLanguageDetectionJobResponseTypeDef](./type_defs.md#describedominantlanguagedetectionjobresponsetypedef) 


```python
# describe_dominant_language_detection_job method usage example with argument unpacking

kwargs: DescribeDominantLanguageDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_dominant_language_detection_job(**kwargs)
```

1. See [:material-code-braces: DescribeDominantLanguageDetectionJobRequestRequestTypeDef](./type_defs.md#describedominantlanguagedetectionjobrequestrequesttypedef) 

### describe\_endpoint

Gets the properties associated with a specific endpoint.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_endpoint)

```python
# describe_endpoint method definition

await def describe_endpoint(
    self,
    *,
    EndpointArn: str,
) -> DescribeEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEndpointResponseTypeDef](./type_defs.md#describeendpointresponsetypedef) 


```python
# describe_endpoint method usage example with argument unpacking

kwargs: DescribeEndpointRequestRequestTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.describe_endpoint(**kwargs)
```

1. See [:material-code-braces: DescribeEndpointRequestRequestTypeDef](./type_defs.md#describeendpointrequestrequesttypedef) 

### describe\_entities\_detection\_job

Gets the properties associated with an entities detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_entities_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_entities_detection_job)

```python
# describe_entities_detection_job method definition

await def describe_entities_detection_job(
    self,
    *,
    JobId: str,
) -> DescribeEntitiesDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEntitiesDetectionJobResponseTypeDef](./type_defs.md#describeentitiesdetectionjobresponsetypedef) 


```python
# describe_entities_detection_job method usage example with argument unpacking

kwargs: DescribeEntitiesDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_entities_detection_job(**kwargs)
```

1. See [:material-code-braces: DescribeEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#describeentitiesdetectionjobrequestrequesttypedef) 

### describe\_entity\_recognizer

Provides details about an entity recognizer including status, S3 buckets
containing training data, recognizer metadata, metrics, and so on.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_entity_recognizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_entity_recognizer)

```python
# describe_entity_recognizer method definition

await def describe_entity_recognizer(
    self,
    *,
    EntityRecognizerArn: str,
) -> DescribeEntityRecognizerResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEntityRecognizerResponseTypeDef](./type_defs.md#describeentityrecognizerresponsetypedef) 


```python
# describe_entity_recognizer method usage example with argument unpacking

kwargs: DescribeEntityRecognizerRequestRequestTypeDef = {  # (1)
    "EntityRecognizerArn": ...,
}

parent.describe_entity_recognizer(**kwargs)
```

1. See [:material-code-braces: DescribeEntityRecognizerRequestRequestTypeDef](./type_defs.md#describeentityrecognizerrequestrequesttypedef) 

### describe\_events\_detection\_job

Gets the status and details of an events detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_events_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_events_detection_job)

```python
# describe_events_detection_job method definition

await def describe_events_detection_job(
    self,
    *,
    JobId: str,
) -> DescribeEventsDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeEventsDetectionJobResponseTypeDef](./type_defs.md#describeeventsdetectionjobresponsetypedef) 


```python
# describe_events_detection_job method usage example with argument unpacking

kwargs: DescribeEventsDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_events_detection_job(**kwargs)
```

1. See [:material-code-braces: DescribeEventsDetectionJobRequestRequestTypeDef](./type_defs.md#describeeventsdetectionjobrequestrequesttypedef) 

### describe\_flywheel

Provides configuration information about the flywheel.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_flywheel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_flywheel)

```python
# describe_flywheel method definition

await def describe_flywheel(
    self,
    *,
    FlywheelArn: str,
) -> DescribeFlywheelResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFlywheelResponseTypeDef](./type_defs.md#describeflywheelresponsetypedef) 


```python
# describe_flywheel method usage example with argument unpacking

kwargs: DescribeFlywheelRequestRequestTypeDef = {  # (1)
    "FlywheelArn": ...,
}

parent.describe_flywheel(**kwargs)
```

1. See [:material-code-braces: DescribeFlywheelRequestRequestTypeDef](./type_defs.md#describeflywheelrequestrequesttypedef) 

### describe\_flywheel\_iteration

Retrieve the configuration properties of a flywheel iteration.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_flywheel_iteration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_flywheel_iteration)

```python
# describe_flywheel_iteration method definition

await def describe_flywheel_iteration(
    self,
    *,
    FlywheelArn: str,
    FlywheelIterationId: str,
) -> DescribeFlywheelIterationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeFlywheelIterationResponseTypeDef](./type_defs.md#describeflywheeliterationresponsetypedef) 


```python
# describe_flywheel_iteration method usage example with argument unpacking

kwargs: DescribeFlywheelIterationRequestRequestTypeDef = {  # (1)
    "FlywheelArn": ...,
    "FlywheelIterationId": ...,
}

parent.describe_flywheel_iteration(**kwargs)
```

1. See [:material-code-braces: DescribeFlywheelIterationRequestRequestTypeDef](./type_defs.md#describeflywheeliterationrequestrequesttypedef) 

### describe\_key\_phrases\_detection\_job

Gets the properties associated with a key phrases detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_key_phrases_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_key_phrases_detection_job)

```python
# describe_key_phrases_detection_job method definition

await def describe_key_phrases_detection_job(
    self,
    *,
    JobId: str,
) -> DescribeKeyPhrasesDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeKeyPhrasesDetectionJobResponseTypeDef](./type_defs.md#describekeyphrasesdetectionjobresponsetypedef) 


```python
# describe_key_phrases_detection_job method usage example with argument unpacking

kwargs: DescribeKeyPhrasesDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_key_phrases_detection_job(**kwargs)
```

1. See [:material-code-braces: DescribeKeyPhrasesDetectionJobRequestRequestTypeDef](./type_defs.md#describekeyphrasesdetectionjobrequestrequesttypedef) 

### describe\_pii\_entities\_detection\_job

Gets the properties associated with a PII entities detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_pii_entities_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_pii_entities_detection_job)

```python
# describe_pii_entities_detection_job method definition

await def describe_pii_entities_detection_job(
    self,
    *,
    JobId: str,
) -> DescribePiiEntitiesDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribePiiEntitiesDetectionJobResponseTypeDef](./type_defs.md#describepiientitiesdetectionjobresponsetypedef) 


```python
# describe_pii_entities_detection_job method usage example with argument unpacking

kwargs: DescribePiiEntitiesDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_pii_entities_detection_job(**kwargs)
```

1. See [:material-code-braces: DescribePiiEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#describepiientitiesdetectionjobrequestrequesttypedef) 

### describe\_resource\_policy

Gets the details of a resource-based policy that is attached to a custom model,
including the JSON body of the policy.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_resource_policy)

```python
# describe_resource_policy method definition

await def describe_resource_policy(
    self,
    *,
    ResourceArn: str,
) -> DescribeResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeResourcePolicyResponseTypeDef](./type_defs.md#describeresourcepolicyresponsetypedef) 


```python
# describe_resource_policy method usage example with argument unpacking

kwargs: DescribeResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.describe_resource_policy(**kwargs)
```

1. See [:material-code-braces: DescribeResourcePolicyRequestRequestTypeDef](./type_defs.md#describeresourcepolicyrequestrequesttypedef) 

### describe\_sentiment\_detection\_job

Gets the properties associated with a sentiment detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_sentiment_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_sentiment_detection_job)

```python
# describe_sentiment_detection_job method definition

await def describe_sentiment_detection_job(
    self,
    *,
    JobId: str,
) -> DescribeSentimentDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeSentimentDetectionJobResponseTypeDef](./type_defs.md#describesentimentdetectionjobresponsetypedef) 


```python
# describe_sentiment_detection_job method usage example with argument unpacking

kwargs: DescribeSentimentDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_sentiment_detection_job(**kwargs)
```

1. See [:material-code-braces: DescribeSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#describesentimentdetectionjobrequestrequesttypedef) 

### describe\_targeted\_sentiment\_detection\_job

Gets the properties associated with a targeted sentiment detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_targeted_sentiment_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_targeted_sentiment_detection_job)

```python
# describe_targeted_sentiment_detection_job method definition

await def describe_targeted_sentiment_detection_job(
    self,
    *,
    JobId: str,
) -> DescribeTargetedSentimentDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTargetedSentimentDetectionJobResponseTypeDef](./type_defs.md#describetargetedsentimentdetectionjobresponsetypedef) 


```python
# describe_targeted_sentiment_detection_job method usage example with argument unpacking

kwargs: DescribeTargetedSentimentDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_targeted_sentiment_detection_job(**kwargs)
```

1. See [:material-code-braces: DescribeTargetedSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#describetargetedsentimentdetectionjobrequestrequesttypedef) 

### describe\_topics\_detection\_job

Gets the properties associated with a topic detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").describe_topics_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.describe_topics_detection_job)

```python
# describe_topics_detection_job method definition

await def describe_topics_detection_job(
    self,
    *,
    JobId: str,
) -> DescribeTopicsDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DescribeTopicsDetectionJobResponseTypeDef](./type_defs.md#describetopicsdetectionjobresponsetypedef) 


```python
# describe_topics_detection_job method usage example with argument unpacking

kwargs: DescribeTopicsDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.describe_topics_detection_job(**kwargs)
```

1. See [:material-code-braces: DescribeTopicsDetectionJobRequestRequestTypeDef](./type_defs.md#describetopicsdetectionjobrequestrequesttypedef) 

### detect\_dominant\_language

Determines the dominant language of the input text.

Type annotations and code completion for `#!python session.create_client("comprehend").detect_dominant_language` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_dominant_language)

```python
# detect_dominant_language method definition

await def detect_dominant_language(
    self,
    *,
    Text: str,
) -> DetectDominantLanguageResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: DetectDominantLanguageResponseTypeDef](./type_defs.md#detectdominantlanguageresponsetypedef) 


```python
# detect_dominant_language method usage example with argument unpacking

kwargs: DetectDominantLanguageRequestRequestTypeDef = {  # (1)
    "Text": ...,
}

parent.detect_dominant_language(**kwargs)
```

1. See [:material-code-braces: DetectDominantLanguageRequestRequestTypeDef](./type_defs.md#detectdominantlanguagerequestrequesttypedef) 

### detect\_entities

Detects named entities in input text when you use the pre-trained model.

Type annotations and code completion for `#!python session.create_client("comprehend").detect_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_entities)

```python
# detect_entities method definition

await def detect_entities(
    self,
    *,
    Text: str = ...,
    LanguageCode: LanguageCodeType = ...,  # (1)
    EndpointArn: str = ...,
    Bytes: Union[str, bytes, IO[Any], StreamingBody] = ...,
    DocumentReaderConfig: DocumentReaderConfigTypeDef = ...,  # (2)
) -> DetectEntitiesResponseTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: DocumentReaderConfigTypeDef](./type_defs.md#documentreaderconfigtypedef) 
3. See [:material-code-braces: DetectEntitiesResponseTypeDef](./type_defs.md#detectentitiesresponsetypedef) 


```python
# detect_entities method usage example with argument unpacking

kwargs: DetectEntitiesRequestRequestTypeDef = {  # (1)
    "Text": ...,
}

parent.detect_entities(**kwargs)
```

1. See [:material-code-braces: DetectEntitiesRequestRequestTypeDef](./type_defs.md#detectentitiesrequestrequesttypedef) 

### detect\_key\_phrases

Detects the key noun phrases found in the text.

Type annotations and code completion for `#!python session.create_client("comprehend").detect_key_phrases` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_key_phrases)

```python
# detect_key_phrases method definition

await def detect_key_phrases(
    self,
    *,
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
) -> DetectKeyPhrasesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: DetectKeyPhrasesResponseTypeDef](./type_defs.md#detectkeyphrasesresponsetypedef) 


```python
# detect_key_phrases method usage example with argument unpacking

kwargs: DetectKeyPhrasesRequestRequestTypeDef = {  # (1)
    "Text": ...,
    "LanguageCode": ...,
}

parent.detect_key_phrases(**kwargs)
```

1. See [:material-code-braces: DetectKeyPhrasesRequestRequestTypeDef](./type_defs.md#detectkeyphrasesrequestrequesttypedef) 

### detect\_pii\_entities

Inspects the input text for entities that contain personally identifiable
information (PII) and returns information about them.

Type annotations and code completion for `#!python session.create_client("comprehend").detect_pii_entities` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_pii_entities)

```python
# detect_pii_entities method definition

await def detect_pii_entities(
    self,
    *,
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
) -> DetectPiiEntitiesResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: DetectPiiEntitiesResponseTypeDef](./type_defs.md#detectpiientitiesresponsetypedef) 


```python
# detect_pii_entities method usage example with argument unpacking

kwargs: DetectPiiEntitiesRequestRequestTypeDef = {  # (1)
    "Text": ...,
    "LanguageCode": ...,
}

parent.detect_pii_entities(**kwargs)
```

1. See [:material-code-braces: DetectPiiEntitiesRequestRequestTypeDef](./type_defs.md#detectpiientitiesrequestrequesttypedef) 

### detect\_sentiment

Inspects text and returns an inference of the prevailing sentiment ( `POSITIVE`,
`NEUTRAL`, `MIXED`, or `NEGATIVE`).

Type annotations and code completion for `#!python session.create_client("comprehend").detect_sentiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_sentiment)

```python
# detect_sentiment method definition

await def detect_sentiment(
    self,
    *,
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
) -> DetectSentimentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: DetectSentimentResponseTypeDef](./type_defs.md#detectsentimentresponsetypedef) 


```python
# detect_sentiment method usage example with argument unpacking

kwargs: DetectSentimentRequestRequestTypeDef = {  # (1)
    "Text": ...,
    "LanguageCode": ...,
}

parent.detect_sentiment(**kwargs)
```

1. See [:material-code-braces: DetectSentimentRequestRequestTypeDef](./type_defs.md#detectsentimentrequestrequesttypedef) 

### detect\_syntax

Inspects text for syntax and the part of speech of words in the document.

Type annotations and code completion for `#!python session.create_client("comprehend").detect_syntax` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_syntax)

```python
# detect_syntax method definition

await def detect_syntax(
    self,
    *,
    Text: str,
    LanguageCode: SyntaxLanguageCodeType,  # (1)
) -> DetectSyntaxResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SyntaxLanguageCodeType](./literals.md#syntaxlanguagecodetype) 
2. See [:material-code-braces: DetectSyntaxResponseTypeDef](./type_defs.md#detectsyntaxresponsetypedef) 


```python
# detect_syntax method usage example with argument unpacking

kwargs: DetectSyntaxRequestRequestTypeDef = {  # (1)
    "Text": ...,
    "LanguageCode": ...,
}

parent.detect_syntax(**kwargs)
```

1. See [:material-code-braces: DetectSyntaxRequestRequestTypeDef](./type_defs.md#detectsyntaxrequestrequesttypedef) 

### detect\_targeted\_sentiment

Inspects the input text and returns a sentiment analysis for each entity
identified in the text.

Type annotations and code completion for `#!python session.create_client("comprehend").detect_targeted_sentiment` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.detect_targeted_sentiment)

```python
# detect_targeted_sentiment method definition

await def detect_targeted_sentiment(
    self,
    *,
    Text: str,
    LanguageCode: LanguageCodeType,  # (1)
) -> DetectTargetedSentimentResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
2. See [:material-code-braces: DetectTargetedSentimentResponseTypeDef](./type_defs.md#detecttargetedsentimentresponsetypedef) 


```python
# detect_targeted_sentiment method usage example with argument unpacking

kwargs: DetectTargetedSentimentRequestRequestTypeDef = {  # (1)
    "Text": ...,
    "LanguageCode": ...,
}

parent.detect_targeted_sentiment(**kwargs)
```

1. See [:material-code-braces: DetectTargetedSentimentRequestRequestTypeDef](./type_defs.md#detecttargetedsentimentrequestrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("comprehend").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.generate_presigned_url)

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


### import\_model

Creates a new custom model that replicates a source custom model that you
import.

Type annotations and code completion for `#!python session.create_client("comprehend").import_model` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.import_model)

```python
# import_model method definition

await def import_model(
    self,
    *,
    SourceModelArn: str,
    ModelName: str = ...,
    VersionName: str = ...,
    ModelKmsKeyId: str = ...,
    DataAccessRoleArn: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (1)
) -> ImportModelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ImportModelResponseTypeDef](./type_defs.md#importmodelresponsetypedef) 


```python
# import_model method usage example with argument unpacking

kwargs: ImportModelRequestRequestTypeDef = {  # (1)
    "SourceModelArn": ...,
}

parent.import_model(**kwargs)
```

1. See [:material-code-braces: ImportModelRequestRequestTypeDef](./type_defs.md#importmodelrequestrequesttypedef) 

### list\_datasets

List the datasets that you have configured in this Region.

Type annotations and code completion for `#!python session.create_client("comprehend").list_datasets` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_datasets)

```python
# list_datasets method definition

await def list_datasets(
    self,
    *,
    FlywheelArn: str = ...,
    Filter: DatasetFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDatasetsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DatasetFilterTypeDef](./type_defs.md#datasetfiltertypedef) 
2. See [:material-code-braces: ListDatasetsResponseTypeDef](./type_defs.md#listdatasetsresponsetypedef) 


```python
# list_datasets method usage example with argument unpacking

kwargs: ListDatasetsRequestRequestTypeDef = {  # (1)
    "FlywheelArn": ...,
}

parent.list_datasets(**kwargs)
```

1. See [:material-code-braces: ListDatasetsRequestRequestTypeDef](./type_defs.md#listdatasetsrequestrequesttypedef) 

### list\_document\_classification\_jobs

Gets a list of the documentation classification jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_document_classification_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classification_jobs)

```python
# list_document_classification_jobs method definition

await def list_document_classification_jobs(
    self,
    *,
    Filter: DocumentClassificationJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDocumentClassificationJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentClassificationJobFilterTypeDef](./type_defs.md#documentclassificationjobfiltertypedef) 
2. See [:material-code-braces: ListDocumentClassificationJobsResponseTypeDef](./type_defs.md#listdocumentclassificationjobsresponsetypedef) 


```python
# list_document_classification_jobs method usage example with argument unpacking

kwargs: ListDocumentClassificationJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_document_classification_jobs(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassificationJobsRequestRequestTypeDef](./type_defs.md#listdocumentclassificationjobsrequestrequesttypedef) 

### list\_document\_classifier\_summaries

Gets a list of summaries of the document classifiers that you have created See
also: [AWS API
Documentation](https://docs.aws.amazon.com/goto/WebAPI/comprehend-2017-11-27/ListDocumentClassifierSummaries).

Type annotations and code completion for `#!python session.create_client("comprehend").list_document_classifier_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifier_summaries)

```python
# list_document_classifier_summaries method definition

await def list_document_classifier_summaries(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDocumentClassifierSummariesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListDocumentClassifierSummariesResponseTypeDef](./type_defs.md#listdocumentclassifiersummariesresponsetypedef) 


```python
# list_document_classifier_summaries method usage example with argument unpacking

kwargs: ListDocumentClassifierSummariesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_document_classifier_summaries(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassifierSummariesRequestRequestTypeDef](./type_defs.md#listdocumentclassifiersummariesrequestrequesttypedef) 

### list\_document\_classifiers

Gets a list of the document classifiers that you have created.

Type annotations and code completion for `#!python session.create_client("comprehend").list_document_classifiers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_document_classifiers)

```python
# list_document_classifiers method definition

await def list_document_classifiers(
    self,
    *,
    Filter: DocumentClassifierFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDocumentClassifiersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DocumentClassifierFilterTypeDef](./type_defs.md#documentclassifierfiltertypedef) 
2. See [:material-code-braces: ListDocumentClassifiersResponseTypeDef](./type_defs.md#listdocumentclassifiersresponsetypedef) 


```python
# list_document_classifiers method usage example with argument unpacking

kwargs: ListDocumentClassifiersRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_document_classifiers(**kwargs)
```

1. See [:material-code-braces: ListDocumentClassifiersRequestRequestTypeDef](./type_defs.md#listdocumentclassifiersrequestrequesttypedef) 

### list\_dominant\_language\_detection\_jobs

Gets a list of the dominant language detection jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_dominant_language_detection_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_dominant_language_detection_jobs)

```python
# list_dominant_language_detection_jobs method definition

await def list_dominant_language_detection_jobs(
    self,
    *,
    Filter: DominantLanguageDetectionJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListDominantLanguageDetectionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: DominantLanguageDetectionJobFilterTypeDef](./type_defs.md#dominantlanguagedetectionjobfiltertypedef) 
2. See [:material-code-braces: ListDominantLanguageDetectionJobsResponseTypeDef](./type_defs.md#listdominantlanguagedetectionjobsresponsetypedef) 


```python
# list_dominant_language_detection_jobs method usage example with argument unpacking

kwargs: ListDominantLanguageDetectionJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_dominant_language_detection_jobs(**kwargs)
```

1. See [:material-code-braces: ListDominantLanguageDetectionJobsRequestRequestTypeDef](./type_defs.md#listdominantlanguagedetectionjobsrequestrequesttypedef) 

### list\_endpoints

Gets a list of all existing endpoints that you've created.

Type annotations and code completion for `#!python session.create_client("comprehend").list_endpoints` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_endpoints)

```python
# list_endpoints method definition

await def list_endpoints(
    self,
    *,
    Filter: EndpointFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEndpointsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EndpointFilterTypeDef](./type_defs.md#endpointfiltertypedef) 
2. See [:material-code-braces: ListEndpointsResponseTypeDef](./type_defs.md#listendpointsresponsetypedef) 


```python
# list_endpoints method usage example with argument unpacking

kwargs: ListEndpointsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_endpoints(**kwargs)
```

1. See [:material-code-braces: ListEndpointsRequestRequestTypeDef](./type_defs.md#listendpointsrequestrequesttypedef) 

### list\_entities\_detection\_jobs

Gets a list of the entity detection jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_entities_detection_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entities_detection_jobs)

```python
# list_entities_detection_jobs method definition

await def list_entities_detection_jobs(
    self,
    *,
    Filter: EntitiesDetectionJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEntitiesDetectionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EntitiesDetectionJobFilterTypeDef](./type_defs.md#entitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: ListEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listentitiesdetectionjobsresponsetypedef) 


```python
# list_entities_detection_jobs method usage example with argument unpacking

kwargs: ListEntitiesDetectionJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_entities_detection_jobs(**kwargs)
```

1. See [:material-code-braces: ListEntitiesDetectionJobsRequestRequestTypeDef](./type_defs.md#listentitiesdetectionjobsrequestrequesttypedef) 

### list\_entity\_recognizer\_summaries

Gets a list of summaries for the entity recognizers that you have created.

Type annotations and code completion for `#!python session.create_client("comprehend").list_entity_recognizer_summaries` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entity_recognizer_summaries)

```python
# list_entity_recognizer_summaries method definition

await def list_entity_recognizer_summaries(
    self,
    *,
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEntityRecognizerSummariesResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListEntityRecognizerSummariesResponseTypeDef](./type_defs.md#listentityrecognizersummariesresponsetypedef) 


```python
# list_entity_recognizer_summaries method usage example with argument unpacking

kwargs: ListEntityRecognizerSummariesRequestRequestTypeDef = {  # (1)
    "NextToken": ...,
}

parent.list_entity_recognizer_summaries(**kwargs)
```

1. See [:material-code-braces: ListEntityRecognizerSummariesRequestRequestTypeDef](./type_defs.md#listentityrecognizersummariesrequestrequesttypedef) 

### list\_entity\_recognizers

Gets a list of the properties of all entity recognizers that you created,
including recognizers currently in training.

Type annotations and code completion for `#!python session.create_client("comprehend").list_entity_recognizers` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_entity_recognizers)

```python
# list_entity_recognizers method definition

await def list_entity_recognizers(
    self,
    *,
    Filter: EntityRecognizerFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEntityRecognizersResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EntityRecognizerFilterTypeDef](./type_defs.md#entityrecognizerfiltertypedef) 
2. See [:material-code-braces: ListEntityRecognizersResponseTypeDef](./type_defs.md#listentityrecognizersresponsetypedef) 


```python
# list_entity_recognizers method usage example with argument unpacking

kwargs: ListEntityRecognizersRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_entity_recognizers(**kwargs)
```

1. See [:material-code-braces: ListEntityRecognizersRequestRequestTypeDef](./type_defs.md#listentityrecognizersrequestrequesttypedef) 

### list\_events\_detection\_jobs

Gets a list of the events detection jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_events_detection_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_events_detection_jobs)

```python
# list_events_detection_jobs method definition

await def list_events_detection_jobs(
    self,
    *,
    Filter: EventsDetectionJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListEventsDetectionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: EventsDetectionJobFilterTypeDef](./type_defs.md#eventsdetectionjobfiltertypedef) 
2. See [:material-code-braces: ListEventsDetectionJobsResponseTypeDef](./type_defs.md#listeventsdetectionjobsresponsetypedef) 


```python
# list_events_detection_jobs method usage example with argument unpacking

kwargs: ListEventsDetectionJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_events_detection_jobs(**kwargs)
```

1. See [:material-code-braces: ListEventsDetectionJobsRequestRequestTypeDef](./type_defs.md#listeventsdetectionjobsrequestrequesttypedef) 

### list\_flywheel\_iteration\_history

Information about the history of a flywheel iteration.

Type annotations and code completion for `#!python session.create_client("comprehend").list_flywheel_iteration_history` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_flywheel_iteration_history)

```python
# list_flywheel_iteration_history method definition

await def list_flywheel_iteration_history(
    self,
    *,
    FlywheelArn: str,
    Filter: FlywheelIterationFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFlywheelIterationHistoryResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FlywheelIterationFilterTypeDef](./type_defs.md#flywheeliterationfiltertypedef) 
2. See [:material-code-braces: ListFlywheelIterationHistoryResponseTypeDef](./type_defs.md#listflywheeliterationhistoryresponsetypedef) 


```python
# list_flywheel_iteration_history method usage example with argument unpacking

kwargs: ListFlywheelIterationHistoryRequestRequestTypeDef = {  # (1)
    "FlywheelArn": ...,
}

parent.list_flywheel_iteration_history(**kwargs)
```

1. See [:material-code-braces: ListFlywheelIterationHistoryRequestRequestTypeDef](./type_defs.md#listflywheeliterationhistoryrequestrequesttypedef) 

### list\_flywheels

Gets a list of the flywheels that you have created.

Type annotations and code completion for `#!python session.create_client("comprehend").list_flywheels` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_flywheels)

```python
# list_flywheels method definition

await def list_flywheels(
    self,
    *,
    Filter: FlywheelFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListFlywheelsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: FlywheelFilterTypeDef](./type_defs.md#flywheelfiltertypedef) 
2. See [:material-code-braces: ListFlywheelsResponseTypeDef](./type_defs.md#listflywheelsresponsetypedef) 


```python
# list_flywheels method usage example with argument unpacking

kwargs: ListFlywheelsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_flywheels(**kwargs)
```

1. See [:material-code-braces: ListFlywheelsRequestRequestTypeDef](./type_defs.md#listflywheelsrequestrequesttypedef) 

### list\_key\_phrases\_detection\_jobs

Get a list of key phrase detection jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_key_phrases_detection_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_key_phrases_detection_jobs)

```python
# list_key_phrases_detection_jobs method definition

await def list_key_phrases_detection_jobs(
    self,
    *,
    Filter: KeyPhrasesDetectionJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListKeyPhrasesDetectionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: KeyPhrasesDetectionJobFilterTypeDef](./type_defs.md#keyphrasesdetectionjobfiltertypedef) 
2. See [:material-code-braces: ListKeyPhrasesDetectionJobsResponseTypeDef](./type_defs.md#listkeyphrasesdetectionjobsresponsetypedef) 


```python
# list_key_phrases_detection_jobs method usage example with argument unpacking

kwargs: ListKeyPhrasesDetectionJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_key_phrases_detection_jobs(**kwargs)
```

1. See [:material-code-braces: ListKeyPhrasesDetectionJobsRequestRequestTypeDef](./type_defs.md#listkeyphrasesdetectionjobsrequestrequesttypedef) 

### list\_pii\_entities\_detection\_jobs

Gets a list of the PII entity detection jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_pii_entities_detection_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_pii_entities_detection_jobs)

```python
# list_pii_entities_detection_jobs method definition

await def list_pii_entities_detection_jobs(
    self,
    *,
    Filter: PiiEntitiesDetectionJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListPiiEntitiesDetectionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: PiiEntitiesDetectionJobFilterTypeDef](./type_defs.md#piientitiesdetectionjobfiltertypedef) 
2. See [:material-code-braces: ListPiiEntitiesDetectionJobsResponseTypeDef](./type_defs.md#listpiientitiesdetectionjobsresponsetypedef) 


```python
# list_pii_entities_detection_jobs method usage example with argument unpacking

kwargs: ListPiiEntitiesDetectionJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_pii_entities_detection_jobs(**kwargs)
```

1. See [:material-code-braces: ListPiiEntitiesDetectionJobsRequestRequestTypeDef](./type_defs.md#listpiientitiesdetectionjobsrequestrequesttypedef) 

### list\_sentiment\_detection\_jobs

Gets a list of sentiment detection jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_sentiment_detection_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_sentiment_detection_jobs)

```python
# list_sentiment_detection_jobs method definition

await def list_sentiment_detection_jobs(
    self,
    *,
    Filter: SentimentDetectionJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListSentimentDetectionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: SentimentDetectionJobFilterTypeDef](./type_defs.md#sentimentdetectionjobfiltertypedef) 
2. See [:material-code-braces: ListSentimentDetectionJobsResponseTypeDef](./type_defs.md#listsentimentdetectionjobsresponsetypedef) 


```python
# list_sentiment_detection_jobs method usage example with argument unpacking

kwargs: ListSentimentDetectionJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_sentiment_detection_jobs(**kwargs)
```

1. See [:material-code-braces: ListSentimentDetectionJobsRequestRequestTypeDef](./type_defs.md#listsentimentdetectionjobsrequestrequesttypedef) 

### list\_tags\_for\_resource

Lists all tags associated with a given Amazon Comprehend resource.

Type annotations and code completion for `#!python session.create_client("comprehend").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_tags_for_resource)

```python
# list_tags_for_resource method definition

await def list_tags_for_resource(
    self,
    *,
    ResourceArn: str,
) -> ListTagsForResourceResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# list_tags_for_resource method usage example with argument unpacking

kwargs: ListTagsForResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.list_tags_for_resource(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef) 

### list\_targeted\_sentiment\_detection\_jobs

Gets a list of targeted sentiment detection jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_targeted_sentiment_detection_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_targeted_sentiment_detection_jobs)

```python
# list_targeted_sentiment_detection_jobs method definition

await def list_targeted_sentiment_detection_jobs(
    self,
    *,
    Filter: TargetedSentimentDetectionJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTargetedSentimentDetectionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TargetedSentimentDetectionJobFilterTypeDef](./type_defs.md#targetedsentimentdetectionjobfiltertypedef) 
2. See [:material-code-braces: ListTargetedSentimentDetectionJobsResponseTypeDef](./type_defs.md#listtargetedsentimentdetectionjobsresponsetypedef) 


```python
# list_targeted_sentiment_detection_jobs method usage example with argument unpacking

kwargs: ListTargetedSentimentDetectionJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_targeted_sentiment_detection_jobs(**kwargs)
```

1. See [:material-code-braces: ListTargetedSentimentDetectionJobsRequestRequestTypeDef](./type_defs.md#listtargetedsentimentdetectionjobsrequestrequesttypedef) 

### list\_topics\_detection\_jobs

Gets a list of the topic detection jobs that you have submitted.

Type annotations and code completion for `#!python session.create_client("comprehend").list_topics_detection_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.list_topics_detection_jobs)

```python
# list_topics_detection_jobs method definition

await def list_topics_detection_jobs(
    self,
    *,
    Filter: TopicsDetectionJobFilterTypeDef = ...,  # (1)
    NextToken: str = ...,
    MaxResults: int = ...,
) -> ListTopicsDetectionJobsResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: TopicsDetectionJobFilterTypeDef](./type_defs.md#topicsdetectionjobfiltertypedef) 
2. See [:material-code-braces: ListTopicsDetectionJobsResponseTypeDef](./type_defs.md#listtopicsdetectionjobsresponsetypedef) 


```python
# list_topics_detection_jobs method usage example with argument unpacking

kwargs: ListTopicsDetectionJobsRequestRequestTypeDef = {  # (1)
    "Filter": ...,
}

parent.list_topics_detection_jobs(**kwargs)
```

1. See [:material-code-braces: ListTopicsDetectionJobsRequestRequestTypeDef](./type_defs.md#listtopicsdetectionjobsrequestrequesttypedef) 

### put\_resource\_policy

Attaches a resource-based policy to a custom model.

Type annotations and code completion for `#!python session.create_client("comprehend").put_resource_policy` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.put_resource_policy)

```python
# put_resource_policy method definition

await def put_resource_policy(
    self,
    *,
    ResourceArn: str,
    ResourcePolicy: str,
    PolicyRevisionId: str = ...,
) -> PutResourcePolicyResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: PutResourcePolicyResponseTypeDef](./type_defs.md#putresourcepolicyresponsetypedef) 


```python
# put_resource_policy method usage example with argument unpacking

kwargs: PutResourcePolicyRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "ResourcePolicy": ...,
}

parent.put_resource_policy(**kwargs)
```

1. See [:material-code-braces: PutResourcePolicyRequestRequestTypeDef](./type_defs.md#putresourcepolicyrequestrequesttypedef) 

### start\_document\_classification\_job

Starts an asynchronous document classification job.

Type annotations and code completion for `#!python session.create_client("comprehend").start_document_classification_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_document_classification_job)

```python
# start_document_classification_job method definition

await def start_document_classification_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    JobName: str = ...,
    DocumentClassifierArn: str = ...,
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
    FlywheelArn: str = ...,
) -> StartDocumentClassificationJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: StartDocumentClassificationJobResponseTypeDef](./type_defs.md#startdocumentclassificationjobresponsetypedef) 


```python
# start_document_classification_job method usage example with argument unpacking

kwargs: StartDocumentClassificationJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
}

parent.start_document_classification_job(**kwargs)
```

1. See [:material-code-braces: StartDocumentClassificationJobRequestRequestTypeDef](./type_defs.md#startdocumentclassificationjobrequestrequesttypedef) 

### start\_dominant\_language\_detection\_job

Starts an asynchronous dominant language detection job for a collection of
documents.

Type annotations and code completion for `#!python session.create_client("comprehend").start_dominant_language_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_dominant_language_detection_job)

```python
# start_dominant_language_detection_job method definition

await def start_dominant_language_detection_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    JobName: str = ...,
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> StartDominantLanguageDetectionJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: StartDominantLanguageDetectionJobResponseTypeDef](./type_defs.md#startdominantlanguagedetectionjobresponsetypedef) 


```python
# start_dominant_language_detection_job method usage example with argument unpacking

kwargs: StartDominantLanguageDetectionJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
}

parent.start_dominant_language_detection_job(**kwargs)
```

1. See [:material-code-braces: StartDominantLanguageDetectionJobRequestRequestTypeDef](./type_defs.md#startdominantlanguagedetectionjobrequestrequesttypedef) 

### start\_entities\_detection\_job

Starts an asynchronous entity detection job for a collection of documents.

Type annotations and code completion for `#!python session.create_client("comprehend").start_entities_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_entities_detection_job)

```python
# start_entities_detection_job method definition

await def start_entities_detection_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: str = ...,
    EntityRecognizerArn: str = ...,
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
    FlywheelArn: str = ...,
) -> StartEntitiesDetectionJobResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: StartEntitiesDetectionJobResponseTypeDef](./type_defs.md#startentitiesdetectionjobresponsetypedef) 


```python
# start_entities_detection_job method usage example with argument unpacking

kwargs: StartEntitiesDetectionJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
    "LanguageCode": ...,
}

parent.start_entities_detection_job(**kwargs)
```

1. See [:material-code-braces: StartEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#startentitiesdetectionjobrequestrequesttypedef) 

### start\_events\_detection\_job

Starts an asynchronous event detection job for a collection of documents.

Type annotations and code completion for `#!python session.create_client("comprehend").start_events_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_events_detection_job)

```python
# start_events_detection_job method definition

await def start_events_detection_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    TargetEventTypes: Sequence[str],
    JobName: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> StartEventsDetectionJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: StartEventsDetectionJobResponseTypeDef](./type_defs.md#starteventsdetectionjobresponsetypedef) 


```python
# start_events_detection_job method usage example with argument unpacking

kwargs: StartEventsDetectionJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
    "LanguageCode": ...,
    "TargetEventTypes": ...,
}

parent.start_events_detection_job(**kwargs)
```

1. See [:material-code-braces: StartEventsDetectionJobRequestRequestTypeDef](./type_defs.md#starteventsdetectionjobrequestrequesttypedef) 

### start\_flywheel\_iteration

Start the flywheel iteration.This operation uses any new datasets to train a new
model version.

Type annotations and code completion for `#!python session.create_client("comprehend").start_flywheel_iteration` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_flywheel_iteration)

```python
# start_flywheel_iteration method definition

await def start_flywheel_iteration(
    self,
    *,
    FlywheelArn: str,
    ClientRequestToken: str = ...,
) -> StartFlywheelIterationResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StartFlywheelIterationResponseTypeDef](./type_defs.md#startflywheeliterationresponsetypedef) 


```python
# start_flywheel_iteration method usage example with argument unpacking

kwargs: StartFlywheelIterationRequestRequestTypeDef = {  # (1)
    "FlywheelArn": ...,
}

parent.start_flywheel_iteration(**kwargs)
```

1. See [:material-code-braces: StartFlywheelIterationRequestRequestTypeDef](./type_defs.md#startflywheeliterationrequestrequesttypedef) 

### start\_key\_phrases\_detection\_job

Starts an asynchronous key phrase detection job for a collection of documents.

Type annotations and code completion for `#!python session.create_client("comprehend").start_key_phrases_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_key_phrases_detection_job)

```python
# start_key_phrases_detection_job method definition

await def start_key_phrases_detection_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: str = ...,
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> StartKeyPhrasesDetectionJobResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: StartKeyPhrasesDetectionJobResponseTypeDef](./type_defs.md#startkeyphrasesdetectionjobresponsetypedef) 


```python
# start_key_phrases_detection_job method usage example with argument unpacking

kwargs: StartKeyPhrasesDetectionJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
    "LanguageCode": ...,
}

parent.start_key_phrases_detection_job(**kwargs)
```

1. See [:material-code-braces: StartKeyPhrasesDetectionJobRequestRequestTypeDef](./type_defs.md#startkeyphrasesdetectionjobrequestrequesttypedef) 

### start\_pii\_entities\_detection\_job

Starts an asynchronous PII entity detection job for a collection of documents.

Type annotations and code completion for `#!python session.create_client("comprehend").start_pii_entities_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_pii_entities_detection_job)

```python
# start_pii_entities_detection_job method definition

await def start_pii_entities_detection_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    Mode: PiiEntitiesDetectionModeType,  # (3)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (4)
    RedactionConfig: RedactionConfigTypeDef = ...,  # (5)
    JobName: str = ...,
    ClientRequestToken: str = ...,
    Tags: Sequence[TagTypeDef] = ...,  # (6)
) -> StartPiiEntitiesDetectionJobResponseTypeDef:  # (7)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: PiiEntitiesDetectionModeType](./literals.md#piientitiesdetectionmodetype) 
4. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
5. See [:material-code-braces: RedactionConfigTypeDef](./type_defs.md#redactionconfigtypedef) 
6. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
7. See [:material-code-braces: StartPiiEntitiesDetectionJobResponseTypeDef](./type_defs.md#startpiientitiesdetectionjobresponsetypedef) 


```python
# start_pii_entities_detection_job method usage example with argument unpacking

kwargs: StartPiiEntitiesDetectionJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "Mode": ...,
    "DataAccessRoleArn": ...,
    "LanguageCode": ...,
}

parent.start_pii_entities_detection_job(**kwargs)
```

1. See [:material-code-braces: StartPiiEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#startpiientitiesdetectionjobrequestrequesttypedef) 

### start\_sentiment\_detection\_job

Starts an asynchronous sentiment detection job for a collection of documents.

Type annotations and code completion for `#!python session.create_client("comprehend").start_sentiment_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_sentiment_detection_job)

```python
# start_sentiment_detection_job method definition

await def start_sentiment_detection_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: str = ...,
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> StartSentimentDetectionJobResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: StartSentimentDetectionJobResponseTypeDef](./type_defs.md#startsentimentdetectionjobresponsetypedef) 


```python
# start_sentiment_detection_job method usage example with argument unpacking

kwargs: StartSentimentDetectionJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
    "LanguageCode": ...,
}

parent.start_sentiment_detection_job(**kwargs)
```

1. See [:material-code-braces: StartSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#startsentimentdetectionjobrequestrequesttypedef) 

### start\_targeted\_sentiment\_detection\_job

Starts an asynchronous targeted sentiment detection job for a collection of
documents.

Type annotations and code completion for `#!python session.create_client("comprehend").start_targeted_sentiment_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_targeted_sentiment_detection_job)

```python
# start_targeted_sentiment_detection_job method definition

await def start_targeted_sentiment_detection_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    LanguageCode: LanguageCodeType,  # (3)
    JobName: str = ...,
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (4)
    Tags: Sequence[TagTypeDef] = ...,  # (5)
) -> StartTargetedSentimentDetectionJobResponseTypeDef:  # (6)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-brackets: LanguageCodeType](./literals.md#languagecodetype) 
4. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
5. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
6. See [:material-code-braces: StartTargetedSentimentDetectionJobResponseTypeDef](./type_defs.md#starttargetedsentimentdetectionjobresponsetypedef) 


```python
# start_targeted_sentiment_detection_job method usage example with argument unpacking

kwargs: StartTargetedSentimentDetectionJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
    "LanguageCode": ...,
}

parent.start_targeted_sentiment_detection_job(**kwargs)
```

1. See [:material-code-braces: StartTargetedSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#starttargetedsentimentdetectionjobrequestrequesttypedef) 

### start\_topics\_detection\_job

Starts an asynchronous topic detection job.

Type annotations and code completion for `#!python session.create_client("comprehend").start_topics_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.start_topics_detection_job)

```python
# start_topics_detection_job method definition

await def start_topics_detection_job(
    self,
    *,
    InputDataConfig: InputDataConfigTypeDef,  # (1)
    OutputDataConfig: OutputDataConfigTypeDef,  # (2)
    DataAccessRoleArn: str,
    JobName: str = ...,
    NumberOfTopics: int = ...,
    ClientRequestToken: str = ...,
    VolumeKmsKeyId: str = ...,
    VpcConfig: VpcConfigTypeDef = ...,  # (3)
    Tags: Sequence[TagTypeDef] = ...,  # (4)
) -> StartTopicsDetectionJobResponseTypeDef:  # (5)
    ...
```

1. See [:material-code-braces: InputDataConfigTypeDef](./type_defs.md#inputdataconfigtypedef) 
2. See [:material-code-braces: OutputDataConfigTypeDef](./type_defs.md#outputdataconfigtypedef) 
3. See [:material-code-braces: VpcConfigTypeDef](./type_defs.md#vpcconfigtypedef) 
4. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
5. See [:material-code-braces: StartTopicsDetectionJobResponseTypeDef](./type_defs.md#starttopicsdetectionjobresponsetypedef) 


```python
# start_topics_detection_job method usage example with argument unpacking

kwargs: StartTopicsDetectionJobRequestRequestTypeDef = {  # (1)
    "InputDataConfig": ...,
    "OutputDataConfig": ...,
    "DataAccessRoleArn": ...,
}

parent.start_topics_detection_job(**kwargs)
```

1. See [:material-code-braces: StartTopicsDetectionJobRequestRequestTypeDef](./type_defs.md#starttopicsdetectionjobrequestrequesttypedef) 

### stop\_dominant\_language\_detection\_job

Stops a dominant language detection job in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_dominant_language_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_dominant_language_detection_job)

```python
# stop_dominant_language_detection_job method definition

await def stop_dominant_language_detection_job(
    self,
    *,
    JobId: str,
) -> StopDominantLanguageDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopDominantLanguageDetectionJobResponseTypeDef](./type_defs.md#stopdominantlanguagedetectionjobresponsetypedef) 


```python
# stop_dominant_language_detection_job method usage example with argument unpacking

kwargs: StopDominantLanguageDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.stop_dominant_language_detection_job(**kwargs)
```

1. See [:material-code-braces: StopDominantLanguageDetectionJobRequestRequestTypeDef](./type_defs.md#stopdominantlanguagedetectionjobrequestrequesttypedef) 

### stop\_entities\_detection\_job

Stops an entities detection job in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_entities_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_entities_detection_job)

```python
# stop_entities_detection_job method definition

await def stop_entities_detection_job(
    self,
    *,
    JobId: str,
) -> StopEntitiesDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopEntitiesDetectionJobResponseTypeDef](./type_defs.md#stopentitiesdetectionjobresponsetypedef) 


```python
# stop_entities_detection_job method usage example with argument unpacking

kwargs: StopEntitiesDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.stop_entities_detection_job(**kwargs)
```

1. See [:material-code-braces: StopEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#stopentitiesdetectionjobrequestrequesttypedef) 

### stop\_events\_detection\_job

Stops an events detection job in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_events_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_events_detection_job)

```python
# stop_events_detection_job method definition

await def stop_events_detection_job(
    self,
    *,
    JobId: str,
) -> StopEventsDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopEventsDetectionJobResponseTypeDef](./type_defs.md#stopeventsdetectionjobresponsetypedef) 


```python
# stop_events_detection_job method usage example with argument unpacking

kwargs: StopEventsDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.stop_events_detection_job(**kwargs)
```

1. See [:material-code-braces: StopEventsDetectionJobRequestRequestTypeDef](./type_defs.md#stopeventsdetectionjobrequestrequesttypedef) 

### stop\_key\_phrases\_detection\_job

Stops a key phrases detection job in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_key_phrases_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_key_phrases_detection_job)

```python
# stop_key_phrases_detection_job method definition

await def stop_key_phrases_detection_job(
    self,
    *,
    JobId: str,
) -> StopKeyPhrasesDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopKeyPhrasesDetectionJobResponseTypeDef](./type_defs.md#stopkeyphrasesdetectionjobresponsetypedef) 


```python
# stop_key_phrases_detection_job method usage example with argument unpacking

kwargs: StopKeyPhrasesDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.stop_key_phrases_detection_job(**kwargs)
```

1. See [:material-code-braces: StopKeyPhrasesDetectionJobRequestRequestTypeDef](./type_defs.md#stopkeyphrasesdetectionjobrequestrequesttypedef) 

### stop\_pii\_entities\_detection\_job

Stops a PII entities detection job in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_pii_entities_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_pii_entities_detection_job)

```python
# stop_pii_entities_detection_job method definition

await def stop_pii_entities_detection_job(
    self,
    *,
    JobId: str,
) -> StopPiiEntitiesDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopPiiEntitiesDetectionJobResponseTypeDef](./type_defs.md#stoppiientitiesdetectionjobresponsetypedef) 


```python
# stop_pii_entities_detection_job method usage example with argument unpacking

kwargs: StopPiiEntitiesDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.stop_pii_entities_detection_job(**kwargs)
```

1. See [:material-code-braces: StopPiiEntitiesDetectionJobRequestRequestTypeDef](./type_defs.md#stoppiientitiesdetectionjobrequestrequesttypedef) 

### stop\_sentiment\_detection\_job

Stops a sentiment detection job in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_sentiment_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_sentiment_detection_job)

```python
# stop_sentiment_detection_job method definition

await def stop_sentiment_detection_job(
    self,
    *,
    JobId: str,
) -> StopSentimentDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopSentimentDetectionJobResponseTypeDef](./type_defs.md#stopsentimentdetectionjobresponsetypedef) 


```python
# stop_sentiment_detection_job method usage example with argument unpacking

kwargs: StopSentimentDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.stop_sentiment_detection_job(**kwargs)
```

1. See [:material-code-braces: StopSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#stopsentimentdetectionjobrequestrequesttypedef) 

### stop\_targeted\_sentiment\_detection\_job

Stops a targeted sentiment detection job in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_targeted_sentiment_detection_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_targeted_sentiment_detection_job)

```python
# stop_targeted_sentiment_detection_job method definition

await def stop_targeted_sentiment_detection_job(
    self,
    *,
    JobId: str,
) -> StopTargetedSentimentDetectionJobResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: StopTargetedSentimentDetectionJobResponseTypeDef](./type_defs.md#stoptargetedsentimentdetectionjobresponsetypedef) 


```python
# stop_targeted_sentiment_detection_job method usage example with argument unpacking

kwargs: StopTargetedSentimentDetectionJobRequestRequestTypeDef = {  # (1)
    "JobId": ...,
}

parent.stop_targeted_sentiment_detection_job(**kwargs)
```

1. See [:material-code-braces: StopTargetedSentimentDetectionJobRequestRequestTypeDef](./type_defs.md#stoptargetedsentimentdetectionjobrequestrequesttypedef) 

### stop\_training\_document\_classifier

Stops a document classifier training job while in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_training_document_classifier` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_training_document_classifier)

```python
# stop_training_document_classifier method definition

await def stop_training_document_classifier(
    self,
    *,
    DocumentClassifierArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_training_document_classifier method usage example with argument unpacking

kwargs: StopTrainingDocumentClassifierRequestRequestTypeDef = {  # (1)
    "DocumentClassifierArn": ...,
}

parent.stop_training_document_classifier(**kwargs)
```

1. See [:material-code-braces: StopTrainingDocumentClassifierRequestRequestTypeDef](./type_defs.md#stoptrainingdocumentclassifierrequestrequesttypedef) 

### stop\_training\_entity\_recognizer

Stops an entity recognizer training job while in progress.

Type annotations and code completion for `#!python session.create_client("comprehend").stop_training_entity_recognizer` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.stop_training_entity_recognizer)

```python
# stop_training_entity_recognizer method definition

await def stop_training_entity_recognizer(
    self,
    *,
    EntityRecognizerArn: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_training_entity_recognizer method usage example with argument unpacking

kwargs: StopTrainingEntityRecognizerRequestRequestTypeDef = {  # (1)
    "EntityRecognizerArn": ...,
}

parent.stop_training_entity_recognizer(**kwargs)
```

1. See [:material-code-braces: StopTrainingEntityRecognizerRequestRequestTypeDef](./type_defs.md#stoptrainingentityrecognizerrequestrequesttypedef) 

### tag\_resource

Associates a specific tag with an Amazon Comprehend resource.

Type annotations and code completion for `#!python session.create_client("comprehend").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
) -> Dict[str, Any]:
    ...
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 


```python
# tag_resource method usage example with argument unpacking

kwargs: TagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "Tags": ...,
}

parent.tag_resource(**kwargs)
```

1. See [:material-code-braces: TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef) 

### untag\_resource

Removes a specific tag associated with an Amazon Comprehend resource.

Type annotations and code completion for `#!python session.create_client("comprehend").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.untag_resource)

```python
# untag_resource method definition

await def untag_resource(
    self,
    *,
    ResourceArn: str,
    TagKeys: Sequence[str],
) -> Dict[str, Any]:
    ...
```



```python
# untag_resource method usage example with argument unpacking

kwargs: UntagResourceRequestRequestTypeDef = {  # (1)
    "ResourceArn": ...,
    "TagKeys": ...,
}

parent.untag_resource(**kwargs)
```

1. See [:material-code-braces: UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef) 

### update\_endpoint

Updates information about the specified endpoint.

Type annotations and code completion for `#!python session.create_client("comprehend").update_endpoint` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_endpoint)

```python
# update_endpoint method definition

await def update_endpoint(
    self,
    *,
    EndpointArn: str,
    DesiredModelArn: str = ...,
    DesiredInferenceUnits: int = ...,
    DesiredDataAccessRoleArn: str = ...,
    FlywheelArn: str = ...,
) -> UpdateEndpointResponseTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: UpdateEndpointResponseTypeDef](./type_defs.md#updateendpointresponsetypedef) 


```python
# update_endpoint method usage example with argument unpacking

kwargs: UpdateEndpointRequestRequestTypeDef = {  # (1)
    "EndpointArn": ...,
}

parent.update_endpoint(**kwargs)
```

1. See [:material-code-braces: UpdateEndpointRequestRequestTypeDef](./type_defs.md#updateendpointrequestrequesttypedef) 

### update\_flywheel

Update the configuration information for an existing flywheel.

Type annotations and code completion for `#!python session.create_client("comprehend").update_flywheel` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.update_flywheel)

```python
# update_flywheel method definition

await def update_flywheel(
    self,
    *,
    FlywheelArn: str,
    ActiveModelArn: str = ...,
    DataAccessRoleArn: str = ...,
    DataSecurityConfig: UpdateDataSecurityConfigTypeDef = ...,  # (1)
) -> UpdateFlywheelResponseTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: UpdateDataSecurityConfigTypeDef](./type_defs.md#updatedatasecurityconfigtypedef) 
2. See [:material-code-braces: UpdateFlywheelResponseTypeDef](./type_defs.md#updateflywheelresponsetypedef) 


```python
# update_flywheel method usage example with argument unpacking

kwargs: UpdateFlywheelRequestRequestTypeDef = {  # (1)
    "FlywheelArn": ...,
}

parent.update_flywheel(**kwargs)
```

1. See [:material-code-braces: UpdateFlywheelRequestRequestTypeDef](./type_defs.md#updateflywheelrequestrequesttypedef) 

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("comprehend").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> ComprehendClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("comprehend").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehend.html#Comprehend.Client.__aexit__)

```python
# __aexit__ method definition

await def __aexit__(
    self,
    exc_type: Any,
    exc_val: Any,
    exc_tb: Any,
) -> Any:
    ...
```




### get_paginator

Type annotations and code completion for `#!python session.create_client("comprehend").get_paginator` method with overloads.

- `client.get_paginator("list_document_classification_jobs")` -> [ListDocumentClassificationJobsPaginator](./paginators.md#listdocumentclassificationjobspaginator)
- `client.get_paginator("list_document_classifiers")` -> [ListDocumentClassifiersPaginator](./paginators.md#listdocumentclassifierspaginator)
- `client.get_paginator("list_dominant_language_detection_jobs")` -> [ListDominantLanguageDetectionJobsPaginator](./paginators.md#listdominantlanguagedetectionjobspaginator)
- `client.get_paginator("list_endpoints")` -> [ListEndpointsPaginator](./paginators.md#listendpointspaginator)
- `client.get_paginator("list_entities_detection_jobs")` -> [ListEntitiesDetectionJobsPaginator](./paginators.md#listentitiesdetectionjobspaginator)
- `client.get_paginator("list_entity_recognizers")` -> [ListEntityRecognizersPaginator](./paginators.md#listentityrecognizerspaginator)
- `client.get_paginator("list_key_phrases_detection_jobs")` -> [ListKeyPhrasesDetectionJobsPaginator](./paginators.md#listkeyphrasesdetectionjobspaginator)
- `client.get_paginator("list_pii_entities_detection_jobs")` -> [ListPiiEntitiesDetectionJobsPaginator](./paginators.md#listpiientitiesdetectionjobspaginator)
- `client.get_paginator("list_sentiment_detection_jobs")` -> [ListSentimentDetectionJobsPaginator](./paginators.md#listsentimentdetectionjobspaginator)
- `client.get_paginator("list_topics_detection_jobs")` -> [ListTopicsDetectionJobsPaginator](./paginators.md#listtopicsdetectionjobspaginator)




# SageMakergeospatialcapabilitiesClient

> [Index](../README.md) > [SageMakergeospatialcapabilities](./README.md) > SageMakergeospatialcapabilitiesClient

!!! note ""

    Auto-generated documentation for [SageMakergeospatialcapabilities](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities)
    type annotations stubs module [types-aiobotocore-sagemaker-geospatial](https://pypi.org/project/types-aiobotocore-sagemaker-geospatial/).

## SageMakergeospatialcapabilitiesClient

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial")`
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client)

```python
SageMakergeospatialcapabilitiesClient usage example

from aiobotocore.session import get_session
from types_aiobotocore_sagemaker_geospatial.client import SageMakergeospatialcapabilitiesClient

session = get_session()
async with session.create_client("sagemaker-geospatial") as client:
    client: SageMakergeospatialcapabilitiesClient
```

## Exceptions


`aiobotocore` client exceptions are generated in runtime.
This class provides code completion for `#!python session.create_client("sagemaker-geospatial").exceptions` structure.

```python
SageMakergeospatialcapabilitiesClient.exceptions usage example

async with session.create_client("sagemaker-geospatial") as client:
    try:
        do_something(client)
    except (
            client.AccessDeniedException,
        client.ClientError,
        client.ConflictException,
        client.InternalServerException,
        client.ResourceNotFoundException,
        client.ServiceQuotaExceededException,
        client.ThrottlingException,
        client.ValidationException,
    ) as e:
        print(e)
```

```python
SageMakergeospatialcapabilitiesClient usage type checking example

from types_aiobotocore_sagemaker_geospatial.client import Exceptions

def handle_error(exc: Exceptions.AccessDeniedException) -> None:
    ...
```


## Methods


### can\_paginate

Check if an operation can be paginated.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").can_paginate` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.can_paginate)

```python
# can_paginate method definition

def can_paginate(
    self,
    operation_name: str,
) -> bool:
    ...
```


### close

Closes underlying endpoint connections.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").close` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.close)

```python
# close method definition

await def close(
    self,
) -> None:
    ...
```


### delete\_earth\_observation\_job

Use this operation to delete an Earth Observation job.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").delete_earth_observation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.delete_earth_observation_job)

```python
# delete_earth_observation_job method definition

await def delete_earth_observation_job(
    self,
    *,
    Arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_earth_observation_job method usage example with argument unpacking

kwargs: DeleteEarthObservationJobInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_earth_observation_job(**kwargs)
```

1. See [:material-code-braces: DeleteEarthObservationJobInputRequestTypeDef](./type_defs.md#deleteearthobservationjobinputrequesttypedef) 

### delete\_vector\_enrichment\_job

Use this operation to delete a Vector Enrichment job.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").delete_vector_enrichment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.delete_vector_enrichment_job)

```python
# delete_vector_enrichment_job method definition

await def delete_vector_enrichment_job(
    self,
    *,
    Arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# delete_vector_enrichment_job method usage example with argument unpacking

kwargs: DeleteVectorEnrichmentJobInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.delete_vector_enrichment_job(**kwargs)
```

1. See [:material-code-braces: DeleteVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#deletevectorenrichmentjobinputrequesttypedef) 

### export\_earth\_observation\_job

Use this operation to export results of an Earth Observation job and optionally
source images used as input to the EOJ to an Amazon S3 location.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").export_earth_observation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_earth_observation_job)

```python
# export_earth_observation_job method definition

await def export_earth_observation_job(
    self,
    *,
    Arn: str,
    ExecutionRoleArn: str,
    OutputConfig: OutputConfigInputTypeDef,  # (1)
    ClientToken: str = ...,
    ExportSourceImages: bool = ...,
) -> ExportEarthObservationJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: OutputConfigInputTypeDef](./type_defs.md#outputconfiginputtypedef) 
2. See [:material-code-braces: ExportEarthObservationJobOutputTypeDef](./type_defs.md#exportearthobservationjoboutputtypedef) 


```python
# export_earth_observation_job method usage example with argument unpacking

kwargs: ExportEarthObservationJobInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "ExecutionRoleArn": ...,
    "OutputConfig": ...,
}

parent.export_earth_observation_job(**kwargs)
```

1. See [:material-code-braces: ExportEarthObservationJobInputRequestTypeDef](./type_defs.md#exportearthobservationjobinputrequesttypedef) 

### export\_vector\_enrichment\_job

Use this operation to copy results of a Vector Enrichment job to an Amazon S3
location.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").export_vector_enrichment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.export_vector_enrichment_job)

```python
# export_vector_enrichment_job method definition

await def export_vector_enrichment_job(
    self,
    *,
    Arn: str,
    ExecutionRoleArn: str,
    OutputConfig: ExportVectorEnrichmentJobOutputConfigTypeDef,  # (1)
    ClientToken: str = ...,
) -> ExportVectorEnrichmentJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: ExportVectorEnrichmentJobOutputConfigTypeDef](./type_defs.md#exportvectorenrichmentjoboutputconfigtypedef) 
2. See [:material-code-braces: ExportVectorEnrichmentJobOutputTypeDef](./type_defs.md#exportvectorenrichmentjoboutputtypedef) 


```python
# export_vector_enrichment_job method usage example with argument unpacking

kwargs: ExportVectorEnrichmentJobInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "ExecutionRoleArn": ...,
    "OutputConfig": ...,
}

parent.export_vector_enrichment_job(**kwargs)
```

1. See [:material-code-braces: ExportVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#exportvectorenrichmentjobinputrequesttypedef) 

### generate\_presigned\_url

Generate a presigned url given a client, its method, and arguments.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").generate_presigned_url` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.generate_presigned_url)

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


### get\_earth\_observation\_job

Get the details for a previously initiated Earth Observation job.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").get_earth_observation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.get_earth_observation_job)

```python
# get_earth_observation_job method definition

await def get_earth_observation_job(
    self,
    *,
    Arn: str,
) -> GetEarthObservationJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetEarthObservationJobOutputTypeDef](./type_defs.md#getearthobservationjoboutputtypedef) 


```python
# get_earth_observation_job method usage example with argument unpacking

kwargs: GetEarthObservationJobInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_earth_observation_job(**kwargs)
```

1. See [:material-code-braces: GetEarthObservationJobInputRequestTypeDef](./type_defs.md#getearthobservationjobinputrequesttypedef) 

### get\_raster\_data\_collection

Use this operation to get details of a specific raster data collection.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").get_raster_data_collection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.get_raster_data_collection)

```python
# get_raster_data_collection method definition

await def get_raster_data_collection(
    self,
    *,
    Arn: str,
) -> GetRasterDataCollectionOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetRasterDataCollectionOutputTypeDef](./type_defs.md#getrasterdatacollectionoutputtypedef) 


```python
# get_raster_data_collection method usage example with argument unpacking

kwargs: GetRasterDataCollectionInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_raster_data_collection(**kwargs)
```

1. See [:material-code-braces: GetRasterDataCollectionInputRequestTypeDef](./type_defs.md#getrasterdatacollectioninputrequesttypedef) 

### get\_tile

Gets a web mercator tile for the given Earth Observation job.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").get_tile` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.get_tile)

```python
# get_tile method definition

await def get_tile(
    self,
    *,
    Arn: str,
    ImageAssets: Sequence[str],
    Target: TargetOptionsType,  # (1)
    x: int,
    y: int,
    z: int,
    ExecutionRoleArn: str = ...,
    ImageMask: bool = ...,
    OutputDataType: OutputTypeType = ...,  # (2)
    OutputFormat: str = ...,
    PropertyFilters: str = ...,
    TimeRangeFilter: str = ...,
) -> GetTileOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: TargetOptionsType](./literals.md#targetoptionstype) 
2. See [:material-code-brackets: OutputTypeType](./literals.md#outputtypetype) 
3. See [:material-code-braces: GetTileOutputTypeDef](./type_defs.md#gettileoutputtypedef) 


```python
# get_tile method usage example with argument unpacking

kwargs: GetTileInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "ImageAssets": ...,
    "Target": ...,
    "x": ...,
    "y": ...,
    "z": ...,
}

parent.get_tile(**kwargs)
```

1. See [:material-code-braces: GetTileInputRequestTypeDef](./type_defs.md#gettileinputrequesttypedef) 

### get\_vector\_enrichment\_job

Retrieves details of a Vector Enrichment Job for a given job Amazon Resource
Name (ARN).

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").get_vector_enrichment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.get_vector_enrichment_job)

```python
# get_vector_enrichment_job method definition

await def get_vector_enrichment_job(
    self,
    *,
    Arn: str,
) -> GetVectorEnrichmentJobOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: GetVectorEnrichmentJobOutputTypeDef](./type_defs.md#getvectorenrichmentjoboutputtypedef) 


```python
# get_vector_enrichment_job method usage example with argument unpacking

kwargs: GetVectorEnrichmentJobInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.get_vector_enrichment_job(**kwargs)
```

1. See [:material-code-braces: GetVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#getvectorenrichmentjobinputrequesttypedef) 

### list\_earth\_observation\_jobs

Use this operation to get a list of the Earth Observation jobs associated with
the calling Amazon Web Services account.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").list_earth_observation_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.list_earth_observation_jobs)

```python
# list_earth_observation_jobs method definition

await def list_earth_observation_jobs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    SortBy: str = ...,
    SortOrder: SortOrderType = ...,  # (1)
    StatusEquals: EarthObservationJobStatusType = ...,  # (2)
) -> ListEarthObservationJobOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-brackets: EarthObservationJobStatusType](./literals.md#earthobservationjobstatustype) 
3. See [:material-code-braces: ListEarthObservationJobOutputTypeDef](./type_defs.md#listearthobservationjoboutputtypedef) 


```python
# list_earth_observation_jobs method usage example with argument unpacking

kwargs: ListEarthObservationJobInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_earth_observation_jobs(**kwargs)
```

1. See [:material-code-braces: ListEarthObservationJobInputRequestTypeDef](./type_defs.md#listearthobservationjobinputrequesttypedef) 

### list\_raster\_data\_collections

Use this operation to get raster data collections.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").list_raster_data_collections` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.list_raster_data_collections)

```python
# list_raster_data_collections method definition

await def list_raster_data_collections(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
) -> ListRasterDataCollectionsOutputTypeDef:  # (1)
    ...
```

1. See [:material-code-braces: ListRasterDataCollectionsOutputTypeDef](./type_defs.md#listrasterdatacollectionsoutputtypedef) 


```python
# list_raster_data_collections method usage example with argument unpacking

kwargs: ListRasterDataCollectionsInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_raster_data_collections(**kwargs)
```

1. See [:material-code-braces: ListRasterDataCollectionsInputRequestTypeDef](./type_defs.md#listrasterdatacollectionsinputrequesttypedef) 

### list\_tags\_for\_resource

Lists the tags attached to the resource.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").list_tags_for_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.list_tags_for_resource)

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

### list\_vector\_enrichment\_jobs

Retrieves a list of vector enrichment jobs.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").list_vector_enrichment_jobs` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.list_vector_enrichment_jobs)

```python
# list_vector_enrichment_jobs method definition

await def list_vector_enrichment_jobs(
    self,
    *,
    MaxResults: int = ...,
    NextToken: str = ...,
    SortBy: str = ...,
    SortOrder: SortOrderType = ...,  # (1)
    StatusEquals: str = ...,
) -> ListVectorEnrichmentJobOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-brackets: SortOrderType](./literals.md#sortordertype) 
2. See [:material-code-braces: ListVectorEnrichmentJobOutputTypeDef](./type_defs.md#listvectorenrichmentjoboutputtypedef) 


```python
# list_vector_enrichment_jobs method usage example with argument unpacking

kwargs: ListVectorEnrichmentJobInputRequestTypeDef = {  # (1)
    "MaxResults": ...,
}

parent.list_vector_enrichment_jobs(**kwargs)
```

1. See [:material-code-braces: ListVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#listvectorenrichmentjobinputrequesttypedef) 

### search\_raster\_data\_collection

Allows you run image query on a specific raster data collection to get a list of
the satellite imagery matching the selected filters.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").search_raster_data_collection` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.search_raster_data_collection)

```python
# search_raster_data_collection method definition

await def search_raster_data_collection(
    self,
    *,
    Arn: str,
    RasterDataCollectionQuery: RasterDataCollectionQueryWithBandFilterInputTypeDef,  # (1)
    NextToken: str = ...,
) -> SearchRasterDataCollectionOutputTypeDef:  # (2)
    ...
```

1. See [:material-code-braces: RasterDataCollectionQueryWithBandFilterInputTypeDef](./type_defs.md#rasterdatacollectionquerywithbandfilterinputtypedef) 
2. See [:material-code-braces: SearchRasterDataCollectionOutputTypeDef](./type_defs.md#searchrasterdatacollectionoutputtypedef) 


```python
# search_raster_data_collection method usage example with argument unpacking

kwargs: SearchRasterDataCollectionInputRequestTypeDef = {  # (1)
    "Arn": ...,
    "RasterDataCollectionQuery": ...,
}

parent.search_raster_data_collection(**kwargs)
```

1. See [:material-code-braces: SearchRasterDataCollectionInputRequestTypeDef](./type_defs.md#searchrasterdatacollectioninputrequesttypedef) 

### start\_earth\_observation\_job

Use this operation to create an Earth observation job.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").start_earth_observation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.start_earth_observation_job)

```python
# start_earth_observation_job method definition

await def start_earth_observation_job(
    self,
    *,
    ExecutionRoleArn: str,
    InputConfig: InputConfigInputTypeDef,  # (1)
    JobConfig: JobConfigInputTypeDef,  # (2)
    Name: str,
    ClientToken: str = ...,
    KmsKeyId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> StartEarthObservationJobOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: InputConfigInputTypeDef](./type_defs.md#inputconfiginputtypedef) 
2. See [:material-code-braces: JobConfigInputTypeDef](./type_defs.md#jobconfiginputtypedef) 
3. See [:material-code-braces: StartEarthObservationJobOutputTypeDef](./type_defs.md#startearthobservationjoboutputtypedef) 


```python
# start_earth_observation_job method usage example with argument unpacking

kwargs: StartEarthObservationJobInputRequestTypeDef = {  # (1)
    "ExecutionRoleArn": ...,
    "InputConfig": ...,
    "JobConfig": ...,
    "Name": ...,
}

parent.start_earth_observation_job(**kwargs)
```

1. See [:material-code-braces: StartEarthObservationJobInputRequestTypeDef](./type_defs.md#startearthobservationjobinputrequesttypedef) 

### start\_vector\_enrichment\_job

Creates a Vector Enrichment job for the supplied job type.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").start_vector_enrichment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.start_vector_enrichment_job)

```python
# start_vector_enrichment_job method definition

await def start_vector_enrichment_job(
    self,
    *,
    ExecutionRoleArn: str,
    InputConfig: VectorEnrichmentJobInputConfigTypeDef,  # (1)
    JobConfig: VectorEnrichmentJobConfigTypeDef,  # (2)
    Name: str,
    ClientToken: str = ...,
    KmsKeyId: str = ...,
    Tags: Mapping[str, str] = ...,
) -> StartVectorEnrichmentJobOutputTypeDef:  # (3)
    ...
```

1. See [:material-code-braces: VectorEnrichmentJobInputConfigTypeDef](./type_defs.md#vectorenrichmentjobinputconfigtypedef) 
2. See [:material-code-braces: VectorEnrichmentJobConfigTypeDef](./type_defs.md#vectorenrichmentjobconfigtypedef) 
3. See [:material-code-braces: StartVectorEnrichmentJobOutputTypeDef](./type_defs.md#startvectorenrichmentjoboutputtypedef) 


```python
# start_vector_enrichment_job method usage example with argument unpacking

kwargs: StartVectorEnrichmentJobInputRequestTypeDef = {  # (1)
    "ExecutionRoleArn": ...,
    "InputConfig": ...,
    "JobConfig": ...,
    "Name": ...,
}

parent.start_vector_enrichment_job(**kwargs)
```

1. See [:material-code-braces: StartVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#startvectorenrichmentjobinputrequesttypedef) 

### stop\_earth\_observation\_job

Use this operation to stop an existing earth observation job.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").stop_earth_observation_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.stop_earth_observation_job)

```python
# stop_earth_observation_job method definition

await def stop_earth_observation_job(
    self,
    *,
    Arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_earth_observation_job method usage example with argument unpacking

kwargs: StopEarthObservationJobInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.stop_earth_observation_job(**kwargs)
```

1. See [:material-code-braces: StopEarthObservationJobInputRequestTypeDef](./type_defs.md#stopearthobservationjobinputrequesttypedef) 

### stop\_vector\_enrichment\_job

Stops the Vector Enrichment job for a given job ARN.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").stop_vector_enrichment_job` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.stop_vector_enrichment_job)

```python
# stop_vector_enrichment_job method definition

await def stop_vector_enrichment_job(
    self,
    *,
    Arn: str,
) -> Dict[str, Any]:
    ...
```



```python
# stop_vector_enrichment_job method usage example with argument unpacking

kwargs: StopVectorEnrichmentJobInputRequestTypeDef = {  # (1)
    "Arn": ...,
}

parent.stop_vector_enrichment_job(**kwargs)
```

1. See [:material-code-braces: StopVectorEnrichmentJobInputRequestTypeDef](./type_defs.md#stopvectorenrichmentjobinputrequesttypedef) 

### tag\_resource

The resource you want to tag.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").tag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.tag_resource)

```python
# tag_resource method definition

await def tag_resource(
    self,
    *,
    ResourceArn: str,
    Tags: Mapping[str, str],
) -> Dict[str, Any]:
    ...
```



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

The resource you want to untag.

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").untag_resource` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.untag_resource)

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

### \_\_aenter\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").__aenter__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.__aenter__)

```python
# __aenter__ method definition

await def __aenter__(
    self,
) -> SageMakergeospatialcapabilitiesClient:
    ...
```


### \_\_aexit\_\_



Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").__aexit__` method.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-geospatial.html#SageMakergeospatialcapabilities.Client.__aexit__)

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

Type annotations and code completion for `#!python session.create_client("sagemaker-geospatial").get_paginator` method with overloads.

- `client.get_paginator("list_earth_observation_jobs")` -> [ListEarthObservationJobsPaginator](./paginators.md#listearthobservationjobspaginator)
- `client.get_paginator("list_raster_data_collections")` -> [ListRasterDataCollectionsPaginator](./paginators.md#listrasterdatacollectionspaginator)
- `client.get_paginator("list_vector_enrichment_jobs")` -> [ListVectorEnrichmentJobsPaginator](./paginators.md#listvectorenrichmentjobspaginator)




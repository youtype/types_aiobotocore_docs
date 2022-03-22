<a id="examples-for-aiobotocore-kinesisvideoarchivedmedia-module"></a>

# Examples for aiobotocore KinesisVideoArchivedMedia module

> [Index](../README.md) > [KinesisVideoArchivedMedia](./README.md) > Examples

- [Examples for aiobotocore KinesisVideoArchivedMedia module](#examples-for-aiobotocore-kinesisvideoarchivedmedia-module)
  - [Client](#client)
    - [Implicit type annotations](#implicit-type-annotations)
    - [Explicit type annotations](#explicit-type-annotations)

<a id="client"></a>

## Client

<a id="implicit-type-annotations"></a>

### Implicit type annotations

Can be used with `types-aiobotocore[kinesis-video-archived-media]` package
installed.

Write your `KinesisVideoArchivedMedia` code as usual, type checking and code
completion should work out of the box.

```python
from aiobotocore.session import get_session


session = get_session()

# client has type KinesisVideoArchivedMediaClient
# and provides type checking and code completion
async with session.create_client("kinesis-video-archived-media") as client:
    
    # result has type bool
    # and provides type checking and code completion
    # IDE should show a hint with argument names and types
    result = await client.can_paginate()
    

    
    # paginator has type ListFragmentsPaginator and provides type checking
    # and code completion for paginate method
    paginator = client.get_paginator("list_fragments")
    async for item in paginator.paginate(...):
        # item has type ListFragmentsOutputTypeDef
        print(item)
    

    
```

<a id="explicit-type-annotations"></a>

### Explicit type annotations

With `types-aiobotocore-lite[kinesis-video-archived-media]` or a standalone
`types_aiobotocore_kinesis_video_archived_media` package, you have to
explicitly specify `client: KinesisVideoArchivedMediaClient` type annotation.

All other type annotations are optional, as types should be discovered
automatically. However, these type annotations can be helpful in your functions
and methods.

```python
from aiobotocore.session import get_session

from types_aiobotocore_kinesis_video_archived_media.client import KinesisVideoArchivedMediaClient
from types_aiobotocore_kinesis_video_archived_media.type_defs import bool
from types_aiobotocore_kinesis_video_archived_media.paginator import ListFragmentsPaginator

from types_aiobotocore_kinesis_video_archived_media.literals import PaginatorName



session = get_session()

async with session.create_client("kinesis-video-archived-media") as client:
    client: KinesisVideoArchivedMediaClient

    
    result: bool = client.can_paginate()
    

    
    paginator_name: PaginatorName = "list_fragments"
    paginator: ListFragmentsPaginator = client.get_paginator(paginator_name)
    async for item in paginator.paginate(...):
        item: ListFragmentsOutputTypeDef
        print(item)
    

    
```

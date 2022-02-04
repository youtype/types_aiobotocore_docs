<a id="paginators-for-aiobotocore-s3control-module"></a>

# Paginators for aiobotocore S3Control module

> [Index](..) > [S3Control](.) > Paginators

Auto-generated documentation for
[S3Control](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control)
type annotations stubs module
[types-aiobotocore-s3control](https://pypi.org/project/types-aiobotocore-s3control/).

- [Paginators for aiobotocore S3Control module](#paginators-for-aiobotocore-s3control-module)
  - [ListAccessPointsForObjectLambdaPaginator](#listaccesspointsforobjectlambdapaginator)

<a id="listaccesspointsforobjectlambdapaginator"></a>

## ListAccessPointsForObjectLambdaPaginator

Type annotations for
`aiobotocore.create_client("s3control").get_paginator("list_access_points_for_object_lambda")`.

Can be used directly:

```python
from aiobotocore.session import Session

from types_aiobotocore_s3control.paginator import ListAccessPointsForObjectLambdaPaginator

def get_list_access_points_for_object_lambda_paginator() -> ListAccessPointsForObjectLambdaPaginator:
    return Session().create_client("s3control").get_paginator("list_access_points_for_object_lambda")
```

Boto3 documentation:
[S3Control.Paginator.ListAccessPointsForObjectLambda](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3control.html#S3Control.Paginator.ListAccessPointsForObjectLambda)

Arguments for `ListAccessPointsForObjectLambdaPaginator.paginate` method:

- `AccountId`: `str` *(required)*
- `PaginationConfig`:
  [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)

`ListAccessPointsForObjectLambdaPaginator.paginate` returns
`_PageIterator`\[[ListAccessPointsForObjectLambdaResultTypeDef](./type_defs.md#listaccesspointsforobjectlambdaresulttypedef)\].

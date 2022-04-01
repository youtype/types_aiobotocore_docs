# AppIntegrationsService module

> [Index](../README.md) > AppIntegrationsService


!!! note ""

    Auto-generated documentation for [AppIntegrationsService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService)
    type annotations stubs module [types-aiobotocore-appintegrations](https://pypi.org/project/types-aiobotocore-appintegrations/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `AppIntegrationsService`.

### From PyPI with pip

Install `types-aiobotocore` for `AppIntegrationsService` service.

```bash
# install with aiobotocore type annotations
python -m pip install 'types-aiobotocore[appintegrations]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'types-aiobotocore-lite[appintegrations]'


# standalone installation
python -m pip install types-aiobotocore-appintegrations
```



## How to uninstall

```bash
python -m pip uninstall -y types-aiobotocore-appintegrations
```

## Usage

Code samples can be found in [Examples](./usage.md).

## AppIntegrationsServiceClient

Type annotations and code completion for  `#!python session.create_client("appintegrations")` as [AppIntegrationsServiceClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client)

```python title="Usage example"
from aiobotocore.session import get_session

from types_aiobotocore_appintegrations.client import AppIntegrationsServiceClient


session = get_session()
async with session.create_client("appintegrations") as client:
    client: AppIntegrationsServiceClient
```








## Literals

Type annotations for [literals](./literals.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_appintegrations.literals import AppIntegrationsServiceServiceName

def get_value() -> AppIntegrationsServiceServiceName:
    return "appintegrations"
```

- [AppIntegrationsServiceServiceName](./literals.md#appintegrationsserviceservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from types_aiobotocore_appintegrations.type_defs import CreateDataIntegrationRequestRequestTypeDef

def get_value() -> CreateDataIntegrationRequestRequestTypeDef:
    return {
        "Name": ...,
    }
```

- [CreateDataIntegrationRequestRequestTypeDef](./type_defs.md#createdataintegrationrequestrequesttypedef)
- [CreateDataIntegrationResponseTypeDef](./type_defs.md#createdataintegrationresponsetypedef)
- [CreateEventIntegrationRequestRequestTypeDef](./type_defs.md#createeventintegrationrequestrequesttypedef)
- [CreateEventIntegrationResponseTypeDef](./type_defs.md#createeventintegrationresponsetypedef)
- [DataIntegrationAssociationSummaryTypeDef](./type_defs.md#dataintegrationassociationsummarytypedef)
- [DataIntegrationSummaryTypeDef](./type_defs.md#dataintegrationsummarytypedef)
- [DeleteDataIntegrationRequestRequestTypeDef](./type_defs.md#deletedataintegrationrequestrequesttypedef)
- [DeleteEventIntegrationRequestRequestTypeDef](./type_defs.md#deleteeventintegrationrequestrequesttypedef)
- [EventFilterTypeDef](./type_defs.md#eventfiltertypedef)
- [EventIntegrationAssociationTypeDef](./type_defs.md#eventintegrationassociationtypedef)
- [EventIntegrationTypeDef](./type_defs.md#eventintegrationtypedef)
- [GetDataIntegrationRequestRequestTypeDef](./type_defs.md#getdataintegrationrequestrequesttypedef)
- [GetDataIntegrationResponseTypeDef](./type_defs.md#getdataintegrationresponsetypedef)
- [GetEventIntegrationRequestRequestTypeDef](./type_defs.md#geteventintegrationrequestrequesttypedef)
- [GetEventIntegrationResponseTypeDef](./type_defs.md#geteventintegrationresponsetypedef)
- [ListDataIntegrationAssociationsRequestRequestTypeDef](./type_defs.md#listdataintegrationassociationsrequestrequesttypedef)
- [ListDataIntegrationAssociationsResponseTypeDef](./type_defs.md#listdataintegrationassociationsresponsetypedef)
- [ListDataIntegrationsRequestRequestTypeDef](./type_defs.md#listdataintegrationsrequestrequesttypedef)
- [ListDataIntegrationsResponseTypeDef](./type_defs.md#listdataintegrationsresponsetypedef)
- [ListEventIntegrationAssociationsRequestRequestTypeDef](./type_defs.md#listeventintegrationassociationsrequestrequesttypedef)
- [ListEventIntegrationAssociationsResponseTypeDef](./type_defs.md#listeventintegrationassociationsresponsetypedef)
- [ListEventIntegrationsRequestRequestTypeDef](./type_defs.md#listeventintegrationsrequestrequesttypedef)
- [ListEventIntegrationsResponseTypeDef](./type_defs.md#listeventintegrationsresponsetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ScheduleConfigurationTypeDef](./type_defs.md#scheduleconfigurationtypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateDataIntegrationRequestRequestTypeDef](./type_defs.md#updatedataintegrationrequestrequesttypedef)
- [UpdateEventIntegrationRequestRequestTypeDef](./type_defs.md#updateeventintegrationrequestrequesttypedef)


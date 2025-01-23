# Paginators

> [Index](../README.md) > [ConfigService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [ConfigService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#configservice)
    type annotations stubs module [types-aiobotocore-config](https://pypi.org/project/types-aiobotocore-config/).

## DescribeAggregateComplianceByConfigRulesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_aggregate_compliance_by_config_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeAggregateComplianceByConfigRules.html#ConfigService.Paginator.DescribeAggregateComplianceByConfigRules)

```python
# DescribeAggregateComplianceByConfigRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeAggregateComplianceByConfigRulesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeAggregateComplianceByConfigRulesPaginator = client.get_paginator("describe_aggregate_compliance_by_config_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAggregateComplianceByConfigRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeAggregateComplianceByConfigRulesPaginator](./paginators.md#describeaggregatecompliancebyconfigrulespaginator)
3. item: [:material-code-braces: DescribeAggregateComplianceByConfigRulesResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAggregateComplianceByConfigRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: ConfigRuleComplianceFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeAggregateComplianceByConfigRulesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ConfigRuleComplianceFiltersTypeDef](./type_defs.md#configrulecompliancefilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAggregateComplianceByConfigRulesResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAggregateComplianceByConfigRulesRequestPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAggregateComplianceByConfigRulesRequestPaginateTypeDef](./type_defs.md#describeaggregatecompliancebyconfigrulesrequestpaginatetypedef) 
## DescribeAggregateComplianceByConformancePacksPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_aggregate_compliance_by_conformance_packs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeAggregateComplianceByConformancePacks.html#ConfigService.Paginator.DescribeAggregateComplianceByConformancePacks)

```python
# DescribeAggregateComplianceByConformancePacksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeAggregateComplianceByConformancePacksPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeAggregateComplianceByConformancePacksPaginator = client.get_paginator("describe_aggregate_compliance_by_conformance_packs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAggregateComplianceByConformancePacksResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeAggregateComplianceByConformancePacksPaginator](./paginators.md#describeaggregatecompliancebyconformancepackspaginator)
3. item: [:material-code-braces: DescribeAggregateComplianceByConformancePacksResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconformancepacksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAggregateComplianceByConformancePacksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeAggregateComplianceByConformancePacksResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: AggregateConformancePackComplianceFiltersTypeDef](./type_defs.md#aggregateconformancepackcompliancefilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeAggregateComplianceByConformancePacksResponseTypeDef](./type_defs.md#describeaggregatecompliancebyconformancepacksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAggregateComplianceByConformancePacksRequestPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAggregateComplianceByConformancePacksRequestPaginateTypeDef](./type_defs.md#describeaggregatecompliancebyconformancepacksrequestpaginatetypedef) 
## DescribeAggregationAuthorizationsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_aggregation_authorizations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeAggregationAuthorizations.html#ConfigService.Paginator.DescribeAggregationAuthorizations)

```python
# DescribeAggregationAuthorizationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeAggregationAuthorizationsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeAggregationAuthorizationsPaginator = client.get_paginator("describe_aggregation_authorizations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeAggregationAuthorizationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeAggregationAuthorizationsPaginator](./paginators.md#describeaggregationauthorizationspaginator)
3. item: [:material-code-braces: DescribeAggregationAuthorizationsResponseTypeDef](./type_defs.md#describeaggregationauthorizationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeAggregationAuthorizationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeAggregationAuthorizationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeAggregationAuthorizationsResponseTypeDef](./type_defs.md#describeaggregationauthorizationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeAggregationAuthorizationsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeAggregationAuthorizationsRequestPaginateTypeDef](./type_defs.md#describeaggregationauthorizationsrequestpaginatetypedef) 
## DescribeComplianceByConfigRulePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_compliance_by_config_rule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeComplianceByConfigRule.html#ConfigService.Paginator.DescribeComplianceByConfigRule)

```python
# DescribeComplianceByConfigRulePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeComplianceByConfigRulePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeComplianceByConfigRulePaginator = client.get_paginator("describe_compliance_by_config_rule")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeComplianceByConfigRuleResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeComplianceByConfigRulePaginator](./paginators.md#describecompliancebyconfigrulepaginator)
3. item: [:material-code-braces: DescribeComplianceByConfigRuleResponseTypeDef](./type_defs.md#describecompliancebyconfigruleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeComplianceByConfigRulePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeComplianceByConfigRuleResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeComplianceByConfigRuleResponseTypeDef](./type_defs.md#describecompliancebyconfigruleresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeComplianceByConfigRuleRequestPaginateTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeComplianceByConfigRuleRequestPaginateTypeDef](./type_defs.md#describecompliancebyconfigrulerequestpaginatetypedef) 
## DescribeComplianceByResourcePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_compliance_by_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeComplianceByResource.html#ConfigService.Paginator.DescribeComplianceByResource)

```python
# DescribeComplianceByResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeComplianceByResourcePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeComplianceByResourcePaginator = client.get_paginator("describe_compliance_by_resource")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeComplianceByResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeComplianceByResourcePaginator](./paginators.md#describecompliancebyresourcepaginator)
3. item: [:material-code-braces: DescribeComplianceByResourceResponseTypeDef](./type_defs.md#describecompliancebyresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeComplianceByResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceType: str = ...,
    ResourceId: str = ...,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeComplianceByResourceResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeComplianceByResourceResponseTypeDef](./type_defs.md#describecompliancebyresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeComplianceByResourceRequestPaginateTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeComplianceByResourceRequestPaginateTypeDef](./type_defs.md#describecompliancebyresourcerequestpaginatetypedef) 
## DescribeConfigRuleEvaluationStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_config_rule_evaluation_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeConfigRuleEvaluationStatus.html#ConfigService.Paginator.DescribeConfigRuleEvaluationStatus)

```python
# DescribeConfigRuleEvaluationStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConfigRuleEvaluationStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConfigRuleEvaluationStatusPaginator = client.get_paginator("describe_config_rule_evaluation_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigRuleEvaluationStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConfigRuleEvaluationStatusPaginator](./paginators.md#describeconfigruleevaluationstatuspaginator)
3. item: [:material-code-braces: DescribeConfigRuleEvaluationStatusResponseTypeDef](./type_defs.md#describeconfigruleevaluationstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigRuleEvaluationStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeConfigRuleEvaluationStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConfigRuleEvaluationStatusResponseTypeDef](./type_defs.md#describeconfigruleevaluationstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConfigRuleEvaluationStatusRequestPaginateTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigRuleEvaluationStatusRequestPaginateTypeDef](./type_defs.md#describeconfigruleevaluationstatusrequestpaginatetypedef) 
## DescribeConfigRulesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_config_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeConfigRules.html#ConfigService.Paginator.DescribeConfigRules)

```python
# DescribeConfigRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConfigRulesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConfigRulesPaginator = client.get_paginator("describe_config_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConfigRulesPaginator](./paginators.md#describeconfigrulespaginator)
3. item: [:material-code-braces: DescribeConfigRulesResponseTypeDef](./type_defs.md#describeconfigrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigRuleNames: Sequence[str] = ...,
    Filters: DescribeConfigRulesFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeConfigRulesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: DescribeConfigRulesFiltersTypeDef](./type_defs.md#describeconfigrulesfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeConfigRulesResponseTypeDef](./type_defs.md#describeconfigrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConfigRulesRequestPaginateTypeDef = {  # (1)
    "ConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigRulesRequestPaginateTypeDef](./type_defs.md#describeconfigrulesrequestpaginatetypedef) 
## DescribeConfigurationAggregatorSourcesStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_configuration_aggregator_sources_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeConfigurationAggregatorSourcesStatus.html#ConfigService.Paginator.DescribeConfigurationAggregatorSourcesStatus)

```python
# DescribeConfigurationAggregatorSourcesStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConfigurationAggregatorSourcesStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConfigurationAggregatorSourcesStatusPaginator = client.get_paginator("describe_configuration_aggregator_sources_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigurationAggregatorSourcesStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConfigurationAggregatorSourcesStatusPaginator](./paginators.md#describeconfigurationaggregatorsourcesstatuspaginator)
3. item: [:material-code-braces: DescribeConfigurationAggregatorSourcesStatusResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsourcesstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigurationAggregatorSourcesStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeConfigurationAggregatorSourcesStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: AggregatedSourceStatusTypeType](./literals.md#aggregatedsourcestatustypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeConfigurationAggregatorSourcesStatusResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsourcesstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConfigurationAggregatorSourcesStatusRequestPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationAggregatorSourcesStatusRequestPaginateTypeDef](./type_defs.md#describeconfigurationaggregatorsourcesstatusrequestpaginatetypedef) 
## DescribeConfigurationAggregatorsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_configuration_aggregators")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeConfigurationAggregators.html#ConfigService.Paginator.DescribeConfigurationAggregators)

```python
# DescribeConfigurationAggregatorsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConfigurationAggregatorsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConfigurationAggregatorsPaginator = client.get_paginator("describe_configuration_aggregators")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConfigurationAggregatorsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConfigurationAggregatorsPaginator](./paginators.md#describeconfigurationaggregatorspaginator)
3. item: [:material-code-braces: DescribeConfigurationAggregatorsResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConfigurationAggregatorsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigurationAggregatorNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeConfigurationAggregatorsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConfigurationAggregatorsResponseTypeDef](./type_defs.md#describeconfigurationaggregatorsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConfigurationAggregatorsRequestPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConfigurationAggregatorsRequestPaginateTypeDef](./type_defs.md#describeconfigurationaggregatorsrequestpaginatetypedef) 
## DescribeConformancePackStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_conformance_pack_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeConformancePackStatus.html#ConfigService.Paginator.DescribeConformancePackStatus)

```python
# DescribeConformancePackStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConformancePackStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConformancePackStatusPaginator = client.get_paginator("describe_conformance_pack_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConformancePackStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConformancePackStatusPaginator](./paginators.md#describeconformancepackstatuspaginator)
3. item: [:material-code-braces: DescribeConformancePackStatusResponseTypeDef](./type_defs.md#describeconformancepackstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConformancePackStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConformancePackNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeConformancePackStatusResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConformancePackStatusResponseTypeDef](./type_defs.md#describeconformancepackstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConformancePackStatusRequestPaginateTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConformancePackStatusRequestPaginateTypeDef](./type_defs.md#describeconformancepackstatusrequestpaginatetypedef) 
## DescribeConformancePacksPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_conformance_packs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeConformancePacks.html#ConfigService.Paginator.DescribeConformancePacks)

```python
# DescribeConformancePacksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeConformancePacksPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeConformancePacksPaginator = client.get_paginator("describe_conformance_packs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeConformancePacksResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeConformancePacksPaginator](./paginators.md#describeconformancepackspaginator)
3. item: [:material-code-braces: DescribeConformancePacksResponseTypeDef](./type_defs.md#describeconformancepacksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeConformancePacksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConformancePackNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeConformancePacksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeConformancePacksResponseTypeDef](./type_defs.md#describeconformancepacksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeConformancePacksRequestPaginateTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeConformancePacksRequestPaginateTypeDef](./type_defs.md#describeconformancepacksrequestpaginatetypedef) 
## DescribeOrganizationConfigRuleStatusesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_organization_config_rule_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeOrganizationConfigRuleStatuses.html#ConfigService.Paginator.DescribeOrganizationConfigRuleStatuses)

```python
# DescribeOrganizationConfigRuleStatusesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeOrganizationConfigRuleStatusesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeOrganizationConfigRuleStatusesPaginator = client.get_paginator("describe_organization_config_rule_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationConfigRuleStatusesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeOrganizationConfigRuleStatusesPaginator](./paginators.md#describeorganizationconfigrulestatusespaginator)
3. item: [:material-code-braces: DescribeOrganizationConfigRuleStatusesResponseTypeDef](./type_defs.md#describeorganizationconfigrulestatusesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationConfigRuleStatusesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationConfigRuleNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeOrganizationConfigRuleStatusesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrganizationConfigRuleStatusesResponseTypeDef](./type_defs.md#describeorganizationconfigrulestatusesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOrganizationConfigRuleStatusesRequestPaginateTypeDef = {  # (1)
    "OrganizationConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConfigRuleStatusesRequestPaginateTypeDef](./type_defs.md#describeorganizationconfigrulestatusesrequestpaginatetypedef) 
## DescribeOrganizationConfigRulesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_organization_config_rules")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeOrganizationConfigRules.html#ConfigService.Paginator.DescribeOrganizationConfigRules)

```python
# DescribeOrganizationConfigRulesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeOrganizationConfigRulesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeOrganizationConfigRulesPaginator = client.get_paginator("describe_organization_config_rules")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationConfigRulesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeOrganizationConfigRulesPaginator](./paginators.md#describeorganizationconfigrulespaginator)
3. item: [:material-code-braces: DescribeOrganizationConfigRulesResponseTypeDef](./type_defs.md#describeorganizationconfigrulesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationConfigRulesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationConfigRuleNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeOrganizationConfigRulesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrganizationConfigRulesResponseTypeDef](./type_defs.md#describeorganizationconfigrulesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOrganizationConfigRulesRequestPaginateTypeDef = {  # (1)
    "OrganizationConfigRuleNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConfigRulesRequestPaginateTypeDef](./type_defs.md#describeorganizationconfigrulesrequestpaginatetypedef) 
## DescribeOrganizationConformancePackStatusesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_organization_conformance_pack_statuses")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeOrganizationConformancePackStatuses.html#ConfigService.Paginator.DescribeOrganizationConformancePackStatuses)

```python
# DescribeOrganizationConformancePackStatusesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeOrganizationConformancePackStatusesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeOrganizationConformancePackStatusesPaginator = client.get_paginator("describe_organization_conformance_pack_statuses")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationConformancePackStatusesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeOrganizationConformancePackStatusesPaginator](./paginators.md#describeorganizationconformancepackstatusespaginator)
3. item: [:material-code-braces: DescribeOrganizationConformancePackStatusesResponseTypeDef](./type_defs.md#describeorganizationconformancepackstatusesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationConformancePackStatusesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationConformancePackNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeOrganizationConformancePackStatusesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrganizationConformancePackStatusesResponseTypeDef](./type_defs.md#describeorganizationconformancepackstatusesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOrganizationConformancePackStatusesRequestPaginateTypeDef = {  # (1)
    "OrganizationConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConformancePackStatusesRequestPaginateTypeDef](./type_defs.md#describeorganizationconformancepackstatusesrequestpaginatetypedef) 
## DescribeOrganizationConformancePacksPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_organization_conformance_packs")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeOrganizationConformancePacks.html#ConfigService.Paginator.DescribeOrganizationConformancePacks)

```python
# DescribeOrganizationConformancePacksPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeOrganizationConformancePacksPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeOrganizationConformancePacksPaginator = client.get_paginator("describe_organization_conformance_packs")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeOrganizationConformancePacksResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeOrganizationConformancePacksPaginator](./paginators.md#describeorganizationconformancepackspaginator)
3. item: [:material-code-braces: DescribeOrganizationConformancePacksResponseTypeDef](./type_defs.md#describeorganizationconformancepacksresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeOrganizationConformancePacksPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationConformancePackNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeOrganizationConformancePacksResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeOrganizationConformancePacksResponseTypeDef](./type_defs.md#describeorganizationconformancepacksresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeOrganizationConformancePacksRequestPaginateTypeDef = {  # (1)
    "OrganizationConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeOrganizationConformancePacksRequestPaginateTypeDef](./type_defs.md#describeorganizationconformancepacksrequestpaginatetypedef) 
## DescribePendingAggregationRequestsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_pending_aggregation_requests")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribePendingAggregationRequests.html#ConfigService.Paginator.DescribePendingAggregationRequests)

```python
# DescribePendingAggregationRequestsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribePendingAggregationRequestsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribePendingAggregationRequestsPaginator = client.get_paginator("describe_pending_aggregation_requests")  # (2)
    async for item in paginator.paginate(...):
        item: DescribePendingAggregationRequestsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribePendingAggregationRequestsPaginator](./paginators.md#describependingaggregationrequestspaginator)
3. item: [:material-code-braces: DescribePendingAggregationRequestsResponseTypeDef](./type_defs.md#describependingaggregationrequestsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribePendingAggregationRequestsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribePendingAggregationRequestsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribePendingAggregationRequestsResponseTypeDef](./type_defs.md#describependingaggregationrequestsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribePendingAggregationRequestsRequestPaginateTypeDef = {  # (1)
    "PaginationConfig": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribePendingAggregationRequestsRequestPaginateTypeDef](./type_defs.md#describependingaggregationrequestsrequestpaginatetypedef) 
## DescribeRemediationExecutionStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_remediation_execution_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeRemediationExecutionStatus.html#ConfigService.Paginator.DescribeRemediationExecutionStatus)

```python
# DescribeRemediationExecutionStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeRemediationExecutionStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeRemediationExecutionStatusPaginator = client.get_paginator("describe_remediation_execution_status")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRemediationExecutionStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeRemediationExecutionStatusPaginator](./paginators.md#describeremediationexecutionstatuspaginator)
3. item: [:material-code-braces: DescribeRemediationExecutionStatusResponseTypeDef](./type_defs.md#describeremediationexecutionstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRemediationExecutionStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigRuleName: str,
    ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[DescribeRemediationExecutionStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceKeyTypeDef](./type_defs.md#resourcekeytypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: DescribeRemediationExecutionStatusResponseTypeDef](./type_defs.md#describeremediationexecutionstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRemediationExecutionStatusRequestPaginateTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRemediationExecutionStatusRequestPaginateTypeDef](./type_defs.md#describeremediationexecutionstatusrequestpaginatetypedef) 
## DescribeRetentionConfigurationsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("describe_retention_configurations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/DescribeRetentionConfigurations.html#ConfigService.Paginator.DescribeRetentionConfigurations)

```python
# DescribeRetentionConfigurationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import DescribeRetentionConfigurationsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: DescribeRetentionConfigurationsPaginator = client.get_paginator("describe_retention_configurations")  # (2)
    async for item in paginator.paginate(...):
        item: DescribeRetentionConfigurationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [DescribeRetentionConfigurationsPaginator](./paginators.md#describeretentionconfigurationspaginator)
3. item: [:material-code-braces: DescribeRetentionConfigurationsResponseTypeDef](./type_defs.md#describeretentionconfigurationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python DescribeRetentionConfigurationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    RetentionConfigurationNames: Sequence[str] = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[DescribeRetentionConfigurationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: DescribeRetentionConfigurationsResponseTypeDef](./type_defs.md#describeretentionconfigurationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: DescribeRetentionConfigurationsRequestPaginateTypeDef = {  # (1)
    "RetentionConfigurationNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: DescribeRetentionConfigurationsRequestPaginateTypeDef](./type_defs.md#describeretentionconfigurationsrequestpaginatetypedef) 
## GetAggregateComplianceDetailsByConfigRulePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_aggregate_compliance_details_by_config_rule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/GetAggregateComplianceDetailsByConfigRule.html#ConfigService.Paginator.GetAggregateComplianceDetailsByConfigRule)

```python
# GetAggregateComplianceDetailsByConfigRulePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetAggregateComplianceDetailsByConfigRulePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetAggregateComplianceDetailsByConfigRulePaginator = client.get_paginator("get_aggregate_compliance_details_by_config_rule")  # (2)
    async for item in paginator.paginate(...):
        item: GetAggregateComplianceDetailsByConfigRuleResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetAggregateComplianceDetailsByConfigRulePaginator](./paginators.md#getaggregatecompliancedetailsbyconfigrulepaginator)
3. item: [:material-code-braces: GetAggregateComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getaggregatecompliancedetailsbyconfigruleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetAggregateComplianceDetailsByConfigRulePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    ConfigRuleName: str,
    AccountId: str,
    AwsRegion: str,
    ComplianceType: ComplianceTypeType = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetAggregateComplianceDetailsByConfigRuleResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetAggregateComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getaggregatecompliancedetailsbyconfigruleresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetAggregateComplianceDetailsByConfigRuleRequestPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
    "ConfigRuleName": ...,
    "AccountId": ...,
    "AwsRegion": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetAggregateComplianceDetailsByConfigRuleRequestPaginateTypeDef](./type_defs.md#getaggregatecompliancedetailsbyconfigrulerequestpaginatetypedef) 
## GetComplianceDetailsByConfigRulePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_compliance_details_by_config_rule")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/GetComplianceDetailsByConfigRule.html#ConfigService.Paginator.GetComplianceDetailsByConfigRule)

```python
# GetComplianceDetailsByConfigRulePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetComplianceDetailsByConfigRulePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetComplianceDetailsByConfigRulePaginator = client.get_paginator("get_compliance_details_by_config_rule")  # (2)
    async for item in paginator.paginate(...):
        item: GetComplianceDetailsByConfigRuleResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetComplianceDetailsByConfigRulePaginator](./paginators.md#getcompliancedetailsbyconfigrulepaginator)
3. item: [:material-code-braces: GetComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getcompliancedetailsbyconfigruleresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetComplianceDetailsByConfigRulePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigRuleName: str,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetComplianceDetailsByConfigRuleResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetComplianceDetailsByConfigRuleResponseTypeDef](./type_defs.md#getcompliancedetailsbyconfigruleresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetComplianceDetailsByConfigRuleRequestPaginateTypeDef = {  # (1)
    "ConfigRuleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetComplianceDetailsByConfigRuleRequestPaginateTypeDef](./type_defs.md#getcompliancedetailsbyconfigrulerequestpaginatetypedef) 
## GetComplianceDetailsByResourcePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_compliance_details_by_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/GetComplianceDetailsByResource.html#ConfigService.Paginator.GetComplianceDetailsByResource)

```python
# GetComplianceDetailsByResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetComplianceDetailsByResourcePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetComplianceDetailsByResourcePaginator = client.get_paginator("get_compliance_details_by_resource")  # (2)
    async for item in paginator.paginate(...):
        item: GetComplianceDetailsByResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetComplianceDetailsByResourcePaginator](./paginators.md#getcompliancedetailsbyresourcepaginator)
3. item: [:material-code-braces: GetComplianceDetailsByResourceResponseTypeDef](./type_defs.md#getcompliancedetailsbyresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetComplianceDetailsByResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceType: str = ...,
    ResourceId: str = ...,
    ComplianceTypes: Sequence[ComplianceTypeType] = ...,  # (1)
    ResourceEvaluationId: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetComplianceDetailsByResourceResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ComplianceTypeType](./literals.md#compliancetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetComplianceDetailsByResourceResponseTypeDef](./type_defs.md#getcompliancedetailsbyresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetComplianceDetailsByResourceRequestPaginateTypeDef = {  # (1)
    "ResourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetComplianceDetailsByResourceRequestPaginateTypeDef](./type_defs.md#getcompliancedetailsbyresourcerequestpaginatetypedef) 
## GetConformancePackComplianceSummaryPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_conformance_pack_compliance_summary")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/GetConformancePackComplianceSummary.html#ConfigService.Paginator.GetConformancePackComplianceSummary)

```python
# GetConformancePackComplianceSummaryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetConformancePackComplianceSummaryPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetConformancePackComplianceSummaryPaginator = client.get_paginator("get_conformance_pack_compliance_summary")  # (2)
    async for item in paginator.paginate(...):
        item: GetConformancePackComplianceSummaryResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetConformancePackComplianceSummaryPaginator](./paginators.md#getconformancepackcompliancesummarypaginator)
3. item: [:material-code-braces: GetConformancePackComplianceSummaryResponseTypeDef](./type_defs.md#getconformancepackcompliancesummaryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetConformancePackComplianceSummaryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConformancePackNames: Sequence[str],
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[GetConformancePackComplianceSummaryResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetConformancePackComplianceSummaryResponseTypeDef](./type_defs.md#getconformancepackcompliancesummaryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetConformancePackComplianceSummaryRequestPaginateTypeDef = {  # (1)
    "ConformancePackNames": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetConformancePackComplianceSummaryRequestPaginateTypeDef](./type_defs.md#getconformancepackcompliancesummaryrequestpaginatetypedef) 
## GetOrganizationConfigRuleDetailedStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_organization_config_rule_detailed_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/GetOrganizationConfigRuleDetailedStatus.html#ConfigService.Paginator.GetOrganizationConfigRuleDetailedStatus)

```python
# GetOrganizationConfigRuleDetailedStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetOrganizationConfigRuleDetailedStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetOrganizationConfigRuleDetailedStatusPaginator = client.get_paginator("get_organization_config_rule_detailed_status")  # (2)
    async for item in paginator.paginate(...):
        item: GetOrganizationConfigRuleDetailedStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetOrganizationConfigRuleDetailedStatusPaginator](./paginators.md#getorganizationconfigruledetailedstatuspaginator)
3. item: [:material-code-braces: GetOrganizationConfigRuleDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconfigruledetailedstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetOrganizationConfigRuleDetailedStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationConfigRuleName: str,
    Filters: StatusDetailFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetOrganizationConfigRuleDetailedStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: StatusDetailFiltersTypeDef](./type_defs.md#statusdetailfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetOrganizationConfigRuleDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconfigruledetailedstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetOrganizationConfigRuleDetailedStatusRequestPaginateTypeDef = {  # (1)
    "OrganizationConfigRuleName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOrganizationConfigRuleDetailedStatusRequestPaginateTypeDef](./type_defs.md#getorganizationconfigruledetailedstatusrequestpaginatetypedef) 
## GetOrganizationConformancePackDetailedStatusPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_organization_conformance_pack_detailed_status")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/GetOrganizationConformancePackDetailedStatus.html#ConfigService.Paginator.GetOrganizationConformancePackDetailedStatus)

```python
# GetOrganizationConformancePackDetailedStatusPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetOrganizationConformancePackDetailedStatusPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetOrganizationConformancePackDetailedStatusPaginator = client.get_paginator("get_organization_conformance_pack_detailed_status")  # (2)
    async for item in paginator.paginate(...):
        item: GetOrganizationConformancePackDetailedStatusResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetOrganizationConformancePackDetailedStatusPaginator](./paginators.md#getorganizationconformancepackdetailedstatuspaginator)
3. item: [:material-code-braces: GetOrganizationConformancePackDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconformancepackdetailedstatusresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetOrganizationConformancePackDetailedStatusPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    OrganizationConformancePackName: str,
    Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[GetOrganizationConformancePackDetailedStatusResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: OrganizationResourceDetailedStatusFiltersTypeDef](./type_defs.md#organizationresourcedetailedstatusfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetOrganizationConformancePackDetailedStatusResponseTypeDef](./type_defs.md#getorganizationconformancepackdetailedstatusresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetOrganizationConformancePackDetailedStatusRequestPaginateTypeDef = {  # (1)
    "OrganizationConformancePackName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetOrganizationConformancePackDetailedStatusRequestPaginateTypeDef](./type_defs.md#getorganizationconformancepackdetailedstatusrequestpaginatetypedef) 
## GetResourceConfigHistoryPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("get_resource_config_history")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/GetResourceConfigHistory.html#ConfigService.Paginator.GetResourceConfigHistory)

```python
# GetResourceConfigHistoryPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import GetResourceConfigHistoryPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: GetResourceConfigHistoryPaginator = client.get_paginator("get_resource_config_history")  # (2)
    async for item in paginator.paginate(...):
        item: GetResourceConfigHistoryResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [GetResourceConfigHistoryPaginator](./paginators.md#getresourceconfighistorypaginator)
3. item: [:material-code-braces: GetResourceConfigHistoryResponseTypeDef](./type_defs.md#getresourceconfighistoryresponsetypedef) 


### paginate

Type annotations and code completion for `#!python GetResourceConfigHistoryPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    resourceId: str,
    laterTime: TimestampTypeDef = ...,
    earlierTime: TimestampTypeDef = ...,
    chronologicalOrder: ChronologicalOrderType = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[GetResourceConfigHistoryResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-brackets: ChronologicalOrderType](./literals.md#chronologicalordertype) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: GetResourceConfigHistoryResponseTypeDef](./type_defs.md#getresourceconfighistoryresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: GetResourceConfigHistoryRequestPaginateTypeDef = {  # (1)
    "resourceType": ...,
    "resourceId": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetResourceConfigHistoryRequestPaginateTypeDef](./type_defs.md#getresourceconfighistoryrequestpaginatetypedef) 
## ListAggregateDiscoveredResourcesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("list_aggregate_discovered_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/ListAggregateDiscoveredResources.html#ConfigService.Paginator.ListAggregateDiscoveredResources)

```python
# ListAggregateDiscoveredResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import ListAggregateDiscoveredResourcesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: ListAggregateDiscoveredResourcesPaginator = client.get_paginator("list_aggregate_discovered_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListAggregateDiscoveredResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [ListAggregateDiscoveredResourcesPaginator](./paginators.md#listaggregatediscoveredresourcespaginator)
3. item: [:material-code-braces: ListAggregateDiscoveredResourcesResponseTypeDef](./type_defs.md#listaggregatediscoveredresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListAggregateDiscoveredResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ConfigurationAggregatorName: str,
    ResourceType: ResourceTypeType,  # (1)
    Filters: ResourceFiltersTypeDef = ...,  # (2)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (3)
) -> AioPageIterator[ListAggregateDiscoveredResourcesResponseTypeDef]:  # (4)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: ResourceFiltersTypeDef](./type_defs.md#resourcefilterstypedef) 
3. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
4. See [:material-code-braces: ListAggregateDiscoveredResourcesResponseTypeDef](./type_defs.md#listaggregatediscoveredresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListAggregateDiscoveredResourcesRequestPaginateTypeDef = {  # (1)
    "ConfigurationAggregatorName": ...,
    "ResourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListAggregateDiscoveredResourcesRequestPaginateTypeDef](./type_defs.md#listaggregatediscoveredresourcesrequestpaginatetypedef) 
## ListConfigurationRecordersPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("list_configuration_recorders")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/ListConfigurationRecorders.html#ConfigService.Paginator.ListConfigurationRecorders)

```python
# ListConfigurationRecordersPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import ListConfigurationRecordersPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: ListConfigurationRecordersPaginator = client.get_paginator("list_configuration_recorders")  # (2)
    async for item in paginator.paginate(...):
        item: ListConfigurationRecordersResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [ListConfigurationRecordersPaginator](./paginators.md#listconfigurationrecorderspaginator)
3. item: [:material-code-braces: ListConfigurationRecordersResponseTypeDef](./type_defs.md#listconfigurationrecordersresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListConfigurationRecordersPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: Sequence[ConfigurationRecorderFilterTypeDef] = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListConfigurationRecordersResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ConfigurationRecorderFilterTypeDef](./type_defs.md#configurationrecorderfiltertypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListConfigurationRecordersResponseTypeDef](./type_defs.md#listconfigurationrecordersresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListConfigurationRecordersRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListConfigurationRecordersRequestPaginateTypeDef](./type_defs.md#listconfigurationrecordersrequestpaginatetypedef) 
## ListDiscoveredResourcesPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("list_discovered_resources")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/ListDiscoveredResources.html#ConfigService.Paginator.ListDiscoveredResources)

```python
# ListDiscoveredResourcesPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import ListDiscoveredResourcesPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: ListDiscoveredResourcesPaginator = client.get_paginator("list_discovered_resources")  # (2)
    async for item in paginator.paginate(...):
        item: ListDiscoveredResourcesResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [ListDiscoveredResourcesPaginator](./paginators.md#listdiscoveredresourcespaginator)
3. item: [:material-code-braces: ListDiscoveredResourcesResponseTypeDef](./type_defs.md#listdiscoveredresourcesresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListDiscoveredResourcesPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    resourceType: ResourceTypeType,  # (1)
    resourceIds: Sequence[str] = ...,
    resourceName: str = ...,
    includeDeletedResources: bool = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListDiscoveredResourcesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: ResourceTypeType](./literals.md#resourcetypetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListDiscoveredResourcesResponseTypeDef](./type_defs.md#listdiscoveredresourcesresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListDiscoveredResourcesRequestPaginateTypeDef = {  # (1)
    "resourceType": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListDiscoveredResourcesRequestPaginateTypeDef](./type_defs.md#listdiscoveredresourcesrequestpaginatetypedef) 
## ListResourceEvaluationsPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("list_resource_evaluations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/ListResourceEvaluations.html#ConfigService.Paginator.ListResourceEvaluations)

```python
# ListResourceEvaluationsPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import ListResourceEvaluationsPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: ListResourceEvaluationsPaginator = client.get_paginator("list_resource_evaluations")  # (2)
    async for item in paginator.paginate(...):
        item: ListResourceEvaluationsResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [ListResourceEvaluationsPaginator](./paginators.md#listresourceevaluationspaginator)
3. item: [:material-code-braces: ListResourceEvaluationsResponseTypeDef](./type_defs.md#listresourceevaluationsresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListResourceEvaluationsPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Filters: ResourceEvaluationFiltersTypeDef = ...,  # (1)
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> AioPageIterator[ListResourceEvaluationsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-braces: ResourceEvaluationFiltersTypeDef](./type_defs.md#resourceevaluationfilterstypedef) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: ListResourceEvaluationsResponseTypeDef](./type_defs.md#listresourceevaluationsresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListResourceEvaluationsRequestPaginateTypeDef = {  # (1)
    "Filters": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListResourceEvaluationsRequestPaginateTypeDef](./type_defs.md#listresourceevaluationsrequestpaginatetypedef) 
## ListTagsForResourcePaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("list_tags_for_resource")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/ListTagsForResource.html#ConfigService.Paginator.ListTagsForResource)

```python
# ListTagsForResourcePaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import ListTagsForResourcePaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")  # (2)
    async for item in paginator.paginate(...):
        item: ListTagsForResourceResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [ListTagsForResourcePaginator](./paginators.md#listtagsforresourcepaginator)
3. item: [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


### paginate

Type annotations and code completion for `#!python ListTagsForResourcePaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    ResourceArn: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[ListTagsForResourceResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: ListTagsForResourceRequestPaginateTypeDef = {  # (1)
    "ResourceArn": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: ListTagsForResourceRequestPaginateTypeDef](./type_defs.md#listtagsforresourcerequestpaginatetypedef) 
## SelectAggregateResourceConfigPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("select_aggregate_resource_config")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/SelectAggregateResourceConfig.html#ConfigService.Paginator.SelectAggregateResourceConfig)

```python
# SelectAggregateResourceConfigPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import SelectAggregateResourceConfigPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: SelectAggregateResourceConfigPaginator = client.get_paginator("select_aggregate_resource_config")  # (2)
    async for item in paginator.paginate(...):
        item: SelectAggregateResourceConfigResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [SelectAggregateResourceConfigPaginator](./paginators.md#selectaggregateresourceconfigpaginator)
3. item: [:material-code-braces: SelectAggregateResourceConfigResponseTypeDef](./type_defs.md#selectaggregateresourceconfigresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SelectAggregateResourceConfigPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Expression: str,
    ConfigurationAggregatorName: str,
    MaxResults: int = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SelectAggregateResourceConfigResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SelectAggregateResourceConfigResponseTypeDef](./type_defs.md#selectaggregateresourceconfigresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SelectAggregateResourceConfigRequestPaginateTypeDef = {  # (1)
    "Expression": ...,
    "ConfigurationAggregatorName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SelectAggregateResourceConfigRequestPaginateTypeDef](./type_defs.md#selectaggregateresourceconfigrequestpaginatetypedef) 
## SelectResourceConfigPaginator

Type annotations and code completion for `#!python session.create_client("config").get_paginator("select_resource_config")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config/paginator/SelectResourceConfig.html#ConfigService.Paginator.SelectResourceConfig)

```python
# SelectResourceConfigPaginator usage example

from aiobotocore.session import get_session

from types_aiobotocore_config.paginator import SelectResourceConfigPaginator

session = get_session()
async with session.create_client("config") as client:  # (1)
    paginator: SelectResourceConfigPaginator = client.get_paginator("select_resource_config")  # (2)
    async for item in paginator.paginate(...):
        item: SelectResourceConfigResponseTypeDef
        print(item)  # (3)
```

1. client: [ConfigServiceClient](./client.md)
2. paginator: [SelectResourceConfigPaginator](./paginators.md#selectresourceconfigpaginator)
3. item: [:material-code-braces: SelectResourceConfigResponseTypeDef](./type_defs.md#selectresourceconfigresponsetypedef) 


### paginate

Type annotations and code completion for `#!python SelectResourceConfigPaginator.paginate` method.

```python
# paginate method definition

def paginate(
    self,
    *,
    Expression: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> AioPageIterator[SelectResourceConfigResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: SelectResourceConfigResponseTypeDef](./type_defs.md#selectresourceconfigresponsetypedef) 


```python
# paginate method usage example with argument unpacking

kwargs: SelectResourceConfigRequestPaginateTypeDef = {  # (1)
    "Expression": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: SelectResourceConfigRequestPaginateTypeDef](./type_defs.md#selectresourceconfigrequestpaginatetypedef) 

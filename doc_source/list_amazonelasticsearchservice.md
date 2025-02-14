# Actions, Resources, and Condition Keys for Amazon Elasticsearch Service<a name="list_amazonelasticsearchservice"></a>

Amazon Elasticsearch Service \(service prefix: `es`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/)\.
+ View a list of the [API operations available for this service](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html)\.

**Topics**
+ [Actions Defined by Amazon Elasticsearch Service](#amazonelasticsearchservice-actions-as-permissions)
+ [Resources Defined by Amazon Elasticsearch Service](#amazonelasticsearchservice-resources-for-iam-policies)
+ [Condition Keys for Amazon Elasticsearch Service](#amazonelasticsearchservice-policy-keys)

## Actions Defined by Amazon Elasticsearch Service<a name="amazonelasticsearchservice-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. Use policies to grant permissions to perform an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\.

The **Resource** column indicates whether each action supports resource\-level permissions\. If there is no value for this column, you must specify all resources \("\*"\) in the `Resource` element of your policy statement\. If the column includes a resource type, then you can specify an ARN of that type in a statement with that action\. Required resources are indicated in the table with an asterisk \(\*\)\. If you specify a resource\-level permission ARN in a statement using this action, then it must be of this type\. Some actions support multiple resource types\. If the resource type is optional \(not indicated as required\), then you can choose to use one but not the other\.

For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access Level | Resource Types \(\*required\) | Condition Keys | Dependent Actions | 
| --- | --- | --- | --- | --- | --- | 
|   [ AddTags ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-addtags)  | Grants permission to attach resource tags to an Amazon ES domain\. | Tagging |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ CreateElasticsearchDomain ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-createelasticsearchdomain)  | Grants permission to create an Amazon ES domain\. | Write |   [ domain ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ DeleteElasticsearchDomain ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-deleteelasticsearchdomain)  | Grants permission to delete an Amazon ES domain and all of its data\. | Write |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ DeleteElasticsearchServiceRole ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-deleteelasticsearchservicerole)  | Grants permission to delete the service\-linked role required for Amazon ES domains that use VPC access\. | Write |  |  |  | 
|   [ DescribeElasticsearchDomain ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-describeelasticsearchdomain)  | Grants permission to view a description of the domain configuration for the specified Amazon ES domain, including the domain ID, domain service endpoint, and domain ARN\. | Read |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ DescribeElasticsearchDomainConfig ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-describeelasticsearchdomainconfig)  | Grants permission to view a description of the configuration options and status of an Amazon ES domain\. | Read |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ DescribeElasticsearchDomains ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-describeelasticsearchdomain)  | Grants permission to view a description of the domain configuration for up to five specified Amazon ES domains\. | List |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ DescribeElasticsearchInstanceTypeLimits ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-describeinstancetypelimits)  | Grants permission to view the instance count, storage, and master node limits for a given Elasticsearch version and instance type\. | List |  |  |  | 
|   [ DescribeReservedElasticsearchInstanceOfferings ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-describereservedelasticsearchinstanceofferings)  | Grants permission to fetch reserved instance offerings for ES | List |  |  |  | 
|   [ DescribeReservedElasticsearchInstances ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-describereservedelasticsearchinstances)  | Grants permission to fetch ES reserved instances already purchased by customer | List |  |  |  | 
|   ESHttpDelete  | Grants permission to send HTTP DELETE requests to the Elasticsearch APIs\. | Write |   [ domain ](#amazonelasticsearchservice-domain)   |  |  | 
|   ESHttpGet  | Grants permission to send HTTP GET requests to the Elasticsearch APIs\. | Read |   [ domain ](#amazonelasticsearchservice-domain)   |  |  | 
|   ESHttpHead  | Grants permission to send HTTP HEAD requests to the Elasticsearch APIs\. | Read |   [ domain ](#amazonelasticsearchservice-domain)   |  |  | 
|   ESHttpPost  | Grants permission to send HTTP POST requests to the Elasticsearch APIs\. | Write |   [ domain ](#amazonelasticsearchservice-domain)   |  |  | 
|   ESHttpPut  | Grants permission to send HTTP PUT requests to the Elasticsearch APIs\. | Write |   [ domain ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ GetCompatibleElasticsearchVersions ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-getcompatibleelasticsearchversions)  | Grants permission to fetch list of compatible elastic search versions to which Amazon ES domain can be upgraded | List |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ GetUpgradeHistory ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-getupgradehistory)  | Grants permission to fetch upgrade history for given ES domain | Read |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ GetUpgradeStatus ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-getupgradestatus)  | Grants permission to fetch upgrade status for given ES domain | Read |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ ListDomainNames ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-listdomainnames)  | Grants permission to display the names of all Amazon ES domains that the current user owns\. | List |  |  |  | 
|   [ ListElasticsearchInstanceTypes ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-listelasticsearchinstancetypes)  | Grants permission to list all Elasticsearch instance types that are supported for a given Elasticsearch version\. | List |  |  |  | 
|   [ ListElasticsearchVersions ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-listelasticsearchversions)  | Grants permission to list all supported Elasticsearch versions on Amazon ES\. | List |  |  |  | 
|   [ ListTags ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-listtags)  | Grants permission to display all of the tags for an Amazon ES domain\. | Read |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ PurchaseReservedElasticsearchInstance ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-purchasereservedelasticsearchinstance)  | Grants permission to purchase ES reserved instances | Write |  |  |  | 
|   [ RemoveTags ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-listtags)  | Grants permission to remove tags from Amazon ES domains\. | Tagging |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ UpdateElasticsearchDomainConfig ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-updateelasticsearchdomainconfig)  | Grants permission to modify the configuration of an Amazon ES domain, such as the instance type or number of instances\. | Write |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 
|   [ UpgradeElasticsearchDomain ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-configuration-api.html#es-configuration-api-actions-upgradeelasticsearchdomain)  | Grants permission to initiate upgrade of elastic search domain to given version | Write |   [ domain\* ](#amazonelasticsearchservice-domain)   |  |  | 

## Resources Defined by Amazon Elasticsearch Service<a name="amazonelasticsearchservice-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonelasticsearchservice-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ domain ](https://docs.aws.amazon.com/elasticsearch-service/latest/developerguide/es-ac.html)  |  arn:$\{Partition\}:es:$\{Region\}:$\{Account\}:domain/$\{DomainName\}  |  | 

## Condition Keys for Amazon Elasticsearch Service<a name="amazonelasticsearchservice-policy-keys"></a>

Elasticsearch Service has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available Keys for Conditions](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.
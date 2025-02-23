# Actions, Resources, and Condition Keys for Amazon GuardDuty<a name="list_amazonguardduty"></a>

Amazon GuardDuty \(service prefix: `guardduty`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/guardduty/latest/ug/what-is-guardduty.html)\.
+ View a list of the [API operations available for this service](https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_api_ref.html)\.
+ Learn how to secure this service and its resources by [using IAM](https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_managing_access.html) permission policies\.

**Topics**
+ [Actions Defined by Amazon GuardDuty](#amazonguardduty-actions-as-permissions)
+ [Resources Defined by Amazon GuardDuty](#amazonguardduty-resources-for-iam-policies)
+ [Condition Keys for Amazon GuardDuty](#amazonguardduty-policy-keys)

## Actions Defined by Amazon GuardDuty<a name="amazonguardduty-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. Use policies to grant permissions to perform an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\.

The **Resource** column indicates whether each action supports resource\-level permissions\. If there is no value for this column, you must specify all resources \("\*"\) in the `Resource` element of your policy statement\. If the column includes a resource type, then you can specify an ARN of that type in a statement with that action\. Required resources are indicated in the table with an asterisk \(\*\)\. If you specify a resource\-level permission ARN in a statement using this action, then it must be of this type\. Some actions support multiple resource types\. If the resource type is optional \(not indicated as required\), then you can choose to use one but not the other\.

For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_amazonguardduty.html)

## Resources Defined by Amazon GuardDuty<a name="amazonguardduty-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#amazonguardduty-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ detector ](https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_managing_access.html#guardduty-resources)  |  arn:$\{Partition\}:guardduty:$\{Region\}:$\{Account\}:detector/$\{DetectorId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonguardduty-aws_ResourceTag___TagKey_)   | 
|   [ filter ](https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_managing_access.html#guardduty-resources)  |  arn:$\{Partition\}:guardduty:$\{Region\}:$\{Account\}:detector/$\{DetectorId\}/filter/$\{FilterName\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonguardduty-aws_ResourceTag___TagKey_)   | 
|   [ ipset ](https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_managing_access.html#guardduty-resources)  |  arn:$\{Partition\}:guardduty:$\{Region\}:$\{Account\}:detector/$\{DetectorId\}/ipset/$\{IPSetId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonguardduty-aws_ResourceTag___TagKey_)   | 
|   [ threatintelset ](https://docs.aws.amazon.com/guardduty/latest/ug/guardduty_managing_access.html#guardduty-resources)  |  arn:$\{Partition\}:guardduty:$\{Region\}:$\{Account\}:detector/$\{DetectorId\}/threatintelset/$\{ThreatIntelSetId\}  |   [ aws:ResourceTag/$\{TagKey\} ](#amazonguardduty-aws_ResourceTag___TagKey_)   | 

## Condition Keys for Amazon GuardDuty<a name="amazonguardduty-policy-keys"></a>

Amazon GuardDuty defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   [ aws:RequestTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-requesttag)  | Filters actions based on the presence of tag key\-value pairs in the request | String | 
|   [ aws:ResourceTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-resourcetag)  | Filters actions based on tag key\-value pairs attached to the resource | String | 
|   [ aws:TagKeys ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-tagkeys)  | Filters actions based on the presence of tag keys in the request | String | 
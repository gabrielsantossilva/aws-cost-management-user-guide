# User\-Defined Cost Allocation Tags<a name="custom-tags"></a>

User\-defined tags are tags that you define, create, and apply to resources\. After you have created and applied them, you can activate them on the Billing and Cost Management console for cost allocation tracking\. After you activate them, they appear on your cost allocation report\. You can then use the tags on your cost allocation report to track your AWS costs\. Tags are not applied to resources that were created before the tags were created\.

**Note**  
As a best practice, do not include sensitive information in tags\.
Only master accounts in an organization and single accounts that aren't members of an organization have access to the **Cost Allocation Tags** manager in the Billing and Cost Management console\.

## Applying User\-Defined Cost Allocation Tags<a name="allocation-how"></a>

For ease of use and best results, use the AWS Tag Editor to create and apply user\-defined tags\. The Tag Editor provides a central, unified way to create and manage your user\-defined tags\. For more information, see [Working with Tag Editor](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/tag-editor.html) in the [AWS Resource Groups User Guide](https://docs.aws.amazon.com/ARG/latest/userguide/welcome.html)\.

For supported services, you can also apply tags to resources using the API or the AWS Management Console\. Each AWS service has its own implementation of tags\. You can work with these implementations individually or use Tag Editor to simplify the process\. For a full list of services that support tags, see [Supported Resources for Tag\-based Groups](https://docs.aws.amazon.com/ARG/latest/userguide/supported-resources.html#supported-resources-console-tagbased) and [Resource Groups Tagging API Reference](https://docs.aws.amazon.com/resourcegroupstagging/latest/APIReference/Welcome.html)\.

After you create and apply user\-defined tags, you can activate them for cost allocation\. If you activate your tags for cost allocation, it's a good idea to devise a set of tag keys that represent how you want to organize your costs\. Your cost allocation report displays the tag keys as additional columns with the applicable values for each row, so it's easier to track your costs if you use a consistent set of tag keys\. 

**Note**  
User\-defined cost allocation tags created by linked accounts can take up to 24 hours to appear in the Billing and Cost Management console\. To speed up the process, you can trigger a manual refresh\. For more information, see [Refreshing User\-Defined Cost Allocation Tags](refresh-cost-alloc-tags.md)

Some services launch other AWS resources that the service uses, such as Amazon EMR or AWS Marketplace launching an EC2 instance\. If the supporting service \(EC2\) supports tagging, you can tag the supporting resources \(such as the associated Amazon EC2 instance\) for your report\. For a full list of resources that can be tagged, use the Tag Editor to search\. For more information about how to search for resources using Tag Editor, see [ Searching for Resources to Tag](https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/searching-resources-to-tag.html)\. 
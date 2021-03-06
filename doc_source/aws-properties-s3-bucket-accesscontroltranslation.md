# Amazon S3 Bucket AccessControlTranslation<a name="aws-properties-s3-bucket-accesscontroltranslation"></a>

<a name="aws-properties-s3-bucket-accesscontroltranslation-description"></a>The `AccessControlTranslation` property type specifies replica ownership of the AWS account that owns the destination bucket\.

<a name="aws-properties-s3-bucket-accesscontroltranslation-inheritance"></a> `AccessControlTranslation` is a property of the [ReplicationDestination](aws-properties-s3-bucket-replicationconfiguration-rules-destination.md) property type\.

## Syntax<a name="aws-properties-s3-bucket-accesscontroltranslation-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-s3-bucket-accesscontroltranslation-syntax.json"></a>

```
{
  "[Owner](#cfn-s3-bucket-accesscontroltranslation-owner)" : String
}
```

### YAML<a name="aws-properties-s3-bucket-accesscontroltranslation-syntax.yaml"></a>

```
[Owner](#cfn-s3-bucket-accesscontroltranslation-owner): String
```

## Properties<a name="aws-properties-s3-bucket-accesscontroltranslation-properties"></a>

`Owner`  <a name="cfn-s3-bucket-accesscontroltranslation-owner"></a>
Specifies the replica ownership\. For default and valid values, see [PUT bucket replication](https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTreplication.html) in the *Amazon Simple Storage Service API Reference*\.  
 *Required*: Yes  
 *Type*: String  
 *Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt) 
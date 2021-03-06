# Elastic Load Balancing V2 AuthenticateCognitoConfig<a name="aws-properties-elasticloadbalancingv2-listener-authenticatecognitoconfig"></a>

<a name="aws-properties-elasticloadbalancingv2-listener-authenticatecognitoconfig-description"></a>The `AuthenticateCognitoConfig` property type specifies request parameters to use when integrating with Amazon Cognito to authenticate users\.

<a name="aws-properties-elasticloadbalancingv2-listener-authenticatecognitoconfig-inheritance"></a> `AuthenticateCognitoConfig` is a property of the [Elastic Load Balancing V2 Action](aws-properties-elasticloadbalancingv2-listener-defaultactions.md) property type\.

## Syntax<a name="aws-properties-elasticloadbalancingv2-listener-authenticatecognitoconfig-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-elasticloadbalancingv2-listener-authenticatecognitoconfig-syntax.json"></a>

```
{
  "[AuthenticationRequestExtraParams](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-authenticationrequestextraparams)" : { String:String, ... } ,
  "[OnUnauthenticatedRequest](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-onunauthenticatedrequest)" : String,
  "[Scope](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-scope)" : String,
  "[SessionCookieName](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-sessioncookiename)" : String ,
  "[SessionTimeout](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-sessiontimeout)" : Number,
  "[UserPoolArn](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpoolarn)" : String,
  "[UserPoolClientId](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpoolclientid)" : String ,
  "[UserPoolDomain](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpooldomain)" : String
}
```

### YAML<a name="aws-properties-elasticloadbalancingv2-listener-authenticatecognitoconfig-syntax.yaml"></a>

```
[AuthenticationRequestExtraParams](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-authenticationrequestextraparams): { String:String, ... }
[OnUnauthenticatedRequest](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-onunauthenticatedrequest): String
[Scope](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-scope): String
[SessionCookieName](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-sessioncookiename): String
[SessionTimeout](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-sessiontimeout): Number
[UserPoolArn](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpoolarn): String
[UserPoolClientId](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpoolclientid): String
[UserPoolDomain](#cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpooldomain): String
```

## Properties<a name="aws-properties-elasticloadbalancingv2-listener-authenticatecognitoconfig-properties"></a>

`AuthenticationRequestExtraParams`  <a name="cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-authenticationrequestextraparams"></a>
The query parameters \(up to 10\) to include in the redirect request to the authorization endpoint\.  
 *Required*: No  
 *Type*: *Type*: String to String map  
*Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt)

`OnUnauthenticatedRequest`  <a name="cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-onunauthenticatedrequest"></a>
The behavior if the user is not authenticated\. The following are possible values:  
+ `deny`: Return an HTTP 401 Unauthorized error\.
+ `allow`: Allow the request to be forwarded to the target\.
+ `authenticate`: Redirect the request to the IdP authorization endpoint\. This is the default value\.
 *Required*: No  
 *Type*: String  
*Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt)

`Scope`  <a name="cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-scope"></a>
The set of user claims to be requested from the IdP\. The default is `openid`\.   
To verify which scope values your IdP supports and how to separate multiple values, see the documentation for your IdP\.  
 *Required*: No  
 *Type*: String  
*Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt)

`SessionCookieName`  <a name="cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-sessioncookiename"></a>
The name of the cookie used to maintain session information\. The default is `AWSELBAuthSessionCookie`\.  
 *Required*: No  
 *Type*: String  
*Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt)

`SessionTimeout`  <a name="cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-sessiontimeout"></a>
The maximum duration of the authentication session, in seconds\. The default is 604800 seconds \(7 days\)\.  
 *Required*: Yes  
 *Type*: *Type*: Number  
*Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt)

`UserPoolArn`  <a name="cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpoolarn"></a>
The Amazon Resource Name \(ARN\) of the Amazon Cognito user pool\.  
 *Required*: Yes  
 *Type*: String  
*Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt)

`UserPoolClientId`  <a name="cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpoolclientid"></a>
The ID of the Amazon Cognito user pool client\.  
 *Required*: Yes  
 *Type*: String  
*Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt)

`UserPoolDomain`  <a name="cfn-elasticloadbalancingv2-listener-authenticatecognitoconfig-userpooldomain"></a>
The domain prefix or fully\-qualified domain name of the Amazon Cognito user pool\.  
 *Required*: Yes  
 *Type*: String  
*Update requires*: [No interruption](using-cfn-updating-stacks-update-behaviors.md#update-no-interrupt)

## See Also<a name="aws-properties-elasticloadbalancingv2-listener-authenticatecognitoconfig-seealso"></a>
+ [AuthenticateCognitoActionConfig](https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_AuthenticateCognitoActionConfig.html) in the *Elastic Load Balancing API Reference version 2015\-12\-01*
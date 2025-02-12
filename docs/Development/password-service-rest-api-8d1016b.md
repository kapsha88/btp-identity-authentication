<!-- loio8d1016b602704b9db38d55daa92c32e6 -->

# Password Service REST API

The password service is used for operations related to user passwords, such as verification of the user name and the password combination.



## Verify Username and Password Combination

Verify the username and password combination, or verify the thing ID and password combination.



## Request

**URI:**`https://<tenant ID>.accounts.ondemand.com/service/users/password`

> ### Note:  
> *Tenant ID* is an automatically generated ID by the system. The first administrator created for the tenant receives an activation e-mail with a URL in it. This URL contains the *tenant ID*. For more information about your tenants, see [Viewing Assigned Tenants and Administrators](../viewing-assigned-tenants-and-administrators-f56e6f2.md).

**HTTP Method:***POST*



### Request Headers


<table>
<tr>
<th valign="top">

Header



</th>
<th valign="top">

Required



</th>
<th valign="top">

Values



</th>
</tr>
<tr>
<td valign="top">

`Basic Authorization`



</td>
<td valign="top">

Yes



</td>
<td valign="top">

Username and password are provided by the user.

> ### Note:  
> Depending on the allowed logon identifiers for the user, the username can be the `User ID`, `Login Name`, or `E-Mai`. For more information, see [Configure Allowed Logon Identifiers](../Operation-Guide/configure-allowed-logon-identifiers-3adf1ff.md).

> ### Caution:  
> If the user provides wrong password, then each verification counts as a failed logon attempt. The password locks when the number of the allowed failed logon attempts is reached. The number depends on the password policy applied for the application. For more information, see [Configuring Password Policies](../Operation-Guide/configuring-password-policies-12b3395.md).



</td>
</tr>
<tr>
<td valign="top">

`Content-Type`



</td>
<td valign="top">

Yes



</td>
<td valign="top">

application/json



</td>
</tr>
</table>



### Request Example

```
POST /service/users/password
Basic Authentication: Username/Password
```



## Response



### Response Status and Error Codes


<table>
<tr>
<th valign="top">

Code



</th>
<th valign="top">

Result or X-Message Code



</th>
<th valign="top">

Description



</th>
</tr>
<tr>
<td valign="top">

200 OK



</td>
<td valign="top">

Success



</td>
<td valign="top">

When the username and password combination or thing ID and password combination is verified.



</td>
</tr>
<tr>
<td valign="top" rowspan="8">

401 Unauthorized



</td>
<td valign="top">

PASSWORD\_LOCKED



</td>
<td valign="top">

When the password is locked for 60 minutes.



</td>
</tr>
<tr>
<td valign="top">

PASSWORD\_DISABLED



</td>
<td valign="top">

When the password is disabled.



</td>
</tr>
<tr>
<td valign="top">

USER\_INACTIVE



</td>
<td valign="top">

When the user is not in status active.



</td>
</tr>
<tr>
<td valign="top">

PASSWORD\_RESET\_REQUIRED



</td>
<td valign="top">

When the user must reset his or her password before logon.



</td>
</tr>
<tr>
<td valign="top">

PASSWORD\_CHANGE\_REQUIRED



</td>
<td valign="top">

When the user must change his or her password before logon.



</td>
</tr>
<tr>
<td valign="top">

INITIAL\_PASSWORD\_EXPIRED



</td>
<td valign="top">

When the initial password of the user has expired. After the validity of the initial password expires, the user can't log on to the application and must contact the administrator.



</td>
</tr>
<tr>
<td valign="top">

INVALID\_AUTHORIZATION\_HEADER\_LENGTH



</td>
<td valign="top">

The time-based one-time password \(TOTP\) code is not provided, but Two-Factor Authentication \(TFA\) with TOTP is enabled.



</td>
</tr>
<tr>
<td valign="top">

INVALID\_OTP\_CODE



</td>
<td valign="top">

Wrong TOTP code was provided.



</td>
</tr>
</table>



### Response Example

On success, the HTTP Response Body contains:

```
 {
       "uid": "P000000",
       "first_name": "Dona",
       "last_name": "Moore",
       "mail": "dona.moore@example.com"
       "type": "employee"
    }
```

 

**Related Information**  


[General Error Codes](general-error-codes-182352d.md "The following table lists error codes that may be returned from any method on any resource URI.")

[Configure Risk-Based Authentication for an Application](../Operation-Guide/configure-risk-based-authentication-for-an-application-bc52fbf.md#loiobc52fbf3d59447bbb6aa22f80d8b6056 "You can define rules for authentication according to different risk factors and apply actions like Allow, Deny, and Two-Factor Authentication.")

[Configure User Access to the Application](../Operation-Guide/configure-user-access-to-the-application-8b147c4.md "You can configure public access to the application allowing self-registration, or you can restrict the access to existing users or users registered by an application.")


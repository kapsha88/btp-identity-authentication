<!-- copyc5b80bfbbb70478d983f6861943197d8 -->

# Create OpenID Connect Application for Client Credentials Flow

You can create a new OpenID Connect application.



## Context

To create a new OpenID Connect application you have to add a new application to the list of applications in Identity Authentication, and then set the protocol of application to OpenID Connect.

To create a new OpenID Connect application, choose your scenario and follow the procedure there.



<a name="copyc5b80bfbbb70478d983f6861943197d8__steps_qqh_hfk_q4"/>

## Procedure

1.  Sign in to the administration console for SAP Cloud Identity Services.

2.  Choose the *Applications* tile.

3.  Choose the *Create* button on the left-hand panel and fill in the information in the dialog box.

4.  Provide the following information and save your configuration:


    <table>
    <tr>
    <th valign="top">

    Fields


    
    </th>
    <th valign="top">

    Notes


    
    </th>
    </tr>
    <tr>
    <td valign="top">

    *Display Name*


    
    </td>
    <td valign="top">

    Required. The display name of the application appears on the logon and registration pages.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    *Home URL*


    
    </td>
    <td valign="top">

    Optional. Users are redirected to the *Home URL* after activating their accounts, when they are created via a CSV file import or the user registration service of Identity Authentication.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    *Type*


    
    </td>
    <td valign="top">

    Optional.


    
    </td>
    </tr>
    <tr>
    <td valign="top">

    *Parent Application*


    
    </td>
    <td valign="top">

    Optional.

    > ### Remember:  
    > Newly created applications with an assigned parent application will inherit all the configurations from the parent except for the `Client ID` and `Secrets`. The inherited configurations will be marked as such.


    
    </td>
    </tr>
    </table>
    
    Once the application has been created, the system displays the message ***Application <name of application\> created***.

    The newly created application appears on the list with the applications on the left. It is selected and you can set its protocol to OpenID Connect.

5.  Choose *Trust* \> *SINGLE SIGN-ON* \> *Protocol* 

    > ### Caution:  
    > Make sure that the application you want to configure as OpenID connect is selected on the left.

6.  Select the *OpenID Connect* radio-button.

7.  Save your selection.

    The system displays the message ***Application <name of application\> updated***.

    > ### Note:  
    > \(Optional\) If necessary, configure additional settings for the application. For more information about the supported configurations for the OpenID Connect applications, see the following links:
    > 
    > -   [Configure Secrets for API Authentication](configure-secrets-for-api-authentication-5c3c35e.md)
    > -   [Configure Certificates for API Authentication](configure-certificates-for-api-authentication-c408083.md)


**Related Information**  


[OpenID Connect](openid-connect-a789c9c.md "You can use Identity Authentication for authentication in OpenID Connect protected applications.")


<!-- copy411c3c6aa5f244579edbcc294dbe62d6 -->

# Create OpenID Connect Application for Authorization Code Flow

Create a new OpenID Connect application for authorization code flow.



## Context

To create a new OpenID Connect application follow the procedure below:



<a name="copy411c3c6aa5f244579edbcc294dbe62d6__steps_qqh_hfk_q4"/>

## Procedure

1.  Sign in to the administration console for SAP Cloud Identity Services.

2.  Under *Applications and Resources*, choose the *Applications* tile.

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

    The system displays the message ******.

    > ### Note:  
    > \(Optional\) If necessary, configure additional settings for the application. For more information about the supported configurations for the OpenID Connect applications, see the following links:Application <name of application\> updated
    > 
    > -   [Change an Application's Display Name](change-an-application-s-display-name-83d65d0.md)
    > -   [Configure an Application's Home URL](configure-an-application-s-home-url-be6d6f2.md)
    > -   [Visit an Application's Web Page](visit-an-application-s-web-page-2b67225.md)
    > -   [Configure the User Attributes Sent to the Application](configure-the-user-attributes-sent-to-the-application-d361407.md)
    > -   [Configure the Default Attributes Sent to the Application](configure-the-default-attributes-sent-to-the-application-a2f1e46.md)
    > -   [Configure Secrets for API Authentication](configure-secrets-for-api-authentication-5c3c35e.md)
    > -   [Configure Certificates for API Authentication](configure-certificates-for-api-authentication-c408083.md)
    > -   [Enable or Disable Kerberos Authentication for an Application](enable-or-disable-kerberos-authentication-for-an-application-11121c9.md)
    > -   [Configure Risk-Based Authentication for an Application](configure-risk-based-authentication-for-an-application-bc52fbf.md#loiobc52fbf3d59447bbb6aa22f80d8b6056)
    > -   [Configure User Access to the Application](configure-user-access-to-the-application-8b147c4.md)
    > -   [Authenticating Identity Provider for an Application](authenticating-identity-provider-for-an-application-b3aae12.md)
    > -   [Enable E-Mail Verification](enable-e-mail-verification-483d26c.md)
    > -   [Configuring Password Policies](configuring-password-policies-12b3395.md)
    > -   [Configuring Privacy Policies](configuring-privacy-policies-ed48466.md)
    > -   [Configuring Terms of Use](configuring-terms-of-use-61d3a86.md)
    > -   [Display Application Name on Logon Page](display-application-name-on-logon-page-c02798e.md)
    > -   [Configure a Logo for an Application](configure-a-logo-for-an-application-778f748.md)
    > -   [Configure a Branding Style for an Application](configure-a-branding-style-for-an-application-32f8d33.md)
    > -   [Configure Registration and Upgrade Forms](configure-registration-and-upgrade-forms-93a9e18.md)
    > -   [Protecting Self-Registration with Phone Verification](protecting-self-registration-with-phone-verification-5834b6e.md)
    > -   [Protecting Application Forms with Google reCAPTCHA](protecting-application-forms-with-google-recaptcha-b84ce17.md)
    > -   [Configure Identity Federation](configure-identity-federation-c029bbb.md)
    > -   [Configure SAML 2.0 Authentication Request to Corporate IdPs](configure-saml-2-0-authentication-request-to-corporate-idps-7eac7e8.md)


**Related Information**  


[OpenID Connect](openid-connect-a789c9c.md "You can use Identity Authentication for authentication in OpenID Connect protected applications.")


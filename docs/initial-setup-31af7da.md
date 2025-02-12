<!-- loio31af7da133874e199a7df1d42905241b -->

# Initial Setup

Getting started with Identity Authentication - tenants and administration console.

For more information about the tenant model, tenant licensing, and obtaining a new or additional tenant in Identity Authentication, see [Tenant Model and Licensing](tenant-model-and-licensing-93160eb.md).

You can access the tenant's administration console for SAP Cloud Identity Services by using the console's URL.

> ### Note:  
> The URL has the following pattern:
> 
> `https://<tenant ID>.accounts.ondemand.com/admin`
> 
> *Tenant ID* is an automatically generated ID by the system. The first administrator created for the tenant receives an activation e-mail with a URL in it. This URL contains the *tenant ID*. For more information about your tenants, see [Viewing Assigned Tenants and Administrators](viewing-assigned-tenants-and-administrators-f56e6f2.md).
> 
> If you have a configured custom domain, the URL has the `<your custom domain>/admin` pattern.

> ### Note:  
> When the Identity Authentication tenant is initially provisioned to your organization, only one user is added as a tenant administrator. After that, due to possible legal and security issues, SAP adds additional tenant administrators only in exceptional cases \(for example, the existing administrator left the company, or for some reason there is no active administrator for this tenant\). To avoid access related issues in such cases, it is always a good practice for you to assign more than one administrators. Adding additional ones is exclusively in the responsibility of the current tenant administrators. For more information, see [Add Administrators](Operation-Guide/add-administrators-bbbdbdd.md#loiobbbdbdd3899942ce874f3aae9ba9e21d).

> ### Note:  
> If you experience troubles in accessing your Identity Authentication tenant, you can report an incident on [SAP Support Portal Home](https://support.sap.com/en/index.html) with a component `BC-IAM-IDS`.

**Related Information**  


[What Is Identity Authentication?](what-is-identity-authentication-2788271.md "Authentication and single sign-on for users in the cloud.")

[Tenant Model and Licensing](tenant-model-and-licensing-93160eb.md "This document provides information about the tenant model, tenant licensing, and obtaining a tenant of Identity Authentication.")

[Product Details](product-details-4d404b1.md)

[Operation Guide](Operation-Guide/operation-guide-6a8e67c.md "This guide is for administrators. It explains how administrators can configure Identity Authentication so that users can have all enhanced features for each scenario.")


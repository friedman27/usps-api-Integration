# USPS-API-Integration
This integration was written to validate addresses using the [USPS Addresses 3.0 REST API](https://developer.usps.com/addressesv3).

To set up this integration:
* Create an account at https://developer.usps.com/apis
* Create an app on your USPS account. This will provide a client id and secret to use for OAuth. OAuth docs at https://developer.usps.com/oauth.
* Store this information in a named credential as an external credential in Salesforce, configuring the id and secret in a principal parameter.
* Permissions to this external credential must be provided to all users using this integration via a profile or permission set.

>This named credential is referenced in the USPSAddressRequest apex class via the 'NAMED_CREDENTIAL' variable.
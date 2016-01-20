{:shortdesc: .shortdesc}

# Protecting cloud resources with {{site.data.keyword.amashort}}
{: #protecting-resources}

With the {{site.data.keyword.amashort}} service, you can protect your Node.js and Java-based backend applications that are running on {{site.data.keyword.Bluemix_notm}} with mobile-enabled OAuth security and monitoring.
{:shortdesc}

## Authorization filter
{: #auth-filter}
The {{site.data.keyword.amashort}} Server SDK has authorization filters that you can use to protect your backend applications.  The authorization filter intercepts incoming requests and validates whether an authorization header is present. If the authorization header is not present or is invalid, the filter returns a response with HTTP 401. The {{site.data.keyword.amashort}} Client SDK knows how to intercept an HTTP 401 response that is returned by the {{site.data.keyword.amashort}} Server SDK and triggers the authentication flow.

## Authorization header



{
```
* `imf.user`: Specifies the user identity that is extracted from the ID token. If there no ID token exists, this field holds an empty object.
* `imf.device`: Specifies the device identity that is extracted from the ID token. If no ID token exists, this field holds an empty object.

## Next steps
{: #next-steps}
* [Protecting Node.js resources](protecting-resources-nodejs.html)
* [Protecting Java for Liberty resources](protecting-resources-java.html)
* [Local development](protecting-resources-local.html)
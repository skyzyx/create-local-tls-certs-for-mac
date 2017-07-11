# How to create local TLS certificates for development on macOS

Largely based on [“Generating Self-Signed SSL Certificates for Use with Bluemix Custom Domains”](https://www.tonyerwin.com/2014/09/generating-self-signed-ssl-certificates.html), by Tony Erwin.

The examples in this tutorial are from macOS Sierra (10.12).

## Create a local Certificate Authority

By creating a Certificate Authority (a.k.a., a “CA”) and trusting it locally, any certificate that we create using this CA will also be trusted locally. This can simplify the development of _HTTPS_ websites on your local machine.

Start by opening _Keychain Access_. You can either search for it inside Spotlight, or you can traverse the file system for _Computer_ → _Applications_ → _Utilities_ → _Keychain Access_.

### Create a Certificate Authority

![](images/new-ca-selection.png)


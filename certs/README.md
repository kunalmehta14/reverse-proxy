### Certificate instructions
> Use PEM and KEY files for certificates.
### Using Openssl to convert required files
> Exporting PEM file
````
openssl pkcs12 -in ".pfx" -nokeys -out "cert.pem"
````
> Exporting KEY file
````
pkcs12 -in ".pfx" -nocerts -nodes -out "private.key"
````
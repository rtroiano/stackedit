
# Coyote Point Load Balancer
Coyote point load balancers handle the network load for our servers. It also is where our SSLs live and controls https requests for our domains.

## Updating SSL Certificates

On the newer firmware 10.3.3a (which is currently at HQ) to update the SSL follow these steps:

1.  Under the System tab click Certificate    
2.  Click the + sign if adding a new cert
3.  Name it, I was using the format  _site.CA_ where site is the site you are using i.e. satav.CA
4.  Then using a program (we used xca in the past, details below) export the certificate file and key (if needed) and upload them by clicking Commit
5.  Verify by going to https://site from the HQ intranet

 

## Using XCA to export cert:
1.  Open the main.xdb file located on core02: Groups/IT Services/Documents/main.xdb 
2.  In the certs tab click on the cert that you need exported click export 
3.  The format is usually PEM with Certicate chain (I think with chain it has been some time since I did this)
4.  Change the file name since \ and * is bad to use in naming    
5.  Then OK
    

## Using XCA to export key:


1.  Open the main.xdb file located on core02: Groups/IT Services/Documents/main.xdb    
2.  In the Private Keys tab click on the key that you need exported click export    
3.  The format is usually PEM and Export the private part of the Key too checked    
4.  Change the file name since \ is bad to use in naming    
5.  Then OK

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTY4MTE1OTg5M119
-->
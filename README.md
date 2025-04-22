# reverse-proxy

In this repository, we have included scripts that are necessary to run a reverse proxy that will forward requests to Cryptolens Web API. The goal of this setup is to have a custom url and IP that is used to verify license keys. For example, if the IP needs to be from a certain geographical location or if you want to use your custom domain, a reverse proxy can accomplish that.

To get started, the following steps are recommended:
1. Obtain a Linux VM.
2. Install Nginx.
3. Change the `default.conf` in the `/etc/nginx/conf.d` to the one in this repository. The key is to include all the "location" blocks (and add more if necessary), as well as to set the domain name that you will be using.
4. If you link a subdomain to the VM, you can use Let's Encrypt to manage the SSL certificate.

If you would need any help or would like us to manage the reverse proxy on your behalf, please reach out to us at support@cryptolens.io.

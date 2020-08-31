### How to configure Fastly for PlatformSH

##### Step 1

Install and enable the default configuration for the Fastly module. This will add specific cache tags to the header to help Fastly recognizes pages it needs to cache.

##### Step 2 

Deploy that code to your Platform branch.
In Fastly Add your domain and origin server. The origin server is your PlatformSH backend origin endpoint which is the same as the cname used for a DNS switch.

##### Step 3

When using a custom domain a TLS-enabled domain is required so go ahead and set this up in Fastly. Once this has been set up you should have received a TLS-enabled domain and CNAME.

##### Step 4

Point your current DNS provider to the Fastly TLS-enabled domain.

##### Step 5

Test if you have a valid TLS cert.
Test if you get hits on the Varnish cache using the Stats tab in Fastly
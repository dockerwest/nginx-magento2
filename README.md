Nginx image for magento2
========================

Nginx container for magento2 applications. Magento is not installed in the Image.

Environment variables
---------------------

### DNS_RESOLVER

By setting `DNS_RESOLVER` you can make sure that nginx will run without the
fastcgi already available. Nginx will resolve the name of the application
container via DNS. When you set `DNS_RESOLVER` to 'auto' the value set in
`/etc/resolv.conf` inside the container will be used by nginx for resolving
(This will default to docker interal dns resolving). If you want to use an
external resolver you can also set a specific ipv4 address.

Versions
--------

The following versions are available:
- stable: last stable version of nginx
- mainline: last mainline version of nginx

License
-------

MIT License (MIT). See [License File](LICENSE.md) for more information.

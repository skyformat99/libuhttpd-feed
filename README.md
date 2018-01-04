# libuhttpd-openwrt

# How to use
Add new feed into "feeds.conf.default":

    src-git libuhttpd https://github.com/zhaojh329/libuhttpd.git

Install libuhttpd packages:

    ./scripts/feeds update libuhttpd
    ./scripts/feeds install libuhttpd

Select package libuhttpd in menuconfig and compile new image.

    Libraries  --->
        Networking  --->
            <*> libuhttpd-mbedtls.................................... libuhttpd (mbedtls)
            < > libuhttpd-nossl....................................... libuhttpd (NO SSL)
            < > libuhttpd-openssl.................................... libuhttpd (openssl)
            < > libuhttpd-wolfssl.................................... libuhttpd (wolfssl)

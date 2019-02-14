Riot For yunohost
=================

[![Integration level](https://dash.yunohost.org/integration/riot.svg)](https://ci-apps.yunohost.org/ci/apps/riot%20%28Community%29/lastBuild/consoleFull)  
[![Install riot with YunoHost](https://install-app.yunohost.org/install-with-yunohost.png)](https://install-app.yunohost.org/?app=riot)

> *This package allow you to install riot quickly and simply on a YunoHost server.  
If you don't have YunoHost, please see [here](https://yunohost.org/#/install) to know how to install and enjoy it.*

Overview
--------

It's a webclient for matrix. For a matrix server you can install synapse on your server : https://github.com/YunoHost-Apps/synapse_ynh

Yunohost chattroom with matrix : [https://riot.im/app/#/room/#yunohost:matrix.org](https://riot.im/app/#/room/#yunohost:matrix.org)

**Shipped version:** 1.0.0

Screenshots
-----------

![](https://about.riot.im/wp-content/themes/riot/img/slider-video.png)

![](https://about.riot.im/wp-content/themes/riot/img/main-mob1.png)
![](https://about.riot.im/wp-content/themes/riot/img/slider-phone.png)

Demo
----

* [Official demo](https://riot.im/app)

Documentation
-------------

 * Official documentation: https://about.riot.im/need-help/
 * YunoHost documentation: There no other documentations, feel free to contribute.

YunoHost specific features
--------------------------

### Multi-users support

Now this application support the sso. If you want to use the sso you need to define the path to the default homeserver as your homeserver witch is installed on your yunohost instance.

### Supported architectures

* x86-64b - [![Build Status](https://ci-apps.yunohost.org/ci/logs/riot%20(Community).svg)](https://ci-apps.yunohost.org/ci/apps/riot/)
* ARMv8-A - [![Build Status](https://ci-apps-arm.yunohost.org/ci/logs/riot%20(Community).svg)](https://ci-apps-arm.yunohost.org/jenkins/job/riot/)
* Jessie x86-64b - [![Build Status](https://ci-stretch.nohost.me/jenkins/job/riot%20(Community).svg)](https://ci-stretch.nohost.me/jenkins/job/riot/)

<!--## Limitations

* Any known limitations.-->

Additional informations
-----------------------

### Important Security Note

We do not recommend running Riot from the same domain name as your Matrix
homeserver (synapse).  The reason is the risk of XSS (cross-site-scripting)
vulnerabilities that could occur if someone caused Riot to load and render
malicious user generated content from a Matrix API which then had trusted
access to Riot (or other apps) due to sharing the same domain.

We have put some coarse mitigations into place to try to protect against this
situation, but it's still not good practice to do it in the first place.  See
https://github.com/vector-im/riot-web/issues/1977 for more details.

Links
-----

 * Report a bug: https://github.com/YunoHost-Apps/riot_ynh/issues
 * App website: https://riot.im/
 * YunoHost website: https://yunohost.org/

---

Install
-------

From command line:

`sudo yunohost app install -l riot https://github.com/YunoHost-Apps/riot_ynh`

Upgrade
-------

From command line:

`sudo yunohost app upgrade riot -u https://github.com/YunoHost-Apps/riot_ynh`

Developers infos
----------------

Please do your pull request to the [testing branch](https://github.com/YunoHost-Apps/riot_ynh/tree/testing).

To try the testing branch, please proceed like that.
```
sudo yunohost app install https://github.com/YunoHost-Apps/riot_ynh/tree/testing --debug
or
sudo yunohost app upgrade riot -u https://github.com/YunoHost-Apps/riot_ynh/tree/testing --debug
```

License
-------

Riot-Web is published under the Apache License : https://github.com/vector-im/riot-web/blob/master/LICENSE

Todo for official App
---------------------

- Improve documentation

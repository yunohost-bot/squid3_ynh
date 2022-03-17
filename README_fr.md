# squid3 pour YunoHost

[![Niveau d'intégration](https://dash.yunohost.org/integration/squid3.svg)](https://dash.yunohost.org/appci/app/squid3) ![](https://ci-apps.yunohost.org/ci/badges/squid3.status.svg) ![](https://ci-apps.yunohost.org/ci/badges/squid3.maintain.svg)  
[![Installer squid3 avec YunoHost](https://install-app.yunohost.org/install-with-yunohost.svg)](https://install-app.yunohost.org/?app=squid3)

*[Read this readme in english.](./README.md)*
*[Lire ce readme en français.](./README_fr.md)*

> *Ce package vous permet d'installer squid3 rapidement et simplement sur un serveur YunoHost.
Si vous n'avez pas YunoHost, regardez [ici](https://yunohost.org/#/install) pour savoir comment l'installer et en profiter.*

## Vue d'ensemble

## Squid: Proxy with Optimising Web Delivery

Squid is a caching proxy for the Web supporting HTTP, HTTPS, FTP, and more. It reduces bandwidth and improves response times by caching and reusing frequently-requested web pages. Squid has extensive access controls and makes a great server accelerator.


**Version incluse :** 1.0~ynh3



## Avertissements / informations importantes

## Instruction

1. The app can not be **multi-instance**(can't be installed many times on same server).
2. **LDAP** is there(Registered users can use there login username and password to browser internet through the proxy)
3. **Port number** used by the proxy will be sent to the **admin mail** of the Yunohost server.
4. The username and password is **asked twice** first time you start the browser(I have no idea why this happens).

## Configure Squid3 for Firefox

1. Go to **Preferences -> General -> network proxy**
1. Select **Manual proxy configuration**
1. In **HTTP Proxy** enter your **domain name or server IP** and in **Port** enter the port sent to your **admin email**.
1. Check **Use this proxy server for all protocols**.
1. Under **No Proxy for** enter this **localhost, 127.0.0.1**.
1. **Save and restart** the Firefox.

If you try Squid 3 in any other way please write the instruction in the issue so that I can add it to the readme

## Special Thanks
Thanks to **Fred** to write the instruction to configure Squid for YunoHost. French: https://memo-linux.com/installer-squid3-sur-un-serveur-yunohost/

## Documentations et ressources

* Site officiel de l'app : http://www.squid-cache.org
* Documentation YunoHost pour cette app : https://yunohost.org/app_squid3
* Signaler un bug : https://github.com/YunoHost-Apps/squid3_ynh/issues

## Informations pour les développeurs

Merci de faire vos pull request sur la [branche testing](https://github.com/YunoHost-Apps/squid3_ynh/tree/testing).

Pour essayer la branche testing, procédez comme suit.
```
sudo yunohost app install https://github.com/YunoHost-Apps/squid3_ynh/tree/testing --debug
ou
sudo yunohost app upgrade squid3 -u https://github.com/YunoHost-Apps/squid3_ynh/tree/testing --debug
```

**Plus d'infos sur le packaging d'applications :** https://yunohost.org/packaging_apps
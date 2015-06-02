title: Upgrading from Grails 2.x to Grails 3
date: 2015-06-01 11:14:08
tags:
- grails
- groovy
- upgrade
---

## Upgrading Grails from Grails 2.x to Grails 3

Grails 3 brings some significant upgrade of the underlying components of Grails. 
As a result there are a number of areas of change

* Project structure differences
* File location differences
* Configuration differences
* Package name differences
* Legacy Gant Scripts
* Gradle Build System
* Changes to Plugins
* Source vs Binary Plugins

As a result one of the most transparent ways to upgrade as we will show below is to:
* Create a new Grails 3.0 application
* Copy (strtegically) the source files into the correct locations in the new application.

## Upgrading Steps
* installing grails 3 with gvm


### Installing Grails 3 with Gvm
The groovy version management  tools gvm is an excellent way to manage multiple versions of groovy and grails

To install the new version of grails:

```
gvm install grails 3.0.1

Downloading: grails 3.0.1

  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
  0     0    0     0    0     0      0      0 --:--:-- --:--:-- --:--:--     0
100   392    0   392    0     0    604      0 --:--:-- --:--:-- --:--:--  1209
100  157M  100  157M    0     0  9399k      0  0:00:17  0:00:17 --:--:-- 17.4M

Installing: grails 3.0.1
Done installing!

Do you want grails 3.0.1 to be set as default? (Y/n): n

```

You can switch between various versions of grails using something like:

```
gvm current grails 3.0.1
```

---
title: Quick-Start
metadata:
    description: These are the options to get CSYCMS - (We see only one option for now. If you'd like to go any other way of installing, then you'll have to go it alone).
    keywords: csycms, file-based content management system, knowledge base, static site generator, nodejs
    author: Brian Onang'o
---


# QuickStart

These are the options to get CSYCMS: (We see only one option for now. If you'd like to go any other way of installing, then you'll have to go it alone).

### Just Testing 

If you'd like to just test csycms, then there is no need to install the whole system. Just follow these steps. (Please jump to the next section to see how to install csycms as a service for production environments)

```
git clone git@github.com:csymapp/csycms.git
```

or you are new to github or to ssh, then you may have a hard time with the previous command. In that case you can use:

```
git clone https://github.com/csymapp/csycms.git
```

Then copy the configuration files

```
cd csycms
cp .env.example .env
```

then run your site using the command

```
SITE={yoursitename} PORT={porttorunsitein} node bin/app.js
```

### From GitHub

We have created an [installation script](https://github.com/csymapp/csycms/blob/master/Install/installCsycms.sh) which you can use to install CSYCMS. 

```
cd /tmp
wget https://raw.githubusercontent.com/csymapp/csycms/master/Install/installCsycms.sh
chmod +x installCsycms.sh
./installCsycms.sh
```

Then follow the installation instructions as directed by the script.

You will have to edit [some configurations](/csycms/Configuration)
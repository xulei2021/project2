.. highlight:: console

Appendix A: Netronome Repositories
==================================

All the software mentioned in this document can be obtained via the official
Netronome repositories. Please find instructions below on how to enable access
to the aforementioned repositories from your respective linux distributions.

Importing GPG-key
-----------------

Download and Import GPG-key to your local machine:

For RHEL/Centos 7.5, download the public key::

    # wget https://rpm.netronome.com/gpg/NetronomePublic.key

Import the public key::

    # rpm --import NetronomePublic.key

For Ubuntu 18.04 LTS, download the public key::

    # wget https://deb.netronome.com/gpg/NetronomePublic.key

Import the public key::

    # apt-key add NetronomePublic.key

Configuring repositories
------------------------

For RHEL/Centos 7.5, add Netronome's repository::

    # cat << 'EOF' > /etc/yum.repos.d/netronome.repo
    [netronome]
    name=netronome
    baseurl=https://rpm.netronome.com/repos/centos/
    gpgcheck=0
    enabled=1
    EOF
    yum makecache

For Ubuntu 18.04 LTS, add Netronome's repository::

    # mkdir -p /etc/apt/sources.list.d/
    # echo "deb https://deb.netronome.com/apt stable main" > \
        /etc/apt/sources.list.d/netronome.list

Update repository lists::

    # apt-get update


列表样式

* 无序列表 **（内容前加星号和一个空格）**
  
 * 1 
 * 2
 * 3

* 有序列表 **（内容前加井号、一个点和一个空格）**

 #. 111
 #. 222
 #. 333
  
For details, see https://zh-sphinx-doc.readthedocs.io/en/latest/tutorial.html#id3

Title
============

请参看以下示例:: 

 xxxxxxxxxxxx
 





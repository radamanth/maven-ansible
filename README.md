radamanth.maven-ansible 
=========

A small role to install Maven and Oracle Java on an unbuntu server (may be working for debian in general) 

Requirements
------------

Ubuntu platform

Role Variables
--------------

```yaml
# Maven version to install
mvn_version: "3.3.3"
# Where to find the package
mvn_url: "http://wwwftp.ciril.fr/pub/apache/maven/maven-3/{{mvn_version}}/binaries/apache-maven-{{mvn_version}}-bin.tar.gz"
# Maven directory owner username
mvn_owner: "mvnuser"
# Maven directory owner group
mvn_group: "mvn"
# Maven installation directory
mvn_destdir: "/usr/local/apache-maven"
# Mavend installation directory filemode
mvn_file_mode: "0775"
```

Dependencies
------------

This role require the radamanth.java-oracle-ansible role

see: https://github.com/radamanth/java-oracle-ansbile
see: meta/main.yml for  dependency version


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: maven_servers
      roles:
         - { role: radamanth.maven-ansible, version: 1.0.0 }

License
-------

GPLV2

Author Information
------------------


I've been a computer science engineer for more than 10 years now, I've discovered Ansible in 2014, and fell in love with it. I use it in my company to manage different server since then. Feel free to visit our site www.neovia.fr

I'm also one of the founder of Immozeo, where Ansible is also greatly used. ( www.immozeo.com)


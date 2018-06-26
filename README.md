BlockSci Ansible role
=====================

This ansible role installs and sets up BlockSci.

It is based on the original installation instructions in the Blocksci documentation (linked at the end of this README)

Requirements
------------

* Requires Python 3 and Ubuntu 16.04

* CMake 
The Blocksci install also requires cmake version 3.7 or above. Since Apt currently does not have an updated cmake this role also contains tasks to install cmake 3.11.0 in usr/local/bin. However, those tasks will not run if there is already a copy of cmake in usr/local/bin, this is to prevent any dependency problems in the users stack. 

Example Playbook
----------------

    - hosts: example_server
      roles:
         - blocksci

Original Compile Code
--------------------

https://citp.github.io/BlockSci/compiling.html#ubuntu-16-04

Author Information
------------------

Unchained Capital
* Abdullah Yusuf (www.github.com/Ayusuf95) 
* Nelson Todd (www.github.com/nelsontodd)

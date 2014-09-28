# This is InfiniDB 4.6.2

## Build prerequisites
To build InfiniDB from source you will need:

  * a CentOS/RHEL 5/6, debian 6/7 or Ubuntu 12/14 linux host configured for software development

Along with a working C++ compiler and GNU software development tools you will need the following extra packages:

  * expect
  * zlib-devel
  * ncurses-devel
  * libxml2-devel
  * readline-devel

## Build steps

### Build environment

    mkdir infinidb-src
    cd infinidb-src

### InfiniDB MySQL

    git clone https://github.com/allfs/mysql-1 mysql
    cd mysql
    ./configure --prefix=$HOME/infinidb/mysql
    make
    make install
    
### InfiniDB

    cd ..
    git clone https://github.com/allfs/infinidb
    cd infinidb
    ./configure --prefix=$HOME/infinidb
    make
    make install
	
### Setup production environment

   ln -s $HOME/infinidb /usr/local/Calpont	
    
This will leave you with `$HOME/infinidb` as a binary tree. Follow the Binary Download
instructions in the InfiniDB 4.6 Installation Guide (available on http://www.infinidb.co/).

## How to Contribute
  * You may submit your contributions via GitHub pull requests.
  * The submission must be by the original author.
  * Along with any pull requests, please state that the contribution is your original work
and that you license the work to the project under the project's open source license
and the InfiniDB Contributor Agreement
(see InfiniDBContributorAgreement.pdf). Whether or not you state this explicitly,
by submitting any copyrighted material via pull request, email, or other means you agree to
license the material under the project's open source license and warrant that you have the
legal authority to do so.
  * The InfiniDB Project committee will review your pull request and shall decide when and
whether to merge your request in the main InfiniDB project. The InfiniDB Project
committee will inform you of any decision regarding your request.


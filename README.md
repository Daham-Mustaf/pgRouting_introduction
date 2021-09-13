# pgRouting_introduction
# Table of contents
1. [pgRouting Introduction](#introduction)
- [Installation](#install)
- [pgRouting Installing in the database](#ex)
- [`ogrinfo`: ](#datasource)
- [`--help` getting help: ](#help)
- [`--long-usage` full help:](#fullhelp)


## pgRouting Introduction <a name="introduction"></a>
pgRouting is a PostGIS extension that brings routing tools to the table. pgRouting offers an extensive set of algorithms to choose from, can solve traveling salesman problems, calculate drive time zones, and even obey turn restrictions and avoid one-way streets.
With such a toolbox, one can create some pretty serious routing services that can be consumed, for example, by web applications.
## Installing the pgRouting extension<a name="install"></a>
pgRouting can be installed via ports:
```bash
cd /usr/ports/databases/pgRouting
```
```bash
make install clean
```
or package:
```bash
pkg install pgrouting
```
Homebrew
```bash
brew install pgrouting
```
git

To download the repository
```bash
git clone git://github.com/pgRouting/pgrouting.git
cd pgrouting
git checkout v3.1.3
```

## Installing the pgRouting extension<a name="ex"></a>
Many distributions of PostGIS are equipped with pgRouting already. Execute the following SQL to check whether you have pgRouting onboard:
```j
   select pgr_version();
   ```   
Once you have the binaries set up, enable the extension by executing the following:
createdb routing
```j
psql routing -c 'CREATE EXTENSION PostGIS'
psql routing -c 'CREATE EXTENSION pgRouting'
  ```
  or
```j
    CREATE EXTENSION pgrouting;
   ```
   At this stage, we should be ready to continue with pgRouting.
  


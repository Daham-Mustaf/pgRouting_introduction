# pgRouting_introduction
# Table of contents
1. [pgRouting Introduction](#introduction)
- [Installation](#install)
- [pgRouting extension](#ex)
- [`ogrinfo`: ](#datasource)
- [`--help` getting help: ](#help)
- [`--long-usage` full help:](#fullhelp)


## pgRouting Introduction <a name="introduction"></a>
pgRouting is a PostGIS extension that brings routing tools to the table. pgRouting offers an extensive set of algorithms to choose from, can solve traveling salesman problems, calculate drive time zones, and even obey turn restrictions and avoid one-way streets.
With such a toolbox, one can create some pretty serious routing services that can be consumed, for example, by web applications.
## Installing the pgRouting extension<a name="install"></a>


## Installing the pgRouting extension<a name="ex"></a>
Many distributions of PostGIS are equipped with pgRouting already. Execute the following SQL to check whether you have pgRouting onboard:
```j
   select pgr_version();
   ```   
Once you have the binaries set up, enable the extension by executing the following:
```j
    CREATE EXTENSION pgrouting;
   ```
   At this stage, we should be ready to continue with pgRouting.
  


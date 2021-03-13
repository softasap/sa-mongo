sa-mongo
========

[![Build Status](https://github.com/softasap/sa-mongo/workflows/CI/badge.svg?event=push)](https://github.com/softasap/sa-mongo/actions?query=workflow%3ACI)
[![Build Status](https://travis-ci.org/softasap/sa-mongo.svg?branch=master)](https://travis-ci.org/softasap/sa-mongo)


Role to install MongoDB 3.2, 3.4. 3.6, 4.0 or 4.2 on ubuntu based box.


| Distribution |   MongoDB 2.6 | MongoDB 3.2 | MongoDB 3.4 | MongoDB 3.6 | MongoDB 4.0 | | MongoDB 4.2 |
| ------------ |:-------------:|:-----------:|:-----------:|:-----------:|:-----------:|:-----------:|
| Ubuntu 14.04 | :white_check_mark: | :white_check_mark:| :white_check_mark:| :no_entry:| :no_entry:| :no_entry:|
| Ubuntu 16.04 | :no_entry: | :white_check_mark:| :white_check_mark:| :white_check_mark:| :white_check_mark:| :white_check_mark:|
| Ubuntu 18.04 | :no_entry: | :white_check_mark:| :white_check_mark:| :white_check_mark:| :white_check_mark:| :white_check_mark:|

- :white_check_mark: - should work fine
- :interrobang: - there were no production deploys for a while
- :no_entry: - not recommended for installation

Check for mongodb EOL for versions.  Generally, you should target latest or previous release.
Historic releases are provided for compability with old deployments that were using that role.

Version is controlled by  mongo_version parameter.

```
mongo_version: "4.2"  #  "2.6" | "3" | "3.2" | "3.4" | "3.6" | "4.0" | "4.2"
mongo_family: "org" # "org" | "enterprise"
```


Example:

Simple

```YAML


     - {
         role: "sa_mongo",
         mongo_version: "4.2"
       }

```

Advanced:

```YAML


     - {
         role: "sa_mongo",
         mongo_version: "4.2",
         mongo_family: "enterprise"
       }

```




Usage with ansible galaxy workflow
----------------------------------

If you installed the sa_mongo role using the command


`
   ansible-galaxy install softasap.sa_mongo
`

the role will be available in the folder library\softasap.mongo.
Please adjust the path accordingly.

```YAML

     - {
         role: "softasap.sa_mongo"
       }

```


Copyright and license
---------------------

Code is dual licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) and the [MIT License] (http://opensource.org/licenses/MIT). Choose the one that suits you best.

Reach us:

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)

Join gitter discussion channel at [Gitter](https://gitter.im/softasap)

Discover other roles at  http://www.softasap.com/roles/registry_generated.html

visit our blog at http://www.softasap.com/blog/archive.html

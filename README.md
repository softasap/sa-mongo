sa-mongo
========

[![Build Status](https://travis-ci.org/softasap/sa-mongo.svg?branch=master)](https://travis-ci.org/softasap/sa-mongo)


Role to install MongoDB 2.4 2.6 or 3.* on ubuntu based box.

Version is controlled by  mongo_version parameter.

mongo_version: "3.2"  #  "2.6" | "3" | "3.2"


Example:

```YAML


     - {
         role: "sa-mongo",
         mongo_version: "3.2"
       }

```


Usage with ansible galaxy workflow
----------------------------------

If you installed the sa-mongo role using the command


`
   ansible galaxy install softasap.sa-mongo
`

the role will be available in the folder library\softasap.mongo.
Please adjust the path accordingly.

```YAML

     - {
         role: "softasap.mongo"
       }

```


Copyright and license
---------------------

Code licensed under the [BSD 3 clause] (https://opensource.org/licenses/BSD-3-Clause) or the [MIT License] (http://opensource.org/licenses/MIT).

Subscribe for roles updates at [FB] (https://www.facebook.com/SoftAsap/)



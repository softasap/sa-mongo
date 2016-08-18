sa-mongo
========

[![Build Status](https://travis-ci.org/softasap/sa-mongo.svg?branch=master)](https://travis-ci.org/softasap/sa-mongo)


Role to install MongoDB 2.4 2.6 or 3.* on ubuntu based box.

Version is controlled by  mongo_version parameter.

mongo_version: "3.2"  #  "2.6" | "3" | "3.2"


Example:

<pre>


     - {
         role: "sa-mongo",
         mongo_version: "3.2"
       }

</pre>

README
======

[![Build Status](https://travis-ci.org/checkdomain/Comodo.svg)](https://travis-ci.org/checkdomain/Comodo)
[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/checkdomain/Comodo/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/checkdomain/Comodo/?branch=master)
[![Coverage Status](https://coveralls.io/repos/checkdomain/Comodo/badge.svg?branch=master&service=github)](https://coveralls.io/github/checkdomain/Comodo?branch=master)
[![SensioLabsInsight](https://insight.sensiolabs.com/projects/3119495f-5473-4396-9c36-0151add717e9/mini.png)](https://insight.sensiolabs.com/projects/3119495f-5473-4396-9c36-0151add717e9)


What is Checkdomain/Comodo
--------------------------
Checkdomain/Comodo is a library to connect with the comodo SSL Api. It yet offers functions to apply, revoke certificates and to resend the DCV mail.

The API also offers a function to enter the DCV authorization code, which has been sent to customer by mail.

Requirements
------------
Checkdomain/comodo requires
php >= 5.5

Installation
------------
The easiest way to install this library is through [composer](http://getcomposer.org/). Just add the following lines to your **composer.json** file:

```json
{
   "require": {
        "checkdomain/comodo": "dev-master"
    }
}
```
Another way would be to download this library and configure the autoloading yourself. This library relies on a [PSR-0](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-0.md) compatible autoloader for automatic class loading.

Usage
-----
To send a request to comodo, just instantiate the Util class and call any of the available functions.

The API always throws and Exception , if a parameter is missing or wrong formatted, or anything else did not work.

If a request has been successfully, you will get the return value true, or in case of using the AutoApply or
GetDCVEmailAddressList function, you receive a result-object with additional information.

Contributing
------------
Checkdomain/comodo is open source. There are a lot of functions left in the API to be integrated:

https://secure.comodo.net/api/pdf/webhostreseller/sslcertificates/

Pull requests will be reviewed and merged fast.

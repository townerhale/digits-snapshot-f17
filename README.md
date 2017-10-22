# digits-snapshot-f17

Here is a snapshot of the Digits code after completion of Part 6.  

The master branch uses the original version of simple schema at [https://github.com/aldeed/meteor-simple-schema](https://github.com/aldeed/meteor-simple-schema).


## Installation

First, [install Meteor](https://www.meteor.com/install).

Second, clone or download this github repo. 

Third, cd into the app directory install the required libraries with:

```
$ meteor npm install
```

Once the libraries are installed, you can run the application by invoking the "start" script in the package.json file:

```
$ meteor npm run start
```


**Note regarding bcrypt warning.** You will get the following message when you run this application:

```
Note: you are using a pure-JavaScript implementation of bcrypt.
While this implementation will work correctly, it is known to be
approximately three times slower than the native implementation.
In order to use the native implementation instead, run

  meteor npm install --save bcrypt

in the root directory of your application.
```

On some operating systems (particularly Windows), installing bcrypt is much more difficult than implied by the above message. Bcrypt is only used in Meteor for password checking, so the performance implications are negligible until your site has very high traffic. You can safely ignore this warning without any problems.

If all goes well, the template application will appear at [http://localhost:3000](http://localhost:3000). 

Lastly, you can run ESLint over the code in the imports/ directory with:

```
meteor npm run lint
```
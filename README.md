1. Settting  up  FASTLANE CI is _not_ what the  official doc says
 - first, get ready to set up `rvm`  to use exactly ruby 2.3.3 at the moment of creating this doc (you can check current required ruby version by checking  .ruby-version file in the root of fastlane ci doc)
 - second,  make sure ur ruby version is compiled with open ssl option (google 'rvm macos ruby openssl')
 - third, *to run CI you first run the web server in the /web directory, and to  do that you need to  install it's dependencies:*
  - brew  install node
  - node install #the rest  of the dependencies
  - after node is installed, you have  to run web server first, then fastlance ci, second
  - doc can be found here: https://github.com/fastlane/ci/blob/master/web

2. For now, fastlane CI requires  you to have private github repo!!!
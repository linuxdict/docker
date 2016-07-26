This is fpm with CentOS 7:latest

More about fpm: https://rubygems.org/gems/fpm

https://github.com/jordansissel/fpm/wiki

Example: 

1. mkdir "pwd"/rpmsrc

2. put files you want to pack into rpm to "pwd"/rpmsrc/mytest

3. docker run  --name fpmbuild --rm -v "pwd"/rpmsrc:/build liuedy/centos-fpm fpm --verbose -f -s dir -t rpm --name myrpmname --description "Why I am doing this" -v 1.0.0 mytest

4. fetch your build from "pwd"/rpmsrc

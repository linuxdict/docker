This is fpm with CentOS 7:latest

More about fpm: https://rubygems.org/gems/fpm
https://github.com/jordansissel/fpm/wiki

Example: 
1. mkdir `pwd`/build

2. put files you want to pack into rpm to `pwd`/build/mytest

3. docker run  --name fpmbuild --rm -v `pwd`/rpmbuild:/build liuedy/fpm:latest fpm --verbose -f -s dir -t rpm --name additional_fonts --description "Why I am doing this" -v 1.0.0 mytest

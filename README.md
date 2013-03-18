# 왜?
chef에서 노드를 추가하는데 knife bootstrap 명령을 사용한다. 하지만 chef-server에서는 12.04 apt 버전의 bootstrap을 제공하지 않고 있어서 만들었다.

# 사용법
 ```
 $ git clone git://github.com/whitekid/chef-bootstrap.git
 $ sudo ln -s chef-bootstrap/ubuntu12.04-apt.erb /usr/lib/ruby/vendor_ruby/chef/knife/bootstrap/ubuntu10.04-apt.erb
 $ knife bootstrap <ip-address> -d ubuntu-12.04-apt --bootstrap-version 0.10
 ```

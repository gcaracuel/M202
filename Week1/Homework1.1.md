M202 Homework 1.1
========================

### Prerequisites (Ubuntu)

```
	sudo apt-get install sysstat libgl1-mesa-dev
```

- Download the 32-bit or 64-bit deb package.
```
	curl -OL https://mms.mongodb.com/download/agent/monitoring/mongodb-mms-monitoring-agent_2.1.2.43-1_i386.deb
```
or
```
	curl -OL https://downloads.mongodb.com/on-prem-mms/deb/mongodb-mms_1.4.1.62-1_x86_64.deb
```

- Install the package

```
	sudo dpkg -i mongodb-mms-monitoring-agent_2.1.2.43-1_i386.deb
```
or 
```
	sudo dpkg -i mongodb-mms_1.4.1.62-1_x86_64.deb
```

- Edit /etc/mongodb-mms/monitoring-agent.config and enter your API key:
	mmsApiKey=\<Here your MMS KEy\>

- Start the agent
```
	sudo start mongodb-mms-monitoring-agent
```

- Start mongo, start a replica or use  to build a test shard environment

- Install MongoProc 
```
	wget https://s3.amazonaws.com/edu-downloads.10gen.com/1.0/mongoProc_linux_i686.tar.gz

	tar -zxvf mongoProc_linux_i686.tar.gz

	./mongoProc --console
```

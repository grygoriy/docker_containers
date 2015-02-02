FROM grygoriy/java7
MAINTAINER Grygoriy Mykhalyuno <email@grygoriy.com>

RUN apt-get update && apt-get install -y wget && apt-get clean && \
	wget http://ftp.piotrkosoft.net/pub/mirrors/ftp.apache.org/zookeeper/zookeeper-3.3.6/zookeeper-3.3.6.tar.gz && \
	tar xzf zookeeper-3.3.6.tar.gz && \
	rm zookeeper-3.3.6.tar.gz
RUN	cp zookeeper-3.3.6/conf/zoo_sample.cfg zookeeper-3.3.6/conf/zoo.cfg
RUN mkdir /tmp/zookeeper/
	

EXPOSE 2181

# Define default command.
CMD ["zookeeper-3.3.6/bin/zkServer.sh", "start-foreground"]
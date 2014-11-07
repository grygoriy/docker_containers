FROM grygoriy/java7

RUN \
  apt-get update && \
  apt-get install -y maven && \
  apt-get clean

RUN mkdir ~/.m2

# Define default command.
CMD ["bash"]
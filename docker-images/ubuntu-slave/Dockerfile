FROM ubuntu
RUN apt update && apt install -y default-jdk docker.io ssh git curl python3-pip
RUN mkdir /var/run/sshd && chmod 0755 /var/run/sshd
RUN useradd jenkins -p saPEBZUoWBIjs -m -G docker -d /home/jenkins \
    && ssh-keygen -A
CMD /usr/sbin/sshd -D

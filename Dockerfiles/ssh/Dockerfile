FROM i386/ubuntu
RUN apt-get update
RUN apt-get install openssh-server -y
RUN ssh-keygen -t rsa -f /root/.ssh/id_rsa -q -P ""
RUN chmod 700 /root/.ssh
RUN mv /root/.ssh/id_rsa.pub /root/.ssh/authorized_keys
RUN mv /root/.ssh/id_rsa /root/.ssh/id.pem
RUN chmod 600 /root/.ssh/authorized_keys
RUN echo 'PublicAuthentication yes' >> /etc/ssh/sshd_config
EXPOSE 22
CMD service ssh start && bash 

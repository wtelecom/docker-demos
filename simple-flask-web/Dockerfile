FROM centos:7
# Update repos and install enterprise linux repository
RUN yum -y update && yum -y install epel-release
# Install pip
RUN yum -y install python-pip
# Install commander dependencies
ADD ./requirements.txt /usr/src/app/
RUN pip install -r /usr/src/app/requirements.txt
# Execute
CMD python /usr/app/server.py

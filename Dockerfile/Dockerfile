FROM ubuntu:17.04
MAINTAINER rodrigolucianocosta@hotmail.com

#Install any needed packages specified in requirements.txt

RUN apt-get update
RUN apt-get install -y nginx
RUN apt-get clean
RUN apt-get -y install python-pip

##install pip and update tools
RUN pip install --upgrade pip && \
    pip install pip-tools

# Install any needed packages specified in requirements.txt
#RUN pip install -r requirements.txt

#Make the port 80 avaliable to the world outside container
EXPOSE 80

#Define default command
CMD ["bash"]

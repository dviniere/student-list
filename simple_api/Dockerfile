FROM python:2.7-stretch
MAINTAINER Formation ATOS <atos@formation.fr>
ADD student_age.py /
RUN apt-get update -y && apt-get install python-dev python3-dev libsasl2-dev python-dev libldap2-dev libssl-dev -y 
RUN pip install flask==1.1.2 flask_httpauth==4.1.0 flask_simpleldap python-dotenv==0.14.0
VOLUME /data
EXPOSE 5000
CMD [ "python", "./student_age.py" ]

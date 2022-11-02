FROM rundeck/rundeck:4.7.0
LABEL maintainer "Serdal Ozkan <donserdal@hotmail.com>"

RUN sudo apt update
RUN sudo apt install python3-pip python-is-python3 ansible -y
RUN sudo sh -c 'yes | pip install requests urllib3 pywinrm'

VOLUME ["/home/rundeck/server/data"]


EXPOSE 4440
ENTRYPOINT [ "/tini", "--", "docker-lib/entry.sh" ]
# Updated 2022-6-25

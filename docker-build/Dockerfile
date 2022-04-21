FROM rundeck/rundeck:4.1.0
LABEL maintainer "Serdal Ozkan <donserdal@hotmail.com>"

RUN sudo apt install python3-pip python-is-python3 
RUN sudo pip install requests urllib3 pywinrm

VOLUME ["/home/rundeck/server/data"]


EXPOSE 4440
ENTRYPOINT [ "/tini", "--", "docker-lib/entry.sh" ]
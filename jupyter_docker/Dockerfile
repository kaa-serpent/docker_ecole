FROM python:3

RUN apt-get update && apt-get install -y python3-pip

WORKDIR /Documents
COPY . .
RUN pip3 install -r requirement.txt
RUN pip3 install jupyter

RUN apt install vim -y
RUN pip3 install --user virtualenv

ENTRYPOINT ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--allow-root"]

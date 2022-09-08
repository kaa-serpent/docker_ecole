FROM python:3.8-alpine

WORKDIR /python-docker

COPY requirement.txt requirement.txt
RUN pip3 install -r requirement.txt

COPY . .
# lancer avec python
#CMD python3 app.py  # ne fonctionne pas
#CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]
ENTRYPOINT [ "python" ]

CMD ["app.py"]
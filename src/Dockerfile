FROM python:3.10.2

WORKDIR /usr/src/app

COPY softdes.py ./
COPY adduser.py ./
COPY desafio.py ./
COPY quiz.db ./
COPY users.csv ./

RUN pip install flask flask_httpauth datetime

RUN python adduser.py

ENTRYPOINT ["python"]

CMD ["softdes.py"]
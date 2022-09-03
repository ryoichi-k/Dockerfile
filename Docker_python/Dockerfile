FROM python:alpine

WORKDIR /myapp

COPY ./requirements.txt requirements.txt

# requirements.txt記載のライブラリを全てインストール
RUN pip install -r requirements.txt

RUN pip install --upgrade pip

RUN python -m pip install jupyterlab

# port 8001
CMD ["python","-m","http.server","8001","--cgi"]
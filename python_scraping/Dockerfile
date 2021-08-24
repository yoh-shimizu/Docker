FROM python:3.7
WORKDIR /app
# 作業ディレクトリ作成
RUN mkdir /app/source
RUN mkdir /app/data
# apt-getのアップデートなど
RUN apt-get -y update
RUN apt-get -y upgrade
RUN apt-get install -y apt-utils git

RUN pip install \
    selenium \
    beautifulsoup4 \
    requests
FROM ubuntu:16.04
WORKDIR /root

RUN apt update
RUN apt upgrade -y
RUN apt install -y ruby-build autoconf subversion bison
RUN apt install -y mecab mecab-ipadic-utf8 wget
RUN apt build-dep -y ruby2.3 ruby-sqlite3 ruby-mecab

ENV PATH /root/.rbenv/shims:$PATH
RUN rbenv install 1.8.7-p375
RUN rbenv local 1.8.7-p375

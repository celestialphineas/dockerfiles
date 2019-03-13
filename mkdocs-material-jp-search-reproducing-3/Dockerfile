FROM python:2.7
WORKDIR /tmp
RUN rm -rf /tmp/*
RUN git clone https://github.com/squidfunk/mkdocs-material /tmp
RUN pip install -r /tmp/requirements.txt
RUN pip install python-markdown-math
RUN python /tmp/setup.py install
RUN git clone https://github.com/celestialphineas/ckcers-tutorial /ckcers-tutorial
WORKDIR /ckcers-tutorial
RUN rm -rf /tmp
EXPOSE 8000
CMD mkdocs serve

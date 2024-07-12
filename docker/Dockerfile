FROM python:3.12-bookworm

WORKDIR /usr/src/app

COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

COPY imap2rss ./imap2rss

ENV DATA_DIR=/data
ENV BIND=0.0.0.0:3042

CMD [ "python", "-m", "imap2rss" ]
FROM golang:1.7.1

ADD import_dashboards /dashboard

WORKDIR /dashboard

ENV $ES "http://elasticsearch:9200""
ENV USER "elastic"
ENV PASS "changeme"

CMD ["./import_dashboards", "-es", "$ES", "-user", "$USER", "-pass", "$PASS"]
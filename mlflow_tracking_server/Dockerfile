FROM python:3.9

LABEL maintainer "Florian Muchow <flmuchow@gmail.com>"
LABEL edited by "Allen ML Wu <Allen_ML_Wu@wistron.com>"

RUN pip install mlflow==1.18 && \
    pip install awscli --upgrade --user && \
    pip install boto3==1.16.46

ENV PORT 5000

COPY files/run.sh /

ENTRYPOINT ["/run.sh"]

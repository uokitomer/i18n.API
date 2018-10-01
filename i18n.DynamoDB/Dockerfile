FROM amazon/dynamodb-local

USER root
ENV SHARED=-sharedDb
ENV MODE=-dbPath
ENV VOL_PATH=/data

RUN if [[ ! -z $VOL_PATH ]]; then /bin/mkdir -p -m 0777 $VOL_PATH; fi 

ENTRYPOINT [""]

EXPOSE 8000

CMD java -jar DynamoDBLocal.jar ${MODE} ${VOL_PATH} ${SHARED}
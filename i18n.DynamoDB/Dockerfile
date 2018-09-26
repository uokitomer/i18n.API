FROM amazon/dynamodb-local

USER root

RUN mkdir -p -m 0777 /data

CMD ["-jar", "DynamoDBLocal.jar", "-sharedDb", "-dbPath", "/home/dynamodblocal/"]
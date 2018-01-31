Start a cluster:

-docker-compose up -d

Destroy a cluster:

-docker-compose stop


ports:
   - target: 9094
     published: 9094
     protocol: tcp
     mode: host


port 9092 for INSIDE listeners
port 9093 for BROKER listeners
port 9094 for OUTSIDE listeners


zookeeper:  ports: - 2181:2181
kafka:  ports: -9092 -9093 -9094

# apache-kafka

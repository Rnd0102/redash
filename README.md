# redash
Deployment Redash on Kubernetes
reference : https://github.com/getredash/redash/blob/master/docker-compose.yml

# Prerequsites:
1. A working K8s cluster
2. kubectl configured to work against your cluster
3. A PostgreSQL database URL with the redash database (not schema, only database) already created.

# Deployment
1. Clone this repository
2. create the DB schema:
   kubectl exec redash-server-xxxxxxxxx -c redash-server -- /app/bin/docker-entrypoint create_db`
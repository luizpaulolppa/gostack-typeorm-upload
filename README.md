# gostack-typeorm-upload

# Create new docker database
docker run --name NAME -e POSTGRES_PASSWORD=PASSWORD -p 5432:5432 -d postgres
docker run --name gostack_desafio06 -e POSTGRES_PASSWORD=docker -e POSTGRES_DB=gostack_desafio06 -p 5432:5432 -d postgres

docker ps -a
docker start ID

# Create new migration
yarn typeorm migration:create -n NAME_MIGRATE

# Run migrations
yarn typeorm migration:run

# Revert last migration
yarn typeorm migration:revert

# Show performed migrations
yarn typeorm migration:show


docker run --name gostack_desafio06 -e POSTGRES_PASSWORD=docker -p 5432:5432 -d postgres

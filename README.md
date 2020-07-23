DATABASE_URL=postres://postgres:postgres@172.18.0.2:5432/users_dev ./target/release/service run -p 8082
DATABASE_URL=postres://postgres:postgres@172.18.0.2:5432/users_dev ./target/release/service run -p 8080
DATABASE_URL=postres://postgres:postgres@172.18.0.2:5432/users_dev ./target/release/service run
DATABASE_URL=postres://postgres:postgres@172.18.0.2:5432/users_dev ./services/users/target/release/service run
docker-compose -f docker-compose-dev.yml run users ./services run
docker-compose -f docker-compose-dev.yml run users ./service init

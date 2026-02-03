COMPOSE = docker compose -f srcs/docker-compose.yml

all: up

up:
	$(COMPOSE) up -d --build

down:
	$(COMPOSE) down

clean:
	$(COMPOSE) down -v

fclean: clean
	sudo rm -rf /home/hporta-c/data
	docker system prune -af

re: clean up

.PHONY: all up down clean re

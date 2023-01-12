#!make

help: _header
	${info }
	@echo Opciones:
	@echo ---------------------------------
	@echo start
	@echo workspace
	@echo workspace-metasploitable2
	@echo stop / stop-all
	@echo build
	@echo stats / logs
	@echo clean
	@echo ---------------------------------

_header:
	@echo -------
	@echo Openvas (Modified by Julen Inigo)
	@echo -------

_urls: _header
	${info }
	@echo ----------------------------------
	@echo [Openvas] http://localhost:9392
	@echo ----------------------------------

_start:
	@docker compose up -d

start: _header _start _urls

stop:
	@docker compose stop

workspace:
	@docker exec -it openvas /bin/bash

workspace-metasploitable2:
	@docker exec -it metasploitable2 /bin/bash
stop-all:
	@docker stop $(shell docker ps -aq)

build:
	@docker compose build --pull

stats:
	@docker stats

logs:
	@docker compose logs openvas

clean:
	@docker compose down -v --remove-orphans

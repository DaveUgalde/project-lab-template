# Project Lab Template

Reproducible Environment developed with docker, VS Code Dev Containers, Foam (knowledge graph) & Ollama (local AI).

## Requirements

- Docker Desktop installed.
- VS Code with extension "Dev Containers".

## How to Use this template

1. Create a new repository from this template (use the botton "Use this template" in GitHub).
2. Clone your new repository in local.
3. Open the folder en VS Code.
4. Once the notification appears "Reopen in Container", click on it (or run `F1 > Dev Containers: Reopen in Container`).
5. Wait to build the container. Python, Foam & Ollama will be ready.
6. (Optional) Download a Language model: Open your terminal Integrated and execute: `ollama pull qwen2.5:14b`. 

## Structure:

- `.devcotainer/` - Configuration of the container of developement.
- `.foam/` - Active the knowledge graph Foam.
- `docker-compose.yml` - Run Ollama like service and the container of development.
- .gitignore - Files to exclude.
- README.md - This Document



## Customization

You can add services (DB, etc) editing `docker-componse.yml`.
The extensions of VS Code are defines in `devcontainer.json`.


## Start to work

- To create a knowledge graph: write concept/title embrace with doble square [[]] in any Markdown. Foam detects the link and show the graph (`F1 > Foam: Show graph`).
- To add programming languages: edit `.devcontainer/devcontainer.json` and include the Dev Container Features required (Node.js, Rust, Go, etc)
- To add Databases or any other service: edit docker-compose.yml and include PostgresSQL, Redis, etc. Then rebuild the container (`F1 -> Dev Containers: Rebuild and Reopen in Container`) 




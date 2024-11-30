# Practical RAG: Building Specialized Chatbots Step-by-Step

By Hocine Abdellatif Houari, [@hahouari](https://github.com/hahouari).

## Slides

Presentation can be found in [PDF](https://github.com/hahouari/practical_rag_course/blob/dev/presentation.pdf).

## RAG Steps

[This flow chart](https://github.com/hahouari/practical_rag_course/blob/dev/steps.png) explains how RAG steps are implemented under this course.

## Code Execution Prerequisites

- Python v3.12 environment, highly recommended using [Anaconda](https://www.anaconda.com/products/distribution).
- [SurrealDB](https://surrealdb.com/install) v2.1.2.
- [Surrealist](https://surrealdb.com/surrealist) v3.1.2.
- OpenAI API key, [here is how to get it](https://www.youtube.com/watch?v=bK5MQr6CXc8).

## Steps to run

### Setup Project

1. Copy `.env.example` to `.env` and fill the variables.

2. If you are not using SurrealDB through docker, [install it in your machine](https://surrealdb.com/docs/surrealdb/installation).

3. (Optional) If you want to install pip packages all at once:

   ```sh
   pip install -r requirements.txt
   ```

### Start the database

```sh
# if you are using docker
docker compose up
# or not using docker
surreal start -A --user root --pass root --bind 127.0.0.1:28900 surrealkv:data.db
```

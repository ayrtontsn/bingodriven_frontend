#Link do bingo:
https://bingodriven-frontend-1ckxb9774-ayrton-nascimentos-projects.vercel.app/

#comando para subir o projeto COM DOCKER COMPOSE
    docker compose up -d

#comando para subir o projeto SEM DOCKER COMPOSE
    docker build -t daily-kindness-frontend .
    docker run -d --name front-end -p 8080:80 daily-kindness-frontend
    //acessar: (http://localhost:8080/)
#Link do bingo:
https://bingodriven-frontend-1ckxb9774-ayrton-nascimentos-projects.vercel.app/

# Criar o arquivo `.env` com base no exemplo do `.env.example`;

#comando para subir o projeto SEM DOCKER COMPOSE
    docker build --build-arg VITE_BACKEND=http://localhost:5000 -t daily-kindness-frontend .
    docker run -d --name front-end --network mynetwork -p 8080:80 -e VITE_BACKEND=http://localhost:5000 daily-kindness-frontend

    # O argumento `--build-arg` é onde o backend está hospedado, nesse caso está hospedado no `localhost:5000`
    # Devem estar na mesma `--network`, nesse caso estão na rede `mynetwork`
    
    # acessar: (http://localhost:8080/)

#comando para subir o projeto COM DOCKER COMPOSE
    docker compose up -d --build


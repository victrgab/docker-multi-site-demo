# 🐳 Projeto Docker: Orquestração Multi-Site com NGINX

Este repositório é um projeto acadêmico para a disciplina de **Engenharia de Software**, demonstrando a orquestração de múltiplos serviços web isolados utilizando **Docker** e **Docker Compose**.

---

## ✨ Tecnologias Utilizadas

- **Containerização:** Docker & Docker Compose  
- **Servidor Web:** NGINX (`nginx:alpine`)  
- **Frontend:** HTML5, CSS3, JavaScript  

---

## 👨‍💻 Equipe / Autores

Este projeto foi desenvolvido por:

- [**Victor Gabriel de Oliveira Brito**](https://github.com/victrgab)  
- [**Pablo Caldeira Gomes Monteiro**](https://github.com/PabloCGM)  
- [**Walter Lucas Barros da Conceição**](https://github.com/wluca1)  
- [**João Marcos R C Marques**](https://github.com/JoaoRCM653)  
- [**João Gabriel Silva de Melo**](https://github.com/sopadmakc0)  
- [**Enzo Kauê Batista Ferreira**](https://github.com/EnzoKaue)  

---

## 🚀 O Projeto

O ambiente é composto por três sites independentes, cada um servido por seu próprio contêiner NGINX, demonstrando o conceito de isolamento de serviços:

1.  **Site 1**: Uma página de sucesso com uma animação de confirmação (Verde).
2.  **Site 2**: Uma segunda página de sucesso com estilo e cor diferentes (Azul).
3.  **Site 3**: Um serviço "secreto" que serve como um *Easter Egg*.

---

## 📂 Estrutura de Diretórios

A estrutura do projeto é organizada para que cada serviço tenha seus próprios arquivos de frontend de forma clara.
```
.
├── site1/
│   └── index.html      # Página de sucesso do Site 1 (Verde)
├── site2/
│   └── index.html      # Página de sucesso do Site 2 (Azul)
├── site3/
│   └── index.html      # Página "Easter Egg" (A Surpresa!)
├── .gitignore          # Arquivo para o Git ignorar itens desnecessários
├── docker-compose.yml  # Arquivo "maestro" que orquestra todos os serviços
└── README.md           # Esta documentação
```
---

## ⚙️ Como Executar o Projeto

**Pré-requisitos:** Docker e Docker Compose instalados e em execução.

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/victrgab/docker-multi-site-demo.git
    cd docker-multi-site-demo
    ```

2.  **Inicie os contêineres em segundo plano:**
    ```bash
    docker compose up -d
    ```

3.  **Para parar e remover todos os contêineres:**
    ```bash
    docker compose down
    ```

---

## 🌐 Acessando os Serviços

Após iniciar os contêineres, os sites estarão disponíveis nos seguintes endereços:

- **Site 1:** [http://localhost:8080](http://localhost:8080)
- **Site 2:** [http://localhost:8081](http://localhost:8081)
- **Site 3 (A Surpresa):** [http://localhost:8082](http://localhost:8082)

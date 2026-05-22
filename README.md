# arquivo-workflow
semana 8 aula 2
name: Minha Primeira Linha de Montagem

on:
  push:
    branches: [ main ]

jobs:
  construcao:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout do código
        uses: actions/checkout@v4

      - name: Saudacao do Robo
        run: echo "Iniciando a linha de montagem da fabrica!"

      - name: Executar tarefa
        run: echo "Processando materiais..."

Programa client.go

- [ ] Realizar requisição http no server.go solicitando a cotação do dólar
- [ ] A requisição para o server.go deve possuir um timeout de 300ms
- [ ] Salvar a cotação atual recebida no arquivo cotacao.txt no formato de: Dólar: {valor}

Programa server.go

- [ ] Consumir a API contendo o câmbio de Dólar e Real
- [ ] Retornar o resultado no formato JSON para o cliente
  - [ ] Enviar apenas o valor atual do câmbio, campo bid do JSON da API de cotação
- [ ] Usando o package context, registrar no SQLite cada cotação recebida
- [ ] A requisição para a API de cotação de dólar deverá possuir um timeout de 200ms
- [ ] O timeout da operação para persistir os dados no SQLite deverá ser de 10ms
- [ ] Disponibilizar o endpoint para o client.go em /cotacao
- [ ] A porta do servidor http deve ser a 8080

Geral

- [ ] Os 3 contextos deverão retornar erro nos logs caso o tempo de execução seja insuficiente

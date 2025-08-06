# 🔧 Oficina Mecânica – Esquema Conceitual

## 📘 Descrição

Modelo conceitual de banco de dados para uma oficina mecânica, com foco no gerenciamento de ordens de serviço, clientes, veículos, equipes, mecânicos, serviços e peças. Criado com base na narrativa de um desafio da DIO.

---

## 🛠️ Entidades e Relacionamentos

### 🔹 Cliente
- idCliente (PK)
- Nome
- Celular
- Endereço

### 🔹 Veículo
- idVeiculo (PK)
- Modelo
- Placa
- Marca
- Ano
- Cliente_idCliente (FK)

### 🔹 OrdemDeServico
- idOrdemDeServico (PK)
- DataEmissao
- DataConclusao
- Status
- ValorTotal
- Veiculo_idVeiculo (FK)
- Veiculo_Cliente_idCliente (FK)
- Equipe_idEquipe (FK)

### 🔹 Equipe
- idEquipe (PK)
- NomeEquipe

### 🔹 Mecanicos
- idMecanicos (PK)
- Nome
- Endereço
- Especialidade
- Equipe_idEquipe (FK)

### 🔹 Serviços
- idServicos (PK)
- Descrição
- Valor
- OrdemDeServico_idOrdemDeServico (FK)

### 🔹 Peças
- idPeças (PK)
- Descrição
- Valor
- OrdemDeServico_idOrdemDeServico (FK)

---

## 🖼️ Diagrama

![Modelo ER](diagrama2.png)

---

## ✍️ Autor

Desenvolvido por **Vinicius Borges** ([Vborges95](https://github.com/Vborges95))

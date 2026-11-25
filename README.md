# Gym Manager — Customer Registration System

<div align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-yellow" alt="Python 3.10+">
  <img src="https://img.shields.io/badge/Flet-0.21.2-blue" alt="Flet 0.21.2">
  <img src="https://img.shields.io/badge/Storage-JSON-lightgrey" alt="JSON storage">
  <img src="https://img.shields.io/badge/License-MIT-green" alt="MIT License">
</div>

<div align="center">
  <a href="#portugues">🇧🇷 Português</a> |
  <a href="#english">🇺🇸 English</a>
</div>

<a id="portugues"></a>

## 🇧🇷 Português

### Sobre o projeto

O **Gym Manager** é uma aplicação desktop desenvolvida como projeto de estudo para praticar Python e criação de interfaces com Flet. O sistema simula o cadastro e a consulta visual de clientes de uma academia, armazenando os registros localmente em um arquivo JSON.

A aplicação permite registrar clientes com nome, CPF e plano contratado, atribuindo automaticamente uma quantidade de dias de validade conforme o plano selecionado.

### Funcionalidades

- Cadastro de clientes com nome, CPF e plano.
- Formatação automática do CPF durante a digitação.
- Planos disponíveis: Basic, Premium, Gold e VIP.
- Definição da quantidade de dias de validade conforme o plano:
  - Basic: 30 dias.
  - Premium: 60 dias.
  - Gold: 90 dias.
  - VIP: 120 dias.
- Exibição dos clientes cadastrados em uma tabela.
- Persistência local dos registros em arquivo JSON.
- Botão para limpar os campos do formulário.

### Tecnologias

- **Python 3.10+** — linguagem de programação.
- **Flet 0.21.2** — construção da interface gráfica.
- **JSON** — armazenamento local dos dados.

### Arquitetura

O projeto utiliza uma estrutura simples, sem backend ou banco de dados servidor. A interface desenvolvida com Flet executa a lógica da aplicação e utiliza o módulo de persistência para carregar e salvar os registros em um arquivo JSON.

```text
Interface Flet
     |
     v
Lógica da aplicação (main.py)
     |
     v
Persistência local (services/db.py)
     |
     v
Arquivo JSON (services/db.json)
```

### Estrutura do projeto

```text
mvp-customer-register/
├── main.py              # Ponto de entrada e interface principal
├── search.py            # Módulo reservado para a tela de busca
├── services/
│   ├── db.py            # Leitura e gravação dos dados
│   └── db.json          # Armazenamento local dos clientes
└── README.md
```

### Como executar

**Pré-requisitos**

- Python 3.10 ou superior.
- pip.

**1. Clone o repositório**

```bash
git clone https://github.com/braaia/mvp-customer-register.git
cd mvp-customer-register
```

**2. Crie e ative um ambiente virtual (recomendado)**

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

Linux / macOS:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

**3. Instale o Flet**

```bash
pip install flet==0.21.2
```

**4. Execute a aplicação**

```bash
python main.py
```

### Estado do projeto

Projeto de estudo em estágio de protótipo. O fluxo principal de cadastro e armazenamento local está implementado. O módulo de busca está apenas como estrutura inicial e ainda não possui funcionalidade implementada.

### Autor

Desenvolvido por **Braia**.

- GitHub: [github.com/braaia](https://github.com/braaia)
- LinkedIn: [linkedin.com/in/wesleynog](https://www.linkedin.com/in/wesleynog/)

---

<a id="english"></a>

## 🇺🇸 English

### About

**Gym Manager** is a desktop application developed as a study project to practice Python and GUI development with Flet. It simulates customer registration for a gym and stores records locally in a JSON file.

The application allows users to register customers with their name, CPF (Brazilian individual taxpayer identification number), and selected membership plan. Each plan is associated with a predefined number of validity days.

### Features

- Register customers with name, CPF, and membership plan.
- Automatically format CPF input while typing.
- Available plans: Basic, Premium, Gold, and VIP.
- Assign a predefined number of validity days based on the selected plan:
  - Basic: 30 days.
  - Premium: 60 days.
  - Gold: 90 days.
  - VIP: 120 days.
- Display registered customers in a data table.
- Store customer records locally in a JSON file.
- Clear the registration form fields.

### Technologies

- **Python 3.10+** — programming language.
- **Flet 0.21.2** — graphical user interface framework.
- **JSON** — local data storage.

### Architecture

The project uses a simple architecture with no backend server or server-based database. The Flet interface runs the application logic and uses a persistence module to load and save customer records in a JSON file.

```text
Flet Interface
      |
      v
Application Logic (main.py)
      |
      v
Local Persistence (services/db.py)
      |
      v
JSON File (services/db.json)
```

### Project Structure

```text
mvp-customer-register/
├── main.py              # Application entry point and main interface
├── search.py            # Placeholder for the search view
├── services/
│   ├── db.py            # Data loading and saving
│   └── db.json          # Local customer data storage
└── README.md
```

### How to Run

**Prerequisites**

- Python 3.10 or later.
- pip.

**1. Clone the repository**

```bash
git clone https://github.com/braaia/mvp-customer-register.git
cd mvp-customer-register
```

**2. Create and activate a virtual environment (recommended)**

Windows:

```bash
python -m venv .venv
.venv\Scripts\activate
```

Linux / macOS:

```bash
python3 -m venv .venv
source .venv/bin/activate
```

**3. Install Flet**

```bash
pip install flet==0.21.2
```

**4. Run the application**

```bash
python main.py
```

### Project Status

Study project at the prototype stage. The main customer registration and local storage flow is implemented. The search module is currently a placeholder and does not yet provide a working search feature.

### Author

Developed by **Braia**.

- GitHub: [github.com/braaia](https://github.com/braaia)
- LinkedIn: [linkedin.com/in/wesleynog](https://www.linkedin.com/in/wesleynog/)

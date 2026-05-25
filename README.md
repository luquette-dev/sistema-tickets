# 🎫 Sistema de Tickets de TI

Sistema de gerenciamento de chamados (help desk) desenvolvido em Python com banco de dados SQLite. Projeto criado para simular o fluxo real de atendimento em um service desk corporativo.

---

## 📋 Sobre o projeto

Este projeto nasceu do desejo de entender como funciona um sistema de tickets por dentro — a mesma estrutura usada por ferramentas como Jira Service Desk, GLPI e Zendesk. Em vez de apenas usar essas ferramentas, construí uma do zero para aprender os conceitos fundamentais de suporte de TI.

---

## ⚙️ Funcionalidades

- ✅ Abertura de tickets com título, descrição, categoria e prioridade
- ✅ Listagem com filtro por status, categoria ou prioridade
- ✅ Atualização de status com registro de técnico responsável
- ✅ Histórico completo de cada chamado
- ✅ Relatório resumido por status, categoria e prioridade
- ✅ Ordenação automática por criticidade (crítica → alta → média → baixa)
- ✅ Banco de dados SQLite persistente

---

## 🗂️ Categorias e prioridades

**Categorias:** `hardware` · `software` · `rede` · `acesso` · `outro`

**Prioridades:** `baixa` · `media` · `alta` · `critica`

**Status:** `aberto` → `em_andamento` → `resolvido` → `fechado`

---

## 🚀 Como rodar

### Pré-requisitos
- Python 3.8 ou superior
- Nenhuma dependência externa (apenas bibliotecas padrão do Python)

### Instalação

```bash
# Clone o repositório
git clone https://github.com/seu-usuario/sistema-tickets.git
cd sistema-tickets

# Execute o sistema
python src/main.py
```

---

## 🖥️ Demonstração

```
=======================================================
        SISTEMA DE TICKETS DE TI — HELP DESK
=======================================================

  1. Abrir novo ticket
  2. Listar tickets
  3. Ver detalhes de um ticket
  4. Atualizar status de ticket
  5. Ver histórico de ticket
  6. Relatório resumido
  0. Sair
```

---

## 🏗️ Estrutura do projeto

```
sistema-tickets/
├── src/
│   ├── main.py          # Interface de terminal (menu interativo)
│   ├── tickets.py       # Lógica de negócio (abrir, listar, atualizar)
│   └── database.py      # Conexão e inicialização do banco SQLite
├── data/
│   └── tickets.db       # Banco de dados (gerado automaticamente)
├── docs/
│   └── ...              # Documentação adicional
├── .gitignore
└── README.md
```

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|------------|-----|
| Python 3   | Linguagem principal |
| SQLite3    | Banco de dados local |
| datetime   | Controle de timestamps |

---

## 📚 Conceitos aplicados

- CRUD completo (Create, Read, Update, Delete)
- Relacionamento entre tabelas (tickets ↔ histórico)
- Filtros dinâmicos em SQL
- Separação de responsabilidades (database · business logic · interface)
- Fluxo de atendimento baseado em ITIL (conceitos de incidente e SLA)

---

## 🔮 Próximas melhorias

- [ ] Interface web com Flask
- [ ] Sistema de login para técnicos
- [ ] Exportação de relatórios em CSV
- [ ] Notificações por e-mail ao abrir/resolver chamado
- [ ] Dashboard com gráficos

---

## 👤 Autor

**Gabriel Luquette**  
Estudante de Sistemas de Informação — FMU  
[LinkedIn](https://linkedin.com/in/seu-perfil) · [GitHub](https://github.com/luquette-dev)

---

> Projeto desenvolvido para aprendizado prático de Python, banco de dados e conceitos de service desk/ITIL.

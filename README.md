# Plan It Agenda

**Versão 1.0 — Sistema Desktop para Agendamento de Serviços de Estética**

## 💡 Sobre o Projeto

O **Plan It Agenda** é um sistema desktop desenvolvido em Java (Swing) que ajuda profissionais da área de estética — como Nail Designers — a gerenciarem seus clientes, serviços e agendamentos. O sistema oferece visualização de agenda, exportação de relatórios e controle por perfil de usuário (Administrador e Funcionário).

Projeto acadêmico para a disciplina de Desenvolvimento de Software Desktop (UniRios - Sistemas de Informação).

---

## 🛠️ Tecnologias Utilizadas

| Camada                  | Tecnologia         |
|-------------------------|--------------------|
| Linguagem               | Java (POO)         |
| Interface Gráfica       | Java Swing         |
| Banco de Dados          | MySQL              |
| Estilização Visual      | FlatLaf            |
| Gerenciador de Build    | Maven              |
| IDE recomendada         | IntelliJ IDEA      |

---

## ⚙️ Funcionalidades

- Login com controle de perfil (Admin e Funcionário)
- Cadastro, edição e exclusão de Clientes e Serviços
- Agendamento com verificação de conflito de horário
- Visualização semanal e mensal da agenda
- Consulta de histórico por cliente ou serviço
- Geração de relatórios (.CSV)
- Interface moderna com padrão visual padronizado

---

## 🧪 Como Executar o Programa

### 📌 Pré-requisitos

- Java JDK 17 ou superior
- MySQL Server 5.7+ ou MariaDB
- Maven
- IDE (recomendado: IntelliJ IDEA)

---

### 🗄️ Configuração do Banco de Dados

1. Crie um banco de dados chamado `planitagenda`.

2. Execute o script SQL localizado em:
```
src/main/resources/planitagenda.sql
```

3. Certifique-se de que as credenciais do seu banco estão corretas no arquivo:
```
src/main/resources/db.properties
```

Exemplo:
```properties
db.url=jdbc:mysql://localhost:3306/planitagenda
db.user=root
db.password=12345
```

> ⚠️ Caso altere o nome do banco ou a senha, atualize também o `db.properties`.

---

### 🚀 Compilar e Rodar

1. Clone o repositório:
```bash
git clone https://github.com/pauloolileite/PlanIt.git
cd PlanIt
```

2. Compile o projeto com Maven:
```bash
mvn clean package
```

3. Execute a aplicação:
```bash
java -jar out/artifacts/PlanIt_jar/PlanIt.jar
```

---

## 📁 Estrutura do Projeto

```
PlanIt/
├── src/main/
│   ├── Controller/     # Lógica de controle (MVC)
│   ├── DAO/            # Camada de acesso a dados
│   ├── Model/          # Entidades do sistema
│   ├── Utils/          # Utilitários e componentes visuais
│   └── View/           # Telas do sistema (Swing)
├── src/main/resources/
│   ├── db.properties   # Configuração do banco
│   ├── planitagenda.sql# Script SQL para criação do banco
│   └── Icons/, Imagens/# Recursos visuais
├── out/artifacts/      # JAR final gerado
├── pom.xml             # Configuração Maven
└── README.md           # Este documento
```

---

## 🔐 Usuário Padrão

- **Usuário**: `admin`
- **Senha**: `1234`

---

## 🧾 Licença

Este é um projeto acadêmico, sem fins lucrativos. Todos os direitos reservados ao autor.

---

## 👨‍💻 Autor

**Paulo Victor Oliveira Leite da Silva**  
Estudante de Sistemas de Informação - UniRios  
[GitHub: pauloolileite](https://github.com/pauloolileite)

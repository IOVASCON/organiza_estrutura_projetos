# 📝 Descrição  

![Logo](logo.webp)

Este projeto visa agilizar e padronizar a criação de novos projetos em Python por meio de um script Bash automatizado. Com um único comando, o script gera a estrutura essencial de diretórios e arquivos, configurando o ambiente de desenvolvimento de forma rápida e eficiente.  

## 🎯 Objetivo do Projeto

O objetivo principal deste projeto é **eliminar a repetição de tarefas manuais na configuração inicial de projetos Python, proporcionando uma estrutura organizada e pronta para uso, reduzindo erros e aumentando a produtividade dos desenvolvedores**.  

## 🚀 Funcionalidades

- **Criação Automática da Estrutura do Projeto:** Gera diretórios como `src/`, `tests/`, `docs/`, entre outros.  
- **Configuração do Ambiente Virtual:** Inicializa um ambiente virtual para o gerenciamento de dependências.  
- **Geração de Arquivos Essenciais:** Inclui `README.md`, `.gitignore`, `requirements.txt` e arquivos de inicialização do projeto.  
- **Facilidade de Uso:** Executa tudo com um único comando, tornando o processo simples e eficiente.

## 🛠️ Como Usar o Script de Configuração do Projeto

Este projeto foi configurado usando o script **`setup_project.sh`**, que cria automaticamente:

- Estrutura básica de pastas e arquivos.
- Ambiente virtual configurado.
- Dependências essenciais instaladas.

## 📂 1. Estrutura do Projeto

A estrutura gerada pelo script inclui:

📦 nome_do_projeto/
├── 📂 src/           # Código-fonte principal
├── 📂 data/          # Dados para simulações ou testes
├── 📂 tests/         # Scripts para testes unitários
├── 📂 docs/          # Documentação adicional
├── 📂 images/        # Imagens coletadas ou geradas no desenvolvimento
├── 📂 venv/          # Ambiente virtual (ignorado pelo Git)
└── 📄 .gitignore     # Arquivos a serem ignorados pelo Git

## 🔧 2. Como Usar o Script

### Passo 1: Salve o Script

Salve o código do script como **`setup_project.sh`** no seu computador.

### Passo 2: Dê Permissão de Execução

No terminal, execute o seguinte comando para permitir a execução do script:

chmod +x setup_project.sh

### Passo 3: Execute o Script

Para criar um novo projeto, execute o script com o nome do projeto como argumento:

./setup_project.sh nome_do_projeto

## ▶️ 3. Como Executar o Projeto

### Passo 1: Ative o Ambiente Virtual

- **No Windows (Git Bash ou Terminal VSCode):**

  source venv/Scripts/activate

- **No Linux/Mac:**

  source venv/bin/activate

### Passo 2: Execute o Arquivo Principal

Depois de ativar o ambiente virtual, execute o arquivo principal do projeto:

python main.py

## 📦 4. Como Adicionar Dependências

### Instalar um Pacote

Instale um pacote necessário ao projeto usando o comando:

pip install nome_do_pacote

### Atualizar o **`requirements.txt`**

Depois de instalar os pacotes, atualize o arquivo **`requirements.txt`** com o seguinte comando:

pip freeze > requirements.txt

## 🔍 5. Usando o `pipreqs`

### Para Gerar um Arquivo de Dependências Enxuto

Você pode usar o **`pipreqs`** para criar um **`requirements.txt`** contendo apenas as bibliotecas usadas diretamente no projeto.

### Passo 1: Instale o `pipreqs`

Ative o ambiente virtual e instale o **`pipreqs`**:

pip install pipreqs

### Passo 2: Gere o Arquivo

No diretório do projeto, execute:

pipreqs ./ --force

- **`./`**: Representa o diretório atual.
- **`--force`**: Sobrescreve o arquivo **`requirements.txt`** existente.

## 🗂️ 6. Manutenção no GitHub

### Atenção ao **`.gitignore`**

Certifique-se de manter o arquivo **`.gitignore`** atualizado para evitar versionar arquivos desnecessários, como:

- O diretório **`venv/`** (ambiente virtual).
- Arquivos temporários ou de cache.

## 🎯 7. Resultado Esperado

Após executar o script, você terá:

- Uma estrutura organizada de diretórios e arquivos.
- Um ambiente virtual configurado.
- Dependências instaladas e um **`requirements.txt`** gerado.
- Um **`.gitignore`** configurado corretamente.
- Um **`USAGE.md`** com instruções claras de uso.

![Resultado Final](https://via.placeholder.com/800x400?text=Resultado+Final)

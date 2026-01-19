# Python REFramework

Framework padrão para automações Python seguindo o padrão REFramework (Robotic Enterprise Framework).

## 📋 Descrição

Este projeto implementa o padrão REFramework em Python, uma arquitetura robusta para automações que oferece:

- **Tratamento de exceções**: Gestão inteligente de erros de sistema e negócio
- **Processamento transacional**: Gestão de filas com estados bem definidos
- **Configuração centralizada**: Arquivo YAML para todas as configurações
- **Logging estruturado**: Sistema de logs detalhado para rastreabilidade
- **Arquitetura modular**: Separação clara de responsabilidades

## 🏗️ Estrutura do Projeto

```text
python-reframework/
├── data/
│   ├── input/          # Arquivos de entrada
│   ├── output/         # Arquivos de saída
│   └── work/           # Arquivos temporários
├── settings/
│   └── config.yaml     # Configurações do projeto
├── src/
│   ├── adapters/       # Adaptadores (Queue, etc)
│   ├── core/           # Configurações e utilitários centrais
│   ├── states/         # Estados do REFramework
│   └── main.py         # Ponto de entrada
└── tests/              # Testes automatizados
```

## 🚀 Como Usar

### Pré-requisitos

- Python 3.8+
- pip

### Instalação

1. Clone o repositório:

```bash
git clone https://github.com/DBCBR/python-reframework.git
cd python-reframework
```

1. Instale as dependências:

```bash
pip install -r requirements.txt
```

1. Configure o arquivo `settings/config.yaml` conforme necessário

### Execução

```bash
python src/main.py
```

## 🔄 Estados do REFramework

1. **Init State**: Inicialização e carregamento de configurações
2. **Get Transaction State**: Obtém item da fila para processar
3. **Process Transaction State**: Processa o item atual
4. **End State**: Finalização e limpeza

## ⚙️ Configuração

Edite o arquivo `settings/config.yaml` para personalizar:

- Parâmetros de execução
- Número máximo de tentativas
- Caminhos de arquivos
- Outras configurações do processo

## 🧪 Testes

Execute os testes com:

```bash
python -m pytest tests/
```

## 📝 Licença

Este projeto está sob licença MIT.

## 👥 Contribuindo

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou pull requests.

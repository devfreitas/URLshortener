# Encurtador de URL com Python

Um projeto simples desenvolvido em **Python** que permite encurtar URLs utilizando a API gratuita do **TinyURL**. O programa funciona via terminal e oferece um menu interativo para facilitar o uso.

## Funcionalidades

* Encurtar URLs utilizando a API do TinyURL.
* Validação básica da URL informada.
* Interface simples via terminal.
* Tratamento de erros de conexão e requisições.
* Opção para encurtar várias URLs sem reiniciar o programa.

## Tecnologias Utilizadas

* Python 3.x
* Biblioteca `requests`
* API TinyURL

## Instalação

1. Clone este repositório:

```bash
git clone https://github.com/devfreitas/URLshortener.git
```

2. Acesse a pasta do projeto:

```bash
cd URLshortener
```

3. Instale a dependência necessária:

```bash
pip install requests
```

## Como Executar

Execute o arquivo principal:

```bash
python main.py
```

## Exemplo de Uso

```text
=== Encurtador de URL usando TinyURL ===

1. Encurtar URL
2. Sair

Escolha uma opção (1/2): 1

Digite a URL que deseja encurtar:
https://www.google.com

URL encurtada com sucesso!

Original: https://www.google.com
Encurtada: https://tinyurl.com/xxxxx
```

## Estrutura do Projeto

```text
encurtador-url
 ┣ main.py
 ┣ README.md
 ┗ requirements.txt (opcional)
```

## Funcionamento

O programa realiza os seguintes passos:

1. Exibe um menu de opções.
2. Solicita a URL que será encurtada.
3. Verifica se a URL começa com `http://` ou `https://`.
4. Envia uma requisição para a API do TinyURL.
5. Exibe a URL encurtada ao usuário.
6. Permite realizar novas operações até que o usuário escolha sair.

## Exemplo de Requisição

```python
requests.get(f"https://tinyurl.com/api-create.php?url={url}")
```

## Dependências

Instale a biblioteca necessária com:

```bash
pip install requests
```

Ou utilize um arquivo `requirements.txt` contendo:

```text
requests
```

Depois execute:

```bash
pip install -r requirements.txt
```

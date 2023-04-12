# chatGPT_candidatos
**Criando um chatGPT organizacional para a busca de candidatos a vagas de trabalho baseado em banco de currículos em pdf usando linguagem natural.**

Olá, vou mostrar como você pode treinar o modelo do [chatGPT](https://openai.com/blog/chatgpt) para que use seus próprios dados em PDF de currículos que sua empresa tenha, para que a área de Recursos Humanos ou alguém em busca de candidatos possa, de forma natural, fazer consultas e literalmente conversar com a inteligência  economizando tempo e sendo mais assertivos na busca.

Para simular um banco de dados de currículos, eu pedi ao ChatGPT que criasse 20 currículos com dados simulados de pessoas e com algumas categorias como idioma, objetivo etc. \
Eu separei estes arquivos em 20 PDFs, simulando o que geralmente as empresas têm em pastas na rede ou nos computadores.

**Informações**
* Dados: arquivos pdf dos currículos com dados simulados em /docs 
* Modelo já treinado e indexados para estes dados: arquivo index.json 

Caso tenha mais dados coloque-os na pasta docs e execute o script novamente para treinar o modelo novamente.

**1 - Tenha o git instalado** 

[Download aqui](https://git-scm.com/downloads)

**2 - Clone o repositório para seu computador**

`git clone https://github.com/geovanijpires/chatGPT_candidatos.git`

**3 - Instalação do python:**

[Download aqui](https://www.python.org/downloads/)

**4 - Crie o ambiente virtual do python e ative**

`python -m venv .env` \
`.env\Scrits\activate`

**5 - Instale os pacotes necessários**

`pip install -r requirements.txt`

**6 -Gere sua chave da OpenAI** 

[Cadastro e acesso a openai](https://platform.openai.com/signup) 

Gere a chave indo em: [https://platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys)

**7 - Insira sua chave da OpenAI no arquivo app.py**

`os.environ["OPENAI_API_KEY"] = 'Sua chave OpenIA Api aqui'`

**8 - Treine o modelo e execute a aplicação do chat**

`python app.py`

**9 - Ao término da execução do script acesse a interface para interagir com o chat**

[http://127.0.0.1:7860](http://127.0.0.1:7860)

Referências: \
https://openai.com/blog/chatgpt \
https://beebom.com/how-train-ai-chatbot-custom-knowledge-base-chatgpt-api/

# PersonalCheff
<!---Esses são exemplos. Veja https://shields.io para outras pessoas ou para personalizar este conjunto de escudos. Você pode querer incluir dependências, status do projeto e informações de licença aqui--->
![Python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![HTML](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
<img src="exemplo.jpg" alt="exemplo imagem">
>Uma aplicação web de receitas chamada PersonalCheff desenvolvida durante o curso de Python no Senac Americana. A aplicação listará receitas e clicando em cada nome de receita você pode ver a receita completa.
### Lista de tarefas
Segue a lista de tarefas a serem desenvolvidas no projeto:
- [X] Pré-requisitos
    - [X] Instalar o Python
    - [X] Instalar Visual Studio Code
- [X] Criar e ativar o ambiente virtual
```
python -m venv .\venv\
venv\Scripts\activate
```
- [ X] Instalar o Django
- [X] Criar o projeto PersonalCheff
```
django-admin.py startproject PersonalCheff2
```
- [X] Subir o servidor e testar o projeto
```
entrar na pasta do projeto
cd PersonalCheff2

executar o projeto no servidor
python manage.py runserver
```
- [X] Alterar o idioma do projeto para `pt-br`
```
abrir o arquivo `settings.py` e na linha 106 para trocar `en-us` para `pt-br`
```
- [X] Alterar o timezone do projeto para `America/Sao_Paulo`
```
ir em settings e mudar o timezone
```
- [X] Criar o app receitas
```
* preciso estar dentro da pasta (PersonalCheff2) criar um app receitas
python manage.py startapp receitas
```
- [X] Registrar o app receitas
```
no arquivo settings.py adicionar o app receitas na lista de apps
INSTALED_APPS[
    ...
    'receitas',
]
```
- [X] Configurar a rota inicial(index)
- [X] Criar a view para a rota inicial
- [X] Registrar a rota inicial
- [X]Criar arquivo index.html
- [X] Integrar arquivos estáticos (CSS, JS)
    - Dentro da pasta do projeto (PersonalCheff2), criar a pasta **static**
    - Dentro da pasta **static**, colocar as imagens, os arquivos css e os arquivos js que for utilizar
    - No arquivo **settings.py**:
         - realize a importação da biblioteca **os** através do comando **import os**
         - na linha 58 adicione o caminho dos templates da seguinte forma:
         ```python
          'DIRS': [os.path.join(BASE_DIR, 'receitas/templates')],
         ```
         - no final do arquivo, após a linha **STATIC_URL** insira o seguinte código:
         ```python
        STATIC_ROOT = os.path.join(BASE_DIR, 'static')
        STATICFILES_DIRS = [
            os.path.join(BASE_DIR, 'PersonalCheff2/static')
        ]
        ```
        - **STATIC_URL** :  configuração da rota através do qual os arquivos estáticos seram servidos
        - **STATIC_ROOT** : configuração da pasta de saída(destino) dos arquivos estáticos
        - **STATICFILES_DIRS** : configuração da(s)  pasta de origem dos arquivos estáticos.
        - após realizar essas configurações execute, no terminal, o comando **python manage.py collectstatic**
        - na primeira linha do arquivo **index.html** insira **{% load static %}**. Esse comando deve ser usado em todos os arquivos em que você for utilizar arquivos estáticos.
        - insira uma imagem utilizando o comando **<img src="{% static 'logo.png'  %}">**. Sempre que for utilizar um arquivo estático você deve utilizar **{% static 'nome-do-arquivo' %}**
    - [X] Utilizando links
      - para criar um link para a página index, independente de onde você esteja utilize o comando **url**:
     ```python
        <a href="{% url 'index' %}">Página inicial</a>
     ```
  - [X] Criando o base.html
    - na pasta **templates** crie o arquivo **base.html**. Esse arquivo contém todo o código de estrutura comum à todas as paginas. Nesse arquivo deve ficar tudo que tiver antes do **body** e tudo que tiver depois do **/body**.
- [] Separando em partials
    -
- [] Renderizando dados dinamicamente
    -
- [] Criando um dicionario com as receitas
    -
- [] Criando o banco de dados(MySQL/MariaDB)
    -
- [] Instalando o conector do bando de dados MySQL
    -
- [] Criando o modelo da receita
    - 
- [] Criando a migration (mapeamento)
    -
- [] Realizando a migration
    -
- [] Registrando um modelo no admin
    -
- [] Criando um usuário para o ambiente administrativo
    -



## 📝 Licença
Esse projeto está sob licença. Veja o arquivo [LICENÇA](LICENSE.md) para mais detalhes.
[⬆ Voltar ao topo](#nome-do-projeto)<br>
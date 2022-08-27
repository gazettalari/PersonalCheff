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
- [ ] Configurar a rota inicial(index)
- [ ] Criar a view para a rota inicial
- [ ] Registrar a rota inicial
- [ ]Criar arquivo index.html

## 📝 Licença
Esse projeto está sob licença. Veja o arquivo [LICENÇA](LICENSE.md) para mais detalhes.
[⬆ Voltar ao topo](#nome-do-projeto)<br>
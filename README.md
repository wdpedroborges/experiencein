# ExperienceIn

- Trata-se de uma rede social desenvolvida em Django, onde os usuários podem convidar uns aos outros para eventos.

# Tecnologias utilizadas

- Python 3.7
- virtualenv
- Django 2.2
- Bootstrap

# Link para a aplicação em funcionamento:

http://xpedrostewart.pythonanywhere.com/

# Execução Local

git clone https://github.com/wdpedroborges/experiencein

cd experiencein/experiencein

manage.py runserver

# Passos de Implantação em PythonAnywhere.com

1. git clone https://github.com/wdpedroborges/experiencein

2. pip3 install virtualenv

3. mkvirtualenv --python=/usr/bin/python3.7 experiencein-virtualenv

4. pip install django==2.2

5. Crie um novo "web app"

6. Selecione a configuração manual: "Manual configuration (including virtaulenvs)"

7. Selecione a versão 3.7 do Python

8. Web # Virtualenv # Enter path to a virtualenv, if desired # /home/xpedrostewart/.virtualenvs/experiencein-virtualenv

9. Clique no link WSGI configuration file na seção Code da página de configuração de nossa web app

10. Deixe somente a seção do Django no arquivo, as demais seções deverão ser deletadas

11. Troque "mysite" por "experiencein"

12. Files # experiencein # experiencein # setting.py # ALLOWED_HOSTS  = ['xpedrostewart.pythonanywhere.com']

13. No final do arquivo settings.py, acrescente: STATIC_ROOT = '/home/xpedrostewart/experiencein/static'

14. Procure DEBUG = True e mulde para False

15. Acesse o bash, entre na pasta experiencein e dê o comando: python manage.py collectstatic

16. Dashborad # Web # Static files # Enter URL = /static/ e Enter path = /home/xpedrostewart/experiencein/static
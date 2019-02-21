1. Create Python environment at aws-flask\venv:
$ conda create --prefix venv python=3.7

2. Activate the environment
$ cd venv
$ conda activate %cd%

3. Install the serverless plugins:
$ cd ..
$ cd app
$ sls plugin install -n serverless-wsgi
$ sls plugin install -n serverless-python-requirements

3. Install flask and freeze the requirements
$ pip install flask
$ pip freeze > requirements.txt

4. Deploy
$ sls deploy
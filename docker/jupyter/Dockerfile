# kaggleのpython環境をベースにする
FROM gcr.io/kaggle-images/python:v91

# コマンドをprint
RUN set -x
# RUN pip install pipenv \
#  && pipenv install --system --dev

# setup jupyter
RUN jupyter notebook --generate-config -y && \
    sed -i -e "s/#c.NotebookApp.ip = 'localhost'/c.NotebookApp.ip = '*'/" /root/.jupyter/jupyter_notebook_config.py && \
    sed -i -e "s/#c.NotebookApp.allow_remote_access = False/c.NotebookApp.allow_remote_access = True/" /root/.jupyter/jupyter_notebook_config.py
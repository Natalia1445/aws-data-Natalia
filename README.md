# Instalación de programas requeridos para el Módulo Data ✅
## Python Versión 3.12 en Ubuntu
Se buscó la instalación en el buscador de Google en la página oficial, se encontró el código pero no la forma de instalación, por lo que se buscó directamente una guía de instalación en
Google, y se encontró la siguiente página https://launchpad.net/~deadsnakes/+archive/ubuntu/ppa, sin embargo, Ubuntu seguía sin encontrar el comando python3.12 por la versión de Ubuntu,
y se procedió a otra alternativa de instalación, el cual se encuentra en la siguiente página, el cual consiste instalar la versión de Python desde el código 
o archivo del creador o desarrollador oficial. https://wiki.crowncloud.net/?How_to_Install_Python_3_12_on_Ubuntu_20_04.
## Docker y Docker Compose 
En el caso de Docker fue más sencillo, pues se siguieron los pasos que se encuentran en la documentación oficial, y se instaló correctamente. 
https://docs.docker.com/engine/install/ubuntu/ 
##  Virtual Env
En el buscador de Google se solicitó lo siguiente: virtualenv on ubuntu for python 3.12. Y entre los resultados arrojados, se encontró la siguiente página y se utilizaron los comandos 
de la segunda respuesta https://stackoverflow.com/questions/77230254/cannot-properly-create-a-virtual-enviroment-in-python-3-12 : 
sudo apt install python3.12-venv
python3.12 -m venv new_venv
## Jupyter Notebook 
Se encontró la documentación oficial, en la siguiente página, se encuentran los comandos utilizados: https://jupyter.org/install hasta Jupyter notebook, primero se intentó solo instalar 
Nupyter Notebook, pero al marcar error, se optó por seguir las instrucciones de forma secuencial y finalmente pudo correr Jupyter Notebook 
pip install jupyterlab
jupyter lab
pip install notebook
jupyter notebook 



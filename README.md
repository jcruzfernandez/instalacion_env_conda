# instalacion_env_conda
Notas que servirán para instalacion de anaconda y entornos virtuales en Jupyter 

Se asume que ya tienes instalado Jupyter en tu maquina ;)
1. Una vez instalado anaconda a traves de https://www.anaconda.com/distribution/#download-section

2. Crear los entornos virtuales que necesites:
    
    >>> conda create --name nombre_env
    
2.1 Crear un entorno virtual con una version de Python especifica:

    >>> conda create --name nombre_env python=3.7
    >>> conda create -n nombre_env python=3.6

3. En tu entorno virtual se instala ipykernel:
    
    >>>python -m pip install ipykernel
    
4. Finalmente ingresamos tu entorno virtual mediante el siguiente comando:

    >>> python -m ipykernel install --user --name (nombre de tu entorno virutal) --display-name "Alias de tu entorno virtual, puede ser el mismo nombre de tu entorno"
 
 Deberia aparecerte el siguiente mensaje si todo salio correcto:
 
 Installed kernelspec (nombre de tu entorno virtual) in C:\User\user\appdata\roaming\jupyter\kernels\(nombre de tu entorno virtual)
 

*INSTALACION FORZADA DE LIBRERIAS MEDIANTE PIP

>>> pip install --upgrade --force-reinstall (libreria)

Si se desea ejecutar jupyter en una direccion o ruta ayuda el siguiente codigo:

>>> jupyter notebook --notebook-dir=C:/Usuario/Carpeta/Subcarpeta/NoteBooks

La ruta puede ir sin comillas dobles ("") o simples ('') tal como se observa en el ejemplo de arriba

#
Espero sea de Ayuda

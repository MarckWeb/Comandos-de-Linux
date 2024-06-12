- __mkdir (Make Directory)__ -. Crea un nuevo directorio.

```bash
mkdir nombre_del_directorio
```

Para crear directorios padres si no existen:

```bash
mkdir -p directorio_padre/diretorio_hijo/
```

```bash
# Ejemplo
┌──(marck㉿kali)-[~]
└─$ mkdir apuntes_linux
-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
lo que indica que se ha creado el directorio correctamente.


┌──(marck㉿kali)-[~]
└─$ mkdir -p directorio_padre/directorio_hijo/archivo.txt
-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
indicando que se han creado el directorio, 
el directorio padre, el hijo y el archivo correctamente.
```

- __rmdir (Remove Directory)__ -. Elimina un directorio vacío.

```bash
rmdir nombre_del_directorio
```

```bash
# Ejemplo
┌──(marck㉿kali)-[~]
└─$ rmdir apuntes_linux
-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
indicando que se elimino el directorio. 
```

- __rm (Remove)__ -. Elimina archivos o directorios.

```bash
rm nombre_del_archivo
```
Para eliminar un directorio y su contenido de forma recursiva:

```bash
rm -r nombre_del_directorio
```

```bash
# Ejemplo
┌──(marck㉿kali)-[~]
└─$ rm archivo.py 
-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
indicando que se elimino el archivo.   

♦ Eliminar directorio con contenido:                                          
┌──(marck㉿kali)-[~]
└─$ rm -r  directorio_padre 

-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
indicando que se elimino el directorio mas sus 
archivos que contenia.   
```

- __touch__ -. Crea un archivo vacío o actualiza la fecha de modificación de un archivo existente..

```bash
touch nombre_del_archivo
```

```bash
# Ejemplo
┌──(marck㉿kali)-[~]
└─$ touch archivo_nuevo.txt

-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
indicando que se creo el nuevo archivo. 
```
- __cat__ -. Muestra el contenido de un archivo.

```bash
cat nombre_del_archivo
```

```bash
# ejemplo de salida
┌──(marck㉿kali)-[~]
└─$ cat archivo.txt

-----------------Salida--------------------
Contenido del archivo...
```
 
- __cp (Copy)__ -. Copia archivos o directorios. No necesitas estar en una posición específica dentro del directorio, pero debes especificar las rutas correctas para el archivo o directorio de origen y de destino. 

```bash
cp directorio_origen directorio_destino
```
```bash
# Ejemplo
┌──(usuario㉿kali)-[~]
└─$ cp archivo.py Documentos/

-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
indicando que se ha hecho una copia del archivo al 
directorio indicado 
```
Por ejemplo, si estás en /home/usuario/documentos y quieres hacer una copia archivo.txt a archivo_copia.txt en el mismo directorio:

```bash
cp archivo.txt archivo_copia.txt
```

```bash
# Ejemplo
┌──(usuario㉿kali)-[~]
└─$ cp archivo.py archivo_copia.py

-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
indicando que se ha hecho una copia del archivo
en el mismo directorio. 
```

Si el archivo de origen está en un directorio diferente, necesitas proporcionar la ruta completa o relativa:
Por ejemplo, si quieres copiar archivo.txt desde /home/usuario/downloads a /home/usuario/documentos:

```bash
cp /home/usuario/downloads/archivo.txt /home/usuario/documentos/archivo.txt 
```

Para copiar un directorio y su contenido: y se siguen los mismo pasos anteriores para copiar a otro directorio

```bash
cp -r directorio_origen directorio_destino
```
```bash
# Ejemplo
┌──(marck㉿kali)-[~]
└─$ cp /home/marck/usernames2.txt /home/marck/Desktop/usernames2.txt

-----------------Salida--------------------
Si no hay errores, no se mostrará ninguna salida, 
indicando que se ha hecho una copia del archivo
en al otro directorio. 
```
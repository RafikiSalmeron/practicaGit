1. Clona el repositorio 
    ```
    git clone https://github.com/DavidBernalGonzalez/practicaGit.git
    ```  
    ```
    git remote set-url origin https://github.com/RafikiSalmeron/practicaGit.git  
    ```
    ```
    cd practicaGit/
    ```
2. Visualiza las distintas ramas  
    ```
    git branch -a
    ```
3. Dentro del repositorio hay una carpeta llamada practica01, la encontrarás en la rama “practica01”. Sitúate en rama "practica01" para ver la carpeta practica01.  
    ```
    git checkout practica01
    ```
4. Sitúate en el directorio practica1 y edita los archivos a tu gusto. Una vez editados los ficheros, haz un git status para ver que ha pasado con los ficheros.
    ```
    cd practica01/
    ```
    ```
    git status
    ```
5. Crea una rama nueva, llámala practica1_APELLIDOS_NOMBRE
    ```
    git branch practica1_SALMERON_MARTOS_RAFAEL
    ```
6. Muévete a la rama que has creado (practica1_APELLIDOS_NOMBRE)
    ```
    git checkout practica1_SALMERON_MARTOS_RAFAEL
    ```
7. En el directorio raíz, crea el fichero practica1_APELLIDOS_NOMBRE.txt y cualquier cosa en su interior. Y haz un commit de los cambios.
    ```
    cd ..
    ```
    ```
    touch practica1_SALMERON_MARTOS_RAFAEL.txt
    ```
    ```
    git add .
    ```
    ```
    git commit -m "Practica creada en raiz"
    ```
8. Vuelve a hacer otro commit revirtiendo los cambios (haciendo un nuevo commit) y sube los cambios al repositorio remoto:
    ```
    git add .
    ```
    ```
    git commit -m "Fichero con mi nombre"
    ```
    ```
    git push --set-upstream origin practica1_SALMERON_MARTOS_RAFAEL
    ```
9. Vuelve a la rama “practica1”.
    ```
    git checkout practica01
    ```
10. Haz un merge de tu rama con practica1
    ```
    git merge practica1_SALMERON_MARTOS_RAFAEL -m "Merge de mi rama"
    ```
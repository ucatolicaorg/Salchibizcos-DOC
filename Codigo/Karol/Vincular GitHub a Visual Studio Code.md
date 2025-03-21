Vincular un repositorio de GitHub a Visual Studio Code
---
**Requerimientos**
- GitHub for desktop: https://desktop.github.com/download/
- Visual Studio Code

**Instrucciones**
- Abrir la cuenta de GitHub desde el escritorio
- Clonar el repositorio en GitHub for Desktop o desde el repositorio online dar click en _<> Code_'_, y _Open with GitHub Desktop_
- Realizar los cambios necesarios (Preferiblemente en tu propia carpeta para no afectar los otros, no es recomendable dos personas trabajando en la misma carpeta)
- Guardar los cambios o avances
    
    Se debe realizar desde la terminal, desde escritorio (Símbolo de sistema) o desde Visual Studio Code (Ctrl + Shift + ñ)
    - Agregar los archivos modificados al área de preparación

            git add .
    - Hacer un commit con un mensaje descriptivo 

            git commit -m "Descripción de los cambios"
    
        Recomendable que sea la fecha y hora o un conteo del commit

    - Subir los cambios al repositorio remoto

        **Primera vez**

            git push -u origin main
        
        Este comando se usa la primera vez que subes una rama al repositorio remoto. La opción -u (o --set-upstream) establece un upstream para que, en futuros git push y git pull, no tengas que especificar la rama manualmente.

        **Después de la primera vez**

        Una vez que ya configuraste el upstream con _-u_, puedes usar simplemente

            git push origin main
        
        o incluso solo

            git push
        
        Si la rama principal no es _main_, usa _git branch_ para verificar el nombre y reemplázalo en el comando

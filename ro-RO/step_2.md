## Crearea unui controler

Să începem prin crearea unui controler, care va fi folosit pentru a colecta puncte.

+ Deschideți proiectul "Catch the Dots" Scratch online la <a href="http://jumpto.cc/dots-go" target="_blank">jumpto.cc/dots-go</a> sau descarca-l de la <a href="http://jumpto.cc/dots-get" target="_blank">jumpto.cc/dots-get</a> și apoi deschideți dacă utilizați editorul offline.
    
    Ar trebui să vedeți un controler pentru personaj:
    
    ![captură de ecran](images/dots-controller.png)

+ Rotiți controlerul spre dreapta când apăsați tasta săgeată dreapta:
    
    ```blocks
        when flag clicked
        forever
            if <key [right arrow v] pressed?> then
                turn right (3) degrees
            end
        end
    ```

+ Testați-vă controlerul - ar trebui să se rotească spre dreapta.
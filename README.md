# Preparar o ambiente de trabalho
- É necessário um computador com o sistema operativo *windows*, *macos* ou *linux*.
- É necessário instalar o *visual studio code* [aqui](https://code.visualstudio.com).
- É necessário instalar, se já não estiver instalado, o *python* [aqui](https://www.python.org/downloads/).

# Preparar o visual studio code
- É necessário instalar a extensão do *python* para o *visual studio code* [aqui](https://marketplace.visualstudio.com/items?itemName=ms-python.python).
- criar uma pasta no disco com o nome ` programação ` ou ` pragramacao ` e dentro dessa pasta outra pasta com o nome de ` curso_python `, é aqui onde vamos trabalhar com *visual studio code*. **Nota:** podem ser outros nomes para as pastas.
- No *visual studio code* é necessário selecionar qual o interpretador de *python* a usar. Para isso vamos ao menu *View* e selecionamos o submenu *Command Palette*, vai aparecer um caixa com o símbolo > e o cursor a piscar. Escrevemos nessa caixa ` Python: Select Interpreter ` de seguida escolhemos a versão do python que queremos, no nosso caso pode ser a versão 3.8, mas outra versão acima de 3.0 pode ser.

<p align="center">  
    <b>Python: Select Interpreter</b>
</p>
<p align="center">
  <img src="imagens/python_interpreter.png" width="40%">
</p>

<p align="center">  
    <b>Versão do Python</b>
</p>
<p align="center">
  <img src="imagens/python_selection.png" width="40%">
</p>


# Contentores
###### Alternativa para quem não consegue instalar o python ou não sabe trabalhar com o python na linha de comandos do windows. ***Nota:*** também pode ser instalado por quem conseguiu concluir o processo anterior e quer aprender outras alternativas. Também é importante conseguir instalar o docker para que possamos todos usar os mesmos comandos, independentemente se conseguimos concluir com sucesso ou não o passo anterior.

## Docker
- IMPORTANTE: Docker Desktop requires Windows 10 Pro or Enterprise version 15063 to run.
- É necessário instalar a aplicação ***docker*** [aqui](https://www.docker.com/products/docker-desktop). Pode ser necessário fazer um registo, mas é grátis [aqui](https://docker.events.cube365.net/docker/dockercon/).
- Depois do ***docker*** instalado vamos testá-lo. Na linha de comandos (terminal ou cmd) escrever o seguinte comando: `docker --version `. Se correr tudo bem aparecerá algo do tipo: ```Docker version 19.03.5, build 633a0ea ```.
- Agora vamos fazer mais um teste. Na linha de comandos escrever: ` docker run hello-world `. Se correr tudo bem, entre outras coisas, aparecerá no terminal: ```Hello from Docker! ```.
- Vamos agora instalar o python na aplicação docker para podermos trabalhar. Para tal escrever o seguinte na linha de comandos: ` docker pull python `.
- Agora antes de podermos usar o ***docker*** e o ***python*** vamos configurar a pasta onde vamos trabalhar nas preferencias do docker. O docker quando foi instalado adicionou um icon à barra de menus. Clicamos nesse icon e aparece um menu onde vamos escolher preferencias. Aparecerá um janela como a imagem abaixo. Seguindo o esquema da janela da imagem carregamos no sinal **(+)** e vamos até à pasta que escolhemos para trabalhar (que de acordo com o que aqui foi dito é: ` progamação/curso_python `; se for no windows será do tipo: ` c:\programação\curso_python `; Se for linux será do tipo: ` /home/programação/curso_python ` e se for no mac será do tipo: ` /Users/rubenfernandes/programação/curso_python `).

<p align="center">  
    <b>Docker: preferências</b>
</p>
<p align="center">
  <img src="imagens/preferencias_docker.png" width="60%">
</p>

- Agora já podemos começar a usar o docker. Para podermos correr os programas que fazemos temos de entrar no contentor e escrever o comando para correr o nosso programa.

    - Para entrar no contertor e interagir com ele escrevemos na linha de comandos o código abaixo indicado. ***Nota:*** o caminho logo depois do parâmetro -v é o caminho para o nosso código no pc. Que no nosso caso depende do sistema operativo. Assim, cada um terá de ajustar. No caso do windows, e supondo que as pastas criadas foram as aqui sugeridas é: ` c:\programação\curso_python `. No meu caso é: ` /Users/rubenfernandes/programacao/curso_python `. No caso do linux é: ` /home/programacao/curso_python `.
    <p></p>
    
    ```
    docker run -w /curso_python --rm -it -v /Users/rubenfernandes/programacao/curso_python:/curso_python python /bin/bash 
    ```
    
    <p align="center">  
      <b>comando: docker run</b>
    </p>
    <p align="center">
      <img src="imagens/entrar_docker.png" width="100%">
    </p>
    
    <p align="center">  
      <b>dentro do docker</b>
    </p>
    <p align="center">
      <img src="imagens/no docker.png" width="100%">
    </p>
    
    - para sair escrevemos na linha de comando ` exit `.

<p align="center">
  <img src="imagens/sair docker.png" width="100%">
</p>

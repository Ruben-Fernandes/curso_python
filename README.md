# Preparar o ambiente de trabalho
- É necessário um computador com o sistema operativo *windows*, *macos* ou *linux*.
- É necessário instalar o *visual studio code* [aqui](https://code.visualstudio.com).
- É necessário instalar, se já não estiver instalado, o *python* [aqui](https://www.python.org/downloads/).

# Preparar o visual studio code
- É necessário instalar a extensão do *python* para o *visual studio code* [aqui](https://marketplace.visualstudio.com/items?itemName=ms-python.python).
- criar uma pasta no disco com o nome ***programação*** e dentro dessa pasta outra pasta com o nome de ***curso_python***, é aqui onde vamos trabalhar com *visual studio code*. **Nota:** podem ser outros nomes para as pastas.
- No *visual studio code* é necessário selecionar qual o interpretador de *python* a usar. Para isso vamos ao menu *View* e selecionamos o submenu *Command Palette*, vai aparecer um caixa com o símbolo > e o cursor a piscar. Escrevemos nessa caixa ***Python: Select Interpreter*** de seguida escolhemos a versão do python que queremos, no nosso caso pode ser a versão 3.8, mas outra versão acima de 3.0 pode ser.

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
###### Alternativa para quem não consegue instalar o python ou não sabe trabalhar com o python na linha de comandos do windows. **Nota:** também pode ser instalado por quem consegui concluir o processo anterior.

## Docker

- É necessário instalar a aplicação ***docker*** [aqui](https://www.docker.com/products/docker-desktop). Pode ser necessário fazer um registo, mas é grátis [aqui](https://docker.events.cube365.net/docker/dockercon/).
- Depois do ***docker*** instalado vamos testá-lo. Na linha de comandos (terminal ou cmd) escrever o seguinte comando: ***docker --version***. Se correr tudo bem aparecerá algo do tipo: ***Docker version 19.03.5, build 633a0ea***.
- Agora vamos fazer mais um teste. Na linha de comandos escrever: ***docker run hello-world***. Se correr tudo bem, entre outras coisas, aparecerá no terminal: ***Hello from Docker!***.
- Vamos agora instalar o python na aplicação docker para podermos trabalhar. Para tal escrever o seguinte na linha de comandos: ***docker pull python**

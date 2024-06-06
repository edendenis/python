<!-- LOGOTIPO DO PROJETO -->
<div style="display: flex; justify-content: center;">
   <a href="https://github.com/edendenis/python">
     <img src="figures/gold_edf_technology_logo_transparent_background_and_gold_name.png" alt="Logo" width="160" height="160">
   </a>
</div>

<h3 align="center">Configurar/instalar/usar o `Python 3.8` no `Linux Ubuntu`</h3>

<!-- <div style="display: flex; justify-content: center;">
  <a href="https://zenodo.org/doi/10.5281/zenodo.10668919">
    <img src="https://zenodo.org/badge/758237447.svg" alt="DOI">
  </a>
</div> -->

<p align="center">
 Neste documento estão contidos os principais comandos e configurações para configurar/instalar/usar o `Google Chrome` no `Linux Ubuntu`.
 <br />
 <a href="https://github.com/edendenis/python"><strong>Explore os documentos »</strong></a>
 <br />
 <br />
 <a href="https://github.com/edendenis/python">Ver demonstração</a>
 ·
 <a href="https://github.com/edendenis/python">Relatar bug</a>
 ·
 <a href="https://github.com/edendenis/python">Solicitar recurso</a>
</p>


# Configurar/instalar/usar o `Python 3.8` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar/usar o `Python 3.8` no `Linux Ubuntu`.

## _Abstract_

_In this document are contained the main commands and settings to set up/install the `Python 3.8` on `Linux Ubuntu`._


### Construído com

Esta seção deve listar todas as principais estruturas/bibliotecas usadas para inicializar seu projeto. Deixe quaisquer complementos/plugins para a seção de agradecimentos. Aqui estão alguns exemplos.

* [![Python 3.8](https://img.shields.io/badge/Python%203.8-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org/)
* [![Anaconda](https://img.shields.io/badge/Anaconda-44A833?style=flat-square&logo=anaconda&logoColor=white)](https://www.anaconda.com/)

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>


<!-- COMEÇANDO -->
### Começando

Este é um exemplo de como você pode dar instruções sobre como configurar seu projeto localmente.
Para obter uma cópia local instalada e funcionando, siga estas etapas simples de exemplo.

### Pré-requisitos

Este é um exemplo de como listar os itens necessários para usar o software e como instalá-los.
* Python 3.8
* Anaconda 24.1.0
* Git
* IDE para executar o arquivo `.ipynb` (PyCharm, Spyder, VS Code etc.)

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>


## Descrição [2]

### `Python`

O `Python` é uma linguagem de programação de alto nível, interpretada e multiparadigma, conhecida por sua simplicidade e legibilidade. Criada por Guido van Rossum e lançada em 1991, `Python` oferece uma sintaxe clara e concisa, tornando-a ideal para iniciantes e experientes. Sua ampla biblioteca padrão e vasta comunidade de desenvolvedores facilitam a criação de uma variedade de aplicativos, desde scripts simples até aplicativos web complexos, aprendizado de máquina e ciência de dados. `Python` é valorizado por sua portabilidade, interoperabilidade e escalabilidade, sendo uma escolha popular em muitas áreas da computação e além.

## 1. Como configurar/instalar/usar o `Python` no `Linux Ubuntu` [1]

Para configurar/instalar/usar o `Python` no `Linux Ubuntu`, você pode seguir estes passos:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.2 Remover pacotes `.deb` antigos ou duplicados do cache local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando: `sudo apt autoclean`

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando: `sudo apt autoremove -y`

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`: `sudo apt update`

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes: `sudo apt --fix-broken install`

    2.6 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando: `sudo apt clean` 
    
    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:  `sudo apt list --upgradable`

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`: `sudo apt full-upgrade -y`
    

3. Baixe a versão desejada do python em: <https://www.python.org/>


Para instalar um arquivo `.tar.xz` ou `.tgz`, você geralmente precisará descompactar o arquivo e, dependendo do conteúdo, compilar e instalar os programas ou bibliotecas. Vou detalhar os passos para ambas as extensões, considerando que você está utilizando um sistema baseado em Linux:

### 1.1 Para um arquivo `.tar.xz`:

1. Abra o `Terminal Emulator`.

2. **Descompacte o arquivo usando o comando `tar`:** `sudo tar -xf <arquivo>.tar.xz`

    Substitua `<arquivo>` pelo nome do seu arquivo.

3. **Navegue até o diretório descompactado:** `cd <nome_do_diretorio>`

    Substitua `<nome_do_diretorio>` pelo nome do diretório criado após a descompactação.

4. Leia qualquer arquivo de instrução como `README` ou `INSTALL` para entender o processo de instalação específico do software.

5. **Instalar o `make`**: O `make` pode ser instalado com o comando: `sudo apt install make -y`

6. **Instale o compilador C e outras ferramentas necessárias:**: `sudo apt install build-essential -y`

7. **Instalar o `gcc`**: `sudo apt install gcc -y`

8. **Verificar se o GCC está instalado**: Você pode verificar se o GCC foi instalado corretamente com o seguinte comando: `gcc --version`

    Se este comando retornar informações sobre a versão do GCC, significa que o compilador está instalado.

9. Geralmente, você seguirá os passos de configuração, compilação e instalação: `./configure --enable-optimizations  # antes era somente ./configure`

10. **Compile e instale o Python:** Após configurar, compile o código fonte e instale-o com os seguintes comandos:

    ```
    make -j 8  # Onde `8` é o número de núcleos que você deseja usar para a compilação
    sudo make altinstall 
    ```

    Usar `make altinstall` em vez de `make install` previne que esta versão do `Python` substitua a versão padrão do sistema.

11. **Verifique a instalação:** Após a instalação, verifique se o `Python` foi instalado corretamente com o comando: `python3.8 --version`

Se tudo correu bem, este comando deve retornar a versão do `Python` que você acabou de instalar.

Esses passos devem ajudá-lo a instalar o `Python 3.8.10` no seu sistema Linux. Note que as etapas específicas podem variar ligeiramente dependendo da sua distribuição `Linux`.


### 1.1 Adicionar o `Python` ao `$PATH` do `Linux Ubuntu`

O executável do `Python` pode não ser encontrado porque não foi adicionado ao seu `$PATH`. O `$PATH` é uma variável de ambiente que diz ao sistema onde procurar por programas executáveis. Quando você compila e instala o `Python` a partir do código fonte, geralmente ele é instalado em `/usr/local/bin`, a menos que você especifique um local diferente.

#### 1.1.1 Passos para resolver o problema
    
    1. Verifique se o `Python` está instalado em `/usr/local/bin`: Você pode verificar isso com o seguinte comando: `ls /usr/local/bin | grep python`

    Procure por algo como `python3.8` ou apenas `python` se você criou um link simbólico.

    2. Verifique a sua variável `$PATH`: `echo $PATH`

    Certifique-se de que `/usr/local/bin` está incluído. Se não estiver, você precisará adicionar esse diretório ao seu `$PATH`.
    
    3. Adicionar `/usr/local/bin` ao seu `$PATH`: Se `/usr/local/bin` não estiver no seu `$PATH`, você pode adicionar temporariamente com o comando: `export PATH=$PATH:/usr/local/bin`

    Para tornar essa mudança permanente, adicione a linha acima ao final do seu arquivo `~/.bashrc` ou `~/.profile` (dependendo do seu shell e configurações) e depois recarregue o arquivo com: `source ~/.bashrc`
    
    ou reinicie o terminal.
    
    4. Criar um link simbólico para `python`: Muitas distribuições já têm o comando `python` apontando para `python3`. Se o seu não tem e você instalou uma versão específica, como `python3.8`, você pode criar um link simbólico para `python`: `sudo ln -s /usr/local/bin/python3.8 /usr/local/bin/python`

    5. Verificar novamente: Após adicionar `/usr/local/bin` ao seu `$PATH` ou criar o link simbólico, tente novamente: `python --version`

    Se após seguir esses passos o `Python` ainda não for reconhecido, verifique novamente se você seguiu todos os passos corretamente e se o `Python` foi de fato instalado em `/usr/local/bin`. Se o problema persistir, pode valer a pena verificar novamente o processo de instalação ou o config.log para eventuais erros durante a instalação.

## 2. Código completo para configurar/instalar/usar

Para configurar/instalar/usar o `Python` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando: `Ctrl + Alt + T`

2. Digite o seguinte comando e pressione `Enter`:

    ```
    NÂO há.
    ```


<!-- LICENÇA -->
## Licença

Distribuído sob a licença MIT. Consulte `LICENSE.txt` para obter mais informações.

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>

<!-- ROTEIRO -->
## Roteiro

- [x] Adicionar registro de alterações
- [x] Adicionar links de volta ao topo
- [x] Adicionar modelos adicionais com exemplos
- [x] Suporte multilíngue
     - [ ] Espanhol
     - [ ] Inglês
     - [ ] Português
     - [x] Português brasileiro 

Consulte os [problemas abertos](https://github.com/edendenis/google_chrome/issues) para obter uma lista completa dos recursos propostos (e problemas conhecidos).

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>


<!-- CONTRIBUIÇÔES -->
## Contribuições

As contribuições são o que tornam a comunidade de código aberto um lugar incrível para aprender, inspirar e criar. Qualquer contribuição que você fizer será **muito apreciada**.

Se você tiver uma sugestão que possa melhorar isso, bifurque o repositório e crie uma solicitação `pull`. Você também pode simplesmente abrir um problema com a tag “aprimoramento”.
Não se esqueça de dar uma estrela ao projeto! Obrigado novamente!

1. Bifurque o projeto
2. Crie sua ramificação de recursos (`git checkout -b feature/AmazingFeature`)
3. Confirme suas alterações (`git commit -m 'Add some AmazingFeature'`)
4. Envie para a filial (`git push origin feature/AmazingFeature`)
5. Abra uma solicitação pull

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>


<!-- ACKNOWLEDGMENTS -->
## Agradecimentos

* [Best README Template](https://github.com/othneildrew/Best-README-Template?tab=readme-ov-file)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Malven's Flexbox Cheatsheet](https://flexbox.malven.co/)
* [Malven's Grid Cheatsheet](https://grid.malven.co/)
* [Img Shields](https://shields.io)
* [GitHub Pages](https://pages.github.com)
* [Font Awesome](https://fontawesome.com)
* [React Icons](https://react-icons.github.io/react-icons/search)

<p align="right">(<a href="#readme-top">voltar ao topo</a>)</p>


## Referências

[3] OPENAI. ***Instalar arquivos tar.xz/tgz..*** Disponível em: <https://chat.openai.com/c/0ce53031-41c5-4185-93d7-0156e1d2cb2a> (texto adaptado). Acessado em: 13/03/2024 13:47.

[2] OPENAI. ***Vs code: editor popular.*** Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado). Acessado em: 13/03/2024 13:48.



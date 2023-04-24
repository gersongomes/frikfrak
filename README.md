# frikfrak
the best frik frak game youve ever seen in your life.

##SHADOW CALL
## Visao Geral dos atores e cenarios usados no jogo

PS:não coloquei exemlos de imagens para evitar que o relatorio fique demasiado extenso.
  
Para o jogo, resolvi usar 3 atores para o player 1 no caso Xa, Xb e Xc e 3 atores para o player 2 que seriam Od, Oe e Of.
O tabuleiro por sua vez é constituído por 9 quadrados, em que cada uma delas é um ator que irá interagir quando ele for clicado, se estivermos no modo gráfico.
Existem alguns botões de açpão também que quando clicados realizam ações específicas, como o enter, que ao ser clicado nos enviará para o menu principal, o quit, que para o jogo por completo, o sound, que ao ser clicado nos envia para o cenario de som onde podemos encontrar 3 botõens, um sinal - para diminuir o volume do som, um sinal + para aumentar o volume do som e uma seta para voltar ao menu principal.
No menu principal, ao clicar no botao play, vc será redirecionado ao cenário onde você pode escolher o modo que você deseja jogar, no modo aventura ou Humano-IA(ainda não está disponível para essa versão), no modo Multiplayer Versus ou Humano-Humano(Para a próxima versão será possível fazer a escolha de personagens, e estas aparecerão como player 1, que será o sobrevivente, e o player 2 que vem como assassino como default) e por ultimo o modo Multiplayer CO-OP,onde será aberto um tabuleiro maior, de 9 peças, onde você e o seu companhei podem jogam contra um IA(ainda não está disponível para essa versão também).
Ao ecolher o modo Multiplayer Versus, que é a unica opção disponível para essa versão, você será redirecionado para um cenário onde você vai escolher o tipo de jogabilidade que vc quer para o jogo, no caso o Modo gráfico ou o Modo Consola.

Ao escolher o modo que você deseja o jogo começa, onde na tela se encontra o botão de menu, ao ser clicado significa que vc desitiu do jogo atual e quer recomeçar, o tabuleiro, as 6 peças do lado do tabulerio, onde, se você estiver no modo gráfico, é só dar um clik na peça e um clik aonde você quer que ela vá, se você estiver no modo consola, é só digitar a letra da peça, e o numero do lugar aonde você quer que ela vá, por exemplo: a7, a peça Xa(todas as peças serão identificadas visualmente) irá para a posição 7(a numeração do tabuleiro será disponibilizado no botão quando você for escolher o modo consola ou gráfico, tem um mini tutorial na imagem do botão).

Quando o player 1(que representa o sobrevivente) vencer, seremeos enviados ao cenário de vencedor, onde além do titulo dizendo quem é o vencedor, teremos dois botões, o restart, que ao ser clicado nos enviará ao menu principal, reiniciando assim o jogo, e o quit que ira parar o jogo por completo.

## Codigos do jogo
  ##Primeiro cenário e Atores
   
    O primeiro cenário possui um unico ator, no caso, o botão enter, os códigos desse botão são basicamente, ao ser clicado na bandeira ela deve ir para a posiçao x e     y previamente determinado, se o cenario for o primeiro cenário ele deve aparecer, se não ele deve se esconder. Equanto ela estiver tocando o mouse, ela aumentar de     tamanho e luminozidade até certo ponto e se não estiver a tocar no mouse ela volta ao normal.
   
    Ao ser clicado,ela emite uma mensagem ¨clik¨ e ¨enter¨. Uma mensagem é basicamente o mesmo que uma variável, porém é mais volátil e prático. 
    Ao receber as mensagens, será reproduzido o som do ¨clik¨ do botão e o cenário será mudada para o menu principal.
    
  ## Menu Principal e Atores
    No menu principal temos 3 atores, o play, o sound e o quit.
    Ambos os botões têm os mesmos codigos de luminozidade e tamanho anteriormente,a posição x e y especifica quando a bandeira for clicada, se estiver no cenario menu     principal eles aparecem, se nao eles escondem e o som ao emitir a mensagem clik. Porém eles se diferem na mensagem que envião ao serem clicados, o botão quit ao       ser clicado emite uma mensagem para parar tudo, ao receber essa mensagem o jogo trava. O botão sound ao ser clicado emite uma mensagem que ao ser recebido nos         mudará para o cenário de som, onde temos os botões de -, + e uma seta para voltar ao menu principal. Todos os botões têm os mesmo codigos de estilo que os do menu     principal, porém os sinai - e + nao emitem a mensagem de clik. 
    O botão - ao ser clicado emite uma mensagem de volume down para abaixar o volume, e o sinal + faz o exato oposto.
    A seta, ao ser clicada emite a mensagem ¨menu¨ que nos enviará ao menu principal e a mensagem ¨clik¨.
    No menu principal, além dos codigos anteriormente mencionados, o botão play ainda dispõe de uma mensagem ao ser clicado. Ao ser clicado ele emite uma mensagem que     nos enviará à pagina para escolher o modo que pretendemos jogar, os modos anteriormente mencionados.
    Ao clicar no primeiro modo Adventure, o ator ¨Adventure¨ mostrará uma mensagem na tela dizendo que essa opção não está disponível para essa versão do Shadow Call,     e mudará a variavel ¨modes¨, que determina o modo em que estamos para 1, essa variavel é inutil para essa versão.
    Ao Clicar no terceiro, modo Mulriplayer Co-OP, acontecerá exatamente o mesmo que o primeiro.
    E por fim, ao clicar no segundo, modo Multiplayer Versus, será emitido uma mensagem que nos enviará ao cenário seguinte onde escolheremos a jogabilidade, no caso       consola ou gráfica.
    É digno de nota que todos os botões possuem os mesmos efeitos sonoros que os outros.

  ##Cenario de ecolha de Jogabilidade e Atores
  
   Neste cenário encontra-se dois atores, um para escolher o modo gráfico e outro para escolher o modo consola, ao escolher o modo gráfico a variável ¨Modo Grafico¨       será mudado para 1, ativando assim o modo gráfico e será emitido uma mensagem de inicio do jogo, ao escolher o modo consola a variável ¨Modo gráfico¨ será alterada     para 0, mostrando assim que não estamos mais no modo gráfico, e só temos duas opções, se não é um logicamente é o outro, e também, do mesmo modo, será emitida uma     mensagem de início do jogo.
  
  ##Campo de jogo
  
    Neste cenário temoos:
      
      ## Botão de Menu
        Possui todos os codigos para os efeitos visuais e sonoros semelhante aos outros, e ao ser clicado emitirá a mensagem ¨enter¨ que nos enviará ao menu principal,         reiniciando assim o jogo.
        
      ## Peças
         O player atual é escolhido por meio de uma variável chamada ¨currentplayer¨, essa variavel é alterada inicialmente para 1, no começo do jogo, após a primeira          jogada do player 1 ela será incrementada(+1), de seguida após a jogada do player 2 ela será decrementada(-1) e assim sucessivamente.
      
          O jogador X pode ser excolhide de duas formas:
          -No modo gráfico: Ao ser clicado, ela mudará o valor da variavel ¨jogX¨ que representa literamente Jogador X, para 1 e os outros JogX1 e JogX2 para 0, isso               se as variáveis, Modo gráfico e currentplayer estiverem em 1.
        
          -No modo Consola: ao ser clicado a letra a ela fará exatamente o mesmo que no modo gráfico.
        
       Existe uma outra variável que definirá o numero da posição em que o x se encontra, se X for igual a 0 ele encontra-se do lado do tabuleiro, como no principio do         jogo, se X for igual a 5 ela vai para a posição x e y estipulada no codigo que representa exatamente a posição 5 do tabuleiro.
      
      
       Para as outras duas peças do Player 1 é exatamente o mesmo excepto pelo nome das variáveis que ao envés de ser X agora serão X1 ou X2.
      
       O mesmo vale para o player 2 é exatamente o mesmo com a exceção de que passam a ser O, O1 e O2.
      
      ## Tabuleiro
        Cada quadrado do tabuleiro é um ator, de 1 a 9. Ao ser clicado o é executado o código de que se nao for verdade que este espaço do do tabuleiro ela deve seguir         à proxima condiçao, se nao deve exibir uma mensagem na tela de que a area esta ocupada,se sim deve seguir à condição se modo gráfico for 1 ela deve seguir para         a proxima condiçao para garantir que o curentplayer é 1 ou dois, verificado o current player, a seguir vai verificar que peça foi escolhida JogX, Jog O1,...           ,de seguida vem a condição das unicas posições que podem jogar nesse quadrado, no caso apenas dos quadrados vizinhos na horizontal e vertical, e no caso do             bloco 5, na diagonal. se todas essas condições forem atendida ela mudará o valor de X, X1, X2, O, O1 ou O2 para o valor do numero do quadrado que segundo o             codigo introduzido nas peças ela irá para a respetiva posição. Ainda no mesmo código, ao mover-se entre os blocos, linha 1,2,3 coluna 1,2,3 e diagonal 1 e 2           (referente ao X) e as mesmas variáveis com a lentra O no meio ex Diagonal O1(referente ao O), essa variáveis incrementam(+1) ou decrementam(-1) conforme a             posição selecionada, fazendo assim com que o numero de cada uma seja o numero de elementos do mesmo player em tal direção. EX: linha1 = 2 diagonal 1= 1                 diagonal 2= 1 coluna1=1 coluna3=1 significa que temos duas peças do player 1 na mesma linha, linha 1, essas peças se encontram na coluna 1 e coluna 3, o que           quer dizer que elas se encontram na posição 1 e 3 pois além da linha e colunas, as diagonais também estão a 1.
        A mesma lógica se repete para todos os blocos do tabuleiro.
        Quando as variviáveis linha 1, linha 2, linha 3, coluna 1, coluna 2 , coluna 3, diagonal 1 ou diagonal 2 forem = 3 a variável vencedor será alterado para 1,           mostrando assim que o player 1 venceu e o cenário será mudado para o cenario de vencedor do player 1 ou X, nesse cenário temos dois botõ com exatamente as             mesmas caracteristicas sonoras e visuais que os outros botões do menu primmcipal, porém o Restart ao ser clicado emitirá a mensagem ¨enter¨ que reiniciará o           jogo, e o quit que ao ser clicadao irá parar tudo, neutralizando assim o jogo. O mesmo acontece se as mesmas variaveis(versão O, ex: Linha O1) forem igual a 3,         porem quando as variaveis do O forem igual a 3, seremos redirecionados ao cenário Game Over com os mesmos botões de Restart e Quit que o cenário Vencedor               anteriormente explicado.
        
     ##Código nos cenários

       Os códigos do cenário servem basicamente para alterar de cenario conforme a mensagem, ou conforme o valor da variavel, para mudar de som conforme os mesmos, e          para zerar e econder todas as variáveis quando a bandeira for clicada e quando receber a mensagem enter para poder zerar o jogo.



//Algumas atualizações para a próxima versão seriam os o menu, durante o jogo que terá os botões quit e restart, a opção para aumentar e diminuir o volume, a opção para escolher musicas de fundo. A escolha de avatares subreviventes e o seu skin, os skins do assassino, a história inicial de como tudo começou, incluido narração(em inglês) e trilha sonora, um video macabro do assassino em ação e as opções Multiplayer CO-OP e Adventure mode. Ansiosos para a próxima versão? Pois é, Eu Também.//
        
      
     
  
  



    
    

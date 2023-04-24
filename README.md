# frikfrak
the best frik frak game youve ever seen in your life.

##SHADOW CALL
## Visao Geral dos atores e cenarios usados no jogo

PS:não coloquei exemlos de imagens para evitar que o relatorio fique demasiado extenso.
  
Para o jogo, resolvi usar 3 atores para o player 1 no caso Xa, Xb e Xc e 3 atores para o player 2 que seriam Od, Oe e Of.
O tabuleiro por sua vez é constituído por 9 quadrados, em que cada uma delas é um ator que irá interagir quando ele for clicado (se estivermos no modo gráfico).
Existem alguns botões de ação também que quando clicados realizam ações específicas, como o enter, que ao ser clicado nos enviará para o menu principal, o quit, que pára o jogo por completo, o sound, que ao ser clicado nos envia para o cenário de som onde podemos encontrar 3 botões, um sinal - para diminuir o volume do som, um sinal + para aumentar o volume do som e uma seta para voltar ao menu principal.
No menu principal, ao clicar no botão play, você será redirecionado ao cenário onde você pode escolher o modo em que você deseja jogar: no modo aventura ou Humano-IA(ainda não está disponível para essa versão), no modo Multiplayer Versus ou Humano-Humano(Para a próxima versão será possível fazer a escolha de personagens, e estas aparecerão como player 1, que será o sobrevivente, e o player 2 que vem como assassino por default) e por último o modo Multiplayer CO-OP,onde será aberto um tabuleiro maior, de 9 peças do player 1, 9 linhas e 9 colunas, onde você e o seu companheiro podem jogar contra um IA(ainda não está disponível para essa versão também).
Ao escolher o modo Multiplayer Versus, que é a única opção disponível para essa versão, você será redirecionado para um cenário onde você vai escolher o tipo de jogabilidade que você quer para o jogo, no caso o Modo gráfico ou o Modo Consola.

Ao escolher o modo que você deseja o jogo começa, onde na tela se encontra o botão de menu, ao ser clicado significa que você desistiu do jogo atual e quer recomeçar, o tabuleiro, as 6 peças do lado do tabulerio, onde, se você estiver no modo gráfico, é só dar um clik na peça e um clik aonde você quer que ela vá, se você estiver no modo consola, é só digitar a letra da peça, e o numero do lugar aonde você quer que ela vá, por exemplo: a7, a peça Xa(todas as peças serão identificadas visualmente) irá para a posição 7(a numeração do tabuleiro será disponibilizado no botão quando você for escolher o modo consola ou gráfico, tem um mini tutorial na imagem do botão).

Quando o player 1(que representa o sobrevivente) vencer, seremeos enviados ao cenário de vencedor, onde além do título dizendo quem é o vencedor, teremos dois botões, o restart, que ao ser clicado nos enviará ao menu principal, reiniciando assim o jogo, e o quit que irá parar o jogo por completo.

## Códigos do jogo
  ##Primeiro cenário e Atores
   
    O primeiro cenário possui um único ator, no caso, o botão enter. Os códigos desse botão são basicamente, ao ser clicado na bandeira ela deve ir para a posiçao x e     y previamente determinados, se o cenário for o primeiro cenário ele deve aparecer, se não ele deve se esconder. Equanto ela estiver tocando o mouse, ela deve           aumentar de tamanho e luminozidade até certo ponto, e se não estiver a tocar no mouse ela volta ao normal.
   
    Ao ser clicado, ela emite uma mensagem ¨clik¨ e ¨enter¨. Uma mensagem é basicamente o mesmo que uma variável, porém é mais volátil e prático. 
    Ao receber as mensagens, será reproduzido o som do ¨clik¨ do botão e o cenário será mudado para o menu principal.
    
  ## Menu Principal e Atores
    No menu principal temos 3 atores, o play, o sound e o quit.
    Ambos os botões têm os mesmos códigos de luminozidade e tamanho anteriormente mencionados, a posição x e y específica,... quando a bandeira for clicada, se estiver     no cenário menu principal eles aparecem, se não eles se escondem e o som ao emitir a mensagem clik. Porém eles se diferem na mensagem que enviam ao serem clicados,     o botão quit, ao ser clicado, emite uma mensagem para parar tudo, ao receber essa mensagem o jogo trava. O botão sound ao ser clicado emite uma mensagem que ao ser     recebida nos mudará para o cenário de som, onde temos os botões de -, + e uma seta para voltar ao menu principal. Todos os botões têm os mesmo códigos de estilo       que os do menu principal, porém os sinais - e + não emitem a mensagem de clik. 
    O botão - ao ser clicado emite uma mensagem de volume down para abaixar o volume, e o sinal + faz o exato oposto.
    A seta, ao ser clicada emite a mensagem ¨menu¨, que nos enviará ao menu principal, juntamente com a mensagem ¨clik¨.
    No menu principal, além dos códigos anteriormente mencionados, o botão play ainda dispõe de uma mensagem ao ser clicado. Ao ser clicado ele emite uma mensagem que     nos enviará à pagina para escolher o modo que pretendemos jogar, os modos anteriormente mencionados.
    Ao clicar no primeiro, modo Adventure, o ator ¨Adventure¨ mostrará uma mensagem na tela dizendo que essa opção não está disponível para essa versão do Shadow Call,     e mudará a variável ¨modes¨, que determina o modo em que estamos para 1, essa variável é inutil para essa versão.
    Ao Clicar no terceiro, modo Mulriplayer CO-OP, acontecerá exatamente o mesmo que o primeiro.
    E por fim, ao clicar no segundo, modo Multiplayer Versus, será emitido uma mensagem que nos enviará ao cenário seguinte onde escolheremos a jogabilidade, no caso       consola ou gráfica.
    Também há um botão, uma seta, que ao ser clicado emitirá a mensagem menu e nos enviará para o menu principal, ela possui todas as caracteristicas que a seta           encontrada no cenário de som.
    É digno de nota que todos os botões possuem os mesmos efeitos sonoros e visuais que os outros anteriormente mencionados. 

  ##Cenário de escolha de Jogabilidade e Atores
  
   Neste cenário encontra-se dois atores, um para escolher o modo gráfico e outro para escolher o modo consola, ao escolher o modo gráfico a variável ¨Modo Gráfico¨       será mudada para 1, ativando assim o modo gráfico e será emitido uma mensagem de início do jogo, ao escolher o modo consola a variável ¨Modo gráfico¨ será alterada     para 0, mostrando assim que não estamos mais no modo gráfico, e só temos duas opções, se não é um logicamente é o outro, e também, do mesmo modo, será emitida uma     mensagem de início do jogo.
  
  ##Campo de jogo
  
    Neste cenário temoos:
      
      ## Botão de Menu
        Possui todos os códigos para os efeitos visuais e sonoros semelhante aos outros, e ao ser clicado emitirá a mensagem ¨enter¨ que nos enviará ao menu principal,         reiniciando assim o jogo.
        
      ## Peças
         O player atual é escolhido por meio de uma variável chamada ¨currentplayer¨, essa variável é alterada inicialmente para 1 no começo do jogo, após a primeira          jogada do player 1 ela será incrementada(+1), de seguida após a jogada do player 2 ela será decrementada(-1) e assim sucessivamente.
      
          O jogador X pode ser excolhido de duas formas:
          -No modo gráfico: Ao ser clicado, ela mudará o valor da variável ¨jogX¨ que representa literamente Jogador X, para 1 e os outros JogX1 e JogX2 para 0. Isso              se as variáveis, Modo gráfico e currentplayer estiverem em 1.
        
          -No modo Consola: ao ser clicado a letra a ela fará exatamente o mesmo que no modo gráfico.
        
       Existe uma outra variável que definirá o numero da posição em que o x se encontra, se X for igual a 0 ele encontra-se do lado do tabuleiro, como no princípio do        jogo, se X for igual a 5 ela vai para a posição x e y estipulada no código que representa exatamente a posição 5 do tabuleiro.
      
      
       Para as outras duas peças do Player 1 é exatamente o mesmo, excepto pelo nome das variáveis que ao envés de ser X agora serão X1 ou X2.
      
       O mesmo vale para o player 2, é exatamente o mesmo com a exceção de que passam a ser O, O1 e O2.
      
      ## Tabuleiro
        Cada quadrado do tabuleiro é um ator, de 1 a 9. Ao ser clicado é executado o código de que se não for verdade que este espaço do tabuleiro está ocupado ela             deve seguir à proxima condiçao, se não, deve exibir uma mensagem na tela de que a área esta ocupada, se sim, deve seguir à condição se modo gráfico for 1. Se           modo gráfico for 1 ela deve seguir para a próxima condição para garantir que o curentplayer é 1 ou dois, verificado o current player, a seguir vai verificar           que peça foi escolhida JogX, Jog O1,...,de seguida vem a condição das únicas posições que podem jogar nesse quadrado, no caso apenas dos quadrados vizinhos na         horizontal e vertical, e no caso do bloco 5, na diagonal. se todas essas condições forem atendidas ela mudará o valor de X, X1, X2, O, O1 ou O2 para o valor do         número do quadrado que segundo o código introduzido nas peças ela irá para a respetiva posição. Ainda no mesmo código, ao mover-se entre os blocos, linha 1,2,3         coluna 1,2,3 e diagonal 1 e 2 (referente ao X) e as mesmas variáveis, com a lentra O no meio, ex Diagonal O1(referente ao O), essas variáveis incrementam(+1)           ou decrementam(-1) conforme a posição selecionada, fazendo assim com que o número de cada uma seja o número de elementos do mesmo player em tal direção. EX:           linha1 = 2 diagonal 1= 1 diagonal 2= 1 coluna1=1 coluna3=1 significa que temos duas peças do player 1 na mesma linha, linha 1, essas peças se encontram na             coluna 1 e coluna 3, o que quer dizer que elas se encontram na posição 1 e 3 pois além da linha e colunas, as diagonais também estão a 1.
        A mesma lógica se repete para todos os blocos do tabuleiro.
        Quando as variáveis linha 1, linha 2, linha 3, coluna 1, coluna 2 , coluna 3, diagonal 1 ou diagonal 2 forem = 3 a variável vencedor será alterado para 1,             mostrando assim que o player 1 venceu e o cenário será mudado para o cenário de vencedor do player 1 ou X, nesse cenário temos dois botões com exatamente as           mesmas características sonoras e visuais que os outros botões do menu primmcipal, porém o Restart ao ser clicado emitirá a mensagem ¨enter¨ que reiniciará o           jogo, e o quit que ao ser clicadao irá parar tudo, neutralizando assim o jogo. O mesmo acontece se as mesmas variáveis(versão O, ex: Linha O1) forem iguais a           3, porém quando as variáveis do O forem iguais a 3, seremos redirecionados ao cenário Game Over com os mesmos botões de Restart e Quit que o cenário Vencedor           anteriormente explicado.
        
     ##Código nos cenários

       Os códigos do cenário servem basicamente para alterar de cenário conforme a mensagem recebida, ou conforme o valor da variável, para mudar de som, conforme os          mesmos, para zerar e esconder todas as variáveis quando a bandeira for clicada e quando receber a mensagem enter para poder zerar o jogo.



//Algumas atualizações para a próxima versão seriam os botões no menu durante o jogo,serão adicionados os botões quit e restart, a opção para aumentar e diminuir o volume, e ainda no menu será adicionada a opção para escolher músicas de fundo. Será adicionado ao jogo a opção de escolha de avatares subreviventes e o seu skin, os skins do assassino, a história inicial de como tudo começou, incluindo a narração(em inglês) e trilha sonora, um vídeo macabro do assassino em ação e as opções Multiplayer CO-OP e Adventure mode passaram a funcionar. Ansiosos para a próxima versão? Pois é, Eu Também.//
        
      
     
  
  



    
    

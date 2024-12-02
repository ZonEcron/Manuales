# Placar ZonEcron
## Manual do Usuário

![Placar](../images/scoreboard/scoreborad.png)

1. [Introdução](#1-introdução)
   - [1.1 Especificações Técnicas](#11-especificações-técnicas)
   - [1.2 Principais Funcionalidades](#12-principais-funcionalidades)
   - [1.3 Componentes](#13-componentes)
   - [1.4 Montagem e Alimentação](#14-montagem-e-alimentação)
2. [Tela](#2-tela)
   - [2.1 Descrição Geral](#21-descrição-geral)
   - [2.2 Buzzer Integrado](#22-buzzer-integrado)
   - [2.3 Comunicação com o Ecossistema ZonEcron](#23-comunicação-com-o-ecossistema-zonecron)
   - [2.4 Modos de Operação na Tela](#24-modos-de-operação-na-tela)
     - [2.4.1 Modo Cronômetro](#241-modo-cronômetro)
     - [2.4.2 Modo Largada](#242-modo-largada)
     - [2.4.3 Modo Reconhecimento de Pista](#243-modo-reconhecimento-de-pista)
     - [2.4.4 Modo Jogos](#244-modo-jogos)
   - [2.5 Exibição de Mensagens](#25-exibição-de-mensagens)
     - [2.5.1 Mensagens Iniciais](#251-mensagens-iniciais)
     - [2.5.2 Bateria dos Sensores](#252-bateria-dos-sensores)
     - [2.5.3 Mensagens de Erro dos Sensores](#253-mensagens-de-erro-dos-sensores)
     - [2.5.4 Protetor de Tela](#254-protetor-de-tela)
     - [2.5.5 Mensagens Personalizadas](#255-mensagens-personalizadas)
   - [2.6 Limites](#26-limites)
3. [Servidor Web Embutido](#3-servidor-web-embutido)
   - [3.1 Descrição](#31-descrição)
   - [3.2 Redes WiFi](#32-redes-wifi)
     - [3.2.1 Conectar-se à Rede WiFi do Placar](#321-conectar-se-à-rede-wifi-do-placar)
     - [3.2.2 Alteração de Nome, Senha e Segurança](#322-alteração-de-nome-senha-e-segurança)
     - [3.2.3 Recuperação de Credenciais WiFi](#323-recuperação-de-credenciais-wifi)
     - [3.2.4 Conectar o Placar à uma Rede WiFi Externa](#324-conectar-o-placar-à-uma-rede-wifi-externa)
   - [3.3 Páginas Web](#33-páginas-web)
     - [3.3.1 Info](#331-info)
     - [3.3.2 Arquivos](#332-arquivos)
     - [3.3.3 WiFi](#333-wifi)
     - [3.3.4 Personalização](#334-personalização)
     - [3.3.5 Especiais](#335-especiais)
     - [3.3.6 Controle Remoto](#336-controle-remoto)
     - [3.3.7 Monitor](#337-monitor)
     - [3.3.8 Software](#338-software)
     - [3.3.9 Streaming](#339-streaming)
4. [Contato](#4-contato)

---

## 1. Introdução

### 1.1 Especificações Técnicas
- Tela LED 16x64 de alta luminosidade, com indicação de até 999,99s, faltas e recusas.
- Resolução máxima de 0,001s.
- Relógio principal com cristal de quartzo de 16 MHz.
- Desvio médio em 24 horas: ±20 ppm.
- Precisão do sistema com [ZonEcron Original](./original.md) (placar + células): de +0ms a +2ms.
- Precisão do sistema com [barras](./sensorBars.md) ou [invisível](./invisible.md) (placar + células): de +0ms a +6ms.
- Relógio em tempo real com TCXO ±2ppm para data e hora, com bateria substituível (duração de 10 anos).
- Conexão sem fio de 2,4 GHz com o ecossistema ZonEcron.
- Servidor web para até 4 usuários simultâneos.
- Memória para os últimos 3000 resultados, com data e hora.

---

### 1.2 Principais Funcionalidades
- Resolução em milissegundos para tempos inferiores a 10 segundos ou centésimos para tempos iguais ou superiores a 10 segundos.
- Indicadores na tela para faltas (máximo 9), recusas e eliminações.
- Alertas na tela para células fotoelétricas desalinhadas.
- Relógio em tempo real com data e hora.
- Medição da temperatura interna.
- Protetor de tela personalizável (adicione o nome do seu clube, por que não?).
- Controle via página web por smartphone/tablet/PC.
- Contagem regressiva para reconhecimento de pista, com pausa e configurável em passos de 1 minuto.
- Contagem regressiva de 15 segundos para largada em competições de alto nível.
- Compatível com gambler e snooker, incluindo sinal acústico.
- Passagens múltiplas por uma mesma célula em percursos complexos.
- Personalização das cores da interface web a qualquer momento.
- Mensagens personalizadas exibidas na tela por um tempo definido.

---

### 1.3 Componentes

O placar ZonEcron é composto por:
- Uma tela LED.
- Um tripé para sustentar a tela.
- Um cabo de alimentação padrão (230V 50Hz).
- Uma maleta para transporte prático.
- Dependendo do modelo, um buzzer/sirene interno ou externo.

**Nota Importante**: Certifique-se de ter um conjunto de células sem fio ZonEcron (original ou invisível) configuradas para se comunicar com a tela.

---

### 1.4 Montagem e Alimentação

Montar o placar ZonEcron é simples, mas aqui estão algumas dicas para garantir um resultado perfeito:

1. **Comece com o tripé**:
   - Abra as pernas e as estenda. Fixe-as com os parafusos borboleta e certifique-se de que o tripé esteja estável no chão.
   - Se não for necessário muita altura ou em dias ventosos, é melhor não estender a parte mais fina das pernas. Você também pode pendurar um peso no gancho inferior para maior estabilidade.
   - Se o terreno estiver irregular, ajuste as pernas e use os níveis de bolha no tripé para garantir que a cabeça esteja horizontal.
   - Certos movimentos do tripé foram intencionalmente limitados para melhorar a estabilidade e evitar quedas da tela. A cabeça do tripé pode girar apenas verticalmente para orientar a tela. Solte a rotação com o botão lateral.

2. **Fixe a tela ao tripé**:
   - Abra o parafuso borboleta na parte superior do tripé.
   - Encaixe a base quadrada da tela no suporte do tripé até que esteja bem fixa.
   - Aperte o parafuso borboleta e verifique se tudo está firmemente preso.

   **Atenção!** Não tente mover o tripé com a tela montada, pois isso pode danificar a base de fixação. Se precisar mudar de lugar, desmonte a tela primeiro e depois mova o tripé.

3. **Conecte o cabo de alimentação**:
   - Conecte o cabo primeiro na tela e depois a uma tomada.
   - Se usar uma extensão, deixe folga suficiente para evitar puxões em caso de tropeços.

4. **Ligue a tela**:
   - Pressione o interruptor na parte inferior da tela.
   - Se tudo estiver correto, o interruptor acenderá, e em menos de 2 segundos, as mensagens iniciais aparecerão na tela. Consulte a seção [2.5.1](#251-mensagens-iniciais) para mais detalhes.
   - Se o interruptor não acender, o problema provavelmente está no fusível integrado na tomada da tela. Abra o compartimento do fusível. Os placares novos sempre incluem um fusível de reposição dentro do mesmo compartimento, separado do fusível ativo. Substitua-o e tente novamente.

---

## 2 Tela

### 2.1 Descrição Geral

O placar ZonEcron foi projetado pensando em sua funcionalidade e durabilidade, mas também no conforto dos usuários. Aqui estão suas principais características:

- **Material**: A estrutura principal é feita de plástico, ideal para facilitar as comunicações por rádio. Os cantos possuem peças impressas em 3D com bordas arredondadas para evitar arestas vivas.
- **Manutenção**: Não é necessário realizar manutenção, exceto por uma limpeza externa com um pano úmido. Caso seja necessário acessar os componentes internos, os painéis frontal e traseiro podem ser removidos soltando os parafusos nas arestas e cantos. Os painéis são vedados com silicone para evitar a entrada de água da chuva. Essa vedação pode ser facilmente removida, mas será necessário aplicar novo silicone após abrir os painéis.
- **Ventilação**: Possui duas grades; uma delas contém um ventilador que extrai o ar quente do interior, enquanto a outra permite a entrada de ar fresco, evitando o superaquecimento dos componentes eletrônicos.
- **Parte Inferior**:
  - Tomada de alimentação com interruptor e fusível.
  - Acoplamento para montar a tela no tripé.
  - Nas versões com buzzer externo, encontrará o encaixe para fixá-lo e o conector correspondente.

---

### 2.2 Buzzer Externo/Interno

O buzzer emitirá sinais sonoros nos seguintes casos:
- **Fim do tempo de reconhecimento de pista**: Emitirá bipes curtos e intermitentes durante 8 segundos.
- **Modo games snooker**: Quando o tempo configurado para abertura for atingido, soará um bip pela duração configurada.
- **Modo games gambler**: Emitirá um bip ao final do tempo de abertura e outro ao final do tempo de fechamento, pela duração configurada.

**Atenção!** No caso do reconhecimento de pista, o buzzer sempre emitirá um som intermitente, como um despertador. Nos modos de jogos, o sinal enviado ao buzzer será contínuo, mas alguns modelos de buzzer possuem alternância integrada em sua eletrônica. Se desejar usar seu próprio buzzer, escolha um que funcione a 12V e consuma menos de 0,5A.

---

### 2.3 Comunicação com o Ecossistema ZonEcron

Todos os dispositivos do ecossistema ZonEcron vêm pré-configurados para se conectarem automaticamente entre si. Cada conjunto é codificado de forma única para evitar interferências entre áreas próximas. Por isso, os elementos de um conjunto comunicar-se-ão apenas entre si, não sendo possível, por exemplo, usar as células de um conjunto com o placar de outro.

A **ordem de inicialização** é indiferente; não importa se liga primeiro a tela, as células ou a mochila, tudo se conectará automaticamente. No entanto, recomenda-se que as células estejam ligadas e alinhadas antes de ligar a tela, para que os níveis de bateria sejam exibidos corretamente nas mensagens iniciais. Consulte a seção [2.5.1](#251-mensagens-iniciais) para mais detalhes.

Além disso, no [**ZonEcron Original**](./original.md), o tempo desaparecerá do pequeno display das células e será exibido o nível de bateria iluminando os 4 pontos do display da seguinte forma:
- 100% a 81% -> 4 pontos.
- 80% a 61% -> 3 pontos.
- 60% a 41% -> 2 pontos.
- 40% a 21% -> 1 ponto.
- 20% a 0% -> Display desligado.

---

### 2.4 Exibição dos Modos de Operação

#### 2.4.1 Modo Cronômetro

Este é o modo principal do placar ZonEcron, onde são exibidos:

- **Tempo**: Mostrado em tamanho grande.
- **Faltas e Recusas**: No lado direito, com um "F" e "R" antes dos números. Se "eliminado" for marcado, estes serão substituídos por "ELI", mas o cronômetro continuará funcionando para permitir correções ou registrar o tempo final do competidor.

![Correndo](../images/scoreboard/disp_running.jpg)
Display mostrando o tempo em execução.

**Exibição de tempo**:
- Quando o tempo está em execução: Um único decimal (atualizado a cada décimo de segundo).
- Quando o tempo está parado:
  - Milissegundos se for inferior a 10 segundos.
  - Centésimos se for igual ou superior a 10 segundos.

**Tempo máximo**: Ao ultrapassar 100 segundos (algo raro em um percurso normal de agility), os números se estreitam para exibir cinco dígitos no total. O tempo máximo exibido dessa forma é 999,99 segundos. O tempo total pode ser visualizado na web no [controle remoto](#336-controle-remoto).

---

#### 2.4.2 Modo Largada

Neste modo, a tela exibe uma contagem regressiva (segundos e décimos) previamente configurada, geralmente de 15 segundos.

O operador do cronômetro deve resetar o placar antes de cada competidor usando o [controle](#336-controle-remoto). Após o sinal do juiz, deve-se iniciar a contagem regressiva predefinida. Após isso:
- Se o cachorro interromper a célula durante a contagem regressiva, o cronômetro começará normalmente.
- Se a contagem regressiva chegar a 0 sem interrupção da célula, o cronômetro começará mesmo assim, ignorando a primeira passagem pela célula.

---

#### 2.4.3 Modo Reconhecimento de Pista

Este modo exibe uma contagem regressiva em minutos e segundos para o reconhecimento de pista. Por padrão, começa em 7 minutos, mas o tempo pode ser ajustado em passos de 1 minuto enquanto está pausado ou em execução:
- **Importante**: Neste modo, as células não têm efeito.
- **Ao finalizar a contagem regressiva**:
  - A mensagem "Tempo encerrado" será exibida.
  - Um bip intermitente será emitido por 8 segundos.

---

#### 2.4.4 Modo Games

Este modo é projetado para os jogos "snooker" e "gambler" do WAO (World Agility Open).

- **Snooker**: Cronometragem normal até que o tempo configurado seja alcançado, momento em que um sinal sonoro é emitido (a duração do sinal é configurável).
- **Gambler**:
  - O tempo permanece oculto com a mensagem "Tempus Fugit."
  - Quando o tempo de abertura é atingido, o primeiro sinal sonoro é emitido e o cronômetro volta a ser exibido normalmente.
  - Quando o tempo de fechamento é atingido, o segundo sinal sonoro é emitido (disponível apenas no modo gambler).
  - Em ambas as fases, se a célula for ativada antes do tempo definido, o tempo decorrido é exibido e o sinal sonoro não é emitido.
  - O segundo sinal pode ser desativado configurando o tempo de fechamento para 0 segundos.

Exemplo de gambler com tempo de abertura de 30s e tempo de fechamento de 12s:
- No início do percurso, o cronômetro está oculto e a mensagem "Tempus Fugit" é exibida na tela.
- Após 30 segundos de percurso, o primeiro sinal sonoro é emitido e o cronômetro volta a ser exibido normalmente.
- Após 42 segundos de percurso (12 segundos após o tempo de abertura), o segundo sinal sonoro é emitido.

**DICA**: Se o ambiente for barulhento, recomenda-se reforçar o sinal sonoro com um apito ou outro alerta manual.

---

## 2.5 Exibição de Mensagens

### 2.5.1 Mensagens Iniciais

Ao ligar o placar ZonEcron, quatro mensagens aparecerão na tela nos primeiros segundos:
1. Marca e modelo.
![initial](../images/scoreboard/disp_initial.jpeg)
2. Nome do clube (proteção de tela configurada).
![club](../images/scoreboard/disp_club.jpeg)
3. Hora e data do dispositivo.
![dateTime](../images/scoreboard/disp_dateTime.jpeg)
4. Nome da rede WiFi (própria ou externa) e endereço IP.
![WiFiIP](../images/scoreboard/disp_wifi_IP.jpeg)

Se qualquer célula detectar uma passagem durante essas mensagens, elas serão interrompidas e o cronômetro mudará automaticamente para a tela principal, começando a contagem. Por isso, se precisar verificar a hora, a data ou os dados da rede, é melhor ligar as células após visualizar todas as mensagens.

Preste atenção especial às mensagens 3 e 4: certifique-se de que a data e a hora estejam corretas [veja a seção 3.3.1](#331-info) e lembre-se da rede WiFi e do IP atribuído para gerenciar o servidor web [veja a seção 3.2](#32-conectar-ao-servidor).

---

### 2.5.2 Bateria dos Sensores

Ao ligar um par de células pela primeira vez, será exibida a porcentagem de bateria do receptor. A bateria do emissor também será exibida, caso este esteja corretamente alinhado com o receptor. Se desejar verificar o estado das baterias posteriormente sem desligar e religar tudo, isso pode ser feito pelo navegador [veja a seção 3.3.1](#331-info).

---

### 2.5.3 Mensagens de Erro dos Sensores

Se um sensor estiver desalinhado (exceto no modo de reconhecimento de pista), uma mensagem de alerta aparecerá indicando o sensor afetado. Se o cronômetro estiver em execução, ele continuará contando, mas não exibirá o tempo até que o sensor esteja devidamente alinhado.

---

### 2.5.4 Protetor de Tela

Se o cronômetro permanecer parado por mais de 2 minutos, o protetor de tela será ativado. Ele exibirá um texto deslizante alternado com a hora a cada 10 segundos. O texto exibido pode ser configurado [veja a seção 3.3.4](#334-personalização).

---

### 2.5.5 Mensagens Personalizadas

É possível configurar mensagens personalizadas em duas linhas, com até 10 caracteres por linha. A [seção 3.3.4](#334-personalização) explica como fazer isso. Essas mensagens só serão exibidas quando o cronômetro estiver parado e desaparecerão se um comando de reinício for enviado ou se alguma célula detectar uma passagem.

---

### 2.6 Limites

- O cronômetro pode medir mais de 1.000 segundos, mas a tela só exibe até 999,99 segundos. Para visualizar tempos superiores, use as páginas do [controle remoto](#336-controle-remoto) ou do [monitor](#337-monitor).
- O número máximo de faltas que o placar pode registrar é 9.
- O número máximo de recusas que pode registrar é 2. A partir da terceira recusa, será exibido como eliminado.

---

## 3 Servidor Web Embutido

### 3.1 Descrição

O placar ZonEcron inclui um servidor web interno que permite consultar, configurar e controlar o cronômetro a partir de qualquer dispositivo com conexão WiFi (smartphone, tablet, PC) sem necessidade de software adicional. Este servidor web pode se conectar a uma rede WiFi existente ou criar sua própria rede WiFi, eliminando a necessidade de conexão com a Internet.

---

### 3.2 Redes WiFi

#### 3.2.1 Conectar-se à Rede WiFi do Placar

Ao ligar o placar ZonEcron, se nenhuma outra rede tiver sido configurada (por exemplo, na primeira vez que for ligado), ele criará sua própria rede WiFi. Cada placar possui um nome de rede e uma senha únicos:

  - **Nome da rede**: ZonEcronXXXXXXXXXXXX
  - **Senha**: XXXXXXXXXXXX

Onde "XXXXXXXXXXXX" são números e letras maiúsculas de A a F. Portanto, ao procurar e encontrar a rede, você já saberá a senha... você e qualquer outra pessoa... então, assim que possível, altere a senha (e o nome da rede) conforme explicado na [seção 3.3.3](#333-wifi).
![WiFi Password](../images/scoreboard/phone_password.jpg)

Conecte-se a essa rede WiFi e, uma vez conectado:

1. Seu dispositivo pode alertá-lo de que a rede não tem conexão com a Internet (obviamente). Certifique-se de manter a conexão.
![Keep WiFi](../images/scoreboard/phone_keepWiFi.jpg)

2. **Nota Importante**: Alguns smartphones têm a função "WiFi+" (ou similar) que muda automaticamente para dados móveis se a rede WiFi não tiver Internet. Desative essa função para evitar problemas.
3. Abra um navegador da web (Chrome, Firefox, etc.) e digite o endereço `http://192.168.4.1`. Isso levará você à página inicial do placar, onde poderá ver seu status [veja a seção 3.3.1](#331-info).

---

#### 3.2.2 Alterar Nome, Senha e Segurança

Recomendamos alterar o nome da rede e a senha padrão seguindo as instruções da [seção 3.3.3](#333-wifi). Isso é importante para proteger seu dispositivo, assim como você faria com o roteador da sua casa.

Em competições oficiais, evite usar a rede WiFi gerada pelo placar. O servidor é simples, e sua única proteção é a senha da rede. Nestes casos, conecte o placar a uma rede WiFi robusta criada por um roteador adequado para ambientes movimentados ou, como último recurso, desative o WiFi.

---

#### 3.2.3 Recuperação de Credenciais WiFi

Esqueceu a senha da rede do seu placar ZonEcron? Não se preocupe, existe um procedimento simples para reconectar o placar:

1. Desligue o placar ZonEcron e as células.
2. No seu celular, crie um ponto de acesso WiFi com o nome "**Recuperame**" e a senha "**Admin1234**" (atenção às letras maiúsculas e minúsculas).
![Recovery WiFi](../images/scoreboard/phone_recover.jpg)

3. Ligue o placar ZonEcron.
4. Aguarde até que ele se conecte à rede "**Recuperame**" (do seu celular).
5. Na tela do placar ZonEcron, aparecerão o nome da rede ("Recuperame") e o endereço IP atribuído pelo seu celular.
6. Acesse esse endereço IP no navegador do seu celular para reconfigurar o nome e a senha da rede criada pelo placar ZonEcron conforme explicado na [seção 3.3.3](#333-wifi).

**Não consegue acessar?**:
- Se "Recuperame" não aparecer na tela, significa que o placar não se conectou à rede compartilhada pelo seu celular. Certifique-se de ter digitado corretamente o nome da rede e a senha (atenção às letras maiúsculas e minúsculas) e que seu celular está criando uma rede de 2,4 GHz. Redes mais recentes de 5 GHz não são compatíveis.
- Se a rede "Recuperame" aparecer, certifique-se de que é a sua rede e não uma gerada por outro celular na área.
- Se ainda assim não conseguir acessar, entre em contato conosco para suporte personalizado em [ZonEcron@gmail.com](mailto:ZonEcron@gmail.com?subject=Problemas%20de%20conexão).

---

#### 3.2.4 Conectar o Placar à uma Rede WiFi Externa

1. Ao ligar o placar, verifique a rede WiFi e o IP nos [mensagens iniciais](#251-mensagens-iniciais).
2. Conecte seu celular/tablet/PC à mesma rede WiFi. Se for a rede criada pelo placar, siga os passos da [seção 3.2.1](#321-conectar-se-ao-wifi-do-placar).
3. Acesse a página da web com as [configurações de WiFi](#333-wifi).
4. Na seção "Conectar a outra rede WiFi", verifique se está ativado; caso não esteja, ative.
5. No menu suspenso dessa seção, selecione a rede WiFi à qual deseja conectar o placar e insira e confirme a senha.
6. Após clicar em "Aplicar", um aviso aparecerá; ao aceitá-lo, o servidor web será reiniciado.
7. Observe as mensagens na tela para verificar se o placar se conectou à rede WiFi configurada. Caso contrário, repita os passos, certificando-se de inserir a senha corretamente.
8. **Importante**: A senha não pode conter caracteres especiais, barra invertida ( \ ) ou ponto e vírgula ( ; ). A rede WiFi deve ser de 2,4 GHz. Redes mais recentes de 5 GHz não são compatíveis.

**DICA**: Para não perder mensagens na tela devido ao possível início do cronômetro, realize essa configuração com as células desligadas.

Assista ao vídeo (Ative as legendas no idioma de sua preferência, pois o áudio está em espanhol):  
[Ver o vídeo no YouTube](https://youtu.be/FqYA5eCeje0)  

---

### 3.3 Páginas Web

Ao acessar a página web do placar ZonEcron, a página principal será a aba "Info". Dependendo se você está acessando de um celular ou de um PC, as abas aparecerão na parte superior ou no lado esquerdo, respectivamente. Cada aba oferece opções diferentes para configurar o placar ou simplesmente consultar certas informações.

---

#### 3.3.1 Info

Nesta seção, você pode:

- **Sincronizar data e hora**: Ajuste a data e a hora do cronômetro para coincidir com as do seu dispositivo pressionando um botão.
- **Verificar a temperatura interna**: Muito útil para garantir que tudo está funcionando corretamente.
- **Verificar o status das células**: Se estiverem ligadas, você pode verificar a porcentagem de bateria de cada uma.
- **Ver as informações da versão do placar**.

Página de informação:
![Página principal da web](../images/scoreboard/web_main.png)

---

#### 3.3.2 Arquivos

Nesta aba, você pode gerenciar os arquivos armazenados no servidor do placar ZonEcron. Em especial, destacamos os **registros de tempo**, que são arquivos nomeados como `cronoLog#.txt` e contêm os tempos registrados. Aqui, `#` é um número de 0 a 3. Clique neles para visualizá-los e consultar todos os tempos registrados pelo placar.

- **Lista de arquivos**: Mostra uma lista de todos os arquivos e, ao final, o espaço total ocupado e disponível. Este servidor é muito leve, utilizando apenas alguns KB.
- **Carregar arquivos**: Esta opção não deve ser usada em condições normais. Por isso, não compartilhamos a chave necessária aqui. Caso precise dela sob nossa orientação, forneceremos a chave. Um exemplo seria substituir o logotipo ZonEcron pelo logotipo da sua associação, mas o arquivo deve atender a certos requisitos, e pediremos para revisá-lo antes do upload.
- **Excluir arquivos**: O mesmo que acima.
- **Excluir registros de tempo**: Inserindo a chave "disturbingLackOfFaith", o servidor apagará todos os **registros de tempo** e começará a registrar a partir do zero. Isso pode ser útil se você não quiser manter registros de uma competição anterior ao iniciar uma nova. Geralmente, isso não é necessário, pois o placar sobrescreve os registros mais antigos para evitar a falta de espaço.

**DICA**: Se você tiver vários **registros de tempo**, o atual (onde o placar está gravando novos registros) será o menor em tamanho.

Exemplo de registro de tempos: 
![Registros em texto](../images/scoreboard/web_logs.png)

---

#### 3.3.3 WiFi

O placar ZonEcron pode criar sua própria rede WiFi ou se conectar a uma existente. Por padrão, ele se lembrará da última rede usada e tentará se conectar a ela. Caso não consiga, criará sua própria rede WiFi.

Nesta aba, você pode gerenciar a rede WiFi criada pelo placar e/ou a rede à qual ele deve se conectar. Apenas um modo (rede própria ou externa) estará ativo. Embora seja possível ativar ambos os modos simultaneamente para alterações temporárias, não recomendamos operar com ambos os modos ativados regularmente, pois isso pode causar problemas de conexão.

- **Criar rede WiFi própria**: Ative ou desative a rede e altere o nome e a senha conforme necessário. Útil para recuperação do WiFi.
- **Conectar-se a uma rede existente**: Analise as redes disponíveis e selecione a qual se conectar. Mostra também a qualidade do sinal após a conexão.
- **Reiniciar**:
  - **Reiniciar**: Essa opção desligará e ligará o servidor (não o placar). Isso cortará todas as conexões WiFi ativas no momento.
  - **Resetar**: Essa opção apagará as configurações de WiFi e restaurará os valores de fábrica. Em seguida, reiniciará o servidor como na opção anterior.

Como mencionado, este servidor é muito compacto e possui capacidade limitada. Recomendamos no máximo 3 usuários simultâneos para conexões estáveis.

**DICA**: Se você desligar ambos os modos (rede própria e externa), o placar ZonEcron ficará sem WiFi (as células continuarão funcionando) até que seja reiniciado. Isso pode ser útil se você suspeitar de interferências intencionais.

---

#### 3.3.4 Personalização

Aqui você pode ajustar vários aspectos para personalizar o placar ZonEcron de acordo com suas necessidades:

- **Clube**: Configure duas linhas de texto com até 10 caracteres cada, normalmente o nome do clube. Este texto será usado como protetor de tela quando o placar estiver inativo por mais de 2 minutos.
- **Mensagens temporárias**: Defina mensagens que aparecerão na tela enquanto o cronômetro estiver parado. Você pode definir sua duração ou deixá-las indefinidas (tempo 0). Essas mensagens desaparecerão se o cronômetro for reiniciado ou se uma célula detectar uma passagem.
- **Cores**: Altere as cores da interface web. As alterações são imediatamente visíveis, mas só serão salvas após confirmação. Evite combinações que possam ser desconfortáveis para os olhos. Por exemplo:

![Cores vibrantes](../images/scoreboard/web_colors.png)

---

#### 3.3.5 Modos Especiais

Nesta seção, você pode configurar modos especiais para competições ou treinos:

- **Games**: Configure os parâmetros para realizar uma rodada de games, conforme explicado na [seção 2.4.4](#244-modo-games).
- **Detecção múltipla**: Configure as detecções extras necessárias para que o cronômetro pare e a tela exiba o tempo congelado durante as detecções intermediárias, enquanto o cronômetro continua rodando.
- **Tempo de partida**: Ative o modo de partida e configure o tempo de início (por padrão, 15 segundos) para funcionar conforme explicado na [seção 2.4.2](#242-modo-largada).

Ao aplicar o modo Jogos ou o modo Detecção Múltipla, uma mensagem de confirmação será exibida na tela (se o cronômetro estiver parado):

- Modo games:
![games](../images/scoreboard/disp_games.jpeg)

- Modo detecção múltipla:
![extra](../images/scoreboard/disp_extra.jpeg)

---

#### 3.3.6 Controle Remoto

A partir desta tela, o operador do cronômetro pode gerenciar (por exemplo, usando seu celular) as funções principais do cronômetro, como:

- Marcar faltas, recusas e eliminações.
- Reiniciar o cronômetro.
- Ativar o modo de reconhecimento de pista e ajustar seu tempo.

Controle remoto em um celular:
![Controle Remoto](../images/scoreboard/web_remote.png)

O controle remoto também exibe o tempo em execução, o estado de bateria fraca ou desalinhamento das células, e os últimos 5 resultados na parte inferior para consulta rápida da equipe de pista.
![Últimos Resultados](../images/scoreboard/web_latest.png)

Algumas regras:

- **Recusas no início**: Se o cronômetro estiver reiniciado, marcar uma recusa iniciará o tempo e ignorará a primeira passagem pela célula. (Se o cronômetro não estiver reiniciado, a recusa será adicionada ao resultado exibido na tela).
- **Correções**: Você pode corrigir faltas, recusas e eliminações mesmo após o término do percurso.
- **Reiniciar**: Este botão só estará ativo por 5 segundos após o término de um percurso ou quando o competidor estiver eliminado, para evitar reinícios acidentais (que não podem ser corrigidos).

---

#### 3.3.7 Monitor

A tela do monitor exibe as mesmas informações do controle remoto, mas sem botões. É ideal para placares de vídeo voltados ao público, pois também pode exibir o logotipo do clube como plano de fundo.

---

#### 3.3.8 Software

Nesta seção, você pode configurar a conexão do placar com um software de terceiros via websocket. Embora originalmente projetado para comunicar-se com a plataforma [FlowAgility](https://www.flowagility.com/), o placar pode se conectar a qualquer software que possua um servidor websocket usando o protocolo de mensagens [descrito aqui](https://github.com/ZonEcron/ZonEcron-Interfacing/blob/main/WebsocketClient.md#4-mode-meanings-and-examples).

Note que, para conectar o placar desta forma, ele deve estar conectado a uma rede WiFi externa, conforme descrito na [seção 3.2.4](#324-conectar-o-placar-a-uma-rede-wifi-externa). Além disso, se o software for uma plataforma online, como é o caso do FlowAgility, essa rede WiFi externa deve ter acesso à Internet.

Nesta página, você encontrará:

- **Endereço do software**: Esta seção contém os dados necessários para conectar-se à plataforma FlowAgility (e, eventualmente, a outros softwares de terceiros):
  - URL: Endereço ao qual o placar deve tentar se conectar. Este endereço deve ser fornecido pelo software ao qual deseja se conectar.
  - Endereço MAC: O endereço MAC do placar. FlowAgility solicita esse endereço para gerar a URL de conexão mencionada acima.
  - Por fim, há um indicador mostrando o estado atual da conexão.
- **Serial & WS client connection log**: Exibe as mensagens recebidas do cronômetro e do software de terceiros. Este log tem um máximo de 5000 caracteres; ao atingir o limite, as mensagens mais antigas serão apagadas para exibir as mais recentes. Além disso, este log não é salvo; se a página for fechada ou recarregada, o log será reiniciado.
- **DANGER ZONE - KEEP AWAY BUTTERFINGERS**: Nesta seção, que recomendamos não tocar (a menos que você saiba o que está fazendo), após pressionar o botão, aparecerão os seguintes campos:
  - SSL: Para usar uma conexão websocket segura (wss) ou normal (ws).
  - Porta: Para alterar a porta do servidor ao qual o placar deve se conectar.
  - Informações extras: Para exibir mais informações no log.

---

#### 3.3.9 Streaming

Esta tela não está acessível diretamente pelo menu, mas pode ser visualizada na lista de arquivos.

Ela foi projetada para ser capturada por programas de streaming e exibir a contagem em tempo real.  
![Streaming web](../images/scoreboard/web_streaming.png)

Se você precisar de algo mais sofisticado ou personalizável, pode usar [nosso HTML personalizável](https://github.com/ZonEcron/FlowAgilityStreamingInfo). Ele foi criado para se conectar também com o FlowAgility, mas não é obrigatório, e as informações não utilizadas podem ser ocultadas. Personalize-o como preferir e conecte ao placar para um streaming/videowall impressionante.  
![Flow Agility Streaming Info](../images/scoreboard/FASI.png)  

---

## 4 Contato

Para suporte técnico, dúvidas ou sugestões, entre em contato conosco pelo e-mail: [ZonEcron@gmail.com](mailto:ZonEcron@gmail.com?subject=placar%20ZonEcron).

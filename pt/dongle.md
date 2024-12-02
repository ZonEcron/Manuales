# ZONECRON GATEWAY - MANUAL
## Manual do Usuário

![Dongle](../images/dongle/dongle.png)

### Conteúdo

1. [Introdução](#1-introdução)
2. [Preparativos](#2-preparativos)
   - [2.1 Janela "Não fechar"](#21-janela-não-fechar)
   - [2.2 Antes de começar](#22-antes-de-começar)
3. [Conexões e acessibilidade](#3-conexões-e-acessibilidade)
   - [3.1 Conexão ao dongle Zonecron](#31-conexão-ao-dongle-zonecron)
   - [3.2 Conexão ao Flowagility](#32-conexão-ao-flowagility)
   - [3.3 Acessando de outros dispositivos na rede](#33-acessando-de-outros-dispositivos-na-rede)
4. [Exibição e operação](#4-exibição-e-operação)
   - [4.1 Operação do cronômetro pelo aplicativo](#41-operação-do-cronômetro-pelo-aplicativo)
   - [4.2 Exibindo o cronômetro em uma tela](#42-exibindo-o-cronômetro-em-uma-tela)
   - [4.3 Turno](#43-turno)
   - [4.4 Exibições em streaming](#44-exibições-em-streaming)
   - [4.5 Personalização de streaming](#45-personalização-de-streaming)
5. [Diversos](#5-diversos)
   - [5.1 Múltiplos cronômetros](#51-múltiplos-cronômetros)
   - [5.2 Informações](#52-informações)
   - [5.3 Saindo do aplicativo](#53-saindo-do-aplicativo)

---

## 1 Introdução

O ZonEcron©, e quando dizemos ZonEcron©, queremos que você imagine luzes de néon e fogos de artifício ao fundo (ok, vou pular esta parte para o restante do manual, caso contrário, ficará muito longo)—como eu estava dizendo, o ZonEcron© foi projetado para atender à necessidade de cronometrar a execução de zonas (pista, paliçada e gangorra) e, logicamente, também para cronometrar sequências curtas para determinar qual opção é melhor.

Adicionar um dongle para gerenciar o cronômetro a partir de um computador foi uma evolução lógica. O placar ZonEcron© já possui seu próprio servidor web, tornando esta combinação mochila com APP redundante. Portanto, se você possui um placar ZonEcron©, esta mochila com o APP é um método redundante de se comunicar com o cronômetro.

O APP pode ser baixado [aqui](https://zonecron.github.io/ZonEcronGW/).

---

## 2. Preparativos

### 2.1 Janela "Não fechar"

1. Quando o aplicativo é iniciado, uma janela será aberta que não deve ser fechada. Na própria janela, aparece "NÃO FECHAR ESTA JANELA" em inglês.
2. Uma série de comandos pode ser digitada nesta janela para testes ou resolução de problemas. Nesta janela, digite "HELP" e pressione a tecla Enter para mais informações.
3. Os comandos e respostas nesta janela estão em inglês. Apenas o manual e a ajuda são traduzidos para o idioma padrão configurado.

---

### 2.2 Antes de começar

1. Quando o aplicativo é iniciado, um navegador (Firefox, Chrome, etc.) também deve abrir com a página da web que contém este manual. Se não abrir, isso pode ser devido a restrições de segurança na máquina que está executando o aplicativo. Nesse caso, abra um navegador e digite o seguinte endereço: 
    - http://localhost:8080
2. Pode ser necessário tentar diferentes portas entre 8081 e 8100, se a porta 8080 já estiver ocupada quando o aplicativo foi iniciado: 
    - http://localhost:8081
    - http://localhost:8082 
    - ...
3. No canto superior direito, o idioma da sessão atual pode ser alterado, mas o idioma padrão não será modificado.
4. O menu à esquerda possui quatro opções: "Informações", "Conectar", "Controles" e "Telões". Ao clicar, por exemplo, na seção "Informações", aparece um submenu com mais quatro opções: "Manual", "Sistema", "Tempos" e "Licença". Ao clicar, por exemplo, em "Sistema", você é redirecionado para a página da web com opções para configurar o idioma padrão (para que você não precise alterá-lo sempre que o aplicativo for iniciado) e outras informações do sistema. A partir daqui, as referências a cada seção serão abreviadas. Este exemplo é abreviado como **Informações -> Sistema**.
5. O computador deve reconhecer o dongle ZonEcron quando estiver conectado. Normalmente, um tom deve soar quando qualquer dispositivo USB for conectado. Se não, você precisará instalar os drivers para o chip CH340G. Aqui está o site do fabricante: https://www.wch-ic.com/downloads/CH341SER_ZIP.html .
6. Para os passos seguintes, o dongle deve permanecer desconectado do computador até que seja instruído de outra forma.
7. Se você pretende se conectar à plataforma FlowAgility, certifique-se de que o computador tenha acesso à Internet, por exemplo, navegando até um site de notícias.

---

## 3. Conexões e acessibilidade

### 3.1 Conexão ao dongle Zonecron

1. Para conectar o dongle ao aplicativo, clique no menu à esquerda em **Conectar -> Dongle**.
2. A seção "porta serial" tem um menu suspenso com as portas seriais disponíveis no computador. Preste atenção a quais são elas.
3. Conecte o dongle ZonEcron ao computador.
4. Clique em atualizar e verifique as portas seriais novamente. O dongle será a nova porta que não estava lá antes.
5. Clique em conectar, e uma mensagem cinza aparecerá: "Aberto. Aguardando um sinal do dongle." Se tudo correr bem, após dois ou três segundos, ela ficará verde claro, indicando "Dongle encontrado. Aguardando sinal do timer."
6. Ao iniciar ou parar o timer cortando o feixe das células, a mensagem deve mudar para "Dongle e timer verificados." em verde escuro. Se não, revise todo o processo de conexão.

---

### 3.2 Conexão ao Flowagility

1. Selecione no menu à esquerda **Conectar -> FlowAgility**.
2. Copie o endereço MAC de 12 caracteres.
3. No site da FlowAgility https://FlowAgility.com , após fazer login, acesse o teste onde você tem acesso de organizador.
4. Selecione o ícone de gerenciamento de timer na parte superior. Uma vez lá, cole o endereço MAC copiado anteriormente no campo correspondente e clique em "Parear com o timer."
5. A página mudará e uma URL semelhante a "flowagility.com/ws/timer/123456ABCDEF" aparecerá. Copie essa URL.
6. De volta à página **Conectar -> FlowAgility**, cole a URL no campo "URL" e clique em conectar.
7. Se tudo estiver correto, a mensagem "Conectado." deve aparecer em verde. Se não, revise todo o processo a partir do passo 2. Tenha cuidado para não incluir espaços antes ou depois do texto ao copiar, e não inclua "https://" ou "www" – apenas copie a URL fornecida.
8. Uma vez conectado, o timer também deve aparecer como conectado na página da FlowAgility. Se não, atualize a página.
9. Você pode testar iniciar e parar o timer, e ele deve iniciar e parar na página da FlowAgility. Você também pode testar redefinir o timer a partir da página da FlowAgility e verificar se o timer foi redefinido.
10. A comunicação bidirecional agora está estabelecida.

---

### 3.3 Acessando de outros dispositivos na rede

1. Este aplicativo faz com que o computador em que está sendo executado atue como um servidor web local. Portanto, as páginas da web podem ser acessadas de qualquer outro dispositivo (PC, tablet, celular) que esteja na mesma rede.
2. Para acessar de outro dispositivo, basta abrir um navegador (Firefox, Chrome, ...) e digitar o endereço que aparece em **Informações -> Sistema** na seção "Acesso à Web", na linha "De outros dispositivos na rede".
3. **Por exemplo**, é possível:
    - Ter o computador reservado em uma mesa com o dongle conectado e o aplicativo em execução sem supervisão
    - Marcar falhas e recusas de um celular na borda da arena
    - Exibir o tempo, falhas e recusas em uma televisão na entrada do ringue

---

## 4. Exibição e operação

### 4.1 Operação do cronômetro pelo aplicativo

1. O timer pode ser controlado a partir do aplicativo clicando na seção **Controles -> Timer** no menu à esquerda.
2. No exemplo anterior, isso seria o que é aberto no celular.
3. Os controles são bastante intuitivos. Você pode aumentar e diminuir falhas e recusas, deletar e restaurar, marcar tempos de reconhecimento e mais.
4. Vale ressaltar que, para reiniciar o timer, o par deve primeiro ser eliminado. Isso é para evitar reinicializações acidentais, pois um reinício não pode ser desfeito.
5. Se o aplicativo estiver conectado ao FlowAgility, esses controles não são necessários, pois usar ambas as opções ao mesmo tempo (controles e FlowAgility) pode causar erros na gravação dos resultados.

---

### 4.2 Exibindo o cronômetro em uma tela

1. Selecione **Telões -> Monitor** no menu à esquerda.
2. No exemplo anterior, isso seria o que é aberto no navegador de uma smart TV.
3. Esta página é projetada para exibir o timer ao público em um monitor/televisão de tamanho médio a grande que permita a leitura das informações a uma certa distância.
4. O timer em execução será exibido, assim como as falhas e recusas recebidas dos controles ou da plataforma FlowAgility.
5. Na parte inferior, existem dois seletores para mudar as cores de fundo e do texto, caso você queira dar uma aparência mais festiva ou corporativa. Recomendamos usar cores com bom contraste entre si.

---

### 4.3 Turno

1. Essa funcionalidade é um bônus que não está relacionada ao timer em si. A ideia é semelhante ao exemplo do timer, onde, a partir de um celular, você indica o número do cão na pista, e em um monitor ou televisão separado, esse número é exibido em grande formato.
2. O controle para essa função está localizado no menu à esquerda em **Controles -> Turno**. É possível gerenciar a indicação do número do cão na pista, bem como o número da altura do salto atual: 20 (XS na Espanha), 30 (S), 40 (M), 50 (I) e 60 (L).
3. Para exibir o turno ao público, mostre a tela localizada no menu à esquerda em **Telões -> Turno** em um monitor ou smart TV. Essas informações são muito úteis para os competidores verem o número à distância e organizarem seus tempos de preparação.
4. Assim como na tela do timer, as cores de fundo e do número podem ser alteradas com os dropdowns na parte inferior.

---

### 4.4 Exibições em streaming

1. As seções **Telões -> Streaming** e **Telões -> Streaming FA** são projetadas para serem capturadas por programas de streaming.
2. Elas diferem em que a primeira é uma versão simplificada da segunda para quando o FlowAgility não é utilizado, mas com as mesmas opções de personalização.

---

### 4.5 Personalização de streaming

Como as telas de streaming são especialmente projetadas e altamente personalizáveis, estamos dedicando uma seção para explicar as possibilidades que elas oferecem.

1. Um clique duplo em uma área vazia da tela abrirá a janela geral.
2. Nesta janela geral, você pode inserir manualmente a distância do percurso para exibir o cálculo de velocidade em tempo real. A velocidade não será exibida durante os primeiros 5 segundos do percurso. O campo de entrada "Velocidade Máxima" é usado para evitar mostrar velocidades excessivamente altas. Se a aplicação estiver conectada ao FlowAgility, as informações de distância serão atualizadas automaticamente. Caso contrário, a distância deve ser inserida manualmente para cada corrida.
3. A partir desta janela geral, você também pode fazer upload de uma imagem de fundo, que será salva com o restante das personalizações quando você salvar.
4. Na tela "streaming FA", esta janela incluirá a opção de se conectar ao FlowAgility. Para atualizar as informações, você deve inserir a URL de conexão fornecida pelo FlowAgility neste menu e pressionar o botão de conectar.
5. Na parte inferior desta janela geral, há um botão para entrar no modo de edição. Neste modo, você pode arrastar e soltar cada texto (tempo, faltas, nome do cão, etc.) para posicioná-lo onde quiser. Um clique duplo em cada texto abrirá uma janela de propriedades onde você pode mudar seu tamanho, cor, transparência, etc. Se qualquer janela estiver aberta, você não poderá arrastar e soltar nada, exceto a própria janela. Ela deve ser fechada para arrastar ou editar outros textos.
6. Ativar a opção "Ocultar" para um elemento não o esconderá até que você saia do modo de edição. No modo normal (não edição), o elemento "Eliminado" e os elementos "Faltas" e "Recusas" alternarão (um ou outro) dependendo se a dupla foi eliminada ou não. No modo de edição, ambos serão visíveis para que possam ser editados. Por exemplo, se você decidir ocultar permanentemente "Faltas" e "Recusas" ativando a opção "Ocultar", o elemento "Eliminado" manterá seu comportamento no modo normal, tornando-se visível apenas quando a dupla for eliminada, e vice-versa.
7. No modo de edição, você pode desfazer as últimas 100 ações com Ctrl + Z ou refazer as últimas 100 ações desfeitas com Shift + Ctrl + Z.
8. Depois de concluir a personalização, clique duas vezes em uma área vazia para exibir novamente a janela geral e pressione o botão para sair do modo de edição.
9. Na mesma janela, pressionar o botão de salvar salvará os ajustes feitos e os manterá mesmo se a página da web for fechada e aberta novamente mais tarde.
10. Pressionar o botão de salvar também sincronizará esses ajustes em todas as **mesmas janelas do navegador** exibindo a mesma página de streaming. Esse recurso permite que você modifique o design da janela em uma instância e, ao salvar, atualize a janela sendo transmitida sem mostrar os menus e propriedades abertos para modificações.
11. No caso de um erro de comunicação com o cronômetro ou a plataforma FlowAgility, uma tentativa de reconexão será feita continuamente com uma pausa de 5 segundos entre as tentativas.
12. O botão Importar/Exportar permite que você salve a configuração em um arquivo para backups ou migrações. A função de importação está disponível apenas para novas configurações ou configurações recentemente redefinidas. Se a opção de importação não aparecer, você precisará pressionar o botão de redefinir para reiniciar as configurações, pois qualquer alteração transformará o botão de importação em um botão de exportação.
13. Alguns botões ou ações exibirão uma mensagem de ajuda pop-up quando clicados ou quando o mouse pairar sobre o elemento por alguns segundos.

---

## 5. Diversos

### 5.1 Múltiplos cronômetros

1. É possível executar o programa várias vezes se você tiver vários dongles com seus cronômetros para cursos simultâneos, por exemplo.
2. Nesse caso, cada instância da aplicação criará um ponto de acesso diferente, com o mesmo endereço, mas uma porta diferente, por exemplo: 
    - http://localhost:8080
    - http://localhost:8081
3. Os códigos necessários para se conectar com o FlowAgility (endereço MAC) serão consecutivos.
4. As páginas para as primeiras 8 instâncias serão abertas com cores diferentes para diferenciá-las facilmente. A partir da nona, se isso acontecer, elas serão abertas com a cor padrão.

---

### 5.2 Informações

1. Na página da web **Informações -> Sistema**, você pode:
   - Selecionar o idioma padrão.
   - Visualizar os endereços para acessar a aplicação a partir do computador onde está sendo executada ou de outro dispositivo na mesma rede. Por exemplo, se seu computador estiver conectado ao Wi-Fi e seu celular também estiver conectado à mesma rede, você pode acessar a aplicação do seu celular inserindo o endereço exibido na seção "Acesso Web", na linha "De outros dispositivos na rede".
   - Visualizar o status da bateria das células do ZonEcron.
   - Visualizar informações básicas sobre o dongle (chato).
   - Visualizar os últimos 10 tempos registrados pelo cronômetro no dia atual em ordem reversa (mais recente primeiro), se a aplicação estiver conectada ao dongle.
2. Na página da web **Informações -> Tempos**, todos os tempos registrados pelo cronômetro no dia atual são exibidos. Tempos de dias anteriores também estão disponíveis em arquivos de texto (um por dia) na pasta "logs" dentro da pasta da aplicação.
3. Na página da web **Informações -> Manual**, você pode consultar este manual.
4. Na página da web **Informações -> Sobre**, você pode ler a licença de uso.

---

### 5.3 Saindo do aplicativo

1. Para fechar a aplicação, basta fechar a janela "NÃO FECHAR" ou digitar o comando "sair" nela.
2. Todas as páginas da web abertas em qualquer dispositivo perderão a comunicação e pararão de receber informações atualizadas.
3. Todos os dados de configuração serão salvos. Se uma conexão bem-sucedida foi estabelecida com o dongle ou o FlowAgility, essa configuração também será salva. Na próxima vez que a aplicação for iniciada, tentará automaticamente se conectar ao dongle e ao FlowAgility usando essa configuração.
4. Em dias diferentes, a conexão com o FlowAgility muda, portanto, não funcionará de um dia para o outro.

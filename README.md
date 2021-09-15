# **Curso Formação Fundamental Linux**

# **Sistema Operacional**

Um sistema operacional (SO) é uma coleção de programas que inicializam o hardware do computador. Fornece rotinas básicas para controle de dispositivos. Fornece gerência, escalonamento e interação de tarefas. Mantém a integridade de sistema.

Oi pessoal, vamos lá? Sistema operacional(SO)? O que é isso? Será que é apenas um grande software de alto porte que opera simplesmente para digitar um texto qualquer ou jogar paciência spider? rs! Errado! Nessa matéria vamos saber a verdade sobre o que é um sistema operacional.

Há muitos tipos de Sistemas Operacionais, cuja complexidade varia e depende de que tipo de funções é provido, e para que computador esteja sendo usado. Alguns sistemas são responsáveis pela gerência de muitos usuários, outros controlam dispositivos de hardware como bombas de petróleo.

O sistema operacional funciona com a iniciação de processos que este irá precisar para funcionar corretamente. Esses processos poderão ser arquivos que necessitam de ser frequentemente atualizados, ou arquivos que processam dados úteis para o sistema. Poderemos ter acesso a vários processos do sistema operacional a partir do gerenciador de tarefas, onde se encontram todos os processos que estão em funcionamento desde a inicialização do sistema operacional até a sua utilização atual.

## **O Sistema Operacional é...**

O sistema operacional é uma coleção de programas que:

- Inicializa o hardware do computador;
- Fornece rotinas básicas para controle de dispositivos;
- Fornece gerência, escalonamento e interação de tarefas;
- Mantém a integridade de sistema.

Um Sistema Operacional muito simples para um sistema de controle de segurança poderia ser armazenado numa memória ROM (Só de Leitura - um chip que mantém instruções para um computador), e assumir o controle ao ser ligado o computador. Sua primeira tarefa seria reajustar (e provavelmente testar) os sensores de hardware e alarmes, e então ativar uma rotina monitorando ininterruptamente todos os sensores introduzidos. Se o estado de qualquer sensor de entrada for mudado, é ativada uma rotina de geração de alarme.

Em um grande computador multiusuário, com muitos terminais, o Sistema Operacional é muito mais complexo. Tem que administrar e executar todos os pedidos de usuários e assegurar que eles não interferiram entre si. Tem que compartilhar todos os dispositivos que são seriais por natureza (dispositivos que só podem ser usados por um usuário de cada vez, como impressoras e discos) entre todos os usuários que pedem esse tipo de serviço. O SO poderia ser armazenado em disco, e partes dele serem carregadas na memória do computador (RAM) quando necessário. Utilitários são fornecidos para:

- Administração de Arquivos e Documentos criados por usuários;
- Desenvolvimento de Programas;
- Comunicação entre usuários e com outros computadores;
- Gerenciamento de pedidos de usuários para programas, espaço de armazenamento e prioridade.

Adicionalmente, o SO precisaria apresentar a cada usuário uma interface que aceita, interpreta, e então executa comandos ou programas do usuário. Essa interface é comumente chamada de SHELL (=cápsula, manteremos o nome original em inglês) ou interpretador de linha de comando (CLI). Em alguns sistemas ela poderia ser uma simples linha de texto que usam palavras chaves (como MSDOS ou UNIX); em outros sistemas poderiam ser gráficas, usando janelas e um dispositivo apontador como um mouse (como Windows95 ou X – Windows).

## **As Várias Partes de um Sistema Operacional**

Um sistema operacional de um computador que é usado por muitas pessoas ao mesmo tempo, é um sistema complexo. Contém milhões de linhas de instruções escritas por programadores. Para tornar os sistemas operacionais mais fáceis de serem escritos, eles são construídos como uma série de módulos, cada módulo sendo responsável por uma função. Os módulos típicos em um grande SO multiusuário geralmente são:

- Núcleo (Kernel em inglês - também conhecido como "executivo");
- Gerenciador de processo;
- Escalonador (Scheduler, em inglês);
- Gerenciador de arquivo.

## **O Núcleo – Um Executivo em Tempo Real**

O núcleo de um sistema operacional é algumas vezes chamado de EXECUTIVO em tempo real. Algumas das funções executadas por ele são:

- Chaveamento entre programas;
- Controle e programação de dispositivo de hardware;
- Gerenciamento de memória;
- Gerenciamento de processos;
- Escalonamento de tarefas;
- Comunicação entre processos;
- Processamento de exceções e de interrupção .

Nosso sistema simples de monitoração de segurança não teria todas as funções acima, já que provavelmente seria um sistema mono tarefa, executando apenas um programa. Como tal, não precisaria processar permutas entre mais de um programa ou permitir comunicação entre programas (comunicação entre processos). A gerência da memória seria desnecessária, já que o programa residiria permanentemente em ROM ou em EPROM (uma forma programável especial de ROM).

Um sistema operacional projetado para manusear um grande número de usuários precisaria de um núcleo para executar todas as funções acima. Programas de usuários geralmente são armazenados em disco, assim precisa ser carregado em memória antes de ser executado. Isso apresenta a necessidade de gerência da memória, já que a memória do computador precisaria ser pesquisada para localizar uma área livre para carregar um programa de usuário na mesma. Quando o usuário tivesse encerrada a execução do programa, a memória consumida por ele precisaria ser liberada e se tornaria disponível para outro usuário quando solicitado.

Gerenciamento e Escalonamento (Scheduling) de processos também são necessários, de forma que todos os programas possam ser executados razoavelmente. Não há como um programa de um usuário específico ser executado numa área de extensão, negando o funcionamento de qualquer outro programa, e fazendo todos os outros usuários esperarem. Adicionalmente, alguns programas poderiam precisar ser executados mais frequentemente que outros, por exemplo, checando comunicações de rede ou imprimindo. Alguns programas podem precisar ser suspensos temporariamente, e serem reiniciados depois, assim introduzindo a necessidade da comunicação inter-programas.

## **Programando um computador**

Um programa é uma sequência de instruções ao computador. Quando o programador de software (uma pessoa que escreve programas para serem executados em um computador) desenvolve um programa, este é convertido em uma longa lista de instruções que são executadas pelo sistema de computador.

Em sistemas operacionais nós falamos mais de um processo do que de um programa. Nos sistemas operacionais modernos, só uma porção de um programa é carregada em cada instante. O resto do programa espera numa unidade de disco até que se precise do mesmo. Isso economiza espaço de memória.

Os programas no computador são executados por processadores. Um processador é um chip no computador que executa instruções de programa. Processadores executam milhões de instruções por segundo.

## **Um Processo**

Um processo ou tarefa é uma porção de um programa em alguma fase de execução. Um programa pode consistir de várias tarefas, cada uma com funcionamento próprio ou como uma unidade (talvez se comunicando entre si periodicamente).

## **A Thread (fileira / linha)**

Uma thread é uma parte separada de um processo. Um processo pode consistir de várias threads cada uma das quais sendo executada separadamente. Por exemplo, uma thread poderia tratar refresh e gráficos na tela, outra thread trataria impressão, outra thread trataria o mouse e o teclado. Isso dá bom tempo de resposta em programas complexos. Windows NT é um exemplo de um sistema operacional que suporta multi-thread.

## **Sistemas Operacionais de Multi-processo**

Alguns sistemas executam só um único processo, outros sistemas executam múltiplos processos de cada vez. A maioria dos computadores é baseada num único processador, e um processador pode executar só uma instrução de cada vez. Assim, como é possível um único processador executar processos múltiplos? A resposta mais imediata é que ele não faz desse modo. O processador do computador executa um processo por um período pequeno de tempo, e então muda para o próximo processo e assim por diante. Como o processador executa milhões de instruções por segundo, isso dá a impressão de muitos processos serem executados ao mesmo tempo.

Em um sistema de computador que suporta mais de um processo de cada vez, algum mecanismo deve ser usado para intercalar de uma tarefa para outra. Há dois métodos principais usados para fazer essa troca:

- Escalonamento por Cooperação indica que uma tarefa que está sendo executada atualmente deixará voluntariamente em algum momento o processador e permitirá que outros processos sejam executados.
- Escalonamento Preemptivo significa que uma tarefa corrente será interrompida (forçou a se render) e o processador se dedica a outro processo em estado de espera.

O problema da mudança por cooperação é que um processo poderia demorar e assim negar a execução de outros processos e poderia resultar em nenhum trabalho ser feito. Um exemplo de um sistema de cooperação é o Windows 3.O escalonamento preemptivo é melhor. Dá mais respostas a todos os processos e ajuda a prevenir (ou reduz o número de ocorrências de) contra o medo de máquinas travadas. Windows NT é um exemplo de tal sistema operacional.

**Nota:** Só para programas de 32bits em Windows 95 há escalonamento preemptivo. Programas de 16bits ainda são escalonados cooperativamente, o que significa que ainda é fácil para um programa de 16bits travar um computador Windows.

## **Contexto de Troca**

Quando o processador muda de um processo a outro, o seu estado (o processador registra e associa os dados) deve ser salvo, pois algum tempo depois, será reiniciado o processo e continuará como se nunca fora interrompido. Uma vez esse estado tenha sido salvo, o próximo processo em espera é ativado. Isso envolve carga nos registradores do processador e na memória, com todos os dados previamente salvos, e reiniciando na instrução que seria executada quando houve a última interrupção. O ato de mudar de um processo a outro é chamado troca de contexto. Um período de tempo que um processo execute antes de ser trocado é chamado de time slice ou período de quantum.

## **Escalonamento (Scheduling)**

A decisão de qual o próximo processo deve ser executado é chamado escalonamento (scheduling), e pode ser feito em uma grande variedade de maneiras. Escalonadores por cooperação geralmente são muito simples, já que os processos são organizados em fila circular (ROUND ROBIN). Quando um processo corrente se deixa, vai para o fim da fila. O processo no topo da fila é então executado, e todos os processos se movimentam um lugar para cima na fila. Isso provê uma medida justa, mas não impede que um processo monopolize o sistema (não se deixando).

Escalonadores preemptivos usam um relógio em tempo real que gera interrupção a intervalos regulares (digamos, a cada 1/100 de um segundo). Cada vez que uma interrupção ocorre, o processador muda para outra tarefa. Sistemas que geralmente empregam esse tipo de escalonamento atribuem prioridades a cada processo, de forma que alguns podem ser executados mais frequentemente que outros.

## **Carga do Sistema Operacional**

O SO pode ser carregado na memória de um computador de duas maneiras.:

- Já está presente em ROM
- É carregado a partir do disco quando o computador é ligado.

Se o SO já está presente em ROM (para sistemas tipo controladores industriais, bombas de petróleo, etc), ele ganhará controle imediato do processador ao ser ligado o computador. Para sistemas mais complexos, o SO é armazenado normalmente em mídia secundária (como disco), e é carregado em RAM quando o computador é ligado. A vantagem desse tipo de sistema é que o escalonamento para o SO é mais fácil de fazer e programar.

## **O processo de BOOTSTRAP**

Descreve a ação da carga inicial do sistema operacional do disco para a RAM. Uma pequena rotina armazenada em ROM, chamada de CARREGADOR de BOOTSTRAP ou IPL (Carregador de Programa Inicial), lê uma rotina especial de carga no disquete. Em sistema baseado em disquete, essa rotina normalmente reside na trilha 00, setor 00 (ou 01), e é chamado de setor de booting. O código contido no setor é transferido para a RAM, e então é executada. Tem a responsabilidade exclusiva de carregar o resto do sistema operacional na memória.

![](http://www.oficinadanet.com.br/imagens/coluna/851/bootstra.gif)

## **Tipos diferentes de processamentos em SOs**

Sistemas operacionais são divididos em categorias que definem as suas características. Sistemas modernos podem usar combinações de essas categorias descritas a seguir.

### **Batch (.bat – em LOTE)**

O tipo mais antigo de SO permite só um programa ser executado de cada vez. O programa que é carregado no computador é executado completamente. Os dados usados pelo programa não podem ser modificados enquanto o programa está sendo executado. Qualquer erro no programa ou nos dados significa começar tudo novamente.

### **Interativo**

Esses permitem a modificação e entrada de dados ainda durante a execução do programa. Sistemas típicos são reservas de voo aéreo e linguagens como BASIC.

### **Time-Sharing / Multiusuário**

Esses SOs compartilham o computador entre mais de um usuário, e adota técnicas de escalonamento preemptivo.

### **Multitarefas**

Mais de um processo pode ser executado concorrentemente. O processador é escalonado rapidamente entre os processos. Um usuário pode ter mais de um processo executado de cada vez.

### **Tempo Real**

Principalmente usado em controle de processos, telecomunicações, etc. O SO monitora várias entradas que afetam a execução de processos, mudando os modelos de computadores do ambiente, e assim afetando as saídas, dentro de um período de tempo garantido (normalmente < 1 segundo).

### **Multiprocessamento**

Um computador que tem mais de um processador central dedicados na execução de processos. Bom. Espero que vocês gostem. Até a próxima.

# **Kernel dos Sistemas Operacionais**

O Kernel é a parte mais importante de qualquer sistema operacional sendo considerado o núcleo do sistema

Neste artigo vamos abordar as estruturas do Kernel no Linux, e aprender como funciona todo seu processo de gerenciamento.

Ele é responsável pelas funções de baixo nível, como gerenciamento de memória, gerenciamento de processos, subsistemas de arquivos, rede, suporte aos dispositivos e periféricos conectados ao computador. Os núcleos dos sistemas operacionais podem ser implementados de duas formas básicas: Kernel monolítico e o microkernel.

O Kernel monolítico é estruturado em um único arquivo binário, um único processo que executa inteiramente em modo protegido. Ele possui desempenho superior na passagem de mensagens, mas apresenta inúmeras desvantagens como a dificuldade de alterações no núcleo e o desperdício de recursos, pois os drivers de dispositivos permanecem constantemente em memória, mesmo quando os dispositivos não estão sendo utilizados.

## **Estrutura do Kernel Monolítico**

No microkernel apenas uma pequena parte do núcleo executa em modo protegido para acessar diretamente o hardware, como também é responsável pela comunicação entre processos e gerência de memória.

O restante do sistema roda em modo usuário, uma vez que executa tarefas que não necessitam acessar diretamente o hardware, e seus serviços clássicos são assegurados por processos servidores.

![](http://www.oficinadanet.com.br/imagens/post/10330/kernel_monolitico.png)

## **Estrutura do Microkernel**

![](http://www.oficinadanet.com.br/imagens/post/10330/micro_kernel.png)

Os recursos do sistema são acessados através de um protocolo cliente/servidor, e para incluir um novo serviço basta acrescentar um novo servidor. O microkernel possui um desempenho inferior ao modelo monolítico, mas podem-se alterar suas partes sem a necessidade de reiniciar a máquina permitindo a expansão para um sistema distribuído de forma mais fácil.

Pode-se entender o microkernel paralelo como um conjunto de microkernels locais cooperativos, um em cada nó da máquina paralela. O ponto crucial é a comunicação entre processos sobre um mesmo processador ou em processadores diferentes, de acordo com um protocolo cliente/servidor. O módulo responsável pela comunicação possui as funções básicas para receber mensagens originárias de outros processadores, receber resultados de operações executadas remotamente e enviar mensagens destinadas a outros processadores.

Sua organização é baseada no modelo cliente/servidor, onde os serviços do sistema são implementados por servidores especializados. Os Clientes, que são programas de aplicação, solicitam os serviços ao sistema operacional que os encaminham aos processos servidores. Estes recebem a solicitação e a executam, enviando o resultado de volta ao microkernel e então à aplicação.

Maiores detalhes sobre o funcionamento dos processos do Kernel, podemos encontrar em: [http://www.kernel.org](http://www.kernel.org/) .

# **Licenças de software**

Entenda o que é software livre e outras licenças de softwares.

## **Software Livre**

Qualquer programa que tem a liberdade de ser usado, copiado, modificado e redistribuído. Opõe-se ao conceito de software proprietário. Pode ser vendido ou disponibilizado gratuitamente. Um caso é o da Red Hat que comercializa o Red Hat Enterprise Linux. A possibilidade de modificações implica na abertura de seu código fonte. A maioria dos softwares livres é licenciada como GNU GPL ou BSD.

## **GPL**

A Licença Pública Geral GNU acompanha os pacotes distribuídos pelo Projeto GNU (General Public License). É a mais utilizada, sendo adotada pelo Linux. Ela impede que o software seja integrado em um software proprietário e garante os direitos autorais. Não permite que as liberdades originais sejam limitadas, nem que sejam impostas restrições que impeçam a distribuição da mesma forma que foram adquiridos.

## **BSD**

A licença BSD foi inicialmente utilizada nos softwares da Berkeley Software Distribution. Ela impõe poucas restrições sobre as formas de uso, alterações e redistribuição do software e, por isso, é chamada de copycenter. O programa pode ser vendido e não precisa incluir o código fonte.

## **Software em Domínio Público**

O autor do software relega a propriedade do programa e este se torna bem comum, ou seja, não possui copyright. Entretanto, o autor pode restringir que modificações sejam feitas.

## **Copyleft**

Retira barreiras à utilização, difusão e modificação do software, mas impedem a utilização não-autorizada. Ele requer que as alterações sejam livres, passando adiante a liberdade de copiá-lo e modificá-lo novamente.

## **Software proprietário**

É aquele cuja cópia, redistribuição ou modificação são proibidos pelo autor em determinado grau. É necessário solicitar permissão ou pagar para utilizar. Pode ser freeware, shareware, trial ou demo.

## **Freeware**

Software proprietário que é disponibilizado gratuitamente, mas não pode ser modificado.

## **Shareware**

É o software disponibilizado gratuitamente por um período de tempo ou com algumas funções abertas, mas que implica no posterior pagamento pela sua licença.

## **Trial**

Versão de teste de vários softwares. É disponibilizada algumas funções, geralmente por 30 dias, para que o usuário experimente o programa para saber se ele atende às suas necessidades.

## **Demo**

Versão de demonstração, semelhante ao Trial. É possível usar o programa por um tempo ou com apenas algumas funções disponíveis.

## **Software Comercial**

É o software desenvolvido com o objetivo de lucrar.

## **Open Source**

O software de código aberto é aquele que disponibiliza seu código fonte e restringe-se aos termos técnicos da questão. Pode ser livre, ou proprietário. Algumas empresas como IBM, HP, Intel e Nokia investem em software de código aberto.

# **Alguns dos softwares livres mais utilizados**

Engana-se quem pensa ser um software livre todos aqueles programas grátis que encontramos por aí. Um software livre é muito mais do que isto. Vamos discorrer sobre o que é e quais são os mais utilizados neste artigo.

Encontramos na internet diversos programas que não tem custo algum para se fazer download, dentro destes certamente estão os chamados softwares livres. Mas eles não se resumem à isso. A Free Software Foundation (FSF) descreve sua existência como : "Uma organização sem fins lucrativos com a missão mundial de promover a liberdade do usuário do computador e defender os direitos de todos os usuários de software livre".

Segundo esta definição, a FSF é uma das fundações responsáveis por fiscalizar e organizar o leque de softwares livres espalhados pelo mundo, em outras palavras, os desenvolvedores de softwares devem seguir algumas diretrizes para enquadrar-se como software livre. Já não é mais tão simplório assim, é? A definição propriamente dita de "software livre" é: Aquele software que respeita a liberdade da comunidade dos usuários. O que significa esta liberdade? Significa que qualquer usuário tem caminho aberto para executar, estudar, distribuir, alterar, melhorar, piorar, copiar qualquer parte do software ou até mesmo ele por inteiro.

Você também pode associar as palavras Open Source (Código aberto) aos softwares livres. Este tema gera discussão entre os programadores e afins por conta de algum viés ideológico que diferencia de fato, um movimento do outro. A rigor, a diferença está na ideologia de cada parte. A Free Software Foundation está voltada para o ativismo político e ideológico.

Um exemplo desta diferença pode ser descrito assim: A Adobe pode abrir o código fonte dos programas como Photoshop, InDesign, Corel Draw para visualização, mas não para cópia ou alteração. Sendo assim, os softwares podem ser considerados como Código Aberto, mas não como Software Livre. Pegou?

Só para deixar mais claro, um programa de código aberto pode não ser um software livre. Mas o contrário é obrigatório, ou seja, todo software livre deve ter seu código aberto e disponível para alterar, acrescentar e etc. O movimento Open Source não pode ser citado se não for acompanhado do hacker Eric Raymond. Já os Softwares livres são encabeçados pelo hacker Richard Stallman. Mas vamos deixar as diferenças para os Softwares livres/Open Source contra os softwares proprietários (fechados/pagos).

## **Sistemas Operacionais**

### **Linux**

Já ouviu falar, não é? Ele é talvez o Software Livre mais utilizado no mundo. Foi criado pelo finlandês Linus Torvalds, é inspirado no sistema Minix e está sob a licença GPL (General Public License) que libera para cópia, estudo, modificação entre outras opções de alteração do seu código fonte. Apoia a utilização de software como LibreOffice - também software livre - além de outras categorias de programas concorrentes aos famosos e proprietários como o Gimp e não CorelDraw.

### **OpenSolaris**

Projeto da Sun Microsystems, posteriormente adquirida pela Oracle, utiliza uma plataforma semelhante ao Linux e tem a licença GNU GPL. Inicialmente era um software proprietário, entretanto foi abrindo gradativamente seu código. O Solaris é uma versão do UNIX System V Release.

## **Ferramentas de Desenvolvimento**

### **Compilador C: GCC**

Conhecido inicialmente como GNU Compilador para C, suporta nos dias de hoje diversas linguagens além da original "C", com C++, Java, Ada e Fortran. Um software livre que atende à licença GPL e funciona em sistemas operacionais como UNIX, Linux e OS X.

### **Eclipse**

Utilizado para desenvolver aplicações em Java. Por meio de plugins, outras linguagens podem ser utilizadas: C, C++, Fortran, Java Script, PHP, entre outros. O programa é "desenhado" quase totalmente em Java e a base do código é originária da IBM VisualAge. O Eclipse possui o código aberto, entretanto não é compatível como a licença GNU.

### **NetBeans**

Outro software de código aberto. Ambiente para desenvolvimento nas linguagens convencionais (Java, C, C++, PHP, Groovy). O programa é desenvolvido pela Oracle e funciona em múltiplas plataformas, como Windows, Linux, Mac OS. Foi criado em 1996 e é um dos mais utilizados neste segmento.

## **Serviços**

### **Apache**

O software livre de código aberto é um dos servidores HTTP mais utilizados no mundo. Criado em 1995 por Rob McCool, funciona em diversas plataformas operacionais (Windows, OS/2, Linux, Unix).

### **MySQL**

O sistema de gerenciamento de banco de dados que utiliza linguagem SQL (Structure Query Language). Foi criado na Suécia durante a década de 80, porém em 2008 a Oracle comprou por mais de R$ 1 bilhão de dólares a empresa Sun Microsystems e junto com ela, todos os seus softwares. O MySQL é um dos mais utilizados no mundo. Para ter uma ideia da popularidade do programa, usuários como NADA, Nokia, Sony, Google e outras gigantes empresas conhecidas no mundo.

## **Usuário Final**

### **VLC**

O VLC media player é um excelente reprodutor multimídia, usado no mundo todo. Está disponível para todas as plataformas e sistemas operacionais. O software é leve, muito rápido e é capaz de rodar quase todos os formatos de áudio e vídeo disponíveis no mercado. Seguindo a tendência, o VLC já tem suporte para formatos em HD e aceleração gráfica. Este software é um dos que prova que os softwares livres podem ser tão excelentes quanto os softwares proprietários, muito por conta das constantes melhorias em seu código aberto.

### **GIMP**

O nome GNU Image Manipulation Program lhe diz alguma coisa? Então, o GIMP é um programa de código aberto licenciado pela GPL (General Public License). Foi criado explicitamente para ser uma alternativa livre ao uso do Adobe Photoshop. O programa roda em qualquer sistema operacional.

### **WordPress**

O sistema de gerenciamento de conteúdo na Web tem seu foco direcionado para a confecção de blogs, é escrito em PHP com banco de dados em MySQL. Junto com Blogger, é um dos mais importantes criadores de blogs disponíveis na web por conter ferramentas diferenciais. O Wordpress foi criado em 2010 e atente à licença GPL versão 2.

A lista de programas livres e de código aberto é muito extensa para citar todas aqui, os exemplos que citamos acima são simplesmente alguns dos mais conhecidos e utilizados no mundo.

# **Linux**

Linux é um termo utilizado para se referir a sistemas operacionais que utilizem o núcleo Linux. O núcleo Linux foi desenvolvido pelo programador finlandês Linus Torvalds, inspirado no sistema Minix. O seu código fonte está disponível sob a licença GPL (versão 2) para que qualquer pessoa o possa utilizar, estudar, modificar e distribuir livremente de acordo com os termos da licença.

Inicialmente desenvolvido e utilizado por grupos de entusiastas em computadores pessoais, os sistemas operacionais com núcleo Linux passaram a ter a colaboração de grandes empresas como IBM, Sun Microsystems, Hewlett-Packard (HP), Red Hat, Novell, Oracle, Google, Mandriva e Canonical.

Apoiado por pacotes igualmente estáveis e cada vez mais versáteis de softwares livres para escritório (LibreOffice, por exemplo) ou de uso geral (projeto GNU) e por programas para micro e pequenas empresas que na maioria dos casos em nada ficam a dever aos seus concorrentes proprietários, e interfaces gráficas cada vez mais amigáveis como o KDE e o GNOME, o núcleo Linux, conhecido por sua estabilidade e robustez, tem gradualmente caído no domínio popular, encontrando-se cada vez mais presente nos computadores de uso pessoal atuais. Mas já há muito que o Linux destaca-se como o núcleo preferido em servidores de grandes porte, encontrando-se quase sempre presente nos mainframes de grandes empresas e até mesmo no computador mais rápido do mundo, o Tianhe-2, chinês.

## **História**

O núcleo Linux foi, originalmente, escrito por Linus Torvalds do Departamento de Ciência da Computação da Universidade de Helsinki, Finlândia, com a ajuda de vários programadores voluntários através da Usenet (uma espécie de sistema de listas de discussão existente desde os primórdios da Internet).

Linus Torvalds começou o desenvolvimento do núcleo como um projeto particular, inspirado pelo seu interesse no Minix, um pequeno sistema UNIX desenvolvido por Andrew S. Tanenbaum. Ele limitou-se a criar, nas suas próprias palavras, "um Minix melhor que o Minix" ("a better Minix than Minix"). E depois de algum tempo de trabalho no projeto, sozinho, enviou a seguinte mensagem para comp.os.minix:

Você suspira pelos bons tempos do Minix-1.1, quando os homens eram homens e escreviam seus próprios "device drivers"? Você está sem um bom projeto em mãos e deseja trabalhar num S.O. que possa modificar de acordo com as suas necessidades? Acha frustrante quando tudo funciona no Minix? Chega de noite ao computador para conseguir que os programas funcionem? Então esta mensagem pode ser exatamente para você. Como eu mencionei há um mês atrás, estou trabalhando numa versão independente de um S.O. similar ao Minix para computadores AT-386. Ele está, finalmente, próximo do estado em que poderá ser utilizado (embora possa não ser o que você espera), e eu estou disposto a disponibilizar o código-fonte para ampla distribuição. Ele está na versão 0.02... contudo eu tive sucesso ao executar bash, gcc, gnu-make, gnu-sed, compress etc. Nele.

Curiosamente, o nome Linux foi criado por Ari Lemmke, administrador do site ftp.funet.fi que deu esse nome ao diretório FTP onde o núcleo Linux estava inicialmente disponível. Linus inicialmente tinha-o batizado como "Freax".

No dia 5 de outubro de 1991 Linus Torvalds anunciou a primeira versão "oficial" do núcleo Linux, versão 0.02. Desde então muitos programadores têm respondido ao seu chamado, e têm ajudado a fazer do Linux o sistema operacional que é hoje. No início era utilizado por programadores ou só por quem tinha conhecimentos, usavam linhas de comando. Hoje isso mudou, existem diversas empresas que criam os ambientes gráficos, as distribuições cada vez mais amigáveis de forma que uma pessoa com poucos conhecimentos consegue usar o Linux. Hoje o Linux é um sistema estável e consegue reconhecer muitos periféricos sem a necessidade de se instalar os drivers de som, vídeo, modem, rede, entre outros.

## **Núcleo**

O termo Linux refere-se ao núcleo (em inglês: "kernel") do sistema operacional. O termo também é usado pelos meios de comunicação e usuários para referir-se aos sistemas operacionais baseados no núcleo Linux agregado a outros programas. Segundo Tanenbaum e Silberschatz, um núcleo pode ser considerado o próprio sistema operacional, quando este é definido como um gerenciador de recursos de hardware.

### **Arquitetura**

O Linux é um núcleo monolítico: as funções do núcleo (escalonamento de processos, gerenciamento de memória, operações de entrada/saída, acesso ao sistema de arquivos) são executadas no espaço de núcleo. Uma característica do núcleo Linux é que algumas das funções (drivers de dispositivos, suporte à rede, sistema de arquivos, por exemplo) podem ser compiladas e executadas como módulos (em inglês: LKM - loadable kernel modules), que são bibliotecas compiladas separadamente da parte principal do núcleo e podem ser carregadas e descarregadas após o núcleo estar em execução.

### **Portabilidade**

Embora Linus Torvalds não tivesse como objetivo inicial tornar o Linux um sistema portátil, ele evoluiu nessa direção. Linux é hoje um dos núcleos de sistemas operativos mais portáteis, correndo em sistemas desde o iPaq (um computador portátil) até o IBM S/390 (um denso e altamente custoso mainframe).

Os esforços de Linus foram também dirigidos a um diferente tipo de portabilidade. Portabilidade, de acordo com Linus, era a habilidade de facilmente compilar aplicações de uma variedade de código fonte no seu sistema; consequentemente, o Linux originalmente tornou-se popular em parte devido ao esforço para que os códigos-fonte GPL ou outros favoritos de todos corressem em Linux.

O Linux hoje funciona em dezenas de plataformas, desde mainframes até um relógio de pulso, passando por várias arquiteturas: x86 (Intel, AMD), x86-64 (Intel EM64T, AMD64), ARM, PowerPC, Alpha, SPARC e etc, com grande penetração também em sistemas embarcados, como handhelds, PVR, consola de videojogos, celulares, TVs e centros multimídia, entre outros.

### **Termos de licenciamento**

Inicialmente, Torvalds lançou o Linux sob uma licença de software que proibia qualquer uso comercial. Isso foi mudado de imediato para a GNU General Public License. Essa licença permite a distribuição e mesmo a venda de versões possivelmente modificadas do Linux, mas requer que todas as cópias sejam lançadas dentro da mesma licença e acompanhadas do código fonte.

Apesar de alguns dos programadores que contribuem para o núcleo permitirem que o seu código seja licenciado com GPL versão 2 ou posterior, grande parte do código (incluído as contribuições de Torvalds) menciona apenas a GPL versão 2. Isto faz com que o núcleo como um todo esteja sob a versão 2 exclusivamente, não sendo de prever sua adoção da nova GPLv3.

### **Sistemas de arquivos suportados**

O Linux possui suporte de leitura e escrita a vários sistema de arquivos, de diversos sistemas operacionais, além de alguns sistemas nativos. Por isso, quando o Linux é instalado em dual boot com outros sistemas (Windows, por exemplo) ou mesmo funcionando como Live CD, ele poderá ler e escrever nas partições formatadas em FAT e NTFS. Por isto, Live CDs Linux são muito utilizados na manutenção e recuperação de outros sistemas operacionais.

Entre os sistemas de ficheiros suportados pelo Linux, podemos citar UFS (Unix), FAT, NTFS, JFS, XFS, HPFS, Minix e ISO 9660 (sistema de ficheiros usado em CD-ROMs), este último também com as extensões RRIP (IEEE P1282) e ZISOFS . Alguns sistemas de ficheiros nativos são, dentre outros, Ext2, Ext3, Ext4, ReiserFS e Reiser4. Alguns sistemas de ficheiros com características especiais são SWAP, UnionFS, SquashFS, Tmpfs, Aufs e NFS, dentre outros.

## **Sistema operacional**

Logo que Linus Torvalds passou a disponibilizar o Linux, ou seja na sua versão 0.01, já havia suporte ao disco rígido, tela, teclado e portas seriais, o sistema de arquivos adotava o mesmo layout do Minix (embora não houvesse código do Minix no Linux), havia extensos trechos em assembly, e ela já era capaz de rodar o bash e o gcc.

A linha guia quando implementei o Linux foi: fazê-lo funcionar rápido. Eu queria o núcleo simples, mas poderoso o suficiente para rodar a maioria dos aplicativos Unix. By: Linus Torvals

O próprio usuário deveria procurar os programas que dessem funcionalidade ao seu sistema, compilá-los e configurá-los. Talvez por isso, o Linux tenha carregado consigo a etiqueta de sistema operativo apenas para técnicos. Foi neste ambiente que surgiu a MCC Interim Linux, do Manchester Computer Centre, a primeira distribuição Linux, desenvolvida por Owen Le Blanc da Universidade de Manchester, capaz de ser instalada independentemente em um computador. Foi uma primeira tentativa de facilitar a instalação do Linux.

Desde o começo, o núcleo Linux incluía um sistema básico para chamadas do sistema e acesso aos dispositivos do computador. O núcleo de um sistema operativo define entre várias operações, o gerenciamento da memória, de processos, dos dispositivos físicos no computador e é uma parte essencial de qualquer sistema operacional utilizável, contudo para um sistema operacional adquirir funcionalidade são necessários também vários outros aplicativos que determinam funções específicas que aquele sistema será capaz de desenvolver, os aplicativos existentes em um sistema operacional com a única exceção do núcleo são determinados pelo usuário do computador, como por exemplo: interpretadores de comandos, gerenciadores de janelas, que oferecem respectivamente uma interface para o usuário do computador, CLI ou GUI, e outros aplicativos como editores de texto, editores de imagem, tocadores de som, e, mas não necessariamente, compiladores.

A maioria dos sistemas inclui ferramentas e utilitários baseados no BSD e tipicamente usam XFree86 ou X.Org para oferecer a funcionalidade do sistemas de janelas X — interface gráfica. Assim como também oferecem ferramentas desenvolvidas pelo projeto GNU.

No momento do desenvolvimento do Linux, vários aplicativos já vinham sendo reunidos pelo Projeto GNU da Free Software Foundation (‘Fundação Software Livre’), que embarcara em um subprojeto que ainda continua para obter um núcleo, o GNU Hurd. Porém devido a várias complicações o projeto GNU e demora em desenvolver o Hurd, Stallman acabou adotando o núcleo Linux como base para distribuir os programas do projeto GNU , não obstante diversas pessoas e instituições tiveram a mesma ideia e assim várias distribuições começaram a surgir baseadas no núcleo desenvolvido inicialmente por Linus.

## **Distribuições**

Atualmente, um Sistema Operacional Linux ou GNU/Linux completo (uma "Lista de distribuições de Linux ou GNU/Linux") é uma coleção de software livre (e por vezes não-livres) criados por indivíduos, grupos e organizações de todo o mundo, incluindo o núcleo Linux. Companhias como a Red Hat, a SuSE, a Mandriva (união da Mandrake com a Conectiva) e a Canonical (desenvolvedora do Ubuntu Linux), bem como projetos de comunidades como o Debian ou o Gentoo, compilam o software e fornecem um sistema completo, pronto para instalação e uso. Patrick Volkerding também fornece uma distribuição Linux, o Slackware.

As distribuições do Linux ou GNU/Linux começaram a receber uma popularidade limitada desde a segunda metade dos anos 90, como uma alternativa livre para os sistemas operacionais Microsoft Windows e Mac OS, principalmente por parte de pessoas acostumadas com o Unix na escola e no trabalho. O sistema tornou-se popular no mercado de Desktops e servidores, principalmente para a Web e servidores de bancos de dados.

No decorrer do tempo, várias distribuições surgiram e desapareceram, cada qual com sua característica. Algumas distribuições são maiores outras menores, dependendo do número de aplicações e sua finalidade. Algumas distribuições de tamanhos menores cabem num disquete com 1,44 MB, outras precisam de vários CDs, existindo até algumas versões em DVD.

Todas elas tem o seu público e sua finalidade, as pequenas (que ocupam poucos disquetes) são usadas para recuperação de sistemas danificados ou em monitoramento de redes de computadores.

Dentre as maiores, distribuídas em CDs, podem-se citar: Slackware, Debian, Suse, e Conectiva. Cada distribuição é, em tese, um sistema operacional independente, de modo que os programas compilados para uma distribuição podem não rodar em outra, embora usem o mesmo núcleo (o Linux propriamente dito). A distribuição Conectiva Linux, por exemplo, tinha as suas aplicações traduzidas em português, o que facilitou que usuários que falam a Língua Portuguesa tenham aderido melhor a esta distribuição. Hoje esta distribuição foi incorporada à Mandrake, o que resultou na Mandriva. Para o português, existe também a distribuição brasileira Kurumin (essa distribuição foi descontinuada pelo seu mantenedor), construída sobre Knoppix e Debian, e a Caixa Mágica, existente nas versões 32 bits, 64 bits, Live CD 32 bits e Live CD 64 bits, e com vários programas open source: LibreOffice, Mozilla Firefox, entre outros.

Existem distribuições com ferramentas para configuração que facilitam a administração do sistema.

As principais diferenças entre as distribuições estão nos seus sistemas de pacotes, nas estruturas dos diretórios e na sua biblioteca básica. Por mais que a estrutura dos diretórios siga o mesmo padrão, o FSSTND é um padrão muito relaxado, principalmente em arquivos onde as configurações são diferentes entre as distribuições. Então normalmente todos seguem o padrão FHS (File Hierarchy System), que é o padrão mais novo. Vale lembrar, entretanto, que qualquer aplicativo ou driver desenvolvido para Linux pode ser compilado em qualquer distribuição que vai funcionar da mesma maneira.

Quanto à biblioteca, é usada a biblioteca libc, contendo funções básicas para o sistema Operacional Linux. O problema está quando do lançamento de uma nova versão da Biblioteca libc, algumas das distribuições colocam logo a nova versão, enquanto outras aguardam um pouco. Por isso, alguns programas funcionam numa distribuição e noutras não.

Existe um movimento LSB (Linux Standard Base) que proporciona uma maior padronização. Auxilia principalmente vendedores de software que não liberam para distribuição do código fonte, sem tirar características das distribuições. O sistemas de pacotes não é padronizado.

ArchLinux, Debian, Fedora, Mandriva, Mint, Opensuse, PCLinuxOS, Puppy, Sabayon, Slackware e Ubuntu são algumas das distribuições mais utilizadas actualmente, listadas aqui por ordem alfabética.

Um exemplo de distribuição que corre num CD é o Kurumin Linux, criado por Carlos Eduardo Morimoto, baseada no Knoppix.

De entre as distribuições consideradas mais difíceis de gerir (por preferirem assegurar a estabilidade tecnológica em detrimento da interface de utilizador), destacam-se a Debian, Gentoo e Slackware.

Existem também distribuições Linux para sistemas móveis, como tablets e smartphones, sendo o Android, desenvolvido pelo Google, a mais difundida de todas. Outras distribuições Linux para sistemas móveis são o Maemo e o MeeGo.

## **Código aberto e programas livres**

Um programa, assim como toda obra produzida atualmente, seja ela literária, artística ou tecnológica, possui um autor. Os Direitos sobre a ideia ou originalidade da obra do autor, que incluem essencialmente distribuição, reprodução e uso é feito no caso de um programa através de sua licença.

Existem dois movimentos que regem o licenciamento de programas no mundo livre, os programas de código aberto e os programas livres. Os dois representados respectivamente pela OSI e pela FSF oferecem licenças para produção de software, sendo seus maiores representantes a licença BSD e a GPL.

O Linux oferece muitos aplicativos de open source, contudo nem todos podem ser considerados programas livres, dependendo exclusivamente sob qual licença estes programas são distribuídos. Os programas distribuídos sob tais licenças possuem as mais diversas funcionalidades, como desktops, escritório, edição de imagem e inclusive de outros sistemas operacionais.

Também existem organizações inclusive no mundo livre como a organização Linux Simples para o Usuário Final (SEUL) que tem como objetivo adotar a maior gama possível de aplicativos de alta qualidade produzidos sobre a GPL. É um projeto voluntário que atualmente se foca no aprendizado de Linux, seu uso na ciência e em documentos de advocacia, bem como gerenciar e coordenar projetos de desenvolvimento de aplicativos.

## **Controvérsias quanto ao nome**

Linux foi o nome dado ao núcleo de sistema operacional criado por Linus Torvalds. Por extensão, sistemas operacionais que usam o núcleo Linux são chamados genericamente de Linux. Entretanto, a Free Software Foundation afirma tais sistemas operacionais são, na verdade, sistemas GNU, e o nome mais adequado para tais sistemas é GNU/Linux, uma vez que grande parte do código-fonte dos sistemas operacionais baseados em Linux são ferramentas do projeto GNU.

Há muita controvérsia quanto ao nome. Eric Raymond afirma, no Jargon File, que a proposta da FSF só conseguiu a "aceitação de uma minoria" e é resultado de uma "disputa territorial". Linus Torvalds afirma que consideraria "justo" que tal nome fosse atribuído a uma distribuição do projeto GNU, mas que chamar os sistemas operacionais Linux como um todo de GNU/Linux seria "ridículo". Linus disse não se importar sobre qual o nome usado, considera a proposta da GNU como "válida" ("ok") mas prefere usar o termo "Linux".

### **Sobre o símbolo**

![](http://upload.wikimedia.org/wikipedia/commons/thumb/3/35/Tux.svg/160px-Tux.svg.png)

O símbolo do software foi escolhido pelo seu criador (Linus Torvalds),que um dia estava no zoológico e foi surpreendido pela mordida de um pinguim. Fato curioso e discutido até hoje.

Em 1996, muitos integrantes da lista de discussão "Linux-Kernel" estavam discutindo sobre a criação de um logotipo ou de um mascote que representasse o Linux. Muitas das sugestões eram paródias ao logotipo de um sistema operacional concorrente e muito conhecido (Windows). Outros eram monstros ou animais agressivos. Linus Torvalds acabou entrando nesse debate ao afirmar em uma mensagem que gostava muito de pinguins. Isso foi o suficiente para dar fim à discussão.

Depois disso, várias tentativas foram feitas numa espécie de concurso para que a imagem de um pinguim servisse aos propósitos do Linux, até que alguém sugeriu a figura de um "pinguim sustentando o mundo". Em resposta, Linus Torvalds declarou que achava interessante que esse pinguim tivesse uma imagem simples: um pinguim "gordinho" e com expressão de satisfeito, como se tivesse acabado de comer uma porção de peixes. Torvalds também não achava atraente a ideia de algo agressivo, mas sim a ideia de um pinguim simpático, do tipo em que as crianças perguntam "mamãe, posso ter um desses também?". Ainda, Torvalds também frisou que trabalhando dessa forma, as pessoas poderiam criar várias modificações desse pinguim. Isso realmente acontece.

Quando questionado sobre o porquê de pinguins, Linus Torvalds respondeu que não havia uma razão em especial, mas os achava engraçados e até citou que foi bicado por um "pinguim assassino" na Austrália e ficou impressionado como a bicada de um animal aparentemente tão inofensivo podia ser tão dolorosa.

## **Distribuições Linux**

- Debian
- Mint
- Ubuntu
- Mageia
- Fedora
- openSUSE
- Elementary
- Arch
- Zorin
- Puppy
- PCLinuxOS
- CentOS
- Lubuntu
- Manjaro
- Kali
- Red Hat
- Slackware
- Sabayon
- Kubuntu
- KNOPPIX
- Gentoo
- Mandriva
- Backbox
- SUSE
- Chakra

No link [http://distrowatch.com](http://distrowatch.com/), você poderá consultar mais detalhes sobre as distribuições Linux:

# **Dispositivos no Linux**

Os dispositivos são algo que temos que conhecer no Linux, senão se perdemos aos poucos nas configurações mais básicas.

## **O que são dispositivos?**

Um dispositivo é todo o componente de hardware, e do sistema operacional. Um dispositivo é "algo especial" que é compartilhado com o Kernel, ou seja, um exemplo de dispositivo são as impressoras, CD-ROMs, modems, portas, mouse, HDs, etc. No Linux, os dispositivos físicos são tratados como arquivos. Estes arquivos são um tipo especial no sistema de arquivos e se encontram no diretório /dev. Se você executar um ls neste diretório, verá que existe um muitos arquivos. Cada arquivo neste diretório corresponderá a um dispositivo de acordo com o seu tipo.

Se você usava DOS/Windows antes, você acessava o drive C:, lembra? No Linux não existe isso! Vai ser um dispositivo no lugar. Você vai usar isso o tempo todo, porque vamos mexer com mouse, com impressora, IDE’s, SCSI’s, etc. Então aqui temos alguns arquivos do /dev e seus respectivos dispositivos:

### **/dev/hdXX ou /dev/sdXX**

Aqui é correspondente às Interfaces IDEs, ou seja, tudo que tiver conectado nos cabos IDEs. Exemplos, podemos citar HD’s e CD-ROM’s. O xx significa qual IDE, onde o primeiro x corresponde a qual IDE, e o segundo x (opcional) corresponde a partição. Veja a tabela à seguir:

| **_Dispositivo_** | **_Descrição_**                      |
| :---------------- | :----------------------------------- |
| _/dev/hda_        | _IDE Primária Master_                |
| _/dev/hda1_       | _Partição 1 da IDE Primária Master_  |
| _/dev/hda2_       | _Partição 2 da IDE Primária Master_  |
| _/dev/hdb_        | _IDE Primária Slave_                 |
| _/dev/hdb1_       | _Partição 1 da IDE Primária Slave_   |
| _/dev/hdb2_       | _Partição 2 da IDE Primária Slave_   |
| _/dev/hdc_        | _IDE Secundária Master_              |
| _/dev/hdc1_       | _Partição 1 da IDE Master_           |
| _/dev/hdc2_       | _Partição 2 da IDE Master_           |
| _/dev/sda_        | _SATA Master_                        |
| _/dev/sda1_       | _Partição 1 da SATA Primária Master_ |
| _/dev/sda2_       | _Partição 2 da SATA Primária Master_ |
| _/dev/sdb_        | _SATA Primária Slave_                |
| _/dev/sdb1_       | _Partição 1 da SATA Primária Slave_  |
| _/dev/sdb2_       | _Partição 2 da SATA Primária Slave_  |
| _/dev/sdc_        | _SATA Secundária Master_             |
| _/dev/sdc1_       | _Partição 1 da SATA Master_          |
| _/dev/sdc2_       | _Partição 2 da SATA Master_          |

Perceba aqui que cada hdx or sdx vai até os números 2, mas não é apenas até o 2, pode ir mais longe. Dependendo de quantas partições tiver o seu HD, pode ser 3, ou 4, ou 9 por exemplo.

### **/dev/fdX**

Aqui é o dispositivo equivalente ao drive de disquete, onde o x corresponde a qual driver. Caso você tenha apenas um drive, esse drive vai ser o /dev/fd0. Se tiver 2 drives, o primeiro será /dev/fd0 e o segundo /dev/fd1, e por aí vai.

### **/dev/ttyX**

Quando você se loga no seu Linux, você acaba de se logar nesse terminal. Ou seja, um terminal serve para você se logar e usar uma shell (interpretador de comandos). O /dev/ttyX corresponde a cada terminal, onde X vai ser substituído pelo número do terminal (são dezenas se quiser). Pode ser /dev/tty1 (Terminal 1), /dev/tty3 (Terminal 3), /dev/tty8 (Terminal 8) e por aí vai.

Você também pode se deparar com /dev/ttypX. Neste caso é para terminais acessados por telnet/ssh.

### **/dev/ttySX**

Portas seriais! Na versão 2.2.x do kernel, estas portas seriais correspondem ao modem, ao mouse, e outras coisas ligadas nas ‘COMs’. Veja a tabela:

| **_Dispositivo_** | **_Descrição_**         |
| :---------------- | :---------------------- |
| _/dev/ttyS0_      | _COM1 (Porta serial 1)_ |
| _/dev/ttyS1_      | _COM2 (Porta serial 2)_ |
| _/dev/ttyS2_      | _COM3 (Porta serial 3)_ |
| _/dev/ttyS3_      | _COM4 (Porta serial 4)_ |

Agora se você usa um kernel com versão anterior a 2.2.x (antigo), ao invés de ser /dev/ttySX, vai ser /dev/cuaX. Ou seja, você terá os equivalentes como /dev/cua0, /dev/cua1, /dev/cua2 e /dev/cua3. E estes dispositivos /dev/cuaX são usados para determinar os modems.

### **/dev/lpX**

Corresponde a porta da impressora ou porta de um serviço paralelo. X é o número correspondente a porta 0 = LPT1 por exemplo.

### **/dev/plipX**

Esse dispositivo corresponde a uma conexão de cabo paralelo. O X será o número correspondente a porta, como no exemplo anterior.

### **/dev/console**

Este é um dispositivo especial, simbolizando os consoles (terminais não-gráficos).

### **/dev/null**

Este é um dispositivo nulo, ou seja, tudo que você mandar ou se referir a ele, será nulamente mandado para um buraco negro.

### **eth X**

Este é um dispositivo de rede, uma interface de rede vaja a tabela baixo.

| **_Dispositivo_** | **_Descrição_**              |
| :---------------- | :--------------------------- |
| _eth0_            | _Primeira interface de rede_ |
| _eth1_            | _Segunda interface de rede_  |

### **wlan X**

Este é um dispositivo de rede, mas uma interface de rede Wireless (WI-FI)

| **_Dispositivo_** | **_Descrição_**              |
| :---------------- | :--------------------------- |
| _wlan0_           | _Primeira interface de rede_ |
| _wlan1_           | _Segunda interface de rede_  |

# **Estrutura de diretórios Linux**

No sistema operacional Linux a estrutura de diretórios é diferente da estrutura Microsoft, por exemplo no Windows a nossa primeira partição vai ser o "c:" no Linux é o "/" a raiz do sistema operacional. Vamos verificar os principais diretórios do nosso sistema.

## **Tabela de diretórios**

| **_Nome_** | **_Descrição_**                                                                                                                                                                                                                   |
| :--------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _/_        | _Este é o diretório raiz. Aqui é onde a arvore de diretórios começa._                                                                                                                                                             |
| _/bin_     | _Este diretório contem programas executáveis que são necessários em modo single user e que sobem com o sistema ou são utilizados para a reparação_                                                                                |
| _/boot_    | _Contém arquivos estáticos para o boot loader. Este diretório armazena os arquivos que são necessários durante o processo de boot_                                                                                                |
| _/dev_     | _Arquivos de dispositivos, que se referem a dispositivos físicos._                                                                                                                                                                |
| _/etc_     | _Contem arquivos de configuração do sistema. A grande maioria dos softwares, como X11, podem ter seus arquivos em diretórios abaixo do /etc por exemplo: /etc/X11._                                                               |
| _/home_    | _Contém o diretório home dos usuários, os arquivos dos usuários geralmente ficam abaixo deste diretório por exemplo: /home/flownerd, mais isso depende das decisões do administrador do sistema._                                 |
| _/lib_     | _Este diretório armazena as bibliotecas compartilhadas do sistema necessárias para o processo de boot e para executar os comandos na raiz do sistema._                                                                            |
| _/media_   | _Este diretório contem ponto de montagem para dispositivos removíveis tais como CD e DVD ou Pen-Drivers._                                                                                                                         |
| _/mnt_     | _Este diretório é um ponto de montagem para montagem temporária de sistemas de arquivos._                                                                                                                                         |
| /opt       | Este diretório deve contem arquivos estáticos de softwares adicionais.                                                                                                                                                            |
| /proc      | Este é o ponto de montagem para o sistema de arquivos proc, que prove informações sobre processos que estão rodando e kernel. Para mais informações do proc consulte: man 5 proc                                                  |
| /root      | Este diretório é geralmente o diretório home do usuário root.                                                                                                                                                                     |
| /sbin      | Como o /bin, este diretório armazena comandos necessários para o processo de boot do sistema, mais que não são executados pelo usuário comum, somente pelo usuário root.                                                          |
| /srv       | Este diretório contem dados específicos que serão utilizados pelo sistema.                                                                                                                                                        |
| /tmp       | Este diretório contem arquivos temporários que podem ser deletados sem aviso, tais como arquivos de tarefas agendadas ou sistema de inicialização.                                                                                |
| /usr       | Este diretório geralmente é montado em uma partição separada. Ele deve armazenar somente arquivos compartilhados, dados somente leitura, que podem ser montados por varias máquinas rodando Linux como um sistema de boot remoto. |
| /var       | Este diretório contem arquivos variáveis, tais como spool de impressão, e-mail e arquivos de log.                                                                                                                                 |

Podemos obter mais informações a respeito da hierarquia do sistema de arquivos com o seguinte comando.

```bash
root@flownerd:~# man hier
```

# **Tipos de arquivos**

Os tipos de arquivo que se pode encontrar no sistema GNU/Linux são identificados por suas funções dentro do sistema. São eles:

- Diretórios: são arquivos que permitem o armazenamento de outros arquivos em formato de árvore
- Arquivos comuns: são arquivos gerais do sistema, tais como arquivos textos, imagens, entre outros
- Arquivos especiais: são arquivos utilizados para comunicação com dispositivos como discos, portas de entrada e saída, entre outros. A maioria desse arquivos ficam armazenados no /dev
- Links: são arquivos que são utilizados para permitir que um determinado arquivo fique disponível (ou visível) em vários locais do sistema. Um link é como se criar um "atalho" no sistema
- Sockets: são arquivos utilizados para comunicação entre processos executados no S.O. Sockets, na verdade, são pontos de comunicação que permitem que processos se comuniquem de maneira transparente
- Pipes: são arquivos que facilitam a comunicação entre processos dentro do sistema

Essa diferenciação no sistema é verificada por meio de caracteres que identificam os arquivos. A seguir, uma tabela que mostra as identificações possíveis em um sistema.

## **Tabela de tipo de arquivos**

| **_Tipos de arquivos_** | **_Descrição_**                              |
| :---------------------- | :------------------------------------------- |
| _b_                     | _Dispositivo de bloco (Dispositivos físico)_ |
| _c_                     | _Dispositivo orientado a caractere_          |
| _d_                     | _Diretório_                                  |
| _p_                     | _Pipe_                                       |
| _-_                     | _Arquivo regular_                            |
| _l_                     | _Link simbólico_                             |
| _s_                     | _Socket_                                     |

# **O Debian GNU/Linux**

## **Afinal de contas, o que é o Debian?**

O Projeto Debian é uma associação de indivíduos que têm como causa comum criar um sistema operacional livre. O sistema operacional que criamos é chamado Debian GNU/Linux, ou simplesmente Debian.

Um sistema operacional é o conjunto de programas básicos e utilitários que fazem seu computador funcionar. No núcleo do sistema operacional está o kernel. O kernel é o programa mais fundamental no computador e faz todas as operações mais básicas, permitindo que você execute outros programas.

Os sistemas Debian atualmente usam o kernel Linux. O Linux é uma peça de software criada inicialmente por Linus Torvalds com a ajuda de milhares de programadores espalhados por todo o mundo.

No entanto, há trabalho em andamento para fornecer o Debian com outros kernels, primeiramente com o Hurd. O Hurd é um conjunto de servidores que rodam no topo de um micro kernel (como o Mach), os quais implementam diferentes características. O Hurd é software livre produzido pelo projeto GNU.

Uma grande parte das ferramentas básicas que formam o sistema operacional são originadas do projeto GNU; daí os nomes: GNU/Linux e GNU/Hurd. Essas ferramentas também são ferramentas livres.

Claro que o que todos queremos são aplicativos: programas que nos ajudam a conseguir fazer o que desejamos fazer, desde edição de documentos até a administração de negócios, passando por jogos e desenvolvimento de mais software. O Debian vem com mais de 37500 pacotes (softwares pré-compilados e empacotados em um formato amigável, o que faz com que sejam de fácil instalação em sua máquina) — todos eles são livres.

É mais ou menos como uma torre: Na base dela está o kernel. Sobre ele todas as ferramentas básicas e acima estão todos os outros softwares que você executa em seu computador. No topo da torre está o Debian — organizando e arrumando cuidadosamente as coisas, de modo que tudo funcione bem quando todos esses componentes trabalham em conjunto.

## **É tudo realmente livre?**

Você deve estar pensando: porque as pessoas gastam tantas horas de seu tempo para escrever software, empacotá-lo cuidadosamente e então dá-lo? As respostas são tão variadas como as pessoas que contribuem. Algumas pessoas o fazem porque gostam de ajudar outras pessoas. Muitos escrevem programas para aprender mais sobre computadores. Mais e mais pessoas estão procurando maneiras de evitar o preço inflado do software comercial. Uma grande multidão contribui como agradecimento por todo o bom software livre que receberam dos outros. Muitos na universidade criam softwares para fazer com que os resultados de suas pesquisas tenham um maior e melhor uso. Empresas ajudam a manter o software livre para que possam ter uma palavra em como ele se desenvolve -- não há maneira mais rápida de conseguir uma característica do que desenvolvê-la você mesmo. Claro que vários de nós apenas acha isso muito legal!

O Debian é tão compromissado com o software livre que decidimos que seria útil que esse compromisso fosse formalizado em um documento escrito. Assim, nosso Contrato Social nasceu.

Apesar do Debian acreditar no software livre, há casos em que as pessoas querem ou precisam colocar software não-livre em suas máquinas. Sempre que possível, o Debian suportará esses usuários. Há ainda um número crescente de pacotes cujo único trabalho é instalar software não-livre em sistemas Debian.

### **Livre? Mas os CDs ou a banda de rede custam dinheiro.**

Você pode estar perguntando: Se o software é livre (free, em inglês, também significa 'grátis') então por que eu tenho que pagar a um vendedor por um CD ou a um servidor de Internet pela conexão para fazer o download do mesmo?

Quando você compra um CD, está pagando pelo tempo de alguém, pelo investimento para criar os discos e pelo risco (no caso de todos os CDs não serem vendidos). Em outras palavras, você está pagando por uma mídia física usada para entregar o software, não pelo software em si.

Quando usamos a palavra "free", estamos nos referindo a liberdade de software, não a custo zero. Você pode ler mais sobre o que consideramos "software livre" e o que a Free Software Foundation diz sobre o assunto.

## **A maior parte do software custa centenas de dólares americanos. Como vocês podem dá-lo assim?**

Uma pergunta melhor é: Como as empresas de software podem cobrar tanto assim? Desenvolver software não é como fazer um carro. Uma vez feita uma cópia do seu software, os custos de produção para se fazer um mais um milhão de cópias são muito pequenos (essa é uma boa razão para a Microsoft ter bilhões de dólares no banco).

Olhe de outro modo: se você tivesse um suprimento infinito de areia no seu quintal você iria querer dar essa areia. Mesmo assim, seria idiota pagar para um caminhão levá-la para outras pessoas. Você faria com que as outras pessoas viessem buscar sua areia eles mesmos (o que seria equivalente a comprar um CD). Isso é exatamente o que o Debian faz e essa é a razão dos CDs/DVDs serem tão baratos (por volta de USD$ 12 dólares por 4 DVDs).

O Debian não ganha dinheiro vendendo CDs. Mesmo assim, é necessário dinheiro para pagar despesas como registro de domínio e hardware. Assim, pedimos que você compre seus CDs de um dos vendedores de CD que doam uma parte do valor da venda ao projeto Debian.

## **Que hardware é suportado?**

O Debian pode ser executado em quase todos os computadores pessoais, incluindo os mais antigos. Cada novo lançamento do Debian geralmente suporta um número maior de arquiteturas. Para consultar uma lista completa das arquiteturas atualmente suportadas, leia a documentação da distribuição estável.

Quase todo hardware comum é suportado. Se você quer ter certeza de que todos os dispositivos conectados à sua máquina são suportados, confira o Linux Hardware Compatibility HOWTO.

Há algumas companhias que fazem com suportar seu hardware seja difícil, não lançando as especificações para o mesmo. Isso significa que você pode não conseguir usar o hardware produzido por essas empresas com o GNU/Linux. Algumas empresas fornecem um driver não-livre, mas isso é um problema, porque a empresa pode ir à falência ou parar de suportar o hardware que você tem. Recomendamos que você só compre hardware de fabricantes que têm drivers livres para seus produtos.

## **Ainda não estou convencido.**

Não nos dê ouvidos, experimente o Debian você mesmo. Já que o espaço em disco tem se tornado cada vez menos caro, você pode provavelmente dispor de 2GB de espaço em disco. Se você não quer ou não precisa de um desktop gráfico, 600MB são suficientes. O Debian pode facilmente ser instalado nesse espaço extra e coexistir com seu sistema operacional existente. Se você vier a precisar de mais espaço, simplesmente remova um dos seus sistemas operacionais (e depois de ver o poder de um sistema Debian, temos certeza de que não será o Debian o sistema removido).

Experimentar um novo sistema operacional irá tomar uma considerável parte de seu tempo, e você provavelmente não tem muito tempo sobrando. Por essa razão compilamos uma lista de prós e contras do Debian. Isso deve ajudá-lo a decidir se isso tudo vale a pena. Esperamos que você aprecie nossa honestidade e franqueza.

## **Referências**

- Página principal do Debian: https://www.debian.org/index.pt.html
- Sobre o Debian: https://www.debian.org/intro/about.pt
- Por que o Debian: https://www.debian.org/intro/why\_debian.pt.html
- História do Debian: https://www.debian.org/doc/manuals/project-history/
- Ftp Debian Brasil: ftp://ftp.br.debian.org/debian

## **Instalação do Debian**

[Instalação do Debian 11 no VirtualBox](https://youtu.be/s9e-xhCy7hg)

# **CentOS GNU/Linux**

O CentOS, abreviação de Community Enterprise Operating System, é uma distribuição Linux de classe Enterprise derivada de códigos fonte gratuitamente distribuídos pela Red Hat Enterprise Linux e mantida pelo CentOS Project.

A numeração das versões é baseada na numeração do Red Hat Enterprise Linux. Por exemplo, o CentOS 4 é baseado no Red Hat Enterprise Linux 4. A diferença básica entre um e outro é o fornecimento de suporte pago na aquisição de um Red Hat Enterprise Linux. Funcionalmente, pode-se considerar os sistemas clones.

CentOS proporciona um grande acesso aos softwares padrão da indústria, incluindo total compatibilidade com os pacotes de softwares preparados especificamente para os sistemas da Red Hat Enterprise Linux. Isso lhe dá o mesmo nível de segurança e suporte, através de updates, que outras soluções Linux Enterprise, porém sem custo.

Suporta tanto ambientes de servidores para aplicações de missão crítica quanto ambientes de estações de trabalho e ainda possui uma versão Live CD.

CentOS possui numerosas características, incluindo: uma comunidade ativa e crescente, um rápido desenvolvimento e teste de pacotes, uma extensa rede para downloads, desenvolvedores acessíveis, múltiplos canais de suporte incluindo suporte em português e suporte comercial através de parceiros.

No dia 7 de janeiro de 2014 a Red Hat anunciou a incorporação do projeto e comunidade CentOS aos seus portfólio. Segundo anúncio essa incorporação trará benefícios para a comunidade de usuários de ambas as distribuições, gerando maiores inovações nos projetos livres adotados e para toda a arquitetura corporativa.

- Página principal do CentOS: https://www.centos.org/
- Sobre o CentOS: https://www.centos.org/about/
- Mirror: https://www.centos.org/download/mirrors/

## **Instalação do CentOS**

[Instalação do CentOS 8 no VirtualBox](https://youtu.be/YshX-S2JSFg)

# **Começando o uso do sistema GNU/Linux**

## **Acessando o sistema**

Em sistemas GNU/Linux, precisa-se ter em mente o sistema de permissões de acessos que o sistema fornece. Todo sistema Linux possui um gerenciamento de usuários concentrado e garante a segurança do sistema.

Efetuar o login, no Linux, significa fornecer o nome de um usuário pré- cadastrado no sistema, bem como, uma senha para esse usuário. Só assim o sistema fornece acesso a ele, de acordo com a permissão do usuário.

Os usuários são divididos inicialmente em dois níveis de acesso:

- Usuário comum: usuário com acesso restrito aos recursos do sistema, utiliza no prompt de comando o sinal $. Normalmente possui acesso à sua pasta pessoal e à navegação em determinados diretórios do sistema.

Exemplo de login com usuário comum:

```bash
Linux flownerd 5.10.0-8-amd64 #1 SMP Debian 5.10.46-4 (2021-08-03) x86_64

The programs included with the Debian GNU/Linux system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
permitted by applicable law.
Last login: Mon Sep 13 12:01:37 2021 from 192.168.0.101
```

- Usuário root (ou superusuário): usuário com acesso total ao sistema. Conhecido também como "administrador", ele é responsável pelo acesso ao sistema sem restrições e possui sinal # como identificador de prompt.

Exemplo de login com o usuário root.

```bash
Linux flownerd 5.10.0-8-amd64 #1 SMP Debian 5.10.46-4 (2021-08-03) x86_64

The programs included with the Debian GNU/Linux system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
permitted by applicable law.
Last login: Mon Sep 13 11:24:06 2021
root@flownerd:~#
```

### **Login em Console texto**

Após o processo de inicialização do sistema, será mostrado um prompt que pedirá um usuário e uma senha de acesso.

```bash
Debian GNU/Linux 11 flownerd tty1

flownerd login:
```

### **Login Gráfico**

Outra forma de realizar o login no sistema é através do ambiente gráfico, também chamado de 'X'.

## **Terminais Virtuais**

Quando se fala de GNU/Linux, pode-se ter em mente sempre o suporte a multiusuários, ou seja, pode-se logar (efetuar o login) com vários usuários simultaneamente, pois o sistema dá essa possibilidade. Esses logins podem ser realizados através de terminais locais, ambiente gráfico ou até mesmo via rede, com o acesso ao shell remoto (ssh) ou interface gráfica remota.

No caso dos logins em modo texto, serão usadas as teclas de funções Fn para alternar entre esses terminais (consoles).

Note que quando se está em um terminal texto, é apresentado na parte superior da tela, em que terminal se está logado. Na figura a seguir, pode-se ver o login efetuado no terminal 1, chamado de tty1.

```bash
Debian GNU/Linux 11 flownerd tty1

flownerd login:
```

Agora será pressionada a tecla alt + F2. Note que a tela de login permanecerá a mesma, porém, haverá um novo terminal, o tty2, disponível para um novo login.

```bash
Debian GNU/Linux 11 flownerd tty2

flownerd login:
```

Normalmente, a maior parte das distribuições disponibiliza terminais que vão do tty1 ao tty6, totalizando seis terminais textos (consoles).

Seguindo a sequência de terminais, na tecla de função F7 será carregado o primeiro modo gráfico do S.O. Outra opção interessante é poder alternar entre os terminais texto e gráfico.

Se estivermos executando o terminal gráfico podemos alterar para o terminal texto executando ctrl + alt + f1 desta forma vamos para o tty1, se executarmos ctrl + alt + f2 vamos para o tty2 e assim por diante.

Se estivermos executando o terminal texto podemos alterar para o terminal gráfico executando alt + f7.

## **O Comando login**

Esse comando é responsável por carregar um prompt de login sobre o interpretador de comandos que está em execução neste momento. Ele é muito útil quando se está logado como root e se necessita realizar o login com outro usuário, sem fechar a conexão do root.

Veja a seguir um exemplo de uso do comando login a partir de um login real em um prompt.

```bash
root@flownerd:~# login
flownerd login: douglas
Password:
Linux flownerd 5.10.0-8-amd64 #1 SMP Debian 5.10.46-4 (2021-08-03) x86_64

The programs included with the Debian GNU/Linux system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
permitted by applicable law.
Last login: Mon Sep 13 12:04:19 -03 2021 from 192.168.0.101 on pts/0
douglas@flownerd:~$
```

## **O Comando Clear (ctrl+l)**

O clear limpa sua tela, se possível. Ele procura no ambiente pelo tipo de terminal e depois no banco de dados terminfo para saber como limpar a tela.

```bash
root@flownerd:~# clear
```

## **Encerrando o Acesso ao Sistema**

### **O Comando Logout**

Pode-se utilizar o comando logout, na linha de comando, para se desconectar do sistema:

```bash
root@flownerd:~# logout
```

### **O Comando Halt**

Máquinas com o sistema operacional Linux têm como característica a estabilidade constante, não havendo necessidade de desligá-las. Em raros casos, quando se necessite trocar algum periférico ou recompilar um novo Kernel, é necessário reiniciar o S.O. para esses fins. Normalmente a função de desligamento é permitida apenas para o superusuário, porém, nos sistemas mais novos, os usuários comuns também possuem permissão para tal finalidade, dependendo do comando executado.

O comando halt diz ao sistema que ele deverá desligar imediatamente.

```bash
root@flownerd:~# halt
```

#### **Parâmetros do Comando Halt:**

| **_Parâmetro_** | **_Descrição_**                                                          |
| :-------------- | :----------------------------------------------------------------------- |
| _-n_            | _Não sincroniza o sistema de arquivos antes de reiniciar ou parar._      |
| _-f_            | _Força parar ou reiniciar, não chama o shutdown_                         |
| _-i_            | _Apenas desliga todas as interfaces de rede_                             |
| _-h_            | _Coloca dos os drivers do sistema em modo de stand-by e para ou desliga_ |

### **O Comando Reboot**

O comando reboot chama o comando shutdown e, ao final deste, reinicia o sistema.

```bash
root@flownerd:~# reboot
```

#### **Parâmetros do Comando Reboot:**

| **_Parâmetro_** | **_Descrição_**                                                     |
| :-------------- | :------------------------------------------------------------------ |
| _-n_            | _Não sincroniza o sistema de arquivos antes de reiniciar ou parar._ |
| _-f_            | _Força parar ou reiniciar, não chama o shutdown_                    |
| _-i_            | _Apenas desliga todas as interfaces de rede_                        |

### **O Comando Shutdown**

O comando shutdown encerra todos os processamentos.

```bash
root@flownerd:~# shutdown [opções] [-t sec] time [mensagem de alerta]
```

#### **Parâmetros do comando halt**

| **_Parâmetro_** | **_Descrição_**                                                                                       |
| :-------------- | :---------------------------------------------------------------------------------------------------- |
| _-r_            | _Reinicia o sistema depois de parar_                                                                  |
| _-h_            | _Reinicia ou desliga o sistema_                                                                       |
| _-f_            | _Pula a checagem do sistema de arquivos na reinicialização_                                           |
| _-F_            | _Força a checagem do sistema de arquivos na reinicialização_                                          |
| _-t sec_        | _Especifica quantos segundos serão esperados para para executar uma ação de shutdown, halt ou reboot_ |
| _now_           | _Executa o comando imediatamente_                                                                     |

**_Exemplos:_**

Reinicia o máquina no momento

```bash
root@flownerd:~# shutdown -r now
```

Desliga a maquina no momento

```bash
root@flownerd:~# shutdown -h now
```

Manda o sinal de reiniciar a maquina em 60 minutos e informa todos os usuário logados da ação

```bash
root@flownerd:~# shutdown -r 60 "Desligando a maquina em 60 Minutos"
```

### **O Comando Poweroff**

O comando poweroff tem a mesma função do halt, ele serve para paralisar o sistema e desligá-lo:

```bash
root@flownerd:~# poweroff
```

#### **Parâmetros do Comando Poweroff:**

| **_Parâmetro_** | **_Descrição_**                                                     |
| :-------------- | :------------------------------------------------------------------ |
| _-n_            | _Não sincroniza o sistema de arquivos antes de reiniciar ou parar._ |
| _-f_            | _Força parar ou reiniciar, não chama o shutdown_                    |
| _-i_            | _Apenas desliga todas as interfaces de rede_                        |

## **Tempo de Uso e de Acesso ao Sistema**

O administrador de um sistema necessita possuir ferramentas que o mantenham informado sobre os acessos e processos que os usuários executam, para que possa ter controle sobre o sistema e para que esse sistema esteja seguro. Para isso existem os seguintes comandos:

### **O Comando Whoami**

Lista a identificação do usuário que está executando o comando.

```bash
root@flownerd:~# whoami
root
```

### **O Comando Who**

O comando who mostra quais usuários estão logados no sistema, no momento.

```bash
root@flownerd:~# who
root     pts/0        2021-09-13 12:05 (192.168.0.101)
douglas  pts/0        2021-09-13 12:21
```

#### **Parâmetros do Comando who**

| **_Parâmetro_** | **_Descrição_**                             |
| :-------------- | :------------------------------------------ |
| -b              | Horário da última inicialização do sistema  |
| -d              | Mostra os processos mortos                  |
| -H              | Mostra os cabeçalhos                        |
| -l              | Mostra os ttys disponíveis                  |
| --ips           | Mostra endereços ips ao invés de hostnames. |
| -u              | Mostra os usuários logados                  |

Exemplo de utilização do comando who com os cabeçalhos e os usuários logados

```bash
who -Hu
NOME     LINHA        HORÁRIO         OCIOSO        PID COMENTÁRIO
root     pts/0        2021-09-13 12:05   .           649 (192.168.0.101)
douglas  pts/0        2021-09-13 12:21   .           668
```

### **O Comando w**

Mostra quem está acessando o sistema e o que eles estão executando. O w lista as informações sobre os usuários que estão acessando concorrentemente a máquina e seus processos.

O cabeçalho mostra, em ordem, o tempo atual, o tempo que o sistema está ativo, quantos usuários estão acessando o sistema e a média de carga do sistema nos últimos 1, 5 e 15 minutos.

```bash
root@flownerd:~# w
 12:34:47 up  1:10,  2 users,  load average: 0,00, 0,00, 0,00
USUARIO  TTY     DE               LOGIN@   OCIOSO JCPU   PCPU O QUE
root     pts/0    192.168.0.101    12:05    2.00s  0.26s  0.01s w
douglas  pts/0    -                12:21    2.00s  0.26s  0.02s -bash
```

### **O Comando uptime**

Diz há quanto tempo o sistema está funcionando.

O uptime fornece a resposta de uma linha com as seguintes informações: a hora atual, há quanto tempo o sistema está funcionando, quantos usuários estão atualmente usando o sistema e a média de carga no sistema para os últimos 1, 5 e 15 minutos.

Esta é a mesma informação contida no cabeçalho mostrado por **w**.

```bash
root@flownerd:~# uptime
 12:32:41 up  1:08,  2 users,  load average: 0,00, 0,01, 0,00
```

### **O Comando last**

O comando last armazena os últimos logins de cada usuário. O seu conteúdo é armazenado no arquivo: **/var/log/wtmp**. Os dados que são armazenados nesse arquivo e que se consegue visualizar com esse comando são:

- Usuários
- O terminal ou serviço utilizado
- O endereço IP ou o nome da máquina
- Data e Hora
- A duração das sessões

A seguir, pode-se visualizar o resultado do comando last.

```bash
root@flownerd:~# last
douglas  pts/0                         Mon Sep 13 12:21   still logged in
root     pts/0        192.168.0.101    Mon Sep 13 12:05 - 12:21  (00:15)
douglas  pts/0        192.168.0.101    Mon Sep 13 12:04 - 12:05  (00:01)
douglas  pts/0        192.168.0.101    Mon Sep 13 12:01 - 12:01  (00:00)
root     tty1                          Mon Sep 13 11:24 - 12:22  (00:58)
reboot   system boot  5.10.0-8-amd64   Mon Sep 13 11:23   still running
root     tty1                          Mon Sep 13 11:22 - down   (00:01)
root     tty1                          Mon Sep 13 11:22 - 11:22  (00:00)
douglas  tty1                          Mon Sep 13 11:21 - 11:21  (00:00)
root     tty1                          Mon Sep 13 11:21 - 11:21  (00:00)
reboot   system boot  5.10.0-8-amd64   Mon Sep 13 11:21 - 11:23  (00:02)
root     tty1                          Sun Sep 12 15:38 - down   (00:00)
reboot   system boot  5.10.0-8-amd64   Sun Sep 12 15:38 - 15:38  (00:00)
root     tty1                          Sun Sep 12 15:36 - down   (00:00)
reboot   system boot  5.10.0-8-amd64   Sun Sep 12 15:36 - 15:37  (00:00)
douglas  tty1                          Sun Sep 12 15:23 - down   (00:06)
reboot   system boot  5.10.0-8-amd64   Sun Sep 12 15:21 - 15:29  (00:08)
douglas  tty1                          Sun Sep 12 13:31 - crash  (01:50)
root     tty1                          Sun Sep 12 13:30 - 13:31  (00:00)
reboot   system boot  5.10.0-8-amd64   Sun Sep 12 13:30 - 15:29  (01:59)

wtmp inicia Sun Sep 12 13:30:38 2021
```

### **O Comando lastlog**

Lastlog armazena quando o usuário logou pela última vez, o seu conteúdo é armazenado no arquivo: **/var/log/lastlog**. A seguir, veja um exemplo do comando lastlog.

```bash
root@flownerd:~# lastlog
Nome de Usuário         Porta     De             Último
root             pts/0    192.168.0.101    seg set 13 12:05:55 -0300 2021
daemon                                     **Nunca logou**
bin                                        **Nunca logou**
sys                                        **Nunca logou**
sync                                       **Nunca logou**
games                                      **Nunca logou**
man                                        **Nunca logou**
lp                                         **Nunca logou**
mail                                       **Nunca logou**
news                                       **Nunca logou**
uucp                                       **Nunca logou**
proxy                                      **Nunca logou**
www-data                                   **Nunca logou**
backup                                     **Nunca logou**
list                                       **Nunca logou**
irc                                        **Nunca logou**
gnats                                      **Nunca logou**
nobody                                     **Nunca logou**
_apt                                       **Nunca logou**
systemd-timesync                           **Nunca logou**
systemd-network                            **Nunca logou**
systemd-resolve                            **Nunca logou**
messagebus                                 **Nunca logou**
avahi-autoipd                              **Nunca logou**
sshd                                       **Nunca logou**
douglas          pts/0                     seg set 13 12:21:11 -0300 2021
systemd-coredump                           **Nunca logou**
```

### **O Comando lastb**

Lastb armazena as tentativas de login mal sucessidadas que em alguns casos podem identificar uma tentativa de invasão, o seu conteúdo é armazenado no arquivo: **/var/log/btmp**. A seguir, veja um exemplo do comando lastb.

```bash
root@flownerd:~# lastb
douglas  ssh:notty    192.168.0.101    Mon Sep 13 12:01 - 12:01  (00:00)

btmp inicia Mon Sep 13 12:01:24 2021
```

# **Primeiros comandos e documentações**

## **Navegando e Manipulando o Sistema de Arquivos**

### **O Comando Ls**

Este comando lista informações sobre os arquivos e diretórios.

Vamos ver o exemplo do comando ls

```bash
root@flownerd:~# ls /
bin   dev  home        initrd.img.old  lib32  libx32	  media  opt   root  sbin  sys	usr  vmlinuz
boot  etc  initrd.img  lib	       lib64  lost+found  mnt	 proc  run   srv   tmp	var  vmlinuz.old
```

Este comando ls tem muitas opções vamos destacar algumas abaixo:

#### **Parâmetros do Comando ls**

| **_Parâmetro_** | **_Descrição_**                                                                                                   |
| :-------------- | :---------------------------------------------------------------------------------------------------------------- |
| _-a_            | _Lista todas as entradas no diretório e arquivos ocultos_                                                         |
| _-B_            | _Não lista arquivos que terminem com ~ que são arquivos de backup automático_                                     |
| _--color_       | _Mostra a saída do comando com cores diferenciando os tipos de arquivos, opções podem ser: always, never ou auto_ |
| _-d_            | _Lista os diretórios ao invés de seus conteúdos_                                                                  |
| _-F_            | \*Adiciona indicadores de tipo podem ser (\*/=>@) para as entradas\*                                              |
| _-g_            | _Igualmente a opção de -l porém não lista o usuário dono_                                                         |
| _-G_            | _Com a opção -l para não listar o grupo dono_                                                                     |
| _-h_            | _Com a opção -l mostra o tamanho em formato (K,M,G,T)_                                                            |
| _-i_            | _Mostra o inode do arquivo_                                                                                       |
| _-l_            | _Mostra a saída em formato de lista longa_                                                                        |
| _-n_            | _Igualmente a opção -l mas mostra a saída em formato numérico para usuários e grupos_                             |
| _-Q_            | _Mostra a saída entre aspas duplas ""_                                                                            |
| _-r_            | _Inverte a ordem da listagem_                                                                                     |
| _-R_            | _Faz a listagem recursiva_                                                                                        |
| _-S_            | _Com a opção -l ordena pelo tamanho dos arquivos_                                                                 |
| _-t_            | _Ordena pela data de modificação, o mais novo primeiro_                                                           |
| _-x_            | _Lista as entradas por linhas ao invés de colunas_                                                                |
| _-X_            | _Com a opção -l ordena de forma alfabética por tipo de extensão_                                                  |
| _-Z_            | _Com a opção -l mostra as entradas SELinux para cada arquivo_                                                     |
| _-1_            | _Lista um arquivo por linha_                                                                                      |

Nós podemos fazer a utilização do comando ls com múltiplas opções por exemplo: Uma listagem dos arquivos do diretório /root mostrando os arquivos ocultos e ordenando de forma reversa pode ser efetuada da seguinte forma

```bash
root@flownerd:~# ls -lar /root
total 20
-rw-r--r--  1 root root  161 jul  9  2019 .profile
-rw-r--r--  1 root root  571 abr 10 17:00 .bashrc
-rw-------  1 root root  254 set 13 14:25 .bash_history
drwxr-xr-x 18 root root 4096 set 12 13:24 ..
drwx------  2 root root 4096 set 12 13:31 .
```

### **Metacaracteres (caracteres coringas)**

Os metacaracteres são caracteres que possuem uma propriedade especial no interpretador de comandos. Além disso, eles são utilizados para facilitar o emprego dos comandos no Linux, principalmente quando se trabalha com a manipulação de arquivos.

#### **O caractere "?"**

Quando um nome de arquivo é esperado, ele casa com um caractere qualquer, ou seja, a ? representa um único e qualquer caractere no nome de um arquivo. Por exemplo:

Primeiramente serão criados alguns arquivos como modelo para que se possa analisar o resultado do uso da "?".

```bash
root@flownerd:~# touch flownerd.txt flownerd1.txt flownerd2.txt
```

Agora serão usados os metacaracteres para filtrar a listagem dos arquivos "flownerd" que foram criados.

```bash
root@flownerd:~# ls -l flownerd?.txt
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd1.txt
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd2.txt
```

#### **O Caractere \* (asterisco)**

Este é um caractere coringa que substitui qualquer caractere referenciado, não importando a quantidade de vezes de substituições, diferente do "?", que substitui apenas um único caractere.

**_Exemplo:_**

```bash
root@flownerd:~# ls -l flownerd*.txt
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd1.txt
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd2.txt
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd.txt
```

Vamos listar todos os arquivos que comecem com flownerd

```bash
root@flownerd:~# ls -l flownerd.*
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd.txt
```

Agora vamos ver um exemplo combinando os caracteres especiais

```bash
root@flownerd:~# ls -l flownerd?.*
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd1.txt
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd2.txt
```

Com esses metacaracteres pode-se, filtrar vários resultados no sistema, a fim de manipular os nossos comandos.

### **O Comando cd**

Para entrar e sair de diretórios, podemos fazer a utilização do comando cd.

Para entramos no diretório /etc podemos executar o seguinte comando

```bash
root@flownerd:~# cd /etc
```

Para voltar um diretório podemos executar o seguinte comando

```bash
root@flownerd:/etc# cd ..
```

Agora se precisar voltar para o diretório anteriormente acessado podemos utilizar o seguinte comando

```bash
root@flownerd:~# cd -
```

Se precisar acessar o diretório home do usuário atualmente logado podemos utilizar o seguinte comando

```bash
root@flownerd:~# cd ~
```

### **O Comando pwd**

Para saber em que nível hierárquico de diretório estamos, basta usar o comando pwd que vai nos retornar em qual diretório estamos.

```bash
root@flownerd:~# pwd
/root
```

### **O Comando mkdir**

Para criar diretórios podemos utilizar o comando mkdir como abaixo

```bash
root@flownerd:~# mkdir flownerd
```

Se precisar criar um diretório e um subdiretório de uma vez podemos utilizar a opção -p que vai criar os diretórios dependentes

```bash
root@flownerd:~# mkdir -p /aula/flownerd/fundamentos
```

Agora por exemplo se precisarmos criar um diretório que o seu nome contenha espaço podemos utilizar as aspas "" para efetuar a criação da seguinte forma

```bash
root@flownerd:~# mkdir -p "meu diretorio"
```

### **O Comando touch**

O comando touch pode ser utilizado para criar um arquivo vazio, porem ele é utilizado para alterar o timestamps do arquivo, ou seja ele atualiza a hora de acesso e modificação do arquivo.

Por exemplo para criarmos um arquivo vazio podemos utilizar o touch da seguinte forma:

```bash
root@flownerd:~# touch flownerd.doc
```

Agora vamos listar o arquivo para verificarmos as suas propriedades

```bash
root@flownerd:~# ls -l
total 0
-rw-r--r-- 1 root root 0 set 13 23:44 flownerd.doc
```

Note que o nosso arquivo tem tamanho 0 e a data de criação é 8 de junho as 12:26. Agora se eu executar o touch neste arquivo vai ser atualizada a data de acesso dele, vamos testar

```bash
root@flownerd:~# touch flownerd.doc
```

Agora se eu listar o arquivo novamente vou ter outra hora de acesso

```bash
root@flownerd:~# ls -l
total 0
-rw-r--r-- 1 root root 0 set 13 23:45 flownerd.doc
```

### **O comando cp**

O comando cp é utilizado para copiar de uma origem para um destino podendo ser um arquivo ou diretório ou podemos copiar múltiplas origem para um destino também.

Vamos a um exemplo vamos copiar o arquivo /etc/resolv.conf para o diretório /srv

```bash
root@flownerd:~# cp /etc/resolv.conf /srv
```

Vamos listar o /srv para verificar a nossa copia

```bash
root@flownerd:~# ls -l /srv
total 4
-rw-r--r-- 1 root root 60 set 13 23:45 resolv.conf
```

Agora se eu precisar dois ou mais arquivos de uma única vez eu posso fazer da seguinte forma

```bash
root@flownerd:~# cp /etc/network/interfaces /etc/motd /srv
```

Agora vamos listar o /srv para verificarmos a nossa copia

```bash
root@flownerd:~# ls -l /srv/
total 12
-rw-r--r-- 1 root root 498 set 13 23:46 interfaces
-rw-r--r-- 1 root root 286 set 13 23:46 motd
-rw-r--r-- 1 root root  60 set 13 23:45 resolv.conf
```

Note que os nosso arquivos estão lá.

Agora se eu precisar copiar um diretório e todo o seu conteúdo eu preciso passar a opção -r que orienta o cp a copiar o diretório e todo o seu conteúdo de forma recursiva

Vamos a um exemplo

```bash
root@flownerd:~# cp -r /etc/network /srv
```

Aqui copiamos o nosso diretório /etc/network para o diretório /srv, vamos listar a nossa copia

```bash
root@flownerd:~# ls -l /srv/
total 16
-rw-r--r-- 1 root root  498 set 13 23:46 interfaces
-rw-r--r-- 1 root root  286 set 13 23:46 motd
drwxr-xr-x 7 root root 4096 set 13 23:47 network
-rw-r--r-- 1 root root   60 set 13 23:45 resolv.conf
```

#### **Parâmetros do Comando cp:**

| **_Parâmetro_** | **_Descrição_**                                                                               |
| :-------------- | :-------------------------------------------------------------------------------------------- |
| _-a_            | _Copia os arquivos ou diretórios preservando as permissões e links_                           |
| _-f_            | _Sobrescreve arquivos ou diretórios sem perguntar_                                            |
| _-i_            | _Utiliza o modo interativo perguntando se deseja ou não sobrescrever um diretório ou arquivo_ |
| _-p_            | _Preserva permissões e data de criação_                                                       |
| _-R ou -r_      | _Copia os diretórios de forma recursiva_                                                      |

### **O comando mv**

O comando mv é utilizado para mover ou renomear de uma origem para um destino ou podemos copiar múltiplas origem para um destino também.

```bash
root@flownerd:~# mv flownerd.txt flownerd.old
```

Podemos também copiar múltiplos arquivos para um diretório vamos ver o exemplo abaixo:

```bash
root@flownerd:~# mv flownerd*.* /srv
```

Agora vamos listar os nossos arquivos no diretório /srv

```bash
root@flownerd:~# ls -l /srv/
total 16
-rw-r--r-- 1 root root    0 set 13 23:45 flownerd.doc
-rw-r--r-- 1 root root    0 set 13 23:49 flownerd.old
-rw-r--r-- 1 root root  498 set 13 23:46 interfaces
-rw-r--r-- 1 root root  286 set 13 23:46 motd
drwxr-xr-x 7 root root 4096 set 13 23:47 network
-rw-r--r-- 1 root root   60 set 13 23:45 resolv.conf
```

#### **Parâmetros do Comando mv:**

| **_Parâmetro_** | **_Descrição_**                                                                               |
| :-------------- | :-------------------------------------------------------------------------------------------- |
| _-f_            | _Sobrescreve arquivos ou diretórios sem perguntar_                                            |
| _-i_            | _Utiliza o modo interativo perguntando se deseja ou não sobrescrever um diretório ou arquivo_ |
| _-u_            | _Move somente quando a origem é mais nova que no destino_                                     |

### **O comando rm**

O comando rm é utilizado para remover arquivos ou diretório, porém não padrão o rm não remove diretórios por padrão precisamos especificar esta ação.

```bash
root@flownerd:~# rm /srv/resolv.conf
```

Agora vamos listar o diretório para checarmos se o arquivo foi ou não deletado.

```bash
root@flownerd:~# ls -l /srv
total 12
-rw-r--r-- 1 root root    0 set 13 23:45 flownerd.doc
-rw-r--r-- 1 root root    0 set 13 23:49 flownerd.old
-rw-r--r-- 1 root root  498 set 13 23:46 interfaces
-rw-r--r-- 1 root root  286 set 13 23:46 motd
drwxr-xr-x 7 root root 4096 set 13 23:47 network
```

Note que não existe mais o arquivo resolv.conf no diretório /srv, agora vamos mandar remover o diretório network que está no diretório /srv

```bash
root@flownerd:~# rm /srv/network
rm: não foi possível remover '/srv/network': É um diretório
```

Note que não podemos remover o diretório /srv/network pois não passamos o parâmetro para remover diretórios

Vamos passar o parâmetro -r agora para remover o diretório

```bash
root@flownerd:~# rm -r /srv/network
```

Agora vamos listar o diretório para checarmos se o diretório foi ou não removido

```bash
root@flownerd:~# ls -l /srv/
total 8
-rw-r--r-- 1 root root   0 set 13 23:45 flownerd.doc
-rw-r--r-- 1 root root   0 set 13 23:49 flownerd.old
-rw-r--r-- 1 root root 498 set 13 23:46 interfaces
-rw-r--r-- 1 root root 286 set 13 23:46 motd
```

Como podemos notar não existe mais o diretório network em /srv

#### **Parâmetros do Comando rm**

| **_Parâmetro_** | **_Descrição_**                                                                               |
| :-------------- | :-------------------------------------------------------------------------------------------- |
| _-f_            | _Sobrescreve arquivos ou diretórios sem perguntar_                                            |
| _-i_            | _Utiliza o modo interativo perguntando se deseja ou não sobrescrever um diretório ou arquivo_ |
| _-r ou -R_      | _Remove diretório(s) e seu(s) conteúdo(s) recursivamente_                                     |

**\*OBS:** O comando rm -rf pode ser fatal para o sistema quando executado de maneira errada, pois podemos remover o sistema inteiro\*

### **O comando rmdir**

O comando rmdir é utilizado para remover diretório(s) vazio(s).

Vamos efetuar um teste vamos criar o diretório /etc/network para o /srv

```bash
root@flownerd:~# cp -r /etc/network /srv
```

Agora vamos tentar remover ele com o rmdir

```bash
root@flownerd:~# rmdir /srv/network
rmdir: falhou em remover '/srv/network': Arquivo ou diretório inexistente
```

Note que não conseguimos remover porque o diretório não esta vazio, vamos fazer mais um teste. Vamos criar um diretório vazio

```bash
root@flownerd:~# mkdir /srv/empty
```

Agora vamos tentar remover ele

```bash
root@flownerd:~# rmdir /srv/empty
```

Note que agora não recebemos nenhum aviso, vamos checar no /srv se o diretório foi removido.

```bash
root@flownerd:~# ls -l /srv/
total 8
-rw-r--r-- 1 root root   0 set 13 23:45 flownerd.doc
-rw-r--r-- 1 root root   0 set 13 23:49 flownerd.old
-rw-r--r-- 1 root root 498 set 13 23:46 interfaces
-rw-r--r-- 1 root root 286 set 13 23:46 motd
```

Nos podemos remover um arvore de diretórios vazia por exemplo, vamos testar vamos criar 3 diretórios em sequencia.

```bash
root@flownerd:~# mkdir -p a/b/c
```

Vamos listar o diretório a para verificar o seu conteúdo

```bash
root@flownerd:~# ls -lR a
a:
total 4
drwxr-xr-x 3 root root 4096 set 14 09:48 b

a/b:
total 4
drwxr-xr-x 2 root root 4096 set 14 09:48 c

a/b/c:
total 0
```

Agora vamos remover eles de uma vez

```bash
root@flownerd:~# rmdir -p a/b/c
```

Como podemos notar não tivermos nenhum erro de retorno.

### **O comando file**

O comando file determina o tipo de arquivo, pois podemos ter um arquivo com a extensão .txt sendo um arquivo .mp3 ou o inverso vamos a um exemplo, vamos criar um arquivo chamado tocar.mp3

```bash
root@flownerd:~# touch tocar.mp3
```

Agora vamos listar o nosso arquivo

```bash
root@flownerd:~# ls -l tocar.mp3
-rw-r--r-- 1 root root 0 set 14 09:49 tocar.mp3
```

Note que a única informação que temos é que o nosso arquivo é regular pelo caractere identificar "-"

Agora vamos checar ele com o comando file

```bash
root@flownerd:~# file tocar.mp3
tocar.mp3: empty
```

Como podemos notar o file identificou o nosso arquivo como sendo um arquivo vazio, vamos checar um arquivo binário por exemplo para verificar o resultado

Vamos listar o arquivo /bin/bash

```bash
root@flownerd:~#  ls -l /bin/bash
-rwxr-xr-x 1 root root 1234376 ago  4 17:25 /bin/bash
```

Note que a única informação que temos é que o nosso arquivo é regular como o tocar.mp3, agora vamos verificar o nosso arquivo com o comando file.

```bash
root@flownerd:~# file /bin/bash
/bin/bash: ELF 64-bit LSB pie executable, x86-64, version 1 (SYSV), dynamically linked, interpreter /lib64/ld-linux-x86-64.so.2, BuildID[sha1]=3313b4cb119dcce16927a9b6cc61dcd97dfc4d59, for GNU/Linux 3.2.0, stripped
```

Note que o resultado é diferente, pois temos um arquivo binário

Vamos checar outro arquivo o /etc/passwd por exemplo que é outro arquivo regular.

```bash
root@flownerd:~# file /etc/passwd
/etc/passwd: ASCII text
```

### **O comando type**

O comando type é utilizado para encontrar a localização de um comando ou se um arquivo é um comando interno.

Vamos checar o comando passwd

```bash
root@flownerd:~# type passwd
passwd é /usr/bin/passwd
```

Note que temos a localização do comando passwd que é /usr/bin/passwd

Vamos checar o comando cd que é o comando para entrar ou sair de um diretório.

```bash
root@flownerd:~# type cd
cd é um comando interno do shell
```

## **Ligações (Links)**

Links são pseudo-arquivos que apontam para um arquivo real. O conceito pode parecer um pouco estranho, a princípio, mas os links são úteis e muito utilizados no Linux.

Existem dois tipos de links, os soft links e os hard links.

### **Soft Links**

Links simbólicos são atalhos que apontam para um arquivo. Um link simbólico pode apontar para um arquivo em qualquer lugar, seja na mesma partição, em outra ou até em locais remotos, como NFS, por exemplo.

Por ser um arquivo, um link simbólico ocupa espaço em disco.

Para identificar um link simbólico, pode-se executar o comando ls -l no diretório onde ele se encontra. Os links simbólicos são identificados pela letra "l" à esquerda da lista de permissões e não as contêm, na verdade. As permissões do arquivo real é que são utilizadas. Se o arquivo real for apagado, o link simbólico vira um "link morto" (dead link), ou seja, aponta para um local que não existe.

Para criarmos um link simbólico devemos utilizar o comando ln, vamos a alguns exemplos.

Vamos fazer um link do arquivo /etc/passwd para o /srv/passwd

```bash
root@flownerd:~# ln -s /etc/passwd /srv/passwd
```

Agora vamos listar o diretório /srv para checarmos o seu conteúdo

```bash
root@flownerd:~# ls -l /srv
total 8
drwxr-xr-x 2 root root 4096 set 14 13:47 flownerd
-rw-r--r-- 1 root root    0 set 14 14:04 flownerd10.txt
-rw-r--r-- 1 root root    0 set 14 13:56 flownerd1.txt
-rw-r--r-- 1 root root    0 set 14 13:54 flownerd2.txt
-rw-r--r-- 1 root root    0 set 14 13:53 flownerd.doc
-rw-r--r-- 1 root root    0 set 14 13:40 flownerd.txt
lrwxrwxrwx 1 root root   11 set 14 17:33 passwd -> /etc/passwd
-rw-r--r-- 1 root root   60 set 14 13:56 resolv.conf
-rw-r--r-- 1 root root    0 set 14 09:49 tocar.mp3
```

Note que o último arquivo tem uma flecha → apontando para o arquivo original que esta localizado em /etc/passwd, podemos notar também. que o caractere que identifica o arquivo é um l identificando que temos um link simbólico.

Vamos listar outro link simbólico padrão do sistema Debian.

```bash
root@flownerd:~# ls -l /vmlinuz
lrwxrwxrwx 1 root root 27 set 12 13:24 /vmlinuz -> boot/vmlinuz-5.10.0-8-amd64
```

Note que é um link simbólico apontando para a imagem do kernel no sistema.

Em nosso sistema temos muitos links para facilitar o acesso a algumas informações.

### **Hard Link**

Hard links, na verdade, não são links, apenas nova referência ao arquivo armazenado no sistema de arquivos. As duas entradas contêm nomes diferentes, mas apontam para o mesmo local físico no disco (inode) compartilhando, portanto, além do mesmo conteúdo, os dois arquivos terão as mesmas permissões, ou seja, os dois arquivos são o mesmo, porém, com nomes diferente. Se o arquivo verdadeiro for apagado, o hard link continua apontando para o mesmo local físico sendo acessível da mesma forma.

O hard link possui duas limitações. São elas:

- O arquivo original e o hard link devem, obrigatoriamente, estar localizados no mesmo sistema de arquivos, já que o hard link aponta para um endereço físico (inode) e não se pode garantir que estes endereços sejam únicos em vários sistemas de arquivos. Imagine, por exemplo, um arquivo localizado no inode 50, no sistema de arquivos sda5. Não se pode garantir que em outro sistema de arquivos, sda8 por exemplo, não haja um outro arquivo com número de inode 50.
- A outra limitação é que um hard link não pode apontar para um diretório. Hard links não ocupam espaço no sistema de arquivos.

Vamos verificar como efetuamos a criação de um hard link, no exemplo abaixo.

Primeiro vamos verificar o inode do arquivo /etc/passwd pois vamos criar um hard link dele

```bash
root@flownerd:~# ls -li /etc/passwd
4895428 -rw-r--r--. 1 root root 1048 set 12 15:03 /etc/passwd
```

Note que o inode do nosso arquivo é 4895428, o nosso hard link vai ter que ter o mesmo inode. Vamos criar o nosso hard link

```bash
root@flownerd:~# ln /etc/passwd /passwd
```

Agora vamos listar o nosso hard link

```bash
root@flownerd:~# ls -li /passwd
4895428 -rw-r--r-- 2 root root 1099 Jun 8 09:34 /passwd
```

Note que o nosso hard link tem o mesmo inode o arquivo original e o caractere identificar de arquivo continua o mesmo "-" .

## **Documentação**

Uma das características mais interessantes e importantes do Linux é a existência de grande quantidade de documentos que possibilitam ao usuário conhecer o sistema. Um fator importante no estudo do sistema é saber que tipo de documentos existem, além de conhecer as várias fontes de documentação disponíveis na Internet.

### **O Comando man**

Os manuais do Linux seguem determinados padrões e costumam ser armazenados no disco rígido, podendo ser acessados pelo comando man, que formata e permite a visualização das páginas do manual on-line. Esta versão reconhece as variáveis de ambiente MANPATH e (MAN)PAGER, o que possibilita a personalização do conjunto de páginas e até do formato das páginas. No caso de existir uma especificação de seção pelo usuário, será exibida apenas a página correspondente. Caso o nome contenha uma "barra" (/), então ele será testado como se fosse um nome de arquivo, podendo-se utilizar man ./cnc.5 ou mesmo man /cd/foo/bar.1.gz. O man tentará salvar as páginas do manual que tenham sido formatadas, buscando reduzir o tempo excluindo a formatação das páginas, na próxima vez que o comando for acionado.

As páginas do manual-padrão do Linux estão disponíveis localmente no sistema, conforme relacionadas abaixo:

- Comandos do usuário
- Chamadas ao sistema
- Bibliotecas de funções
- Dispositivos
- Formatos de arquivos
- Jogos
- Informações gerais
- Administração do sistema

Tradicionalmente, versões formatadas das páginas no diretório de origem especificado em /etc/man.config são salvas no arquivo específico, no diretório de destino também especificado por ele, mas outros mapeamentos dos diretórios contendo manuais podem ser especificados em /etc/man.config. Isto indica que, obviamente, nenhuma página formatada poderá ser salva no caso da inexistência de um diretório especificado por ele.

Por exemplo para visualizarmos as páginas de manuais para o comando ls podemos executar o seguinte comando

```bash
root@flownerd:~# man ls
```

Para sair do manual basta pressionar a tecla q

#### **Opções do comando man**

| **_Parâmetro_** | **_Descrição_**                                                                                                                                                                                                                                           |
| :-------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _-C_            | _Especifica o arquivo de configuração de deve ser utilizado_                                                                                                                                                                                              |
| _-f_            | _Pesquisa por uma determinada página de manual_                                                                                                                                                                                                           |
| _-M_            | _Especifica a lista de diretórios a serem pesquisados na busca pelas páginas de manual, ignorando a variável de ambiente MANPATH._                                                                                                                        |
| _-P paginador_  | _Especifica qual paginador será usado, ignorando o paginador-padrão._                                                                                                                                                                                     |
| _-a_            | _Por padrão, o man encerrará após apresentar a primeira página de manual encontrada. Ao utilizar a opção -a_                                                                                                                                              |
| _-c_            | _Reformata a página fonte de manual, mesmo existindo uma versão já formatada. Isso ajudará principalmente quando a página for formatada para uma tela com um número diferente de colunas ou se uma página pré-formatada estiver eventualmente corrompida_ |
| _-m sistema_    | _Especifica um conjunto alternativo de páginas de manual a serem pesquisadas através do nome de sistema especificado._                                                                                                                                    |
| _-W_            | _Lista apenas um nome de arquivo por linha, sem qualquer informação adicional. Esta opção é útil em comando do shell, tais como man -aW man xargs ls -l_                                                                                                  |

Observe que a opção -c força a reformatação da página, mesmo que uma outra página recente esteja disponível. Conclui-se, então, que o man é uma ferramenta poderosa e expande as possibilidades do usuário de desenvolver sozinho suas pesquisas, bastando conhecer um mínimo de opções.

### **O Comando whatis**

O comando whatis procura por nome de páginas de manuais e mostra a página de manual e a sua descrição para cada combinação encontrada.

```bash
root@flownerd:~# whatis passwd
passwd (5)           - arquivo de senhas
passwd (1)           - change user password
passwd (1ssl)        - compute password hashes
```

Note que tivemos o retorno de 3 páginas de manual com um número entre parênteses este número é a sessão do man, para chamar o manual para a ultima linha do nossa saída podemos executar o seguinte comando

```bash
root@flownerd:~# man 1ssl passwd
```

### **O Comando help e info**

Os comando help e info são ferramentas auxiliares para pesquisas locais, sem a estrutura do comando man, mas bastante interessantes e com resultados satisfatórios em pesquisas mais manuais.

O comando help mostra os comandos internos do shell bash. Para acessar os comandos do help e suas variáveis podemos digitar na linha de comando help como abaixo

```bash
root@flownerd:~# help
```

Temos da mesma forma o comando info que temos uma descri ação sobre os comandos que ele da suporte, o comando info é mais explicativo para chamarmos o info podemo digitar na linha de comando info como abaixo.

```bash
root@flownerd:~# info
```

### **As opções -h e --help dos comando**

A maioria dos comando tem suporte as opção -h ou --help que traz um help rápido a respeito do nosso comando, vamos pegar o exemplo do comando rm.

```bash
root@flownerd:~# rm --help
Uso: rm [OPÇÃO]... [ARQUIVO]...
Remove (desvincula) o(s) ARQUIVO(s).

  -f, --force           ignora arquivos e argumentos inexistentes,
                          nunca questiona
  -i                    questiona antes de cada remoção
  -I                    questiona uma vez antes de remover mais que três
                          arquivos ou ao remover recursivamente;
                          menos intrusivo que -i, mas ainda oferecendo alguma
                          proteção contra a maioria dos equívocos
      --interactive[=QUANDO]
[...]
```

Como podemos notar temos uma ajuda sobre como o comando funciona e suas opções.

### **O comando apropos**

O comando apropos faz uma pesquisa nas paginas de manuais pela palavra-chave que é passada para ele, o apropos pode pesquisar tanto por um comando como em sua descrição, vamos a um exemplo abaixo

Vamos pesquisar pela palavra compiler

```bash
root@flownerd:~# apropos compiler
tic (1)              - the terminfo entry-description compiler
xsubpp (1)           - compiler to convert Perl XS code into C code
zic (8)              - timezone compiler
```

Aqui temos o retorno de todos os comandos que tem referencias a palavra compiler, agora para chamar o manual basta digitar o man número da sessão e o comando exemplo.

```bash
root@flownerd:~# man 1 tic
```

### **Outras fontes de Documentação**

Indiscutivelmente, a Internet foi e ainda é o principal meio de popularização e desenvolvimento do Linux, e é na Internet que os projetos, as informações e as atualizações estão disponíveis imediatamente à sua evolução. Um dos principais expoentes desta tendência é o LDP (Linux Documentation Project), projeto que trabalha em torno de um desenvolvimento de documentação de alta qualidade, com as características do conceito de software livre. A colaboração e a pesquisa no desenvolvimento e tradução de guias e HOWTOs, páginas dos manuais, etc., não só com o intuito de desenvolver o projeto, mas facilitar a sua disponibilização, faz com que a consulta dos vários temas relacionados possa se tornar cada vez mais dinâmica.

### **Referências para Documentação na Internet**

- Foca Linux: http://www.guiafoca.org/
- BR-Linux: http://www.br-linux.org/
- Dicas-L: http://www.dicas-l.com.br/
- Linux Documentation Project: http://tldp.org/
- Viva o Linux: http://www.vivaolinux.com.br
- Wiki do Kernel: https://www.wiki.kernel.org/

## **Localizando arquivos**

### **O comando find**

O comando find pesquisa a árvore de diretórios com raiz dada pelo nome do arquivo fornecido para avaliação, através de uma expressão avaliada da esquerda para a direita, de acordo com as regras de precedência até que o resultado seja conhecido e, neste ponto, o find vai para o próximo nome de arquivo.

**_Sintaxe:_**

```bash
root@flownerd:~# find [diretório de pesquisa] [parametros] [arquivos]
```

#### **Parâmetros do Comando find**

| _Parâmetro_        | _Descrição_                                                                                                                                           |
| :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------- |
| _-maxdepth levels_ | _Aqui nos limitamos a nossa pesquisa a quantidade máxima de níveis de diretórios que vamos efetuar a pesquisa._                                       |
| _-noleaf_          | _Não utiliza otimização na pesquisa, está opção é necessário quando efetuamos pesquisas em CD/DVD ou pesquisas em sistemas de arquivos MS-DOS ou AFS_ |
| _-regextype type_  | _Utiliza uma expressão regular para efetuar a pesquisa_                                                                                               |
| _-xdev_            | _Não efetua pesquisa em outros sistemas de arquivos._                                                                                                 |

| _-amin n_          | _Pesquisa arquivos que foram acessados nos n últimos minutos atras._                                                                                                                                                                                                                                                                                                                                         |
| :----------------- | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _-atime n_         | _Pesquisa arquivos que foram acessados nas últimas n\*24 horas atras. Por exemplo se especificar uma pesquisa utilizando -atime +1 vamos procurar arquivos que foram acessados pelo menos 2 dias atras._                                                                                                                                                                                                     |
| _-cmin n_          | _Pesquisa arquivos que o status do arquivo foi modificado nos últimos n minutos atras._                                                                                                                                                                                                                                                                                                                      |
| _-ctime n_         | _Pesquisa arquivos que o status do arquivo foi modificado nas últimas n horas atras._                                                                                                                                                                                                                                                                                                                        |
| _-empty_           | _Pesquisa arquivos que estão vazios ou são um arquivos regulares ou um diretórios._                                                                                                                                                                                                                                                                                                                          |
| _-executable_      | _Pesquisa arquivos executáveis e diretórios que podem ser pesquisados._                                                                                                                                                                                                                                                                                                                                      |
| _-gid n_           | _Pesquisa arquivos que o gid é n_                                                                                                                                                                                                                                                                                                                                                                            |
| _-group gname_     | _Pesquisa arquivos que pertencem ao grupo gname_                                                                                                                                                                                                                                                                                                                                                             |
| _-iname pattern_   | _Efetua a pesquisa por pattern porem não diferencia maiúsculas e minusculas._                                                                                                                                                                                                                                                                                                                                |
| _-inum n_          | _Pesquisa por arquivos que tenham o inode n_                                                                                                                                                                                                                                                                                                                                                                 |
| _-mmin n_          | _Pesquisa arquivos que foram modificado nos n últimos minutos atras._                                                                                                                                                                                                                                                                                                                                        |
| _-mtime n_         | _Pesquisa arquivos que foram modificados nas n últimas horas atras._                                                                                                                                                                                                                                                                                                                                         |
| _-name pattern_    | _Pesquisa arquivos baseados no padrão informado, Os metacaracteres ('\*', '?' e '[]') podem ser utilizados._                                                                                                                                                                                                                                                                                                 |
| _-nogroup gid_     | _Pesquisa arquivos que não tenham o gid informado_                                                                                                                                                                                                                                                                                                                                                           |
| _-nouser uid_      | _Pesquisa arquivos que não tenham o uid informado._                                                                                                                                                                                                                                                                                                                                                          |
| _-perm mode_       | _Pesquisa arquivos pelos exatos bits de permissões pode ser (octal ou simbólico). Ex: -perm g=w aqui vamos pesquisar pela permissão 0020. Aqui é considerado a permissão somente escrita para o grupo não considerando as outras permissões, se desejar pesquisar por exemplo: -perm -g=w aqui estamos pesquisando arquivos cuja a permissão do grupo é escrita não se importando com as outras permissões._ |
| _-readable_        | _Pesquisa arquivos que podem ser lidos._                                                                                                                                                                                                                                                                                                                                                                     |
| _-regex pattern_   | _Pesquisa arquivos que casam com a expressão regular._                                                                                                                                                                                                                                                                                                                                                       |
| _-size n [cwbkMG]_ | <p>_Pesquisa por arquivos que usem n unidades de espaço em disco. Os sufixos utilizados são._</p><p>_b – para blocos de 512-bytes é o padrão utilizado_</p><p>_c – para bytes_</p><p>_w – para words de dois bytes_</p><p>_k - para kilobytes (unidade de 1024 bytes)_</p><p>_M – para Megabytes (unidades de 1048576 bytes)_</p><p>_G – para Gigabytes (unidades de 1073741824 bytes)_</p>                  |
| _-type t_          | <p>_Pesquisa arquivos pelo seu tipo o t pode ser:_</p><p>_b – dispositivo de bloco_</p><p>_c – dispositivo de caractere_</p><p>_d – diretório_</p><p>_p – pipe_</p><p>_f – arquivo regular_</p><p>_l – link simbólico_</p><p>_s – socket_</p>                                                                                                                                                                |
| _-uid n_           | _Pesquisa arquivos que o seu uid é n_                                                                                                                                                                                                                                                                                                                                                                        |
| _-user uname_      | _Pesquisa arquivos que o dono seja uname (podemos utilizar uid aqui também. invés do nome)_                                                                                                                                                                                                                                                                                                                  |
| _-writable_        | _Pesquisa por arquivos que podem ser escritos_                                                                                                                                                                                                                                                                                                                                                               |
| _-exec command_    | _Executa um comando caso a pesquisa retorne true._                                                                                                                                                                                                                                                                                                                                                           |

#### **Exemplos do uso do find.**

Vamos efetuar uma pesquisa do diretório /srv pesquisando por aquivos que no nome contenham teste

```bash
root@flownerd:~# find /srv -name "teste*"
```

Vamos efetuar uma pesquisa do diretório /usr e vamos pesquisar por arquivos .html que geralmente são documentações, porém vamos utilizar o -iname não não se preocuparmos se estão em caixa alta ou não.

```bash
root@flownerd:~# find /usr -iname "*.HtmL"
```

Agora vamos fazer uma pesquisa do diretório /tmp por arquivos com o nome de core e que sejam do tipo arquivo regular e vamos exclui-los caso encontremos algum.

```bash
root@flownerd:~# find /tmp -iname core -type f -print | xargs /bin/rm -f
```

Agora vamos pesquisar no diretório /home arquivos do tipo regular e vamos executar o comando file para cada arquivo encontrado.

```bash
root@flownerd:~# find /home -type f -exec file '{}' \;
```

Opção utilizando xargs

```bash
root@flownerd:~# find /home -type f | xargs file
```

Vamos fazer uma pesquisa diretório home do usuário flownerd e vamos verificar quais arquivos foram modificados nas últimas 24 horas.

```bash
root@flownerd:~# find /home/flownerd -mtime 0
```

Vamos efetuar uma pesquisa nos diretório /sbin e /usr/sbin por arquivos que tenham permissão de execução porém não tenha a permissão de leitura.

```bash
root@flownerd:~# find /sbin /usr/sbin -executable ! -readable -print
```

Agora vamos efetuar uma pesquisa por arquivos que tenham permissão de escrita para o dono e o grupo dono do arquivo e permissão de leitura para outros no diretório /etc

```bash
root@flownerd:~# find /etc -perm 664
```

### **O comando whereis**

O comando whereis pesquisa o fontes/binários e seções de manuais para os arquivos especificados na pesquisa

#### **Opções do comando whereis**

| **_Parâmetro_** | **_Descrição_**                                                                                                                                                                                             |
| :-------------- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _-b_            | _Pesquisa por arquivos binários_                                                                                                                                                                            |
| _-m_            | _Pesquisa por seções nos manuais_                                                                                                                                                                           |
| _-s_            | _Pesquisa por arquivos fontes._                                                                                                                                                                             |
| _-u_            | _Pesquisa por entradas não usuais. Um arquivo não usual pode ser uma entrada que não foi requisitada. Desta maneira whereis -m -u \* pesquisa por arquivos no diretório corrente que não tem documentações_ |
| _-B_            | _Altera ou caso contrário limita os lugares onde o whereis vai pesquisar por binários._                                                                                                                     |
| _-M_            | _Altera ou caso contrário limita os lugares onde o whereis vai pesquisar por seções do manual_                                                                                                              |
| _-S_            | _Altera ou caso contrário limita os lugares onde o whereis vai pesquisar por código fonte._                                                                                                                 |

Vamos pesquisar informações sobre o comando find

```bash
root@flownerd:~# whereis find
find: /usr/bin/find /usr/share/man/man1/find.1.gz /usr/share/info/find.info-1.gz /usr/share/info/find.info.gz /usr/share/info/find.info-2.gz
```

Agora vamos procurar somente informações sobre as seções do manual para o find.

```bash
root@flownerd:~# whereis -m find
find: /usr/share/man/man1/find.1.gz /usr/share/info/find.info-1.gz /usr/share/info/find.info.gz /usr/share/info/find.info-2.gz
```

### **O comando which**

O comando which retorna a caminho completo de um arquivo executável que está na PATH.

Vamos pesquisar o caminho completo do comando man

```bash
root@flownerd:~# which man
/usr/bin/man
```

### **Os comando updatedb e locate**

O comando updatedb atualiza ou cria um banco de dados usado pelo para efetuar pesquisa pelo comando locate. Este arquivo contem uma lista de entradas que podem ser arvores de diretórios que foram atualizadas pelo sistema, diferente do find que pesquisa em tempo real o locate vai pesquisar na base de dados que foi gerada pelo updatedb ou seja se ouve alguma alteração do sistema de arquivos a pesquisa com o locate ainda não vai poder pesquisar esta alteração enquanto o updatedb não atualizar o seu banco.

Para gerarmos uma base de dados com o updatedb podemos utilizar o comando abaixo.

```bash
root@flownerd:~# updatedb
```

Podemos utilizar a opção --output=dbfile onde o dbfile é o caminho que podemos armazenar o nosso banco de dados, o padrão é /var/cache/locate/locatedb.

#### **Opções do comando locate**

| **_Parâmetro_** | **_Descrição_**                                                                                                                              |
| :-------------- | :------------------------------------------------------------------------------------------------------------------------------------------- |
| _-b_            | _Pesquisa pelo padrão informado_                                                                                                             |
| _-c_            | _Ao invés de mostrar o resultado da pesquisa vai retornar o numero de combinações encontradas_                                               |
| _-d_            | _Especifica o caminho para o banco de dados do updatedb caso esteja em outro lugar caso tenha utilizar o --output=dbfile no comando updatdb_ |
| _-e_            | _Mostra somente as entradas que se referem a arquivos existentes quando o comando locate foi executado._                                     |
| _-i_            | _Não diferencia maiúsculas e minusculas._                                                                                                    |
| _-l_            | _Limita a quantidade de resultados retornados pelo comando locate._                                                                          |
| _-S_            | _Mostra as estatísticas sobre cada entrada lida da base de dados._                                                                           |

Vamos verificar as estáticas da nossa base de dados

```bash
root@flownerd:~# locate -S
O banco de dados /var/cache/locate/locatedb está no formato GNU LOCATE02.
Banco de dados teve sua última alteração em 2021:09:14 21:37:56.171652706 -0300
Tamanho do banco de dados do locate: 351529 bytes
Todos os nomes de arquivos: 34293
Nomes de arquivos devem ter um comprimento cumulativo de 1462209 bytes.
Destes nomes de arquivos,

        0 contém espaço em branco,
        0 contém caracteres de nova linha,
        e 2 contém caracteres com o bit alto definido.
Taxa de compressão 75,96% (maior é melhor)
```

Vamos efetuar uma pesquisa pelo X11, porém vamos se importar se estão em caixa alta ou não e vamos limitar a nossa saída a 10.

```bash
root@flownerd:~# locate -i X11 -l 10
/etc/X11
/etc/X11/xkb
/usr/lib/modules/5.10.0-8-amd64/kernel/drivers/hwmon/max1111.ko
/usr/lib/modules/5.10.0-8-amd64/kernel/drivers/iio/adc/max11100.ko
/usr/lib/modules/5.10.0-8-amd64/kernel/drivers/iio/adc/max1118.ko
/usr/lib/systemd/system/x11-common.service
/usr/lib/tmpfiles.d/x11.conf
/usr/lib/x86_64-linux-gnu/libX11.so.6
/usr/lib/x86_64-linux-gnu/libX11.so.6.4.0
/usr/share/X11
```

## **Visualizando e manipulando arquivos**

### **O comando cat**

Utilizamos o comando cat para concatenar ou visualizar o conteúdo de arquivos.

#### **Opções do comando cat**

| **_Parâmetro_** | **_Descrição_**                                  |
| :-------------- | :----------------------------------------------- |
| _-A_            | _Equivalente a -vET_                             |
| _-b_            | _Numera a saída das linhas que não estão vazias_ |
| _-e_            | _Equivalente a -vE_                              |
| _-E_            | _Mostra $ no final de cada linha_                |
| _-n_            | _Numera as todas as linhas de saída do arquivo_  |
| _-s_            | _Suprime a saída de linhas vazias repetidas_     |
| _-t_            | _Equivalente a -vT_                              |
| _-T_            | _Mostra TAB como um caractere ^I_                |
| _-v_            | _Usa a notação -M e ^, exceto para LFD e TAB_    |

Vamos visualizar o arquivo /etc/motd com o comando cat

```bash
root@flownerd:~# cat /etc/motd

The programs included with the Debian GNU/Linux system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
permitted by applicable law.
```

Como podemos notar se não passarmos nenhum parâmetro para o cat ele vai nos retornar o conteúdo do arquivo em alguns casos precisamos numerar a saída e podemos utilizar a opção -b para numerar as linhas que não estão em branco ou -n para numerar todas as linhas até as em branco.

```bash
root@flownerd:~# cat -b /etc/motd

     1  The programs included with the Debian GNU/Linux system are free software;
     2  the exact distribution terms for each program are described in the
     3  individual files in /usr/share/doc/*/copyright.

     4  Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent
     5  permitted by applicable law.
```

### **O comando tac**

O comando tac tem a mesma função do cat porém em forma inversa, ou seja imprime o arquivo de baixo para cima.

Vamos testar o tac no mesmo arquivo que testamos com o cat

```bash
root@flownerd:~# tac /etc/motd
permitted by applicable law.
Debian GNU/Linux comes with ABSOLUTELY NO WARRANTY, to the extent

individual files in /usr/share/doc/*/copyright.
the exact distribution terms for each program are described in the
The programs included with the Debian GNU/Linux system are free software;
```

### **O comando zcat**

O comando zcat é utilizado para visualizar dados compactados em formato gzip sem precisar descompactá-los.

Vamos testar o zcat em um arquivo compactado no formato gz.

```bash
root@flownerd:~# zcat /usr/share/doc/apt/NEWS.Debian.gz
apt (2.1.16) unstable; urgency=medium

  Automatically remove unused kernels on apt {dist,full}-upgrade. To revert
  to previous behavior, set APT::Get::AutomaticRemove::Kernels to false or
  pass --no-auto-remove to the command. apt-get remains unchanged.

  Packages files can now set the Phased-Update-Percentage field to restrict
  update rollout to a specified percentage of machines. Previously, this has
  only been available to users of Ubuntu's update-manager tool. See
  apt_preferences(5) for details and how to configure multiple systems to get
  the same updates. Phased updates are disabled in chroots for now to not
  break buildd-style setups.
[...]
```

### **O comando bzcat**

O comando bzcat é utilizado para visualizar dados compactados em formato bzip2 sem precisar descompactá-los.

Vamos testar o bzcat em um arquivo compactado no formato bz2.

```bash
root@flownerd:~# tar -cjf passwd.tar.bz2 /etc/passwd 2> /dev/null
root@flownerd:~# bzcat passwd.tar.bz2
```

### **O comando xzcat**

O comando xzcat é utilizado para visualizar dados compactados em formato xz sem precisar descompactá-los.

Vamos testar o xzcat em um arquivo compactado no formato xz.

```bash
root@flownerd:~# tar -cJf interfaces.tar.xz /etc/network/interfaces 2> /dev/null
root@flownerd:~# xzcat interfaces.tar.xz
```

### **O comando head**

O comando head lista as 10 primeiras linhas de um arquivo informado.

#### **Parâmetros do comando head**

| **_Parâmetro_** | **_Descrição_**                                 |
| :-------------- | :---------------------------------------------- |
| _-n n_          | _Lista as n primeiras linhas do arquivo_        |
| _-q_            | _Nunca imprime o nome do arquivo no cabeçalho_  |
| _-v_            | _Sempre imprime o nome do arquivo no cabeçalho_ |

Vamos listar as 10 primeiras linhas do arquivo /etc/passwd com o comando head

```bash
root@flownerd:~# head /etc/passwd
root:x:0:0:root:/root:/bin/bash
daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
bin:x:2:2:bin:/bin:/usr/sbin/nologin
sys:x:3:3:sys:/dev:/usr/sbin/nologin
sync:x:4:65534:sync:/bin:/bin/sync
games:x:5:60:games:/usr/games:/usr/sbin/nologin
man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
```

Como são somente as 10 primeiras linhas do arquivo não precisamos especificar parametros, porém agora vamos listar as 15 primeiras linhas do arquivo /etc/inittab e vamos listar o nome do arquivo no cabeçalho.

```bash
root@flownerd:~# head -n 15 -v /etc/nsswitch.conf
==> /etc/nsswitch.conf <==
# /etc/nsswitch.conf
#
# Example configuration of GNU Name Service Switch functionality.
# If you have the `glibc-doc-reference' and `info' packages installed, try:
# `info libc "Name Service Switch"' for information about this file.

passwd:         files systemd
group:          files systemd
shadow:         files
gshadow:        files

hosts:          files dns
networks:       files

protocols:      db files
```

### **O comando tail**

O comando tail lista as 10 últimas linhas de um arquivo informado.

#### **Parâmetros do comando tail**

| **_Parâmetro_** | **_Descrição_**                                                     |
| :-------------- | :------------------------------------------------------------------ |
| _-n n_          | _Lista as n primeiras linhas do arquivo_                            |
| _-q_            | _Nunca imprime o nome do arquivo no cabeçalho_                      |
| _-v_            | _Sempre imprime o nome do arquivo no cabeçalho_                     |
| _-f_            | _Fica visualizando o arquivo em tempo esperando por novas entradas_ |

Vamos listar as 10 últimas linhas do arquivo /etc/passwd com o comando tail

```bash
root@flownerd:~# tail /etc/passwd
nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
_apt:x:100:65534::/nonexistent:/usr/sbin/nologin
systemd-timesync:x:101:101:systemd Time Synchronization,,,:/run/systemd:/usr/sbin/nologin
systemd-network:x:102:103:systemd Network Management,,,:/run/systemd:/usr/sbin/nologin
systemd-resolve:x:103:104:systemd Resolver,,,:/run/systemd:/usr/sbin/nologin
messagebus:x:104:110::/nonexistent:/usr/sbin/nologin
avahi-autoipd:x:105:113:Avahi autoip daemon,,,:/var/lib/avahi-autoipd:/usr/sbin/nologin
sshd:x:106:65534::/run/sshd:/usr/sbin/nologin
douglas:x:1000:1000:Douglas,,,:/home/douglas:/bin/bash
systemd-coredump:x:999:999:systemd Core Dumper:/:/usr/sbin/nologin
```

Como são somente as 10 últimas linhas do arquivo não precisamos especificar parametros, porém agora vamos listar as 15 últimas linhas do arquivo /etc/inittab e vamos listar o nome do arquivo no cabeçalho.

```bash
root@flownerd:~# tail -n 15 -v /etc/services
==> /etc/services <==
amandaidx       10082/tcp                       # amanda backup services
amidxtape       10083/tcp                       # amanda backup services
sgi-cmsd        17001/udp               # Cluster membership services daemon
sgi-crsd        17002/udp
sgi-gcd         17003/udp                       # SGI Group membership daemon
sgi-cad         17004/tcp                       # Cluster Admin daemon
binkp           24554/tcp                       # binkp fidonet protocol
asp             27374/tcp                       # Address Search Protocol
asp             27374/udp
csync2          30865/tcp                       # cluster synchronization tool
dircproxy       57000/tcp                       # Detachable IRC Proxy
tfido           60177/tcp                       # fidonet EMSI over telnet
fido            60179/tcp                       # fidonet EMSI over TCP

# Local services
```

### **O comando nl**

O comando nl lista um arquivo passado como parâmetro e numera as linhas como o comando cat com a opção de -n.

Vamos listar o arquivo /etc/passwd com o nl

```bash
root@flownerd:~# nl /etc/passwd
     1  root:x:0:0:root:/root:/bin/bash
     2  daemon:x:1:1:daemon:/usr/sbin:/usr/sbin/nologin
     3  bin:x:2:2:bin:/bin:/usr/sbin/nologin
     4  sys:x:3:3:sys:/dev:/usr/sbin/nologin
     5  sync:x:4:65534:sync:/bin:/bin/sync
     6  games:x:5:60:games:/usr/games:/usr/sbin/nologin
     7  man:x:6:12:man:/var/cache/man:/usr/sbin/nologin
     8  lp:x:7:7:lp:/var/spool/lpd:/usr/sbin/nologin
     9  mail:x:8:8:mail:/var/mail:/usr/sbin/nologin
    10  news:x:9:9:news:/var/spool/news:/usr/sbin/nologin
    11  uucp:x:10:10:uucp:/var/spool/uucp:/usr/sbin/nologin
    12  proxy:x:13:13:proxy:/bin:/usr/sbin/nologin
    13  www-data:x:33:33:www-data:/var/www:/usr/sbin/nologin
    14  backup:x:34:34:backup:/var/backups:/usr/sbin/nologin
    15  list:x:38:38:Mailing List Manager:/var/list:/usr/sbin/nologin
    16  irc:x:39:39:ircd:/run/ircd:/usr/sbin/nologin
    17  gnats:x:41:41:Gnats Bug-Reporting System (admin):/var/lib/gnats:/usr/sbin/nologin
    18  nobody:x:65534:65534:nobody:/nonexistent:/usr/sbin/nologin
    19  _apt:x:100:65534::/nonexistent:/usr/sbin/nologin
    20  systemd-timesync:x:101:101:systemd Time Synchronization,,,:/run/systemd:/usr/sbin/nologin
    21  systemd-network:x:102:103:systemd Network Management,,,:/run/systemd:/usr/sbin/nologin
    22  systemd-resolve:x:103:104:systemd Resolver,,,:/run/systemd:/usr/sbin/nologin
    23  messagebus:x:104:110::/nonexistent:/usr/sbin/nologin
    24  avahi-autoipd:x:105:113:Avahi autoip daemon,,,:/var/lib/avahi-autoipd:/usr/sbin/nologin
    25  sshd:x:106:65534::/run/sshd:/usr/sbin/nologin
    26  douglas:x:1000:1000:Douglas,,,:/home/douglas:/bin/bash
    27  systemd-coredump:x:999:999:systemd Core Dumper:/:/usr/sbin/nologin
```

### **O comando more**

O comando more é usado quando se quer, paginar a saída de de um arquivo que vai ser mais do que uma página inteira ou a saída de um comando que vai ser muito longo. Temo que considerar que o more só página para frente ou seja depois que paginou para baixo não podemos voltar.

Vamos testar o more com uma pesquisa

```bash
root@flownerd:~# find /etc -iname "*.conf" | more
```

Caso se tenha um arquivo muito grande que queira visualizar podemos chamar direto o more para visualizá-lo como o comando cat, como no exemplo abaixo:

```bash
root@flownerd:~# more /etc/services
```

### **O comando zmore**

O comando zmore funciona como o more porém é utilizado para visualiar arquivos compactados no formato gzip

```bash
root@flownerd:~# zmore /usr/share/doc/tar/NEWS.gz
```

### **O comando bzmore**

O comando bzmore funciona como o more porém é utilizado para visualiar arquivos compactados no formato bzip2

```bash
root@flownerd:~# bzmore /root/passwd.tar.bz2
```

### **O comando xzmore**

O comando xzmore funciona como o more porém é utilizado para visualiar arquivos compactados no formato xz.

```bash
root@flownerd:~# xzmore /root/interfaces.tar.xz
```

### **O comando less**

O comando less é usado quando se quer, paginar a saída de de um arquivo que vai ser mais do que uma página inteira ou a saída de um comando que vai ser muito longo. Diferente do more o less nós conseguimos paginar tanto para baixo como para cima o arquivo.

Vamos testar o more com uma pesquisa

```bash
root@flownerd:~# find /etc -iname "*.conf" | less
```

Caso se tenha um arquivo muito grande que queira visualizar podemos chamar direto o less para visualizá-lo como o comando cat, como no exemplo abaixo:

```bash
root@flownerd:~# less /etc/services
```

### **O comando zless**

O comando zless funciona como o less porém é utilizado para visualiar arquivos compactados no formato gzip

```bash
root@flownerd:~# zless /usr/share/doc/tar/NEWS.gz
```

### **O comando bzless**

O comando bzless funciona como o less porém é utilizado para visualiar arquivos compactados no formato bzip2

```bash
root@flownerd:~# bzless /root/passwd.tar.bz2
```

### **O comando xzless**

O comando xzless funciona como o less porém é utilizado para visualiar arquivos compactados no formato xz

```bash
root@flownerd:~# xzless /root/interfaces.tar.xz
```

### **O comando dos2unix**

O comando dos2unix converte um arquivo texto do formato MS-DOS para o formato Unix que em alguns casos podem dar muita dor de cabeça para um administrador Linux a diferença na terminação da linha

Para utilizar este comando basta passar para o comando o arquivo que deseja converter.

```bash
root@flownerd:~# dos2unix arquivo.txt
```

### **O comando unix2dos**

O comando unix2dos converte um arquivo texto do formato Unix para o formato MS-DOS

Para utilizar este comando basta passar para o comando o arquivo que deseja converter.

```bash
root@flownerd:~# unix2dos arquivo.txt
```

### **O comando expand**

O comando expand é utilizado para substituir tabulações por espaços, aceitando arquivos na linha de comando ou texto na entrada padrão. Por padrão, coloca-se o resultado na saída padrão.

#### **Parâmetros do comando expand**

| **_Parâmetro_** | **_Descrição_**                                                             |
| :-------------- | :-------------------------------------------------------------------------- |
| _-t n_          | _Substitui as ocorrências de tabulação do texto por n caracteres em branco_ |
| _-i_            | _Substitui somente as ocorrências de tabulação no início da linha_          |

Vamos pegar o exemplo de um arquivo qualquer

```bash
root@flownerd:~# cat /etc/network/interfaces
# This file describes the network interfaces available on your system
# and how to activate them. For more information, see interfaces(5).

source /etc/network/interfaces.d/*

# The loopback network interface
auto lo
iface lo inet loopback

# The primary network interface
allow-hotplug enp0s3
iface enp0s3 inet static
        address 192.168.0.10/24
        gateway 192.168.0.1
        # dns-* options are implemented by the resolvconf package, if installed
        dns-nameservers 8.8.8.8 8.8.4.4
        dns-search flownerd.local
```

Vamos validar se o arquivo esta com tabs

```bash
root@flownerd:~# cat -T /etc/network/interfaces
# This file describes the network interfaces available on your system
# and how to activate them. For more information, see interfaces(5).

source /etc/network/interfaces.d/*

# The loopback network interface
auto lo
iface lo inet loopback

# The primary network interface
allow-hotplug enp0s3
iface enp0s3 inet static
^Iaddress 192.168.0.10/24
^Igateway 192.168.0.1
^I# dns-* options are implemented by the resolvconf package, if installed
^Idns-nameservers 8.8.8.8 8.8.4.4
^Idns-search flownerd.local
```

Agora vamos utilizar o expand para trocar as tabulações por espaços

```bash
root@flownerd:~# expand -t 1 /etc/network/interfaces
# This file describes the network interfaces available on your system
# and how to activate them. For more information, see interfaces(5).

source /etc/network/interfaces.d/*

# The loopback network interface
auto lo
iface lo inet loopback

# The primary network interface
allow-hotplug enp0s3
iface enp0s3 inet static
 address 192.168.0.10/24
 gateway 192.168.0.1
 # dns-* options are implemented by the resolvconf package, if installed
 dns-nameservers 8.8.8.8 8.8.4.4
 dns-search flownerd.local
```

Agora se validarmos a saida do comando com o cat

```bash
root@flownerd:~# expand -t 1 /etc/network/interfaces | cat -A
# This file describes the network interfaces available on your system$
# and how to activate them. For more information, see interfaces(5).$
$
source /etc/network/interfaces.d/*$
$
# The loopback network interface$
auto lo$
iface lo inet loopback$
$
# The primary network interface$
allow-hotplug enp0s3$
iface enp0s3 inet static$
 address 192.168.0.10/24$
 gateway 192.168.0.1$
 # dns-* options are implemented by the resolvconf package, if installed$
 dns-nameservers 8.8.8.8 8.8.4.4$
 dns-search flownerd.local$
```

### **O comando unexpand**

O comando unexpand é utilizado para substituir espaços por tabulações no começo da linha, aceitando arquivos na linha de comando ou texto na entrada padrão. Por padrão, coloca-se o resultado na saída padrão.

#### **Parâmetros do comando unexpand**

| **_Parâm._** | **_Descrição_**                                                             |
| :----------- | :-------------------------------------------------------------------------- |
| _-t n_       | _Substitui as ocorrências de tabulação do texto por n caracteres em branco_ |
| _-a_         | _Substitui somente as ocorrências de tabulação no início da linha_          |

Vamos pegar o exemplo de um arquivo qualquer

```bash
root@flownerd:~# head /etc/ssh/sshd_config
#       $OpenBSD: sshd_config,v 1.103 2018/04/09 20:41:22 tj Exp $

# This is the sshd server system-wide configuration file.  See
# sshd_config(5) for more information.

# This sshd was compiled with PATH=/usr/bin:/bin:/usr/sbin:/sbin

# The strategy used for options in the default sshd_config shipped with
# OpenSSH is to specify options with their default value where
# possible, but leave them commented.  Uncommented options override the
```

Agora vamos utilizar o expand para trocar as tabulações por espaços

```bash
root@flownerd:~#  head /etc/ssh/sshd_config | unexpand -t 1
#       $OpenBSD: sshd_config,v 1.103 2018/04/09 20:41:22 tj Exp $

# This is the sshd server system-wide configuration file.               See
# sshd_config(5) for more information.

# This sshd was compiled with PATH=/usr/bin:/bin:/usr/sbin:/sbin

# The strategy used for options in the default sshd_config shipped with
# OpenSSH is to specify options with their default value where
# possible, but leave them commented.           Uncommented options override the
```

### **O comando rev**

O comando rev inverte as linhas como se fosse um espelho

Vamos verificar um exemplo do rev no arquivo /etc/motd

```bash
root@flownerd:~# rev /etc/motd

;erawtfos eerf era metsys xuniL/UNG naibeD eht htiw dedulcni smargorp ehT
eht ni debircsed era margorp hcae rof smret noitubirtsid tcaxe eht
.thgirypoc/*/cod/erahs/rsu/ ni selif laudividni

tnetxe eht ot ,YTNARRAW ON YLETULOSBA htiw semoc xuniL/UNG naibeD
.wal elbacilppa yb dettimrep
```

# **Editores de Texto**

## **Introdução**

A edicão de texto é uma das tarefas mais frequentemente executadas por seres humanos em ambientes computacionais, em qualquer nível. Usuários finais, administradores de sistemas, programadores de software, desenvolvedores web, e tantas outras categorias, todos eles, constantemente, necessitam editar textos.

Usuários finais editam texto para criar documentos, enviar e-mails, atualizar o blog, escrever recados ou simplesmente trocar mensagens instantâneas pela internet. Administradores de sistemas editam arquivos de configuração, criam regras de segurança, editam scripts e manipulam saídas de comandos armazenados em arquivos de texto. Programadores desenvolvem códigos-fonte e a documentação de programas essencialmente em editores de texto. Desenvolvedores web interagem com editores de texto para criarem layout e dinâmica de sites.

Tamanha é a frequência e onipresença da tarefa de edição de texto que a eficiência, flexibilidade e o repertório de ferramentas de editores de texto tornam-se quesitos críticos para se atingir produtividade e conforto na edição de textos.

Qualquer tarefa de aprendizado requer um certo esforço. Todo programa introduz novos conceitos, opções e configurações que transformam o modo de operação do usuário. Em princípio, quanto maior o esforço, maior o benefício. Quem quer apenas escrever textos, pode-se contentar com um editor básico, cuja as únicas opções ao digitar o texto, abrir e salvar o documento ou pode utilizar um editor que permita pré-configurações, formatar o conteúdo, revisar a ortografia, etc, além da ação básica que é escrever textos.

Qualquer usuário de computador pode abrir o primeiro tipo de editor e imediatamente começar a escrever, a curto prazo, sua ação terá consequências imediatas e não requer conhecimentos adicionais. Por outro lado, esse usuário terá que fazer esforço para digitar o mesmos cabeçalho todos os dias.

O outro tipo de editor permite que o usuário pré-configure o cabeçalho do documento e todos os dias esse trecho já estará digitado. Em contrapartida, o usuário deve aprender como pré-configurar o editor. O que requer esforço para aprender a utilizar o programa escolhido. O benefício somente será observado a médio/longo prazo, quando o tempo ganho ao utilizar a configuração será superior ao tempo consumido aprendendo sobre o programa.

## **O editor Nano**

Nano é um editor que deve ser executado a partir de um terminal, e se concentra em simplicidade. Nano é um clone do antigo editor de texto Pico, o editor para o cliente de e-mail Pine, que foi muito popular lá pelos anos 90, em UNIX e sistemas do tipo UNIX. O Pine foi substituído pelo Alpine e o Pico pelo Nano, mas algumas coisas não mudaram - assim como a simplicidade de edição com o Nano.

Nano foi criado em 1999 com o nome de "TIP" (uma sigla, um acrônimo recursivo que significa "TIP Isn't Pine", ou "TIP não é o Pine") por Chris Allagretta. Allagretta decidiu criar este clone do Pico porque o programa não foi liberado sob a GPL. O nome foi mudado oficialmente em 10 de janeiro de 2000 para diminuir a confusão entre o novo editor e o comando "tip" (o comando "tip" é comum em Sun Solaris).

Nano usa combinações muito simples de teclas para trabalhar com arquivos. Um arquivo é aberto ou iniciado com o comando:

```bash
root@flownerd:~# nano <nomedoarquivo>
```

Onde <nomedoarquivo> é o nome do arquivo que você deseja abrir. Ou, se você precisa editar um arquivo que somente o usuário root tem acesso, faça

```bash
root@flownerd:~# sudo nano <nomedoarquivo>
```

Quando o arquivo estiver aberto no Nano, você verá uma pequena lista de exemplos de comando na parte inferior da janela do terminal.

Todas as combinações de teclas para Nano começam com a tecla CTRL. Para executar um comando você deve manter a tecla CTRL pressionada e clicar na segunda tecla para executar a ação. As combinações mais comuns para Nano são:

- CTRL-X - Sai do editor. Se você estiver no meio da edição de um arquivo, o processo de saída irá perguntar se você quer salvar seu trabalho.
- CTRL-R - Ler um arquivo em seu arquivo de trabalho atual. Isso permite que você adicione o texto de outro arquivo enquanto trabalha dentro de um novo arquivo.
- CTRL-C - Mostra a posição atual do cursor.
- CTRL-K - 'recorta' o texto.
- CTRL-U - 'cola' o texto.
- CTRL-S - Salva o arquivo e continua trabalhando.
- CTRL-T - verifica a ortografia do seu texto.
- CTRL-W - faz uma busca no texto.
- CTRL-A - leva o cursor para o início da linha.
- CTRL-E - leva o cursor para o fim da linha.
- CTRL-G - mostra a ajuda do Nano.

Para obter mais comandos do nano basta digitar CTRL + G

## **O editor VI**

O VI é um dos editores de texto mais populares em sistemas de tipo Unix/Linux. Apesar da sua ergonomia muito limitada, este editor é fantástico, com ele é possível fazer coisas inacreditáveis. Muitos usuários do mundo Unix/Linux preferem optar por outros editores devido sua complexidade, como joe, elvis, nano, pico, mcedit, emacs etc. Vale ressaltar que este artigo não tem como finalidade levantar nenhuma discussão quanto a preferência dos usuários com relação aos outros editores de textos.

O programa foi criado por Bill Joy em 1976 para o BSD. O nome VI é uma forma abreviada para visual. Em 1991 foi lançado o editor vim, uma derivação melhorada do vi (o nome vim é abreviação para Vi IMproved, ou Vi Melhorado). Ele está presente em quase todas as distribuições Linux, oferecendo mais recursos que seu antecessor.

Usuários do editor Emacs, que também surgiu em 1976, acabam sempre gerando discussões com usuários mais assíduos do vi por questões de gosto pessoal, apesar de que o padrão Unix exige a presença do editor vi, o que o torna mais disseminado.

Como é pequeno e leve, pode ser colocado dentro de disquetes para ser utilizado em manutenção ou mesmo usado em situações em que há pouco recurso computacional.

Sintaxe para abrir um arquivo com o vim

```bash
root@flownerd:~# vim <nomedoarquivo>
```

### **Ajuda integrada**

O Vim possui uma ajuda integrada muito completa, s ̃ao mais de 100 arquivos somando milhares de linhas. O único inconveniente é não haver ainda tradução para o português, sendo o inglês seu idioma oficial; entretanto, as explicações costumam ser sintéticas e diretas, de forma que noções em inglês seriam suficientes para a compreensão de grande parte do conteúdo da ajuda integrada.

**OBS:** No Vim quase todos os comandos podem ser abreviados, no caso "help" pode ser chamado por "h" e assim por diante. Um comando só pode ser abreviado até o ponto em que este nome mais curto não coincida com o nome de algum outro comando existente.

Para chamar a ajuda do Vim pressione Esc e em seguida:

| _Comando_ | _Descrição_                               |
| :-------- | :---------------------------------------- |
| _:help_   | _Versão longa do comando_                 |
| _:h_      | _Versão abreviada do comando_             |
| _F1_      | _Versão por atalho de funções do teclado_ |

### **Modos de operação**

A tabela abaixo mostra uma referência rápida para os modos de operação do Vim, a seguir mais detalhes sobre cada um dos modos.

| **_Modo_** | **_Descrição_**                                 | **_Atalho_**   |
| :--------- | :---------------------------------------------- | :------------- |
| _Normal_   | _Para deletar, copiar, formatar, etc_           | _<Esc>_        |
| _Inserção_ | _Prioritariamente, digitação de texto_          | _I,a,I,A,o,O_  |
| _Visual_   | _Seleção de blocos verticais e linhas inteiras_ | _V, v, Ctrl-v_ |
| _Comando_  | _Uma verdadeira linguagem de programação_       | _<Esc>:_       |

Em oposição a esmagadora maioria dos editores o Vim é um editor que trabalha com "modos de operação (modo de inserção, modo normal, modo visual e etc)", o que a princípio dificulta a vida do iniciante, mas abre um universo de possibilidades, pois ao trabalhar com modos distintos uma tecla de atalho pode ter vários significados, exemplificando: Em modo normal pressionar 'dd' apaga a linha atual, já a em modo de inserção ele irá se comportar como se você estivesse usando qualquer outro editor, ou seja, irá inserir duas vezes a letra 'd'.

Em modo normal pressionar a tecla 'v' inicia uma seleção visual (use as setas de direção). Para sair do novo visual <Esc>. Como um dos princípios do vim é agilidade pode-se usar ao invés de setas (em modo normal) as letras h,l,k,j como se fossem setas:

```bash
       k

h             l

       j
```

Imagine as letras acima como teclas de diração, a letra 'k' é uma seta acima da letra 'j' é uma seta para abaixo e assim por diante.

### **Entrando em modo de edição**

| **_Comando_** | **_Descrição_**                                     |
| :------------ | :-------------------------------------------------- |
| _a_           | _Inicia inserção de texto após o caractere atual_   |
| _i_           | _Inicia inserção de texto antes do caractere atual_ |
| _A_           | _Inicia inserção de texto no final da linha_        |
| _I_           | _Inicia inserção de texto no começo da linha_       |
| _o_           | _Inicia a inserção de texto na linha abaixo_        |
| _O_           | _Inicia a inserção de texto na linha acima_         |

Outra possibilidade é utilizar a tecla <Insert> para entrar no modo de inserção de texto antes do caractere atual, ou seja, o mesmo que a tecla i. Uma vez no modo de inserção, a tecla <Insert> permite alternar o modo de digitação e inserção de simples de caracteres para substituição de caracteres.

Agora começamos a sentir o gostinho de usar o Vim, uma tecla seja maiúscula ou minúscula, faz muita diferença se você não estiver em modo de inserção, e para sair do modo de inserção e voltar ao modo normal sempre use <Esc>.

### **Erros comuns**

Estando em modo de inserção pressionar 'j' na intenção de rolar o documento, neste caso estaremos inserindo simplesmente a letra 'j'.

Estando em modo normal acionar acidentalmente o "<Caps Lock>" e tentar rolar o documento usando a letra 'J', o efeito é a junção das linhas, alias um ótimo recurso quando a intenção é de fato esta.

Em modo normal tentar digitar um número seguido de uma palavra e ao perceber que nada está sendo digitado, iniciar o modo de inserção, digitando por fim o que se queria, o resultado é que o número que foi digitado inicialmente vira um quantificador para o que se digitou ao entrar no modo de inserção. A palavra aparecerá repetida na quantidade do número digitado. Assim, se você quiser digitar 10 vezes "isto é e um teste" faça assim:

```bash
<Esc> ........... Se assegure de estar em modo normal

10 .............. Quantificador

i ............... Entra no modo de inserção

Isto é um teste <Enter> <Esc>
```

### **Editando**

A principal função de um editor de textos é editar textos. Parece óbvio, mas em meio a inúmeros recursos extras essa simples e crucial função perde-se entre todos os demais.

#### **Abrindo o arquivo para edição**

Portanto, a primeira coisa a fazer é abrir um arquivo. Como visto, para abrir

um arquivo com Vim, digite em um terminal:

```bash
root@flownerd:~# vim texto.txt
```

Onde texto.txt é o nome do arquivo que deseja-se criar ou editar.

Caso deseja abrir o arquivo na linha 10, usa-se:

```bash
root@flownerd:~# vim +10 arquivo
```

Se quiser abrir o arquivo na linha que contém um determinado padrão, digite:

```bash
root@flownerd:~# vim +/padrão arquivo
```

Caso o padrão tenha espaços no nome coloque entre aspas ou use escape "\" a fim de não obter erro.

Se o vim for aberto sem indicação de arquivo pode-se indicar o arquivo a ser editado em modo de comando desta forma

```bash
:e /caminho/do/arquivo
```

### **Escrevendo o texto**

O Vim é um editor que possuí diferentes modos de edição. Entre eles está o modo de inserção, que é o modo onde escreve-se o texto naturalmente.

Para se entrar em modo de inserção, estando em modo normal, pode-se pressionar qualquer uma das teclas abaixo:

#### **Inserindo**

| **_Comando_** | **_Descrição_**                                      |
| :------------ | :--------------------------------------------------- |
| _i_           | _Entra no modo de inserção antes do caractere atual_ |
| _I_           | _Entra no modo de inserção no começo da linha_       |
| _a_           | _Entra no modo de inserção após o caractere atual_   |
| _A_           | _Entra no modo de inserção no final da linha_        |
| _o_           | _Entra no modo de inserção uma linha abaixo_         |
| _O_           | _Entra em modo de inserção uma linha acima_          |
| _<Esc>_       | _Sai do modo de inserção_                            |

#### **Copiar, Colar e Deletar**

| **_Comando_** | **_Descrição_**                                            |
| :------------ | :--------------------------------------------------------- |
| _dd_          | _Deleta a linha atual_                                     |
| _D_           | _Deleta o restante da linha_                               |
| _d$_          | _Deleta do ponto atual até o final da linha_               |
| _d^_          | _Deleta do cursor ao primeiro caractere não-nulo da linha_ |
| _d0_          | _Deleta do cursor ao início da linha_                      |
| _yy_          | _Copia a linha atual_                                      |
| _Y_           | _Copia a linha atual_                                      |
| _ye_          | _Copia do cursor ao fim da palavra_                        |
| _yb_          | _Copia do começo da palavra ao cursor_                     |
| _p_           | _Cola o que foi copiado ou deletado abaixo_                |
| _P_           | _Cola o que foi copiado ou deletado acima_                 |
| _[p_          | _Cola o que foi copiado ou deletado antes do cursor_       |
| _]p_          | _Cola o que foi copiado ou deletado após o cursor_         |
| _x_           | _Apaga o caractere sob o cursor_                           |
| _xp_          | _Troca letras de lugar_                                    |
| _ddp_         | _Troca linhas de lugar_                                    |
| _d5x_         | _Apaga os próximos 5 caracteres_                           |
| _dd_          | _Apaga a linha atual_                                      |
| _5dd_         | _Apaga 5 linhas (também pode ser: d5d)_                    |
| _dw_          | _Apaga uma palavra_                                        |
| _5dw_         | _Apaga 5 palavras (também pode ser: d5w)_                  |
| _dl_          | _Apaga uma letra (sinônimo: x)_                            |
| _dgg_         | _Apaga até o início do arquivo_                            |
| _dG_          | _Apaga até o final do arquivo_                             |
| _d%_          | _Deleta até o próximo (,[,{_                               |
| _da"_         | _Deleta aspas com conteúdo_                                |
| _diw_         | _Apaga palavra mesmo que não esteja posicionado no início_ |
| _dip_         | _Apaga o parágrafo atual_                                  |
| _d4b_         | _Apaga as quatro palavras anteriores_                      |
| _dfx_         | _Apaga até o próximo 'x'_                                  |
| _d/casa/+1_   | _Deleta até a linha após a palavra casa_                   |

Trocando a letra 'd' nos comandos acima por 'c' de change "mudança" ao invés de deletar será feita uma mudança no conteúdo. Por exemplo:

| **_Comando_** | **_Descrição_**                 |
| :------------ | :------------------------------ |
| _ciw_         | _Modifica uma palavra_          |
| _cip_         | _Modifica um parágrafo_         |
| _cis_         | _Modifica uma sentença_         |
| _C_           | _Modifica até o final da linha_ |

#### **Copiando sem deletar**

| **_Comando_** | **_Descrição_**                                                 |
| :------------ | :-------------------------------------------------------------- |
| _yy_          | _Copia a linha atual (sinônimo: Y)_                             |
| _5yy_         | _Copia 5 linhas (também pode ser: y5y ou 5Y)_                   |
| _y/pat_       | _Copia até 'pat'_                                               |
| _yw_          | _Copia uma palavra_                                             |
| _5yw_         | _Copia 5 palavras (também pode ser: y5w)_                       |
| _yl_          | _Copia uma letra_                                               |
| _5yl_         | _Copia 5 letras (também pode ser: y5l)_                         |
| _y^_          | _Copia da posição atual até o início da linha (sinônimo: y0)_   |
| _y$_          | _Copia da posição atual até o final da linha_                   |
| _ygg_         | _Copia da posição atual até o início do arquivo_                |
| _yG_          | _Copia da posição atual até o final do arquivo_                 |
| _yi"_         | _Copia trecho entre aspas (atual -inner)_                       |
| _vip_         | _Seleção visual para parágrafo atual 'inner paragraph'_         |
| _yip_         | _Copia o parágrafo atual_                                       |
| _yit_         | _Copia a tag igual 'inner tag' útil para arquivo HTML,XML, etc_ |

Digite 'P' (p maiúsculo) para colar o texto recém copiado na posição onde encontra-se o cursor, ou 'p' para colar o texto na posição imediatamente após o cursor

### **Comandos de movimentação**

| **_Comando_** | **_Descrição_**                               |
| :------------ | :-------------------------------------------- |
| _Ctrl+f_      | _Move o cursor para a próxima tela_           |
| _Ctrl+b_      | _Move o cursor para a tela anterior_          |
| _H_           | _Move o cursor para a primeira linha da tela_ |
| _M_           | _Move o cursor para o meio da tela_           |
| _L_           | _Move o cursor para a última linha da tela_   |
| _h_           | _Move o cursor um caractere a esquerda_       |
| _j_           | _Move o cursor para a próxima linha_          |
| _k_           | _Move o cursor para linha anterior_           |
| _l_           | _Move o cursor um caractere a direita_        |

### **Comandos de busca**

| **_Comando_** | **_Descrição_**                                                            |
| :------------ | :------------------------------------------------------------------------- |
| _/palavra_    | _Busca pela palavra ou caractere em todo o texto_                          |
| _?palavra_    | _Move o cursor para a ocorrência anterior da palavra_                      |
| _n_           | _Repete o último comando / ou ?_                                           |
| _N_           | _Repete o último comando / ou ? , na direção reversa_                      |
| _Ctrl+g_      | _Mostra o nome do arquivo, o número da linha corrente e o total de linhas_ |

#### **Movendo linhas**

| **_Comando_**  | **_Descrição_**                               |
| :------------- | :-------------------------------------------- |
| _:20,30m 0_    | _Move da linha '20' até '30' para o começo_   |
| _:20,/pat/m 5_ | _Move da linha '20' até 'pat' para a linha 5_ |
| _:m-5_         | _Move a linha atual 5 posições para acima_    |
| _:m0_          | _Move a linha atual para o começo_            |
| _:m$_          | _Move a linha para o final do comento_        |

#### **Desfazendo**

| **_Comando_** | **_Descrição_**                          |
| :------------ | :--------------------------------------- |
| _u_           | _Desfazer_                               |
| _U_           | _Desfaz mudança na última linha editada_ |
| _Ctrl-r_      | _Refaz_                                  |

#### **Salvando**

| **_Comando_**    | **_Descrição_**                                    |
| :--------------- | :------------------------------------------------- |
| _:w_             | _Salva_                                            |
| _:wq_            | _Salva e sai_                                      |
| _:w nome_        | _Salvar como_                                      |
| _:saveas nome_   | _Salvar como_                                      |
| _:sav nome_      | _Mesmo que "saveas nome"_                          |
| _:x_             | _Salva se existirem modificações_                  |
| _:10,20 w! nome_ | _Salva da linha 10 até a linha 20 no arquivo nome_ |
| _:w!_            | _Salvamento forçado_                               |
| _:e!_            | _Reinicia a edição ignorando alterações_           |
| _:X_             | _Salva o arquivo com senha_                        |

#### **Dicas**

| **_Comando_**        | **_Descrição_**                                                                                                             |
| :------------------- | :-------------------------------------------------------------------------------------------------------------------------- |
| _. (ponto)_          | _Repete a última ação_                                                                                                      |
| _:sort u_            | _Ordena e remove as linhas duplicadas_                                                                                      |
| _:sort n_            | _Ordena numericamente_                                                                                                      |
| _:1,15 sort n_       | _Ordena numericamente da linha 1 até a linha 15_                                                                            |
| _:sort /.\*\%8v/_    | _Ordena à partir do 8º caractere_                                                                                           |
| _:pwd_               | _Exibe o diretório atual_                                                                                                   |
| _:cd /diretório_     | _Muda de diretório_                                                                                                         |
| _:changes_           | _Visualiza a lista de alterações_                                                                                           |
| _gUU_                | _Converte a linha para maiúsculo_                                                                                           |
| _guu_                | _Converte a linha para minúsculo_                                                                                           |
| _gUiw_               | _Converte a palavra atual para maiúsculo_                                                                                   |
| _~_                  | _Altera o case do caractere atual_                                                                                          |
| _:g /palavra/ m 0_   | _Move as linhas contendo 'palavra' para o começo (linha zero)_                                                              |
| _:v/^192.168.1.\*/d_ | \*Apaga as linhas que contenham 192.168.1\*.\*                                                                              |
| _:v/\S/d_            | _Apaga linhas vazias_                                                                                                       |
| _:0put =range(1,10)_ | _Insere uma sequência de 1 a 10 à partir da linha inicial "zero"_                                                           |
| _:r arquivo_         | _Insere o arquivo na linha atual_                                                                                           |
| _:0r arquivo_        | _Insere o arquivo na primeira linha_                                                                                        |
| _:'0_                | _Abre o último arquivo editado_                                                                                             |
| _:'1_                | _Abre o penúltimo arquivo editado_                                                                                          |
| _:split arquivo_     | _Divide a tela do vim em horizontal podendo manipular dois arquivos ao mesmo tempo para mudar de arquivo utilize Ctrl + ww_ |
| _:vsplit arquivo_    | _Divide a tela do vim em vertical podendo manipular dois arquivos ao mesmo tempo para mudar de arquivo utilize Ctrl + ww_   |

Para gerar uma sequência de endereços ips por exemplo de 192.168.1.1 até 192.168.1.5 podemos utilizar o seguinte comando no vim

```bash
:for i in range(1,5) | .put ='192.168.1.' .i | endfor
```

### **Comparando arquivo com o vimdiff**

O vim possui um modo para checagem de diferenças entre arquivos, é bastante útil especialmente para programadores, para saber quais são as diferenças entre dois arquivos faz-se:

```bash
root@flownerd:~# vimdiff arquivo1.txt arquivo2.txt
```

### **Utilizando o vimtutor**

Para quem quiser aprender a trabalhar com o vim "editando", basta usar o comando "vimtutor"

```bash
root@flownerd:~# vimtutor
```

Este comando vai abrir um arquivo TXT editável, que no corpo dele, há instruções (em inglês) de como editar textos e fazer movimentação.

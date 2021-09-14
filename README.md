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

Encontramos na internet diversos programas que não tem custo algum para se fazer download, dentro destes certamente estão os chamados softwares livres. Mas eles não se resumem à isso. A Free Software Foundation (FSF) descreve sua existência como : “Uma organização sem fins lucrativos com a missão mundial de promover a liberdade do usuário do computador e defender os direitos de todos os usuários de software livre”.

Segundo esta definição, a FSF é uma das fundações responsáveis por fiscalizar e organizar o leque de softwares livres espalhados pelo mundo, em outras palavras, os desenvolvedores de softwares devem seguir algumas diretrizes para enquadrar-se como software livre. Já não é mais tão simplório assim, é? A definição propriamente dita de “software livre” é: Aquele software que respeita a liberdade da comunidade dos usuários. O que significa esta liberdade? Significa que qualquer usuário tem caminho aberto para executar, estudar, distribuir, alterar, melhorar, piorar, copiar qualquer parte do software ou até mesmo ele por inteiro.

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

Conhecido inicialmente como GNU Compilador para C, suporta nos dias de hoje diversas linguagens além da original “C”, com C++, Java, Ada e Fortran. Um software livre que atende à licença GPL e funciona em sistemas operacionais como UNIX, Linux e OS X.

### **Eclipse**

Utilizado para desenvolver aplicações em Java. Por meio de plugins, outras linguagens podem ser utilizadas: C, C++, Fortran, Java Script, PHP, entre outros. O programa é “desenhado” quase totalmente em Java e a base do código é originária da IBM VisualAge. O Eclipse possui o código aberto, entretanto não é compatível como a licença GNU.

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

Os dispositivos são uma coisa que temos que conhecer no Linux, senão se perdemos aos poucos nas configurações mais básicas.

## **O que são dispositivos?**

Um dispositivo é todo o componente de hardware, e do sistema operacional. Um dispositivo é “algo especial” que é compartilhado com o Kernel, ou seja, um exemplo de dispositivo são as impressoras, CD-ROMs, modems, portas, mouse, HDs, etc. No Linux, os dispositivos físicos são tratados como arquivos. Estes arquivos são um tipo especial no sistema de arquivos e se encontram no diretório /dev. Se você der um ls neste diretório, verá que existe um muitos arquivos. Cada arquivo neste diretório corresponderá a um dispositivo de acordo com o seu tipo.

Se você usava DOS/Windows antes, você acessava o drive C:, lembra? No Linux não existe isso! Vai ser um dispositivo no lugar. Você vai usar isso o tempo todo, porque vamos mexer com mouse, com impressora, IDE’s, SCSI’s, etc. Então aqui temos alguns arquivos do /dev e seus respectivos dispositivos:

### **/dev/hdXX**

Aqui é correspondente às Interfaces IDEs, ou seja, tudo que tiver conectado nos cabos IDEs. Exemplos, podemos citar HD’s e CD-ROM’s. O xx significa qual IDE, onde o primeiro x corresponde a qual IDE, e o segundo x (opcional) corresponde a partição. Veja a tabela à seguir:

| **_Dispositivo_** | **_Descrição_**                     |
| :---------------- | :---------------------------------- |
| _/dev/hda_        | _IDE Primária Master_               |
| _/dev/hda1_       | _Partição 1 da IDE Primária Master_ |
| _/dev/hda2_       | _Partição 2 da IDE Primária Master_ |
| _/dev/hdb_        | _IDE Primária Slave_                |
| _/dev/hdb1_       | _Partição 1 da IDE Primária Slave_  |
| _/dev/hdb2_       | _Partição 2 da IDE Primária Slave_  |
| _/dev/hdc_        | _IDE Secundária Master_             |
| _/dev/hdc1_       | _Partição 1 da IDE Master_          |
| _/dev/hdc2_       | _Partição 2 da IDE Master_          |

Perceba aqui que cada hdx vai até os números 2, mas não é apenas até o 2, pode ir mais longe. Dependendo de quantas partições tiver o seu HD, pode ser 3, ou 4, ou 9 por exemplo.

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
| _wlan0_           | _Segunda interface de rede_  |

# **Estrutura de diretórios Linux**

No sistema operacional Linux a estrutura de diretórios é diferente da estrutura Microsoft, por exemplo no Windows a nossa primeira partição vai ser o “c:” no Linux é o “/” a raiz do sistema operacional. Vamos verificar os principais diretórios do nosso sistema.

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
- Links: são arquivos que são utilizados para permitir que um determinado arquivo fique disponível (ou visível) em vários locais do sistema. Um link é como se criar um “atalho” no sistema
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

- Usuário root (ou superusuário): usuário com acesso total ao sistema. Conhecido também como “administrador”, ele é responsável pelo acesso ao sistema sem restrições e possui sinal # como identificador de prompt.

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
root@flownerd:~# shutdown -r 60 “Desligando a maquina em 60 Minutos”
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
| _-Q_            | _Mostra a saída entre aspas duplas “”_                                                                            |
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

#### **O caractere “?”**

Quando um nome de arquivo é esperado, ele casa com um caractere qualquer, ou seja, a ? representa um único e qualquer caractere no nome de um arquivo. Por exemplo:

Primeiramente serão criados alguns arquivos como modelo para que se possa analisar o resultado do uso da “?”.

```bash
root@flownerd:~# touch flownerd.txt flownerd1.txt flownerd2.txt
```

Agora serão usados os metacaracteres para filtrar a listagem dos arquivos “flownerd” que foram criados.

```bash
root@flownerd:~# ls -l flownerd?.txt
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd1.txt
-rw-r--r-- 1 root root 0 set 13 23:36 flownerd2.txt
```

#### **O Caractere \* (asterisco)**

Este é um caractere coringa que substitui qualquer caractere referenciado, não importando a quantidade de vezes de substituições, diferente do “?”, que substitui apenas um único caractere.

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

Agora por exemplo se precisarmos criar um diretório que o seu nome contenha espaço podemos utilizar as aspas “” para efetuar a criação da seguinte forma

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

Note que a única informação que temos é que o nosso arquivo é regular pelo caractere identificar “-”

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

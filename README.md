# Resumo: Arquitetura Limpa

## Índice

- [Prefácio](#prefácio)
- [Apresentação](#apresentação)
- [Introdução](#introdução)
- [O que são Design e Arquitetura?](#o-que-são-design-e-arquitetura)
- [Um Conto de Dois Valores](#um-conto-de-dois-valores)
- [Paradigmas da Programação](#paradigmas-da-programação)
- [Panorama do Paradigma](#panorama-do-paradigma)
- [Programação Estruturada](#programação-estruturada)
- [Princípios da Programação Estruturada](#princípios-da-programação-estruturada)
- [Programação Orientada a Objetos](#programação-orientada-a-objetos)
- [Programação Funcional](#programação-funcional)
- [Princípios de Design](#princípios-de-design)
- [SRP: O Princípio da Responsabilidade Única](#srp-o-princípio-da-responsabilidade-única)
- [OCP: Princípio Aberto-Fechado](#ocp-princípio-aberto-fechado)
- [LSP: Princípio da Substituição de Liskov](#lsp-princípio-da-substituição-de-liskov)
- [ISP: Princípio da Segregação de Interfaces](#isp-princípio-da-segregação-de-interfaces)
- [DIP: Princípio da Inversão de Dependência](#dip-princípio-da-inversão-de-dependência)
- [Princípios dos componentes](#princípios-dos-componentes)
- [Componentes](#componentes)
- [Coesão de componentes](#coesão-de-componentes)
- [Acoplamento de componentes](#acoplamento-de-componentes)
- [O que é arquitetura?](#o-que-é-arquitetura)
- [Independência](#independência)
- [Fronteiras: Estabelecendo Limite](#fronteiras:-estabelecendo-limite)
---

## Prefácio

A arquitetura de software é um dos pilares fundamentais para o sucesso de um sistema, pois define a estrutura, organização e interação entre os componentes de um software. Uma boa arquitetura não apenas melhora a qualidade de um sistema, mas também reduz custos a longo prazo, tornando-o mais fácil de manter, escalar e adaptar às mudanças do mercado.

---

## Apresentação

A imutabilidade do código é a razão pela qual as regras da arquitetura de software são tão consistentes entre os diversos tipos de sistemas.

---

## Introdução

A arquitetura de software define como um sistema é estruturado, tornando-o mais fácil de modificar e manter. Uma boa arquitetura reduz erros, evita retrabalho e diminui custos, garantindo que novas funcionalidades sejam adicionadas sem comprometer o sistema.

Além disso, um design bem implementado prolonga a vida útil do software, tornando-o mais confiável e sustentável ao longo do tempo.

---

## O que são Design e Arquitetura?

Arquitetura e design de software não possuem definições rígidas — eles se complementam.

- **Arquitetura**: trata da organização geral do sistema e suas interações.
- **Design**: foca na implementação e estrutura interna dos componentes.

Embora tenham focos diferentes, não há uma divisão absoluta entre eles, pois ambos contribuem para a construção de um software bem estruturado.

**Conclusão**: A organização do código impacta diretamente a produtividade e a evolução do software. Um código limpo facilita a manutenção, reduz erros e melhora a eficiência da equipe.

Em vez de lidar com a degradação do sistema e tentar reorganizá-lo depois, o ideal é adotar boas práticas desde o início, garantindo um desenvolvimento sustentável e de qualidade.

---

## Um Conto de Dois Valores

A pressão por entregas rápidas pode levar a um código desorganizado, dificultando a manutenção e reduzindo a produtividade ao longo do tempo.

Embora escrever código limpo demande mais atenção no início, isso evita retrabalho e problemas futuros. Manter boas práticas desde o começo **não atrasa o desenvolvimento**, mas sim garante eficiência e evolução contínua do software.

---

## Paradigmas da Programação

A programação é baseada em três paradigmas fundamentais:

1. **Programação Estruturada**
2. **Programação Orientada a Objetos**
3. **Programação Funcional**

Ao longo do tempo, a área passou por diversas revoluções, e a consolidação desses paradigmas foi uma das principais. É improvável que novos paradigmas surjam, pois esses três já estabelecem a base necessária para o desenvolvimento de software moderno.

---

## Panorama do Paradigma

Os paradigmas de programação não apenas introduzem novas formas de estruturar o código, mas também impõem restrições, eliminando certas capacidades do programador com o objetivo de melhorar a qualidade do software.

- A **programação estruturada** removeu o uso do `goto`, tornando o fluxo mais previsível.
- A **orientação a objetos** restringe o acesso direto aos dados, forçando o encapsulamento para maior organização e segurança.
- A **programação funcional** proíbe a mutação de estado e efeitos colaterais, garantindo previsibilidade, embora limite abordagens tradicionais.

É improvável que surjam novos paradigmas, pois esses três já cobrem todas as formas fundamentais de organização do código. As inovações modernas geralmente combinam ou refinam esses conceitos, mas não introduzem um modelo completamente novo.

---

## Programação Estruturada

A programação estruturada surgiu como uma alternativa ao código desorganizado e caótico dos primeiros programas de computador, onde o uso excessivo de `goto` tornava o fluxo de execução difícil de seguir.

Em 1968, Edsger Dijkstra publicou um artigo intitulado *"Go To Statement Considered Harmful"*, que foi um marco na mudança para um estilo de programação mais disciplinado e estruturado. Esse modelo foi adotado para tornar o código mais previsível, modular e fácil de entender.

---

## Princípios da Programação Estruturada

A programação estruturada se baseia em três estruturas de controle fundamentais:

- **Sequência**: as instruções são executadas uma após a outra, na ordem em que aparecem.
- **Seleção**: decisões condicionais permitem que o programa siga caminhos diferentes (ex: `if`, `switch`).
- **Repetição**: permite a execução repetitiva de blocos de código (ex: `for`, `while`).

Com essas estruturas, é possível escrever qualquer programa sem a necessidade de comandos como `goto`, garantindo um código mais organizado e legível.

A programação estruturada é um pilar essencial para a arquitetura limpa, pois fornece uma base sólida para a organização do código. No entanto, ela não resolve todos os problemas sozinha. A arquitetura limpa vai além, aplicando princípios como separação de responsabilidades, inversão de dependências e modularização — permitindo que sistemas grandes sejam mantidos e escalados ao longo do tempo.

**Conclusão**: a programação estruturada foi um divisor de águas na engenharia de software, reduzindo a complexidade do código e melhorando sua manutenibilidade. No entanto, para aplicações modernas, ela deve ser combinada com princípios arquiteturais sólidos, como os da arquitetura limpa.

---

## Programação Orientada a Objetos

A orientação a objetos na arquitetura limpa tem como foco principal o **polimorfismo**, e não apenas os conceitos clássicos como **encapsulamento** e **herança**.

O uso de **interfaces e abstrações** permite construir sistemas desacoplados, garantindo que as regras de negócio não dependam diretamente de detalhes de implementação como frameworks, bancos de dados ou bibliotecas externas.

O **princípio da inversão de dependência (DIP)** desempenha um papel fundamental, pois impede que módulos de alto nível dependam de módulos de baixo nível. Em vez disso, **ambos devem depender de abstrações**. Isso possibilita substituir implementações sem afetar a lógica central do sistema.

A **herança**, embora útil, pode gerar acoplamento excessivo e dificultar a manutenção do código. A **composição** e o uso de **interfaces** são alternativas mais flexíveis, pois permitem modificar e estender funcionalidades sem afetar o código existente.

Seguindo esses princípios, é possível criar uma arquitetura sustentável, testável e resistente a mudanças, onde a lógica de negócios permanece independente da infraestrutura técnica.

---

## Programação Funcional

A programação funcional (FP) enfatiza a imutabilidade e a ausência de efeitos colaterais, tornando o código mais previsível e fácil de testar. Em contraste com a orientação a objetos, que encapsula estados em objetos, a FP trata funções como cidadãos de primeira classe, permitindo passá-las como argumento e retorná-las de outras funções.

O uso de **funções puras** — aquelas que sempre retornam o mesmo resultado para a mesma entrada e não alteram estados externos — ajuda a evitar dependências ocultas e facilita o paralelismo. Estruturas mutáveis e estados globais devem ser evitados, pois tornam o código difícil de depurar e manter.

Outro conceito importante é a **função de ordem superior**, que permite criar código mais modular e reutilizável, tornando a lógica mais declarativa e menos procedural.

Na arquitetura limpa, os princípios da programação funcional ajudam a manter regras de negócio isoladas da infraestrutura, garantindo que a lógica central do sistema seja previsível e testável.

---

## Princípios de Design

O design de software deve seguir princípios que garantem código limpo, flexível e de fácil manutenção. Os princípios SOLID ajudam a estruturar sistemas modulares e desacoplados:

- **S — Princípio da Responsabilidade Única (SRP)**: uma classe deve ter apenas uma razão para mudar, ou seja, deve ter uma única responsabilidade bem definida.
- **O — Princípio Aberto-Fechado (OCP)**: classes e módulos devem estar abertos para extensão, mas fechados para modificação, evitando mudanças diretas no código existente ao adicionar novas funcionalidades.
- **L — Princípio da Substituição de Liskov (LSP)**: subtipos devem poder substituir seus tipos base sem alterar o comportamento esperado, garantindo herança correta e sem efeitos colaterais inesperados.
- **I — Princípio da Segregação de Interfaces (ISP)**: interfaces devem ser específicas e coesas, evitando que sejam forçadas a implementar métodos que não utilizam.
- **D — Princípio da Inversão de Dependência (DIP)**: o código deve depender de abstrações e não de implementações concretas, promovendo o desacoplamento entre módulos.

Esses princípios garantem código organizado, facilitando testes e manutenção, e tornam o sistema mais resiliente a mudanças ao longo do tempo.

---

## SRP: O Princípio da Responsabilidade Única

O Princípio da Responsabilidade Única (SRP) diz que um módulo ou classe deve ser responsável por um único ator ou papel. Isso significa que ele deve cuidar apenas de uma coisa específica, sem misturar responsabilidades de diferentes partes do sistema.

**Exemplo:**

Imagine um sistema que tem uma classe para gerenciar usuários e outra para notificações:

- A **classe de usuários** deve ser responsável apenas por lidar com a criação, edição e exclusão de usuários. Ela não deve se preocupar em enviar e-mails ou notificar alguém.
- A **classe de notificações** deve ser responsável apenas por enviar notificações, como e-mails ou mensagens.

Se a classe de usuários também tivesse que enviar notificações, ela estaria misturando responsabilidades, o que violaria o SRP. Cada classe ou módulo deve ter um único foco, relacionado a um único ator — seja o usuário ou o sistema de notificações — tornando o código mais claro e fácil de modificar.

---

## OCP: Princípio Aberto-Fechado

O Princípio Aberto-Fechado (Open-Closed Principle) estabelece que **as classes devem estar abertas para extensão, mas fechadas para modificação**. Ou seja, devemos ser capazes de adicionar novas funcionalidades ao sistema sem alterar o código existente.

Esse princípio ajuda a evitar efeitos colaterais inesperados ao modificar o comportamento de classes já existentes, promovendo maior estabilidade e manutenibilidade no sistema.

**Como aplicar?**

- Use **interfaces** ou **classes abstratas** para definir comportamentos genéricos.
- Crie **novas implementações** para adicionar funcionalidades, sem modificar o código base.

**Exemplo:**

Imagine que você tem um sistema de envio de mensagens:

```ts
interface Notificador {
  enviar(mensagem: string): void;
}

class EmailNotificador implements Notificador {
  enviar(mensagem: string): void {
    console.log(`Enviando e-mail: ${mensagem}`);
  }
}

class Mensageiro {
  constructor(private notificador: Notificador) {}

  processar(mensagem: string) {
    this.notificador.enviar(mensagem);
  }
}
```

Se quiser adicionar um **SMSNotificador**, basta criar uma nova classe implementando a interface, sem alterar o `Mensageiro`:

```ts
class SMSNotificador implements Notificador {
  enviar(mensagem: string): void {
    console.log(`Enviando SMS: ${mensagem}`);
  }
}
```

Isso segue o OCP: o código existente não foi modificado, apenas **estendido** com novos comportamentos.

---
## LSP: Princípio da Substituição de Liskov
O Princípio da Substituição de Liskov (Liskov Substitution Principle) afirma que uma subclasse deve ser substituível por sua superclasse sem alterar o comportamento esperado do sistema. Ou seja, os objetos das subclasses devem poder ser usados no lugar de objetos da classe base sem causar erros ou comportamentos inesperados.

Esse princípio garante que o sistema continue funcionando corretamente mesmo quando subclasses são usadas em vez das classes pai. Violá-lo geralmente significa que há um problema na hierarquia de herança ou que a subclasse está alterando regras importantes da superclasse.

Exemplo clássico:

Considere as classes Retângulo e Quadrado.

class Retangulo {
  constructor(public largura: number, public altura: number) {}

  setLargura(l: number) {
    this.largura = l;
  }

  setAltura(h: number) {
    this.altura = h;
  }

  getArea(): number {
    return this.largura * this.altura;
  }
}

class Quadrado extends Retangulo {
  setLargura(l: number) {
    this.largura = l;
    this.altura = l;
  }

  setAltura(h: number) {
    this.largura = h;
    this.altura = h;
  }
}
Ao usar um Quadrado onde se espera um Retângulo, o comportamento pode ser alterado de forma inesperada, pois as operações setLargura e setAltura afetam ambos os lados. Isso viola o LSP, pois o Quadrado não mantém as expectativas de comportamento do Retângulo.

Como aplicar corretamente:

Evite sobrescrever métodos de forma que mudem o comportamento da classe base.

Prefira composição em vez de herança quando as restrições entre as classes são muito diferentes.

Crie abstrações mais genéricas se necessário, garantindo que todas as implementações sigam o mesmo contrato.

Conclusão:
O LSP é essencial para garantir reutilização segura de código e evitar bugs difíceis de detectar. Ele promove heranças corretas e interfaces consistentes, mantendo a integridade do sistema ao longo do tempo.

---

## ISP: Princípio da Segregação de Interfaces

O Princípio da Segregação de Interfaces afirma que **nenhuma classe deve ser forçada a depender de métodos que não utiliza**. Em outras palavras, uma classe não deve ser obrigada a implementar interfaces extensas e genéricas que a forcem a lidar com responsabilidades que não lhe dizem respeito.

Quando uma classe depende de outra que possui muitos métodos irrelevantes para seu contexto, isso pode gerar **acoplamento desnecessário**, tornando o sistema mais frágil. Pequenas alterações em uma interface podem afetar várias classes, mesmo aquelas que não utilizam os métodos alterados, aumentando o risco de **erros inesperados**.

Ao aplicar o ISP corretamente, quebramos interfaces grandes em **interfaces menores e mais específicas**, promovendo um código mais coeso, testável e fácil de manter. Dessa forma, cada classe depende apenas do que realmente precisa, reduzindo o impacto de mudanças e melhorando a modularidade do sistema.

---

---

## DIP: Princípio da Inversão de Dependência

O Princípio da Inversão de Dependência afirma que **módulos de alto nível (regras de negócio)** não devem depender de **módulos de baixo nível (detalhes de implementação)**. Ambos devem depender de **abstrações** (interfaces, por exemplo).

### Mas o que isso significa na prática?

Imagine que você está desenvolvendo um aplicativo de envio de mensagens. Sua regra de negócio diz que “ao acontecer determinado evento, deve ser enviado um aviso ao usuário”.

Sem seguir o DIP, você poderia escrever algo assim:

```ts
class Notificador {
  enviarEmail(usuario: Usuario) {
    // lógica para enviar e-mail
  }
}
```

Nesse caso, a lógica depende diretamente de um serviço de e-mail. Se um dia quiser enviar por SMS ou WhatsApp, terá que modificar o código da regra — o que quebra o princípio de separação de responsabilidades e aumenta o risco de erros.

Aplicando o DIP:

```ts
interface INotificador {
  notificar(usuario: Usuario): void;
}

class NotificadorEmail implements INotificador {
  notificar(usuario: Usuario) {
    // envia por e-mail
  }
}

class ServicoDeAviso {
  constructor(private notificador: INotificador) {}

  executar(usuario: Usuario) {
    this.notificador.notificar(usuario);
  }
}
```
Com isso, o ServicoDeAviso não sabe como a notificação é enviada — ele apenas sabe que precisa chamar o método notificar. Isso torna o sistema mais flexível e desacoplado.

Na prática, não é possível evitar totalmente a dependência de detalhes, em algum ponto do sistema, será necessário usar uma implementação concreta (por exemplo, criar uma instância de NotificadorEmail). No entanto, a ideia é concentrar esses detalhes nas bordas da aplicação, como em uma camada de infraestrutura. Assim, a parte central do sistema continua limpa, estável e fácil de testar ou modificar.

---

## Princípios dos componentes

Os princípios SOLID ajudam a organizar bem classes e funções em sistemas menores. Porém, em sistemas maiores, é necessário ir além e dividir o software em componentes — grupos de classes que trabalham juntas em uma funcionalidade específica. Essa divisão torna o sistema mais modular, reutilizável, fácil de manter e escalável. Sistemas grandes devem ser construídos a partir de componentes menores e bem definidos.

---

## Componentes 

Componentes são unidades de implantação compostas por várias classes e recursos que são construídos, testados e implantados juntos. São blocos de código independentes, responsáveis por funcionalidades específicas dentro de um sistema.

No início da computação, era necessário conhecer com precisão o tamanho dos programas, pois a memória não podia ser alocada dinamicamente. Com o avanço da tecnologia, surgiram técnicas como relocação e memória virtual, permitindo a execução de programas maiores. No entanto, isso também trouxe desafios relacionados à performance e organização.

Dividir um sistema em componentes bem definidos permite melhor organização, reutilização de código, facilidade de manutenção e escalabilidade.

---

## Coesão de componentes

Os princípios de coesão de componentes ajudam a definir onde cada classe deve estar e como organizar os componentes de forma mais lógica e sustentável ao longo do tempo.

REP (Release Reuse Equivalency Principle): funcionalidades devem ser agrupadas de forma que façam sentido serem versionadas e liberadas juntas. Isso evita um monte de coisa solta e incompatível em um único componente.

CCP (Common Closure Principle): apenas o que realmente muda junto deve estar junto. Se partes do código não forem reutilizadas juntas, melhor separá-las em componentes diferentes para evitar dependências desnecessárias.

CRP (Common Reuse Principle): quanto menos acoplamento, melhor. Devemos evitar criar vínculos entre componentes que não precisam estar conectados.

Na prática, não dá pra seguir os três princípios ao mesmo tempo o tempo todo. Às vezes, ao tentar agrupar por reutilização, você quebra a lógica de liberação em conjunto, e vice-versa. O ideal é ir ajustando conforme o projeto evolui, decidindo o que é mais importante em cada momento: facilidade de manutenção, reutilização ou independência entre componentes.

---

## Acoplamento de componentes

O princípio das dependências acíclicas diz que não se deve permitir ciclos no grafo de dependência dos componentes. Em projetos grandes, quando vários desenvolvedores mexem no mesmo código, coisas que antes funcionavam podem parar de funcionar. Antigamente, para tentar evitar esse problema, usava-se o build semanal, onde cada um trabalhava isolado e, na sexta-feira, tudo era juntado. Porém, em projetos maiores isso se torna inviável. A solução encontrada foi dividir o sistema em componentes que pudessem ter suas próprias versões liberadas independentemente. Assim, cada equipe decide se quer usar a nova versão ou continuar na anterior, sem depender do restante do projeto para seguir com seu trabalho. Para que isso funcione, é necessário gerenciar a estrutura de dependências entre os componentes, e o ideal é que essa estrutura seja um grafo acíclico direcionado. Com isso, fica fácil acompanhar o que mudou e organizar as atualizações na ordem correta, sem travar o trabalho das outras equipes.

### O Efeito dos Ciclos e Como Quebrá-los
Quando ocorrem ciclos entre componentes, os desenvolvedores precisam atualizar tudo ao mesmo tempo, porque qualquer alteração em um componente afeta imediatamente os outros, o que elimina a autonomia e a flexibilidade. Para quebrar esses ciclos existem dois caminhos: o primeiro é aplicar o Princípio da Inversão de Dependência (DIP), onde as dependências apontam para abstrações; o segundo é criar um componente intermediário no qual os outros componentes passam a depender. O problema dessa segunda alternativa é que ela deixa a estrutura volátil, pois à medida que o sistema cresce, as dependências podem se concentrar nesse componente, aumentando a fragilidade do projeto.

### Crescimento e Planejamento da Estrutura
É importante entender que não dá para planejar toda a estrutura de componentes de um sistema desde o início. Mesmo que tentássemos, ao final acabaríamos criando um monte de dependências desnecessárias. Por isso, a arquitetura deve ser planejada e organizada conforme o sistema for crescendo e as necessidades forem surgindo.

### O Princípio das Dependências Estáveis (SDP)
Esse princípio determina que devemos tentar manter os componentes mais difíceis de mudar separados dos mais voláteis. Um componente é considerado estável quando outros componentes dependem dele. Isso acontece porque, se ele mudar, será necessário adaptar todos que dependem dele, o que gera um custo alto. Para medir a estabilidade de um componente, conta-se o número de dependências que entram e o número que saem. O SDP (Stable Dependencies Principle) diz que o número de dependências que entram deve ser maior do que o número de dependências que saem. Porém, nem todos os componentes devem ser estáveis. Para que um projeto fosse totalmente estável, ele precisaria ser imutável, o que não faz sentido. Por isso, uma boa convenção é organizar os componentes mais instáveis no topo do diagrama de dependências. Assim, qualquer dependência que apontar para cima estará violando o SDP. E, para corrigir, usa-se o DIP.

### O Princípio das Abstrações Estáveis (SAP)
Em linguagens estaticamente tipadas, às vezes é necessário criar componentes só de interfaces ou classes abstratas para manter o sistema desacoplado. Isso leva ao princípio das abstrações estáveis, que diz que um componente deve ser tão abstrato quanto estável. As políticas de alto nível devem ser colocadas nos componentes estáveis, para evitar que fiquem voláteis. Mas, para que esses componentes estáveis não se tornem rígidos e inflexíveis, aplica-se o princípio do aberto-fechado (OCP), criando classes abstratas que podem ser estendidas sem precisar serem modificadas diretamente.

### Combinando SDP e SAP
Combinando o SAP (Stable Abstractions Principle) e o SDP, forma-se um princípio aplicável a componentes, onde as dependências devem apontar na direção da estabilidade e da abstração. Assim, um componente pode ser parcialmente abstrato e parcialmente estável, mantendo um bom equilíbrio no projeto. Para organizar isso visualmente, costuma-se usar um gráfico de estabilidade versus abstração, onde os componentes são posicionados conforme seu nível de estabilidade e abstração.

### Zonas do Gráfico de Estabilidade e Abstração
Nesse gráfico, existem três regiões principais: a zona da dor, a zona da inutilidade e a sequência principal. A zona da dor é onde ficam os componentes concretos e muito estáveis, como bancos de dados. Esses componentes são perigosos porque qualquer mudança neles afeta o sistema inteiro. Por outro lado, os componentes voláteis, que não mudam muito, não causam problemas nessa zona. Na zona da inutilidade ficam os componentes muito abstratos e que não têm dependentes, geralmente restos de código ou interfaces não implementadas, que não servem para nada. A sequência principal é a linha ideal entre estabilidade e abstração, onde os componentes bem projetados devem se posicionar, equilibrando flexibilidade e segurança. Não é possível manter tudo sempre nessa linha, mas o importante é evitar que os componentes fiquem muito distantes dela. Qualquer componente que esteja muito afastado da sequência principal precisa ser reavaliado e possivelmente reestruturado.

### Conclusão
A conclusão é que essas métricas e princípios ajudam a manter o projeto desacoplado, flexível, sustentável e fácil de manter conforme cresce.

---

## O que é arquitetura? 

A principal função da arquitetura de software é reduzir o custo da vida útil do sistema. O objetivo de um arquiteto não é maximizar a produtividade do programador no curto prazo, mas garantir que o software continue fácil de manter e evoluir ao longo do tempo. Um arquiteto deve continuar programando para manter contato com os desafios reais do código e, assim, tomar decisões melhores. É responsabilidade dele decidir as tecnologias utilizadas com base na performance e nas regras de negócio, mesmo que alguém tenha decidido diferente antes, mantendo o sistema flexível e preparado para mudanças futuras.

A arquitetura deve ser planejada desde o início do projeto. Em equipes pequenas, pode ser uma estrutura mais leve, mas ainda assim precisa existir. Em equipes maiores, deve-se estruturar bem os componentes e responsabilidades de cada parte do sistema para que o desenvolvimento siga um padrão organizado. Além disso, é importante que a arquitetura facilite o processo de implantação, evitando dependências desnecessárias que dificultem a instalação, atualização ou manutenção.

Durante a operação do sistema, uma boa arquitetura evita soluções paliativas, como adicionar hardware desnecessário para compensar problemas de software, pois o foco deve ser administrar bem os recursos, garantindo eficiência. Na fase de manutenção, que é a etapa mais cara da vida de um software, uma boa arquitetura reduz os custos e a dificuldade para adicionar novas funcionalidades ou corrigir falhas, tornando o processo mais seguro e rápido.

Outro ponto fundamental é manter as opções de tecnologia sempre abertas. O sistema não deve ficar preso a frameworks, bancos de dados ou dispositivos específicos sem necessidade. Isso permite que, caso surjam novas soluções melhores, elas possam ser adotadas sem grandes impactos. Por fim, a arquitetura deve garantir a independência de dispositivo, ou seja, o software não pode depender de hardware ou sistemas operacionais específicos e precisa ser fácil de adaptar para diferentes plataformas e ambientes.

Em resumo, arquitetura é sobre manter o sistema saudável e flexível durante toda a sua vida útil, protegendo a regra de negócio e facilitando mudanças, sem se apegar a tecnologias ou soluções passageiras.

---

## Independência

Uma boa arquitetura deve ser capaz de suportar os casos de uso do sistema, facilitar a manutenção, permitir que o desenvolvimento aconteça de forma independente entre as equipes e possibilitar uma implantação rápida e eficiente. Os casos de uso precisam ser claros e visíveis na estrutura do sistema, com nomes e organizações que deixem evidente o que o sistema faz. Por exemplo, em um sistema de pedidos, deve ficar claro quais são os casos de adicionar ou excluir um pedido.

A operação do sistema deve acontecer de forma eficiente, garantindo desempenho, confiabilidade e facilidade de operação. No desenvolvimento, é importante que diferentes equipes consigam trabalhar sem que uma interfira no trabalho da outra, o que só é possível se os componentes do sistema estiverem bem separados. Isso também se reflete na implantação, já que, com o desacoplamento bem feito, é mais fácil adicionar novos casos de uso e publicar atualizações sem comprometer o restante do sistema.

Como na prática não é possível prever tudo, a arquitetura deve manter o maior número de opções abertas pelo máximo de tempo possível. Para isso, é essencial aplicar princípios como o da responsabilidade única e o do fechamento comum, que ajudam a separar elementos que mudam por motivos diferentes e agrupar aqueles que mudam pelos mesmos motivos.

O desacoplamento dos casos de uso consiste em separar a interface de usuário e as regras de negócio de cada caso de uso, mantendo-os organizados verticalmente no sistema. Assim, novos casos podem ser adicionados sem impactar os antigos. Isso também permite que banco de dados e interface sejam agrupados conforme os casos de uso que atendem.

Existem diferentes formas de desacoplar componentes: no nível de código-fonte, controlando as dependências para evitar recompilar tudo; no nível binário, controlando dependências entre bibliotecas ou DLLs para evitar reimplantação desnecessária; e no nível de serviço, controlando dependências até o ponto em que cada unidade de execução funcione de forma independente, como em serviços ou microserviços. O melhor modo de desacoplamento é aquele que oferece o melhor custo-benefício no momento, e a arquitetura deve permitir mudar isso conforme o projeto evolui.

Por fim, é importante evitar unificar elementos que não sejam realmente iguais. Se duas funcionalidades ou telas forem apenas parecidas, mas mudarem por razões diferentes, elas devem permanecer separadas para evitar problemas futuros.

---

## Fronteiras: Estabelecendo Limite

A arquitetura de software serve para manter o sistema desacoplado e proteger as regras de negócio. O principal objetivo da arquitetura é atender corretamente ao domínio, e todas as decisões técnicas, como banco de dados, frameworks e serviços externos, devem ser adiadas até que sejam realmente necessárias.

Para isso, o sistema precisa aplicar o princípio da Inversão de Dependência, onde os detalhes técnicos devem depender das regras de negócio, e não o contrário. Assim, é possível trocar tecnologias sem precisar alterar a lógica principal do sistema.

Deve-se organizar o projeto respeitando o Princípio da Responsabilidade Única (SRP), que afirma que cada módulo ou componente deve ter um único motivo para mudar. Isso significa que o que muda pelos mesmos motivos fica junto, e o que muda por motivos diferentes fica separado.

Além disso, é importante utilizar Abstrações Estáveis, criando interfaces que protegem as regras de negócio das mudanças externas. Assim, qualquer tecnologia externa, como banco de dados ou APIs, se conecta ao sistema por meio dessas interfaces.

Para manter o sistema flexível e preparado para mudanças, é fundamental desacoplar as camadas, tratando detalhes externos como plugins, que se comunicam com o sistema via interfaces. Esse conceito é conhecido como Componentização, onde o sistema é dividido em partes independentes.

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


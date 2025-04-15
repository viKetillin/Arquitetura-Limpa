# Resumo: Arquitetura Limpa

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

---

## Conclusão

A organização do código impacta diretamente a produtividade e a evolução do software. Um código limpo facilita a manutenção, reduz erros e melhora a eficiência da equipe.

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

Programação Estruturada
A programação estruturada surgiu como uma alternativa ao código desorganizado e caótico dos primeiros programas de computador, onde o uso excessivo do goto tornava o fluxo de execução difícil de seguir.

Em 1968, Edsger Dijkstra publicou o artigo "Go To Statement Considered Harmful", que marcou uma virada para um estilo de programação mais disciplinado e organizado. Esse modelo foi adotado para tornar o código mais previsível, modular e fácil de entender.

Princípios da Programação Estruturada
A programação estruturada se baseia em três estruturas de controle fundamentais:

Sequência: as instruções são executadas uma após a outra, na ordem em que aparecem.

Seleção: decisões condicionais permitem que o programa siga caminhos diferentes (ex.: if, switch).

Repetição: permite a execução repetitiva de blocos de código (ex.: for, while).

Com essas estruturas, é possível escrever qualquer programa sem a necessidade de comandos como goto, garantindo um código mais organizado e legível.

Estrutura e Arquitetura
A programação estruturada é um pilar essencial para a arquitetura limpa, pois fornece uma base sólida para a organização do código. No entanto, apesar de ser um avanço importante, ela não resolve sozinha todos os problemas de software.

A arquitetura limpa vai além, aplicando princípios como:

Separação de responsabilidades

Inversão de dependências

Modularização

Esses princípios permitem que sistemas grandes sejam mantidos e escalados ao longo do tempo com mais facilidade.

Conclusão
A programação estruturada foi um divisor de águas na engenharia de software, reduzindo a complexidade do código e melhorando sua manutenibilidade.

No entanto, para aplicações modernas, ela deve ser combinada com princípios arquiteturais sólidos, como os da arquitetura limpa, garantindo que o código continue sustentável e flexível conforme o sistema cresce.

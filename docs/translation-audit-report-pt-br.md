# Auditoria e correções da tradução PT-BR


## Estado das correções — 13/10/2026

A revisão de outubro comparou as 186 proposições rotuladas em português (188 blocos `\problem`,
pois III.VIII está subdividida) com seus
correspondentes em inglês no commit `e09e323`. As correções foram separadas
em commits por assunto na branch `fix/translation-audit-findings`.

- As conclusões verbais de II.II–XI e a afirmação direta de VI.II foram restauradas.
- III.XXVI–XXIX e VI.XXXIII agora exigem círculos iguais; a proporção de VI.XXXIII foi recomposta.
- VI.XV exige igualdade de área; VI.XXII usa terceiras proporcionais;
  VI.XXVI trata da disposição sobre a mesma diagonal, não de comprimentos iguais.
- O Livro V distingue razão de proporção e preserva as hipóteses de múltiplos,
  a ordem de comparação e as relações por conversão.
- As construções usam prolongar, traçar, cordas, partes e ângulos do vértice;
  as condições espaciais usam fora da figura e sobre a circunferência.
- A classe gera Livro e hip. para o português brasileiro e contém a localização
  dos tipos de referência. Os títulos, casos e capitulares remanescentes foram traduzidos.
- A Introdução recebeu correções de calques, concordância e ortografia.
- Os lapsos algébricos herdados foram corrigidos também no inglês. As negações
  duplicadas de `\ngtr` e `\neq` eram da tradução portuguesa; a notação ambígua
  de V.X foi esclarecida nas duas edições.
- IV.XVI enuncia a inscrição do quindecágono no círculo dado e VI.D explicita
  a soma dos retângulos, nas duas edições.

### Inventário de atendimento

Os IDs abaixo pertencem à auditoria de outubro. As faixas de linhas registradas
nas issues são do snapshot anterior à correção.

| ID | Achado | Atendimento |
| --- | --- | --- |
| F01 | A edição portuguesa não está na branch padrão | README documenta a branch e a compilação; integração em master depende de merge |
| F02 | [Dez enunciados do Livro II perderam a conclusão em palavras](https://github.com/brenorb/byrne-euclid/issues/2) | Corrigido |
| F03 | [A primeira metade do teorema VI.II foi cortada](https://github.com/brenorb/byrne-euclid/issues/2) | Corrigido |
| F04 | [Círculos iguais viraram desiguais em cinco proposições](https://github.com/brenorb/byrne-euclid/issues/3) | Corrigido |
| F05 | [VI.XV omite que os triângulos devem ter áreas iguais](https://github.com/brenorb/byrne-euclid/issues/4) | Corrigido |
| F06 | [VI.XXVI transforma alinhamento de diagonais em igualdade de comprimentos](https://github.com/brenorb/byrne-euclid/issues/4) | Corrigido |
| F07 | [VI.XXII confunde terceira proporcional com um terço](https://github.com/brenorb/byrne-euclid/issues/4) | Corrigido |
| F08 | [VI.XXIV e VI.XXXII ficaram com enunciados sintaticamente quebrados](https://github.com/brenorb/byrne-euclid/issues/4) | Corrigido |
| F09 | [VI.XXXIII perdeu o sinal que iguala as duas razões](https://github.com/brenorb/byrne-euclid/issues/3) | Corrigido |
| F10 | [V.V perdeu a hipótese do mesmo múltiplo nas partes retiradas](https://github.com/brenorb/byrne-euclid/issues/5) | Corrigido |
| F11 | [V.IX e V.X perderam o objeto da comparação de razões](https://github.com/brenorb/byrne-euclid/issues/5) | Corrigido |
| F12 | [Razão recebe traduções técnicas incompatíveis](https://github.com/brenorb/byrne-euclid/issues/5) | Corrigido |
| F13 | [A definição V.XX perde a ordem de comparação e altera o latinismo](https://github.com/brenorb/byrne-euclid/issues/5) | Corrigido |
| F14 | [Convertendo e V.XIX têm termos sem sentido matemático](https://github.com/brenorb/byrne-euclid/issues/5) | Corrigido |
| F15 | [O axioma V.I ficou tautológico](https://github.com/brenorb/byrne-euclid/issues/5) | Corrigido |
| F16 | [Without foi traduzido como ausência em vez de posição externa](https://github.com/brenorb/byrne-euclid/issues/6) | Corrigido |
| F17 | [III.XVII permite um ponto interior para a tangente](https://github.com/brenorb/byrne-euclid/issues/6) | Corrigido |
| F18 | [III.XVI perdeu a posição do ponto entre a perpendicular e o círculo](https://github.com/brenorb/byrne-euclid/issues/6) | Corrigido |
| F19 | [Produce / drawn / meet recebem traduções que mudam a construção](https://github.com/brenorb/byrne-euclid/issues/6) | Corrigido |
| F20 | [Falsos amigos adicionais no vocabulário geométrico](https://github.com/brenorb/byrne-euclid/issues/6) | Corrigido |
| F21 | [A definição III.III perdeu o critério de encontro dos círculos](https://github.com/brenorb/byrne-euclid/issues/6) | Corrigido |
| F22 | [Ainda há palavras e títulos não traduzidos no conteúdo visível](https://github.com/brenorb/byrne-euclid/issues/7) | Corrigido |
| F23 | [A classe compõe Book e hyp. na edição brasileira](https://github.com/brenorb/byrne-euclid/issues/7) | Corrigido |
| F24 | Calques na Introdução prejudicam a leitura e o sentido | Corrigido |
| F25 | [IV.XVI pede a construção errada já no inglês](https://github.com/brenorb/byrne-euclid/issues/8) | Corrigido |
| F26 | [Há lapsos simbólicos herdados que sobrevivem na tradução](https://github.com/brenorb/byrne-euclid/issues/8) | Lapsos herdados corrigidos em EN/PT; dupla negação da tradução corrigida em PT |
| F27 | [VI.D/Ptolomeu precisa explicitar a soma dos retângulos](https://github.com/brenorb/byrne-euclid/issues/8) | Corrigido |
| F28 | A conclusão do relatório anterior não descreve o estado auditado | Este relatório substitui a conclusão anterior |

### Validação

- LuaLaTeX / TeX Live 2026, em duas passagens por edição: PT-BR com 278 páginas,
  EN com 271 e RU com 284. Nenhum erro fatal, caractere ausente ou referência
  indefinida nos logs finais.
- Preservados os 188 blocos de enunciados, os rótulos das 186 proposições,
  77 definições, 15 axiomas e 3 postulados da edição portuguesa.
- Varredura das fontes e do texto extraído sem títulos `Theor.`/`theor.`,
  `Case`, `consequently`, `Book` ou `hyp.` remanescentes no conteúdo português.
- Inspeção visual de páginas afetadas pelas conclusões restauradas, pela
  igualdade de áreas, pela relação entre arcos, pela comparação de múltiplos
  e pelo teorema de Ptolomeu. Os três URLs bibliográficos foram preservados.
- Permanecem avisos tipográficos de caixas e de níveis de bookmarks do projeto;
  isso não equivale a uma revisão visual integral de todas as páginas.

O CI compila as três edições em duas passagens, incluindo PT-BR, e usa a
biblioteca Byrne no commit `08c138e09a4ec6326f9c5e3c3b1bfd2201fb695d`.
Comentários de código, títulos bibliográficos originais, versos latinos com
tradução, Q.E.D./Q.E.F. e a decisão editorial de `trapezium/trapezia` foram preservados.

## Histórico da auditoria inicial

As seções seguintes registram o diagnóstico anterior às correções de julho.
Elas não descrevem o estado atual da tradução.

## Escopo

Este relatório revisa `byrne-pt-br-latex.tex` de forma adversarial, com foco em:

1. trechos que permaneceram em inglês;
2. escolhas terminológicas que perdem distinções matemáticas importantes;
3. calques e verbos de construção geométrica pouco naturais em PT-BR;
4. um glossário mínimo para orientar a correção dos Livros II-VI.

## Método

- Comparei `byrne-pt-br-latex.tex` com `byrne-en-latex.tex`.
- Localizei os blocos não traduzidos por faixa de linhas.
- Cruzei os termos com fontes em português de uso matemático real:
  - tradução portuguesa histórica de Euclides/Commandino/Simson;
  - verbetes técnicos em português;
  - material escolar brasileiro para terminologia moderna.

## Fontes-base

Os links completos usados nesta discussão ficam concentrados nesta seção, para que a nota do tradutor e o corpo do relatório possam remeter apenas às chaves bibliográficas `[F6]`, `[F7]` e `[F8]` sem sobrecarregar a redação.

- **[F1]** `byrne-pt-br-latex.tex` e `byrne-en-latex.tex` deste repositório.
- **[F2]** Euclides, *Elementos de Geometria* (Commandino/Simson, 1944): <https://fontesdealencar.org/wp-content/uploads/2018/12/Euclides-Elementos-de-Geometria.pdf>
- **[F3]** Wikipédia, **Quadrilátero**: <https://pt.wikipedia.org/wiki/Quadril%C3%A1tero>
- **[F4]** Wikipédia, **Romboide**: <https://pt.wikipedia.org/wiki/Romboide>
- **[F5]** Brasil Escola, **Quadriláteros**: <https://brasilescola.uol.com.br/matematica/quadrilateros.htm>
- **[F6]** Κέντρο Ελληνικής Γλώσσας, *Λεξικό της Κοινής Νεοελληνικής*, verbete **τραπέζιο**: <https://www.greek-language.gr/greekLang/modern_greek/tools/lexica/triantafyllides/search.html?lq=%CF%84%CF%81%CE%B1%CF%80%CE%AD%CE%B6%CE%B9%CE%BF>
- **[F7]** ΙΕΠ / Υπουργείο Παιδείας (material escolar oficial), nota histórica sobre a classificação de Euclides e o uso posterior em Arquimedes: <https://prosvasimo.iep.edu.gr/Books/Eidikh-Agwgh-PI/books/a_likeiou/l_a_arial-18b/l_a_geom_arial_18b/l_a-b_geom_bm_%2895-180%29_18b.pdf>
- **[F8]** Wolfram MathWorld, **Trapezium**: <https://mathworld.wolfram.com/Trapezium.html>

## Resumo executivo da auditoria inicial

O problema mais grave não é terminológico: os **Livros II a VI continuam majoritariamente em inglês**. Isso significa que a tradução hoje está completa só até o fim do Livro I.

Entre os trechos já traduzidos, há dois problemas de alta gravidade:

1. `rhomboid` foi achatado para `paralelogramo`, apagando a distinção entre **romboide** e **paralelogramo**;
2. `oblong` virou `retângulo alongado`, solução compreensível, mas pior do que a tradição técnica/histórica (`oblongo`) e menos consistente com o vocabulário euclidiano.

Há também problemas de registro técnico:

- `legs` -> `pernas`;
- `draw` -> `desenhar`, onde o português geométrico prefere `traçar`;
- `straight line may be drawn` -> `linha reta possa ser desenhada`, menos idiomático que `se tire` / `se trace`.

## Achados principais

| Severidade | Ocorrência na auditoria inicial | Problema | Motivo | Sugestão | Fontes |
| --- | --- | --- | --- | --- | --- |
| Alta | `byrne-pt-br-latex.tex:3622-4602` (`\part{Book II}`) | Livro II segue em inglês | Não é uma escolha ruim de tradução; é ausência de tradução | Traduzir integralmente o Livro II, começando pelas definições e títulos de proposições | [F1] |
| Alta | `byrne-pt-br-latex.tex:4603-7272` (`\part{Book III}`) | Livro III segue em inglês | Mesmo problema estrutural do Livro II | Traduzir integralmente o Livro III | [F1] |
| Alta | `byrne-pt-br-latex.tex:7273-8520` (`\part{Book IV}`) | Livro IV segue em inglês | Mesmo problema estrutural do Livro II | Traduzir integralmente o Livro IV | [F1] |
| Alta | `byrne-pt-br-latex.tex:8521-10632` (`\part{Book V}`) | Livro V segue em inglês | Mesmo problema estrutural do Livro II | Traduzir integralmente o Livro V | [F1] |
| Alta | `byrne-pt-br-latex.tex:10633-13115` (`\part{Book VI}`) | Livro VI segue em inglês | Mesmo problema estrutural do Livro II | Traduzir integralmente o Livro VI | [F1] |
| Alta | `byrne-pt-br-latex.tex:985` | `rhomboid` foi traduzido como `paralelogramo` | Em Euclides, `rhomboid` é uma espécie particular; `parallelogram` é a classe mais ampla usada depois nas proposições. A troca destrói uma distinção geométrica real | `romboide` | [F2], [F3], [F4] |
| Média-alta | `byrne-pt-br-latex.tex:453` e `:965` | `oblong` virou `retângulo alongado` | É inteligível, mas não é o termo euclidiano consagrado em português. A tradição histórica registra `oblongo`; o resumo sobre quadriláteros em português também preserva `oblongo` | Preferir `oblongo`; alternativa editorial: `retângulo (oblongo)` na primeira ocorrência | [F2], [F3] |
| Média | `byrne-pt-br-latex.tex:593` | `legs` virou `pernas` | Em PT-BR matemático, triângulo tem `lados`; `pernas` soa como calque do inglês e destoa do resto do texto | Preferência editorial: `dois de seus lados são iguais` | [F1], [F2] |
| Média | `byrne-pt-br-latex.tex:1620` | `draw a perpendicular` virou `desenhar uma perpendicular` | Em construções geométricas, o registro consagrado é `traçar`, `tirar`, `erguer`, `descrever`; `desenhar` enfraquece o tom técnico | `traçar uma perpendicular` | [F2] |
| Média | `byrne-pt-br-latex.tex:1012` | `straight line may be drawn` virou `linha reta possa ser desenhada` | O português geométrico clássico e escolar prefere formulações como `se tire`, `se trace` | `Seja concedido que se trace uma reta de qualquer ponto a qualquer outro ponto` | [F2] |
| Média | `byrne-pt-br-latex.tex:453` | `A line drawn from the centre...` virou `Uma linha desenhada...` | Mesmo problema de registro técnico: em geometria, `traçada` / `conduzida` é mais natural que `desenhada` | `Uma reta traçada do centro...` ou `Uma reta conduzida do centro...` | [F2] |

## Observação importante sobre `trapézios` / `trapezium`

`byrne-pt-br-latex.tex:990` traduz `trapeziums` como `trapézios`.

Isso **não é um erro simples de dicionário**, mas um conflito entre:

- o uso euclidiano/histórico, em que `trapezia` designa os quadriláteros residuais ([F2], [F8]);
- o uso moderno do português escolar, em que `trapézio` significa um quadrilátero com um par de lados paralelos ([F5]);
- o uso moderno do grego, em que `τραπέζιο` também significa o quadrilátero com duas lados opostos paralelos, como registra o **Λεξικό της Κοινής Νεοελληνικής**: “το τετράπλευρο του οποίου οι δύο απέναντι πλευρές είναι παράλληλες και άνισες” ([F6]);
- a observação histórica do material oficial grego, segundo a qual em Euclides `τραπέζιο` significa “qualquer quadrilátero”, enquanto “com a acepção moderna” o termo aparece depois em Arquimedes ([F7]).

Por isso, a solução editorial mais robusta para esta tradução é:

1. **não traduzir esse termo por `trapézio` no corpo principal**;
2. manter **`trapezium`**;
3. inserir **nota do tradutor** na primeira ocorrência, explicando que:
   - o termo euclidiano não coincide com o `trapézio` moderno do português;
   - o mesmo desencontro existe também em grego moderno;
   - a acepção moderna é posterior e já aparece associada a Arquimedes ([F7], [F8]).

Em outras palavras: aqui `trapézio` em português **induz falso cognato histórico**. A manutenção de `trapezium` com nota é uma decisão melhor do que traduzir mecanicamente.

### Formulação sugerida para a nota do tradutor

> Mantém-se aqui o termo *trapezium* para evitar confusão com o **trapézio** moderno. Em Euclides, o termo grego correspondente não designa o quadrilátero com um par de lados paralelos, mas a classe residual dos quadriláteros que não são quadrado, oblongo, losango ou romboide. Já no uso moderno, tanto em português quanto em grego, o termo passou a designar o quadrilátero com dois lados opostos paralelos. Cf. o *Λεξικό da Língua Grega Moderna*, verbete **τραπέζιο**; e o manual do ΙΕΠ, p. 46: “Τραπέζιο ονομάζει όχι ό,τι σήμερα εννοούμε με τον όρο αυτό, δηλαδή τετράπλευρο με δύο μόνο πλευρές παράλληλες, αλλά οποιοδήποτε τετράπλευρο. Ο όρος τραπέζιο, με τη σύγχρονη έννοια, απαντάται αργότερα στον Αρχιμήδη” (*tradução livre*: “Ele chama de trapézio não aquilo que hoje entendemos por esse termo, isto é, um quadrilátero com apenas dois lados paralelos, mas qualquer quadrilátero. O termo trapézio, no sentido moderno, aparece mais tarde em Arquimedes.”). Ver referências [F6], [F7] e [F8] na bibliografia deste relatório.

### Decisão editorial registrada

Preferência para a edição PT-BR:

- usar **`trapezium` / `trapezia`** em latim;
- incluir **nota de rodapé** explicando que o latinismo foi mantido porque o sentido histórico da palavra em Euclides **não coincide** com o uso moderno corrente nem em inglês nem no grego moderno;
- evitar `trapézio` no corpo principal dessa definição, porque hoje ele puxa automaticamente uma leitura escolar moderna que não corresponde ao valor classificatório euclidiano original.

## Glossário de correção para os Livros II-VI

Os itens abaixo já aparecem em inglês no arquivo PT-BR e deveriam ser normalizados com o vocabulário técnico em português.

| Termo atual em inglês | Primeira ocorrência em `byrne-pt-br-latex.tex` | Sugestão PT-BR | Observação | Fonte de uso |
| --- | --- | --- | --- | --- |
| `A rectangle` / `right angled parallelogram` | `3642` | `retângulo` / `paralelogramo retângulo` | O texto português histórico usa `paralelogramo retângulo` e `retângulo compreendido por...` | [F2] |
| `contained by` | `3642` | `compreendido por` | Fórmula euclidiana recorrente: “retângulo compreendido por...” | [F2] |
| `Gnomon` | `3679` | `gnômon` | Termo técnico já atestado em português matemático | [F2] |
| `Equal circles are those whose diameters are equal` | `4608` | `Círculos iguais são os que têm diâmetros iguais` | Fórmula direta e idiomática | [F2] |
| `touch a circle` / `tangent` | `4621` em diante | `tocar um círculo` / `ser tangente a` | A tradução portuguesa usa `toca um círculo` e `é tangente de um círculo` | [F2] |
| `inscribed in` | `7295` | `inscrito em` | Vocabulário padrão de geometria plana | [F2] |
| `circumscribed about` | `7298` | `circunscrito a` | Vocabulário padrão de geometria plana | [F2] |
| `aliquot part or submultiple` | `8526` | `parte alíquota ou submúltiplo` | Pode modernizar levemente, mas convém preservar o termo técnico | [F2] |
| `multiple` | `8529` | `múltiplo` | Padrão | [F2] |
| `ratio` | `8532` | `razão` | Padrão | [F2] |
| `Equimultiples or equisubmultiples` | `8546` | `equimúltiplos ou equissubmúltiplos` | Se quiser sabor clássico, `eqüimultíplices` também é atestado | [F2] |
| `duplicate ratio` | `10132` | `razão duplicada` | Termo técnico estabilizado na tradição euclidiana em português | [F2] |
| `triplicate ratio` | `10157` | `razão triplicada` | Mesma observação do item anterior | [F2] |
| `compound ratio` | `10196` | `razão composta` | Termo técnico explícito na tradição portuguesa de Euclides | [F2] |
| `homologous` | `5098` e passim | `homólogos` / `homólogas` | Ex.: `lados homólogos`, `grandezas homólogas` | [F2] |
| `reciprocally proportional` | `10670` e passim | `reciprocamente proporcionais` | Fórmula técnica padrão | [F2] |
| `extreme and mean ratio` | `10673` | `extrema e média razão` | Tradução técnica consolidada do corte áureo em chave euclidiana | [F2] |
| `mean proportional` | `11526` | `média proporcional` | Padrão em geometria e álgebra escolar | [F2] |
| `similar` / `similarly placed` | `10667` e passim | `semelhantes` / `semelhantemente postos` | O português histórico usa `postos`; PT-BR moderno aceita `dispostos` | [F2] |

## Prioridade prática de correção

Se a meta for fechar a tradução com o menor risco técnico possível, a ordem correta é:

1. **Corrigir `romboide` imediatamente**.
2. **Decidir a política editorial para `oblong`**: histórica (`oblongo`) ou mista (`retângulo oblongo` / `retângulo (oblongo)`).
3. **Padronizar o léxico de construção**: `traçar`, `descrever`, `prolongar`, `tirar`.
4. **Traduzir integralmente os Livros II-VI**.
5. Durante essa tradução, aplicar o glossário acima antes de revisar estilo fino.

## Conclusão da auditoria inicial

O arquivo atual não está “quase pronto com alguns termos ruins”; ele está em um estado misto:

- **Livro I**: traduzido, mas com alguns pontos terminológicos a corrigir;
- **Livros II-VI**: ainda substancialmente em inglês.

O ponto mais perigoso para o sentido matemático é `rhomboid -> paralelogramo`. O segundo maior problema é estrutural: a falsa impressão de completude da edição PT-BR, quando mais de dois terços do conteúdo técnico ainda não foram vertidos.

## Verificação de julho de 2026 (substituída)

A revisão de julho registrou a tradução dos cinco livros finais e a correção
 de `romboide`, `oblongo`, `lados`, `traçar` e da nota sobre `trapezium`.
Essas correções estão presentes. Porém, a conclusão de que não havia achados
acionáveis adicionais foi substituída pela revisão de 13/10/2026: o commit
`e09e3236540c25ee77431cfe0cd90e50ff2c5637` ainda continha conclusões verbais
omitidas e erros de sentido, além de resíduos de idioma.

As referências da nota do tradutor usam `[B1]`, `[B2]` e `[B3]` na bibliografia
do volume. Os códigos `[F...]` da auditoria histórica abaixo são fontes
bibliográficas e não devem ser confundidos com os IDs dos achados de outubro.

## Anexo A: Evidências sobre `trapezium` / `τραπέζιον`

Esta seção resume a base documental para a decisão de manter o latinismo `trapezium` / `trapezia`.

### 1. Inglês de Euclides

No texto inglês de referência, a definição aparece como:

> `All other quadrilateral figures are called trapeziums.`

Isso mostra que o termo funciona como **classe residual** dentro da taxonomia dos quadriláteros em Euclides, e não como simples equivalente automático do trapézio escolar moderno.

Fontes:

- [F1]
- [Euclid’s Elements of Geometry](https://www.ms.uky.edu/~sohum/ma330/files/Elements.pdf)

### 2. Grego antigo de Euclides

O texto grego traz:

> `τὰ δὲ παρὰ ταῦτα τετράπλευρα τραπέζια καλείσθω`
> Tradução: `e os quadriláteros além desses sejam chamados trapezia`

Isso confirma que o termo original de Euclides é o grego antigo `τραπέζια`, plural de `τραπέζιον`, e que o valor ali é classificatório: os quadriláteros que restam depois de quadrado, oblongo, losango e romboide.

Fonte:

- [Euclid’s Elements of Geometry](https://www.ms.uky.edu/~sohum/ma330/files/Elements.pdf)

### 3. Etimologia grega

O substantivo antigo é:

> `τραπέζιον`
> Tradução: `mesinha`, literalmente um diminutivo de `mesa`

Etimologicamente, o termo deriva de:

> `τράπεζα`
> Tradução: `mesa`

Isso ajuda a explicar por que o campo semântico original não coincide exatamente com as classificações geométricas escolares modernas.

Fonte:

- [Wiktionary, τραπέζιον](https://en.wiktionary.org/wiki/%CF%84%CF%81%CE%B1%CF%80%CE%AD%CE%B6%CE%B9%CE%BF%CE%BD)

### 4. Grego moderno escolar

No grego moderno escolar atual, `τραπέζιο` já tem o valor moderno de trapézio:

> `Το τετράπλευρο που έχει δύο μόνον πλευρές παράλληλες λέγεται τραπέζιο`
> Tradução: `O quadrilátero que tem somente duas lados paralelos chama-se trapézio`

Ou ainda:

> `Ένα τετράπλευρο ονοµάζεται τραπέζιο όταν έχει δύο µόνο απέναντι πλευρές παράλληλες`
> Tradução: `Um quadrilátero chama-se trapézio quando tem somente duas lados opostos paralelos`

Isso mostra que **nem a Grécia moderna usa hoje o termo como Euclides o usou**.

Fontes:

- [Ebooks escolares gregos](https://ebooks.edu.gr/ebooks/v/html/8547/2692/Geometria_A-Lykeiou_html-empl/index5.html)
- [Resumo escolar grego sobre τραπέζιο](https://blogs.sch.gr/anikolako/files/2020/03/%CF%84%CF%81%CE%B1%CF%80%CE%B5%CE%B6%CE%B9%CE%BF-%CE%B7-%CF%84%CE%B1%CE%BE%CE%B7.pdf)

### 5. Reconhecimento explícito da mudança de sentido na tradição grega atual

Uma nota histórica em material escolar grego atual afirma explicitamente:

> `Τραπέζιο ονομάζει όχι ό,τι σήμερα εννοούμε με τον όρο αυτό, δηλαδή τετράπλευρο με δύο μόνο πλευρές παράλληλες...`
> Tradução: `Ele chama de trapézio não aquilo que hoje entendemos por esse termo, isto é, quadrilátero com somente dois lados paralelos...`

E acrescenta que o termo com o sentido moderno aparece depois:

> `Ο όρος τραπέζιο, με τη σύγχρονη έννοια, απαντάται αργότερα στον Αρχιμήδη.`
> Tradução: `O termo trapézio, com o sentido moderno, aparece mais tarde em Arquimedes.`

Esse é o ponto mais forte para justificar a manutenção de `trapezium` / `trapezia` com nota, em vez de traduzir diretamente por `trapézio`.

Fonte:

- [Notas históricas de geometria escolar grega](https://mathlab.mysch.gr/timeline/docs/geometry_123-124.pdf)

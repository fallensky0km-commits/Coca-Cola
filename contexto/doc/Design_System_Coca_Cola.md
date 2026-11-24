# DESIGN SYSTEM --- COCA-COLA

**Documento de identidade visual e padrões de interface digital**

## 1. Identidade visual da marca

A Coca-Cola possui uma identidade visual reconhecida mundialmente. Seu
Design System deve preservar os elementos tradicionais da marca,
transmitindo alegria, tradição, energia e proximidade com o público.

-   **Cor principal:** Vermelho Coca-Cola.
-   **Cor secundária:** Branco.
-   **Cores complementares:** Preto e tons de cinza.
-   **Estilo:** Moderno, minimalista, comercial e marcante.
-   **Personalidade:** Alegre, tradicional, acessível e memorável.

## 2. Paleta de cores

A paleta utiliza o vermelho como destaque principal, com branco para
contraste e tons neutros para organização das informações.

  Cor                  Aplicação                         Código HEX
  -------------------- --------------------------------- ------------
  Vermelho Coca-Cola   Cor primária                      `#F40009`
  Branco               Cor secundária                    `#FFFFFF`
  Preto                Cor complementar                  `#000000`
  Cinza claro          Fundos e áreas secundárias        `#F5F5F5`
  Vermelho escuro      Estados de interação e destaque   `#B80000`

## 3. Tipografia e hierarquia dos textos

A tipografia deve combinar a personalidade tradicional da marca com a
facilidade de leitura das interfaces digitais.

  Elemento                 Tipografia         Tamanho
  ------------------------ ---------------- ---------
  Título principal (H1)    Helvetica Bold       40 px
  Título secundário (H2)   Helvetica Bold       32 px
  Subtítulo (H3)           Helvetica Bold       24 px
  Título pequeno (H4)      Helvetica Bold       20 px
  Texto normal             Arial                16 px
  Texto secundário         Arial                14 px
  Legendas                 Arial                12 px

**Tipografia especial:** A escrita Spencerian Script, característica do
logotipo Coca-Cola, deve ser preservada para a assinatura da marca e
elementos gráficos específicos, sem prejudicar a leitura dos textos.

## 4. Botões e estados

Os botões devem ser simples, fáceis de identificar e seguir a identidade
visual da empresa.

### Padrões dos botões

-   **Normal:** vermelho com texto branco.
-   **Hover:** vermelho mais escuro.
-   **Ativo:** vermelho escuro com leve redução visual.
-   **Desabilitado:** cinza com texto menos destacado.

### Exemplos de botões

-   **Botão principal:** fundo vermelho `#F40009`, texto branco e
    formato arredondado. Exemplo: "Saiba mais".
-   **Botão secundário:** fundo branco, borda vermelha e texto vermelho.
    Exemplo: "Conheça a marca".
-   **Botão desabilitado:** fundo cinza `#D9D9D9` e texto cinza
    `#777777`. Exemplo: "Indisponível".

## 5. Formulários

Os formulários devem ter aparência limpa, organizada e intuitiva.

**Padrões definidos:**

-   Campos com fundo branco.
-   Bordas cinza-claro.
-   Cantos levemente arredondados.
-   Texto interno em cinza.
-   Campo selecionado com borda vermelha.
-   Mensagens de erro em vermelho.
-   Botão de envio na cor principal da marca.

### Exemplo de formulário

-   **Nome completo:** campo com a indicação "Digite seu nome".
-   **E-mail:** campo com a indicação "exemplo@email.com".
-   **Botão de envio:** botão vermelho com texto branco "Enviar".

## 6. Cards e elementos reutilizáveis

Os cards são utilizados para apresentar produtos, campanhas, informações
e conteúdos promocionais.

  Tipo de card         Conteúdo
  -------------------- -------------------------------------------
  Card de produto      Imagem, nome e descrição do produto.
  Card de campanha     Imagem promocional, título e chamada.
  Card institucional   Informações sobre a marca e sua história.
  Card informativo     Conteúdos, novidades e notícias.

Os cards devem manter uma estrutura visual consistente, com imagens
proporcionais, textos objetivos e espaçamento adequado.

## 7. Bordas, sombras e espaçamentos

  Elemento                 Padrão
  ------------------------ --------------------
  Bordas                   1 px
  Cor das bordas           `#E5E5E5`
  Arredondamento pequeno   4 px
  Arredondamento médio     8 px
  Arredondamento grande    16 px
  Sombras                  Suaves e discretas
  Espaçamento pequeno      8 px
  Espaçamento médio        16 px
  Espaçamento grande       24 px
  Espaçamento extra        32 px

O objetivo é manter uma interface organizada, com boa separação entre os
elementos e sem excesso de informações visuais.

## 8. Regras de responsividade

O site deve funcionar corretamente em computadores, tablets e celulares.

  Dispositivo     Largura de referência Características
  ------------- ----------------------- ----------------------------------
  Celular                    Até 767 px Uma coluna e menu compacto
  Tablet                   768--1023 px Duas colunas quando necessário
  Desktop           A partir de 1024 px Layout amplo e múltiplas colunas

**Regras principais:**

-   Imagens devem se adaptar ao tamanho da tela.
-   Textos devem permanecer legíveis.
-   Botões devem ser acessíveis em dispositivos móveis.
-   Menus devem se adaptar ao espaço disponível.
-   Cards devem reorganizar suas colunas automaticamente.
-   Evitar rolagem horizontal.

## 9. Componentes reutilizáveis

Para manter a consistência visual em todas as páginas, os seguintes
componentes devem ser reutilizados:

  Componente        Função
  ----------------- --------------------------
  Header            Cabeçalho e navegação
  Footer            Rodapé institucional
  Button            Botões de ação
  Product Card      Apresentação de produtos
  Campaign Card     Divulgação de campanhas
  Input             Campos de formulário
  Navigation Menu   Menu de navegação
  Banner            Divulgação de conteúdos
  Modal             Janelas de informações
  Search Bar        Campo de pesquisa

## 10. Implementação em CSS

As variáveis abaixo permitem aplicar as definições do Design System
diretamente em um projeto web.

``` css
:root {
  /* Cores */
  --color-primary: #F40009;
  --color-secondary: #FFFFFF;
  --color-black: #000000;
  --color-gray: #F5F5F5;
  --color-red-dark: #B80000;

  /* Tipografia */
  --font-heading: Helvetica, Arial, sans-serif;
  --font-body: Arial, Helvetica, sans-serif;

  /* Tamanhos */
  --font-h1: 40px;
  --font-h2: 32px;
  --font-h3: 24px;
  --font-body-size: 16px;

  /* Bordas */
  --border-radius-sm: 4px;
  --border-radius-md: 8px;
  --border-radius-lg: 16px;

  /* Espaçamentos */
  --spacing-sm: 8px;
  --spacing-md: 16px;
  --spacing-lg: 24px;
  --spacing-xl: 32px;
}

.button-primary {
  background: var(--color-primary);
  color: var(--color-secondary);
  border: none;
  border-radius: 30px;
  padding: 12px 24px;
  font-weight: bold;
  cursor: pointer;
}

.button-primary:hover {
  background: var(--color-red-dark);
}
```

## 11. Conclusão

O Design System desenvolvido para a Coca-Cola busca preservar a
identidade visual tradicional da empresa e adaptá-la às necessidades das
plataformas digitais.

A utilização de uma paleta de cores consistente, tipografia adequada,
componentes reutilizáveis e regras de responsividade permite criar
páginas organizadas, modernas e funcionais.

Dessa forma, o sistema garante unidade visual, facilita futuras
implementações em CSS ou Tailwind CSS e mantém a personalidade da marca
em todos os elementos do site.

------------------------------------------------------------------------

**Observação:** Os códigos de cores apresentados são uma proposta de
referência para o exercício, não uma declaração de especificação oficial
da Coca-Cola. A implementação deve consultar os padrões oficiais da
marca para uso comercial.

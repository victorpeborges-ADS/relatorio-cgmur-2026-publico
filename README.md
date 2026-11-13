# Relatório CGMUR 2026 — edição pública sem token adicional

Painel de divulgação com estética e gráficos do relatório original, sem identificação
nominal de processos, acesso ao SEI ou endereços internos do SharePoint. Fonte interna
continua preservada no Mac mini.

## Editar e publicar
1. Abra o site no navegador e clique em **Editar relatório**.
2. Altere diretamente textos, indicadores, meses e composição documental; adicione e
   remova seções e métricas. Use **Salvar rascunho** e **Restaurar rascunho**.
3. Clique em **Publicar alterações para todos**. O site abre uma solicitação
   pré-preenchida no GitHub.
4. Acesse o GitHub como `victorpeborges-ADS` e clique em **Submit new issue**.
5. A automação `publicar-relatorio.yml` valida a autoria e conteúdo, atualiza
   `content.json`, fecha a solicitação e o GitHub Pages publica a alteração.

**Não é necessário criar token pessoal.** A publicação usa a sessão do GitHub para
identificar a conta e um `GITHUB_TOKEN` próprio do GitHub Actions, limitado ao
repositório. A edição só é aplicada para pedidos do proprietário da conta.
As solicitações de edição são públicas; não escreva dados internos ou sensíveis.

## PDF
- **Gerar PDF para impressão**: documento com estilo visual do painel.
- **Baixar PDF editável**: PDF AcroForm que permite alterar campos de texto no Acrobat
  ou em leitor compatível. A biblioteca usada é pdf-lib 1.17.1 (MIT).
- O PDF institucional completo (SEI + SharePoint, 12 páginas) é separado da
  versão pública e não foi publicado neste repositório.

## Dados e limitações
Contagens anuais SEI com recorte até 13/11/2026. Um processo pode ter mais de um
documento e um andamento fechado na CGMUR não significa processo concluído.
Metadados e referências do SharePoint foram verificados apenas internamente.
O relatório público é informativo, não substitui a homologação institucional.


## Revisão de design v3 (13/11/2026)
- Identidade visual editorial institucional independente, sem brasão ou identidade oficial indevida;
- Navegação por seções, hierarquia tipográfica e indicadores com melhor leitura;
- Responsividade testada em 320, 390, 768 e 1440 px, com gráficos roláveis sem deslocar a página;
- Modo claro/escuro persistente por navegador, com estilos próprios para impressão em PDF;
- Botões de edição ocultos no modo de leitura; foco visível e opção para reduzir movimento;
- Mantidos o conteúdo, o histórico, a publicação via GitHub autenticado e o PDF editável.

## Indicadores de impacto físico e financeiro (recorte de 13/11/2026)
O painel público apresenta dois gráficos para o recorte documentado de 2026 e
indicadores históricos separados, sem dados pessoais, identificadores internos ou
documentos restritos.

- **307.293 pontos previstos em 2026**: debêntures (213.407, seis projetos
  quantificados com portarias de 2026) e Pró-Cidades (93.886, propostas de
  Aparecida de Goiânia e Foz do Iguaçu encaminhadas à análise da CGMUR).
- **≈ 1.293.910 pontos na carteira histórica**: debêntures (≈ 1.194.461) e
  Pró-Cidades (99.449, três propostas com quantitativos identificados). Inclui
  pontos do recorte de 2026; não somar ao indicador anual.
- **R$ 770.539.723,36 de porte bruto de carteiras**: R$ 382.640.410,68
  em financiamento pretendido no Pró-Cidades e R$ 387.899.312,68 em valores
  declarados de sete projetos de debêntures com portarias de 2026.
- **R$ 319.338.009,15** em teto de debêntures enquadrado nos mesmos sete projetos
  e **R$ 2.461.457,00** no TED UFRGS: referências de outra natureza, não somáveis
  ao porte bruto.
- **Histórico de debêntures até setembro de 2026**: valor de projetos de cerca
  de R$ 2,24 bi, teto enquadrado de cerca de R$ 1,17 bi e emissões registradas
  de cerca de R$ 497,3 mi; categorias distintas e acumuladas, não somáveis.

O editor visual permite mudar os textos e números dos novos gráficos, adicionar e
excluir grupos; os totais de cada conjunto são derivados automaticamente.
O GitHub Actions valida e persiste os novos campos em `content.json`.
O PDF editável passa a conter campos relativos a impacto físico e financeiro.

**Critério de comunicação**: trata-se de metas físicas declaradas e de dimensão
financeira de propostas e projetos; não afirma modernização física concluída,
captação, execução ou desembolso atribuíveis à CGMUR. Os subconjuntos físicos e
monetários não necessariamente correspondem aos mesmos projetos, de modo que
não se deve inferir custo médio por ponto.

Fontes da curadoria (não incorporadas ao repositório público): painel de
debêntures de 22/10/2026, balanço ministerial de 22/09/2026, painel e briefing
Pró-Cidades, propostas técnicas nº 165/172/180/167 e TED 978205/2025.

## 13/11/2026 — reconciliação com painéis detalhados de Pró-Cidades e debêntures

A versão anterior de R$ 382,64 milhões no Pró-Cidades correspondia ao subtotal
de um briefing de maio, **não** à carteira completa de processos da CGMUR.

Os indicadores agregados publicados foram derivados dos painéis HTML fornecidos
pela equipe: Pró-Cidades (carteira CGMUR em 23/09/2026; BI geral em 29/09/2026)
e debêntures (fotografia de 12/08/2026), confrontados com a planilha institucional
de debêntures de 22/10/2026 anteriormente apurada.

**Pró-Cidades, Modalidade 2, carteira CGMUR 2025–2026:** 21 registros de processos,
17 protocolados em 2026, 11 UFs, cinco macrorregiões, referências a pareceres em
todos os registros e seis conclusões favoráveis documentalmente verificadas.
Investimento proposto de R$ 1.428.266.478,03, financiamento solicitado de
R$ 1.335.314.350,96 e contrapartidas de R$ 92.952.127,07.
Os 17 registros de protocolo 2026 concentram investimento de R$ 1.306.176.230,20
e financiamento de R$ 1.223.675.097,18. O painel já distingue números de
propostas, indicadores de mérito e registros do BI nacional: 210 propostas
das duas modalidades, 90 da modalidade 2 no programa, não atribuíveis
integralmente à CGMUR.

**Cuidado com a soma:** os dois registros de Foz do Iguaçu possuem processos
diferentes e valor de R$ 35 milhões cada. Uma exclusão hipotética diminui
o valor total em R$ 35 milhões, mas a identidade do objeto não foi comprovada.
Os 21 registros representam 20 territórios cadastrados (19 municípios e uma
iniciativa estadual). Não se apresentam efeitos causais, contratação, valores
pagos ou resultados físicos como comprovados.

**Debêntures:** o HTML datado de agosto retrata 29 projetos de dez UFs e três
macrorregiões; não substitui o balanço de setembro nem os sete projetos com
portarias publicadas até outubro de 2026. Estes últimos se distribuem por cinco
UFs: três portarias no Sul, três no Sudeste e uma no Nordeste. O painel de
agosto não registra números de pontos físicos comparáveis; o indicador
de 213.407 pontos no recorte 2026 continua fundamentado na planilha de outubro.

**Apresentação:** painel público mantém os indicadores agregados, inclui
barras territoriais e cartões de valores e não publica cópias de processos,
dados nominais, IDs processuais ou documentação interna. A geração de PDF
editável inclui os novos campos de Pró-Cidades e a distribuição de debêntures.

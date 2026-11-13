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

🏦 Conciliações Bancárias — Performance Empreendimentos
Painel de controle das conciliações bancárias da tesouraria da Performance Empreendimentos Imobiliários. Desenvolvido como arquivo HTML único — sem servidor, sem instalação, sem dependências externas em tempo de execução.
---
📋 Sobre o projeto
Ferramenta interna criada para substituir o controle manual de conciliações bancárias em planilhas. Com ela, o time de tesouraria consegue visualizar em tempo real o status das contas de todas as SPEs, filtrar por banco ou tipo de conta, editar datas de conciliação diretamente na tela e acompanhar o progresso do mês com KPIs automáticos.
Público-alvo: Diretor, Coordenador, Assistente e Auxiliar Financeiro.
---
✨ Funcionalidades
Painel de KPIs
Total de contas cadastradas
Quantidade de contas conciliadas no mês
Quantidade de contas sem movimento
Quantidade de contas bloqueadas
Barra de progresso com percentual de conciliação do mês, atualizada em tempo real conforme os filtros
Navegação por banco
Botões no cabeçalho com a logo de cada instituição parceira:
Banco	Banco	Banco
Itaú	Bradesco	Santander
BBM	Genial	Safra
ASA	Sofisa	ABC Brasil
Guanabara	+ Outros	
Navegação por tipo de conta
Segunda barra de filtro com os tipos: Corrente · Investimento · Bloqueada · Obra · Encerrada
Filtros combinados
Todos os filtros funcionam em conjunto:
Tipo de SPE (Holding, Incorporação, Construída, Patrimônio, LO, Obra)
Parceiro (Interna, BRB, Brookfield, Genial, ABC Brasil, Prisma…)
Status de conciliação (sim / sem movimento / bloqueada)
Busca livre por texto (SPE, banco, conta, número)
Tabela de contas
155 registros carregados, cobrindo 67 SPEs ativas
Ordenação clicável em qualquer coluna
Badges coloridos por status de conciliação
Logos dos bancos na coluna "Banco"
Data de conciliação editável
Clique direto na célula da data para editar
Enter ou Tab confirma e salva
Escape cancela e restaura o último valor salvo
Validação automática do formato `DD/MM/AAAA`
Toast de confirmação (verde) ou alerta (amarelo) no canto da tela
Cadastro de nova conta
Botão + Nova Conta no cabeçalho abre modal com formulário completo:
Nº SPE, Tipo, Nome da SPE, Parceiro
Banco, Código COMPE, Agência, Conta
Tipo de conta, Status de conciliação, Data
O registro entra na tabela imediatamente
Rodapé
Exibe o caminho de rede para acesso aos extratos:
```
Z:\Performance\Financeiro\Tesouraria\Saldos contas\2026
```
---
🗂 Estrutura dos dados
Cada registro na tabela representa uma conta bancária e contém os campos:
Campo	Descrição
Nº	Número identificador da SPE
Tipo SPE	Classificação jurídica/operacional
SPE / Empresa	Nome do empreendimento
Parceiro	Parceiro financeiro do empreendimento
Banco	Instituição bancária
Agência	Código da agência
Conta Bancária	Número da conta (corrente, investimento etc.)
Tipo de Conta	Corrente / Investimento / Bloqueada / Obra
Conciliação	sim / s/ mov / bloqueada
Data Conciliada	Data da última conciliação (editável)
---
🚀 Como usar
Faça o download do arquivo `conciliacoes_bancarias.html`
Abra no navegador (Google Chrome, Edge ou Firefox recomendados)
Nenhuma instalação necessária — o arquivo funciona completamente offline
> ℹ️ Todas as logos dos bancos estão embutidas no arquivo como imagens em base64. Não é necessária conexão com a internet para exibir nenhum elemento da página.
---
🔍 Atalhos e comportamentos
Ação	Como fazer
Filtrar por banco	Clicar no botão do banco no cabeçalho
Filtrar por tipo de conta	Clicar na barra secundária abaixo do cabeçalho
Ordenar a tabela	Clicar no título de qualquer coluna
Editar data de conciliação	Clicar diretamente na célula da data
Confirmar edição	Enter ou clicar fora do campo
Cancelar edição	Escape
Adicionar nova conta	Botão "+ Nova Conta" no canto superior direito
Busca livre	Campo de texto na barra de filtros
---
🏗 Detalhes técnicos
Tecnologia: HTML5 + CSS3 + JavaScript puro (sem frameworks)
Arquivo único: tudo embutido — estilos, scripts e logos em base64
Sem back-end: os dados ficam em memória durante a sessão; ao fechar a aba, o estado é resetado
Logos reais: Itaú, Bradesco, Santander, Safra, Sofisa e ABC Brasil carregadas via SVG do repositório público Tgentil/Bancos-em-SVG
Responsivo: adaptado para telas menores (tablet/mobile)
---
📁 Arquivos do repositório
```
📦 conciliacoes-bancarias
├── conciliacoes_bancarias.html   # Página principal (arquivo único)
└── README.md                     # Este documento
```
---
🔄 Próximas melhorias sugeridas
[ ] Persistência local com `localStorage` para manter alterações entre sessões
[ ] Exportação dos dados filtrados para Excel/CSV
[ ] Campo de status de conciliação também editável na tabela
[ ] Integração com arquivo de saldos (`Saldos.xlsx`) via upload
[ ] Histórico de alterações por conta
---
👤 Responsável
Lenin — Financeiro · Performance Empreendimentos Imobiliários  
Tesouraria · Rio de Janeiro, RJ
---
> *Este projeto foi desenvolvido para uso interno. Os dados exibidos são baseados no cadastro de contas bancárias da empresa referentes ao exercício de 2026.*

## Mcp NFe Hub

## Descrição 
O NFe Hub conecta assistentes de IA (Claude, ChatGPT etc.) diretamente à consulta oficial de Notas Fiscais Eletronicas na SEFAZ. A partir da chave de acesso de 44 digitos, retorna em segundos:

- Situação da nota (autorizada, cancelada, denegada)
- Número do protocolo de autorização
- Data e hora da autorização/cancelamento
- Eventos vinculados (cancelamento, carta de correção), quando solicitado

Feito para escritórios de contabilidade e departamentos fiscais que hoje conferem esse status manualmente no portal da SEFAZ ou trocando mensagens de WhatsApp com o cliente ("essa nota autorizou?"). Com o NFe Hub, a pergunta é respondida no mesmo chat onde o time já trabalha, sem precisar abrir outro sistema.

O certificado digital e as credenciais de acesso não passam pelo modelo de IA — ficam apenas na integração com o emissor.

## Categoria/tags
fiscal, nfe, sefaz, contabilidade, brasil, tax, invoice, accounting, finance

## Ferramenta exposta
`consultar_nfe`
- `chave_nfe` (obrigatório): chave de acesso de 44 dígitos da NFe
- `cnpj` (opcional): CNPJ para filtrar/validar a consulta
- `n_recibo` (opcional): número de recibo, quando aplicável
- `retorna_eventos` (opcional): se true, inclui eventos vinculados (cancelamento, CC-e)

## Link do servidor remoto (para o campo "install"/"connect")
https://mcp-nfe-hub.onrender.com/mcp
(tipo de transporte: streamable-http)

## Repositório
https://github.com/cristianosantana/mcp-nfe-hub-v1

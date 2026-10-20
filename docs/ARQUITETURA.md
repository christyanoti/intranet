# Arquitetura e limites do MVP

## Domínios previstos

Diretoria/BI; Recepção e agenda; Clínico/assistencial; Financeiro e faturamento; Recursos Humanos; Estoque e compras; Comunicação; Processos e solicitações; Administração, permissões e auditoria.

## Estado implementado

Interface React/Vite com navegação por domínio, indicadores demonstrativos, lista e formulário de solicitações em memória, filtro e status. Sem servidor, banco de dados, autenticação ou integração com o Lovable. Nenhum dado real deve ser inserido.

## Arquitetura proposta para fase operacional

Frontend React/TypeScript; API com validação no servidor; PostgreSQL; identidade e RBAC por usuário/unidade/setor, auditoria, backups criptografados, notificações e adaptadores de integração. A definição final depende do levantamento de requisitos da FONOCLIN.

## Requisitos antes de uso clínico

LGPD e políticas de dados sensíveis: segregação de perfis, consentimentos/bases legais adequadas, criptografia, trilhas de auditoria, minimização, controle de acesso no servidor, retenção, tratamento de incidentes, restauração de backup e testes de segurança. Não incluir dados reais no protótipo.

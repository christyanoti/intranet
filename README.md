# INTRANET FONOCLIN

Plataforma integrada de gestão dos setores da FONOCLIN.

## Situação

**MVP visual e demonstrativo em `develop`. Não publicado e não autorizado para dados reais.** Interface React/Vite com navegação por setores, painel de indicadores, pesquisa de solicitações, cadastro demonstrativo e alteração de status. Toda a operação ocorre somente na memória do navegador; não existe persistência, autenticação, backend ou integrações clínicas.

## Executar localmente

Requer Node.js 20+.

```bash
npm install
npm run dev
```

Para gerar o bundle: `npm run build`.

## Organização

- `src/main.jsx`: interface e comportamento do protótipo.
- `src/style.css`: identidade visual responsiva.
- `docs/ARQUITETURA.md`: domínios, arquitetura alvo e proteção de dados.
- `docs/FLUXO-DE-PUBLICACAO.md`: regras de governança GitHub/Lovable.

## Branches e publicação

- `develop`: desenvolvimento e testes, sempre.
- `main`: produção; mudanças somente após o comando **Pode publicar!**.
- Antes de publicação: backup com timestamp, revisão, réplica de `develop` para `main`, deploy e relatório comercial em PDF.
- Integração com Lovable somente pelo GitHub; **não enviar prompts ao Lovable**.

## Próximas fases

1. Levantamento dos sistemas e processos reais da FONOCLIN.
2. Autenticação, autorização por perfil, unidade e setor, e auditoria.
3. API, banco de dados, migrações, workflows e notificações.
4. Módulos reais de recepção, agenda, financeiro, RH, compras e comunicação.
5. Segurança e conformidade LGPD antes de qualquer uso de informações de pacientes.

**Não inserir dados pessoais, clínicos ou credenciais nesta versão.**

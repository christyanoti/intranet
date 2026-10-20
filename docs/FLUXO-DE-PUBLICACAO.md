# Governança GitHub / Lovable

- **develop**: única branch de desenvolvimento e teste.
- **main**: branch de produção, sem evolução direta de funcionalidades.
- Lovable conectado via GitHub; **não enviar prompts ao Lovable**.
- Nunca publicar antes da autorização explícita **Pode publicar!**.
- Na autorização: validar testes, criar backup com padrão `YYYYMMDD-HHMMSS`, replicar `develop` em `main`, publicar `main`, verificar saúde da aplicação e produzir relatório comercial de atualização em PDF com linguagem clara e emojis.
- Sem infraestrutura de deploy configurada, a publicação deve ser informada como pendente, nunca presumida.

# Login e gestão de acesso — plano de implementação

## Entrega atual

Tela visual de acesso institucional com e-mail, senha, alternância de visibilidade, mensagem explícita de autenticação indisponível e acesso a demonstração. Não existe serviço de login; não há sessão real, persistência de senha ou validação de usuário. O acesso demonstrativo é **público e não possui qualquer proteção**, sendo adequado apenas a dados fictícios.

## Próxima etapa obrigatória

1. Selecionar provedor de identidade e backend seguro.
2. Criar cadastro de usuários com status ativo/inativo, convite e recuperação de acesso.
3. Implementar validação de credenciais exclusivamente no servidor e tokens/sessões protegidos.
4. Definir papéis: administrador, diretoria, gestor setorial, colaborador, com regras específicas por unidade/setor.
5. Controlar cada API no servidor e gerar trilhas de auditoria para eventos relevantes.
6. Limitar tentativas, implementar MFA para acessos privilegiados, expiração e encerramento de sessões.
7. Testar autenticação, autorização, isolamento de dados e segurança antes de usar dados empresariais.

## Integração

SGG: integração prevista, **fora do escopo deste ciclo**, sem implementação de conector ou sincronização.

## Segurança e publicação

Não usar dados reais nesta prévia. Não guardar segredos em arquivos versionados. Trabalhar sempre em `develop`; produção `main` somente mediante comando **Pode publicar!** com backup e relatório PDF.

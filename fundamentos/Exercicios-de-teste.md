PLANO DE TESTE PARA CADASTRO DE USUARIOS

Introdução:
    Objetivo:Garantir que a funcinalidade de cadastro de usuários esteja funcionando corretamente e atenda aos requisitos especificados.
    Escopo:Testar a funcionalidade de casdastro na página de registros de usuários, incluindo validações de campos, integração com o banco de dados e exibição de mensagens de erro/sucesso
Escopo do teste:
    O que será testado:
        Preenchimento e validação de campos obrigatórios(Email, senha, nome, telefone,etc).
        Regras de validação, como formatos de e-mail e força de senha.
        Comportamento ao tentar cadastrar um usuário com e-mailjá existente.
        Integração com o banco de dados (registro com os dados corretos estão sendo salvos).
        Mensagem de feedback (erro/sucesso) exibidas ao usuário.
    O que está fora do escopo:
        Testar funcionalidades de login ou recuperação de senha(serão testadas separadamente).
Estratégia de teste:
    Tipos de teste aplicados:
        Teste funcional: Verificar se a funcionalidade atende aos requisitos.
        Teste de validação de dados: Garantir que os dados inseridos seguem os padrões esperados.
        Teste de interface (UI): Validar a experiencia do usuário na página de cadastro.
    Forma de execução:
        Os testes serão realizados manualmente e, posteriormente, alguns casos serão automatizados com Selenium e Cypress.
Recursos Necessários:
    Ambiente de teste:
        Sistema Operacional: Windows 10 / ubuntu 20.04.
        Navegadores: Google chrome, mozilla firefox.
        Banco de dados: Mysql (ambiente de homologação).
    Ferramentas:
        Postman (Para testar a api de cadastro).
        Selenium (Para testes automatizados).
        Planilha excel ou testRail (ambiente de homologação).
    Equipe:
        1 analista de Qa.
        1 desenvolvedor para suporte a bugs.
Cronograma:
    Inicio de teste: 29/01/2025.
    Fim previsto: 31/01/2025.
    Datas principais:
        Configuração do ambiente: 29/01/2025.
        Execução dos teste manuais:29/01/2025 tarde e 30/01/2025.
        Relatório final: 31/01/2025.
Casos de teste:
Aqui estão exemplos de casos de teste para o cadastro de usuários:
    Caso de teste 1: Cadastro com dados válidos:
        Objetivos: Garantir que o cadastro é concluido com sucesso e com dados válidos:
    Pré-condições:
        O sistema deve estar disponivel.
        A página de cadastro de estar carregada.
    Passos:
        1.Acessar a página de cadastro.
        2.Preemcher os campos com os dados válidos:
            Nome: João Henrique
            E-mail: joao@teste.com.br
            senha: 123456
            Confirmar senha: 123456
        3.Clicar no botão de cadastrar
    Resultado esperado:
        O sistema exibe a mensagem: "Cadastro realizado com sucesso".
        Os dados são armazenados no banco de dados.
    Caso de teste 2: Cadastro com email inválido:
        Objetivo: Validar a regra de formato para o campo de email.
        pré condições:
            O sistema deve estar disponivel.
        Passos:
            1.Acessar a página de cadastro.
            2.Preencher os campos:
                Nome: João Henrique
                E-mail: joao@teste. (Formato inválido)
                senha: 123456
                Confirmar senha: 123456
            3.Clicar no botão de "cadastrar"
        Resultado esperado:
            O sistema deve exibir uma mensagem de erro: "Email inválido, insira um email no formato correto"
    Caso de teste 3: Cadastro com email já existente
        Objetivo: garantir que o sistema impede o cadastro de emails duplicados.
        Pré-condições:
            O email joao@teste.com.br já cadastrado no banco de dados
        Passos:
            1.acessar a página de cadastro.
            2.Preencher os campos:
                Nome: João Henrique
                E-mail: joao@teste.com.br
                senha: 123456
                Confirmar senha: 123456
            3.Clicar no botão de cadastrar
        Resultado esperado;
            O sistema exibe e mensagem de erro: "Email já cadastrado".
Riscos:
    Possiveis riscos:
        Ambiente de teste não estar configurado corretamente.
        Dados invalidos no banco de dados afetando os testes.
        Conexão instavel com a APi.
    Plano de mitigação:
        Configurar o ambiente com antecedencia.
        utilizar um banco de dados de homologação separado.
Critérios de aceitação:
    Critérios de inicio:
        Ambiente de teste configuirado.
        Requisitos de cadastro definidos e estáveis.
    Critérios de término:
        Todos os casos de teste executados com sucesso.
        Defeitos criticos corrigidos e revalidados.
Relatório Final:
    Após a conclusão dos testes, será gerado um relatório contendo:
    Casos de teste executados.
    Defeitos encontados(Com gravidade e status).
    Conclusões e sugestões de melhorias

    

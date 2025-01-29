Categorias de testes:

Os tipos de teste podem ser dividos em várias categorias:

Funcionais: (Testam o que o sistema faz)
Não funcionais: (Testam como o sistema se comporta)
Estruturais: (analisam o código fonte)
De manutenção: (Avaliam impactos de mudanças)

1. Testes funcionais:
Esses testes verificam a funcionalidade do sistema, se atende aos requisitos esperados. Eles são baseados nas informações do sistema e não levam em conta o código fonte

    Teste de Unidade:
    Testa módulos individuias do código, como funções ou classes.
    É feito por desenvolvedores e usa mocking para simular dependencias
    Normalmente automatizado

    Exemplo: Testar uma função de cálculo de juros para garantir que retorna o valor correto

    Ferramentas:
        Junit(Java)
        PhpUnit(PHP)
        Jest(JavaScript)
    
    Teste de integração:
    Verifica se os módulos so sistema funcionam corretamente juntos.
    Avalia a comunicação entre o banco de dados, back end, api, microserviços, etc.

    Exemplo: Um teste que verifica se o backend retorna corretamente os dados esperados após uma requisição do frontend.
    
    Ferramentas:
    Postman (para apis)
    Cypres (integração front end-brackend)
    RestAssured (Testes de api em java)
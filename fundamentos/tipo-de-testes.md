Categorias de testes:

Os tipos de teste podem ser dividos em várias categorias:

Funcionais: (Testam o que o sistema faz)
Não funcionais: (Testam como o sistema se comporta)
Estruturais: (analisam o código fonte)
De manutenção: (Avaliam impactos de mudanças)

Quanto ao nível de teste (em que parte do sistema o teste é aplicado):

Testes Unitários
Testes de Integração
Testes de Sistema
Testes de Aceitação
Quanto ao objetivo do teste (o que se pretende verificar):

Testes Funcionais
Testes Não Funcionais (Desempenho, Usabilidade, Segurança, etc.)
Testes de Regressão
Testes Exploratórios
Testes de Automação
Quanto à execução (como o teste é realizado):

Testes Manuais
Testes Automatizados

1. Testes funcionais:
Esses testes verificam a funcionalidade do sistema, se atende aos requisitos esperados. Eles são baseados nas informações do sistema e não levam em conta o código fonte

    Teste de Unidade:
    Testa módulos individuias do código, como funções ou classes.
    É feito por desenvolvedores e usa mocking para simular dependencias
    Normalmente automatizado

    Exemplo: Testar uma função de cálculo de juros para garantir que retorna o valor correto

    Outro exemplo, se temos uma funnção que soma(a,b), o teste unitário verifica se soma(2,3) é igual a 5.

    Ferramentas:
        Junit(Java)
        PhpUnit(PHP)
        Jest(JavaScript)
        PyTest(python)

    Pontos positivos:
    Tem facilidade em encontra bug pequenos
    Custo de execução rapida e barata
    Reduz erros em estágios avançados do desenvolvimento

    Pontos negativos:
    Não testa a interação entres os componentes
    Pode dar falso positivo dependendo se as dependencias não forem bem implantadas
    
    Teste de integração:
    Verifica se os módulos so sistema funcionam corretamente juntos.
    Avalia a comunicação entre o banco de dados, back end, api, microserviços, etc.

    Exemplo: Um teste que verifica se o backend retorna corretamente os dados esperados após uma requisição do frontend.
    
    Ferramentas:
    Postman (para apis)
    Cypres (integração front end-brackend)
    RestAssured (Testes de api em java)

    Testes de nivel 


# 📚 Exercício de Fixação 09 – Explorando a API ViaCEP e Evoluindo a Classe Endereco - aula 27/08/2026 

[Edit in StackBlitz next generation editor ⚡️](https://stackblitz.com/~/github.com/mjsoweb/aula27-08-2026)


**Questões teóricas**

1.Qual a vantagem de consultar diretamente a API antes de modificar a classe?
*Garante que você está usando os dados mais recentes e evita salvar informações desatualizadas.*

2.Por que os novos dados devem ser armazenados em atributos privados?
*Protege os dados contra alterações indesejadas de fora da classe (encapsulamento).*

3.Qual a finalidade dos métodos get adicionados à classe?
*Permitem ler os dados de forma segura sem dar acesso direto para modificá-los.*

4.Por que não devemos acessar diretamente os atributos retornados pela API fora de setCep()?
*Porque `setCep()` é o único responsável por buscar, validar e organizar os dados corretamente.*

5.Qual a diferença entre o nome de uma propriedade da API e o nome de um atributo da classe?
*A API usa o padrão dela (ex: `logradouro`), e a classe pode usar o padrão do seu projeto (ex: `rua`).*

6.Por que a classe não precisa utilizar obrigatoriamente os mesmos nomes adotados pelo ViaCEP?
*O código fica mais independente; se a API mudar, você só ajusta o mapeamento interno.*

7.O que aconteceria se a API adicionasse novos campos no futuro?
*Nada quebra, já que a classe só lê o que ela realmente precisa e ignora o resto.*

8.Por que o tratamento com try/catch deve continuar funcionando mesmo após a inclusão de novos atributos?
*Porque o tratamento de erros protege a busca na API, que é independente dos atributos que você escolheu criar depois.*


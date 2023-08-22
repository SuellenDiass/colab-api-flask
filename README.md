<p> <h1 align="center">Criando uma API com Flask no Ambiente COLAB</h1></p>

<p align="center">
    <img width="700" src="https://github.com/SuellenDiass/SuellenDiass/assets/102911341/e581e2d7-9ec9-4ed6-884a-ad7f7408f10d">
</p>
<p> <h4 align="center">Instalando pacotes</h4></p>



<p align="center">
    <img width="700" src="https://github.com/SuellenDiass/SuellenDiass/assets/102911341/07d0654c-e0bd-48a0-aecf-ada086322bf0" alt="Imagem">
</p>
<p> <h4 align="center">api</h4></p>

Estrutura   do código :

1. **Importações:** Começamos importando a classe `Flask` do módulo `flask` e a função `jsonify`. A classe `Flask` nos permite criar um aplicativo da web usando o Flask.

2. **Criação do Aplicativo:** Usamos `app = Flask(__name__)` para criar uma instância do aplicativo Flask. O `__name__` é uma variável especial que representa o nome do módulo atual.

3. **Dados da Planilha:** Definimos os dados da planilha em formato JSON usando um formato de lista de dicionários. Cada dicionário representa uma linha da planilha.

4. **Rota e Função:** Usamos o decorador `@app.route('/index', methods=['GET'])` para criar uma rota para nosso endpoint. O `/index` no decorator indica que nossa rota é acessada através do URL `/index`.

5. **Função da Rota:** Definimos uma função chamada `get_data()` que é executada quando alguém acessa a rota. Essa função retorna os dados da planilha no formato JSON usando a função `jsonify`.

6. **Execução do Aplicativo:** O trecho `if __name__ == '__main__':` garante que o servidor só seja iniciado se o script for executado diretamente (não quando importado como um módulo). Usamos `app.run(debug=True)` para iniciar o servidor Flask em modo de depuração.

Esse foi um exemplo simples para mostrar como criar uma API básica usando o Flask. A estrutura pode se tornar mais complexa à medida que for adicionando mais rotas, lógica de negócios e interações com bancos de dados. No entanto, esse é um ponto de partida para entender como estruturar um aplicativo Flask para criar APIs.



#### Curso Formação Python Developer da Dio.me administrado pelo mentor Diego Renan/Education Tech Lead, DIO

[DIO](https://www.dio.me/).


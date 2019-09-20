# RestPOST-API
https://api-postful.herokuapp.com/


**API**: el acrónimo API que proviene de la interfaz de programación de aplicaciones, es un conjunto de rutinas y estándares establecidos y documentados por una aplicación A, para que otras aplicaciones puedan usar las funciones. de esta aplicación A, sin necesidad de conocer los detalles de la implementación del software.

**REST**: El modelo REST ( RE presentational S tate T ransfer) representa nada más que una "nueva" posibilidad para la creación de servicios web, cuyas principales diferencias con el modelo tradicional (SOAP) son el uso semántico de los métodos HTTP (GET). POST, PUT y DELETE), la ligereza de los paquetes de datos transmitidos en la red y la simplicidad, haciendo innecesaria la creación de capas intermedias


<p align="center">
<img src="https://becode.com.br/wp-content/uploads/2017/02/API-768x520.png" width="50%" height="50%" align="center"/>
</p>

A API criada disponibiliza todos os continentes e paises existentes, retornando os dados de busca no formato **JSON**. Confira abaixo as URLs de acesso a API:

## /paises?nome=[param]
Lista um pais especifico pelo nome, ignorando caixa alta/baixa e acentuações.

## /continentes
Lista todos os continentes existentes.

## /continentes/[id]
Lista um continente em especifico, de acordo com o parâmetro ID passado no corpo da URL.

## /continentes/[id]/paises
Lista todos os paises de um continente especifico.

## /continentes/[id]/paises/[id]
Lista um pais especifico de um continente de acordo com os parâmetros passados no corpo da URL.

## Exemplo:

**/continentes/1/paises/1**

```
{
    "id":1,
    "nome":"África do Sul",
    "capital":"Pretória",
    "area":1221040,
    "populacao":54956920,
    "governo":"República presidencialista",
    "lema":"Diversos povos se unem",
    "hino":"National anthem of South Africa",
    "linguas":"Africâner, Inglês, Ndebele, SeSotho do norte, SeSotho do sul, Suázi, Venda, Xhosa, XiTsonga, Zulu, seTswana",
    "moeda":" Rand sul-africano (ZAR)",
    "vizinhos":"Botsuana, Lesoto, Moçambique, Namíbia, Suazilândia, Zimbábue",
    "f_maritimas":"Oceano Atlântico, Oceano Índico"
}

```

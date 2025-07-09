# Demos-Sesion-8
Repositorio para los demos de la sesión 8 del Bootcamp de GitHub Foundations de Código Facilito

<br>  

Para obtener el secret `DISCUSSION_CATEGORY_ID` se realiza mediante la api de GraphQL en Github en la siguiente dirección: https://docs.github.com/es/graphql/overview/explorer con el siguiente código:
```graphql
{
  repository(owner: "cmix-ice", name: "demo-sesion-8") {
    id
    name
    discussionCategories(first: 10) {
      nodes {
        id
        name
      }
    }
  }
}
```

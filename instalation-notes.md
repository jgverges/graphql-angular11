## apollo
``` ng add apollo-angular```

url: https://rickandmortyapi.com/graphq

### creacion de módulos y components
Ejemplo de creación  con la ruta incorporada
```ng g m components/pages/home/home -m=app --route home --flat ``` 

## Creación de módulos y componentes:
   ~~~
ng g m components/pages/home/home -m=app --route home --flat

ng g shared/components/header 

ng c shared/components/header 

ng g m components/pages/episodes/episodes -m=app --route episodes --flat

ng g m components/pages/notFound/notFound -m=app --route not

ng g m components/pages/characters/characters-card

ng g c components/pages/characters/characters-card

ng g m components/pages/characters/characters-list -m=app --route character-list

ng g m components/pages/characters/characters-details -m=app --route character-details

ng g m components/pages/about/about -m=app --route about
~~~           

## alias para las rutas
en tsconfig.json añadimos en compilerOptions, debajo de "baseUrl":
~~~
"paths" :{
   "@app/*":["src/app/*"],
   "@shared/*":["src/app/shared/*"],
   "@characters/*":["src/app/components/pages/characters/*"],
   "@pages/*":["src/app/components/pages/*"],
   "@enviroment/*":["src/enviroments/*"],
}
~~~

# Funções para o bot do @grupos_ti

### Navegação por categorias:

- Permite que o usuário veja todos os grupos e canais, por meio de botões que aparecerão na tela

- Inicialmente, os botões seriam "Grupos", "Canais" e "Todos", que indicariam ao bot para mostrar, respectivamente, "somente grupos", "somente canais", ou "ambas as opções" (opção padrão).

- Nessa mesma mensagem inicial, também apareceriam os botões "Todos" ou "Selecionar Idiomas". Se o usuário optasse por "todos" (opção padrão), apareceriam grupos/canais de todos os idiomas. Se optasse por "Selecionar Idiomas", poderia escolher os idiomas _(pt, en, es, de, it)_.

- Então, apareceriam categorias, como "Programação" ou "Linux", em forma de botões. Ao selecionar alguma delas, ou o bot mostraria mais opções de categorias (caso ele selecionasse "Linux", por exemplo, em que apareceria "Ubuntu", "Arch", etc..), ou mostraria apenas grupos de uma sub-categoria (caso ele selecionasse "Ubuntu", por exemplo, já que não haveria mais sub-categorias para mostrar).

Essa função de navegação por categorias só ocorreria no privado do Bot. Ela não poderia ser usada em grupos, por exemplo.

Sempre seriam mostradas as opções "Voltar" e "Mostrar grupos/canais"

### Busca inline de grupos/canais:

- Seria um recurso [inline](https://core.telegram.org/bots/inline)

- Possibilitaria buscar grupos e canais via inline.
Usaria a seguinte sintaxe:
> @grupos_tiBot [#grupo|#canal] [#pt, #br, #en, #es, #it, #de] _sua busca aqui_

Caso algum campo opcional fosse otimido, seria usada a opção padrão (buscar tudo)

**Exemplos na prática:**

- Para buscar grupos e canais de Zabbix:
> @grupos_tiBot zabbix

- Para buscar grupos de Python regionais:
> @grupos_tiBot #grupo #br python

- Para buscar canais de Linux em inglês e espanhol:
> @grupos_tiBot #canal #en #pt linux

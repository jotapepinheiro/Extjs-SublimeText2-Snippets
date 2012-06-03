## Sumário

Snippets do Extjs para o [Sublime Text 2](http://www.sublimetext.com/)

## Modo de uso

Abra o menu Preferences -> Browse Packages e adicione a pasta 'Extjs-SublimeText2-Snippets'.

```js
<snippet>
<content>
<![CDATA[this.store${1:$SELECTION} = new Ext.data.JsonStore({
	remoteSort: true,
	root: 'rows',
	totalProperty: '${2:total}',
	idProperty: ['${3:cod}'],
	waitMsg: 'Carregando ${1/(.*)/\u$1/}...',
	baseParams: {
		 action: 'listar${1/(.*)/\u$1/}'
		,start: 0
		,limit: PAGINACAO
	}
	,url: 'include/${1/(.*)/\l$1/}Action.php'
	,fields: [
	     {name: 'cod', type : 'int'}
		,{name: '${4:campo 1}',type: 'string'}
		,{name: '${5:campo 2}',type: 'date',dateFormat: 'Y-m-d'}
	]
});$0]]>
</content>
<tabTrigger>sto</tabTrigger>
<scope>source.js</scope>
<description>Ext.data.JsonStore</description>
</snippet>
```

# Informações

Arquivos: https://github.com/JotapePinheiro/Extjs-SublimeText2-Snippets

Autor: [João Paulo Pinheiro](https://github.com/JotapePinheiro/)
# Bubbler
Bubbler é um menu de bolhas em JavaScript / CSS inspirado no material design. Nenhuma biblioteca necessária.

![demo](http://i.imgur.com/Bg232lt.gif)

# tuto
Para criar um menu, você deve criar uma nova instância do `Bubbler` e passar suas opções.
```JavaScript
var options =
[
	{
		icon:'1',
		label: 'Run alert function',
		callback: function() {
			alert('dasd');
		}
	},
	{
		icon:'<i class="fa fa-id-card" aria-hidden="true"></i>',
		label: 'Test Element 2'
	},
	{
		icon:'3',
		label: 'Test Element 3',
		display: {
			color: 'blue',
			background: 'red'
		}
	}
];

var menu = new Bubbler(options);
```

# Options
`options` deve ser uma matriz de objetos. Cada objeto de opção pode conter vários parâmetros.

# Parameters
`icon` -> Requeridos. O ícone que é exibido para a opção. Suporta qualquer ícone longo de caractere único, incluindo ícones de fonte (pode ser definido como HTML para exibir um ícone de fonte)

`label` ->  Requeridos. O texto que é exibido ao passar o mouse sobre uma opção

`callback` -> Opcional. Esta função é chamada quando o elemento é clicado.

`display` -> Opcional. Defina regras CSS personalizadas.

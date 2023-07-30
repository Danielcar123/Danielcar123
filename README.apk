<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>El latido de mi carazón</title>
	<style>
	/* Estilos para el cuerpo del documento */
	body {
		height: 100vh; /* Altura del cuerpo igual al 100% del viewport */
		width: 100%; /* Ancho del cuerpo igual al 100% del viewport */
		display: grid; /* Se utiliza el sistema de grillas */
		place-items: center; /* Centra los elementos dentro del cuerpo */
		background-color: rgb(9, 4, 26); /* Color de fondo púrpura oscuro */
	}

	/* Estilos para el corazón */
	.heart {
		height: 200px; /* Altura del corazón */
		width: 200px; /* Ancho del corazón */
		background-color: red; /* Color de fondo rojo */
		position: relative; /* Posicionamiento relativo para alinear los pseudo-elementos */
		transform: rotate(45deg); /* Rotación de 45 grados para el corazón */
		animation: latir .8s ease-in-out alternate infinite; /* Animación de latido */
	}

	/* Pseudo-elementos ::before y ::after para crear la forma de corazón */
	.heart::before, .heart::after {
		content: ""; /* Contenido vacío para los pseudo-elementos */
		position: absolute; /* Posicionamiento absoluto con respecto al corazón */
		display: block; /* Se muestran como bloques */
		height: 100%; /* Altura igual al 100% del corazón */
		width: 100%; /* Ancho igual al 100% del corazón */
		border-radius: 50%; /* Borde redondeado para crear la forma de corazón */
		background-color: red; /* Color de fondo rojo para los pseudo-elementos */
	}

	/* Estilos para el pseudo-elemento ::before */
	.heart::before {
		transform: translateY(-100px); /* Desplazamiento hacia arriba para formar la parte superior del corazón */
	}

	/* Estilos para el pseudo-elemento ::after */
	.heart::after {
		transform: translateX(-100px); /* Desplazamiento hacia la izquierda para formar la parte inferior derecha del corazón */
	}

	/* Animación "latir" para el corazón */
	@keyframes latir {
		100% {
			transform: scale(1.3) rotate(45deg); /* Escala y rotación para simular el latido */
		}
	}

	/* Estilos para el contenido del corazón (el texto "Te amo nombre") */
	.heart-content {
		position: absolute; /* Posicionamiento absoluto dentro del corazón */
		top: 40%; /* Alineación vertical del contenido en el centro */
		left: 40%; /* Alineación horizontal del contenido en el centro */
		transform: translate(-50%, -50%) rotate(-45deg); /* Ajuste para centrar y no voltear el texto, rotación opuesta a la del corazón */
		color: white; /* Color del texto en blanco */
		font-size: 24px; /* Tamaño de la letra del texto */
		font-weight: bold; /* Fuente en negrita para el texto */
		text-align: center; /* Alineación del texto al centro */
		z-index: 1; /* Capa z para que el texto aparezca sobre el corazón */
	}
	/* Media query para ajustar estilos en pantallas más pequeñas */
		@media (max-width: 768px) {
			.heart {
				height: 150px; /* Ajustar el tamaño del corazón para pantallas pequeñas */
				width: 150px;
			}

			.heart-content {
				font-size: 18px; /* Ajustar el tamaño de la letra para pantallas pequeñas */
			}
		}
</style>

</head>
<body>
	<div class="heart">
		<div class="heart-content">Te amo "nombre"</div>
	</div>
</body>
</html>

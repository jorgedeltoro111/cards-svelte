<script>
	import { each } from "svelte/internal";
import Card from "./components/Card.svelte";
	const datas = [
		{title: 'Felicidad', message: 'Eres el amor de mi vida, y siempre quiero que lo tengas en cuenta, siempre tendras mi apoyo pase lo que pase porque para mi eres lo mas importante que me ha sucedido. juntos lo hemos construido y somos uno mismo.'},
		{title: 'Tristeza', message: 'Recuerda que siempre hay una solucion para todo y debes pensar que es un sentimiento pasajero solo debes tener tu espacio y depues empujar duro para disfrutar con tus seres queridos, te conozco y se que nunca te rindes.'},
		{title: 'Estres', message: 'Toma asiento, respira y piensa que ese estres no es lo suficientemente fuerte para poder tirar a una mujer tan chingona como tu. Tu eres lo mas importante.'},
		{title: 'Euforia', message: 'Rie, brinca y baila expresa toda tu euforia, me encantas porque eso es lo que te caracteriza. ser plena y feliz.'},
		{title: 'Amor', message: 'Ama a todas las personas que te dan y brindan su apoyo. ellos te aman, yo te amo y siempre estare contigo.'}
	]
</script>
<style>
	:global(body){
		background-color: rgb(243, 81, 81);
	}
</style>
<main>
	{#each datas as data}
		<Card data={data}/>
	{/each}
</main>
<script>
	import Header from "./Header.svelte";
	import PizzaCard from "./PizzaCard.svelte";

	let arrayPizza = [
		{
			image: "/img/image 2pizza.png",
			name: "Pizza2",
			price: "350",
			size: [
				{ name: "20cm", value: "20cm" },
				{ name: "30cm", value: "30cm" },
				{ name: "40cm", value: "40cm" },
			],
		},
		{
			image: "/img/image 2pizza.png",
			name: "Pizza3",
			price: "450",
			size: [
				{ name: "20cm", value: "20cm" },
				{ name: "30cm", value: "30cm" },
				{ name: "40cm", value: "40cm" },
			],
		},
		{
			image: "/img/image 5pizza.png",
			name: "Pizza2",
			price: "350",
			size: [
				{ name: "20cm", value: "20cm" },
				{ name: "30cm", value: "30cm" },
				{ name: "40cm", value: "40cm" },
			],
		},
		{
			image: "/img/image 2pizza.png",
			name: "Pizza2",
			price: "350",
			size: [
				{ name: "20cm", value: "20cm" },
				{ name: "30cm", value: "30cm" },
				{ name: "40cm", value: "40cm" },
			],
		},
		{
			image: "/img/image 2pizza.png",
			name: "Pizza2",
			price: "350",
			size: [
				{ name: "20cm", value: "20cm" },
				{ name: "30cm", value: "30cm" },
				{ name: "40cm", value: "40cm" },
			],
		},
		{
			image: "/img/image 2pizza.png",
			name: "Pizza2",
			price: "350",
			size: [
				{ name: "20cm", value: "20cm" },
				{ name: "30cm", value: "30cm" },
				{ name: "40cm", value: "40cm" },
			],
		},
		{
			image: "/img/image 2pizza.png",
			name: "Pizza2",
			price: "350",
			size: [
				{ name: "20cm", value: "20cm" },
				{ name: "30cm", value: "30cm" },
				{ name: "40cm", value: "40cm" },
			],
		},
		{
			image: "/public/img/image 2pizza.png",
			name: "Pizza2",
			price: "350",
			size: [
				{ name: "20cm", value: "20cm" },
				{ name: "30cm", value: "30cm" },
				{ name: "40cm", value: "40cm" },
			],
		},
	];
</script>

<Header />
<section id="menu">
	<div class="container">
		{#each arrayPizza as pizza}
			<PizzaCard
				image={pizza.image}
				name={pizza.name}
				price={pizza.price}
			/>
		{/each}
	</div>
</section>

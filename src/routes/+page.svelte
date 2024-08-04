<script lang="ts">
	import Button from '$lib/components/ui/button/button.svelte';
	import * as Card from '$lib/components/ui/card/index.js';

	const programmingLanguages = [
		{
			name: 'Rust',
			logo: {
				url: 'https://www.svgrepo.com/show/376347/rust.svg',
				alt: 'Rust Logo'
			}
		},
		{
			name: 'Python',
			logo: {
				url: 'https://www.svgrepo.com/show/452091/python.svg',
				alt: 'Python Logo'
			}
		},
		{
			name: 'Javascript',
			logo: {
				url: 'https://www.svgrepo.com/show/349419/javascript.svg',
				alt: 'Javascript Logo'
			}
		},
		{
			name: 'Java',
			logo: {
				url: 'https://www.svgrepo.com/show/452234/java.svg',
				alt: 'Java Logo'
			}
		},
		{
			name: 'C# (C-Sharp)',
			logo: {
				url: 'https://www.svgrepo.com/show/353622/c-sharp.svg',
				alt: 'C Sharp Logo'
			}
		}
	];
</script>

<section class="space-y-5 pb-12">
	<h1>
		<span class="text-yellow-500">Transforming ideas</span> into <span class="">reality</span>
	</h1>
	<p class="lead">
		It is a creative hub where imagination meets craftsmanship to transform ideas into tangible
		realities. At Preline Agency, we specialize in turning conceptual visions into concrete forms,
		whether it be through design, artistry, or technological innovation.
	</p>
	<div class="flex flex-row items-center gap-5">
		<Button>Contact Us</Button>
		<Button variant="link">Learn More</Button>
	</div>
</section>
<section>
	<h2 class="border-none pb-0 font-bold">Your System, Your Choice!</h2>
	<p class="lead pb-5">
		We can build your system with programming languages that you're already familiar with.
	</p>
	<div class="grid grid-cols-5 items-center justify-between gap-5">
		{#each programmingLanguages as language}
			<Card.Root>
				<Card.Header class="flex flex-row items-center justify-center">
					<img class="h-24 w-24" src={language.logo.url} alt={language.logo.alt} />
				</Card.Header>
				<Card.Footer>
					<h4 class="w-full text-center font-bold">{language.name}</h4>
				</Card.Footer>
			</Card.Root>
		{/each}
	</div>
</section>

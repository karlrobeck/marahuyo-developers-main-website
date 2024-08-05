<script lang="ts">
	import Button from '$lib/components/ui/button/button.svelte';
	import * as Card from '$lib/components/ui/card/index.js';
	import * as Accordion from '$lib/components/ui/accordion/index.js';
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
		},
		{
			name: 'GO',
			logo: {
				url: 'https://www.svgrepo.com/show/452214/go.svg',
				alt: 'Go Programming Language Logo'
			}
		}
	];
</script>

<section class="space-y-5 pb-12">
	<h1>
		<span class="text-yellow-500">Transforming ideas</span> into <span class="">reality</span>
	</h1>
	<p class="lead">
		We are software developers that specialize on building fast, reliable safe programs for your
		business.
	</p>
	<div class="flex flex-row items-center gap-5">
		<Button>Contact Us</Button>
		<Button variant="link">Learn More</Button>
	</div>
</section>
<section class="space-y-5 pb-12">
	<h2 class="border-none">Our Services</h2>
	<p class="lead pb-5">See our services that we offer for your needs.</p>
	<div class="">
		<Accordion.Root>
			<Accordion.Item value="service-1">
				<Accordion.Trigger>Github Project Consulation</Accordion.Trigger>
				<Accordion.Content>
					<p>We offer insdustry standard Code review</p>
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="service-2">
				<Accordion.Trigger>Custom Website for your business</Accordion.Trigger>
				<Accordion.Content>
					<p>
						We offer service to create website for your business, personal porfolio projects, System
						Documentation, and many more.
					</p>
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="service-3">
				<Accordion.Trigger>Google Adsense Compilient website</Accordion.Trigger>
				<Accordion.Content>
					<p>
						Out of the box, all website that we product comply with Google Adsense Specification for
						easy approval
					</p>
				</Accordion.Content>
			</Accordion.Item>
			<Accordion.Item value="service-4">
				<Accordion.Trigger>Figma Prototypes</Accordion.Trigger>
				<Accordion.Content>
					<p>We offer Figma Prototypes for your system / business</p>
				</Accordion.Content>
			</Accordion.Item>
		</Accordion.Root>
	</div>
</section>
<section class="space-y-5 pb-12">
	<h2 class="border-none pb-0 font-bold">Your System, Your Choice!</h2>
	<p class="lead pb-5">
		We can build your system with programming languages that you're already familiar with.
	</p>
	<div class="grid grid-cols-6 items-center justify-between gap-5">
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
<section class="flex flex-col items-center space-y-5 pb-12">
	<h1>Turn your ideas into reality</h1>
	<p class="lead">Contact us for more information.</p>
	<div>
		<Button>Github</Button>
		<Button>Whatsapp</Button>
		<Button>Facebook</Button>
	</div>
</section>

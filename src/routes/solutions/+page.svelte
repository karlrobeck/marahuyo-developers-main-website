<script lang="ts">
	import { Input } from '$lib/components/ui/input';
	import * as Card from '$lib/components/ui/card/index';
	import { Button } from '$lib/components/ui/button';

	const projects = [
		{
			title: 'Rust: Point Of Sale System',
			programmingLanguage: 'Rust',
			images: [
				{
					src: 'https://www.svgrepo.com/show/376347/rust.svg',
					alt: 'Rust Logo'
				}
			],
			description:
				'Rust Based Point of sale system good for cheap operation, fast content delivery and robust security'
		},
		{
			title: 'Maya Payment System',
			programmingLanguage: 'Rust, Python, Go, Javascript',
			images: [
				{
					src: 'https://www.svgrepo.com/show/376347/rust.svg',
					alt: 'Rust Logo'
				}
			],
			description: 'Ready made backend API for processing payments written in multiple languages'
		}
	];
</script>

<h1>Solutions</h1>
<p class="lead">See solutions that we have for most common cases</p>
<div class="w-1/4">
	<Input placeholder="Search" />
</div>
<div class="border border-border"></div>
<section class="grid grid-cols-3 gap-5">
	{#each projects as project}
		<Card.Root>
			<Card.Header>
				<img class="h-64" src={project.images[0].src} alt={project.images[0].alt} />
				<Card.Title>{project.title}</Card.Title>
				<Card.Description>Programming Language: {project.programmingLanguage}</Card.Description>
			</Card.Header>
			<Card.Content>{project.description}</Card.Content>
			<Card.Footer class="gap-5">
				<Button>View Project</Button>
				<Button variant="link">Contact Us for more</Button>
			</Card.Footer>
		</Card.Root>
	{/each}
</section>

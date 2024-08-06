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
					<p>We offer insdustry standard Code review, CI/CD Testing, Documentation and more.</p>
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
				<Accordion.Trigger>Google Adsense Compliant website</Accordion.Trigger>
				<Accordion.Content>
					<p>
						Out of the box, all website that we produce comply with Google Adsense Specification for
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
	<Button variant="link">See our production ready solutions</Button>
</section>
<section class="flex flex-col items-center space-y-5 pb-12">
	<h1>Turn your ideas into reality</h1>
	<p class="lead">Contact us for more information.</p>
	<span class="muted">Email: marahuyodevelopers@gmail.com</span>
	<div>
		<Button target="_blank" href="https://github.com/karlrobeck" class="gap-3">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="16"
				height="16"
				fill="currentColor"
				class="bi bi-facebook"
				viewBox="0 0 16 16"
			>
				<path
					d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951"
				/>
			</svg> Github
		</Button>
		<Button target="_blank" href="whatsapp://send?abid=+639055557351" class="gap-3">
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="16"
				height="16"
				fill="currentColor"
				class="bi bi-whatsapp"
				viewBox="0 0 16 16"
			>
				<path
					d="M13.601 2.326A7.85 7.85 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.9 7.9 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.9 7.9 0 0 0 13.6 2.326zM7.994 14.521a6.6 6.6 0 0 1-3.356-.92l-.24-.144-2.494.654.666-2.433-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931 6.56 6.56 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592m3.615-4.934c-.197-.099-1.17-.578-1.353-.646-.182-.065-.315-.099-.445.099-.133.197-.513.646-.627.775-.114.133-.232.148-.43.05-.197-.1-.836-.308-1.592-.985-.59-.525-.985-1.175-1.103-1.372-.114-.198-.011-.304.088-.403.087-.088.197-.232.296-.346.1-.114.133-.198.198-.33.065-.134.034-.248-.015-.347-.05-.099-.445-1.076-.612-1.47-.16-.389-.323-.335-.445-.34-.114-.007-.247-.007-.38-.007a.73.73 0 0 0-.529.247c-.182.198-.691.677-.691 1.654s.71 1.916.81 2.049c.098.133 1.394 2.132 3.383 2.992.47.205.84.326 1.129.418.475.152.904.129 1.246.08.38-.058 1.171-.48 1.338-.943.164-.464.164-.86.114-.943-.049-.084-.182-.133-.38-.232"
				/>
			</svg> Whatsapp
		</Button>
		<Button
			target="_blank"
			href="https://www.facebook.com/profile.php?id=61563585279659"
			class="gap-3"
		>
			<svg
				xmlns="http://www.w3.org/2000/svg"
				width="16"
				height="16"
				fill="currentColor"
				class="bi bi-facebook"
				viewBox="0 0 16 16"
			>
				<path
					d="M16 8.049c0-4.446-3.582-8.05-8-8.05C3.58 0-.002 3.603-.002 8.05c0 4.017 2.926 7.347 6.75 7.951v-5.625h-2.03V8.05H6.75V6.275c0-2.017 1.195-3.131 3.022-3.131.876 0 1.791.157 1.791.157v1.98h-1.009c-.993 0-1.303.621-1.303 1.258v1.51h2.218l-.354 2.326H9.25V16c3.824-.604 6.75-3.934 6.75-7.951"
				/>
			</svg> Facebook
		</Button>
	</div>
</section>

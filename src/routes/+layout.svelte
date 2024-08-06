<script lang="ts">
	import Button from '$lib/components/ui/button/button.svelte';
	import '../app.css';
</script>

<main class="container max-w-7xl">
	<header class="flex flex-row justify-between p-4">
		<div class="flex flex-row items-center gap-5">
			<img
				class="h-12 w-12 rounded-md"
				src="https://scontent.fmnl25-4.fna.fbcdn.net/v/t39.30808-6/454263195_122098053050459721_951208295823453167_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=6ee11a&_nc_ohc=pxeOlXmFuDYQ7kNvgFtDjnh&_nc_ht=scontent.fmnl25-4.fna&oh=00_AYAa3GKUaxM5HjNRoW8r54KoKuCGQKXUFVg1Er2QVfrIMQ&oe=66B5AC5D"
				alt="Marahuyo developers Logo"
			/>
			<h4 class="font-bold">Marahuyo Developers</h4>
		</div>
		<nav class="flex flex-row items-center gap-5">
			<ul class="flex flex-row items-center gap-5">
				<li>
					<Button variant="link" href="/">Home</Button>
				</li>
				<li>
					<Button variant="link" href="/solutions">Solutions</Button>
				</li>
				<li>
					<Button variant="link" href="/about">About</Button>
				</li>
			</ul>
		</nav>
	</header>
	<div class="space-y-5 p-4 py-24">
		<slot></slot>
	</div>
	<footer class="flex flex-col gap-5 border-t border-border py-12 pb-24">
		<div class="flex flex-row items-center gap-5">
			<img
				class="h-12 w-12 rounded-md"
				src="https://scontent.fmnl25-4.fna.fbcdn.net/v/t39.30808-6/454263195_122098053050459721_951208295823453167_n.jpg?_nc_cat=109&ccb=1-7&_nc_sid=6ee11a&_nc_ohc=pxeOlXmFuDYQ7kNvgFtDjnh&_nc_ht=scontent.fmnl25-4.fna&oh=00_AYAa3GKUaxM5HjNRoW8r54KoKuCGQKXUFVg1Er2QVfrIMQ&oe=66B5AC5D"
				alt="Marahuyo developers Logo"
			/>
			<h4 class="font-bold">Marahuyo Developers</h4>
		</div>
		<span class="small">© 2024 Mayahuyo Developer Team</span>
		<ul>
			<li>
				<Button variant="link" class="w-fit" href="/about/privacy">Privacy Policy</Button>
			</li>
			<li>
				<Button variant="link" class="w-fit" href="/about/terms-and-conditions"
					>Terms of services</Button
				>
			</li>
		</ul>
	</footer>
</main>

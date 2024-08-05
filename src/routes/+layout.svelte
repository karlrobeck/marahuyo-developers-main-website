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
					<Button variant="link">Home</Button>
				</li>
				<li>
					<Button variant="link">Solutions</Button>
				</li>
				<li>
					<Button variant="link">About</Button>
				</li>
			</ul>
			<div class="h-full border-t border-black sm:border-s sm:border-t-0"></div>
			<ul class="flex flex-row items-center gap-5">
				<li>
					<Button variant="ghost">
						<svg
							xmlns="http://www.w3.org/2000/svg"
							width="16"
							height="16"
							fill="currentColor"
							class="bi bi-github"
							viewBox="0 0 16 16"
						>
							<path
								d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27s1.36.09 2 .27c1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.01 8.01 0 0 0 16 8c0-4.42-3.58-8-8-8"
							/>
						</svg>
					</Button>
				</li>
				<li>
					<Button variant="ghost">
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
						</svg>
					</Button>
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
				<Button variant="link" class="w-fit">Privacy Policy</Button>
			</li>
			<li>
				<Button variant="link" class="w-fit">Terms of services</Button>
			</li>
		</ul>
	</footer>
</main>

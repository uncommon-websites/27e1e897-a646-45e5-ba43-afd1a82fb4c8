<script lang="ts">
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";

	let {
		title,
		subtitle,
		imageSrc = "https://www.unc.mn/image-placeholder.svg",
		...rest
	}: {
		title: string;
		subtitle: string;
		imageSrc: string;
		[key: string]: any;
	} = $props();
</script>

<header class="bg-gray-950 text-white border-b border-gray-800" {...rest}>
	<div class="section-px section-py container mx-auto">
		<div class="grid gap-16 lg:gap-20">
			<div class="text-center max-w-4xl mx-auto">
				<h1 class="text-display font-[450] mb-4 tracking-tight text-white">
					{title}
				</h1>
				<p class="text-title2 text-gray-300 font-normal">
					{subtitle}
				</p>
			</div>
			<div class="aspect-video overflow-clip rounded-xl bg-gray-900 border border-gray-800">
				<img
					class="h-full w-full object-cover"
					src={imageSrc}
					alt="Our team collaborating to transform security operations"
				/>
			</div>
		</div>
	</div>
</header>

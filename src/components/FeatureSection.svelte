<script lang="ts">
	export let title: string;
	export let icon: string;
</script>

<section class="relative ">
	<dt>
		<span
			class="absolute flex items-center justify-center h-12 w-12 rounded-md bg-indigo-500 text-white"
		>
			<svg
				class="h-6 w-6"
				xmlns="http://www.w3.org/2000/svg"
				fill="none"
				viewBox="0 0 24 24"
				stroke-width="2"
				stroke="currentColor"
				aria-hidden="true"
			>
				<path stroke-linecap="round" stroke-linejoin="round" d={icon} />
			</svg>
		</span>
		<p class="ml-16 text-lg leading-6 font-medium text-gray-900">{title}</p>
	</dt>
	<dd class="mt-2 ml-16 text-base text-gray-500">
		<slot />
	</dd>
</section>

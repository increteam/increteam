<script>
	import FeatureSection from '../components/FeatureSection.svelte';
</script>

<main class="text-white py-28 text-center bg-indigo-600">
	<h1 class="font-title px-10 text-2xl md:text-4xl uppercase tracking-widest">
		Manage your work's or school's team to share what you need.
	</h1>
</main>

<div class="py-12 bg-white max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
	<span class="lg:text-center">
		<h2 class="text-base text-indigo-600 font-semibold tracking-wide uppercase">Always Updated</h2>
		<p class="mt-2 text-3xl leading-8 font-extrabold tracking-tight text-gray-900 sm:text-4xl">
			A better way of working!
		</p>
		<p class="mt-4 max-w-2xl text-xl text-gray-500 lg:mx-auto">
			Create individual teams that help you share what you need.
		</p>
	</span>

	<dl class="mt-10 space-y-10 md:space-y-0 md:grid md:grid-cols-2 md:gap-x-8 md:gap-y-10">
		<FeatureSection
			title="Instant Update!"
			icon="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9a9 9 0 01-9-9m9 9c1.657 0 3-4.03 3-9s-1.343-9-3-9m0 18c-1.657 0-3-4.03-3-9s1.343-9 3-9m-9 9a9 9 0 019-9"
		>
			Once someone publishes material, just got refresh the page to see the changes instantly.
		</FeatureSection>
		<FeatureSection
			title="Permissions Balance"
			icon="M3 6l3 1m0 0l-3 9a5.002 5.002 0 006.001 0M6 7l3 9M6 7l6-2m6 2l3-1m-3 1l-3 9a5.002 5.002 0 006.001 0M18 7l3 9m-3-9l-6-2m0-2v2m0 16V5m0 16H9m3 0h3"
		>
			Give your members different permissions to access different areas of the app.
		</FeatureSection>
		<FeatureSection title="Fast Team Sharing!" icon="M13 10V3L4 14h7v7l9-11h-7z">
			It's blazingly fast and easy to share documents and seeing them in a nice format.
		</FeatureSection>
		<FeatureSection
			title="Chat"
			icon="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z"
		>
			Create threads of chat and get notified when someone replies to them.
		</FeatureSection>
	</dl>
</div>

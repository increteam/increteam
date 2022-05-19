<script>
	import '../app.css';
	let menuHidden = true;
	let userHidden = true;
</script>

<div class="w-full text-gray-700 bg-white dark-mode:text-gray-200 dark-mode:bg-gray-800">
	<div
		class="flex flex-col max-w-screen-xl px-4 mx-auto md:items-center md:justify-between md:flex-row md:px-6 lg:px-8"
	>
		<div class="p-4 flex flex-row items-center justify-between">
			<a
				href="/"
				class="text-lg font-semibold tracking-widest text-gray-900 uppercase rounded-lg dark-mode:text-white focus:outline-none focus:shadow-outline"
				>INCRETEAM</a
			>
			<button
				class="md:hidden rounded-lg focus:outline-none focus:shadow-outline"
				on:click={() => (menuHidden = !menuHidden)}
			>
				<svg fill="currentColor" viewBox="0 0 20 20" class="w-6 h-6">
					<path
						fill-rule="evenodd"
						d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM9 15a1 1 0 011-1h6a1 1 0 110 2h-6a1 1 0 01-1-1z"
						clip-rule="evenodd"
					/>
				</svg>
			</button>
		</div>
		<nav
			class:hidden={menuHidden}
			class="flex-col flex-grow pb-4 md:pb-0 hidden md:flex md:justify-end md:flex-row"
		>
			<a
				class="px-4 py-2 mt-2 text-sm font-semibold text-gray-900 rounded-lg md:mt-0 hover:text-gray-900 focus:text-gray-900 hover:bg-gray-200 focus:outline-none focus:shadow-outline"
				href="/">Home</a
			>
			<a
				class="px-4 py-2 mt-2 text-sm font-semibold text-gray-900 rounded-lg md:mt-0 hover:text-gray-900 focus:text-gray-900 hover:bg-gray-200 focus:outline-none focus:shadow-outline"
				href="/">Teams</a
			>
			<a
				class="px-4 py-2 mt-2 text-sm font-semibold text-gray-900 rounded-lg md:mt-0 hover:text-gray-900 focus:text-gray-900 hover:bg-gray-200 focus:outline-none focus:shadow-outline"
				href="/">About</a
			>
			<span class="relative">
				<button
					class="bg-slate-600 text-white rounded-full items-center px-3 py-2 mt-2 text-sm font-semibold text-left bg-transparent dark-mode:bg-transparent dark-mode:focus:text-white dark-mode:hover:text-white dark-mode: dark-mode:hover:bg-gray-600 md:w-auto inline md:mt-0 md:ml-4 hover:text-gray-900 focus:text-gray-900 hover:bg-gray-200 focus:bg-gray-200 focus:outline-none focus:shadow-outline"
					on:click={() => (userHidden = !userHidden)}
				>
					AG
				</button>
				<div class="absolute right-0 w-full mt-2 origin-top-right rounded-md shadow-lg md:w-48">
					<div
						class:hidden={userHidden}
						class="px-2 py-2 bg-white rounded-md shadow dark-mode:bg-gray-800"
					>
						<a
							class="block px-4 py-2 mt-2 text-sm font-semibold bg-transparent rounded-lg dark-mode:bg-transparent dark-mode:hover:bg-gray-600 dark-mode: dark-mode:focus:text-white dark-mode:hover:text-white dark-mode:text-gray-200 md:mt-0 hover:text-gray-900 focus:text-gray-900 hover:bg-gray-200 focus:bg-gray-200 focus:outline-none focus:shadow-outline"
							href="/">Settings</a
						>
						<a
							class="block px-4 py-2 mt-2 text-sm font-semibold bg-transparent rounded-lg dark-mode:bg-transparent dark-mode:hover:bg-gray-600 dark-mode: dark-mode:focus:text-white dark-mode:hover:text-white dark-mode:text-gray-200 md:mt-0 hover:text-gray-900 focus:text-gray-900 hover:bg-gray-200 focus:bg-gray-200 focus:outline-none focus:shadow-outline"
							href="/">Privacy Policy</a
						>
					</div>
				</div>
			</span>
		</nav>
	</div>
</div>

<span
	on:click={() => {
		menuHidden ||= true;
		userHidden ||= true;
	}}
>
	<slot />
</span>

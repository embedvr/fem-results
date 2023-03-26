<script lang="ts">
	import MaterialSymbolsBoltOutline from '~icons/material-symbols/bolt-outline';
	import IconoirBrain from '~icons/iconoir/brain';
	import IonChatbubbleEllipsesOutline from '~icons/ion/chatbubble-ellipses-outline';
	import MdiEyeOutline from '~icons/mdi/eye-outline';
</script>

<svelte:head>
	<title>Results Summary Challenge</title>
</svelte:head>

<div
	class="flex h-full flex-col rounded-[2rem] sm:h-fit sm:flex-row sm:bg-white sm:drop-shadow-xl"
>
	<header
		class="flex h-[22rem] flex-col items-center justify-between rounded-b-[2rem] bg-gradient-to-b from-indigo-600 to-indigo-700 p-7 sm:h-[27rem] sm:w-[20rem] sm:rounded-[2rem]"
	>
		<h1 class="text-md font-semibold text-gray-300 opacity-75">Your Result</h1>
		<div
			class="flex h-36 w-36 flex-col items-center justify-center rounded-full bg-gradient-to-b from-indigo-800 to-transparent sm:h-40 sm:w-40"
		>
			<h2 class="text-5xl font-bold text-white">76</h2>
			<span class="font-medium text-gray-300 opacity-75">of 100</span>
		</div>
		<div class="flex flex-col items-center justify-center gap-1 text-center">
			<h3 class="text-2xl font-bold text-white">Great</h3>
			<span class="font-medium text-gray-300 opacity-75"
				>You scored higher than 69% of the people who have taken these tests.</span
			>
		</div>
	</header>
	<main class="flex w-full flex-col sm:w-[20rem]">
		<div class="px-7 py-5">
			<h4 class="text-lg font-medium">Summary</h4>
			<div class="mt-4 flex flex-col justify-around gap-3">
				<div
					class="flex w-full flex-row items-center justify-between rounded-xl bg-red-300 bg-opacity-10 p-4"
				>
					<div
						class="flex flex-row items-center gap-3 font-medium text-red-400"
					>
						<MaterialSymbolsBoltOutline class="h-5 w-5" />
						<span>Reaction</span>
					</div>
					<div class="font-medium">
						<span class="text-black">80</span>
						<span class="text-gray-400"> / 100</span>
					</div>
				</div>
				<div
					class="flex w-full flex-row items-center justify-between rounded-xl bg-yellow-300 bg-opacity-10 p-4"
				>
					<div
						class="flex flex-row items-center gap-3 font-medium text-yellow-400"
					>
						<IconoirBrain class="h-5 w-5" />
						<span>Memory</span>
					</div>
					<div class="font-medium">
						<span class="text-black">92</span>
						<span class="text-gray-400"> / 100</span>
					</div>
				</div>
				<div
					class="flex w-full flex-row items-center justify-between rounded-xl bg-green-300 bg-opacity-10 p-4"
				>
					<div
						class="flex flex-row items-center gap-3 font-medium text-green-400"
					>
						<IonChatbubbleEllipsesOutline class="h-5 w-5" />
						<span>Verbal</span>
					</div>
					<div class="font-medium">
						<span class="text-black">61</span>
						<span class="text-gray-400"> / 100</span>
					</div>
				</div>
				<div
					class="flex w-full flex-row items-center justify-between rounded-xl bg-blue-300 bg-opacity-10 p-4"
				>
					<div
						class="flex flex-row items-center gap-3 font-medium text-blue-400"
					>
						<MdiEyeOutline class="h-5 w-5" />
						<span>Visual</span>
					</div>
					<div class="font-medium">
						<span class="text-black">72</span>
						<span class="text-gray-400"> / 100</span>
					</div>
				</div>
			</div>
		</div>
		<div class="flex h-full w-full items-center justify-center px-7 py-4">
			<button
				class="h-full w-full rounded-full bg-gray-700 from-indigo-600 to-indigo-700 p-4 font-bold text-white transition-colors hover:bg-gradient-to-b active:bg-gradient-to-b"
			>
				Continue
			</button>
		</div>
	</main>
</div>

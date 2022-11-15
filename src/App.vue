<script setup>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import Card from "./components/Card.vue";
import Location from "./components/Location.vue";
import BottomIcon from "./components/BottomIcon.vue";
</script>

<template>
	<div class="w-full flex justify-center items-center pt-9">
		<div
			id="mobile"
			class="border w-72 h-full border-black overflow-x-hidden mb-9"
		>
			<div id="topbar" class="flex py-3 px-2 items-center">
				<span id="locationicon"
					><svg
						xmlns="http://www.w3.org/2000/svg"
						viewBox="0 0 24 24"
						fill="currentColor"
						class="w-4 h-4"
					>
						<path
							fill-rule="evenodd"
							d="M11.54 22.351l.07.04.028.016a.76.76 0 00.723 0l.028-.015.071-.041a16.975 16.975 0 001.144-.742 19.58 19.58 0 002.683-2.282c1.944-1.99 3.963-4.98 3.963-8.827a8.25 8.25 0 00-16.5 0c0 3.846 2.02 6.837 3.963 8.827a19.58 19.58 0 002.682 2.282 16.975 16.975 0 001.145.742zM12 13.5a3 3 0 100-6 3 3 0 000 6z"
							clip-rule="evenodd"
						/>
					</svg>
				</span>
				<div class="pl-2 text-sm font-medium">BH-341, California</div>

				<span id="dorpdownicon" class="ml-auto"
					><svg
						xmlns="http://www.w3.org/2000/svg"
						fill="none"
						viewBox="0 0 24 24"
						stroke-width="1.5"
						stroke="currentColor"
						class="w-6 h-6"
					>
						<path
							stroke-linecap="round"
							stroke-linejoin="round"
							d="M19.5 8.25l-7.5 7.5-7.5-7.5"
						/>
					</svg>
				</span>
			</div>
			<div id="welcome" class="welcome-bg p-4 text-white rounded-b-2xl">
				<div class="flex justify-between">
					<h1 class="text-xl">Welcome Walker!</h1>
					<div
						class="bg-white/20 flex justify-center items-center p-2 rounded-full"
					>
						<span id="bellicon"
							><svg
								xmlns="http://www.w3.org/2000/svg"
								fill="none"
								viewBox="0 0 24 24"
								stroke-width="1.5"
								stroke="currentColor"
								class="w-4 h-4"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									d="M14.857 17.082a23.848 23.848 0 005.454-1.31A8.967 8.967 0 0118 9.75v-.7V9A6 6 0 006 9v.75a8.967 8.967 0 01-2.312 6.022c1.733.64 3.56 1.085 5.455 1.31m5.714 0a24.255 24.255 0 01-5.714 0m5.714 0a3 3 0 11-5.714 0"
								/>
							</svg>
						</span>
					</div>
				</div>
				<div class="h-4"></div>
				<div
					id="serachinput"
					class="flex bg-white rounded-md items-center px-2"
				>
					<span>
						<svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="1.5"
							stroke="currentColor"
							class="w-4 h-4 text-gray-400"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M21 21l-5.197-5.197m0 0A7.5 7.5 0 105.196 5.196a7.5 7.5 0 0010.607 10.607z"
							/>
						</svg>
					</span>
					<input
						type="text"
						placeholder="Search for locations"
						class="w-full rounded-md text-gray-900 text-sm outline-none border-none focus:ring-0 focus:border-none"
					/>
				</div>
				<div class="h-4"></div>
				<div>Recently parked</div>
				<div class="h-2"></div>
				<div>
					<Location />
					<Location />
					<Location />
				</div>
			</div>

			<div id="silderlist">
				<div class="h-4"></div>
				<h3 class="text-black 900 text-sm px-4">Parking Spots near you</h3>
				<div class="h-2"></div>
				<div
					class="flex overflow-hidden min-w-lg pl-4 flex-wrap gap-6"
					style="width: 500px"
				>
					<Card />
					<Card />
				</div>
			</div>
			<!-- <div id="silderlisttype2"></div> -->
			<div class="h2"></div>
			<div
				id="stickynavbar"
				class="flex h-18 gap-4 text-gray-500 text-sm py-2 px-4 rounded-t-xl botton-shadow justify-evenly"
			>
				<div class="flex flex-col">
					<span id="homeicon" class="mx-auto"
						><svg
							xmlns="http://www.w3.org/2000/svg"
							viewBox="0 0 20 20"
							fill="currentColor"
							class="w-6 h-6 fill-green-600"
						>
							<path
								fill-rule="evenodd"
								d="M9.293 2.293a1 1 0 011.414 0l7 7A1 1 0 0117 11h-1v6a1 1 0 01-1 1h-2a1 1 0 01-1-1v-3a1 1 0 00-1-1H9a1 1 0 00-1 1v3a1 1 0 01-1 1H5a1 1 0 01-1-1v-6H3a1 1 0 01-.707-1.707l7-7z"
								clip-rule="evenodd"
							/>
						</svg>
					</span>
					<span class="text-xs text-green-600 font-semibold">Home</span>
				</div>
				<div class="flex flex-col">
					<span id="homeicon" class="mx-auto"
						><svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="1.5"
							stroke="currentColor"
							class="w-6 h-6"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M15 10.5a3 3 0 11-6 0 3 3 0 016 0z"
							/>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M19.5 10.5c0 7.142-7.5 11.25-7.5 11.25S4.5 17.642 4.5 10.5a7.5 7.5 0 1115 0z"
							/>
						</svg>
					</span>
					<span class="text-xs text-gray-600 font-semibold">Home</span>
				</div>
				<div class="flex flex-col">
					<span id="homeicon" class="mx-auto"
						><svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="1.5"
							stroke="currentColor"
							class="w-6 h-6"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M6.75 3v2.25M17.25 3v2.25M3 18.75V7.5a2.25 2.25 0 012.25-2.25h13.5A2.25 2.25 0 0121 7.5v11.25m-18 0A2.25 2.25 0 005.25 21h13.5A2.25 2.25 0 0021 18.75m-18 0v-7.5A2.25 2.25 0 015.25 9h13.5A2.25 2.25 0 0121 11.25v7.5m-9-6h.008v.008H12v-.008zM12 15h.008v.008H12V15zm0 2.25h.008v.008H12v-.008zM9.75 15h.008v.008H9.75V15zm0 2.25h.008v.008H9.75v-.008zM7.5 15h.008v.008H7.5V15zm0 2.25h.008v.008H7.5v-.008zm6.75-4.5h.008v.008h-.008v-.008zm0 2.25h.008v.008h-.008V15zm0 2.25h.008v.008h-.008v-.008zm2.25-4.5h.008v.008H16.5v-.008zm0 2.25h.008v.008H16.5V15z"
							/>
						</svg>
					</span>
					<span class="text-xs text-gray-600 font-semibold">booking</span>
				</div>
				<div class="flex flex-col">
					<span id="homeicon" class="mx-auto"
						><svg
							xmlns="http://www.w3.org/2000/svg"
							fill="none"
							viewBox="0 0 24 24"
							stroke-width="1.5"
							stroke="currentColor"
							class="w-6 h-6"
						>
							<path
								stroke-linecap="round"
								stroke-linejoin="round"
								d="M4.098 19.902a3.75 3.75 0 005.304 0l6.401-6.402M6.75 21A3.75 3.75 0 013 17.25V4.125C3 3.504 3.504 3 4.125 3h5.25c.621 0 1.125.504 1.125 1.125v4.072M6.75 21a3.75 3.75 0 003.75-3.75V8.197M6.75 21h13.125c.621 0 1.125-.504 1.125-1.125v-5.25c0-.621-.504-1.125-1.125-1.125h-4.072M10.5 8.197l2.88-2.88c.438-.439 1.15-.439 1.59 0l3.712 3.713c.44.44.44 1.152 0 1.59l-2.879 2.88M6.75 17.25h.008v.008H6.75v-.008z"
							/>
						</svg>
					</span>
					<span class="text-xs text-gray-600 font-semibold">Menu</span>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	import { fade } from 'svelte/transition';

	let firstName = '';
    let lastName = '';
	let email = '';
    let phone = '';
	let message = '';
	let showMessage = false;
	let showError = false;

	function handleClick() {
		if (firstName && lastName && email && message) {
			showError  = false;
            showMessage = true;
			firstName = '';
            lastName = '';
			email = '';
            phone = '';
			message = '';
		} else {
			showError = true;
            showMessage = false;
		}
	}
</script>


<div id="contact" class="bg-gray-100">
	<div class="max-w-7xl mx-auto py-16 px-4 sm:py-24 sm:px-6 lg:px-8">
		<div class="text-center">
			<h2 class="mt-2 text-3xl font-extrabold text-gray-900 tracking-tight sm:text-4xl">
				Contact us
			</h2>
			<p class="mt-5 max-w-prose mx-auto text-xl text-gray-500">
				We will respond to your query within 24 hours. Thank You
			</p>
		</div>

		<div class="mt-12 relative bg-white shadow-xl">
			<h2 class="sr-only">Contact us</h2>

			<div class="grid grid-cols-1 lg:grid-cols-3">
				<!-- Contact information -->
				<div class="relative overflow-hidden py-10 px-6 bg-indigo-700 sm:px-10 xl:p-12">
					<div class="absolute inset-0 pointer-events-none sm:hidden" aria-hidden="true">
						<svg
							class="absolute inset-0 w-full h-full"
							width="343"
							height="388"
							viewBox="0 0 343 388"
							fill="none"
							preserveAspectRatio="xMidYMid slice"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M-99 461.107L608.107-246l707.103 707.107-707.103 707.103L-99 461.107z"
								fill="url(#linear1)"
								fill-opacity=".1"
							/>
							<defs>
								<linearGradient
									id="linear1"
									x1="254.553"
									y1="107.554"
									x2="961.66"
									y2="814.66"
									gradientUnits="userSpaceOnUse"
								>
									<stop stop-color="#fff" />
									<stop offset="1" stop-color="#fff" stop-opacity="0" />
								</linearGradient>
							</defs>
						</svg>
					</div>
					<div
						class="hidden absolute top-0 right-0 bottom-0 w-1/2 pointer-events-none sm:block lg:hidden"
						aria-hidden="true"
					>
						<svg
							class="absolute inset-0 w-full h-full"
							width="359"
							height="339"
							viewBox="0 0 359 339"
							fill="none"
							preserveAspectRatio="xMidYMid slice"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M-161 382.107L546.107-325l707.103 707.107-707.103 707.103L-161 382.107z"
								fill="url(#linear2)"
								fill-opacity=".1"
							/>
							<defs>
								<linearGradient
									id="linear2"
									x1="192.553"
									y1="28.553"
									x2="899.66"
									y2="735.66"
									gradientUnits="userSpaceOnUse"
								>
									<stop stop-color="#fff" />
									<stop offset="1" stop-color="#fff" stop-opacity="0" />
								</linearGradient>
							</defs>
						</svg>
					</div>
					<div
						class="hidden absolute top-0 right-0 bottom-0 w-1/2 pointer-events-none lg:block"
						aria-hidden="true"
					>
						<svg
							class="absolute inset-0 w-full h-full"
							width="160"
							height="678"
							viewBox="0 0 160 678"
							fill="none"
							preserveAspectRatio="xMidYMid slice"
							xmlns="http://www.w3.org/2000/svg"
						>
							<path
								d="M-161 679.107L546.107-28l707.103 707.107-707.103 707.103L-161 679.107z"
								fill="url(#linear3)"
								fill-opacity=".1"
							/>
							<defs>
								<linearGradient
									id="linear3"
									x1="192.553"
									y1="325.553"
									x2="899.66"
									y2="1032.66"
									gradientUnits="userSpaceOnUse"
								>
									<stop stop-color="#fff" />
									<stop offset="1" stop-color="#fff" stop-opacity="0" />
								</linearGradient>
							</defs>
						</svg>
					</div>
					<h3 class="text-lg font-medium text-white">Contact information</h3>
					<p class="mt-6 text-base text-indigo-50 max-w-3xl">
						If you have any queries or wish to make an appointment, please contact us:

					</p>
					<dl class="mt-8 space-y-6">
						<dt><span class="sr-only">Phone number</span></dt>
						<dd class="flex text-base text-indigo-50">
							<!-- Heroicon name: outline/phone -->
							<svg
								class="flex-shrink-0 w-6 h-6 text-indigo-200"
								xmlns="http://www.w3.org/2000/svg"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
								aria-hidden="true"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z"
								/>
							</svg>
							<span class="ml-3">+44 29 2018 0325</span>
						</dd>
						<dt><span class="sr-only">Email</span></dt>
						<dd class="flex text-base text-indigo-50">
							<!-- Heroicon name: outline/mail -->
							<svg
								class="flex-shrink-0 w-6 h-6 text-indigo-200"
								xmlns="http://www.w3.org/2000/svg"
								fill="none"
								viewBox="0 0 24 24"
								stroke="currentColor"
								aria-hidden="true"
							>
								<path
									stroke-linecap="round"
									stroke-linejoin="round"
									stroke-width="2"
									d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"
								/>
							</svg>
							<span class="ml-3">support@insight-accountants.com</span>
						</dd>
					</dl>
				</div>

				<!-- Contact form -->
				<div class="py-10 px-6 sm:px-10 lg:col-span-2 xl:p-12">
					<h3 class="text-lg font-medium text-gray-900">Send us a message</h3>
					<form
						action="#"
						method="POST"
						class="mt-6 grid grid-cols-1 gap-y-6 sm:grid-cols-2 sm:gap-x-8"
					>
						<div>
							<label for="first_name" class="block text-sm font-medium text-gray-900"
								>First name</label
							>
							<div class="mt-1">
								<input
									type="text"
									name="first_name"
									id="first_name"
                                    bind:value={firstName}
									autocomplete="given-name"
									class="py-3 px-4 block w-full border shadow-sm text-gray-900 focus:ring-indigo-500 focus:border-indigo-500 border-gray-300 rounded-md"
								/>
							</div>
						</div>
						<div>
							<label for="last_name" class="block text-sm font-medium text-gray-900"
								>Last name</label
							>
							<div class="mt-1">
								<input
									type="text"
									name="last_name"
									id="last_name"
                                    bind:value={lastName}
									autocomplete="family-name"
									class="py-3 px-4 block w-full border shadow-sm text-gray-900 focus:ring-indigo-500 focus:border-indigo-500 border-gray-300 rounded-md"
								/>
							</div>
						</div>
						<div>
							<label for="email" class="block text-sm font-medium text-gray-900">Email</label>
							<div class="mt-1">
								<input
									id="email"
									name="email"
									type="email"
                                    bind:value={email}
									autocomplete="email"
									class="py-3 px-4 block w-full border shadow-sm text-gray-900 focus:ring-indigo-500 focus:border-indigo-500 border-gray-300 rounded-md"
								/>
							</div>
						</div>
						<div>
							<div class="flex justify-between">
								<label for="phone" class="block text-sm font-medium text-gray-900">Phone</label>
								<span id="phone-optional" class="text-sm text-gray-500">Optional</span>
							</div>
							<div class="mt-1">
								<input
									type="text"
									name="phone"
									id="phone"
                                    bind:value={phone}
									autocomplete="tel"
									class="py-3 px-4 block w-full border shadow-sm text-gray-900 focus:ring-indigo-500 focus:border-indigo-500 border-gray-300 rounded-md"
									aria-describedby="phone-optional"
								/>
							</div>
						</div>
						
						<div class="sm:col-span-2">
							<div class="flex justify-between">
								<label for="message" class="block text-sm font-medium text-gray-900">Message</label>
								<span id="message-max" class="text-sm text-gray-500">Max. 500 characters</span>
							</div>
							<div class="mt-1">
								<textarea
									id="message"
									name="message"
									rows="4"
                                    bind:value={message}
									class="py-3 px-4 block w-full border shadow-sm text-gray-900 focus:ring-indigo-500 focus:border-indigo-500 border-gray-300 rounded-md"
									aria-describedby="message-max"
								/>
							</div>
						</div>
						<div class="sm:col-span-2 sm:flex sm:justify-end sm:items-center">
                            {#if showMessage}
                            <p class="mr-4 text-indigo-500 font-semibold">Thanks! We recived your message, and someone from our team will try to reply as soon as possible!</p>
                            {/if}
                            {#if showError}
                            <p class="mr-4 text-yellow-500 font-semibold">Please fill all the required fields</p>
                            {/if}
							<button
								type="button"
                                on:click={handleClick}
								class="mt-2 w-full inline-flex items-center justify-center px-6 py-3 border border-transparent rounded-md shadow-sm text-base font-medium text-white bg-indigo-600 hover:bg-indigo-700 focus:outline-none focus:ring-2 focus:ring-offset-2 focus:ring-indigo-500 sm:w-auto"
							>
								Submit
							</button>
						</div>
					</form>
				</div>
			</div>
		</div>
	</div>
</div>

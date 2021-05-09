<script>
    export let name;
    export let image;
    export let positon;
</script>
<li class="sm:py-8">
	<div class="space-y-4 sm:grid sm:grid-cols-3 sm:items-start sm:gap-6 sm:space-y-0">
		<div class="aspect-w-3 aspect-h-2 sm:aspect-w-3 sm:aspect-h-4">
			<img
				class="object-cover shadow-lg rounded-lg"
				src="{image}"
				alt=""
			/>
		</div>
		<div class="sm:col-span-2">
			<div class="space-y-4">
				<div class="text-lg leading-6 font-medium space-y-1">
					<h3>{name}</h3>
					<p class="text-indigo-600">{positon}</p>
				</div>
				<div class="text-lg">
					<p class="text-gray-500">
						<slot></slot>
					</p>
				</div>
				
			</div>
		</div>
	</div>
</li>

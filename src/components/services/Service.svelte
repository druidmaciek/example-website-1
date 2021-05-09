<script>
    export let title;
    export let info;
</script>

<div class="pt-6 ">
    <div class="flow-root h-56 bg-gray-50 rounded-lg px-6 pb-8">
      <div class="-mt-6">
        <div>
          <span class="inline-flex items-center justify-center p-3 bg-indigo-500 rounded-md shadow-lg">
            <slot/>
          </span>
        </div>
        <h3 class="mt-8 text-lg font-medium text-gray-900 tracking-tight">{title}</h3>
        <p class="mt-5 text-base text-gray-500">
          {info}
        </p>
      </div>
    </div>
  </div>

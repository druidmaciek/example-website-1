<script>
	import Person from '../components/Person.svelte';
</script>

<!--
  This example requires Tailwind CSS v2.0+ 
  
  This example requires some changes to your config:
  
  ```
  // tailwind.config.js
  module.exports = {
    // ...
    plugins: [
      // ...
      require('@tailwindcss/aspect-ratio'),
    ]
  }
  ```
-->
<div class="bg-white">
	<div class="mx-auto py-12 px-4 max-w-7xl sm:px-6 lg:px-8 lg:py-24">
		<div class="space-y-12 lg:grid lg:grid-cols-3 lg:gap-8 lg:space-y-0">
			<div class="space-y-5 sm:space-y-4">
				<h2 class="text-3xl font-extrabold tracking-tight sm:text-4xl">About Us</h2>
				<p class="text-xl text-gray-500">
					Based in Cardif, we’re focused on providing modern solutions to accounting and
					bookkeeping. The way businesses operate is changing with your finance data available
					when you want it and where you want it. 
				</p>
				<p class="text-xl text-gray-500">
					Our firm combines the latest cloud-based solutions with the fundamental accountancy and
					bookkeeping services your business needs. Sense Accounting & Bookkeeping is all about
					offering flexible, affordable accounting services, tailored to your situation.
				</p>
			</div>
			<div class="lg:col-span-2">
				<ul
					class="space-y-12 sm:divide-y sm:divide-gray-200 sm:space-y-0 sm:-mt-8 lg:gap-x-8 lg:space-y-0"
				>
					<Person
						name={'Kate Thorpe'}
                        positon={'Co-Founder / CEO'}
						image={'https://images.unsplash.com/photo-1573496799515-eebbb63814f2?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1650&q=80'}
						>Kate qualified as a Chartered Accountant in 2010 with KPMG. Her focus is on improving
						business processes and effectiveness to eliminate unnecessary costs and improve
						profitability. “My passion is improving business systems. I will work with you and your
						team to come up with the ideal solution for the issues you are facing.”</Person
					>
                    <Person
						name={'Ewan Griffin'}
                        positon={'Co-Founder'}
						image={'https://images.unsplash.com/photo-1559718062-361155fad299?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=934&q=80'}
						>Ewan also qualified in 2010 whilst at KPMG.  His keen eye for detail and passion for client service ensures that he delivers outstanding results to his clients.

                        “I tailor my support to meet the needs of your business so you always receive a truly bespoke service.  Let our team ease some of the pains of running your business.”</Person
					>
				</ul>
			</div>
		</div>
	</div>
</div>

<script>
	import Header from '../components/Header.svelte';
	import Logos from '../components/Logos.svelte';
	import Services from '../components/services/List.svelte';
	import Contact from '../components/Contact.svelte';
	import Testimonial from '../components/Testimonial.svelte';
    import About from "../components/About.svelte";
    import Cta from "../components/CTA.svelte";
</script>

<svelte:head>
	<title>Insight Accountants</title>
</svelte:head>

<Header />
<Logos />
<Services />
<Testimonial
	name={'Louis Peters'}
    city={'Newport'}
	image={'https://images.unsplash.com/photo-1559548331-f9cb98001426?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1650&q=80'}
>Fantastic company. Very responsive and helpful, even at a weekend and at end of tax year. Would highly recommend them for all your tax requirements</Testimonial>
<Contact />
<Testimonial
	name={'Grace Burns'}
    city={'Cardiff'}
	image={'https://images.unsplash.com/photo-1598257006463-7c64a5a538cc?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=934&q=80'}
>Looking for an Accountant in Wales? Then you’ve come to the right place. Highly recommend Insight Accountants for its professional service. Had a great first experience, they really went above and beyond to ensure I receive the best service and provided me with some great advice!</Testimonial>
<About/>

<Cta/>
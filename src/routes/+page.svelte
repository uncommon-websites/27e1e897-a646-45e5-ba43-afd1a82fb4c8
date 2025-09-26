<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
	centered={true}
	title="Transform physical security with AI intelligence"
	subtitle="Reduce false alarms by 95% and accelerate investigations 20x with computer vision that automatically clears nuisance alerts."
	customers={[
		{
			name: "Michael Chen",
			position: "Director of Security",
			imageSrc: "/generated/image-centered-portrait-of-a-professional-male.webp"
		},
		{
			name: "Sarah Rodriguez",
			position: "Security Manager",
			imageSrc: "/generated/image-centered-portrait-of-a-professional-fema.webp"
		},
		{
			name: "James Thompson",
			position: "Enterprise Security Executive",
			imageSrc: "/generated/image-centered-portrait-of-a-confident-male-en.webp"
		},
		{
			name: "Lisa Park",
			position: "Corporate Security Director",
			imageSrc: "/generated/image-centered-portrait-of-a-professional-fema.webp"
		},
		{
			name: "Robert Williams",
			position: "Security Operations Manager",
			imageSrc: "/generated/image-centered-portrait-of-a-senior-male-secur.webp"
		}
	]}
/>
<LogoScroller 
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/adobe.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/cisco.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/servicenow.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/gap.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="Intelligent security operations"
	text="Our computer vision AI transforms physical security by automatically detecting threats, clearing false alarms, and enabling natural language investigations across enterprise infrastructure."
/>

<Testimonials
	testimonials={[
		{
			name: "Ted Richie",
			position: "Security Director",
			company: "NorCal Cannabis",
			quote:
				"AI system's superiority over human monitoring for rapid events like fence jumping is remarkable.\nWe can detect threats in 30 seconds that humans simply cannot catch.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Rod Pearson",
			position: "Security Manager",
			company: "Impossible Foods",
			quote:
				"Efficiency gains allow broader security activities beyond manual tasks.\nWe've saved thousands of hours annually while improving our security posture.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Christopher Lyman",
			position: "Security Director",
			company: "SentinelOne",
			quote:
				"Forensics capabilities and efficiency in vastly inefficient security product world.\nNatural language searches transform how we investigate incidents.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	title="Advanced security intelligence"
	subtitle="Computer vision built specifically for security operations"
	features={[
		{
			title: "Auto-clear false alarms",
			description:
				"Reduce false alarms by 95% with AI that automatically identifies and clears nuisance alerts from PACS systems, doors, and perimeter sensors."
		},
		{
			title: "Natural language search",
			description:
				"Search camera footage using plain English queries like 'Show me a person with a red shirt carrying a laptop' or 'How long has this car been here?'"
		},
		{
			title: "Real-time threat detection",
			description:
				"Monitor 100+ threat types simultaneously with 30-second fence jump detection and 10x faster threat response times across enterprise infrastructure."
		}
	]}
/>
<AboutTeaser />
<CallToAction />

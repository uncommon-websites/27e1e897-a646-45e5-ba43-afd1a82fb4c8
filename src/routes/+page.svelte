<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";

	// Icons
	import IconShieldCheck from "~icons/lucide/shield-check";
	import IconSearch from "~icons/lucide/search";
	import IconRadar from "~icons/lucide/radar";
	import IconNetwork from "~icons/lucide/network";
	import IconLock from "~icons/lucide/lock";
	import IconZap from "~icons/lucide/zap";
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
			name: "Victoria Chen-Martinez",
			position: "Chief Security Officer",
			company: "TechFlow Industries",
			quote:
				"Before Ambient.ai, our team was drowning in 200+ false alarms daily. Now we've cut that to just 10 real threats, saving us 40 hours per week and allowing us to focus on actual security strategy instead of chasing ghosts.",
			image: "/generated/image-professional-headshot-of-a-confident-fem.webp"
		},
		{
			name: "Marcus Thompson",
			position: "Director of Physical Security",
			company: "Global Manufacturing Corp",
			quote:
				"The natural language search saved us during a critical incident investigation. What used to take 8 hours of manually reviewing footage now takes 2 minutes with a simple query like 'show me anyone near building C between 2-4 AM.' That's a 240x improvement in investigation speed.",
			image: "/generated/image-professional-headshot-of-an-experienced-.webp"
		},
		{
			name: "Jennifer Wu",
			position: "Security Operations Manager",
			company: "Metropolitan Data Centers",
			quote:
				"The ROI was immediate. Ambient.ai prevented a potential $2.3M data breach by detecting an unauthorized entry attempt that our previous system missed. The AI caught the threat in 15 seconds while our human operators would have needed 8 minutes to notice.",
			image: "/generated/image-professional-headshot-of-an-asian-female.webp"
		}
	]}
/>

<Features
	title="Transform security operations with AI intelligence"
	subtitle="Purpose-built computer vision that eliminates wasted time and accelerates threat response"
	features={[
		{
			title: "Eliminate 95% of false alarms",
			description: "AI automatically identifies and clears nuisance alerts from PACS systems, freeing your team to focus on real threats instead of chasing false positives.",
			icon: IconShieldCheck
		},
		{
			title: "Natural language investigations",
			description: "Search footage in plain English with queries like 'Show me the person in red carrying a laptop' - no more manual scrubbing through hours of video.",
			icon: IconSearch
		},
		{
			title: "Real-time threat detection",
			description: "Monitor 100+ threat types simultaneously with 30-second response times that catch incidents humans miss.",
			icon: IconRadar
		},
		{
			title: "Seamless infrastructure integration",
			description: "Works with your existing cameras and access control systems - no rip-and-replace required.",
			icon: IconNetwork
		},
		{
			title: "Enterprise-grade security",
			description: "GDPR and CCPA compliant with rigorous privacy protection that meets the highest security standards.",
			icon: IconLock
		},
		{
			title: "20x faster investigations",
			description: "Transform forensic analysis from hours to minutes with AI-powered search and automated incident correlation.",
			icon: IconZap
		}
	]}
/>
<AboutTeaser />
<CallToAction />

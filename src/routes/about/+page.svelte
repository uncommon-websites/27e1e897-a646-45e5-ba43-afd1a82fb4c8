<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
		}
	];
</script>

<SecondaryHero
	title="Smarter security starts here"
	subtitle="AI that sees what matters"
	imageSrc="/generated/image-a-group-of-diverse-professionals-in-busi.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Security directors know the frustration all too well. You install hundreds of cameras to protect your facilities, only to spend 95% of your time chasing false alarms—shadows moving at night, wind-blown leaves, routine maintenance triggering alerts. Meanwhile, real threats slip by unnoticed in the noise. This broken reality, where critical security infrastructure becomes a source of inefficiency rather than protection, is exactly what drove us to build Ambient.ai in 2017.",
		"We didn't set out to build another security camera company. Instead, we focused on solving the fundamental problem: teaching computers to see and understand security events like human operators do, but faster and more accurately. Our team spent years developing computer vision intelligence specifically designed for physical security operations, creating a system that could distinguish between genuine threats and nuisance alerts. From Fortune 500 campuses to critical infrastructure, we refined our approach through real-world deployments, always with one goal—eliminate the noise and amplify what matters.",
		"Today, our customers experience what seemed impossible just a few years ago. Security teams at Adobe, TikTok, Cisco, and dozens of other enterprises have reduced false alarms by 95% while accelerating investigations by 20x. Instead of drowning in alerts, operators can focus on preventing incidents and protecting what matters most. We're not just transforming how security works—we're building the foundation for a world where intelligent systems enhance human judgment, turning security from a reactive burden into a proactive advantage."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} generating />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	generating
	stakeholderType="team"
	title="Our team."
	subtitle="Your partners in innovation."
	stakeholders={[
		{
			name: "Alex Morgan",
			position: "Founder & CEO",
			bio: "Started the company with a vision to transform the industry through innovative solutions.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Jamie Chen",
			position: "Chief Design Officer",
			bio: "Award-winning designer with a passion for creating intuitive and beautiful experiences.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Taylor Wright",
			position: "Head of Engineering",
			bio: "Technology enthusiast focused on building scalable systems that make a difference.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<StakeholderGrid
	generating
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Point Nine, TSIC and others"
	stakeholders={[
		{
			name: "Point Nine Capital",
			image: "https://cdn.brandfetch.io/pointnine.com/w/400/h/400/logo?c=1id_elLz2Bd5Ej-dWo7"
		},
		{
			name: "TSIC Ventures",
			image: "https://cdn.brandfetch.io/tiny.vc/w/400/h/400/logo?c=1a2b3c4d5e"
		},
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	generating
	title="Ready to collaborate?"
	subtitle="Let's create something amazing"
	description="Join the companies already leveraging our expertise to transform their digital presence and achieve their business goals."
/>

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
			description: "Pushing the boundaries of computer vision AI to solve the security industry's biggest challenges with breakthrough technology."
		},
		{
			title: "Precision",
			description: "Delivering 95% false alarm reduction through meticulous AI training and rigorous enterprise-grade quality standards."
		},
		{
			title: "Trust",
			description: "Building secure, privacy-compliant solutions that Fortune 500 security directors rely on to protect what matters most."
		},
		{
			title: "Excellence",
			description: "From Y Combinator recognition to Forbes Cloud 100, we earn industry leadership through relentless pursuit of perfection."
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
<Culture {values} />

<StakeholderGrid
	stakeholderType="investor"
	title="Backed by the best."
	subtitle="Recognized by leading accelerators and industry experts"
	stakeholders={[
		{
			name: "Y Combinator",
			image: "https://logo.clearbit.com/ycombinator.com"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to eliminate false alarms?"
	subtitle="See Ambient.ai in action"
	description="Join security directors at Adobe, TikTok, Cisco, and Gap who've reduced false alarms by 95% and accelerated investigations by 20x. Schedule a live threat detection demonstration at your facility."
	imageSrc="/generated/image-a-professional-security-director-in-busi.webp"
/>

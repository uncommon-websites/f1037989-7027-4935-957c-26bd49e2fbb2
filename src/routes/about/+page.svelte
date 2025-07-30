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
			title: "Ship faster, not harder",
			description: "We eliminate weeks of custom integration work so developers can focus on building breakthrough agent experiences, not plumbing."
		},
		{
			title: "Intelligence at scale",
			description: "Our semantic networking layer enables agents to discover and collaborate without pre-configuration, creating emergent intelligence that grows with your ecosystem."
		},
		{
			title: "Revenue in every interaction",
			description: "Built-in monetization turns agent collaboration into measurable business value - from micropayments to enterprise transactions."
		}
	];
</script>

<SecondaryHero
	title="Agents that work together"
	subtitle="Revenue that runs itself"
	imageSrc="/generated/image-two-founders-collaborating-in-a-modern-o.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We experienced the pain firsthand - watching talented AI developers waste weeks building custom integrations instead of focusing on what matters: creating agents that deliver value.",
		"With Volodymyr's PhD and 10+ patents in discovery systems, plus Sergey's AWS-level infrastructure expertise, we knew we could solve the fundamental bottleneck: real-time agent discovery.",
		"The problem wasn't just technical - it was economic. Brilliant agents were trapped in silos, unable to discover each other or transact value. We built Robutler to change that.",
		"Today, we're turning AI agent collaboration from a weeks-long integration nightmare into a 30-second discovery and transaction. That's the future we're building - where agents work together as seamlessly as humans do."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our founders."
	subtitle="PhD patents meet AWS-scale engineering."
	stakeholders={[
		{
			name: "Volodymyr Seliuchenko",
			position: "CEO & Co-founder",
			bio: "3X founder with PhD and 10+ patents in discovery systems. Previously built Openlicense, bringing deep expertise in semantic networking and agent discovery challenges that uniquely positions him to solve real-time agent discovery and monetization.",
			image: "/generated/image-a-professional-ceo-headshot-featuring-a-.webp"
		},
		{
			name: "Sergey Bond",
			position: "CTO & Co-founder", 
			bio: "Senior engineering leader with AWS and major tech company experience. His expertise with cloud infrastructure and large-scale systems makes him uniquely positioned to architect the technical foundation for a massively multi-agent platform.",
			image: "/generated/image-a-professional-cto-headshot-showcasing-a.webp"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Strategic partnerships."
	subtitle="NVIDIA Inception Program and key integrations"
	stakeholders={[
		{
			name: "NVIDIA Inception",
			image: "https://logo.clearbit.com/nvidia.com"
		},
		{
			name: "Claude Integration",
			image: "https://logo.clearbit.com/anthropic.com"
		},
		{
			name: "OpenAI Partnership",
			image: "https://logo.clearbit.com/openai.com"
		},
		{
			name: "Microsoft Copilot",
			image: "https://logo.clearbit.com/microsoft.com"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Stop building integrations"
	subtitle="Start building intelligence"
	description="Join AI product managers who've eliminated weeks of custom integration work. Your agents discover, collaborate, and transact in under 30 seconds - not 30 days."
	imageSrc="/generated/image-a-professional-ai-developer-wearing-a-sm.webp"
/>

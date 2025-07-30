<!--
@component AboutTeaser
A minimalist teaser for the about page.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Volodymyr Seliuchenko",
		role: "Founder & CEO",
		image: "/generated/image-a-professional-headshot-of-a-confident-t.webp"
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-2xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"After building my third company and earning 10+ patents, I realized the biggest bottleneck in AI wasn't the agents themselves—it was getting them to find and work with each other. That's why we built Robutler: to turn what takes weeks into seconds."`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="flex flex-col items-center gap-6">
				<div class="flex items-center gap-4">
					<img
						src={teamMember.image}
						alt={teamMember.name}
						class="size-16 rounded-full object-cover shadow-md"
					/>
					<div class="text-left">
						<div class="text-callout font-semibold">{teamMember.name}</div>
						<div class="text-caption text-emphasis-low">{teamMember.role}</div>
						<div class="text-caption2 text-emphasis-low mt-1">3X Founder • PhD • 10+ Patents</div>
					</div>
				</div>
				<div class="flex items-center gap-4">
					<Button href="/about" variant="primary" size="sm">Learn our story</Button>
					<Button href="/contact" variant="secondary" size="sm">Meet the team</Button>
				</div>
			</div>
		</div>
	</div>
</section>

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
			title: "Speed to insight",
			description: "We eliminate the slow feedback cycles that hold product teams back, delivering actionable insights in hours, not weeks."
		},
		{
			title: "Data-driven clarity",
			description: "Every feature decision should be backed by real user data, not assumptions or opinions."
		},
		{
			title: "Customer obsession",
			description: "Product-market fit happens when you truly understand your users. We help you get closer to your customers than ever before."
		}
	];
</script>

<SecondaryHero
	title="Build products users actually want"
	subtitle="Faster insights, smarter decisions"
	imageSrc="/generated/image-a-diverse-group-of-people-gathered-aroun.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We started in 2018 with a simple goal: make helpful tech that people actually need. While many chase profits, we chose to do things differently.",
		"Beyond making good products, we care about doing the right thing, being kind to our planet, and making sure everyone can use what we build. That's our compass.",
		"From day one, we've asked ourselves: 'Does this actually help people?' This question gets us through tough calls and shapes who we are. We're playing the long game here.",
		"We think about how our work affects real people's lives. We build tech that brings people together, keeps your information safe, and treats everyone fairly. When we stick to these basics, good things happen."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- CTA Section -->
<CallToAction
	title="Stop guessing, start knowing"
	subtitle="Validate product-market fit faster"
	description="Join product managers at leading SaaS startups who've accelerated their path to PMF with 4ow1. Get the user insights you need to make confident feature decisions."
	imageSrc="/generated/image-a-professional-product-manager-sits-at-a.webp"
/>

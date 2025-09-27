<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
	
	// Icons for features
	import IconMessageSquare from "~icons/lucide/message-square";
	import IconTrendingUp from "~icons/lucide/trending-up";
	import IconTarget from "~icons/lucide/target";
	import IconGitBranch from "~icons/lucide/git-branch";
	import IconEye from "~icons/lucide/eye";
	import IconRadar from "~icons/lucide/radar";
</script>

<Hero
	title="Validate faster. Build what matters."
	subtitle="Close the feedback loop. Prioritize with confidence."
	imageSrc="/generated/image-a-cheerful-product-manager-in-their-late.webp"
	centered={false}
/>
<LogoScroller 
	label="Trusted by product teams at leading SaaS companies"
	logoUrls={[
		'https://cdn.brandfetch.io/slack.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/stripe.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/notion.so/w/400/h/400/logo',
		'https://cdn.brandfetch.io/linear.app/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	testimonials={[
		{
			name: "Maya Chen",
			position: "Head of Product",
			company: "VelocityTech",
			quote:
				"4ow1 cut our feature validation cycle from 6 weeks to 2 weeks. We saved $180k in development costs by killing bad ideas early and doubling down on features that actually moved the needle.",
			image: "/generated/image-professional-headshot-of-a-confident-asi.webp"
		},
		{
			name: "Marcus Williams",
			position: "VP Product",
			company: "ScaleForward",
			quote:
				"Before 4ow1, we were flying blind on product-market fit. Now we validate assumptions in days, not months. This prevented a costly $2M pivot and helped us reach Series A 8 months ahead of schedule.",
			image: "/generated/image-professional-headshot-of-a-confident-bla.webp"
		},
		{
			name: "Isabella Rodriguez",
			position: "Senior Product Manager",
			company: "GrowthLab",
			quote:
				"4ow1 eliminated the guesswork in feature prioritization. We increased user retention by 43% in just one quarter by focusing on validated user needs instead of internal assumptions.",
			image: "/generated/image-professional-headshot-of-a-confident-his.webp"
		}
	]}
/>

<Features
	title="Validate faster. Build what matters."
	subtitle="Stop guessing what users want. Get clear signals on what to build next with real-time feedback and data-driven prioritization."
	features={[
		{
			title: "Instant feedback loops",
			description: "Embed lightweight surveys and micro-feedback tools directly in your product without any coding or delays.",
			icon: IconMessageSquare
		},
		{
			title: "Data-driven prioritization",
			description: "AI-powered insights help you spot patterns, track demand, and rank feature requests in one clean dashboard.",
			icon: IconTrendingUp
		},
		{
			title: "Pre-build validation",
			description: "Test concepts and workflows before handing off to engineering, saving weeks of development time.",
			icon: IconTarget
		},
		{
			title: "Development workflow integration",
			description: "Connect feedback directly to your existing tools and processes for seamless product development cycles.",
			icon: IconGitBranch
		},
		{
			title: "Real-time behavior insights",
			description: "Track how users actually interact with your features to understand what drives engagement and retention.",
			icon: IconEye
		},
		{
			title: "Competitive positioning intelligence",
			description: "Monitor market trends and competitor movements to position your features strategically in the market.",
			icon: IconRadar
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />

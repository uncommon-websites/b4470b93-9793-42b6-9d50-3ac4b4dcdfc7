<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
	testimonials={[
  {
    name: "Renata Kim",
    position: "Head of operations",
    company: "Luno Logistics",
    quote:
      "It pays for itself fast. Within two months, we cut onboarding time by 30% and avoided a full-time hire.",
    image:
      "/generated/image-a-professional-headshot-of-an-east-asian.webp"
  },
  {
    name: "Yusuf Dahab",
    position: "Senior product manager",
    company: "Corebrite",
    quote:
      "We saw a 4x return on our subscription cost just from finishing projects sooner and reducing scope creep.",
    image:
      "/generated/image-a-professional-headshot-of-a-middle-east.webp"
  },
  {
    name: "Maeve Connolly",
    position: "Finance systems lead",
    company: "Branchline Insights",
    quote:
      "Our team was up and running in a day. No multi-week setup, no endless training. Just clear value out of the box.",
    image:
      "/generated/image-a-professional-headshot-of-an-irish-woma.webp"
  }
]}
/>

<CallToAction
  title="Get started for free"
  subtitle="Make smarter decisions, faster."
  description="See how easy it is to save time, cut costs, and make better decisions—without adding extra complexity."
  imageSrc="/generated/image-a-happy-customer-enjoying-a-product-in-a.webp"
  callsToAction={[
    { href: '/signup', label: 'Start free', variant: 'primary' },
    { href: '/contact', label: 'Contact sales', variant: 'secondary' }
  ]}
/>

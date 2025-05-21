<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
		{
			title: "Flexible Work",
			description: "Remote-first with flexible hours that respect work-life balance.",
			icon: IconBriefcase
		},
		{
			title: "Growth Opportunities",
			description: "Continuous learning with mentorship and education stipends.",
			icon: IconUsers
		},
		{
			title: "Comprehensive Benefits",
			description: "Health coverage, retirement plans, and generous paid time off.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior Frontend Developer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Backend Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Design Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "UX/UI Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Analyst",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Marketing
		{
			title: "Marketing Specialist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Strategist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Social Media Manager",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
  {
    name: "Michael Chen",
    position: "Senior developer",
    company: "engineering team",
    quote:
      "I'm constantly impressed by the culture we've built. As a senior developer, I’ve seen firsthand how open people are to sharing ideas and lending a hand. Whether I'm pairing on a tough bug or brainstorming with design, I’ve always felt supported and heard.",
    image:
      "/generated/image-a-senior-asian-male-developer-smiling-wa.webp"
  },
  {
    name: "Priya Sharma",
    position: "Product designer",
    company: "design team",
    quote:
      "The learning curve has been steep—but that’s what I wanted. I've had the chance to shadow senior designers, lead user research sessions, and even attend an external design sprint. The company really invests in your growth if you show up hungry to learn.",
    image:
      "/generated/image-a-south-asian-female-product-designer-wo.webp"
  },
  {
    name: "Marcus Johnson",
    position: "Marketing lead",
    company: "marketing team",
    quote:
      "This role has stretched me in ways I didn’t expect. I came in with a background in content and now lead integrated marketing campaigns. The feedback loops are fast, the ownership is real, and the people truly want you to grow.",
    image:
      "/generated/image-a-black-male-marketing-lead-engaged-in-a.webp"
  }
];

	const processSteps = [
  {
    step: 1,
    title: "Apply",
    description: "Submit your resume or LinkedIn URL—no lengthy cover letter required."
  },
  {
    step: 2,
    title: "Meet the team",
    description: "If there's a fit, you'll meet with a few folks across functions for short 30-minute conversations."
  },
  {
    step: 3,
    title: "Work sample",
    description: "You’ll complete a short take-home assignment to showcase how you approach real-world work."
  },
  {
    step: 4,
    title: "Final chat",
    description: "We’ll wrap with a final conversation to calibrate expectations, answer questions, and make sure we’re aligned."
  }
];

	const values = [
		{
			icon: IconHeart,
			title: "Passion",
			description: "We're driven by a shared passion for innovation and excellence."
		},
		{
			icon: IconUsers,
			title: "Collaboration",
			description: "We believe in teamwork and collaboration to achieve great things."
		},
		{
			icon: IconGlobe,
			title: "Global Impact",
			description: "We're committed to making a positive impact on the world."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Create with heart. Grow with purpose."
	subtitle="A place to thrive, feel supported, and make real impact—together."
	imageSrc="/generated/image-a-group-of-diverse-happy-employees-colla.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Work that actually matters. Grow fast, together." />

<div class="mt-16 space-y-6">
  <p class="text-body">
    We're solving real problems for real customers. Your work won't sit on a shelfit'll go live and make a measurable impact.
  </p>
  <p class="text-body">
    We invest deeply in your development: learning budgets, mentorship, and a team built to challenge and support each other.
  </p>
  <p class="text-body">
    We're remote-friendly with flexible hours. We trust you to do your best work, your way.
  </p>
  <p class="text-body">
    Were building a sustainable business with clear values, healthy compensation, and benefits that let you focus on doing great work.
  </p>
</div>
<div class="mt-12 grid gap-4 md:grid-cols-3">
	{#each benefits as benefit}
		<Card {...benefit} />
	{/each}
</div>
</section>

<!-- Culture Section -->
<Culture values={[
  {
    icon: IconHeart,
    title: 'Bias for action',
    description: 'We move quickly and prioritize progress over perfectiondone is better than perfect.'
  },
  {
    icon: IconUsers,
    title: 'Low ego, high output',
    description: 'We work hard to separate ideas from identity. The best idea wins, no matter where it comes from.'
  },
  {
    icon: IconGlobe,
    title: 'Default to transparency',
    description: 'From strategy to feedback, we believe good decisions come from shared contextnot closed rooms.'
  }
]} />

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<div class="mx-auto">
		<h2 class="text-title1 mb-16">Our application process</h2>

		<div class="grid gap-12 md:grid-cols-3">
			{#each processSteps as { step, title, description }, i}
				<div class="flex flex-col">
					<div class="{ICON_CONTAINER_CLASSES} mb-6 size-11">
						<span class="text-headline">{step}</span>
					</div>
					<h3 class="text-headline mb-3">{title}</h3>
					<p class="text-body text-emphasis-low">{description}</p>
				</div>
			{/each}
		</div>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>

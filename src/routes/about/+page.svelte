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
    title: "Teamwork",
    description: "We believe people do their best work when they feel heard, supported, and challenged to grow. Our culture is built on respect, open collaboration, and constant curiosity. We listen first, move as a team, and treat each other with kindness. Every voice counts. Every idea is worth considering. Together, we strive to create work that makes a meaningful difference."
  }
];
</script>

<SecondaryHero
  title="Progress starts with the team"
  subtitle="We create bold software that fuels real-world impact"
  imageSrc="/generated/image-a-group-of-professionals-in-a-modern-off.webp"
/>

<!-- Story Section -->
<Story
  paragraphs={[
    "We started with a question: why is working in spreadsheets still so frustrating? Between the constant exporting, broken formulas, and confusing versions, what used to be a tool for flexibility had become a daily struggle. We had spent years trying to get answers from spreadsheets that were always a step behind—and we believed there had to be a better way.",
    "So we built one. From day one, our goal has been simple: create a spreadsheet that actually fits the way modern teams work. One that connects live to your data, works the way you already think, and clears up the confusion that comes with outdated tools. It’s made for people who prefer clarity over complexity, and speed over setup.",
    "Today, companies use our spreadsheet to stay on the same page without chasing offline files or emailing screenshots. Whether it's product, finance, or operations, teams are moving faster together—with the right numbers in front of them, and fewer hoops in the way. It’s the way spreadsheets should have always worked, and we’re just getting started."
  ]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
  stakeholderType="team"
  title="Our team."
  subtitle="Your partners in innovation."
  stakeholders={[
    {
      name: "Alex Morgan",
      position: "Founder & CEO",
      bio: "Started the company with a vision to transform the industry through innovative solutions.",
      image: "/generated/image-a-headshot-of-a-confident-entrepreneur-w.webp"
    },
    {
      name: "Jamie Chen",
      position: "Chief Design Officer",
      bio: "Award-winning designer with a passion for creating intuitive and beautiful experiences.",
      image: "/generated/image-a-portrait-of-a-creative-asian-designer-.webp"
    },
    {
      name: "Taylor Wright",
      position: "Head of Engineering",
      bio: "Technology enthusiast focused on building scalable systems that make a difference.",
      image: "/generated/image-a-headshot-of-an-african-american-engine.webp"
    }
  ]}
/>

<StakeholderGrid
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
  title="Let's connect."
  subtitle="We're excited to hear from you."
  description="We love meeting new people and sharing what we're building. If you're curious, have ideas, or just want to connect, we’d love to hear from you. Everyone's welcome."
  imageSrc="/generated/image-a-friendly-and-diverse-team-gathered-in-.webp"
  callsToAction={[{ href: '/contact', label: 'Say hello', variant: 'primary' }]}
/>

<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
  centered={true}
  title="Work that moves as fast as you do."
  subtitle="A beautifully designed platform that automates busywork so teams can focus on what matters."
  imageSrc="/generated/image-a-diverse-group-of-business-professional.webp"
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://logo.clearbit.com/unitedhealthgroup.com',
		'https://logo.clearbit.com/google.com',
		'https://logo.clearbit.com/coursera.org'
	]}
/>

<Summary
	title="What we do"
	text="We help small and mid-sized businesses handle finances, payroll, and compliance in one simple platform. Clear costs, easy setup, and no extra hires needed."
/>

<Testimonials
	testimonials={[
		{
			name: "Maria Delgado",
			position: "Owner",
			company: "Sunhouse Bakery",
			quote: "Before we started using it, I was icing cakes until midnight most nights. Now, I’m home for dinner with my family—and still getting more done. It’s saved me hours every week.",
			image: "/generated/image-a-hispanic-woman-the-bakery-owner-is-sta.webp"
		},
		{
			name: "Faisal Khan",
			position: "CTO",
			company: "Helix Systems",
			quote: "Using this platform cut our project risk in half. We’ve avoided costly last-minute bugs and surprise delays that used to derail our timelines. Now launches run smoother, and my engineering team finally has peace of mind to focus on building.",
			image: "/generated/image-a-south-asian-man-the-cto-is-sitting-wit.webp"
		},
		{
			name: "Curtis Rivers",
			position: "Logistics Manager",
			company: "Rapid Route Distribution",
			quote: "We’re no longer burning through our transport budget—monthly costs are finally predictable. It’s like we found extra room in our margin with zero extra effort.",
			image: "/generated/image-an-african-american-man-the-logistics-ma.webp"
		}
	]}
/>

<Features
	title="Features"
	subtitle="Productivity, reimagined for high-velocity teams"
	features={[
		{
			title: "Automate the busywork",
			description: "Set rules once and let the platform handle recurring tasks, reminders, and approvals—so your team can focus on work that matters."
		},
		{
			title: "Insights in real time",
			description: "AI-powered dashboards track projects, blockers, and trends automatically—no manual updates needed."
		},
		{
			title: "Collaboration without compromise",
			description: "Control who sees what with role-based access and encrypted file sharing built to keep sensitive work confidential and secure."
		},
		{
			title: "Customize everything",
			description: "Every view, workflow, and dashboard adapts to how your team actually works—no coding required."
		},
		{
			title: "Help, right when you need it",
			description: "Live chat and hands-on onboarding ensure your team is never stuck and always supported."
		},
		{
			title: "Built to scale with you",
			description: "From 5 to 5,000 users, enjoy lightning-fast performance and uptime that keeps up with your growth."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Get payroll off your plate",
			description:
				"Handle paydays, tax filings, and year-end forms without stress. Our platform automates every step so owners never miss a deadline again.",
			image: "/generated/image-small-business-owner-using-computer-payroll.webp",
			link: {
				href: "/use-cases/payroll-automation",
				label: "Learn more"
			}
		},
		{
			title: "One dashboard for every dollar",
			description:
				"See all expenses, invoices, and budget trends in one place. Make smarter decisions on the fly without chasing down paperwork.",
			image: "/generated/image-finance-manager-reviewing-dashboard-budget.webp",
			link: {
				href: "/use-cases/financial-visibility",
				label: "See the insights"
			}
		},
		{
			title: "Stay compliant, stay carefree",
			description:
				"Local rules keep changing, but you’ll never worry about falling behind. Compliance is built-in—so audits don’t keep you up at night.",
			image: "/generated/image-compliance-officer-checking-documents-smart.webp",
			link: {
				href: "/use-cases/automatic-compliance",
				label: "See how it works"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction
  title="Make your workday simpler"
  subtitle="Switching is easy—and help is always here."
  description="Automate payroll, compliance, and HR tasks—so you spend less time on admin and more on running your business. Switching is seamless, and our team is here to help every step of the way. Thousands of busy leaders already made the move."
  imageSrc="/generated/image-a-cheerful-small-business-owner-standing.webp"
  callsToAction={[
    { href: '/get-started', label: 'Start free trial', variant: 'primary' },
    { href: '/contact', label: 'Talk to a product expert', variant: 'secondary' }
  ]}
/>

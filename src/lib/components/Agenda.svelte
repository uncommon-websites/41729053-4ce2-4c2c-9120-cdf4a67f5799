<script lang="ts">
  import AgendaItem from './AgendaItem.svelte';

  const step1 = {
    date: "Week 1",
    tags: ["Onboarding"],
    items: [
      { time: "Day 1", title: "Download Shiawase and create your profile" },
      { time: "Day 2-3", title: "Video call with Mira AI", subtitle: "Natural conversation to understand your personality" },
      { time: "Day 4-7", content: ["AI creates your personality fingerprint", "System analyzes compatibility patterns", "Your profile goes live to compatible matches"] }
    ]
  };

  const step2 = {
    date: "Week 2-3",
    tags: ["First Connections"],
    items: [
      { time: "Week 2", content: ["Receive your first curated introductions", "See compatibility summaries and profiles", "Start conversations with matched people", "Provide feedback to refine matching"] },
      { time: "Week 3", content: ["Get invited to your first micro-experience", "Meet 4-6 highly compatible people", "Attend intimate gathering (dinner, happy hour, etc.)", "Build your social circle organically"] }
    ]
  };

  const step3 = {
    date: "Ongoing",
    tags: ["Growing Community"],
    items: [
      { time: "Monthly", content: ["Regular curated introductions", "Invitations to compatible micro-experiences", "Host your own gatherings", "AI learns and improves matching accuracy"] },
      { time: "Long-term", title: "Build lasting friendships and find your community" }
    ]
  };
</script>

<section class="px-6 max-w-[1400px] mx-auto">
  <AgendaItem {...step1} isFirst={true} />
  <AgendaItem {...step2} isFirst={false} />
  <AgendaItem {...step3} isFirst={false} />
</section>

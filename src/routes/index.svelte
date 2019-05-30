<script context="module">
  export async function preload({ params }) {
    const res = await this.fetch('https://randomuser.me/api/?results=4');
    const users = await res.json();

    return {
      users: users.results
    };
  }
</script>

<script>
  import ProfileCard from '../components/ProfileCard.svelte';

  export let users;
</script>

<svelte:head>
  <title>Sapper + TailwindCSS Starter</title>
</svelte:head>

{#each users as user}
  <ProfileCard user='{user}' />
{/each}
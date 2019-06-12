<script>
  import { stores } from '@sapper/app';

  const { preloading } = stores();

  console.log('Preloading', preloading);

  export let segment;
</script>

<slot />

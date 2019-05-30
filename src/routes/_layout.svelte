<script>
	import { stores } from "@sapper/app"

	const { preloading } = stores()

	export let segment
</script>

<slot />

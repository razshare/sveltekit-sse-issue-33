<script>
  import { enhance } from '$app/forms';
  export let data;
  const quote = data?.quote;
</script>

<h3>A Loaded Cat Quote</h3>
<span>{$quote?.value ?? ''}</span><br />

<form use:enhance method="post">
  <button>Force reconnect</button>
</form>

<template>
  <div>
    <h2>
	    <a {id} href="#" class="anchor" aria-hidden="true"></a>
	    <span>Programma</span>
    </h2>
  </div>
</template>

<script setup>
</script>

<style>
  h2 {
		font-weight: bold;
		letter-spacing: -0.04em;
		margin: 0;
		font-weight: 600;
	}

	h2 a.anchor {
		display: none;
		position: absolute;
		margin-left: -0.6em;
	}

	h2:hover a.anchor { display: none; }

	h2 > strong {
		display: block;
		white-space: nowrap;
	}
</style>
<script lang="ts">
	import { onMount } from 'svelte';

	let fullName = '';
	let email = '';
	let message = '';

	const handleSubmit = (event: SubmitEvent) => {
		event.preventDefault();
		console.log(fullName, email, message);
	};

	onMount(() => {
		document.title = 'Contato';
	});
</script>

<form on:submit={handleSubmit}>
	<label for="fullName">Nome:</label>
	<input type="text" id="fullName" name="fullName" bind:value={fullName} />

	<label for="email">E-mail:</label>
	<input type="email" id="email" name="email" bind:value={email} />

	<label for="message">Mensagem:</label>
	<textarea id="message" name="message" bind:value={message} />

	<button type="submit">Enviar</button>
</form>

{#if fullName !== ''}
	<ul>
		<li>{fullName}</li>
		<li>{email}</li>
		<li>{message}</li>
	</ul>
{/if}
{#if 1 + 1 === 2}
	acerto!
{/if}

<style>
	input,
	textarea {
		display: block;
		margin-bottom: 1.5rem;
		padding: 0.75rem;
		border: 1px solid #ccc;
		border-radius: 0.25rem;
		width: 100%;
	}

	button[type='submit'] {
		background-color: #007bff;
		color: #fff;
		padding: 0.75rem 1.5rem;
		border: none;
		border-radius: 0.25rem;
		cursor: pointer;
	}
	ul {
		list-style: none;
		padding-left: 0;
	}

	li {
		margin-bottom: 0.5rem;
	}
</style>

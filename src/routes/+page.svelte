<script>
	let info = {
		name: 'Sudarat Chattanon',
		nname: 'Gatuk',
		title: 'Engineering Director',
		company: 'PRODIGY9',
		email: 'sudarat@prodigy9.co',
		phone: '(66)61-387-8484'
	};
</script>

<main class="bg">
	<div class="circles" />

	<div class="card">
		<div cass="main-info">
			<div class="name">{info.name.toUpperCase()} ({info.nname.toUpperCase()})</div>
			<div class="title">{info.title.toUpperCase()}</div>
			<div class="company"><i class="fa-regular fa-building" /> @ {info.company}</div>
		</div>

		<div class="contact">
			<div>Email: {info.email}</div>
			<div>Phone: {info.phone}</div>
		</div>
	</div>
</main>

<style>
	.card {
		display: flex;
		flex-direction: column;
		justify-content: space-between;
		width: 30rem;
		height: 15rem;
		margin: 25vh auto;
		padding: 2rem;
		border: 1px solid plum;
		border-radius: 1rem;
		font-family: 'Bai Jamjuree', sans-serif;
		background-color: #e3e5e8;
	}

	.name {
		font-size: 2rem;
		font-weight: bold;
	}

	.title {
		font-size: 1.5rem;
	}

	.company {
		font-size: 1.5rem;
	}
	.bg {
		position: relative;
		width: 100%;
		height: 100vh;
		margin: auto;
		overflow: hidden;
		background: linear-gradient(
			-70deg,
			#e3e5e8 0%,
			#ebe4e3 10%,
			#e4e1e0 25%,
			#e5cee9 45%,
			#e1b2db 60%,
			#e5a2d4 75%,
			#e282bb 85%,
			#e8398e 100%
		);
	}

	.bg::before,
	.bg::after,
	.bg > .circles,
	.bg > .circles::before,
	.bg > .circles::after {
		filter: blur(75px);
	}

	.bg::before,
	.bg::after {
		position: absolute;
		content: '';
		width: 390px;
		height: 390px;
		border-radius: 100%;
	}

	.bg::before {
		background: #c580a0;
		top: -195px;
		left: -195px;
	}

	.bg::after {
		background: #86e1ef;
		right: -195px;
		top: 50%;
		transform: translateY(-50%);
	}

	.bg > .circles,
	.bg > .circles::before,
	.bg > .circles::after {
		border-radius: 100%;
		position: absolute;
	}

	.bg > .circles::before,
	.bg > .circles::after {
		content: '';
		width: 100%;
		height: 100%;
		top: 50%;
		transform: translateY(-50%);
	}

	.bg > .circles {
		width: 230px;
		height: 230px;
		background: #bfe9fa;
		bottom: -60px;
		left: 75px;
	}

	.bg > .circles::before {
		background: #b88cde;
		left: -40%;
	}

	.bg > .circles::after {
		background: #ba427c;
		right: -20%;
	}
</style>

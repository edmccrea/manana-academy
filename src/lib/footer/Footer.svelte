<footer>
	<div class="footer-grid">
		<div class="logo">
			<!-- <img src="%sveltekit.assets%/manana_logo.png" alt="manana logo" /> -->
		</div>
		<div class="opening-times">
			<h2>Opening Times</h2>
			<p>Monday <span>17:30-19:00</span></p>
			<p>Tuesday <span>18:00-20:00</span></p>
			<p>Wednesday <span>17:30-19:00</span></p>
			<p>Thursday <span>18:00-20:00</span></p>
			<p>Friday <span>Closed</span></p>
			<p>Saturday <span>12:30-13:30</span></p>
			<p>Sunday <span>12:00-14:00</span></p>
		</div>
		<div class="contact">
			<h2>Contact</h2>
		</div>
	</div>

	<div class="footer-bottom">
		<p>Mañana Academy Ystad 2022&copy;</p>
		<div class="socials">
			<p>facebook</p>
			<p>insta</p>
		</div>
	</div>
</footer>

<style>
	footer {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		padding-top: 1rem;
	}

	.footer-grid {
		display: grid;
		grid-template-columns: repeat(3, 1fr);
		width: 100%;
		text-align: center;
	}

	.footer-bottom {
		width: 100%;
		display: flex;
		justify-content: space-between;
	}

	.socials {
		display: flex;
	}

	@media (min-width: 480px) {
		footer {
			padding: 40px 0;
		}
	}
</style>

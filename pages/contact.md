---
 layout: default
 title: Contact
 permalink: /contact/
 weight: 5
---
<html lang="en">
<head>
	<meta charset="UTF-8">
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Contact the team!</title>
	<style>
	* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;

	font-family: 'Fira Sans', sans-serif;
}

.section-contact {
	min-height: 100vh;
	padding-top: 100px;
	padding-bottom: 100px;
	background-image: linear-gradient(175deg, #EEE 50%, #FF9FDB 50%, #9B75D7);

	.container {
		max-width: 1280px;
		margin: 0 auto;
		padding-left: 32px;
		padding-right: 32px;

		@media (min-width: 768px) {
			padding-left: 64px;
			padding-right: 64px;
		}

		@media (min-width: 1024px) {
			padding-left: 128px;
			padding-right: 128px;
		}

		h1 {
			color: #666;
			font-size: 36px;
			text-transform: uppercase;
			text-align: center;
			margin-bottom: 16px;
		}

		p {
			color: #888;
			font-size: 18px;
			line-height: 1.5;
			margin-bottom: 32px;
		}

		form {
			display: grid;
			grid-template-columns: 1fr;
			grid-gap: 16px;
			background-color: #FFF;
			padding: 32px;
			border-radius: 16px;
			box-shadow: 0px 6px 12px rgba(0, 0, 0, 0.2);

			@media (min-width: 768px) {
				grid-template-columns: repeat(2, 1fr);
			}

			.form-group {

				&.full {
					grid-column: 1 / -1;
				}

				label {
					display: block;
					margin-bottom: 5px;
					color: #888;
					font-size: 14px;
				}

				.form-element {
					appearance: none;
					outline: none;
					border: none;

					display: block;
					width: 100%;

					border-radius: 8px;
					padding: 12px 16px;
					background-color: #F3F3F3;
					transition: 0.4s;

					&:focus {
						box-shadow: 0px 0px 6px rgba(0, 0, 0, 0.2);
						background-color: #FFF;
					}
				}

				textarea {
					resize: none;
					min-height: 100px;
				}
			}

			.submit-group {
				grid-column: 1 / -1;
				text-align: right;

				input[type="submit"] {
					appearance: none;
					border: none;
					outline: none;
					background: none;

					padding: 12px 16px;
					background-color: #FF9FDB;
					border-radius: 8px;
					color: #FFF;
					cursor: pointer;
					transition: 0.4s;

					&:hover {
						background-color: #9B75D7;
					}
				}
			}
		}
	}
}
</style>
</head>
<body>
	<main>
		<section class="section-contact">
			<div class="container">
				<h1>Contact the team!</h1>
				<p>Fill out the form below to get in touch with one of our team members. We will try to get back to you within 48 hours. If we do not reply within that time please feel free to use the form again.</p>

				<form>
					<div class="form-group">
						<label for="firstname">First name*</label>
						<input 
							type="text" 
							name="firstname" 
							id="firstname" 
							required 
							class="form-element"
							placeholder="John" />
					</div>
					<div class="form-group">
						<label for="lastname">Last name*</label>
						<input type="text" name="lastname" id="lastname" required class="form-element" placeholder="Doe" />
					</div>
					<div class="form-group">
						<label for="email">Email address*</label>
						<input type="email" name="email" id="email" required class="form-element" placeholder="john.doe@example.com" />
					</div>
					<div class="form-group">
						<label for="company">Company</label>
						<input type="text" name="company" id="company" class="form-element" placeholder="john.doe@example.com" />
					</div>
					<div class="form-group full">
						<label for="message">What are you looking for?</label>
						<textarea name="message" id="message" class="form-element" placeholder="I want a website please..."></textarea>
					</div>
					<div class="submit-group">
						<input type="submit" value="SEND MESSAGE" />
					</div>
				</form>
			</div>
		</section>
	</main>
</body>
</html>
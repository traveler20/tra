# CONTACT

お問い合わせはこちらからお願いします。

```html
<style>
	.c-form {
		max-width: 600px;
	}
	.c-form__item {
		display: flex;
		flex-wrap: wrap;
		justify-content: space-evenly;
		margin-bottom: 20px;
	}
	.c-form__label,
	.c-form__input {
		padding: 10px;
	}
	.c-form__label {
		width: 90%;
	}
	.c-form__input {
		width: 90%;
		font-size: 16px;
		border: solid 1px #333;
		border-radius: 4px;
	}
	.c-form__input:focus-visible {
		outline: #6997c5 auto 1px;
	}
	.c-form__required {
		color: #fff;
		background-color: #6997c5;
		border-radius: 4px;
		padding: 5px 5px;
		margin: 0 0 0 18px;
	}
	textarea.c-form__input {
		height: 160px;
	}
	.c-form__submit {
		text-align: center;
	}
	.c-form__submit button {
		font-size: 18px;
		font-weight: bold;
		color: #fff;
		background-color: #6997c5;
		border: solid 1px #6997c5;
		border-radius: 4px;
		padding: 5px 32px;
		transition: 0.4s;
		cursor: pointer;
	}
	.c-form__submit button:hover {
		color: #6997c5;
		background-color: transparent;
	}

	@media (min-width: 640px) {
		.c-form__item {
			flex-wrap: nowrap;
		}
		.c-form__label {
			width: 40%;
		}
		.c-form__input {
			width: 55%;
		}
	}
</style>
```

```html
<form
	action="https://docs.google.com/forms/u/1/d/e/1FAIpQLSe00eJN0CWayVTtmGW0ONrc6MT8bA5no3F9iHgbGwaOm18KRw/formResponse"
	method="POST"
	target="hidden_iframe"
	onsubmit="submitted=true;"
	class="c-form"
>
	<div class="c-form__item">
		<label class="c-form__label" for="field-name"
			>名前・会社名<span class="c-form__required">必須</span></label
		>
		<input
			name="entry.690315515"
			class="c-form__input"
			id="field-name"
			placeholder="株式会社 山田"
			type="text"
			required="required"
		/>
	</div>
	<div class="c-form__item">
		<label class="c-form__label" for="field-mail"
			>メールアドレス<span class="c-form__required">必須</span></label
		>
		<input
			name="entry.310605352"
			class="c-form__input"
			id="field-mail"
			placeholder="sample@gmail.com"
			type="email"
			required="required"
		/>
	</div>
	<div class="c-form__item">
		<label class="c-form__label" for="field-message">メッセージ内容</label>
		<textarea
			name="entry.1726417427"
			class="c-form__input"
			id="field-message"
			placeholder="お問い合わせ内容"
		></textarea>
	</div>
	<div class="c-form__submit">
		<button type="submit">送信する</button>
	</div>
</form>
<script type="text/javascript">
	let submitted = false;
</script>
<iframe
	name="hidden_iframe"
	id="hidden_iframe"
	style="display: none"
	onload="if(submitted){window.location='/thanks';}"
></iframe>
```

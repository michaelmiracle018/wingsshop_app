<template>
	<div class="success-message-content">
		<div class="success-message-wrap">
			<div class="icon-wrap mt-[20px]">
				<img src="/success.png" alt="check" />
			</div>
			<div class="text-wrap">
				<h5 class="text-xl ">You have successfully palced your order</h5>
			</div>
			<div class="btn-wrap">
				<button @click="handleContunuePurchase">Continue Buying</button>
			</div>
		</div>
	</div>
</template>

<script setup>

const handleContunuePurchase = () => {
    navigateTo('/')
}
	
</script>

<style scoped>
	/* ICON WRAP STYLE */
	.success-message-content {
		display: flex;
		justify-content: center;
		align-items: center;
	}

	.icon-wrap {
		display: flex;
		justify-content: center;
		align-items: center;
	}
	.icon-wrap img {
		width: 100%;
		height: 100%;
		object-fit: cover;
		max-width: 200px;
		max-height: 200px;
	}

	.text-wrap {
		max-width: 505px;
		display: flex;
		justify-content: center;
		align-items: center;
		padding-top: 30px;
	}

	.text-wrap span {
		font-family: "Montserrat-bold";
		font-style: normal;
		font-weight: 500;
		font-size: 20px;
		line-height: 24px;
		text-align: center;
		color: #000000;
	}

	.btn-wrap {
		display: flex;
		justify-content: center;
		align-items: center;
		padding-top: 30px;
	}

	.btn-wrap button {
		width: 100%;
		max-width: 150px;
		height: 46px;
		background: rgba(158, 33, 64, 0.1);
		font-family: "Montserrat";
		font-style: normal;
		font-weight: 400;
		font-size: 15px;
		line-height: 15px;
		text-align: center;
		color: #9e2140;
		border: none;
		outline: none;
		cursor: pointer;
	}

	/* SIDE HUB STYLE */
	.sides-hub {
		display: flex;
		justify-content: flex-end;
		align-items: flex-end;
		padding-top: 150px;
		padding-right: 40px;
		background-color: #f4f1ef;
	}

	p {
		font-family: "Montserrat";
		font-style: normal;
		font-weight: 400;
		font-size: 12px;
		line-height: 15px;
		color: rgba(0, 0, 0, 0.35);
	}
</style>

<template>
	<div id="app">
		<div class="wrap">
			<div class="banner">
				<div class="logo">
					<img src="./assets/logo.png">
				</div>
				<div class="banner-mes">
					<h1>云智出行</h1>
					<div class="line-box">
						<hr class="line">
					</div>
					<p>
						云智出行倡导智慧环保能源,推进互联网技术与<br />
						新能源产业的深度融合,提升用户体验,创造社<br />
						会价值,建设高效智能的移动出行新生态
					</p>
					<div class="QR-code-box">
						<img src="./assets/QRcode.png" alt="" class="QR-code">
					</div>
				</div>
			</div>
			<div class="row-box">
				<div class="title">
					<img src="./assets/left.png">
					<div class="title-text">
						<h1>关于云智</h1>
						<p>ABOUT YUNZHI</p>
					</div>
					<img src="./assets/right.png">
				</div>
				<div class="content">
					<div class="content-box">
						<div class="left">
							<p>
								广东云智科技信息有限公司成立于2018年，注册资金1000万、总部设立在广东肇庆。旗下设有子公司，业务范围：出行服务，能源服务，餐饮服务，系统软件、硬件研发与生产等！<br />
								推进互联网技术与新能源产业的深度融合，提升用户体验，创造社会价值，建设高效智能的移动出行新生态。
							</p>
						</div>
						<div class="right">
							<img src="./assets/rowImg.png">
						</div>
					</div>
				</div>
			</div>
			<div class="row-box">
				<div class="title">
					<img src="./assets/left.png">
					<div class="title-text">
						<h1>联系我们</h1>
						<p>CONTACT US</p>
					</div>
					<img src="./assets/right.png">
				</div>
				<div class="content contact-box">
					<div class="content-box">
						<div class="left">
							<div class="contactUs">
								<div class="company-mes">
									<div class="p-box">
										<span class="icon-img-span"></span>
										<p class="company">广东云智信息科技有限公司</p>
									</div>
									<div class="p-box">
										<span class="icon-img-span">
											<img src="./assets/icon1.png" alt="">
										</span>
										<p>肇庆市端州区星湖大道15号恒裕城首层155-156号</p>
									</div>
									<div class="p-box">
										<span class="icon-img-span">
											<img src="./assets/icon2.png" alt="">
										</span>
										<p>0758-2777310</p>
									</div>
									<div class="p-box">
										<span class="icon-img-span">
											<img src="./assets/icon3.png" alt="">
										</span>
										<p>178126968@qq.com</p>
									</div>
								</div>
							</div>
						</div>
						<div class="right">
							<img src="./assets/rowImg2.png" class="map">
						</div>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
	export default {
		name: 'app',
		components: {

		}
	}
</script>

<style lang="less">
	@bannerMesColor: #fefefe;
	@contactImgHight: 350px;

	.contentChildBox {
		float: left;
		width: calc(96% / 2 - 40px);
		font-size: 1.55vw;
		margin: 10px;
		color: #5a5652;
	}

	body {
		padding: 0;
		margin: 0;
	}

	.wrap {
		width: 100%;
	}

	.banner {
		width: 100%;
		background: url(./assets/banner.png);
		background-size: 100%;
		background-repeat: no-repeat;
		height: 700px;

		.logo {
			img {
				width: 100%;
				margin: 30px 0 0 80px;
			}

			width: 200px;
		}
	}

	.banner-mes {
		margin: 40px 200px 0 0;
		width: 40%;
		float: right;
		color: @bannerMesColor;
		text-align: right;
		letter-spacing: 3px;

		.line-box {
			overflow: hidden;
		}

		.line {
			float: right;
			width: 75px;
			height: 8px;
			background-color: @bannerMesColor;
			border: 0;
		}

		h1 {
			font-size: 2.3vw;
		}

		p {
			font-size: 1.1vw;
			line-height: 35px;
		}

		.QR-code-box {
			width: 30%;
			overflow: hidden;
			float: right;
			margin-top: 25px;
		}

		.QR-code {
			width: 100%;
		}
	}

	.row-box {
		height: 500px;

		.title {
			text-align: center;
			margin-top: 80px;

			.title-text {
				vertical-align: middle;
				display: inline-block;

				p {
					color: #cccccc;
				}

				h1 {
					color: #544e4b;
				}
			}

			img {
				vertical-align: middle;
				width: 50px;
				margin: 0 50px 0 50px;
			}

			h1,
			p {
				margin: 0;
			}
		}

		.content {
			overflow: hidden;

			.content-box {
				overflow: hidden;
				margin: 0 auto;
				width: 70%;
				margin-top: 30px;
			}

			.left {
				.contentChildBox();
				text-align: left;

				p {
					margin: 0;
				}
			}

			.right {
				.contentChildBox();

				img {
					width: 100%;
				}
			}
		}

		.contact-box {
			height: 500px;

			.left {
				height: @contactImgHight;
				position: relative;
			}

			.contactUs {
				box-shadow: 0 2px 20px 10px rgba(0, 0, 0, 0.1);
				height: 300px;
				width: 90%;
				position: absolute;
				top: 50%;
				transform: translateY(-50%);
				background: #fefefe;
				right: -70px;
				border-left: 10px solid #008ed6;

				p {
					color: #262525;
					font-size: 0.9vw;
					float: left;
					margin: 15px;
				}

				.company {
					color: #1d9ad8;
					font-weight: bold;
					font-size: 1.3vw;
				}

				.p-box {
					overflow: hidden;
				}
			}

			.company-mes {
				margin: 50px 0 0 30px;
			}

			.map {
				height: @contactImgHight;
			}

			.content-box {
				height: 100%;
			}

			.icon-img-span {
				width: 25px;
				height: 25px;
				float: left;
				display: inline-block;
				line-height: 53px;

				img {
					width: 100%;
				}
			}
		}
	}

	@media screen and (min-width: 1200px) and (max-width: 1500px) {
		.banner {
			height: 500px;
		}
	}

	@media screen and (min-width: 992px) and (max-width: 1200px) {
		.banner {
			height: 460px;
		}

		.banner-mes p {
			line-height: 30px;
		}

		.banner-mes {
			margin: 0px 150px 0 0;
		}

		.row-box .title {
			margin-top: 30px;
		}

		.row-box {
			height: 360px;
		}

		.row-box .content .content-box {
			width: 80%;
		}

		.icon-img-span {
			line-height: 51px;
		}

		.row-box .contact-box .contactUs {
			width: 110%;
		}

		.row-box .content .right {
			width: calc(96% / 2);
		}
	}

	@media screen and (max-width: 992px) {
		.banner {
			height: 300px;
		}

		.banner .logo {
			width: 100px;
		}

		.banner-mes p {
			line-height: 25px;
		}

		.banner-mes .QR-code-box {
			margin-top: 0;
		}

		.banner-mes {
			margin: 0px 150px 0 0;
		}

		.row-box .title {
			margin-top: 30px;
		}

		.row-box {
			height: 350px;
		}

		.row-box .content .content-box {
			width: 95%;
		}

		.row-box .contact-box .contactUs {
			width: 110%;
		}

		.row-box .content .right {
			width: calc(98% / 2);
		}

		.row-box .contact-box .icon-img-span {
			line-height: 36px;
		}
	}

	@media screen and (max-width: 768px) {
		.wrap {
			min-width: 768px;
		}
	}
</style>

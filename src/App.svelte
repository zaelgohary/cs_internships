<script>
	let headerImg = "assets/images/header.png";
	let headerText = "assets/images/text_header.png"
</script>

<main>
	<header>
		<div>
			<img src={headerImg} alt="studying" class="hero-img"/>
		</div>
		<div class="hero-txt">
			<img src={headerText} alt="header text" class="txt-img"/>
			<p class="logo-description">Start your learning journey with Codescalers and access material for multiple tracks like Software Engineering & QA!</p>
		</div>
	</header>
	<div class="courses">
		<h1 class="title">Courses</h1>

		<div class="wrapper">
			<div class="tabs">
				<div class="tab">
					<input type="radio" name="css-tabs" id="tab-1" checked class="tab-switch">
					<label for="tab-1" class="tab-label">Software Engineering</label>
					<div class="tab-content">My father had a small estate in Nottinghamshire: I was the third of five sons. He sent me to Emanuel College in Cambridge at fourteen years old, where I resided three years, and applied myself close to my studies; but the charge of maintaining me, although I had a very scanty allowance, being too great for a narrow fortune, I was bound apprentice to Mr. James Bates, an eminent surgeon in London, with whom I continued four years. </div>
				</div>
				<div class="tab">
					<input type="radio" name="css-tabs" id="tab-2" class="tab-switch">
					<label for="tab-2" class="tab-label">QA</label>
					<div class="tab-content">My father now and then sending me small sums of money, I laid them out in learning navigation, and other parts of the mathematics, useful to those who intend to travel, as I always believed it would be, some time or other, my fortune to do. </div>
				</div>
				<div class="tab">
					<input type="radio" name="css-tabs" id="tab-3" class="tab-switch">
					<label for="tab-3" class="tab-label">External Links</label>
					<div class="tab-content">When I left Mr. Bates, I went down to my father: where, by the assistance of him and my uncle John, and some other relations, I got forty pounds, and a promise of thirty pounds a year to maintain me at Leyden: there I studied physic two years and seven months, knowing it would be useful in long voyages.</div>
				</div>
			</div>
			<p>Example line outside of tab box</p>
		</div>
	</div>
	<footer>All rights reserved &copy; 2022 Codescalers Egypt</footer>
</main>

<style>
header{
	display: flex;
	justify-content: space-between;
	height: 40vh;
	background-color: #45b5e5;
	color: #fff;
	padding: 4rem 1rem 1rem 2rem;
}

.hero-txt{
	margin-right: 3rem;
	margin-top: 2rem;
}
.hero-img{
	width: 35vw;
	height: 38vh;
}

.txt-img{
	width: 40vw;
	height: 20vh;
}

.logo-description{
	max-width: 40vw;
	font-size: 1.2rem;
}

.courses{
	min-height: 50vh;
	background-color: #232323;
	color: #fff;
	padding: 2rem;
}

.title{
	font-weight: bold;
	text-align: center;
	margin: 0;
}

.wrapper {
  max-width: 95rem;
  width: 100%;
  margin: 0 auto;
}
.tabs {
  position: relative;
  margin: 2rem 0;
  height: 14.75rem;
}
.tabs::before,
.tabs::after {
  content: "";
  display: table;
}
.tabs::after {
  clear: both;
}
.tab {
  float: left;
}
.tab-switch {
  display: none;
}
.tab-label {
  position: relative;
  display: block;
  line-height: 2.75em;
  height: 3em;
  padding: 0 1.618em;
  background: #3a3a3a;
  color: #fff;
  cursor: pointer;
  top: 0;
  transition: all 0.25s;
}
.tab-label:hover {
  top: -0.25rem;
  transition: top 0.25s;
}
.tab-content {
  height: 12rem;
  position: absolute;
  z-index: 1;
  top: 2.75em;
  left: 0;
  padding: 1.618rem;
  background: #fff;
  color: #2c3e50;
  opacity: 0;
  transition: all 0.35s;
}
.tab-switch:checked + .tab-label {
  background: #fff;
  color: #2c3e50;
  border-bottom: 0;
  transition: all 0.35s;
  z-index: 1;
  top: -0.0625rem;
}
.tab-switch:checked + label + .tab-content {
  z-index: 2;
  opacity: 1;
  transition: all 0.35s;
}

footer{
	text-align: center;
	background-color: #45b5e5;
	color: #fff;
	height: 4vh;
	padding-top: 1.5rem;
}
</style>
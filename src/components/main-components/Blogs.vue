<template>
	<section id="blogs" class="py-5 mb-5">
		<div class="container">
			<div class="row gx-5">
				<div class="col-4">
					<!-- BLOGS TEXT -->
					<div class="blogs-text d-flex flex-column">
						<p class="subtitle my-gray">ENJOYABLE INSIGHTS</p>
						<h4 class="title my-blue mb-4">
							Most Viewed <span class="my-primary"> Best Blogs</span>
						</h4>
						<ul class="ps-0">
							<li class="d-flex align-items-center">
								<i class="fas fa-long-arrow-alt-right pe-2 pb-3"></i>
								<p>
									Became a Better Blogger: Content Planning
								</p>
							</li>
							<li>
								<i class="fas fa-long-arrow-alt-right pe-2 pb-3"></i>Promoting
								Your Online Buisness on Pinterest
							</li>
							<li>
								<i class="fas fa-long-arrow-alt-right pe-2 pb-3"></i
								>Gamification and Game-Based Learning
							</li>
							<li>
								<i class="fas fa-long-arrow-alt-right pe-2 pb-3"></i>Designing
								an Online Course from Expert's Perspective
							</li>
							<li>
								<i class="fas fa-long-arrow-alt-right pe-2 pb-3"></i>Why Online
								Courses Are the Future of Education
							</li>
						</ul>
					</div>
				</div>
				<!-- BLOG CARDS -->

				<div v-for="(blog, index) in blogs" :key="index" class="col-4">
					<div class="card mx-o" style="width: 18rem;">
						<img
							:src="require(`../../assets/img/${blog.img}`)"
							class="card-img-top"
							alt="..."
						/>
						<div class="card-body ps-4">
							<p class="my-gray">{{ blog.profession }}</p>
							<h6 class="my-blue">{{ blog.title }}</h6>
							<span class="my-gray me-4 mb-3"
								><i class="far fa-calendar pe-2"></i>{{ blog.data }}</span
							><span class="my-gray mb-3"
								><i class="far fa-eye pe-2"></i>{{ blog.views }}</span
							>
						</div>
					</div>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
	name: "Blogs",
	data() {
		return {
			blogs: [
				{
					profession: "ARTIST",
					img: "artist-blog-03-480x352.jpeg",
					title: "Brush Strokes Energize Trees in Paintings",
					data: "May 15, 2020",
					views: "688",
				},
				{
					profession: "ARTIST",
					img: "artist-blog-01-480x352.jpg",
					title: "Pocket-Sized Notebooks Hold Miniature Pintings",
					data: "May 15, 2020",
					views: "603",
				},
			],
		};
	},
};
</script>

<style scoped lang="scss">
//SCSS

#blogs {
	background-color: #f5f1ed;
	.blogs-text {
		li {
			font-size: 10px;
			font-weight: 800;
		}
	}
	.card-body {
		p {
			font-weight: 600;
			font-size: 12px;
			letter-spacing: 1px;
		}
		h6 {
			font-weight: 700;
			font-size: 14px;
		}
		span {
			font-size: 12px;
			font-weight: 600;
		}
	}
}
</style>

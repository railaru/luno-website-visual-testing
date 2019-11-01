usage:
test: $backstop test
aprove a baseline: $backstop approve

test comments & exceptions:

/ homepage: testimonials are randomized everytime a page loads which cause differences as compared to the baseline

/blog: .blog-card-hero (backgound images sometimes include GIFs which move after creating the baseline which may brake the tests)

/price: wait for <app-price/> to load on the DOM before taking snapshots. Ignore <google-chart> as the price will change overtime 

/careers/jobs: ignore .gallery--wrap img because they're generated randomly and change each time user reloads the page

/careers/who-we-are: ignore .gallery--wrap img and .lunaut-images--wrap--block--icon because they're generated randomly and change each time user reloads the page
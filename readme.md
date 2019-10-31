usage:
test: $backstop test
aprove a baseline: $backstop approve

test exceptions:
/ homepage testimonials are randomized everytime a page loads which cause differences as compared to the baseline
/blog: .blog-card-hero (backgound images sometimes include GIFs which move after creating the baseline which may brake the tests)

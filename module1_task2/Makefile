help :
	@echo "post : post your new post"
	@echo "clean: clears recursively the directory dist"

post: # post your new post
	hugo new posts/${POST_NAME}.md
	sed -i '/title/c\title: "${POST_TITLE}"' content/posts/${POST_NAME}.md

clean: # clears recursively the directory dist
	rm -fr dist

build: 
	hugo > /dev/null 2>&1
build: # builds the site
	hugo > /dev/null 2>&1

clean: # cleans directory dist
	rm -fr dist

post: # post your new post
	hugo new posts/${POST_NAME}.md
	sed -i '/title/c\title: "${POST_TITLE}"' content/posts/${POST_NAME}.md

help : #if helps needed, helps here
	@echo "post : post your new post"
	@echo "clean: cleans recursively the directory dist"
	@echo "build: builds the site"
	@echo "help: information on commands"
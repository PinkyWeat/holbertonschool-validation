build:	## Builds the site using hugo.
		hugo > /dev/null 2>&1

clean:	## Clean the site's directory
		rm -fr dist

post:	## Creates a post using POST_NAME & POST_TITLE.
		hugo new posts/${POST_NAME}.md
		sed -i '/title/c\title: "${POST_TITLE}"' content/posts/${POST_NAME}.md

package: ## produces a file awesome-website.zip, containing the binary awesome-api and the directory dist
	zip -r awesome-website.zip dist/ awesome-api

lint: ## update files README.md and DEPLOY.md to markdownlint
	markdownlint --fix DEPLOY.md

help: ## If helps needed, helps here
	@fgrep -h "##" $(MAKEFILE_LIST) | fgrep -v fgrep | sed -e 's/\\$$//' | sed -e 's/##//'

unit-tests: ## ERROR: No comment found for target unit-tests in ./Makefile

integration-tests: ## ERROR: No comment found for target integration-tests in ./Makefile

validate: ## ERROR: No comment found for target validate in ./Makefile
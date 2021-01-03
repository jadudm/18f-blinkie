all:
	@echo $(PWD)
	docker run -v $(PWD):/site bretfisher/jekyll build --config "_config.yml,_publish.yml"
	rsync  -avH _site/ -e ssh jadudm@jadud.com:~/jadud.com/18f-blinkie
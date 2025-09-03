%: clean %/hugo.toml
	cp -rs $(@)/* ./meta/
	cd ./meta && hugo --gc --minify

clean:
	find meta -type d -name public -exec rm -vr {} + -depth
	find meta -type l -not -path "meta/themes/*" -exec rm -v {} +

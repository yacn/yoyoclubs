%: clean %/hugo.toml
	cp -rl $(CURDIR)/$(@)/* ./meta/
	cd ./meta && hugo --gc --minify

clean:
	find meta -type d -name public -exec rm -vr {} + -depth
	find meta -type f -links +1 -exec rm -v {} +
	find meta -type f -name "hugo.toml" -exec rm -v {} +

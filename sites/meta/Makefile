%: clean site.%.toml
	[ ! -h hugo.toml ] || unlink hugo.toml
	ln -s "./site.$(@).toml" hugo.toml
	hugo --gc --minify
	unlink hugo.toml

clean:
	[ ! -d ./public ] || rm -r ./public/

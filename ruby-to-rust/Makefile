all: target/libdouble_input.so
	ruby src/main.rb

target/libdouble_input.so: src/lib.rs Cargo.toml
	cargo build
	(cd target && ln -nsf debug/libdouble_input-* libdouble_input.so)

clean:
	rm -rf target

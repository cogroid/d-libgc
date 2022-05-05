all:
	sudo mkdir -p /home/cogroid/local/libgc/x64
	cd ../../; \
	./autogen.sh --no-configure; \
	./configure \
	--prefix=/home/cogroid/local/libgc/x64 \
	--docdir=/home/cogroid/local/libgc/x64/share/doc/libgc-7.4.2; \
	export CPPFLAGS="-v"; \
	export CFLAGS="-v"; \
	make

install:
	sudo sh -c 'cd ../../; \
	make install;'
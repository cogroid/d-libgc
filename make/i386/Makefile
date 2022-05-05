all:
	sudo mkdir -p /home/cogroid/local/libgc/i386

	sudo mkdir -p /home/cogroid/local/libatomic_ops/i386
	sudo cp -rf ./libatomic_ops/* /home/cogroid/local/libatomic_ops/i386/

	cd ../../; \
	./autogen.sh --no-configure; \
	./configure \
	ABI=32 \
	--build=i386-linux-gnu \
	--host=i386-linux-gnu \
	CXXFLAGS="-v -m32 -march=i386 " \
	CPPFLAGS="-v -m32 -march=i386 " \
	CFLAGS="-v -m32 -march=i386 " \
	LDFLAGS="-v -m32 -march=i386 " \
	ATOMIC_OPS_CFLAGS="-I /home/cogroid/local/libatomic_ops/i386/include -L/home/cogroid/local/libatomic_ops/i386/lib/i386-linux-gnu -B/home/cogroid/local/libatomic_ops/i386/lib/i386-linux-gnu -latomic_ops " \
	ATOMIC_OPS_LIBS="-I /home/cogroid/local/libatomic_ops/i386/include -L/home/cogroid/local/libatomic_ops/i386/lib/i386-linux-gnu -B/home/cogroid/local/libatomic_ops/i386/lib/i386-linux-gnu -latomic_ops " \
	--prefix=/home/cogroid/local/libgc/i386 \
	--docdir=/home/cogroid/local/libgc/i386/share/doc/libgc-7.4.2; \
	make

install:
	sudo sh -c 'cd ../../; \
	export CPPFLAGS="-v -m32 -march=i386 "; \
	export CFLAGS="-v -m32 -march=i386 "; \
	make install;'

clean:
	cd ../../; \
	make clean
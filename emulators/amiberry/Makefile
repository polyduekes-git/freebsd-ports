PORTNAME=	amiberry
DISTVERSION=	v7.1.0
CATEGORIES=	emulators

MAINTAINER=	polyduekes@proton.me
COMMENT=	Optimized Amiga emulator
WWW=		https://github.com/BlitterStudio/amiberry

LICENSE=	GPLv3
LICENSE_FILE=	${WRKSRC}/LICENSE

BUILD_DEPENDS=${LOCALBASE}/include/sys/sysinfo.h:devel/libsysinfo

LIB_DEPENDS=	libpng.so:graphics/png \
		libportmidi.so:audio/portmidi \
		libenet.so:net/enet \
		libFLAC.so:audio/flac \
		libmpg123.so:audio/mpg123 \
		libmpeg2.so:multimedia/libmpeg2 \
		libzstd.so:archivers/zstd \
		libserialport.so:devel/libserialport

RUN_DEPENDS=	${LOCALBASE}/share/icons/hicolor/index.theme:misc/hicolor-icon-theme

USES=		cmake desktop-file-utils ninja pkgconfig sdl shared-mime-info

USE_SDL=	image2 sdl2 ttf2

USE_GITHUB=	yes
GH_ACCOUNT=	BlitterStudio
GH_PROJECT=	amiberry

.include <bsd.port.mk>

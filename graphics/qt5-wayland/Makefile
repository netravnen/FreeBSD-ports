# $FreeBSD$

PORTNAME=	wayland
DISTVERSION=	${QT5_VERSION}
CATEGORIES=	graphics
PKGNAMEPREFIX=	qt5-

MAINTAINER=	kde@FreeBSD.org
COMMENT=	Qt5 wrapper for Wayland

LIB_DEPENDS=	libfontconfig.so:x11-fonts/fontconfig \
		libfreetype.so:print/freetype2 \
		libwayland-client.so:graphics/wayland \
		libxkbcommon.so:x11/libxkbcommon

USES=		pkgconfig qmake:outsource
USE_GL=		egl gl
USE_GNOME=	glib20
USE_QT5=	core dbus gui qml quick \
		buildtools_build qmake_build
USE_XORG=       x11 xcomposite
QT_DIST=	${PORTNAME}

USE_LDCONFIG=	${PREFIX}/${QT_LIBDIR_REL}

.include <bsd.port.mk>

# $FreeBSD$

PORTNAME=	trident-installer
PORTVERSION=	%%CHGVERSION%%
CATEGORIES=	trident

MAINTAINER=	ken@ixsystems.com
COMMENT=	Graphical ISO installer for Project Trident

LICENSE=	BSD2CLAUSE

RUN_DEPENDS=	lumina-coreutils>=0:x11/lumina-coreutils \
		trident-icons>=0:trident/trident-icons \
		jq>=0:textproc/jq \
		cursor-chameleon-pearl>=0:x11-themes/cursor-chameleon-pearl \
		xinit>=0:x11/xinit \
		${NONEXISTENT}:graphics/drm-kmod \
		xorg-minimal>=0:x11/xorg-minimal \
		xf86-video-scfb>=0:x11-drivers/xf86-video-scfb \
		setxkbmap>=0:x11/setxkbmap \
		pc-sysinstall>=0:sysutils/pc-sysinstall
		

USES=	qmake qt:5
USE_QT=	core gui widgets svg concurrent \
		buildtools_build linguist_build
USE_GITHUB=	yes
GH_ACCOUNT=	project-trident
GH_PROJECT=	trident-installer
GH_TAGNAME=	%%GHTAG%%
WRKSRC_SUBDIR=	src-qt5

.include <bsd.port.mk>

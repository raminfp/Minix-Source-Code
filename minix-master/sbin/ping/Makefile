#	$NetBSD: Makefile,v 1.17 2013/11/09 21:39:27 christos Exp $
#	@(#)Makefile	8.1 (Berkeley) 6/5/93

USE_FORT?= yes	# setuid
RUMPPRG=ping
MAN=	ping.8
BINOWN=	root
BINMODE=4555
LDADD=	-lm
DPADD=	${LIBM}

# BJG - no ipsec
#CPPFLAGS+=	-DIPSEC

#LDADD+= -lipsec
#DPADD+= ${LIBIPSEC}

.if ${MACHINE_ARCH} == "vax"
COPTS.ping.c=-O0
.endif

.include <bsd.prog.mk>

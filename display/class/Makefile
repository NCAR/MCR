#
# mcrtd C++ class makefile
#
I2D=	../include
O2D=	../obj

INCLUDES=	-I/usr/X11R6/include -I${I2D} -I${JLOCAL}/include
DEFINES=
CXXFLAGS=	-g ${INCLUDES} ${DEFINES}

OBJS=	CanvasWindow.o DataBuffer.o XColorMap.o
SRCS=	CanvasWindow.cc DataBuffer.cc XColorMap.cc

HDRS=	${I2D}/mcrtd.h

all: ${OBJS}


${OBJS}: ${HDRS}

CanvasWindow.o:		${I2D}/CanvasWindow.h ${JLOCAL}/include/raf/Window.h
DataBuffer.o:		${I2D}/DataBuffer.h ${JLOCAL}/include/raf/hdrAPI.h
XColorMap.o:		${I2D}/XColorMap.h

clean:
	${RM} *.o

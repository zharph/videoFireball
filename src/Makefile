OPENCV = -lopencv_core -lopencv_highgui -lopencv_imgproc -lopencv_videoio -lopencv_imgcodecs
BOOST = -lboost_filesystem -lboost_system

CFLAGS = -std=c++11 -g -m64 -lrt -fsanitize=address -fno-omit-frame-pointer
# -m64: generate code for 64 bit environment
# -lrt link with libraries

LIBSPATH = -L../lib/x64/


videoFireball: main.cpp
	g++ $(CFLAGS) main.cpp -o videoFireball $(OPENCV) $(BOOST) $(LIBSPATH) -lASICamera2 -lX11


clean:
	rm videoFireball


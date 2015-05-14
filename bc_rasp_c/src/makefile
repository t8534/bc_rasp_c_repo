# This is makefile from bc_pc_emu
#
#

# headers subdirs
#IDIRS = -I. -I./libs/sdl/include/SDL2 -I./sys

CC=gcc   
CFLAGS=-c -Wall $(IDIRS) 

#CXX=g++
#CXXFLAGS=-c -Wall $(IDIRS) 

LDFLAGS=
LDLIBS=
#LDLIBS= -L./libs/sdl/libs -lmingw32 -lSDL2main -lSDL2 

%.o: %.c
	$(CC) $(CFLAGS) $<

# all source subdirs for linker and compilator
#VPATH = ./ libs libs/sdl libs/sdl/libs sys
#VPATH = ./ sys
VPATH = ./ 

all : bc_rasp_c

#bc_rasp_c : bc_rasp_c.o app_timer.o hal.o  
#	$(CC) -o bc_pc_emu_c.exe bc_pc_emu_c.o app_timer.o hal.o $(LDLIBS)
bc_rasp_c : bc_rasp_c.o   
	$(CC) -o bc_rasp_c bc_rasp_c.o $(LDLIBS)


clean:
	rm -f bc_rasp_c bc_rasp_c.o 



##########################################################
### Working base 

## headers subdirs
#IDIRS = -I. -I./display -I./sensor -I./sound  -I./sys  -I./vario
#
#CC=gcc   
#CFLAGS=-c -Wall $(IDIRS) 
#
##CXX=g++
##CXXFLAGS=-c -Wall $(IDIRS) 
#
#LDFLAGS=
#LDLIBS=
#
## all source subdirs for linker and compilator
#VPATH = ./ display sensor sound sys vario
#
#all : vario_emu_pc.exe
#
#vario_emu_pc.exe : vario_emu_pc.o display.o BP085.o sensor.o sound.o app_timer.o hal.o calc.o  
#	$(CC) -o vario_emu_pc.exe vario_emu_pc.o display.o BP085.o sensor.o sound.o app_timer.o hal.o calc.o




	
	
	
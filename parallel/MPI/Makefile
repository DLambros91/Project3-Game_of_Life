CC = mpicc
CFLAGS = -std=gnu99
OUTPUT = ./exec
EXEOBJ = .gol.o
default: $(OUTPUT)
all: default

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

$(OUTPUT): $(EXEOBJ)
	$(CC) $(CFLAGS) $(EXEOBJ) timer.h -o $@

clean:
	rm -f *.o $(OUTPUT)

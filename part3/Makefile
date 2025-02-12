CC = gcc
CFLAGS = -Wall -g -std=gnu99
TARGET = one_list
OBJS = one_list.o linked_list.o

default: $(TARGET)

linked_list.o: linked_list.c
	$(CC) $(CFLAGS) -c -o $@ $<

one_list.o: one_list.c
	$(CC) $(CFLAGS) -c -o $@ $<

$(TARGET): $(OBJS)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS)

run: $(TARGET)
	./$(TARGET)

clean:
	rm $(TARGET) $(OBJS)


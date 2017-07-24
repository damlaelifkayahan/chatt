-include ${BSPROOT}/.config

TX_TARGET = user_tx
RX_TARGET = user_rx

TX_SOURCES = tx.c
# TX_DEPS = mydep.c

RX_SOURCES = receive.c
# RX_DEPS = mydep.c

CFLAGS += -Wall

default: all

all: $(TX_TARGET) $(RX_TARGET)

$(TX_TARGET): $(TX_SOURCES) $(TX_DEPS)
	$(CC) $(CFLAGS) $(TX_SOURCES) $(TX_DEPS) -o $(TX_TARGET)

$(RX_TARGET): $(RX_SOURCES) $(RX_DEPS)
	$(CC) $(CFLAGS) $(RX_SOURCES) $(RX_DEPS) -o $(RX_TARGET)

clean:
	rm -rf $(TARGET)

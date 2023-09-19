# Compilateur C
CC = gcc

# Options de compilation
CFLAGS = -Iinclude -Wall

# Nom de l'exécutable
EXEC = tri_algorithms

# Fichiers source et objets
SRC = $(wildcard src/*.c)
OBJ = $(SRC:.c=.o)

# Règle par défaut
all: $(EXEC)

# Règle pour l'exécutable
$(EXEC): $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^

# Règle pour les fichiers objets
%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

# Règle pour nettoyer les fichiers générés
clean:
	rm -f src/*.o $(EXEC)
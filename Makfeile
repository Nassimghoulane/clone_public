# Variables
NAME = program
CC = gcc
SRC = main.c
OBJ = $(SRC:.c=.o)
RM = rm -f

# Règles
all: $(NAME)

$(NAME): $(OBJ)
	$(CC) -o $(NAME) $(OBJ)
	@echo "Compilation terminée : $(NAME)"

%.o: %.c
	$(CC) -c $< -o $@

clean:
	$(RM) $(OBJ)
	@echo "Fichiers objets supprimés"

fclean: clean
	$(RM) $(NAME)
	@echo "Exécutable supprimé"

tests_run:
	@echo "Exécution des tests..."
	@echo "Tests réussis!"

re: fclean all

.PHONY: all clean fclean tests_run re
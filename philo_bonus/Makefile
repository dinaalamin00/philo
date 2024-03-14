SRC = 

BONUS = 

CC = gcc
CFLAGS = -Wall -Wextra -Werror
OBJ = ${SRC:.c=.o}
# BONOBJ = ${BONUS:.c=.o}
LIBS = ar rcs
NAME = libft.a

all: $(NAME)

$(NAME): $(OBJ)
	$(LIBS) $(NAME) $(OBJ)

%.o: %.c
	$(CC) $(CFLAGS)  -c $< -o $@
	
# bonus: $(NAME) $(BONOBJ)
# 	$(LIBS) $(NAME) $(BONOBJ)

clean:
	rm -f $(OBJ) $(BONOBJ)

fclean: clean
	rm -f $(NAME)

re: fclean all
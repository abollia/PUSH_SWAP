NAME	= libft.a

SRC	= ${IS} ${MEM} ${FD} ${LST} ${STR_OPS} ${TO} ${PRINTF}

IS		=	./is/ft_isalpha.c \
			./is/ft_isdigit.c \
			./is/ft_isalnum.c \
			./is/ft_isascii.c \
			./is/ft_isprint.c 

TO		=	./to/ft_toupper.c \
			./to/ft_tolower.c \
			./to/ft_atoi.c \
			./to/ft_atol.c \
			./to/ft_itoa.c 

MEM		=	./mem/ft_calloc.c \
			./mem/ft_ffa.c \
			./mem/ft_memchr.c \
			./mem/ft_memcmp.c \
			./mem/ft_memcpy.c \
			./mem/ft_memmove.c \
			./mem/ft_memset.c \
			./mem/ft_bzero.c 

FD		=	./fd/ft_putchar_fd.c \
			./fd/ft_putstr_fd.c \
			./fd/ft_putendl_fd.c \
			./fd/ft_putnbr_fd.c

LST		=	./lst/ft_lstnew.c \
			./lst/ft_lstadd_front.c \
			./lst/ft_lstsize.c \
			./lst/ft_lstlast.c \
			./lst/ft_lstadd_back.c \
			./lst/ft_lstdelone.c \
			./lst/ft_lstclear.c \
			./lst/ft_lstiter.c \
			./lst/ft_lstmap.c \
			./lst/ft_lstissorted.c

STR_OPS	=	./str_ops/ft_strlen.c \
			./str_ops/ft_strlcpy.c \
			./str_ops/ft_strlcat.c \
			./str_ops/ft_strchr.c \
			./str_ops/ft_strrchr.c \
			./str_ops/ft_strncmp.c \
			./str_ops/ft_strnstr.c \
			./str_ops/ft_strdup.c \
			./str_ops/ft_substr.c \
			./str_ops/ft_strjoin.c \
			./str_ops/ft_strtrim.c \
			./str_ops/ft_split.c \
			./str_ops/ft_strmapi.c \
			./str_ops/ft_striteri.c

PRINTF	=	./ft_printf/ft_printf.c \
			./ft_printf/ft_print_pxX.c \
			./ft_printf/ft_print_diu.c \
			./ft_printf/ft_print_cs%.c

OBJ	= ${SRC:.c=.o}

CC		= gcc

FLAGS	= -Wall -Werror -Wextra

all:		${NAME}

%.o: %.c
			@${CC} ${FLAGS} -c $< -o ${<:.c=.o}

${NAME}:	${OBJ}
			@ar rcs ${NAME} ${OBJ}

clean:
			@rm -f ${OBJ}

fclean:		clean
			@rm -f ${NAME}

re:			fclean all

.PHONY:		all clean fclean re

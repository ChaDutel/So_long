# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: cdutel-l <cdutel-l@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/11/29 11:52:00 by cdutel-l          #+#    #+#              #
#    Updated: 2022/05/18 12:21:56 by cdutel-l         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRCS = ft_bzero.c ft_isalnum.c ft_isalpha.c ft_isascii.c ft_isdigit.c ft_isprint.c ft_memcpy.c\
	   ft_memmove.c ft_memset.c ft_strlen.c ft_strnstr.c ft_tolower.c ft_toupper.c ft_strchr.c \
	   ft_strrchr.c ft_strncmp.c ft_memchr.c ft_memcmp.c ft_atoi.c ft_strlcpy.c ft_strlcat.c\
	   ft_calloc.c ft_strdup.c ft_substr.c ft_strjoin.c ft_strtrim.c ft_putchar_fd.c ft_putstr_fd.c\
	   ft_putendl_fd.c ft_putnbr_fd.c ft_split.c ft_itoa.c ft_striteri.c ft_strmapi.c\
		ft_printf.c ft_putchar.c ft_putstr_mod.c ft_putstr_mod2.c\
		ft_ifft.c ft_nbh.c ft_nbhmaj.c ft_pvoidh.c ft_string.c ft_unsignedputnbr.c\
		ft_putnbr.c get_next_line_bonus.c get_next_line_utils_bonus.c

SRCSBONUS = ft_lstsize.c ft_lstnew.c ft_lstlast.c ft_lstadd_front.c ft_lstadd_back.c ft_lstdelone.c ft_lstclear.c\
			ft_lstiter.c ft_lstmap.c
OBJS = ${SRCS:.c=.o}
OBJSBONUS = ${SRCSBONUS:.c=.o}

NAME = libft.a

CC = gcc

RM = rm -f

CFLAGS = -Wall -Wextra -Werror

%.o : %.c libft.h Makefile
		${CC} ${CFLAGS} -I includes -c $< -o ${<:.c=.o}

${NAME} : ${OBJS}
		 ar rcs ${NAME} ${OBJS}

all : ${NAME}

clean :
		${RM} ${OBJS} ${OBJSBONUS}

fclean : clean
		${RM} ${NAME}

re : fclean all

bonus : ${NAME} ${OBJSBONUS}
	ar rcs ${NAME} ${OBJSBONUS}

.PHONY : all clean fclean re bonus
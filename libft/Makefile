# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: jdo <jdo@student.42.fr>                    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2020/04/10 12:59:29 by jdo               #+#    #+#              #
#    Updated: 2020/04/14 10:44:14 by jdo              ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME=libft.a
CC=gcc
CFLAGES=-Wall -Werror -Wextra -std=c99
SRCS=ft_atoi.c ft_bzero.c ft_calloc.c ft_isalnum.c ft_isalpha.c ft_isascii.c \
	ft_isdigit.c ft_isprint.c ft_itoa.c ft_memccpy.c ft_memchr.c ft_memcmp.c \
	ft_memcpy.c ft_memmove.c ft_memset.c ft_putchar_fd.c ft_putendl_fd.c\
	ft_putnbr_fd.c ft_putstr_fd.c ft_split.c ft_strchr.c ft_strdup.c\
	ft_strjoin.c ft_strlcat.c ft_strlcpy.c ft_strlen.c ft_strmapi.c\
	ft_strncmp.c ft_strnstr.c ft_strrchr.c ft_strtrim.c ft_substr.c\
	ft_tolower.c ft_toupper.c
BSRCS=ft_lstadd_back.c ft_lstadd_front.c ft_lstclear.c ft_lstdelone.c\
	ft_lstiter.c ft_lstlast.c ft_lstmap.c ft_lstnew.c ft_lstsize.c
OBJS=$(SRCS:.c=.o)
BOBJS=$(BSRCS:.c=.o)
all:$(NAME)

.c.o:
	$(CC) $(CFLAGES) -c $< -o $@ -I.

$(NAME) : $(OBJS)
	ar rc $(NAME) $(OBJS)

clean:
	rm -rf $(OBJS) $(BOBJS)

fclean: clean
	rm -rf $(NAME)

bonus: $(BOBJS) $(OBJS)
	ar rc $(NAME) $(BOBJS) $(OBJS)

re : fclean all

.PHONY : all clean re fclean
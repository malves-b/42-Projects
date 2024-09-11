# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: malves-b <malves-b@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/11/02 13:52:22 by malves-b          #+#    #+#              #
#    Updated: 2023/11/09 12:52:40 by malves-b         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

FILES = \
	ft_printf.c ft_putstr.c \
	ft_print_char.c ft_putnbr.c \
	ft_print_ptr.c ft_putnbr_hex.c \
	ft_unsnbr.c

OBJS = $(FILES:.c=.o)

CC = cc
CFLAGS = -Wall -Wextra -Werror
RM = rm -f

NAME = libftprintf.a

$(NAME): $(OBJS)
	ar rcs $(NAME) $(OBJS)

all: $(NAME)

clean:
	$(RM) $(OBJS)

fclean: clean
	$(RM) $(NAME)

re: fclean $(NAME)

.PHONY: all, clean, fclean, re

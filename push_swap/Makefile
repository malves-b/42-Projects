# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: malves-b <malves-b@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/05/06 11:33:04 by malves-b          #+#    #+#              #
#    Updated: 2024/06/09 18:34:27 by malves-b         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

TARGET = push_swap

FILES = \
	push_swap.c push_swap_utils.c \
	sort_stack_utils2.c \
	sort_stack.c sort_stack_utils.c \
	ft_free.c ft_check.c \
	operations/push.c operations/rev_rotate.c \
	operations/rotate.c operations/swap.c \
	libft/ft_atoi.c libft/ft_isdigit.c \
	libft/ft_split.c libft/ft_strlen.c \
	libft/ft_strncmp.c libft/ft_atol.c\
	libft/ft_calloc.c libft/ft_bzero.c\
	libft/ft_memset.c \
	ft_printf/ft_print_char.c ft_printf/ft_print_ptr.c \
	ft_printf/ft_printf.c ft_printf/ft_putnbr_hex.c \
	ft_printf/ft_putnbr.c ft_printf/ft_putstr.c \
	ft_printf/ft_unsnbr.c

OBJS = $(FILES:.c=.o)

CC		= cc
CFLAGS	= -Wall -Wextra -Werror -g
RM	= rm -f

LIBRARY	=	push_swap.a

all: $(TARGET)

$(TARGET): $(OBJS) $(LIBRARY)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJS) $(LIBRARY)

$(LIBRARY): $(OBJS)
	ar rcs $(LIBRARY) $(OBJS)

%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	$(RM) $(OBJS)

fclean: clean
	$(RM) $(LIBRARY) $(TARGET)

re: fclean all

.PHONY: all, clean, fclean, re

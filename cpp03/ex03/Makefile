# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: pllucian <pllucian@21-school.ru>           +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2021/12/07 22:23:23 by pllucian          #+#    #+#              #
#    Updated: 2021/12/09 01:53:39 by pllucian         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

SRCS =	ClapTrap.cpp \
		ScavTrap.cpp \
		FragTrap.cpp \
		DiamondTrap.cpp \
		main.cpp

OBJS = $(SRCS:.cpp=.o)

INCL =	ClapTrap.hpp \
		ScavTrap.hpp \
		FragTrap.hpp \
		DiamondTrap.hpp

NAME = test

CC = clang++

CFLAGS = -Wall -Wextra -Werror

%.o:		%.cpp
			$(CC) $(CFLAGS) -c $< -o $@

$(NAME):	$(OBJS) $(INCL)
			$(CC) -o $@ $(OBJS)

all:		$(NAME)

clean:
			$(RM) $(OBJS)

fclean:		clean
			$(RM) $(NAME)

re:			fclean all

.PHONY:		all clean fclean re

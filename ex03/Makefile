CXX				= c++
CXXFLAGS			= -Wall -Wextra -Werror -std=c++98
RM				= rm -fr
INC				= HumanA.hpp HumanB.hpp Weapon.hpp
NAME			= UnnecessaryViolence

SOURCES			= main.cpp Weapon.cpp HumanA.cpp HumanB.cpp

SOURCES_O		= $(SOURCES:.cpp=.o)

all:			$(NAME)

$(NAME):	$(SOURCES)
	@$(CXX) $(CXXFLAGS) $(INC) $(SOURCES) -o $(NAME)

clean:
	@$(RM) $(SOURCES_O)

fclean:			clean
	@$(RM) $(NAME)

re:				fclean $(NAME)

exe:
	clear
	@$(RM) $(SOURCES_O)
	@$(RM) $(NAME)
	@$(CXX) $(CXXFLAGS) $(INC) $(SOURCES) -o $(NAME)
	@./$(NAME)

.PHONY:			all clean fclean re exe
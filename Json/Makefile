

THORSANVIL_ROOT			= $(realpath ../)

TARGET					= Json.slib
EXTRA_HEADERS			= ParserShiftReduce.tab.hpp location.hh position.hh stack.hh
CLEAN_EXTRA				= location.hh position.hh stack.hh
NOCOVERAGE				= Lexer.lex ParserShiftReduce.tab
FILE_WARNING_FLAGS		+= -Wno-overloaded-virtual

include ${THORSANVIL_ROOT}/build/tools/Makefile
CXXFLAGS				+= -Wno-deprecated-register

%/ParserShiftReduce.tab.o:  FILE_WARNING_FLAGS  += -Wno-parentheses -Wno-unreachable-code
%/Lexer.lex.o:              FILE_WARNING_FLAGS  += -Wno-sign-compare




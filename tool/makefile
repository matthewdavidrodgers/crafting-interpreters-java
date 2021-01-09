PKG = com.craftinginterpreters.tool
CLASSDIR = classes
SRCDIR = src
JCFLAGS = -g -classpath $(CLASSDIR) -sourcepath $(SRCDIR) -d $(CLASSDIR)
JFLAGS = -classpath $(CLASSDIR)
CMP = javac
EXE = java

CLASSES = GenerateAst.java

default:
	$(CMP) $(JCFLAGS) $(addprefix src/,$(CLASSES))

gen:
	$(EXE) $(JFLAGS) $(PKG).GenerateAst ../lox/src

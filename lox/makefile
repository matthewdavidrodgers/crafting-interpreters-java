PKG = com.craftinginterpreters.lox
CLASSDIR = classes
SRCDIR = src
JCFLAGS = -g -classpath $(CLASSDIR) -sourcepath $(SRCDIR) -d $(CLASSDIR)
JFLAGS = -classpath $(CLASSDIR)
CMP = javac
EXE = java

CLASSES = \
	Expr.java \
	Lox.java \
	Parser.java \
	Scanner.java \
	Token.java \
	TokenType.java \
	Environment.java \
	Interpreter.java \
	RuntimeError.java \
	Stmt.java \
	LoxCallable.java \
	LoxFunction.java \
	Return.java \
	Resolver.java

default:
	$(CMP) $(JCFLAGS) $(addprefix src/,$(CLASSES))

repl:
	$(EXE) $(JFLAGS) $(PKG).Lox

file:
	$(EXE) $(JFLAGS) $(PKG).Lox $(PATH)

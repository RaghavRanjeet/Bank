CPP = g++
FLAGS = -O2 -Wall
EXEC = a.exe

SRCPATH = classes
OBJDIR = ../build

CLASSES = \
	Account.o \
	atm.o \
	backup.o \
	bank.o \
	customer_atm.o \
	customer_bank.o \
	log.o \
	manager.o \
	syntax.o \
	verification.o \

FUNCTS = \
	main.o \
	function.o \

OBJECTS = \
	$(addprefix $(OBJDIR)/, $(FUNCTS)) \
	$(addprefix $(OBJDIR)/, $(CLASSES)) \

all: makedir $(OBJECTS) compile touch

# Rules for source files in current directory
$(OBJDIR)/%.o: %.cpp
	$(CPP) $(FLAGS) -c $< -o $@

# Rules for source files in classes/ directory
$(OBJDIR)/%.o: $(SRCPATH)/%.cpp
	$(CPP) $(FLAGS) -c $< -o $@

# Create build directory if it doesn't exist
makedir:
	if not exist $(OBJDIR) mkdir $(OBJDIR)

# Run the executable
run: all
	$(EXEC)

# Clean build artifacts
clean:
	if exist $(OBJDIR) rmdir /s /q $(OBJDIR)
	if exist $(EXEC) del $(EXEC)

# Link all object files
compile:
	$(CPP) $(FLAGS) $(OBJECTS) -o $(EXEC)

# Final message
touch:
	@echo 
	@echo Compilation done successfully.
	@echo 

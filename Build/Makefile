# GNU Make solution makefile autogenerated by Premake
# Type "make help" for usage help

ifndef config
  config=debug
endif
export config

PROJECTS := hiberlite sqlite sample catch_test hiberlite_test

.PHONY: all clean help $(PROJECTS)

all: $(PROJECTS)

hiberlite: 
	@echo "==== Building hiberlite ($(config)) ===="
	@${MAKE} --no-print-directory -C . -f hiberlite.make

sqlite: 
	@echo "==== Building sqlite ($(config)) ===="
	@${MAKE} --no-print-directory -C . -f sqlite.make

sample: hiberlite sqlite
	@echo "==== Building sample ($(config)) ===="
	@${MAKE} --no-print-directory -C . -f sample.make

catch_test: hiberlite sqlite
	@echo "==== Building catch_test ($(config)) ===="
	@${MAKE} --no-print-directory -C . -f catch_test.make

hiberlite_test: hiberlite sqlite
	@echo "==== Building hiberlite_test ($(config)) ===="
	@${MAKE} --no-print-directory -C . -f hiberlite_test.make

clean:
	@${MAKE} --no-print-directory -C . -f hiberlite.make clean
	@${MAKE} --no-print-directory -C . -f sqlite.make clean
	@${MAKE} --no-print-directory -C . -f sample.make clean
	@${MAKE} --no-print-directory -C . -f catch_test.make clean
	@${MAKE} --no-print-directory -C . -f hiberlite_test.make clean

help:
	@echo "Usage: make [config=name] [target]"
	@echo ""
	@echo "CONFIGURATIONS:"
	@echo "   debug"
	@echo "   release"
	@echo "   debug32"
	@echo "   release32"
	@echo "   debug64"
	@echo "   release64"
	@echo ""
	@echo "TARGETS:"
	@echo "   all (default)"
	@echo "   clean"
	@echo "   hiberlite"
	@echo "   sqlite"
	@echo "   sample"
	@echo "   catch_test"
	@echo "   hiberlite_test"
	@echo ""
	@echo "For more information, see http://industriousone.com/premake/quick-start"

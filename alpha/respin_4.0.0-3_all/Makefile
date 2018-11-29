export SHELL = sh
PACKAGE = respin
VERSION = 4.0.0-2
COPYRIGHTYEAR = 2018
AUTHOR = marcia wilbur
EMAIL = contact@linuxrespin.org

all: debian

debian: 
	[ ! -d ./build/debian/ ] || rm -r ./build/debian/
	mkdir -p ./build/debian/
	mkdir -p ./dist
	
	cp -r src/* ./build/debian/
	
	./tools/debian-package.sh "$(PACKAGE)" "$(VERSION)" "$(AUTHOR)" "$(EMAIL)" "all"


clean:
	rm -rf dist
	rm -rf build


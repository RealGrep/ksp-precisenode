all: build install

build:
	xbuild PreciseNode.csproj
clean:
	-rm -rf obj
	-rm -rf bin

package:
	-rm ~/PreciseNode.zip
	(cd Output; zip -r ~/PreciseNode.zip *)

install:
	-mkdir -p Output/GameData/PreciseNode/Plugins
	cp CHANGES.txt ./Output/GameData/PreciseNode/
	cp LICENSE.txt ./Output/GameData/PreciseNode/
	cp PreciseNode.version ./Output/GameData/PreciseNode/
	cp ./bin/Debug/PreciseNode.dll ./Output/GameData/PreciseNode/Plugins/

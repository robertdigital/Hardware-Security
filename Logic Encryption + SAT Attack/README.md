# Hardware-Security

## Requirements to Install the Tool
		Ubuntu 14.04.04 or 14.04.05 
	Flex: sudo apt-get install flex
	Bison: sudo apt-get install bison
	G++: sudo apt-get install g++
	CPLEX: http://www-01.ibm.com/support/docview.wss?uid=swg21444285

## Logic Encryption and SAT Attack Tool Install
		Download the TAR file
		Unzip the tar file: tar -zxvf logic_enc_tool.tar.gz
		Go to the unzipped folder/logic_encyption/source/src folder
		Update line 54 of makefile with the absolute path
				
		change to the makefile folder (cd  $UNZIP_FOLDER/logic_encyption/source/src)
		execute command: make all
		
## Usage
		All executables are Found in $UNZIP_FOLDER/logic_encyption/source/src/ folder
		Logic Encryption: ./sle ../../benchmarks/original/c880.bench ../../benchmarks/rnd/c880_enc50.bench
		Logic Decryption: ./sld ../../benchmarks/rnd/c880_enc50.bench ../../benchmarks/original/c880.bench

## Understanding and Using SAT TOOL: 		
		1. Learning how SAT works
		2. Using SAT tool - pycosat https://pypi.python.org/pypi/pycosat
		3. Parsing the ouput of SAT sovler and re-using parts of the output. 
		
## NOTE
		Tool based on :https://bitbucket.org/spramod/host15-logic-encryption
		WARNING: DO NOT CLONE THAT REPO AND INSTALL. THE REPO MIGHT NOT BUILD PROPERLY
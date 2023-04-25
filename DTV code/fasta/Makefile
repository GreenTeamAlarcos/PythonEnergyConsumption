compile:
	python3 -m py_compile fasta.python3-3.py
	python3 -m py_compile fasta-d.python3-3.py
	chmod 777 __pycache__/fasta.python3-3.cpython-38.pyc
	chmod 777 __pycache__/fasta-d.python3-3.cpython-38.pyc
	
measure:
	sudo modprobe msr
	sudo ../../RAPL/main "python3 -OO fasta.python3-3.py 25000000" Python fasta

run:
	python3 -OO fasta.python3-3.py 25000000	
run-compiled:
	./__pycache__/fasta.python3-3.cpython-38.pyc 25000000
run-d:
	python3 -OO fasta-d.python3-3.py 25000000
run-compiled-d:
	./__pycache__/fasta-d.python3-3.cpython-38.pyc 25000000

make mem:
	/usr/bin/time -v  /usr/local/src/Python-3.6.1/bin/python3.6 -OO fasta.python3-3.py 25000000

compile:
	python3 -m py_compile binarytrees.py
	chmod 777 __pycache__/binarytrees.cpython-38.pyc
measure:
	sudo modprobe msr
	sudo ../../RAPL/main "/usr/local/src/Python-3.6.1/bin/python3.6 -OO binarytrees.py 21" Python binary-trees

run:
	python3 -OO binarytrees.py 21
run-compiled:
	./__pycache__/binarytrees.cpython-38.pyc 21

mem:
	/usr/bin/time -v /usr/local/src/Python-3.6.1/bin/python3.6 -OO binarytrees.py 21

compile:
	python3 -m py_compile fannkuchredux.python3-4.py
	chmod 777 __pycache__/fannkuchredux.python3-4.cpython-38.pyc
measure:
	sudo modprobe msr
	sudo ../../RAPL/main "/usr/local/src/Python-3.6.1/bin/python3.6 -OO fannkuchredux.python3-4.py 12" Python fannkuch-redux

run:
	python3 -OO fannkuchredux.python3-4.py 12
run-compiled:
	./__pycache__/fannkuchredux.python3-4.cpython-38.pyc 12
mem:
	/usr/bin/time -v /usr/local/src/Python-3.6.1/bin/python3.6 -OO fannkuchredux.python3-4.py 12

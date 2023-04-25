compile:
	python3 -m py_compile regexredux.py
	chmod 777 __pycache__/regexredux.cpython-38.pyc
measure:
	sudo modprobe msr
	sudo ../../RAPL/main "/usr/local/src/Python-3.6.1/bin/python3.6 -OO regexredux.py 0 < ../../regexredux-input5000000.txt" Python regex-redux

run:
	python3 -OO regexredux.py 0 < ../../regexredux-input5000000.txt
run-compiled:
	./__pycache__/regexredux.cpython-38.pyc 0 < ../../regexredux-input5000000.txt

mem:
	/usr/bin/time -v /usr/local/src/Python-3.6.1/bin/python3.6 -OO regexredux.py 0 < ../../regexredux-input5000000.txt

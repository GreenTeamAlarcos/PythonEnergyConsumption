compile:
	python3 -m py_compile spectralnorm.python3-5.py
	python3 -m py_compile spectralnorm-d.python3-5.py
	chmod 777 __pycache__/spectralnorm.python3-5.cpython-38.pyc
	chmod 777 __pycache__/spectralnorm-d.python3-5.cpython-38.pyc

measure:
	sudo modprobe msr
	sudo ../../RAPL/main "/usr/local/src/Python-3.6.1/bin/python3.6 -OO spectralnorm.python3-5.py 5500" Python spectral-norm

run:
	python3 -OO spectralnorm.python3-5.py 5500
run-compiled:
	./__pycache__/spectralnorm.python3-5.cpython-38.pyc 5500
run-d:
	python3 -OO spectralnorm-d.python3-5.py 5500
run-compiled-d:
	./__pycache__/spectralnorm-d.python3-5.cpython-38.pyc 5500

mem:
	/usr/bin/time -v /usr/local/src/Python-3.6.1/bin/python3.6 -OO spectralnorm.python3-5.py 5500

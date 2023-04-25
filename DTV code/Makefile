compile:
	python3 -m py_compile mandelbrot.python3-7.py
	python3 -m py_compile mandelbrot-d.python3-7.py
	chmod 777 __pycache__/mandelbrot.python3-7.cpython-38.pyc
	chmod 777 __pycache__/mandelbrot-d.python3-7.cpython-38.pyc
measure:
	sudo modprobe msr
	sudo ../../RAPL/main "/usr/local/src/Python-3.6.1/bin/python3.6 -OO mandelbrot.python3-7.py 16000" Python mandelbrot

run:
	python3 -OO mandelbrot.python3-7.py 16000
run-compiled:
	./__pycache__/mandelbrot.python3-7.cpython-38.pyc 16000
run-d:
	python3 -OO mandelbrot-d.python3-7.py 16000
run-compiled-d:
	./__pycache__/mandelbrot-d.python3-7.cpython-38.pyc 16000

mem:
	/usr/bin/time -v /usr/local/src/Python-3.6.1/bin/python3.6 -OO mandelbrot.python3-7.py 16000

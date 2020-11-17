now:
	python3 minimax.py

oo:
	python3 oominimax.py

tests:
	make t1
	make t2
	make t3
	make t4

t1:
	make dotest NUM=1

t2:
	make dotest NUM=2

t3:
	make dotest NUM=3

t4:
	make fuckthis 

dotest:
	python3 minimax.py < input.$(NUM) > output.$(NUM)
	diff output.$(NUM) output.$(NUM).correct
	cksum output.$(NUM)
	cksum output.$(NUM).correct

fuckthis:
	python3 oominimax.py < input.1

clean:
	-rm output.?

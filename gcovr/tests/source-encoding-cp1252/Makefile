all:
	$(CXX) -fprofile-arcs -ftest-coverage -fPIC --encoding cp1252 main.cpp -o testcase

run: txt xml html

txt:
	# pass

xml:
	# pass

html:
	./testcase
	$(GCOVR) -d --html-details -o coverage.html --source-encoding cp1252

clean:
	rm -f testcase
	rm -f *.gc*
	rm -f coverage*.html

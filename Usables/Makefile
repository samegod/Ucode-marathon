all: copy part_of_the_matrix little_clean clean
copy:
	mkdir obj
	cp inc/*.h obj/
	cp src/*.c obj/
part_of_the_matrix: object.o
object.o:
	clang -std=c11 -Wall -Wextra -Werror -Wpedantic -o part_of_the_matrix obj/*.c
little_clean:
	rm -rf obj
clean:
	rm -rf obj
	rm -rf *.h
	rm -rf *.c
uninstall: clean
	rm -rf part_of_the_matrix
reinstall: uninstall clean all 
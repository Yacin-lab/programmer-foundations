Subject
---
		Assignment name : join_with_separator 
		Expected files : join_with_separator.c 
		Allowed functions: write 
		---------------------------------------------
		Write a program that takes multiple arguments and a separator (first arg is separator) and prints
		all following args joined by the separator, then newline.
		---------------------------------------------
		$> ./join_with_separator ':' a b c | cat -e 
		a:b:c$
		$> ./join_with_separator '(::)' hello world again | cat -e
		hello(::)world(::)again$
		$> ./join_with_separator | cat -e
		$

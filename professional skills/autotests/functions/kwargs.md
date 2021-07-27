def foo(**kwargs):
	pass
	
Способ передать неограниченное количество именованных аргументов.

В отличии от [[args]], нужно как-то передавать имена внутрь функции в конкретное место, поэтому kwargs имеет специальный метод:

def foo(**kwargs):
	print(kwargs.get('name_arg')+kwargs.get('name_arg2'))
foo(name_arg='one',name_arg2='two')

[[Именные аргументы]]

#python #functions
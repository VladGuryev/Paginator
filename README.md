This repo contains the header paginator.h in which the template class Paginator<Iterator> is 
implemented. The generating func for that class is also realized. The main idea of the issue is
to create a class which would be able to split object into Pages (another template class) of the
certain size. For example, we have 100 objects and want to split them into pages and every page
should contain, for instance, 23 object. The Paginator do all the work. The Paginator<Iterator>
supports range-based for, as well as Page<Iterator>.
The Paginator<Iterator> contains the vector of Page<Iterator>. Of course, there is
no any copying, work only with iterators. It should be noted that the C++14 standard was used 
therefore there is no auto in return types of methods due to impossibility of my C++14 compiler
to deduce types from initializer list. 

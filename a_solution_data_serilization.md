A Solution for Data Serialization

Now I'm working in a company which's name I can't tell.

This company has so many problems about programming, but I can't do anything for this situation, because I'm a little programmer who is sent in this company to help the employees in it to finish job.

But one thing I can do is doing my work well. 

I can't leak the information of this company, so I just give some example about serialization in it.

Suppose we have a struture like this:

```C++
struct Person
{
	char* name[20];
	int;
};
```
	
Boss asks the structure to tranlate to another network, like something I can't tell you. before senting it, they must serialize it.

Most of people in this company use 'memcpy' to copy it, but as CPPer, I don't think that is good idea. I prefrer using vector<unsigned char> and the function copy instead. and overload the 'operator+'
to replace memory functions 'alloc', 'memcpy', 'memset', they are unsafe and dangerous.

# cplusbar
A super simple, light, header-only, C++ progress bar.
Inspider by [gipert's progress bar](https://github.com/gipert/progressbar). Just use it as below:
```c++
#include "ProgressBar.hpp"

int main(int argc, char const ** argv){
	int iterations = 1000000000;
	ProgressBar bar(iterations);
	while(iterations > 0){
		bar.update();
		iterations--;
	}
	bar.finish();
	return 0;
}
```
That would output the following:
```console
[#########-----------------------------------------]  19%
```
You can change static members of the class for some customization.
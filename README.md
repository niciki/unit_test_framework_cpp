# unit_test_framework_cpp
Simple unit test framework on C++ <br/>
For using the framework, you need to create some function, for example, in my example it is called `Testing`. In it, we create an instance of the `Tests` class. We describe several functions in which we perform some calculations, each of which ends with a call to the `Assert` function (not from the C ++ standard library!), Into which three arguments are passed: value 1, value 2, and a comment to determine if it fails which of the unit tests failed. After describing all the functions, in the `Testing` function we call the `Run_test` method, where our functions and a string containing the name of this function are passed. Further, at the very beginning of the execution of our program, you need to call the `Run_test` function
<br/>
All information about pass / fail is contained in stderr, program execution is terminated if at least one test fails <br/>
Example execution for a `test_prog.cpp`:
![изображение](https://user-images.githubusercontent.com/71276784/147965341-6c455c23-19c8-4d57-b40c-e965e6fe4f0f.png)

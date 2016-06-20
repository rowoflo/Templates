# ___project_name___
Short description here...

## Building

From project root directory
```
>> mkdir build
>> cd build
>> cmake ..
>> make
```
Use `make -j<number of concurrent jobs>` for multicore builds. i.e. make -j8 will fully utilize a 8 core processor.
Using more than -j2 on a VM can sometimes cause RAM exaustion.

## Running

From `build` directory
```
>> make run
```
or


## Run test

From `build` directory
```
>> make test
```
or
```
>> make check
```
or
```
>> test/testfoo/testfoo
```

## Generate coverage report

From `build` directory
```
>> cmake -DENABLE_COVERAGE=on ..
>> make coverage
```
View detailed coverage report at `./build/coverage_report/index.html`

## Generate Doxygen files

From 'build' directory
```
>> make doc
``
or
```
>> doxygen ..
```
View detailed coverage report at `./build/doc...`


## Installing

From `build` directory
```
>> make install
```
By default binaries are install into `/usr/local/bin`. To specify a different installation location do
```
>> make DESTDIR={/desired/path} install
```
The default install directory prefix is `/usr/local`. To change the prefix set the `CMAKE_INSTALL_PREFIX` in the CMakeLists.txt file.

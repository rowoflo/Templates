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
>> cmake -DBUILD_TYPE=test ..
>> make test
```
or
```
>> make check
```
or
```
>> ./test/___project_name____test
```

## Generate coverage report

From `build` directory
```
>> cmake -DCMAKE_BUILD_TYPE=test ..
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

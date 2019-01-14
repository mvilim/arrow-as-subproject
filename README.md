This project demonstrates an issue with using Arrow as a CMake subproject.

# Clone recurisvely

```
git clone --recursive https://github.com/mvilim/arrow-as-subproject.git
```

# Test building with old paths
```
mkdir -p build; cd build; cmake ..; make
```

Build should fail.

# Test building patch

```
git apply patch.diff --directory arrow                
mkdir -p build; cd build; cmake ..; make
```

Build should succeed.

# base repository for BabbleSim 

BabbleSim base/common components. Any BabbleSim user will want some of these.

The BabbleSim project consists of many components, most of them optional and each in its own separate git repository.
In this Fork those extenal components are included as git submodules so the [Android Repo](https://source.android.com/setup/develop/repo)
is no longer needed.

## Fetching BabbleSim
with this repository BubbleSim can be fetched by using git alone:
```
mkdir ~/bsim/ && cd ~/bsim/
git clone --recurse-submodules https://github.com/sittkuma/base.git components
ln -s ./components/common/Makefile Makefile
```
and build with:
```
make everything -j 8
```
the rest should be the same as the [BabbleSim Doku](https://babblesim.github.io/)

What is this project ?
----------------------

This project is **NOT** the official opencv repository.

It is a fork of opencv sources hosted at https://github.com/opencv/opencv.

It is used as staging area to maintain and test patches that may be contributed back to the
official repository.


What is the branch naming convention ?
--------------------------------------

Each branch is named following the pattern `slicer-X.Y.Z-YYYY.MM.DD-SHA{N}`

where:

* `X.Y.Z` is the version of the forked project
* `YYYY.MM.DD` is the date of the last official commit associated with the branch.
* `SHA{N}` are the first N characters of the last official commit associated with the branch.

How to update the version of tclap ?
------------------------------------

1. Clone this repository and add a remote to the official project

```
git clone git://github.com/slicer/opencv
cd opencv
git remote add upstream git@github.com:opencv/opencv
git fetch upstream
```

2. Create a new branch following the convention `slicer-X.Y.Z-YYYY.MM.DD-SHA{N}`

3. Cherry-pick the Slicer specific commits from last branch. Resolve conflict as needed.

4. Test the changes

5. Publish the branch. (directly in this repo if you have push rights, or on a fork)

How to be granted push rights ?
-------------------------------

Ask on https://discourse.slicer.org/


Questions
---------

If you have questions, see https://discourse.slicer.org/

# 99bottles_python

99 Bottles of OOP examples in Python 3.

* To spend 30 minutes on your own solution, following [Appendix B](https://www.sandimetz.com/99bottles/sample#appendix-exercise), clone the repo.

* `lib/bottles.py` is an empty placeholder file waiting for your solution.

* `test/bottles_test.py` is the equivalent of [the initial test suite in Ruby](https://github.com/sandimetz/99bottles/blob/b-exercise/test/bottles_test.rb) included in the [`b-exercise` branch in the book's repo](https://github.com/sandimetz/99bottles/tree/b-exercise).

* A proper run of the suite with an empty `lib/bottles.py` file should return:

```bash
$ cat lib/bottles.py
$ python3.6 test/bottles_test.py
Traceback (most recent call last):
  File "test/bottles_test.py", line 10, in <module>
    from lib.bottles import Bottles
ImportError: cannot import name 'Bottles'
```


* If you only put an empty `Bottles` class in this file, the same command would return valid `unittest` output like this:

```bash
$ cat lib/bottles.py
class Bottles(object):
    pass

$ python3.6 test/bottles_test.py
sssEssss
======================================================================
ERROR: test_the_first_verse (__main__.BottlesTest)
----------------------------------------------------------------------
Traceback (most recent call last):
  File "test/bottles_test.py", line 20, in test_the_first_verse
    assert expected == Bottles().verse(99)
AttributeError: 'Bottles' object has no attribute 'verse'

----------------------------------------------------------------------
Ran 8 tests in 0.001s

FAILED (errors=1, skipped=7)
```

### Happy Hacking!

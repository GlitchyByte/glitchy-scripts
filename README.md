# Misc scripts

Final scripts are in the `scripts` directory. Get them from there!

## tinytoken
![Version](https://img.shields.io/badge/Version-1.0.1-blue)

`tinytoken` is a bash script to generate a humanly readable token. Unique every second, as long as it's used with the same salt. Useful to create watchers or scripts that check for change.

    ./tinytoken MY_SALT

To use, copy `tinytoken` script directly into your solution and call it from your build scripts as needed. The file is small enough to be committed as part of your solution.

```bash
# You can output to a file:
./tinytoken MY_SALT > build-code.txt

# Or assign it to a variable:
my_var=$(./tinytoken MY_SALT)
```

## checkfix
![Version](https://img.shields.io/badge/Version-1.1.0-blue)

`checkfix` is a bash script to report `TODO` and `FIXME` comments in your code.

    ./checkfix src

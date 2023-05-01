---
description: >-
  In this article, I will explain and demonstrate why the incorrect use of the
  "touch" command can harm and take unnecessary time in your processes on Linux
---

# 📜 Why you shouldn't use "touch" to create empty files in Linux

### Correct usage of "touch" command

When it comes to creating empty files in Linux, many users default to using the `touch` command. However, it's important to note that the main function of the `touch` command is to modify the time-stamp of existing files. While it can also create a new file if it doesn't already exist, it's not the most efficient method for creating empty files.

Instead, Linux users can utilize the `>` operator in combination with `:` to create empty files quickly and easily while avoiding potential errors. The `:` command does nothing and exits successfully, and when used in combination with `>`, it redirects the standard output of `:` to create an empty file with the specified name.

For example, to create a new empty file called "_myfile.txt_", simply type the following command:

```bash
:> myfile.txt
```

This will create a new file called "_myfile.txt_" in the current directory, without the need for a separate command like `touch`. Using the `>` operator in combination with `:` to create empty files is not only more efficient than using `touch`, but it also avoids potential errors that may occur when using `touch` to create files.

### Benchmark

Sure, it's time for the tests, let's make a simple comparison using the <mark style="color:blue;">`time`</mark> command to calculate the execution time between the **touch** command and the _shell director_ when creating empty files.

In this test, we are going to set up a for loop to create **300** empty files, in the two ways mentioned above.

```bash
# Creating 300 empty files with touch command
for i in {1..300}; do
{
    touch file.txt
}

# Creating 300 empty files with ">" redirection
for i in {1..300}; do
{
    :> file.txt
}

```

We separate the codes without different scripts, run with the `time` prefix, and...

<figure><img src="../.gitbook/assets/image (6).png" alt=""><figcaption><p>Benchmark test</p></figcaption></figure>

Exactly, the loop using `:>` operated 30 times faster than the one using `touch`.

### Conclusion

Okay, now you know that the `touch` command isn't performant enough to create empty files on Linux, but obviously, it won't make any difference in your **day-to-day** operations, but it's worth knowing that you're using it erroneous, anyway, use `touch` command only to modify **time-stamps**, use it correctly :)

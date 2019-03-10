# setdue
This is a todo.txt-cli extension to set or change the due date of a set of tasks

Listed in the [todo.txt-cli addon directory][1].

## Usage:

    todo setdue DUEDATE ITEM# ...

## Parameter conditions: 
 * `DUEDATE` must be a supported date format
 * `ITEM#` must be an integer, several items can be specified separated by spaces

### Supported date formats

| Format       | Description                                                   |
| ---:         | :---                                                          |
| `yyyy-mm-dd` | is the standard\* date format                                 |
| `--mm-dd`    | is the standard\* date format in the current year             |
| `---dd`      | is a date format in the current month and year                |
| `yyyy-Www`   | is the standard\* week reference                              |
| `--Www`      | is a week reference in the current year                       |
| `yyyy-Www-D` | is the standard\* week reference with ordinal week day        |
| `--Www-D`    | is a week reference with ordinal week day in the current year |
| `yyyy-ddd`   | is the standard\* ordinal date                                |
| `--ddd`      | is an ordinal date reference in the current year              |
| `-ddd`       | stands for `ddd` days ago                                     |
| `+ddd`       | stands for `ddd` days starting now                            |
| `today`      | sets due to today                                             |
| `nw`         | stands for next week (this weekday in next week)              |
| `xxx`        | (where `xxx` are the first three letters in a weekday name) is a reference to the next such weekday |

\* according to ISO 8601

[1]:https://github.com/todotxt/todo.txt-cli/wiki/Todo.sh-Add-on-Directory

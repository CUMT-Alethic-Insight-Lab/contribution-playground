# Task 02 — Add a Test / 补一个测试

Write tests for a small sample function and prove they pass.

为一个小型示例函数编写测试,并证明测试通过。

## Goal — 目标

Practice writing meaningful test cases (normal input, edge cases, failure cases) and running them locally.

练习编写有意义的测试用例(正常输入、边界情况、异常情况),并在本地运行通过。

## The Sample Function — 示例函数

```python
def normalize_title(text: str) -> str:
    """Collapse whitespace and capitalize each word.

    >>> normalize_title("  hello   world ")
    'Hello World'
    """
    if not isinstance(text, str):
        raise TypeError("text must be a string")
    return " ".join(text.split()).title()
```

## Steps — 步骤

1. Create a branch named like `test/normalize-title-<your-github-id>`.

   新建分支,命名为 `test/normalize-title-<你的 GitHub ID>` 之类的形式。

2. Create a directory `samples/<your-github-id>/` and put the function above into `normalize_title.py` inside it.

   新建目录 `samples/<你的 GitHub ID>/`,把上面的函数放进该目录下的 `normalize_title.py`。

3. Add `test_normalize_title.py` in the same directory. Cover at least:

   在同一目录添加 `test_normalize_title.py`,至少覆盖:

   | Case | 用例 |
   | --- | --- |
   | Normal input with extra spaces | 含多余空白的正常输入 |
   | Empty string and whitespace-only string | 空字符串与纯空白字符串 |
   | Non-string input raising `TypeError` | 非字符串输入抛出 `TypeError` |
   | One edge case you choose yourself | 一个你自选的边界用例 |

4. Run the tests locally and make sure they pass:

   在本地运行测试并确认通过:

   ```bash
   python -m pytest samples/<your-github-id>/
   ```

   (`unittest` is fine too if you prefer the standard library.)
   (如果你更习惯标准库,用 `unittest` 也可以。)

5. Commit and open a PR. In the description, paste the test command and its result summary.

   提交并发起 PR。在描述中粘贴测试命令与结果摘要。

## Done When — 完成标准

| Check | 检查项 |
| --- | --- |
| Your files live under `samples/<your-github-id>/` only | 文件只放在你自己的 `samples/<ID>/` 目录下 |
| At least four test cases including edge/failure cases | 至少四个用例,含边界与异常情况 |
| Tests pass locally; result shown in PR description | 本地测试通过,结果写入 PR 描述 |
| PR is merged after review | 评审通过后合并 |

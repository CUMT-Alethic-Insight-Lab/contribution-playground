# Task 03 — Review Others / 评审他人 PR

Review someone else's open Pull Request and leave a useful review.

评审其他人处于打开状态的 Pull Request,并留下有价值的评审意见。

## Goal — 目标

Practice the reviewer side of the workflow: reading diffs, checking claims, and giving constructive feedback.

练习协作流程中评审者一侧的工作:阅读 diff、核实描述、给出建设性反馈。

## Steps — 步骤

1. Open the [Pull Requests list](../../pulls) and pick an open PR that is not yours and not yet reviewed.

   打开 [PR 列表](../../pulls),挑一个不是你自己发起、且尚未被评审的打开状态的 PR。

2. Read the PR description first, then the full diff. For each change, ask:

   先读 PR 描述,再看完整 diff。针对每一处改动,问自己:

   | Question | 问题 |
   | --- | --- |
   | Does the diff match what the description claims? | diff 是否与描述一致? |
   | Is the change minimal and focused? | 改动是否最小且聚焦? |
   | For test PRs: do the tests actually cover the stated cases? | 对测试类 PR:测试是否真的覆盖了声称的用例? |
   | Anything sensitive (personal data, credentials) accidentally included? | 是否误带了敏感内容(个人数据、密钥等)? |

3. If the PR includes code, pull the branch locally and run the tests yourself when practical.

   如果 PR 含代码,条件允许时在本地拉取分支并亲自运行测试。

4. Leave a review using GitHub's review feature (Comment / Approve / Request changes). A good review:

   使用 GitHub 的评审功能(Comment / Approve / Request changes)提交评审。好的评审应当:

   | Quality | 要求 |
   | --- | --- |
   | Specific — points to exact lines or cases | 具体——指到具体行或用例 |
   | Constructive — suggests how to improve, not just what is wrong | 建设性——给出改进建议,而非只指出问题 |
   | Honest — request changes when something is actually wrong | 诚实——确实有问题时敢于 Request changes |

5. Follow up: reply if the author responds, and re-review after they update the PR.

   跟进:作者回复后继续交流,作者更新 PR 后再次评审。

## Done When — 完成标准

| Check | 检查项 |
| --- | --- |
| Review submitted via GitHub's review feature | 通过 GitHub 评审功能提交 |
| At least one concrete observation (not just "LGTM") | 至少一条具体意见(不能只有 "LGTM") |
| Tone is respectful and constructive | 语气尊重且有建设性 |

## Notes — 说明

No open PRs right now? Finish Task 01 or 02 first, then review the next person's PR when one appears. You can also pair up with another new member and review each other.

暂时没有打开中的 PR?先完成任务 01 或 02,等下一个 PR 出现时再评审。也可以和另一位新成员结对互评。

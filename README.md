# LangBot CLA Signatures

This repository stores the Contributor License Agreement (CLA) signature records for all repositories in the [langbot-app](https://github.com/langbot-app) organization.

本仓库存储 [langbot-app](https://github.com/langbot-app) 组织下所有仓库的贡献者许可协议（CLA）签署记录。

## How it works / 工作方式

- The CLA text lives in the main repository: [langbot-app/LangBot/CLA.md](https://github.com/langbot-app/LangBot/blob/master/CLA.md)
- When a contributor opens their first pull request in any participating repository, the CLA Assistant workflow prompts them to sign by replying with a designated comment. The signature record is then automatically appended to `signatures/version1/cla.json` in this repository.
- One signature covers all repositories in the organization, for present and future contributions.

- CLA 全文位于主仓库：[langbot-app/LangBot/CLA.md](https://github.com/langbot-app/LangBot/blob/master/CLA.md)
- 贡献者首次在组织内任一接入仓库提交 PR 时，CLA Assistant 工作流会提示其回复指定评论完成签署，签署记录将自动追加到本仓库的 `signatures/version1/cla.json`。
- 一次签署对组织内全部仓库的现在与未来贡献永久有效。

## Signature record format / 签署记录格式

Each record contains the signer's GitHub username, immutable numeric account ID, the ID of the signing comment, a timestamp, and the pull request number — together with this repository's git history, forming a verifiable audit trail.

每条记录包含签署者的 GitHub 用户名、不可变的数字账号 ID、签署评论 ID、时间戳和 PR 编号，配合本仓库的 git 历史构成可验证的审计链。

## Maintenance notes / 维护注意事项

- **Do not edit `signatures/` manually.** Records are appended by the workflow only. (Exception: importing Corporate CLA employee records, which maintainers add following the documented schema.)
- **Do not enable branch protection on `main`.** The workflow pushes signature commits directly to this branch.
- The signature file is created automatically by the workflow upon the first signature — do not pre-create it.

- **请勿手工编辑 `signatures/` 目录**，记录仅由工作流自动追加（例外：导入企业 CLA 员工记录时由维护者按既定 schema 手工添加）。
- **请勿对 `main` 分支开启分支保护**，工作流需要直接向该分支推送签署记录。
- 签名文件由工作流在首次签署时自动创建，请勿预先创建。

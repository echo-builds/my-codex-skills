# Cross-Device Install Prompt

Copy this prompt to another computer's Codex:

```text
请帮我从 GitHub 私有仓库 https://github.com/xufeng-code/my-codex-skills 同步我的个人 Codex Skills 到这台电脑。

我的长期源仓库是：
https://github.com/xufeng-code/my-codex-skills

请做这些事：
1. 检查你是否能访问这个 GitHub 仓库；如果需要授权，请引导我完成 GitHub 授权。
2. 查看仓库中的插件和 skills，尤其是：
   - product-demand-design
   - luojing-prd-review
   - zijun-prd-style
   - pyramid-communication
   - skill-sync-workflow
3. 把这些 skills 安装或同步到本机 Codex 可调用目录：
   ~/.codex/skills/<skill-name>/
4. 确保 skill-sync-workflow 也安装到本机。以后当我说“更新这个 skill / 同步 skill / 推到 GitHub”时，你要按这个 workflow 同时更新本机可调用版本和 GitHub 仓库 xufeng-code/my-codex-skills。
5. 完成后告诉我：本机安装了哪些 skills、每个 skill 的本地路径、对应 GitHub 路径，以及是否需要新建任务才能加载最新版 skill 列表。

注意：不要把公司会议原文、token、敏感文档链接或原始逐字稿同步到 GitHub，除非我明确要求。默认只同步抽象后的方法论和可复用技能说明。
```
